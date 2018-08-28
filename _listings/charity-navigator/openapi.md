swagger: "2.0"
x-collection-name: Charity Navigator
x-complete: 1
info:
  title: CharityNavigatorDataAPI
  description: the-charity-navigator-data-api-provides-access-to-charity-navigatorsratings-research-content-and-charitable-organization-profiles-
  version: 1.0.0
host: api.data.charitynavigator.org
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Organizations/{ein}/Ratings:
    get:
      summary: Get Organizations Ein Ratings
      description: |-
        Retrieve all Charity Navigator ratings for a single organization. <br/>
        ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getRatings
      x-api-path-slug: organizationseinratings-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Ratings
  /Organizations/{ein}/Ratings/{RatingID}:
    get:
      summary: Get Organizations Ein Ratings Rating
      description: |-
        Retrieve a single Rating object for an Organization. Each rating is listed
        once, under its primary `referenceOrganization`. Note that the rating may apply
        to other organizations, and this is represented by `includedOrganizations`,
        which is a collection of hyperlinks to all of the organizations to which the
        rating applies.
        The rating is a point-in-time assessment provided by Charity Navigator, along
        with related metrics and ratios taken from financial statements for a fiscal
        year, on which the rating is based. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getRating
      x-api-path-slug: organizationseinratingsratingid-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ein
      - in: path
        name: RatingID
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Ein
      - Ratings
      - Rating