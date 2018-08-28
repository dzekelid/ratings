---
swagger: "2.0"
x-collection-name: Meetup
x-complete: 0
info:
  title: Meetup Event Comment Subscribe
  description: Subscribe to notifications on updates to a given comment thread
  version: 1.0.0
host: api.meetup.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /2/event_comment_subscribe/:id:
    post:
      summary: Event Comment Subscribe
      description: Subscribe to notifications on updates to a given comment thread
      operationId: events
      x-api-path-slug: 2event-comment-subscribeid-post
      responses:
        200:
          description: OK
      tags:
      - Events
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