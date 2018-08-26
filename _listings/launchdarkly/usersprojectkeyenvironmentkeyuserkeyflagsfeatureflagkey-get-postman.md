{
  "info": {
    "name": "Launch Darkly Get a user by key.",
    "_postman_id": "44d7122b-70ef-4b19-b5a6-4ceea0580bc4",
    "description": "Get a user by key..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "79e69197-3f96-4545-8d11-e75c3f52468b",
          "name": "postEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create an environment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32fca846-11df-4bf9-ba52-a48c1d8ee80a"
            }
          ]
        },
        {
          "id": "a11b3c71-ff50-4473-9965-e736a8483a52",
          "name": "getEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get an environment by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25ae42c7-0dc7-4dc2-a84a-852246f62df7"
            }
          ]
        },
        {
          "id": "237a882b-8d84-4d4e-8b28-9f6c77e40e84",
          "name": "deleteEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an environment by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6f05b60-2eda-4563-9e94-c48934943b9c"
            }
          ]
        },
        {
          "id": "9f50382a-b5cc-46e0-9871-1b7fcc9e7d69",
          "name": "patchEnvironment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "environments/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify an environment by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0bb80583-fac0-43e9-82b7-e6646fafef4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Flag-statuses",
      "item": [
        {
          "id": "d6effa26-c893-42b7-8f73-f4d32bf72f55",
          "name": "getFeatureFlagStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flag-statuses/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of statuses for all feature flags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "17f46701-ff7b-4196-81e3-7eb3f6bcc320"
            }
          ]
        },
        {
          "id": "d309f86d-96a2-4293-8c08-b5cdb5dc3b0a",
          "name": "getFeatureFlagStatuses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flag-statuses/:projectKey/:environmentKey/:featureFlagKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of statuses for all feature flags."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e6bd2144-a13f-4980-9273-d305ea044bfd"
            }
          ]
        }
      ]
    },
    {
      "name": "Flags",
      "item": [
        {
          "id": "caa22723-ea7b-4329-b9af-e59723466186",
          "name": "getFeatureFlags",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of all features in the given project.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9f684ce-ca35-4624-8900-a5000532cf08"
            }
          ]
        },
        {
          "id": "bf8951a4-af60-451c-a9bc-e5cb9aca71e4",
          "name": "postFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a feature flag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88f68cb8-1e75-470a-b534-ba6bc5e88c9c"
            }
          ]
        },
        {
          "id": "499ab2a4-e3f6-4a23-86d8-3ca39692862a",
          "name": "getFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a single feature flag by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04199f81-493f-4835-8596-389decb3096b"
            }
          ]
        },
        {
          "id": "6a56fc30-ed60-44e3-8391-73e38a318100",
          "name": "deleteFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a feature flag by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7bf78d98-c4c5-4d87-afdf-422734f8443b"
            }
          ]
        },
        {
          "id": "b9df61f4-7893-4a84-a146-0692a368f1bd",
          "name": "patchFeatureFlag",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "flags/:projectKey/:featureFlagKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a feature flag by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "046cbafd-7d26-41a0-99c6-b7ba35cf6b48"
            }
          ]
        }
      ]
    },
    {
      "name": "Projects",
      "item": [
        {
          "id": "f60bfbd6-ecd7-4f6c-bf24-e790600166c7",
          "name": "getProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a project by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40278dab-9dff-4f52-8b7a-51e985e8bec8"
            }
          ]
        },
        {
          "id": "99718f7d-1c60-4f3d-a7a4-b65d5d4927f9",
          "name": "deleteProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a project by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cedf3481-38e3-41dc-bfad-a79817568cae"
            }
          ]
        },
        {
          "id": "91f88bc1-7bfb-4135-8f6f-3cf3fa928fc9",
          "name": "patchProject",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "projects/:projectKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                }
              ]
            },
            "method": "PATCH",
            "body": {
              "mode": "raw"
            },
            "description": "Modify a project by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4ace6bc5-9216-4d92-8041-dfe263560c0e"
            }
          ]
        }
      ]
    },
    {
      "name": "User-search",
      "item": [
        {
          "id": "82348050-8452-40bf-a7aa-b6582788c6e1",
          "name": "getSearchUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "user-search/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Search users in launchdarkly based on their last active date, or a search query.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8b17a2e-a92a-41ce-8dba-7fd548ee5682"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "52b0e3e7-dcfc-40e5-88f5-2922b16c43f4",
          "name": "getUsers",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all users in the environment.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bd6f5be-ef07-4cda-8e4c-e45550b0f720"
            }
          ]
        },
        {
          "id": "a241820c-eab0-4912-b954-45ce76096947",
          "name": "getUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7dd3addb-efb2-4dd5-90fa-16cd047dc6bd"
            }
          ]
        },
        {
          "id": "2b16f699-1f92-46ba-bccf-194497cff06d",
          "name": "deleteUser",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a user by id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "862d3d9e-cb40-4ad2-8525-e5d2048bcbf9"
            }
          ]
        },
        {
          "id": "44f392c7-a8e4-44e3-a8e3-a09425667e2f",
          "name": "getUserFlagSettings",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey/flags"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists the current flag settings for a given user.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5d48d8f7-c553-4190-9fac-7e32eb1fa44a"
            }
          ]
        },
        {
          "id": "dfdbdfff-c2b9-4bec-8172-4ecde65f1052",
          "name": "getUserFlagSetting",
          "request": {
            "url": {
              "protocol": "http",
              "host": "app.launchdarkly.com",
              "path": [
                "api",
                "v2",
                "users/:projectKey/:environmentKey/:userKey/flags/:featureFlagKey"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "projectKey",
                  "value": "projectKey",
                  "type": "string"
                },
                {
                  "id": "environmentKey",
                  "value": "environmentKey",
                  "type": "string"
                },
                {
                  "id": "userKey",
                  "value": "userKey",
                  "type": "string"
                },
                {
                  "id": "featureFlagKey",
                  "value": "featureFlagKey",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a user by key.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d0f197b1-6755-4d2c-8ce4-4b5b2a6886d3"
            }
          ]
        }
      ]
    }
  ]
}