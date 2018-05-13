---
swagger: "2.0"
info:
  title: Checks API Checks
  description: Gets a list of all checks that are visible to you as a user or a customer
    depending on the request context.
  version: 1.0.0
host: api.pingdom.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  '/checks ':
    get:
      summary: Checks
      description: "\r\n\t\t\t\tGets a list of all checks that are visible to you
        as a user or a customer depending on the request context"
      operationId: -checks-
      responses:
        200:
          description: OK
      tags:
      - checks
definitions: []
x-collection-name: Pingometer
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