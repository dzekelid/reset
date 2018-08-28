---
swagger: "2.0"
x-collection-name: AWS ElastiCache
x-complete: 0
info:
  title: Amazon ElastiCache API Reset Cache Parameter Group
  version: 1.0.0
  description: |-
    Modifies the parameters of a cache
                parameter group to the engine or system default value.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetCacheParameterGroup:
    get:
      summary: Reset Cache Parameter Group
      description: |-
        Modifies the parameters of a cache
                    parameter group to the engine or system default value.
      operationId: resetCacheParameterGroup
      x-api-path-slug: actionresetcacheparametergroup-get
      parameters:
      - in: query
        name: CacheParameterGroupName
        description: The name of the cache parameter group to reset
        type: string
      - in: query
        name: ParameterNameValues.ParameterNameValue.N
        description: An array of parameter names to reset to their default values
        type: string
      - in: query
        name: ResetAllParameters
        description: If true,             all parameters in the cache parameter group
          are reset to their default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cache Parameter Groups
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