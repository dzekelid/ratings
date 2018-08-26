---
swagger: "2.0"
x-collection-name: NPR
x-complete: 1
info:
  title: NPR One API Reference
  description: npr-one-is-a-smart-application-that-brings-the-best-of-npr-and-member-station-programming-newscasts-podcasts-and-stories-together-to-create-a-new-experience-for-listening--it-provides-an-editorcurated-and-localized-mobile-listening-experience-based-on-the-content-the-listener-chooses-likes-shares-and-enjoys--the-api-provides-all-of-the-content-and-customization-in-a-simple-structured-way-that-is-easy-for-applicationdevelopers-to-implement-
  termsOfService: http://dev.npr.org/develop/terms-of-use
  contact:
    name: NPR One Enterprise Team
    url: http://dev.npr.org
    email: NPROneEnterprise@npr.org
  version: 1.0.0
host: api.npr.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /listening/v2/ratings:
    post:
      summary: Collect new ratings for media previously recommended to the logged-in
        user
      description: |-
        This endpoint is the main mechanism for providing feedback from the user to NPR about the recommendations that are obtained from `GET /listening/v2/recommendations`.

        A fully-populated link to this endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
        Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.

        This endpoint can return a blank JSON.doc or AudioItemDocument depending on the `recommend=true|false` parameter. The `recommend=true` flag allows this endpoint to both receive ratings and send back recommendations in the same call.
      operationId: postRating
      x-api-path-slug: listeningv2ratings-post
      parameters:
      - in: body
        name: body
        description: A list of RatingData objects which contains data about ratings
          such as the id of the content, the rating value, elapsed time and more
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      - in: query
        name: recommend
        description: If set to `false`, this call will return a blank document; otherwise
          it will return a new recommendation object
      responses:
        200:
          description: OK
      tags:
      - News
      - Listening
      - Ratings
---