swagger: "2.0"
x-collection-name: Atlassian
x-complete: 1
info:
  title: Stride API
  description: this-service-provides-public-api-for-the-stride-
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /settings/lookandfeel/custom:
    delete:
      summary: Reset look and feel settings
      description: "Resets the custom look and feel settings for the site or a single
        space.\nThis changes the values of the custom settings to be the same as the
        \ndefault settings. It does not change which settings (default or custom)
        \nare selected. Note, the default space settings are inherited from the \ncurrent
        global settings.\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**: \n'Admin' permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.LookAndFeelResource.resetLookAndFeelSettings_dele
      x-api-path-slug: settingslookandfeelcustom-delete
      parameters:
      - in: query
        name: spaceKey
        description: The key of the space for which the look and feel settings will
          bereset
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Look
      - Feel
      - Settings
  /space/{spaceKey}/theme:
    delete:
      summary: Reset space theme
      description: "Resets the space theme. This means that the space will inherit
        the \nglobal look and feel settings\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
        required**:\n'Admin' permission for the space."
      operationId: com.atlassian.confluence.plugins.restapi.resources.SpaceThemeResource.resetSpaceTheme_delete
      x-api-path-slug: spacespacekeytheme-delete
      parameters:
      - in: path
        name: spaceKey
        description: The key of the space to reset the theme for
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Space
      - Theme
  /api/2/filter/{id}/columns:
    delete:
      summary: Reset columns
      description: Reset the user's column configuration for the filter to the default.
        **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:** Permission
        to log in to Jira (i.e., member of the _users_ [group](https://confluence.atlassian.com/x/24xjL))
        and permission to view the filter.
      operationId: com.atlassian.jira.rest.v2.search.FilterResource.resetColumns_delete
      x-api-path-slug: api2filteridcolumns-delete
      parameters:
      - in: path
        name: id
        description: The ID of the filter
      responses:
        200:
          description: OK
      tags:
      - Reset
      - Columns
  /api/2/user/columns:
    delete:
      summary: Reset user default columns
      description: |-
        Resets the default [issue table columns](https://confluence.atlassian.com/x/XYdKLg) for the user to the system default. If a username is not passed, the calling user's default columns are reset. **[Permissions](https://confluence.atlassian.com/x/FQiiLQ) required:**

        *   To set the columns on any user: _Administer Jira_ [global permission](https://confluence.atlassian.com/adminjiracloud/managing-global-permissions-776636359.html).
        *   To set the calling user's columns: None
      operationId: com.atlassian.jira.rest.v2.issue.UserResource.resetUserColumns_delete
      x-api-path-slug: api2usercolumns-delete
      parameters:
      - in: query
        name: accountId
        description: the account ID
      - in: header
        name: force-account-id
      - in: query
        name: username
        description: The username of the user
      responses:
        200:
          description: OK
      tags:
      - Reset
      - User
      - Default
      - Columns