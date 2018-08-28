swagger: "2.0"
x-collection-name: Meetup
x-complete: 1
info:
  title: Meetup
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
  /2/event_rating:
    post:
      summary: Event Rating
      description: This method allows members to posts rating for an event after it's
        occurred. Only permitted for members who rsvp'd yes or maybe to the event
      operationId: events
      x-api-path-slug: 2event-rating-post
      parameters:
      - in: query
        name: attendee_count
        description: 'DEPRECATED: The number of attendees for the event (organizers/assistant
          organizers/co-organizers/event organizers/event hosts only)'
        type: string
      - in: query
        name: event_id
        description: The ID of the event to fetch ratings data for
        type: string
      - in: query
        name: rating
        description: The members rating (either 1, 2, 3, 4, or 5)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Ratings
  /2/event_ratings:
    get:
      summary: Ratings v2
      description: API method for accessing Meetup comments
      operationId: events
      x-api-path-slug: 2event-ratings-get
      parameters:
      - in: query
        name: event_id
        description: The ID of the event to fetch ratings data for
        type: string
      - in: query
        name: member_id
        description: The ID of a member to filter ratings on
        type: string
      responses:
        200:
          description: OK
      tags:
      - Events
      - Groups