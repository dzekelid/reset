---
swagger: "2.0"
x-collection-name: AWS Storage Gateway Service
x-complete: 1
info:
  title: AWS Storage Gateway Service API
  version: 1.0.0
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
---