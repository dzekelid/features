{
  "info": {
    "name": "Dezrez Gets all the active features for an agency",
    "_postman_id": "b4dc0c73-d773-400f-a142-883e7caab5a9",
    "description": "Gets all the active features for an agency.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SystemStatus",
      "item": [
        {
          "id": "9128c9d5-8ec2-4db3-a154-bd2992ffa386",
          "name": "Branch_UpdateScheduledTaskStatusByidBysystemStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/branch/updatescheduledtaskstatus/:id"
              ],
              "query": [
                {
                  "key": "systemStatus",
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
            "method": "POST",
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
            "description": "Update systemstatus of scheduledtask to active, inactive, deleted or archived.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8aad0180-8e1b-4f0c-9f26-fedc627b2299"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "3ae88c1b-a1df-466f-8401-73acbfc8886d",
          "name": "DefaultToDo_ActiveTasksBytoDoIdByignoreDueDateBypageSizeBypageNumber",
          "request": {
            "url": "http://api.dezrez.com/api/todo/activetasks?ignoreDueDate=%7B%7D&pageNumber=%7B%7D&pageSize=%7B%7D&toDoId=%7B%7D",
            "method": "GET",
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
            "description": "Get the list of active tasks of a todo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "041ffa18-1eb4-4694-b4bb-b00cb373c974"
            }
          ]
        }
      ]
    },
    {
      "name": "S",
      "item": [
        {
          "id": "43719a59-2e40-44f5-86bc-14096740aa36",
          "name": "EnlistedFeature_GetAllValidEnlistedFeaturesForAgency",
          "request": {
            "url": "http://api.dezrez.com/api/enlistedfeature/getvalidforagency",
            "method": "GET",
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
            "description": "Gets all the active features for an agency."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b45b7cfb-b0c6-4bf1-af1f-fd08ba10bfe7"
            }
          ]
        }
      ]
    }
  ]
}