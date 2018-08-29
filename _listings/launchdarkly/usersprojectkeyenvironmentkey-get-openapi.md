---
swagger: "2.0"
x-collection-name: LaunchDarkly
x-complete: 0
info:
  title: Launch Darkly List all users in the environment.
  description: List all users in the environment..
  termsOfService: https://launchdarkly.com/terms
  contact:
    name: LaunchDarkly Support
    url: https://support.launchdarkly.com
    email: support@launchdarkly.com
  version: 2.0.0
host: app.launchdarkly.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{projectKey}/{environmentKey}:
    get:
      summary: List all users in the environment.
      description: List all users in the environment..
      operationId: getUsers
      x-api-path-slug: usersprojectkeyenvironmentkey-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Users
      - Projects
      - Keys
      - EnvironmentKey
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