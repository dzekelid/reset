---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 1
info:
  title: Microsoft Graph API
  description: microsoft-graph-exposes-multiple-apis-from-office-365-and-other-microsoft-cloud-services-through-a-single-endpoint-httpsgraph-microsoft-com--microsoft-graph-simplifies-queries-that-would-otherwise-be-more-complex-
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{id}/resetUnseenCount:
    post:
      summary: Group Reset Unseen Count
      description: 'group: resetUnseenCount Reset the unseenCount of all the posts
        that the current user has not seen since their last visit. Supported for only
        Office 365 groups.'
      operationId: Group:ResetUnseenCount
      x-api-path-slug: groupsidresetunseencount-post
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - Group
      - Reset
      - Unseen
      - Count
---