---
swagger: "2.0"
info:
  title: Disqus Users ListActivity
  description: Users ListActivity
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/listActivity.json:
    get:
      summary: Users ListActivity
      description: "\n     Users ListActivity "
      operationId: users-listactivity
      parameters:
      - in: query
        name: anon_user
        description: Defaults to null                         Looks up an anonymous
          user by unique hash
        type: string
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: include
        description: 'Defaults to [  user,  replies,  following]                         Choices:
          user, replies, following'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to [  forum,  thread]                         You may
          specify relations to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: user
        description: Defaults to null                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - comments
      - users
definitions: []
x-collection-name: Disqus
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