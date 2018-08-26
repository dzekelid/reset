---
swagger: "2.0"
x-collection-name: Okta
x-complete: 1
info:
  title: Users (Okta API)
  description: the-okta-user-apidocsapirestusers-html-provides-operations-to-manage-users-in-your-organization-
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userId}/lifecycle/reset_factors:
    post:
      summary: Reset Factors
      description: Reset factors.
      operationId: postUsersUserLifecycleResetFactors
      x-api-path-slug: usersuseridlifecyclereset-factors-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Factors
  /users/{userId}/lifecycle/reset_password:
    post:
      summary: Reset Password
      description: Reset password.
      operationId: postUsersUserLifecycleResetPassword
      x-api-path-slug: usersuseridlifecyclereset-password-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: sendEmail
      - in: path
        name: userId
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Password
---