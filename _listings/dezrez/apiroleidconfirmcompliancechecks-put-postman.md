{
  "info": {
    "name": "Dezrez Confirms the compliance checks have been carried out on a marketing role",
    "_postman_id": "d87f17cf-9abd-4bb4-bd63-a06e33405b64",
    "description": "Confirms the compliance checks have been carried out on a marketing role.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Confirms",
      "item": [
        {
          "id": "83a73b23-cf29-4b3a-b17e-a54e2020d6e4",
          "name": "Role_ConfirmComplianceChecksByidBynegotiatorId",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/role/:id/confirmcompliancechecks"
              ],
              "query": [
                {
                  "key": "negotiatorId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Confirms the compliance checks have been carried out on a marketing role."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "66cec72c-0575-4ecd-8d91-1389d5749046"
            }
          ]
        }
      ]
    }
  ]
}