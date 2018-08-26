---
swagger: "2.0"
x-collection-name: MockLab
x-complete: 1
info:
  title: WireMock
  version: 1.0.0
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
  /scenarios/reset:
    post:
      summary: Post Scenarios Reset
      description: Reset the state of all scenarios
      operationId: postScenariosReset
      x-api-path-slug: scenariosreset-post
      responses:
        200:
          description: Successful response
      tags:
      - Scenarios
      - Reset
---