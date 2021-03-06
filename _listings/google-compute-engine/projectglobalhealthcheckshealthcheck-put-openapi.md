---
swagger: "2.0"
x-collection-name: Google Compute Engine
x-complete: 0
info:
  title: Google Compute Engine API Update Health Check
  description: Updates a HealthCheck resource in the specified project using the data
    included in the request.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /compute/v1/projects
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{project}/global/healthChecks:
    get:
      summary: Get Health Checks
      description: Retrieves the list of HealthCheck resources available to the specified
        project.
      operationId: compute.healthChecks.list
      x-api-path-slug: projectglobalhealthchecks-get
      parameters:
      - in: query
        name: filter
        description: Sets a filter expression for filtering listed resources, in the
          form filter={expression}
      - in: query
        name: maxResults
        description: The maximum number of results per page that should be returned
      - in: query
        name: orderBy
        description: Sorts list results by a certain order
      - in: query
        name: pageToken
        description: Specifies a page token to use
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
    post:
      summary: Create Health Check
      description: Creates a HealthCheck resource in the specified project using the
        data included in the request.
      operationId: compute.healthChecks.insert
      x-api-path-slug: projectglobalhealthchecks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
  /{project}/global/healthChecks/{healthCheck}:
    delete:
      summary: Delete Health Check
      description: Deletes the specified HealthCheck resource.
      operationId: compute.healthChecks.delete
      x-api-path-slug: projectglobalhealthcheckshealthcheck-delete
      parameters:
      - in: path
        name: healthCheck
        description: Name of the HealthCheck resource to delete
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
    get:
      summary: Get Health Check
      description: Returns the specified HealthCheck resource. Get a list of available
        health checks by making a list() request.
      operationId: compute.healthChecks.get
      x-api-path-slug: projectglobalhealthcheckshealthcheck-get
      parameters:
      - in: path
        name: healthCheck
        description: Name of the HealthCheck resource to return
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
    patch:
      summary: Update Health Check
      description: Updates a HealthCheck resource in the specified project using the
        data included in the request. This method supports patch semantics.
      operationId: compute.healthChecks.patch
      x-api-path-slug: projectglobalhealthcheckshealthcheck-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: healthCheck
        description: Name of the HealthCheck resource to update
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
    put:
      summary: Update Health Check
      description: Updates a HealthCheck resource in the specified project using the
        data included in the request.
      operationId: compute.healthChecks.update
      x-api-path-slug: projectglobalhealthcheckshealthcheck-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: healthCheck
        description: Name of the HealthCheck resource to update
      - in: path
        name: project
        description: Project ID for this request
      responses:
        200:
          description: OK
      tags:
      - Checks
      - Health
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