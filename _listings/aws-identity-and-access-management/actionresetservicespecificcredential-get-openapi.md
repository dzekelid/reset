---
swagger: "2.0"
x-collection-name: AWS Identity and Access Management
x-complete: 0
info:
  title: AWS Identity and Access Management API Reset Service Specific Credential
  version: 1.0.0
  description: Resets the password for a service-specific credential.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetServiceSpecificCredential:
    get:
      summary: Reset Service Specific Credential
      description: Resets the password for a service-specific credential.
      operationId: resetServiceSpecificCredential
      x-api-path-slug: actionresetservicespecificcredential-get
      parameters:
      - in: query
        name: ServiceSpecificCredentialId
        description: The unique identifier of the service-specific credential
        type: string
      - in: query
        name: UserName
        description: The name of the IAM user associated with the service-specific
          credential
        type: string
      responses:
        200:
          description: OK
      tags:
      - Service Specific Credentials
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