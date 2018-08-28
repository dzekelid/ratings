swagger: "2.0"
x-collection-name: Instructure
x-complete: 1
info:
  title: Instructure Canvas Utility APIs
  description: canvas-lms-includes-a-rest-api-for-accessing-and-modifying-data-externally-from-the-main-application-in-your-own-programs-and-scripts--
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /courses/{course_id}/discussion_topics/topic_id/entries/{entry_id}/rating:
    post:
      summary: Rate entry
      description: Rate entry.
      operationId: rate-entry
      x-api-path-slug: coursescourse-iddiscussion-topicstopic-identriesentry-idrating-post
      parameters:
      - in: query
        name: rating
        description: A rating to set on this entry
      responses:
        200:
          description: OK
      tags:
      - Courses
      - Course
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Rating
  /groups/{group_id}/discussion_topics/topic_id/entries/{entry_id}/rating:
    post:
      summary: Rate entry
      description: Rate entry.
      operationId: rate-entry
      x-api-path-slug: groupsgroup-iddiscussion-topicstopic-identriesentry-idrating-post
      parameters:
      - in: query
        name: rating
        description: A rating to set on this entry
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Group
      - Id
      - Discussion
      - Topics
      - Topic
      - Id
      - Entries
      - Entry
      - Id
      - Rating