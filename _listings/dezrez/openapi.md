---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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
  /api/role/{id}/setcompliancechecks:
    put:
      summary: Set the compliance checks on a property marketing role i.e. Valid Epc,
        Proof of ID or Proof of Ownership.
      description: Set the compliance checks on a property marketing role i.e. valid
        epc, proof of id or proof of ownership..
      operationId: Role_SetComplianceChecksByidBysetComplianceChecksDataContract
      x-api-path-slug: apiroleidsetcompliancechecks-put
      parameters:
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: setComplianceChecksDataContract
        description: The flag detail
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Set
      - Compliance
      - Checks
      - "On"
      - Property
      - Marketing
      - Role
      - I
      - E
      - ""
      - Valid
      - Epc
      - ""
      - Proof
      - Of
      - ID
      - Proof
      - Of
      - Ownership
---