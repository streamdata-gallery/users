---
swagger: "2.0"
info:
  title: Akamai API Modify a User
  description: Modify a User
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /user-admin/v1/users/{contactId}:
    put:
      summary: Modify a User
      description: Modify a User
      operationId: useradminv1userscontactid
      parameters:
      - in: query
        name: contactId
        description: Unique identifier for a user
        type: string
      responses:
        200:
          description: OK
      tags:
      - user
      - admin
      - users
      - contact
definitions: []
x-collection-name: Akamai
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