{
  "info": {
    "name": "3Scale Account Management API Account Plan Features Create",
    "_postman_id": "b8b1519f-3ed1-482a-8ea6-12f4b71f87a8",
    "description": "Account plan features create.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Account",
      "item": [
        {
          "id": "47460d5d-4eb1-4131-9573-a3e3b30a72b6",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts.xml?page=%7B%7D&per_page=%7B%7D&provider_key=%7B%7D&state=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e95a5d1-fdab-4af8-9f7c-222aa0f2468f"
            }
          ]
        },
        {
          "id": "be4f9476-866c-4fc9-8a8f-b5e8428b80f9",
          "name": "account",
          "request": {
            "url": "http://su1.3scale.net/admin/api/accounts/find.xml?email=%7B%7D&provider_key=%7B%7D&username=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account find."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72c24b4b-6010-4930-aba0-8b5d47768e50"
            }
          ]
        },
        {
          "id": "e64bbb6c-5444-41f0-a514-cf409411addf",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/messages.xml"
              ],
              "query": [
                {
                  "key": "body",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f836196-54df-4b9c-a91a-96ae8fb59c96"
            }
          ]
        },
        {
          "id": "783c6f84-d27c-45da-812a-2262aaa679a8",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account fetch account plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c75728f5-fdc1-4d7e-be78-14e8704edce8"
            }
          ]
        },
        {
          "id": "bda120b4-15ad-45fa-8add-4c5086d9ad34",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "819d0f62-e2de-47d7-b4d8-8c2ac08aff94"
            }
          ]
        },
        {
          "id": "620441f8-671e-4657-93cd-711bacfb1ffa",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "org_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e358fb47-f41b-46e4-8196-c318b9815793"
            }
          ]
        },
        {
          "id": "83103b92-02cf-4fd0-b2fb-5a8b133921e8",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account delete ."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6663c03a-31d0-4320-8ae9-5176cee0b8ec"
            }
          ]
        },
        {
          "id": "88709e30-b5d2-4cdd-ae06-374fc69d8798",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/approve.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account approve."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0999bb05-3702-4955-8ffb-8439920a72a9"
            }
          ]
        },
        {
          "id": "763ead7d-6c4c-417b-a64d-a6422a21e105",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/change_plan.xml"
              ],
              "query": [
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account change plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61dd1915-a380-41f6-a2b2-738257c9205c"
            }
          ]
        },
        {
          "id": "ff90bccc-28b1-459c-9a6e-ef99314d5807",
          "name": "account",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/credit_card.xml"
              ],
              "query": [
                {
                  "key": "billing_address_address",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_city",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_country",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_phone",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_state",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "billing_address_zip",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_authorize_net_payment_profile_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_expiration_month",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_expiration_year",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_partial_number",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "credit_card_token",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account set credit card."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e08aab11-a867-4b8e-bb0c-60fe5c2c4413"
            }
          ]
        },
        {
          "id": "44e58c68-59ef-4a6b-9b21-33b6f44452e4",
          "name": "account1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/credit_card.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Account delete credit card."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1de9733f-936e-407a-98f3-d8e076aa0f77"
            }
          ]
        },
        {
          "id": "a4702626-b419-4d56-b29f-85f9b70746e8",
          "name": "account1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/make_pending.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account reset to pending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f816e4de-1fdc-4ef7-8e65-a54c1964179f"
            }
          ]
        },
        {
          "id": "4f1b030c-c657-490e-9660-143b914ced01",
          "name": "account2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:id/reject.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
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
            "body": {
              "mode": "raw"
            },
            "description": "Account reject."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93582291-a041-4600-9b39-eb1eb98ebc25"
            }
          ]
        },
        {
          "id": "f3257780-b835-41b3-9887-12ba11fdeca0",
          "name": "account_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/account_plans.xml?provider_key=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e12652c4-37b7-4529-a01d-d17298020470"
            }
          ]
        },
        {
          "id": "7110c1d1-ba56-4265-9a70-fc37dc79b5ca",
          "name": "account_plan",
          "request": {
            "url": "http://su1.3scale.net/admin/api/account_plans.xml?name=%7B%7D&provider_key=%7B%7D&system_name=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd9e9927-59ea-40d0-85bb-dcfba13231b4"
            }
          ]
        },
        {
          "id": "04908ab5-e00f-4b31-a018-898aa1d44f73",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Account plan feature list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eaf7ecca-b2a5-4e9d-a187-320d0ce0a929"
            }
          ]
        },
        {
          "id": "f4650c77-c611-4206-86d2-22c18ee40559",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Account plan features create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb2ed5b1-8c65-4f34-9de8-9f08cc457646"
            }
          ]
        },
        {
          "id": "bac727c7-17a3-4875-9b7f-d23feb5be537",
          "name": "account_plan_feature",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/account_plans/:account_plan_id/features/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_plan_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Account plan features delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "10aaefbb-97ef-454b-9e34-d68b5e1b55aa"
            }
          ]
        }
      ]
    },
    {
      "name": "Application",
      "item": [
        {
          "id": "e5f67908-1432-4eb3-a815-19b25da1d3a4",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a684ad9-1053-4f12-8464-c79c8cb3f993"
            }
          ]
        },
        {
          "id": "48cc41ba-c6bf-4a08-a2c5-b40a94860fef",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "31081bfe-33cc-4380-b55d-495961ae4d1a"
            }
          ]
        },
        {
          "id": "cf6b9c1d-3ee1-4916-beec-84b8fc46ea59",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application key list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7435987-deed-4246-a28d-9eed8760c6b1"
            }
          ]
        },
        {
          "id": "627bfaf0-4411-45ae-9fe5-8e5155dde5ce",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys.xml"
              ],
              "query": [
                {
                  "key": "key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application key create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3154b341-1b52-4a3c-adeb-aba38a4f3e1b"
            }
          ]
        },
        {
          "id": "5900ef3c-8d87-466e-91a8-15a0a4da512e",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/keys/:key.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "key",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Application key delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "55500760-d665-4042-9dde-0b3f80edc42b"
            }
          ]
        },
        {
          "id": "a535ddcc-28be-4588-b558-9bfbf1a7ef67",
          "name": "application1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application referrer filter list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "765ed858-d52d-4e51-b3ab-4f79712e5d11"
            }
          ]
        },
        {
          "id": "11aec24f-91ff-4529-98b6-7fe10ffdf59d",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "referrer_filter",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Application referrer filter create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "433cbbaf-28fd-4932-9d86-92cdd8766e94"
            }
          ]
        },
        {
          "id": "8ebcc4c3-2856-49a2-86f8-ea58fec29406",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:application_id/referrer_filters/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "application_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Application referrer filter delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5fd604be-b498-40cb-bc55-bb4b265da468"
            }
          ]
        },
        {
          "id": "bce7a374-cf1b-4357-af20-b25ccc3e3e6b",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Application read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2d50ca23-9a53-4160-969d-758365c5cfaf"
            }
          ]
        },
        {
          "id": "1b929af3-ff34-4ae8-912c-d2bb09087024",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "description",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "name",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cfdf86f7-c8f1-4250-a737-d85b97120d34"
            }
          ]
        },
        {
          "id": "5d75c94d-4e3d-4dc7-aebd-58ede44b7a5b",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/accept.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application accept."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "53680322-8838-41ac-b739-63ff13c69d65"
            }
          ]
        },
        {
          "id": "2a7e97dc-44d0-4660-b670-6c9061147633",
          "name": "application",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/change_plan.xml"
              ],
              "query": [
                {
                  "key": "plan_id",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application change plan."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cf2d0db-0e94-4f6e-a7ba-382d805dfa79"
            }
          ]
        },
        {
          "id": "9df0d234-305f-4081-9262-df822a68ab6e",
          "name": "application1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/customize_plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application create plan customization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfd3d816-6dd2-4f83-9916-ac1c5d37f882"
            }
          ]
        },
        {
          "id": "c4dfb88b-266a-4bd6-af23-a8c6bd6879ca",
          "name": "application2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/decustomize_plan.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application delete plan customization."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0b4aabc-a615-4ff2-a490-6d7ccdef5729"
            }
          ]
        },
        {
          "id": "d7dfbe90-bece-4d3e-9bc5-f2ab5a0c3b90",
          "name": "application3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/resume.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application resume."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b3dc52c3-93e6-4b8a-97f2-4a4f98262169"
            }
          ]
        },
        {
          "id": "525a3acc-5617-4add-8881-5e73fe1ff45c",
          "name": "application4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/applications/:id/suspend.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Application suspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2e83441f-9172-4cf5-9739-64f3dc42998a"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "7472d1ad-423f-4f36-9721-eb666316cfbb",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "role",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "state",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User list."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97727c4f-6f89-4c2f-b706-affb8632248a"
            }
          ]
        },
        {
          "id": "6384a59f-1236-4ba2-ac0f-4310ee8c2f1c",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "User create."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2053dcc-c458-441f-a6fb-e0fc78a051b2"
            }
          ]
        },
        {
          "id": "305073d1-1dbe-4ec3-afc8-d6571fc813b9",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "User read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8b1add18-ecdb-44bf-83ce-5349b1fb181c"
            }
          ]
        },
        {
          "id": "2db49b6e-7e2e-4111-857c-3c8e720a2ac2",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "additional_fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "email",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "password",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "username",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User update."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fc2a4fa-e41e-4421-b4b8-3d754c709eb5"
            }
          ]
        },
        {
          "id": "c50e5773-1c63-48cb-9e25-45cd7a34db92",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "User delete."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5599c39-50e9-4851-a8fd-09229b34e125"
            }
          ]
        },
        {
          "id": "526378d7-9a86-4647-9166-cce0234a4518",
          "name": "user",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/activate.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User activate."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4e93247-6feb-4afd-b9c5-3e6ea865915d"
            }
          ]
        },
        {
          "id": "98bb65f2-7aeb-4ff5-b3c5-6cf60caf0bc5",
          "name": "user1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/admin.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User change role to admin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d46ed099-be82-4efe-9a4c-2c7c7464d5b8"
            }
          ]
        },
        {
          "id": "79c0e275-d04f-4578-a183-c549240aeb01",
          "name": "user2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/member.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User change role to member."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3cdc46af-e8cf-45ae-af0f-c675b8b879c4"
            }
          ]
        },
        {
          "id": "18b00b08-ff46-43d0-a601-2f654dc0b535",
          "name": "user3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/suspend.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User suspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03776e3d-e86e-42f5-b022-9baa0de44114"
            }
          ]
        },
        {
          "id": "7578abe4-2bb6-4f20-b077-56af65114ac5",
          "name": "user4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "su1.3scale.net",
              "path": [
                "admin/api/accounts/:account_id/users/:id/unsuspend.xml"
              ],
              "query": [
                {
                  "key": "provider_key",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "account_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "User unsuspend."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "91323bc6-ff80-4d0e-b6a4-33390fd92f45"
            }
          ]
        }
      ]
    }
  ]
}