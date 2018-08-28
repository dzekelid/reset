---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Post Requests Reset
  version: 1.0.0
  description: Empty the request journal
basePath: /__admin
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mappings/reset:
    post:
      summary: Post Mappings Reset
      description: Reset stub mappings (restore to defaults defined back the backing
        store)
      operationId: postMappingsReset
      x-api-path-slug: mappingsreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Mappings
      - Reset
  /requests/reset:
    post:
      summary: Post Requests Reset
      description: Empty the request journal
      operationId: postRequestsReset
      x-api-path-slug: requestsreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Requests
      - Reset
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