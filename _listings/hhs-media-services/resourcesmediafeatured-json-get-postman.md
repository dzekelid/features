{
  "info": {
    "name": "HHS Media Services Get the list of featured content in the syndication system",
    "_postman_id": "421ac4e3-9b86-4689-a651-7cd4ef334e1d",
    "description": "Get the list of featured content in the syndication system",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Resources",
      "item": [
        {
          "id": "3e27bc8b-f767-47e7-b10d-1da80667a77f",
          "name": "getFeaturedMedia",
          "request": {
            "url": "http://api.digitalmedia.hhs.gov/api/v2/resources/media/featured.json?max=%7B%7D&offset=%7B%7D&sort=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of featured content in the syndication system"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd7b18d8-e0a0-4fd9-876a-5f1d0a8a3048"
            }
          ]
        }
      ]
    }
  ]
}