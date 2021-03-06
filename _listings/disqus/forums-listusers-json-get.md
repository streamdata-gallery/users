---
swagger: "2.0"
info:
  title: Disqus Forums ListUsers
  description: Forums ListUsers
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
  /forums/listUsers.json:
    get:
      summary: Forums ListUsers
      description: "\n     Forums ListUsers "
      operationId: forums-listusers
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      responses:
        200:
          description: OK
      tags:
      - comments
      - forums
      - lists
      - users
definitions: []
x-collection-name: Disqus
x-streamrank:
  polling_total_time_average: "1.94"
  polling_size_download_average: "22625.11"
  streaming_total_time_average: "1.5"
  streaming_size_download_average: "11322.26"
  change_yes: "620"
  change_no: "589"
  time_percentage: "23"
  size_percentage: "50"
  change_percentage: "51"
  last_run: "2018-05-12"
  days_run: "8"
  minute_run: "0"
---