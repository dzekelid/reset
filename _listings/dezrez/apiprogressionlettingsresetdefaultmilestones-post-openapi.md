---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Reset agency default milestones back to global defaults
  version: 1.0.0
  description: Reset agency default milestones back to global defaults.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/progression/lettings/{id}/resetmilestones:
    post:
      summary: Reset tenant role milestones back to agency defaults
      description: Reset tenant role milestones back to agency defaults.
      operationId: LettingsProgression_ResetRoleMilestonesToDefaultByid
      x-api-path-slug: apiprogressionlettingsidresetmilestones-post
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Tenant
      - Role
      - Milestones
      - Back
      - To
      - Agency
      - Defaults
  /api/progression/lettings/resetdefaultmilestones:
    post:
      summary: Reset agency default milestones back to global defaults
      description: Reset agency default milestones back to global defaults.
      operationId: LettingsProgression_ResetMilestonesToDefault
      x-api-path-slug: apiprogressionlettingsresetdefaultmilestones-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Agency
      - Default
      - Milestones
      - Back
      - To
      - Global
      - Defaults
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