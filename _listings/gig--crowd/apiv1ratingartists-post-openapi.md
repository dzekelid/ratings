---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Rating Artists
  version: 1.0.0
  description: Post rating artists.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/rating/artists:
    post:
      summary: Post Rating Artists
      description: Post rating artists.
      operationId: postApiV1RatingArtists
      x-api-path-slug: apiv1ratingartists-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Rating
      - Artists
  /api/v1/rating/{eventId}/artists:
    get:
      summary: Get Rating Eventid Artists
      description: Get rating eventid artists.
      operationId: getApiV1RatingEventArtists
      x-api-path-slug: apiv1ratingeventidartists-get
      parameters:
      - in: path
        name: eventId
      responses:
        200:
          description: OK
      tags:
      - Rating
      - Eventid
      - Artists
  /api/v1/Rating:
    post:
      summary: Post Rating
      description: Post rating.
      operationId: postApiV1Rating
      x-api-path-slug: apiv1rating-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Rating
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---