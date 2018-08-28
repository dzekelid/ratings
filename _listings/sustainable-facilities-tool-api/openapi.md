swagger: "2.0"
x-collection-name: Sustainable Facilities Tool API
x-complete: 1
info:
  title: Sustainable Facilities Tool API
  description: our-core-api-allows-developers-to-interact-with-the-sustainable-facilities-tool-programmatically--its-designed-for-public-use-and-to-be-easily-integrated-into-other-applications-
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