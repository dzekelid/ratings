---
swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 0
info:
  title: Sustainable Facilities Tool API Building System Rating Systems
  description: Returns all building system rating systems
  termsOfService: https://sftool.gov/developer/terms-of-use
  version: 1.0.0
host: api.data.gov
basePath: /sftool/v1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /building-systems/rating-systems:
    get:
      summary: Building System Rating Systems
      description: Returns all building system rating systems
      operationId: returnBuildingSystemRating
      x-api-path-slug: buildingsystemsratingsystems-get
      responses:
        200:
          description: OK
      tags:
      - Rating Systems
  /building-systems/{parameter}/rating-systems:
    get:
      summary: Building System Rating System
      description: Returns a building system rating system by parameter.
      operationId: returnBuildingSystemRating
      x-api-path-slug: buildingsystemsparameterratingsystems-get
      responses:
        200:
          description: OK
      tags:
      - Rating Systems
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