---
swagger: "2.0"
x-collection-name: The TVDB
x-complete: 0
info:
  title: The TVDB Get User Ratings
  description: Returns an array of ratings for the given user.
  version: 2.1.2
host: api-dev.thetvdb.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user/ratings:
    get:
      summary: Get User Ratings
      description: Returns an array of ratings for the given user.
      operationId: user.ratings.get
      x-api-path-slug: userratings-get
      responses:
        200:
          description: OK
      tags:
      - Television
      - User
      - Ratings
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