swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 1
info:
  title: plentymarkets REST-API
  description: the-plentymarkets-rest-api-expands-the-functionality-of-the-plentymarkets-cms-and-allows-access-to-resources-i-e--data-records-via-unique-uri-paths
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/feedbacks/ratings:
    get:
      summary: List feedback ratings
      description: Lists feedback ratings.
      operationId: getRestFeedbacksRatings
      x-api-path-slug: restfeedbacksratings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Ratings
  /rest/feedbacks/rating:
    post:
      summary: Create a feedback rating
      description: Creates a feedback rating.
      operationId: postRestFeedbacksRating
      x-api-path-slug: restfeedbacksrating-post
      parameters:
      - in: query
        name: ratingRelationTargetId
        description: The ID of the ratings target
      - in: query
        name: ratingRelationTargetTypeId
        description: The type ID of the ratings target
      - in: query
        name: ratingValue
        description: The feedbacks comment message
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating
  /rest/feedbacks/rating/{ratingId}:
    delete:
      summary: Delete a feedback rating
      description: Deletes a feedback rating. The ID of the feedback rating must be
        specified.
      operationId: deleteRestFeedbacksRatingRating
      x-api-path-slug: restfeedbacksratingratingid-delete
      parameters:
      - in: query
        name: feedbackRatingId
        description: The ID of the feedback rating
      - in: path
        name: ratingId
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating
    get:
      summary: Get a feedback rating
      description: Gets a feedback rating. The ID of the feedback rating must be specified.
      operationId: getRestFeedbacksRatingRating
      x-api-path-slug: restfeedbacksratingratingid-get
      parameters:
      - in: query
        name: feedbackRatingId
        description: The ID of the feedback rating
      - in: path
        name: ratingId
      responses:
        200:
          description: OK
      tags:
      - Feedback
      - Rating