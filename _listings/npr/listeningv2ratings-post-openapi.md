---
swagger: "2.0"
x-collection-name: NPR
x-complete: 0
info:
  title: NPR Collect new ratings for media previously recommended to the logged-in
    user
  description: |-
    This endpoint is the main mechanism for providing feedback from the user to NPR about the recommendations that are obtained from `GET /listening/v2/recommendations`.

    A fully-populated link to this endpoint is returned with each individual recommendation and is located in the AudioItemDocument under the `links['recommendations']` object. The query parameters in this link should not be modified.
    Be sure to copy and send back the entire ratings object (RatingData), as new fields may be added to it in the future.

    This endpoint can return a blank JSON.doc or AudioItemDocument depending on the `recommend=true|false` parameter. The `recommend=true` flag allows this endpoint to both receive ratings and send back recommendations in the same call.
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
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---