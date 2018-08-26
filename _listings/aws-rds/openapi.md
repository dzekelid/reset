---
swagger: "2.0"
x-collection-name: AWS RDS
x-complete: 1
info:
  title: AWS RDS API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ResetDBClusterParameterGroup:
    get:
      summary: Reset D B Cluster Parameter Group
      description: Modifies the parameters of a DB cluster parameter group to the
        default value.
      operationId: resetdbclusterparametergroup
      x-api-path-slug: actionresetdbclusterparametergroup-get
      parameters:
      - in: query
        name: DBClusterParameterGroupName
        description: The name of the DB cluster parameter group to reset
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: A list of parameter names in the DB cluster parameter group to
          reset to the default values
        type: string
      - in: query
        name: ResetAllParameters
        description: A value that is set to true to reset all parameters in the DB
          cluster parameter group       to their default values, and false otherwise
        type: string
      responses:
        200:
          description: OK
      tags:
      - Cluster Parameter Groups
  /?Action=ResetDBParameterGroup:
    get:
      summary: Reset D B Parameter Group
      description: Modifies the parameters of a DB parameter group to the engine/system
        default value.
      operationId: resetdbparametergroup
      x-api-path-slug: actionresetdbparametergroup-get
      parameters:
      - in: query
        name: DBParameterGroupName
        description: The name of the DB parameter group
        type: string
      - in: query
        name: Parameters.Parameter.N
        description: An array of parameter names, values, and the apply method for
          the parameter update
        type: string
      - in: query
        name: ResetAllParameters
        description: Specifies whether (true) or not (false) to reset all parameters        in
          the DB parameter group to default values
        type: string
      responses:
        200:
          description: OK
      tags:
      - Parameter Groups
---