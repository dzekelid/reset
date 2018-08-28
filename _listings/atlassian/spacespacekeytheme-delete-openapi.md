---
swagger: "2.0"
x-collection-name: Atlassian
x-complete: 0
info:
  title: Confluence Cloud API Reset space theme
  description: "Resets the space theme. This means that the space will inherit the
    \nglobal look and feel settings\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**:\n'Admin' permission for the space."
  termsOfService: http://atlassian.com/terms/
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