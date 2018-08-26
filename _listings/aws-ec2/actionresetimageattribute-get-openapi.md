---
swagger: "2.0"
x-collection-name: AWS EC2
x-complete: 0
info:
  title: AWS EC2 API Reset Image Attribute
  version: 1.0.0
  description: Resets an attribute of an AMI to its default value.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetImageAttribute:
    get:
      summary: Reset Image Attribute
      description: Resets an attribute of an AMI to its default value.
      operationId: resetimageattribute
      x-api-path-slug: actionresetimageattribute-get
      parameters:
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the      request, and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: ProductCode
        description: The product code
        type: string
      responses:
        200:
          description: OK
      tags:
      - Server Image
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