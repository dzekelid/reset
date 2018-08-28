---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 0
info:
  title: MockLab Post Mappings Reset
  version: 1.0.0
  description: Reset stub mappings (restore to defaults defined back the backing store)
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