---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Confirms the compliance checks have been carried out on a marketing
    role
  version: 1.0.0
  description: Confirms the compliance checks have been carried out on a marketing
    role.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/role/{id}/confirmcompliancechecks:
    put:
      summary: Confirms the compliance checks have been carried out on a marketing
        role
      description: Confirms the compliance checks have been carried out on a marketing
        role.
      operationId: Role_ConfirmComplianceChecksByidBynegotiatorId
      x-api-path-slug: apiroleidconfirmcompliancechecks-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: query
        name: negotiatorId
        description: The negotiator id who confirmed the checks
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Confirms
      - Compliance
      - Checks
      - Have
      - Been
      - Carried
      - Out
      - "On"
      - Marketing
      - Role
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