swagger: "2.0"
x-collection-name: Broadleaf Commerce
x-complete: 1
info:
  title: Broadleaf Commerce API
  description: the-default-broadleaf-commerce-apis
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
    options:
      summary: Options Ratings
      description: Options ratings.
      operationId: optionsRatingsItem
      x-api-path-slug: ratingsitemid-options
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
      - Options
      - Ratings
    patch:
      summary: Patch Ratings
      description: Patch ratings.
      operationId: patchRatingsItem
      x-api-path-slug: ratingsitemid-patch
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