---
swagger: "2.0"
x-collection-name: New Relic
x-complete: 1
info:
  title: New Relic
  version: 1.0.0
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/reset_password.{format}:
    post:
      summary: Add Users  Reset Password. Format
      description: This API endpoints reset the user password, identified by ID
      operationId: postUsersResetPassword.Format
      x-api-path-slug: usersidreset-password-format-post
      parameters:
      - in: path
        name: id
        description: User ID
        type: integer
      responses:
        200:
          description: OK
      tags:
      - Users
      - ""
      - Reset
      - Password.
      - Format
---