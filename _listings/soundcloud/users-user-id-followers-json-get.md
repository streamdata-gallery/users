---
swagger: "2.0"
info:
  title: SoundCloud Get User Followers
  description: Returns a collection of users who follow the user with user id
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/followers.json:
    get:
      summary: Get User Followers
      description: Returns a collection of users who follow the user with user id
      operationId: users.user_id.followers.json.get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - audio
      - users
      - followers
definitions: []
x-collection-name: SoundCloud
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