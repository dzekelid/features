{
  "info": {
    "name": "Launch Darkly Modify a feature flag by ID",
    "_postman_id": "815a830e-d5a5-48ae-8465-9a14442c3c20",
    "description": "Modify a feature flag by id.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Environments",
      "item": [
        {
          "id": "d616e802-7076-4cee-9ee5-17e5c0298b8f",
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
              "id": "a2707069-0126-48fc-9143-4427ca4879e4"
            }
          ]
        },
        {
          "id": "917ed13e-952c-42ed-a585-455572fc99e6",
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
              "id": "078fe416-6393-496f-bc45-53a8d39b82c8"
            }
          ]
        },
        {
          "id": "01c8532d-0164-4350-94d1-133178adf950",
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
              "id": "002dc105-3e0f-42c1-bddf-a815d1477ac8"
            }
          ]
        },
        {
          "id": "bda54219-1e79-40f5-85d8-4d1313e6d012",
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
              "id": "1e882d88-f9a4-4b3e-a8c9-f0f65e94a88b"
            }
          ]
        }
      ]
    },
    {
      "name": "Flag-statuses",
      "item": [
        {
          "id": "3f175a93-ad15-4e8e-9ebd-851fbcce5f47",
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
              "id": "ee6c32d0-128c-4080-84d6-c59add5a0f33"
            }
          ]
        },
        {
          "id": "fa971484-8b7e-4e73-a13f-2167f778cf03",
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
              "id": "2c285b88-72e6-4714-91ba-3660a25c0e91"
            }
          ]
        }
      ]
    },
    {
      "name": "Flags",
      "item": [
        {
          "id": "0dd4a8c3-7e88-4047-8a8c-32f0b926d1fa",
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
              "id": "ed965566-4330-49fc-b686-4b74b987d2da"
            }
          ]
        },
        {
          "id": "40ba93aa-04b1-4c9d-876a-c81279789464",
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
              "id": "ddd6cc80-77b2-4e74-b429-36073dc64fcb"
            }
          ]
        },
        {
          "id": "6e084dad-3cf9-45f1-9b91-92a951afeb25",
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
              "id": "b0e90470-0818-450b-936b-3802b5aa27d8"
            }
          ]
        },
        {
          "id": "2817d318-0372-4b76-9676-a461f5b34ef0",
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
              "id": "b8338fac-d19b-4968-bb78-a3ede371db9c"
            }
          ]
        },
        {
          "id": "758e5662-21a9-4e18-9705-773f15b60138",
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
              "id": "945fcfc3-5eae-4b93-9df6-f96c22d14e83"
            }
          ]
        }
      ]
    }
  ]
}