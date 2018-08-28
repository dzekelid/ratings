---
swagger: "2.0"
x-collection-name: LiveChat
x-complete: 0
info:
  title: LiveChat Chat ratings report
  description: Shows how many chats have been rated and how they have been rated during
    a specified period.
  version: 1.0.0
host: api.livechatinc.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /reports/tickets/ratings:
    get:
      summary: Ticket ratings report
      description: Shows the tickets that were rated during the specified period.
      operationId: ReportsTicketsRatingsGet
      x-api-path-slug: reportsticketsratings-get
      parameters:
      - in: query
        name: date_from
      - in: query
        name: date_to
      - in: query
        name: group
      - in: query
        name: group_by
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Ticket
      - Ratings
      - Report
  /reports/chats/ratings:
    get:
      summary: Chat ratings report
      description: Shows how many chats have been rated and how they have been rated
        during a specified period.
      operationId: ReportsChatsRatingsGet
      x-api-path-slug: reportschatsratings-get
      parameters:
      - in: query
        name: date_from
      - in: query
        name: date_to
      - in: query
        name: group
      - in: query
        name: group_by
      - in: header
        name: X-API-Version
      responses:
        200:
          description: OK
      tags:
      - Chat
      - Ratings
      - Report
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