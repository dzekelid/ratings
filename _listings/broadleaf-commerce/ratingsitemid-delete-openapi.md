---
swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 0
info:
  title: Broadleaf Commerce API Delete Ratings
  description: Delete ratings.
  version: 1.0.0
host: demo.broadleafcommerce.org
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ratings/{itemId}:
    get:
      summary: Get Ratings
      description: Get ratings.
      operationId: getRatingsItem
      x-api-path-slug: ratingsitemid-get
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    head:
      summary: Head Ratings
      description: Head ratings.
      operationId: headRatingsItem
      x-api-path-slug: ratingsitemid-head
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Head
      - Ratings
    post:
      summary: Post Ratings
      description: Post ratings.
      operationId: postRatingsItem
      x-api-path-slug: ratingsitemid-post
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    put:
      summary: Put Ratings
      description: Put ratings.
      operationId: putRatingsItem
      x-api-path-slug: ratingsitemid-put
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
      - Ratings
    delete:
      summary: Delete Ratings
      description: Delete ratings.
      operationId: deleteRatingsItem
      x-api-path-slug: ratingsitemid-delete
      parameters:
      - in: path
        name: itemId
        description: itemId
      - in: query
        name: ratingType
        description: ratingType
      responses:
        200:
          description: OK
      tags:
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