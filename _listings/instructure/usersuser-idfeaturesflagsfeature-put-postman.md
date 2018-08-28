{
  "info": {
    "name": "Instructure Canvas Users API Set feature flag",
    "_postman_id": "2f9cadb2-585a-443f-a28e-67b28cc74f38",
    "description": "Set feature flag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "0cffd8a9-6be3-4942-a5a2-62be9b0f2abf",
          "name": "list-the-activity-stream",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d4eb13c2-ab04-4e46-8e27-8d9040ebbb56"
            }
          ]
        },
        {
          "id": "7312b8e2-57d0-4869-87e2-5c54d8341531",
          "name": "list-the-activity-stream1",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the activity stream."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7a83323d-00c5-4ae1-bb53-a7bc6f7b1006"
            }
          ]
        },
        {
          "id": "dc869016-e83e-4e56-9059-14410e9c08d8",
          "name": "hide-all-stream-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide all stream items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1170e57b-0c08-490a-bb83-6376c1d85c1f"
            }
          ]
        },
        {
          "id": "06a6ddcc-d51e-440c-a831-d95da69641d6",
          "name": "activity-stream-summary",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/activity_stream/summary",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Activity stream summary."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5e27570-0235-4f23-86b7-56a0433a7a34"
            }
          ]
        },
        {
          "id": "4ad4076d-1292-4b22-9959-29f79724b49f",
          "name": "hide-a-stream-item",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/activity_stream/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Hide a stream item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cbc1766f-eba3-4c3e-9462-c0589c41a215"
            }
          ]
        },
        {
          "id": "36ffcc8e-2203-4293-a728-2af4ccac900e",
          "name": "list-bookmarks",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List bookmarks."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd3e12d5-b8b6-4d0d-9832-2d8d85c4b1d4"
            }
          ]
        },
        {
          "id": "7dbc9679-523e-4f84-9746-996fd3fd6b92",
          "name": "create-bookmark",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/bookmarks?data=%7B%7D&name=%7B%7D&position=%7B%7D&url=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93aa4c9e-7da2-44a2-b9a0-7b96af16fd8d"
            }
          ]
        },
        {
          "id": "d142d037-2e06-421b-99d1-cc4eec7ca627",
          "name": "get-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "addba42b-1aca-43f8-b150-59b2c38c18a0"
            }
          ]
        },
        {
          "id": "5d34dd95-b757-44dc-be92-c0d0fe0ad24e",
          "name": "update-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
              ],
              "query": [
                {
                  "key": "data",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "url",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8806c00f-4791-4f40-967b-6a07c3300b56"
            }
          ]
        },
        {
          "id": "63a71ff9-4b7e-4cf8-a2fe-5dad43ceafbc",
          "name": "delete-bookmark",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/bookmarks/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete bookmark."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98dc2983-3540-402b-8952-a6ea9cb12840"
            }
          ]
        },
        {
          "id": "e9f43d1e-2706-4190-9540-28804ba7b282",
          "name": "update-multiple-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences"
              ],
              "query": [
                {
                  "key": "notification_preferences[X][frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update multiple preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d2156ee9-97b7-4cbc-8a6b-a7f208524541"
            }
          ]
        },
        {
          "id": "0f011736-e438-467f-becf-6a33edc41cc1",
          "name": "update-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preferences/notification"
              ],
              "query": [
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b25b94d6-d540-4713-a99e-6a35b3279c5d"
            }
          ]
        },
        {
          "id": "4edf3538-f444-4af6-8ac5-cf97f6b74185",
          "name": "update-preferences-by-category",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:communication_channel_id/notification_preference_categories/category"
              ],
              "query": [
                {
                  "key": "category",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "communication_channel_id",
                  "value": "communication_channel_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update preferences by category."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "44a4cf95-2e73-4148-9152-8b76594c57d6"
            }
          ]
        },
        {
          "id": "c7350854-8243-401e-9ef3-47ff6d12f30a",
          "name": "update-multiple-preferences1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences"
              ],
              "query": [
                {
                  "key": "notification_preferences[X][frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update multiple preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bdd41d64-6e64-4f7d-8a66-65ef6b7716e9"
            }
          ]
        },
        {
          "id": "783a2451-1e11-4c97-8613-4ecd7b1b770b",
          "name": "update-a-preference1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/communication_channels/:type/address/notification_preferences/:notification"
              ],
              "query": [
                {
                  "key": "notification_preferences[frequency]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "type",
                  "type": "string"
                },
                {
                  "id": "notification",
                  "value": "notification",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67520d8c-ec83-424b-9e2b-685a1d658bcf"
            }
          ]
        },
        {
          "id": "8927e72c-233f-4030-8700-9720145e5733",
          "name": "list-course-nicknames",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/course_nicknames",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List course nicknames."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "13959cbd-1898-4590-b75b-f5aa074946ba"
            }
          ]
        },
        {
          "id": "99e477d7-d127-471d-9299-2a949f93d52f",
          "name": "clear-course-nicknames",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/course_nicknames",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Clear course nicknames."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4073d764-f4fd-41d2-a1da-12801b0a96fd"
            }
          ]
        },
        {
          "id": "ed0560cd-73b3-4fd1-9f3b-4af3783745bf",
          "name": "get-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "19bcea8d-7132-43af-a5b5-bfbe039c9dff"
            }
          ]
        },
        {
          "id": "c47eabce-ab34-465d-a50c-aee512326177",
          "name": "set-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "query": [
                {
                  "key": "nickname",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Set course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "52977e74-c38a-40ae-89fa-3b86e5b185ee"
            }
          ]
        },
        {
          "id": "231ad871-6a45-4e59-8fb0-721145805d61",
          "name": "remove-course-nickname",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/course_nicknames/:course_id"
              ],
              "variable": [
                {
                  "id": "course_id",
                  "value": "course_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove course nickname."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6beee32-3286-4674-ae11-7855140f51e7"
            }
          ]
        },
        {
          "id": "9238c138-ef05-40be-9989-88e4756bc24f",
          "name": "list-favorite-courses",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite courses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34aa29a5-3368-469d-b4f1-c1d6380a9f4e"
            }
          ]
        },
        {
          "id": "c3c2bf8b-1e48-433b-958a-a0f3db225e91",
          "name": "reset-course-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/courses",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset course favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e677e58d-2054-46d9-9579-1ec41ef2ff4b"
            }
          ]
        },
        {
          "id": "3972049c-05bd-4fdf-85a0-d199832e4574",
          "name": "add-course-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
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
            "body": {
              "mode": "raw"
            },
            "description": "Add course to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfb14292-e2d7-4ed6-bd38-b44ea47f6d50"
            }
          ]
        },
        {
          "id": "e78d99d1-b715-4dbd-8c3d-0fd3a38f0efb",
          "name": "remove-course-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/courses/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove course from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7aa12f9e-5986-4983-9131-9e9fe51c3cc8"
            }
          ]
        },
        {
          "id": "cd7f2bf3-7679-4f85-82e8-0b8058e247ac",
          "name": "list-favorite-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List favorite groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bed4bf95-47af-48a7-aa1e-2e5f84cc03bb"
            }
          ]
        },
        {
          "id": "6f86cb67-e489-47c2-b6df-6bd4eb8fb376",
          "name": "reset-group-favorites",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/favorites/groups",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Reset group favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "37d30081-5cf5-4972-9233-a8159bb48ab9"
            }
          ]
        },
        {
          "id": "c4ac87fa-d785-4065-be0b-813a7656b352",
          "name": "add-group-to-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
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
            "body": {
              "mode": "raw"
            },
            "description": "Add group to favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "920a7ece-558c-4085-a4ec-7724e0fc6b69"
            }
          ]
        },
        {
          "id": "a90b03fd-0255-4d53-891e-3f663e0226ac",
          "name": "remove-group-from-favorites",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/self/favorites/groups/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Remove group from favorites."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "28219a1e-b34d-49a9-8cee-5c0b8cd357d3"
            }
          ]
        },
        {
          "id": "fa402964-ddc9-4492-bcf2-170e6faca907",
          "name": "list-your-groups",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/groups?context_type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List your groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56d13f1b-0f36-4ef1-ac8c-32d1a16fceb5"
            }
          ]
        },
        {
          "id": "be01c1d2-9694-4b82-b6fd-7696e8c6b2b4",
          "name": "list-the-todo-items",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/todo",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List the todo items."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e1155aa-13de-451f-80fa-1bdb19dd1390"
            }
          ]
        },
        {
          "id": "27256e1c-397a-45d1-8b20-c562764f8548",
          "name": "list-upcoming-assignments-calendar-events",
          "request": {
            "url": "http://canvas.instructure.com/api/v1/users/self/upcoming_events",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List upcoming assignments, calendar events."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "803c585b-e9d2-4737-b56c-be50354bd1e0"
            }
          ]
        },
        {
          "id": "c1e4c7bd-969c-4768-b77b-338db07e712d",
          "name": "show-user-details",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show user details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dcb838a4-58ea-4958-9ad0-926b47588344"
            }
          ]
        },
        {
          "id": "8a83ab81-f38e-45a3-8773-08426940d04a",
          "name": "edit-a-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id"
              ],
              "query": [
                {
                  "key": "user[avatar][token]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[avatar][url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[email]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[locale]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[short_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[sortable_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "user[time_zone]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Edit a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12c82ec6-bda7-43ca-b0c4-d5a9dc1aa62e"
            }
          ]
        },
        {
          "id": "8305d951-c7ed-4a2f-8e56-2156ea3d81af",
          "name": "get-custom-colors",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get custom colors."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "242f96fd-4318-404d-bb6c-d18fc6e5ba8e"
            }
          ]
        },
        {
          "id": "730ae1f8-9c7a-4f0f-a8fa-a02d205837ae",
          "name": "get-custom-color",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors/asset_string"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get custom color."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2f794bc5-5fe5-487b-84a4-a6f743cd916b"
            }
          ]
        },
        {
          "id": "043ea401-da33-403e-87ea-e911e9dd12c9",
          "name": "update-custom-color",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/colors/asset_string"
              ],
              "query": [
                {
                  "key": "hexcode",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update custom color."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8c49a843-8dc5-40be-81fb-ca5d84620fe3"
            }
          ]
        },
        {
          "id": "53d3a9a4-603f-42ad-950b-7b77f19f26d9",
          "name": "merge-user-into-another-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/merge_into/accounts/destination_account_id/users/:destination_user_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "destination_user_id",
                  "value": "destination_user_id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Merge user into another user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e047459b-11fa-46ba-a111-05d42149a1ec"
            }
          ]
        },
        {
          "id": "b648cc07-78c0-4499-997b-43cda1670645",
          "name": "merge-user-into-another-user1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/merge_into/destination_user_id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Merge user into another user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4af2951e-76fb-4291-aa26-49e96307c9b4"
            }
          ]
        },
        {
          "id": "ba791f87-4349-49b4-88bd-2e1fe6f6d11c",
          "name": "update-user-settings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/settings"
              ],
              "query": [
                {
                  "key": "manual_mark_as_read",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Update user settings.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "38070c46-7430-4ab1-99af-1d1f5f9e4a4b"
            }
          ]
        },
        {
          "id": "4f1ab2e2-5856-4cb5-83fd-cb9a857568a6",
          "name": "update-user-settings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:id/settings"
              ],
              "query": [
                {
                  "key": "manual_mark_as_read",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update user settings.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b58743b7-ea7b-4b91-8649-c23359a1805e"
            }
          ]
        },
        {
          "id": "c70c8103-00bd-4275-84b1-266c6ec7d2fc",
          "name": "list-avatar-options",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/avatars"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List avatar options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cd14da0-db20-4936-89e6-e43983bbc4de"
            }
          ]
        },
        {
          "id": "fa0a0e86-0ed9-425f-8ec9-aa10aee87f12",
          "name": "list-calendar-events-for-a-user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/calendar_events"
              ],
              "query": [
                {
                  "key": "all_events",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "context_codes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "end_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "excludes",
                  "value": "%5B%7B%7D%5D",
                  "disabled": false
                },
                {
                  "key": "start_date",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "undated",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List calendar events for a user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6e804c20-39e2-4aad-8b53-656efae68167"
            }
          ]
        },
        {
          "id": "83749ae7-c94a-4346-8bac-69c174c48f0a",
          "name": "list-user-communication-channels",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List user communication channels."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b8a3faa-c6ac-4e2e-af3c-90ae4d94347b"
            }
          ]
        },
        {
          "id": "9f4dabc0-2323-4a86-871f-cde563e643fe",
          "name": "create-a-communication-channel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels"
              ],
              "query": [
                {
                  "key": "communication_channel[address]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "communication_channel[token]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "communication_channel[type]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_confirmation",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a communication channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "715ac677-a6a5-462c-84a8-05d22ddcffc4"
            }
          ]
        },
        {
          "id": "4ceff81b-ab57-48ee-bb70-e2761b2b849f",
          "name": "list-preferences",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/communication_channel_id/notification_preferences"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a575ac8-51eb-401a-b882-2daa78e2bfea"
            }
          ]
        },
        {
          "id": "abd206b4-2bbc-414f-a00f-6b67534ccd28",
          "name": "get-a-preference",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/communication_channel_id/notification_preferences/:notification"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "notification",
                  "value": "notification",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7100051f-8262-42f4-a905-da11cdd0020f"
            }
          ]
        },
        {
          "id": "9e399161-98bd-44d6-b320-76af55221a68",
          "name": "list-of-preference-categories",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/communication_channel_id/notification_preference_categories"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List of preference categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6c730f1-6c9f-4ffd-bd57-c69c95eb8f5f"
            }
          ]
        },
        {
          "id": "82a8ca5f-1324-44c5-bef3-1f4b97d7b888",
          "name": "delete-a-communication-channel",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a communication channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27b15074-095d-4961-8e1f-51c2f1a5bbd3"
            }
          ]
        },
        {
          "id": "5a2c026b-9861-48c2-ab06-c2f1efefcfdb",
          "name": "delete-a-communication-channel1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a communication channel."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "47540d72-a06d-4b6b-a739-b6c1b027b18d"
            }
          ]
        },
        {
          "id": "9004d5ae-b16c-4c0c-84b4-00fd025d6470",
          "name": "list-preferences1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address/notification_preferences"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List preferences."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0729a58-a1cc-41ee-b242-36f82dff5366"
            }
          ]
        },
        {
          "id": "4f60345a-018c-41d1-a150-7386ad46eb58",
          "name": "get-a-preference1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/communication_channels/type/:address/notification_preferences/notification"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "address",
                  "value": "address",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a preference."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daff6b62-abc0-4994-a49b-8c42d4cf297d"
            }
          ]
        },
        {
          "id": "f4ccc776-0f4e-4cb8-b2c6-733cbf84984b",
          "name": "list-content-exports",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content exports."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d7388f6-34ba-4b08-9ca7-9fcf55e7ea81"
            }
          ]
        },
        {
          "id": "d3f12e76-6f6c-4174-be35-ef4a36e729a4",
          "name": "export-content",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports"
              ],
              "query": [
                {
                  "key": "export_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "skip_notifications",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Export content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8eb6d1e-a5a0-4ffb-bf43-8cac67ffa2ef"
            }
          ]
        },
        {
          "id": "dba2293d-f6de-4af7-9583-7948db5ba3c4",
          "name": "show-content-export",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_exports/id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Show content export."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f7fb839-07ee-4ea7-8966-36a0557f4904"
            }
          ]
        },
        {
          "id": "c3a72d25-6b3d-42dc-bf0f-fbf33db83a0c",
          "name": "list-licenses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_licenses"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List licenses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c88202d3-f76c-4463-8673-1bb2d51d62d4"
            }
          ]
        },
        {
          "id": "302a1c8d-501d-4f48-8cbb-e9a2519ee116",
          "name": "list-content-migrations",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List content migrations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "560da594-c5e2-4340-9be5-f0fb28291274"
            }
          ]
        },
        {
          "id": "976e20a8-9950-4538-b1c7-185f97f1edb8",
          "name": "create-a-content-migration",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations"
              ],
              "query": [
                {
                  "key": "date_shift_options[day_substitutions][X]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[new_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_end_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[old_start_date]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[remove_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "date_shift_options[shift_dates]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "migration_type",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[*]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pre_attachment[name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[file_url]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[folder_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[overwrite_quizzes]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_id]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[question_bank_name]",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "settings[source_course_id]",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a content migration."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "af27a1cc-2fee-46d9-ae36-7282728adf31"
            }
          ]
        },
        {
          "id": "b3c35b33-2571-4ae0-9b24-ca165edb068c",
          "name": "list-migration-issues",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List migration issues."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c621ec50-d5c0-45c5-9321-030776f797ed"
            }
          ]
        },
        {
          "id": "3576c3da-741b-41ea-abad-a8214871895b",
          "name": "get-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a migration issue."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31fc9290-e8ec-42ac-b499-f125fb325a89"
            }
          ]
        },
        {
          "id": "f3b595dc-ecb0-4cf7-8b62-68ce18ae9153",
          "name": "update-a-migration-issue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "canvas.instructure.com",
              "path": [
                "api",
                "v1",
                "users/:user_id/content_migrations/content_migration_id/migration_issues/:id"
              ],
              "query": [
                {
                  "key": "workflow_state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "user_id",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Update a migrat