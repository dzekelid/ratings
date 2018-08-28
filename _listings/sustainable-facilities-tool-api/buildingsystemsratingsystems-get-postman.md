{
  "info": {
    "name": "Sustainable Facilities Tool API Building System Rating Systems",
    "_postman_id": "ee85e1d2-5f89-431c-8bdf-dac9823f2f3d",
    "description": "Returns all building system rating systems",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Building Systems",
      "item": [
        {
          "id": "9b3fbfcd-29e1-405c-9be7-c9809cdd097c",
          "name": "returnBuildingSystems",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building systems."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e7de5398-f548-40eb-8d10-4830b2158be4"
            }
          ]
        },
        {
          "id": "bb2d2d72-2b0e-4de3-babf-7924195770be",
          "name": "returnBuildingSystem",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a building system by parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "327e6bcb-5268-46de-9ac0-de2e7917d72f"
            }
          ]
        }
      ]
    },
    {
      "name": "Building System Resources",
      "item": [
        {
          "id": "da3d092f-dc77-4a04-a99f-928df6892ffc",
          "name": "returnBuildingSystemResources",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/resources"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns informational resources for the building system selected by parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "858627e0-0cbd-4ee5-8c60-c0373da70461"
            }
          ]
        }
      ]
    },
    {
      "name": "Case Studies",
      "item": [
        {
          "id": "46af0296-08f5-4918-b7fb-ea123cfda731",
          "name": "returnBuildingSystemCaseStudies",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems/case-studies",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building systems case studies"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "83a74e34-c8b1-422d-9c97-e02a76b57856"
            }
          ]
        },
        {
          "id": "c3ff0e6a-164d-49ac-af09-bcfc46caa329",
          "name": "returnBuildingSystemCaseStudies1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/case-studies"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a building system case study by parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d06ad57-d202-49f5-99ac-fffbb9cb0fbd"
            }
          ]
        }
      ]
    },
    {
      "name": "Mandates",
      "item": [
        {
          "id": "2620c06c-4242-4ec8-9bd5-71b9f5ab6f24",
          "name": "returnBuildingSystemMandates",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems/mandates",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building systems mandates"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb13f69d-64bd-4d39-acca-8f77df3b3e72"
            }
          ]
        },
        {
          "id": "426b0119-69d3-4ff0-ba60-01a2b79a5b34",
          "name": "returnBuildingSystemMandate",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.data.gov",
              "path": [
                "sftool",
                "v1",
                "building-systems/:parameter/mandates"
              ],
              "variable": [
                {
                  "id": "parameter",
                  "value": "parameter",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a building system mandate by parameter."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e018c7d8-a260-4cae-8c8d-4887c58984b0"
            }
          ]
        }
      ]
    },
    {
      "name": "Rating Systems",
      "item": [
        {
          "id": "c4c1ed74-f32e-4d07-b7ba-24e0165e54a4",
          "name": "returnBuildingSystemRating",
          "request": {
            "url": "http://api.data.gov/sftool/v1/building-systems/rating-systems",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all building system rating systems"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a43e9857-3a49-40a6-9776-64c009f42a37"
            }
          ]
        }
      ]
    }
  ]
}