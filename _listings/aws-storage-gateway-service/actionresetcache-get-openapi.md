---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 0
info:
  title: AWS Storage Gateway Service API Reset Cache
  version: 1.0.0
  description: |-
    Resets all cache disks that have encountered a error and makes the disks available
             for reconfiguration as cache storage.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetCache:
    get:
      summary: Reset Cache
      description: |-
        Resets all cache disks that have encountered a error and makes the disks available
                 for reconfiguration as cache storage.
      operationId: resetCache
      x-api-path-slug: actionresetcache-get
      parameters:
      - in: query
        name: GatewayARN
        description: The Amazon Resource Name (ARN) of the gateway
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache
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