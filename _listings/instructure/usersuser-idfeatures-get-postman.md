{
  "info": {
    "name": "Instructure Canvas Users API List features",
    "_postman_id": "39726fa5-0ede-4916-b153-f5a0b9cd0312",
    "description": "List features.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Users",
      "item": [
        {
          "id": "aa48562f-fac6-4086-96ad-bec86ab9f8b7",
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
              "id": "a0a665bd-2b51-44cc-8218-b715be19ade5"
            }
          ]
        },
        {
          "id": "e11bd4d8-85c0-4f16-aca0-a5a0942aaa5c",
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
              "id": "e717acef-d9cb-4b47-a97c-99a042723d7c"
            }
          ]
        },
        {
          "id": "90f53d0b-ff1b-4085-bb13-4de5aa260343",
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
              "id": "0fdd0b8a-3cb2-42e9-ae98-755c27d76bd1"
            }
          ]
        },
        {
          "id": "14ed047d-4854-4d6a-a0c7-e571e5d442b3",
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
              "id": "02be27d0-5c47-4c6c-a918-0b9c0d84ab0d"
            }
          ]
        },
        {
          "id": "78c6a354-3acd-4d90-aba5-858b2eda2b4e",
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
              "id": "6be59931-ede1-4bf9-b04d-2624150c30d2"
            }
          ]
        },
        {
          "id": "e7f3b223-0f21-49ee-98ac-633ad7128bfb",
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
              "id": "a2b959df-8ab8-4e81-8e9a-2d28f8d0fd20"
            }
          ]
        },
        {
          "id": "bb2405da-8395-4397-87a0-6b2c31c36cba",
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
              "id": "78b88f8a-d979-4053-bdf5-2b7699f50a24"
            }
          ]
        },
        {
          "id": "8b3c035e-d84a-4c85-8e40-b01153f11ad9",
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
              "id": "b8cb54b1-9c11-4bc8-b73d-cfbf30398384"
            }
          ]
        },
        {
          "id": "ae633591-0e6d-4f47-84a4-664d8e864d1a",
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
              "id": "56fe034c-c6f9-4eed-aa4b-ce098586bbeb"
            }
          ]
        },
        {
          "id": "f0b4332e-765e-4423-a345-4d844dc89c43",
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
              "id": "f1ef987d-2a39-4172-9554-b726292c7641"
            }
          ]
        },
        {
          "id": "c4ffeba9-66c0-410f-bdaf-73f952611a24",
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
              "id": "a93976f5-dcd6-4171-b48c-fa558b557c45"
            }
          ]
        },
        {
          "id": "8b3e0ec2-fc91-4275-8e6e-bfa17adc6bd1",
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
              "id": "ad791d80-c1cc-4cff-8797-abee8f044787"
            }
          ]
        },
        {
          "id": "3fb77edf-3e70-4001-9d08-d3c94c843d95",
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
              "id": "6e47df7a-0101-46d9-8f98-89065811662b"
            }
          ]
        },
        {
          "id": "6089e8df-65b4-4ec9-852d-6c95b53b6236",
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
              "id": "70f4ea11-2afc-4388-841c-54272de3e7c2"
            }
          ]
        },
        {
          "id": "ef1b44c3-5b73-4a41-bb79-67121bc64ca4",
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
              "id": "0d47502d-73f9-4a0b-8d6f-eee448ed01e4"
            }
          ]
        },
        {
          "id": "d9bdaf43-ddd9-4d0e-bb36-935a4b5d98de",
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
              "id": "459512cf-46dc-43bb-8ba0-8b1d04f5f404"
            }
          ]
        },
        {
          "id": "a2206db0-d78d-4a14-9a1f-26e8a3667da6",
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
              "id": "07b704e7-564d-4b1c-aad9-ce5ffb0f7f80"
            }
          ]
        },
        {
          "id": "a25a16e1-4133-45c8-a3dc-2b35c86f8cb8",
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
              "id": "e0cb91ac-3df9-4d9e-9550-0cfd8b889032"
            }
          ]
        },
        {
          "id": "3d9c4be8-17f0-4666-a1e9-c49190f36c93",
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
              "id": "984f89eb-9866-4cef-875f-32ae910d829f"
            }
          ]
        },
        {
          "id": "16556726-c9ff-4e5d-acee-3177435d7277",
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
              "id": "34a5eca9-ab07-40d9-b600-c54e788aba15"
            }
          ]
        },
        {
          "id": "165863b8-d0aa-404b-a1fa-aec5caa6496e",
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
              "id": "6f623e8a-8374-4d18-94cc-e4f7429ff926"
            }
          ]
        },
        {
          "id": "1abb1af6-c087-4041-b633-86750041537a",
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
              "id": "a60860fc-d154-4a4d-82b5-445e9db6dfbe"
            }
          ]
        },
        {
          "id": "6c5f73ab-62a3-4d9a-bfe5-7ea9789b3803",
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
              "id": "492c6d72-0ded-41b8-ba6d-562ae82751da"
            }
          ]
        },
        {
          "id": "3a2a8633-70f4-490b-9e96-fbe89acb49c6",
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
              "id": "7149e9d7-5908-42bf-84ba-f559804af79a"
            }
          ]
        },
        {
          "id": "88305938-8a82-44f2-8c64-8100c4348668",
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
              "id": "d76c6659-4fe4-4b01-aea4-b1d5d471c514"
            }
          ]
        },
        {
          "id": "de712f7f-31e5-4059-a4a4-37a6702e55ac",
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
              "id": "5cdcd81e-b512-4374-aaea-e95a2505ee8f"
            }
          ]
        },
        {
          "id": "9f2d2098-18b8-42b0-8808-7eda19aabdff",
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
              "id": "bef92086-88cb-4822-8d69-8fdbc6531d2b"
            }
          ]
        },
        {
          "id": "a18e215e-556c-4cec-9a32-c217f44179f7",
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
              "id": "3a5af783-2079-4721-9720-64d396bad784"
            }
          ]
        },
        {
          "id": "8a31c45f-2c8b-489d-ba60-4678a9dec941",
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
              "id": "268e75ce-89c3-47a9-8616-d057a839782c"
            }
          ]
        },
        {
          "id": "d98d6cdb-7e9d-4d33-8199-e156f7dd5b5e",
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
              "id": "f7b95382-b2aa-4696-a5c9-e207f7006361"
            }
          ]
        },
        {
          "id": "75fc6d53-9920-4224-affa-a895fa5e99fc",
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
              "id": "b3865a31-2623-4d1d-9689-a644f4df3cfc"
            }
          ]
        },
        {
          "id": "e7f40e3f-56ff-4177-8863-b8019ca8de27",
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
              "id": "5da55208-f456-4f9e-beb5-f943c35a242f"
            }
          ]
        },
        {
          "id": "014b09d9-da88-4d76-9420-39883f7dbb2b",
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
              "id": "a7823f4f-b520-4a4d-9916-36ee3edea20e"
            }
          ]
        },
        {
          "id": "c89a20da-cf7b-451d-b9e4-e45013740749",
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
              "id": "72325ecd-17fa-4a72-b469-485d0173c18b"
            }
          ]
        },
        {
          "id": "42862917-aa94-450a-98a2-032b62567035",
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
              "id": "944473d3-93e4-4eac-814d-05bc993d7fd1"
            }
          ]
        },
        {
          "id": "77ce3e00-900b-4373-9744-ccbf33da8ec0",
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
              "id": "bb30d79b-2b31-4c18-b3d4-8b7906515311"
            }
          ]
        },
        {
          "id": "4600783f-62e7-4f5f-bf68-981ba2118257",
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
              "id": "5d9f96f5-49b2-446e-8e5f-ddfabf3171d2"
            }
          ]
        },
        {
          "id": "6168eb39-541f-4330-abb9-d7e6b7695abc",
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
              "id": "fa41e19e-e95f-4c7b-a54a-721986300c77"
            }
          ]
        },
        {
          "id": "9f337ce6-afb7-41f1-ac2a-201437fbcf1e",
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
              "id": "eb975a25-1d7b-4533-afdd-c5fd5c113833"
            }
          ]
        },
        {
          "id": "b5c5dec6-31f5-4821-b122-8cf4e79c07a0",
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
              "id": "e1df7b19-f5b5-4b0a-a222-d8192b687686"
            }
          ]
        },
        {
          "id": "cb31391e-8ac9-4b64-bc63-1318e0f84a5e",
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
              "id": "259e31c6-b0c5-4829-b862-e47d0665aa23"
            }
          ]
        },
        {
          "id": "7d5f2831-3df6-48da-9897-100c4d7c922e",
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
              "id": "e7f12833-7376-4ae1-9388-99b9c1b82e69"
            }
          ]
        },
        {
          "id": "5e95506c-155a-46e6-a13c-125f4876475a",
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
              "id": "6f5ad7db-52ac-4530-82e1-affeb290e839"
            }
          ]
        },
        {
          "id": "4cafbd8e-10d2-479b-b6ed-e5f615cc495e",
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
              "id": "1bf0d1d4-a398-49b5-b338-c7145abe91be"
            }
          ]
        },
        {
          "id": "bf905bcf-5960-4834-94b5-898b75eb783d",
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
              "id": "e3b8b683-1df1-4288-8a84-f704a9719696"
            }
          ]
        },
        {
          "id": "fd88de14-8415-43ad-9813-717ed38ba4b5",
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
              "id": "ea7b0e89-a167-45c1-82a4-0e7e16dc5610"
            }
          ]
        },
        {
          "id": "05ef3a05-1a4d-4fe7-8727-1fa41f96a362",
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
              "id": "7883b442-8697-4c4e-9e22-ff839174c399"
            }
          ]
        },
        {
          "id": "f5d53703-5b8c-4456-8430-524d09dc91ed",
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
              "id": "dd274360-061a-4816-b228-d56736d9afe7"
            }
          ]
        },
        {
          "id": "63486b2b-ba96-4a8f-8698-851259008adf",
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
              "id": "09e88fbe-78e4-4848-8ef9-3a5a88364cf7"
            }
          ]
        },
        {
          "id": "2b9d54ce-48d2-4221-8ca0-199f9a38e8f6",
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
              "id": "54b04210-14ad-4e35-bb3b-a00c31c2a289"
            }
          ]
        },
        {
          "id": "9d70043c-4563-4ad2-9640-9bf01e32e166",
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
              "id": "813d6a7b-2ea0-4d82-b5dd-a9da1e5f795c"
            }
          ]
        },
        {
          "id": "33680f17-7889-4379-94cc-e9358b485966",
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
              "id": "ab4d465d-ffdc-49f8-845f-4c51e567efdf"
            }
          ]
        },
        {
          "id": "3271f046-6b4f-4d2e-a1cd-ef65d7143ad6",
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
              "id": "2ff49b22-655d-439b-984f-bbc71d38d2ca"
            }
          ]
        },
        {
          "id": "1d92abdb-837e-4595-88bd-e873e3b175bd",
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
              "id": "8dc29812-268c-4fd5-800d-97bc6e194e42"
            }
          ]
        },
        {
          "id": "943c0a1b-5543-45fc-a0d5-1ba1a1fae55d",
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
              "id": "a3851e36-ca3a-46d8-9c45-86502f54aab1"
            }
          ]
        },
        {
          "id": "4fe4d161-72c8-41e5-bead-f25b23ea3c10",
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
              "id": "bd06274d-7c70-4e0c-9415-d77dab825235"
            }
          ]
        },
        {
          "id": "7569bc5a-20de-45ba-8bdd-24ed7e2b154a",
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
              "id": "1d050766-b1e9-42a6-9a54-28f179933e1b"
            }
          ]
        },
        {
          "id": "733187c3-bf17-45e2-8ba1-a402cf12ccce",
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
              "id": "bc27c234-31e0-4362-85af-7f03ba83cb31"
            }
          ]
        },
        {
          "id": "ff07da36-7d61-4aa5-b054-5ed0455b99b8",
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
              "id": "97220126-5cf6-4830-881f-20e8b1fa610e"
            }
          ]
        },
        {
          "id": "63da0998-2518-4916-816f-c23cc49e4248",
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
            "description": "Update a migration is