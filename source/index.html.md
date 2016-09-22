---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# AnswerOption

## presigns an upload


### Request

#### Endpoint

```
GET /v2/answer_options/images/cache/presign

```

`GET /v2/answer_options/images/cache/presign`

#### Parameters


None known.


### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/9dc8b12a7123b0e8742b2f17db96cbee",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOS0yMlQwOTowNToyOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS85ZGM4YjEyYTcxMjNiMGU4NzQyYjJmMTdkYjk2Y2JlZSJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwOTIyL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDkyMlQwODA1MjlaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160922/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160922T080529Z",
    "x-amz-signature": "7c11f6e939584b07d730193463ad6ac271e156d03b9d30fe1403ddb2bf5e8b70"
  }
}
```



```shell
curl "api.goskive.com/v2/answer_options/images/cache/presign" -X GET 
```
# Authentication

## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OGRhMDI0NjFiOTc2N2IyYjgxZDk0YWE2NjZiYjhkNmExNjJkOGY1ODBmYmM1
ZGQ4MTcxM2UyMmMwNTZkM2RlMTplNDIyMzA2OGM4MjY3YWM0MGFhZTAwMzI4
ODQyZTgxNWY1M2Y2MDgyYzE5N2YzM2RjYTcyYzM3YWFhYzRjZTA5

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 8da02461b9767b2b81d94aa666bb8d6a162d8f580fbc5dd81713e22c056d3de1:e4223068c8267ac40aae00328842e815f53f6082c197f33dca72c37aaac4ce09
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YWNkZDBmMjc3MWViMTNmM2NiNWI3MDc3NDdjYjMwNDlmZDlkNmYwNmE1NTI5
OTJiYjBkOGNhMjBmYjUxZTE5ZjplNmZmYjVmMzE5NjNlMjY5NDVhNmU5MDdl
MjRhYzg5YTQ4ODU0ZGQxMjJjYWRlNTdlMWYyYmQzZGNjNTQyZDc2

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd"}' -X POST \
	-H "Content-Type: application/json" \
	-u acdd0f2771eb13f3cb5b707747cb3049fd9d6f06a552992bb0d8ca20fb51e19f:e6ffb5f31963e26945a6e907e24ac89a48854dd122cade57e1f2bd3dcc542d76
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9fbfe56987fd9c8df8bda8611aba15d58bc15ffa1e24b7b23516064f63ddfea2","client_secret":"70e2bc65d27eb567c04e2d6a8f1150be53f95faae25fb0a07654dbd685fe959d"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9fbfe56987fd9c8df8bda8611aba15d58bc15ffa1e24b7b23516064f63ddfea2","client_secret":"70e2bc65d27eb567c04e2d6a8f1150be53f95faae25fb0a07654dbd685fe959d"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"4d270da891259c51aafc05a6cdcca54e3e10c18c692d2463b7956c0d63a611c2","client_secret":"e41cd663ed9d8e0ab5c4181dd86647f18aebe13658fe0a0edeb09c3187b3b13b"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"4d270da891259c51aafc05a6cdcca54e3e10c18c692d2463b7956c0d63a611c2","client_secret":"e41cd663ed9d8e0ab5c4181dd86647f18aebe13658fe0a0edeb09c3187b3b13b"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"client_credentials","client_id":"a84a49d83cc6b36eabacbab927f759a8ec4d7620720affb85a9b649b4c44f1e5","client_secret":"688267334a14d68e360f1fe2146f08c345d9bdccd392d9944cf3983315253bac"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| client_id *required* | Client ID |
| client_secret *required* | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "bdbf302ad6bf01a927e745d57350162e82f3a94a4ba72a967dda15c133c9db38",
  "token_type": "bearer",
  "created_at": 1474531481
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"a84a49d83cc6b36eabacbab927f759a8ec4d7620720affb85a9b649b4c44f1e5","client_secret":"688267334a14d68e360f1fe2146f08c345d9bdccd392d9944cf3983315253bac"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ODRlM2I3MjBkMDUyNGZjZTg3NjE4YjNkYjQxOGVlZWIxYmNiOGU1YjA5ZWVi
MTY1ZjEyMGMwYzgwOGVlYTc5YjowODI4OTZkYTgyZTFjNjkyNzZjMTJmODFi
MGE2MTZhZDlmZGNkMWEzM2RjNWI1NjgwM2UxNmZmZDNmYzEzZWI0

```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "bda50d8f5429c0621214aad1b51df6aef0ca3e55edbc862ecfbc775e3e8bd9c7",
  "token_type": "bearer",
  "created_at": 1474531482
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 84e3b720d0524fce87618b3db418eeeb1bcb8e5b09eeb165f120c0c808eea79b:082896da82e1c69276c12f81b0a616ad9fdcd1a33dc5b56803e16ffd3fc13eb4
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"abe334f8f572eaa84f96ecdadcce0e615cfc26c0f50f657bb58808069fb53c4b","client_secret":"cee9c644125e8280868deaa13e9010c6b291693c4e51c7077643af192a184dc2"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "access_token": "a9da564a1bd859d995c54292121a5355927ce6ce264f67e42e1b97e75ebddf88",
  "token_type": "bearer",
  "created_at": 1474531483
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"abe334f8f572eaa84f96ecdadcce0e615cfc26c0f50f657bb58808069fb53c4b","client_secret":"cee9c644125e8280868deaa13e9010c6b291693c4e51c7077643af192a184dc2"}' -X POST \
	-H "Content-Type: application/json"
```
## Validation error on create

A missing `client_id` gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| grant_type *required* | Grant type |
| scope  | Scope |
| username *required* | Username |
| password *required* | Password |
| client_id  | Client ID |
| client_secret  | Client Secret |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "validation_failed",
      "error_description": "Validation failed: Application can't be blank"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json"
```
# Campaigns

## Get a campaign


### Request

#### Endpoint

```
GET /v2/campaigns/9
Content-Type: application/json
Authorization: Bearer d1f59b40e8371173c5156eedcf1e203fbac0924cef9973baf2e2d4a4ed4ca69a
```

`GET /v2/campaigns/:campaign_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaign": {
    "id": 9,
    "title": "Recruiting pastry chefs",
    "company_id": 23,
    "precluded_campaign_ids": [

    ],
    "company_profiles": [

    ],
    "banners": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/campaigns/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1f59b40e8371173c5156eedcf1e203fbac0924cef9973baf2e2d4a4ed4ca69a"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer 61fa8ddfce9ae2c361d6fe46bcd4ba159d66a92e4dd8300dfbb01432541b3a69
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":194,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 94,
    "obfuscated_id": "CVi6VU_nV6k",
    "author_id": 920,
    "chapter_id": 194,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:36.619Z",
    "created_at": "2016-09-22T08:05:36.619Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/194/flashcards" -d '{"flashcard":{"chapter_id":194,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61fa8ddfce9ae2c361d6fe46bcd4ba159d66a92e4dd8300dfbb01432541b3a69"
```
## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/195/flashcards
Content-Type: application/json
Authorization: Bearer 30c9deb70603daec4e7dd1ef1ee51fa52495f61048024c2513845dc22ca95ba7
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":195,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 95,
    "obfuscated_id": "uTOhBSQK4CI",
    "author_id": 923,
    "chapter_id": 195,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:37.033Z",
    "created_at": "2016-09-22T08:05:37.033Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "",
    "back_content": "",
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/195/flashcards" -d '{"flashcard":{"chapter_id":195,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30c9deb70603daec4e7dd1ef1ee51fa52495f61048024c2513845dc22ca95ba7"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/193/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 76a59d0547a09105146dc76a39ef4e2a2702296025077125fa7f48ba44b139df
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

193
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

fr
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "flashcard": {
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 917,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:36.196Z",
    "created_at": "2016-09-22T08:05:36.196Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/285c2f0c06d4f257300a3ae90dfbcf4aa5c5c8ff.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/ca61b237ad1a84ddf291b8adcfea3ecc38723a34.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/285c2f0c06d4f257300a3ae90dfbcf4aa5c5c8ff.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/ca61b237ad1a84ddf291b8adcfea3ecc38723a34.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/193/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

193
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

fr
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X POST \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 76a59d0547a09105146dc76a39ef4e2a2702296025077125fa7f48ba44b139df"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/192/flashcards
Content-Type: application/json
Authorization: Bearer 24c7cc119fcea82fe67f796ebda16317dbfb969fbd1abbf56d525c6c0a8b797d
```

`GET /v2/chapters/:chapter_id/flashcards`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcards": [
    {
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 912,
      "chapter_id": 192,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:35.584Z",
      "created_at": "2016-09-22T08:05:35.584Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 912,
      "chapter_id": 192,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:35.620Z",
      "created_at": "2016-09-22T08:05:35.620Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 912,
      "chapter_id": 192,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:35.657Z",
      "created_at": "2016-09-22T08:05:35.657Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/192/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24c7cc119fcea82fe67f796ebda16317dbfb969fbd1abbf56d525c6c0a8b797d"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/125/questions
Content-Type: application/json
Authorization: Bearer 819ff18f9f9d04340c03e1d3e1c0cb659a732ba1dfd747c8fb4388d1fb6ca594
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":125,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 81,
    "obfuscated_id": "jHF1owx40fU",
    "author_id": 595,
    "chapter_id": 125,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:08.978Z",
    "created_at": "2016-09-22T08:05:08.978Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": true,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 162,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 163,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 164,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 165,
        "position": 4,
        "content": "Eggs",
        "content_html": "<p>Eggs</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/125/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":125,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 819ff18f9f9d04340c03e1d3e1c0cb659a732ba1dfd747c8fb4388d1fb6ca594"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/126/questions
Content-Type: application/json
Authorization: Bearer 6cb771b322da726653c8a368d85dee371687cd4ecbee95ae3b122f786695303f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":126,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 82,
    "obfuscated_id": "D5TJ6kac5FE",
    "author_id": 598,
    "chapter_id": 126,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:09.483Z",
    "created_at": "2016-09-22T08:05:09.483Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": null,
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 166,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 167,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/126/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":126,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cb771b322da726653c8a368d85dee371687cd4ecbee95ae3b122f786695303f"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/127/questions
Content-Type: application/json
Authorization: Bearer c1add6dfb703a18f6d23e6c4494b326e906a6b16e19376b0083e4c850f6ccdc1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":127,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 83,
    "obfuscated_id": "FCSR-nKROLo",
    "author_id": 601,
    "chapter_id": 127,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:09.828Z",
    "created_at": "2016-09-22T08:05:09.828Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How do you make **Choux**?",
    "question_html": "How do you make <strong>Choux</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "the explanation is simple: **eggs**",
    "explanation_html": "the explanation is simple: <strong>eggs</strong>",
    "answer_options": [
      {
        "id": 168,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 169,
        "position": 2,
        "content": "Flour and eggs",
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/127/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":127,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1add6dfb703a18f6d23e6c4494b326e906a6b16e19376b0083e4c850f6ccdc1"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/128/questions
Content-Type: application/json
Authorization: Bearer 3a887e40ddfb822f03f75091e41e6bdd5c8e8ccde1940d33e0bca37f3aa7bb45
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":128,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question_html] *required* | Question HTML |
| question[explanation_html] *required* | Explanation HTML |
| question[question]  | Question Markdown |
| question[explanation]  | Explanation Markdown |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options]  | Answer Options |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "question": {
    "id": 84,
    "obfuscated_id": "Hu6DTUHzhWo",
    "author_id": 604,
    "chapter_id": 128,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:05:10.199Z",
    "created_at": "2016-09-22T08:05:10.199Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "de",
    "question": "How many Germans does it take to change a light bulb?",
    "question_html": "How many Germans does it take to change a <strong>light bulb</strong>?",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Think about German humor.",
    "explanation_html": "Think about German <strong>humor</strong>",
    "answer_options": [
      {
        "id": 170,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 171,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 172,
        "position": 3,
        "content": "Two. One that changes it and one that makes this joke work.",
        "content_html": "<p>Two. One that changes it and one that makes this joke work.</p>",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/128/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":128,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a887e40ddfb822f03f75091e41e6bdd5c8e8ccde1940d33e0bca37f3aa7bb45"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/130/questions
Content-Type: application/json
Authorization: Bearer d52b0d7f7ea7cfbe9aae08c240d4957e588daaf2c986e0c19f2fbdf1c4876361
```

`GET /v2/chapters/:chapter_id/questions`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "questions": [
    {
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 610,
      "chapter_id": 130,
      "position": 72,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:10.850Z",
      "created_at": "2016-09-22T08:05:10.734Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 173,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 174,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 86,
      "obfuscated_id": "7q-2LHZR3Kk",
      "author_id": 611,
      "chapter_id": 130,
      "position": 73,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:11.041Z",
      "created_at": "2016-09-22T08:05:10.923Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 175,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 176,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 612,
      "chapter_id": 130,
      "position": 74,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:05:11.236Z",
      "created_at": "2016-09-22T08:05:11.116Z",
      "tags": [

      ],
      "status": "published",
      "published": true,
      "language_code": "de",
      "question": "Clever example question: why did the rspec test not pass?",
      "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
      "shuffle_answers": true,
      "multiple_choice": false,
      "explanation": "This could never explain why it didn't pass. Maybe it did?",
      "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
      "answer_options": [
        {
          "id": 177,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 178,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/130/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d52b0d7f7ea7cfbe9aae08c240d4957e588daaf2c986e0c19f2fbdf1c4876361"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/28
Content-Type: application/json
Authorization: Bearer bcf6ed1f94bdcf3e21f5d10144e23da3b64187877c8992a4f0e3adef676c84d4
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/28" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcf6ed1f94bdcf3e21f5d10144e23da3b64187877c8992a4f0e3adef676c84d4"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/31
Content-Type: application/json
Authorization: Bearer b410d8a5edad0553b101ec8c77d3402cf3fd244260e605beb352e8f0274db950
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/31" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b410d8a5edad0553b101ec8c77d3402cf3fd244260e605beb352e8f0274db950"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/33
Content-Type: application/json
Authorization: Bearer b0f487ec66ad141158d2665bfa2028305ec4858d4fd2d5ccb93a7b9e245b3d15
```

`PATCH /v2/chapters/:chapter_id`

#### Parameters


```json
{"chapter":{"title":"Eggs and Flour"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title]  | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/33" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0f487ec66ad141158d2665bfa2028305ec4858d4fd2d5ccb93a7b9e245b3d15"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/29
Content-Type: application/json
Authorization: Bearer ed7ef0c778e0d8895e1c8a83c045f55c7b71f0c69646bcca78533bf6999db3c0
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/29" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed7ef0c778e0d8895e1c8a83c045f55c7b71f0c69646bcca78533bf6999db3c0"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/27
Content-Type: application/json
Authorization: Bearer 05caeb4c2533da88a21539be040d61e174021434f02a6195fd06c52bce3e9b67
```

`GET /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapter": {
    "id": 27,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-22T08:04:18.463Z",
    "course_id": 27,
    "author_id": 95,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-09-22T08:04:17.934Z",
    "questions_updated_at": "2016-09-22T08:04:17.934Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 99,
        "chapter_id": 27,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:18.446Z",
        "created_at": "2016-09-22T08:04:18.446Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      }
    ],
    "questions": [
      {
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 97,
        "chapter_id": 27,
        "position": 8,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:18.338Z",
        "created_at": "2016-09-22T08:04:18.222Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 15,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 16,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05caeb4c2533da88a21539be040d61e174021434f02a6195fd06c52bce3e9b67"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/32
Content-Type: application/json
Authorization: Bearer cffd2be044d1c575af1048e7ceb1577cd8fbf60219058ff79c85c14123ea5ba0
```

`PATCH /v2/chapters/:chapter_id`

#### Parameters


```json
{"chapter":{"title":"Eggs and Flour"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title]  | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapter": {
    "id": 32,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-22T08:04:19.673Z",
    "course_id": 32,
    "author_id": 114,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": null,
    "questions_updated_at": null,
    "flashcards_count": 0,
    "questions_count": 0,
    "flashcards": [

    ],
    "questions": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/32" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cffd2be044d1c575af1048e7ceb1577cd8fbf60219058ff79c85c14123ea5ba0"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/45/replies
Content-Type: application/json
Authorization: Bearer fb3c3ba6d427f3319ab6777a1db851669183cd937fdbcdf09abb974d5bf8c998
```

`POST /v2/comments/:comment_id/replies`

#### Parameters


```json
{"comment":{"message":"Just keeping the thread alive!"}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 46,
    "author_id": 542,
    "reply_to_id": 45,
    "created_at": "2016-09-22T08:05:04.106Z",
    "status": "published",
    "message": "Just keeping the thread alive!",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |


```shell
curl "api.goskive.com/v2/comments/45/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb3c3ba6d427f3319ab6777a1db851669183cd937fdbcdf09abb974d5bf8c998"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/44/replies
Content-Type: application/json
Authorization: Bearer 2065c841a3eb8f1eca09f1c9f4345ea9547e9983241d205774a40041f5d6682c
```

`POST /v2/comments/:comment_id/replies`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |


```shell
curl "api.goskive.com/v2/comments/44/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2065c841a3eb8f1eca09f1c9f4345ea9547e9983241d205774a40041f5d6682c"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer 6ea999e4088a7f3abacf89cb2a41f2280ddc92c56e3d8f9f579c84ac2977d366
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ea999e4088a7f3abacf89cb2a41f2280ddc92c56e3d8f9f579c84ac2977d366"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/7/republish
Content-Type: application/json
Authorization: Bearer daaf5f46e9e8721b3784164b22347c45a636cdbb3a0163afaf481ea14df5a4ac
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments/7/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daaf5f46e9e8721b3784164b22347c45a636cdbb3a0163afaf481ea14df5a4ac"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer 6f7a8e1370d459b6815b79ab419458b2fcf18c7618d4fe46989ae2ddb6bd7e3a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f7a8e1370d459b6815b79ab419458b2fcf18c7618d4fe46989ae2ddb6bd7e3a"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/8/report
Content-Type: application/json
Authorization: Bearer 728bba0a191a54dbdbdf61dc4c89381e4f01c9b3be5acb3b5c5c5e7aded6d02a
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 728bba0a191a54dbdbdf61dc4c89381e4f01c9b3be5acb3b5c5c5e7aded6d02a"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/16
Content-Type: application/json
Authorization: Bearer e4e5ea243dc50cf48a8b6743140caac08cd8a3160d409e4c4b8d18a71ba1f570
```

`GET /v2/companies/:company_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company": {
    "id": 16,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-09-22T08:04:41.091Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4e5ea243dc50cf48a8b6743140caac08cd8a3160d409e4c4b8d18a71ba1f570"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 3bdb49931852d22210f25317b3aee3dcbc4d4a68c20190dd05afacd297a60cad
```

`GET /v2/companies`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "companies": [
    {
      "id": 17,
      "name": "Fake Company Name 16",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-22T08:04:41.172Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 17",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-22T08:04:41.177Z"
    },
    {
      "id": 19,
      "name": "Fake Company Name 18",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
      "brand_color": "#000000",
      "updated_at": "2016-09-22T08:04:41.181Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bdb49931852d22210f25317b3aee3dcbc4d4a68c20190dd05afacd297a60cad"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/21/company_profiles
Content-Type: application/json
Authorization: Bearer 59f4489cae145eb81ada5834de55ab169f6f55a68c6cc73561c842886ff48eb6
```

`GET /v2/companies/:company_id/company_profiles`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company_profiles": [
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 9,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/87f24f1d1c22af87a4c49901ca6db1d9205da6e7.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/c88539f34738a470d3868a5d08c1e5a58443cdb0.png",
      "widgets": [

      ]
    },
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 8,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/4e8ccb4fdbb03332710724b7199bfb925ebb8588.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/1751c1fcb04de04c20e97d74547e239755abd978.png",
      "widgets": [

      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/21/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59f4489cae145eb81ada5834de55ab169f6f55a68c6cc73561c842886ff48eb6"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/20/company_profiles
Content-Type: application/json
Authorization: Bearer 1ce80d23a40adc6dfa774f64dac9c8eb2de6d004870cb460447c505ad9d79b8b
```

`GET /v2/companies/:company_id/company_profiles`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "company_profiles": [
    {
      "country_codes": [
        "DE",
        "EN"
      ],
      "language_code": "en",
      "id": 5,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/43cd8331a2a1101475dca8b52baf14565bda8d25.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/36ab23184d8eb9448413fbe09f112b2034c6db2d.png",
      "widgets": [
        {
          "id": 1,
          "type": "twitter",
          "prompt": "Check us out on Twitter",
          "username": "SkiveApp",
          "fallback_url": "https://goskive.com"
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/20/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ce80d23a40adc6dfa774f64dac9c8eb2de6d004870cb460447c505ad9d79b8b"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer a7add0cb6b8a9ecd436a4120e00a50396490be2c9b7a69d598ee782cbb84552d
```

`GET /v2/courses/:course_slug/campaigns`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaigns": [
    {
      "id": 5,
      "title": "Campaign 5",
      "company_id": 7,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 3,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/3e3de85f9259343d03d531c0557570e70612c274.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9df145d07eb8d34190b3b56db5884a14a6e7644c.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/69ad62d43dc80a20595b9668db2a008bef68d956.png",
          "target_url": "http://goskive.com",
          "id": 3,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 8,
      "title": "Campaign 8",
      "company_id": 10,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 4,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/b7227ba08020eaf424f385a68712e11390fe76a3.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/15a47e0f0d046fb9c95772f170325321f8fb4d6d.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/4d6ffc06ecfb9d946ae4017c7ee02d2794b0b313.png",
          "target_url": "http://goskive.com",
          "id": 4,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7add0cb6b8a9ecd436a4120e00a50396490be2c9b7a69d598ee782cbb84552d"
```
# Course Chapters

## Authorisation error on create

A student may not create a chapter in an unpublished
            course.

### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9aa939812883a0a637a4150894dea8c6ed3999662bc8b48d689c8b78170a595d
```

`POST /v2/courses/:course_slug/chapters`

#### Parameters


```json
{"chapter":{"title":"Preparing the oven"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title] *required* | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9aa939812883a0a637a4150894dea8c6ed3999662bc8b48d689c8b78170a595d"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e30b0223bfedaefd02e4126cb4733c3edb0dabc7f3162e23ef6baca53e4475a1
```

`POST /v2/courses/:course_slug/chapters`

#### Parameters


```json
{"chapter":{"title":"Preparing the oven"}}
```


| Name | Description |
|:-----|:------------|
| chapter[title] *required* | Chapter title |
| chapter[position]  | Position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "chapter": {
    "id": 1,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-22T08:04:11.820Z",
    "course_id": 1,
    "author_id": 2,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": null,
    "questions_updated_at": null,
    "flashcards_count": 0,
    "questions_count": 0,
    "flashcards": [

    ],
    "questions": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e30b0223bfedaefd02e4126cb4733c3edb0dabc7f3162e23ef6baca53e4475a1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 7,
      "title": "Clever Chapter Title 4",
      "position": 1,
      "updated_at": "2016-09-22T08:04:12.707Z",
      "course_id": 7,
      "author_id": 17,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 8,
      "title": "Clever Chapter Title 5",
      "position": 2,
      "updated_at": "2016-09-22T08:04:12.734Z",
      "course_id": 7,
      "author_id": 18,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 9,
      "title": "Clever Chapter Title 6",
      "position": 3,
      "updated_at": "2016-09-22T08:04:13.070Z",
      "course_id": 7,
      "author_id": 19,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-09-22T08:04:12.629Z",
      "questions_updated_at": "2016-09-22T08:04:12.629Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c266e588f4fbefc9a160d289f616886d7b7f2058b17d238f128b35897f6d724d
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 19,
      "title": "Clever Chapter Title 16",
      "position": 1,
      "updated_at": "2016-09-22T08:04:14.160Z",
      "course_id": 13,
      "author_id": 42,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 20,
      "title": "Clever Chapter Title 17",
      "position": 2,
      "updated_at": "2016-09-22T08:04:14.186Z",
      "course_id": 13,
      "author_id": 43,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 21,
      "title": "Clever Chapter Title 18",
      "position": 3,
      "updated_at": "2016-09-22T08:04:14.438Z",
      "course_id": 13,
      "author_id": 44,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-09-22T08:04:14.082Z",
      "questions_updated_at": "2016-09-22T08:04:14.082Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c266e588f4fbefc9a160d289f616886d7b7f2058b17d238f128b35897f6d724d"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 10,
      "title": "Clever Chapter Title 7",
      "position": 1,
      "updated_at": "2016-09-22T08:04:13.266Z",
      "course_id": 9,
      "author_id": 24,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 11,
      "title": "Clever Chapter Title 8",
      "position": 2,
      "updated_at": "2016-09-22T08:04:13.291Z",
      "course_id": 9,
      "author_id": 25,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 12,
      "title": "Clever Chapter Title 9",
      "position": 3,
      "updated_at": "2016-09-22T08:04:13.317Z",
      "course_id": 9,
      "author_id": 26,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 95a6b240276a79c4037168d67fe8bddd4dfb600866706021584622e08198f563
```

`GET /v2/courses/:course_slug/chapters`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "chapters": [
    {
      "id": 22,
      "title": "Clever Chapter Title 19",
      "position": 1,
      "updated_at": "2016-09-22T08:04:14.592Z",
      "course_id": 14,
      "author_id": 49,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 23,
      "title": "Clever Chapter Title 20",
      "position": 2,
      "updated_at": "2016-09-22T08:04:14.617Z",
      "course_id": 14,
      "author_id": 50,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 24,
      "title": "Clever Chapter Title 21",
      "position": 3,
      "updated_at": "2016-09-22T08:04:14.667Z",
      "course_id": 14,
      "author_id": 51,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95a6b240276a79c4037168d67fe8bddd4dfb600866706021584622e08198f563"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer fb24f0af0c0c35008c0b34cd141e5a8c0e5d7839829924fee5673b4dccc4a044
```

`POST /v2/courses/:course_slug/course_requests`

#### Parameters


```json
{}
```

None known.


### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "course_request": {
    "id": 6,
    "course_id": 21,
    "user_id": 70,
    "updated_at": "2016-09-22T08:04:15.787Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb24f0af0c0c35008c0b34cd141e5a8c0e5d7839829924fee5673b4dccc4a044"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d2da571a1e977a2e54d3620567f4e2d67746e3a7a73d378b2c9ecfbdeba05ad9
```

`GET /v2/courses/:course_slug/course_requests`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course_requests": [
    {
      "id": 1,
      "course_id": 17,
      "user_id": 58,
      "updated_at": "2016-09-22T08:04:15.125Z"
    },
    {
      "id": 2,
      "course_id": 17,
      "user_id": 59,
      "updated_at": "2016-09-22T08:04:15.143Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2da571a1e977a2e54d3620567f4e2d67746e3a7a73d378b2c9ecfbdeba05ad9"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 283d3803db3a796c7cf712db946fbf0a9dab89053829870acfe0bf7b517c9125
```

`DELETE /v2/course_requests/:course_request_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/course_requests/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 283d3803db3a796c7cf712db946fbf0a9dab89053829870acfe0bf7b517c9125"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8eaf65e79493dd73b875f1add308c1894e7aa197ccfae2961c2d274dc23934f5
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8eaf65e79493dd73b875f1add308c1894e7aa197ccfae2961c2d274dc23934f5"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 92da23a852e9d3460493ad9ef9cfeeee1721fcf299d27e6b59440d13f6cef1d8
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92da23a852e9d3460493ad9ef9cfeeee1721fcf299d27e6b59440d13f6cef1d8"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0a97280275a728ebf2243f119512e29b937219a560c00a1ce184134903a71f6a
```

`PATCH /v2/courses/:course_slug`

#### Parameters


```json
{"course":{"title":"Choux pastry 102","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| course[title]  | Title |
| course[topic_id]  | Topic ID |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |



### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a97280275a728ebf2243f119512e29b937219a560c00a1ce184134903a71f6a"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a9c815e4287e0a4e900165f91051a3230d136bf26c7bc4b790598af4fda65b54
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9c815e4287e0a4e900165f91051a3230d136bf26c7bc4b790598af4fda65b54"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions
Content-Type: application/json
Authorization: 
```

`GET /v2/courses/:course_slug`

#### Parameters


```json
include: questions
```


| Name | Description |
|:-----|:------------|
| include  | optional resources to embed |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 161,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 49,
    "additional_university_ids": [

    ],
    "topic_id": 54,
    "discipline_id": 54,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 2,
    "questions_count": 2,
    "users_count": 0,
    "user_generated": false,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": true,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-22T08:04:25.513Z",
    "updated_at": "2016-09-22T08:04:27.072Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 40,
        "title": "Clever Chapter Title 28",
        "position": 1,
        "updated_at": "2016-09-22T08:04:27.019Z",
        "course_id": 49,
        "author_id": 161,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-22T08:04:25.513Z",
        "questions_updated_at": "2016-09-22T08:04:25.513Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 41,
        "title": "Clever Chapter Title 29",
        "position": 2,
        "updated_at": "2016-09-22T08:04:27.063Z",
        "course_id": 49,
        "author_id": 161,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-22T08:04:25.513Z",
        "questions_updated_at": "2016-09-22T08:04:25.513Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 161,
        "chapter_id": 40,
        "position": 20,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:25.733Z",
        "created_at": "2016-09-22T08:04:25.607Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 39,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 40,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 161,
        "chapter_id": 41,
        "position": 22,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:26.133Z",
        "created_at": "2016-09-22T08:04:26.003Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 43,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 44,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 951d9767c10900e9ff987a37ce285c161e4a344b5c2e98692b186ab632e076c4
```

`GET /v2/courses/:course_slug`

#### Parameters


```json
include: questions, flashcards
```


| Name | Description |
|:-----|:------------|
| include  | optional resources to embed |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 166,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 50,
    "additional_university_ids": [

    ],
    "topic_id": 55,
    "discipline_id": 55,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 4,
    "questions_count": 4,
    "users_count": 0,
    "user_generated": false,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": true,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-22T08:04:27.133Z",
    "updated_at": "2016-09-22T08:04:28.621Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 42,
        "title": "Clever Chapter Title 30",
        "position": 1,
        "updated_at": "2016-09-22T08:04:28.574Z",
        "course_id": 50,
        "author_id": 166,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-22T08:04:27.133Z",
        "questions_updated_at": "2016-09-22T08:04:27.133Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 43,
        "title": "Clever Chapter Title 31",
        "position": 2,
        "updated_at": "2016-09-22T08:04:28.614Z",
        "course_id": 50,
        "author_id": 166,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-09-22T08:04:27.133Z",
        "questions_updated_at": "2016-09-22T08:04:27.133Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 167,
        "chapter_id": 42,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:28.407Z",
        "created_at": "2016-09-22T08:04:28.407Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 167,
        "chapter_id": 43,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:28.486Z",
        "created_at": "2016-09-22T08:04:28.486Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 167,
        "chapter_id": 42,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:28.452Z",
        "created_at": "2016-09-22T08:04:28.452Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 167,
        "chapter_id": 43,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:28.524Z",
        "created_at": "2016-09-22T08:04:28.524Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      }
    ],
    "questions": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 167,
        "chapter_id": 42,
        "position": 26,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:27.375Z",
        "created_at": "2016-09-22T08:04:27.241Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 167,
        "chapter_id": 42,
        "position": 27,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:27.560Z",
        "created_at": "2016-09-22T08:04:27.437Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 53,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 54,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 167,
        "chapter_id": 43,
        "position": 28,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:27.770Z",
        "created_at": "2016-09-22T08:04:27.649Z",
        "tags": [

        ],
        "status": "published",
        "published": true,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 55,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 56,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 167,
        "chapter_id": 43,
        "position": 29,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:27.942Z",
        "created_at": "2016-09-22T08:04:27.831Z",
        "tags": [

        ],
        "status": "draft",
        "published": false,
        "language_code": "de",
        "question": "Clever example question: why did the rspec test not pass?",
        "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
        "shuffle_answers": true,
        "multiple_choice": false,
        "explanation": "This could never explain why it didn't pass. Maybe it did?",
        "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
        "answer_options": [
          {
            "id": 57,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 58,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 951d9767c10900e9ff987a37ce285c161e4a344b5c2e98692b186ab632e076c4"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/47/pin
Content-Type: application/json
Authorization: Bearer 9b339d85358db7db9f7d211a57bd51a69f4534c7fd81de2e010b52b7026dfda5
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/47/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b339d85358db7db9f7d211a57bd51a69f4534c7fd81de2e010b52b7026dfda5"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/46/pin
Content-Type: application/json
Authorization: Bearer 90e7b7545cbd0f0d1553c50ed56408cb8936d6a38587b960fd8f37153193759f
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/46/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90e7b7545cbd0f0d1553c50ed56408cb8936d6a38587b960fd8f37153193759f"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 80f54e9320004ee3e6328cb6fcabacf6de4e17464ae6354c717f9bf0c4f70ca2
```

`PATCH /v2/courses/:course_slug`

#### Parameters


```json
{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}
```


| Name | Description |
|:-----|:------------|
| course[title]  | Title |
| course[topic_id]  | Topic ID |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "course": {
    "creator_id": 146,
    "id": 43,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 43,
    "additional_university_ids": [

    ],
    "topic_id": 48,
    "discipline_id": 48,
    "language_code": "fr",
    "exam_months": [

    ],
    "title": "Choux pastry 102",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-09-22T08:04:23.372Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80f54e9320004ee3e6328cb6fcabacf6de4e17464ae6354c717f9bf0c4f70ca2"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 97344b5908cbca23f110a509ed58379ac1d696509d78f8a59fee1516a0c456a4
```

`GET /v2/me/user`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 75,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:04:16.169Z",
    "updated_at": "2016-09-22T08:04:16.169Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97344b5908cbca23f110a509ed58379ac1d696509d78f8a59fee1516a0c456a4"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8d9f825bec03dd4ad3d8b797ff634631abeee77ed52a382804e9334a66f3ad11
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[23]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 76,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      23
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:04:16.283Z",
    "updated_at": "2016-09-22T08:04:16.328Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[23]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d9f825bec03dd4ad3d8b797ff634631abeee77ed52a382804e9334a66f3ad11"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ea316edf066a0d12a421e5538a0f0ce308751d77347d97545a6b3f8a93c6b151
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 78,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:04:16.433Z",
    "updated_at": "2016-09-22T08:04:16.433Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea316edf066a0d12a421e5538a0f0ce308751d77347d97545a6b3f8a93c6b151"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer cbb0e60ed51b7756dff7c10dd77dbba9ef8d54a5e8caafe3358f4fe7140c0b42
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[24]}
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 77,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      24
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:04:16.378Z",
    "updated_at": "2016-09-22T08:04:16.378Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[24]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbb0e60ed51b7756dff7c10dd77dbba9ef8d54a5e8caafe3358f4fe7140c0b42"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 33d8d4dbbacfcb14d16ab4632a3648a62983b3ec5fccb1cd316508143ce60ed3
```

`PATCH /v2/me/user`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="email"

magnus@gmail.sk
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="first_name"

Sven
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="fields_of_study[]"

27
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| user[email]  | Email address |
| user[first_name]  | First name |
| user[last_name]  | Last name |
| user[nickname]  | Nickname |
| user[locale]  | Locale |
| user[image]  | Image |
| user[university_id]  | University ID |
| user[study_level]  | Study Level |
| user[graduation_year]  | Graduation Year |
| user[fields_of_study]  | Fields of study (Topic IDs) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user": {
    "id": 80,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/ef998837575c0c844e63df9ba4a9892ef91fb159.jpg",
    "university_id": null,
    "fields_of_study": [
      27
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:04:16.614Z",
    "updated_at": "2016-09-22T08:04:16.831Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/daab96a110d55ef8a286b3d88907b92c9aa1221b.jpg",
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="email"

magnus@gmail.sk
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="first_name"

Sven
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="fields_of_study[]"

27
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 33d8d4dbbacfcb14d16ab4632a3648a62983b3ec5fccb1cd316508143ce60ed3"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 9c4f78d02d33c1218bceb9406ce24dde654e4dd412dd68f6cf37f72b0a3a4ae0
```

`GET /v2/me/bookmarks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "bookmarks": [
    {
      "id": 3,
      "bookmarkable_id": 65,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 66,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 67,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c4f78d02d33c1218bceb9406ce24dde654e4dd412dd68f6cf37f72b0a3a4ae0"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 26b03dbfd898792bc3a08a9978e8ddd5162ed0b75b3035a9836be0700e8db1bc
```

`GET /v2/me/campaigns`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "campaigns": [
    {
      "id": 10,
      "title": "Campaign 9",
      "company_id": 24,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 10,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/653938ceeed87e42b62d7feeca02cd82da1acb27.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/d204067fe9ed5e993ed4b1188ce57016fdd8b991.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/498551b0a405b9134839281bc158747e85383832.png",
          "target_url": "http://goskive.com",
          "id": 5,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 11,
      "title": "Campaign 10",
      "company_id": 25,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 11,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/6557160cf523e6b44ee9eac06061463b0fcbd3b1.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/f4961300e395cd3802066da84ade8e1cdd20826f.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/8aa5bf11cc13a7de5c7089d33a8ff916dd8f8472.png",
          "target_url": "http://goskive.com",
          "id": 6,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26b03dbfd898792bc3a08a9978e8ddd5162ed0b75b3035a9836be0700e8db1bc"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 83ae9084ba25d5dfc18d9c005a2bd21339c25b64497eea7a779720adcedb9b69
```

`GET /v2/me/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 84,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-3",
      "html_url": "https://goskive.com/course/mit-course-3",
      "slug": "mit-course-3",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 29,
      "discipline_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 3",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 1,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:04:17.077Z",
      "shortname": "mit-course-3"
    },
    {
      "creator_id": 85,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-4",
      "html_url": "https://goskive.com/course/mit-course-4",
      "slug": "mit-course-4",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 30,
      "discipline_id": 30,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 4",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 1,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:04:17.162Z",
      "shortname": "mit-course-4"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83ae9084ba25d5dfc18d9c005a2bd21339c25b64497eea7a779720adcedb9b69"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 17260734a7b231c1c91f68111b05bf166120e24a3f623d5ee917d5ff855cdd2c
```

`GET /v2/me/jobs`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "job_postings": [
    {
      "id": 4,
      "title": "Job Posting4",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 28,
      "company": {
        "id": 28,
        "name": "Fake Company Name 23",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
        "brand_color": "#000000",
        "updated_at": "2016-09-22T08:05:34.399Z"
      },
      "created_at": "2016-09-22T08:05:34.402Z",
      "updated_at": "2016-09-22T08:05:34.402Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17260734a7b231c1c91f68111b05bf166120e24a3f623d5ee917d5ff855cdd2c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer c57d9dd81da930c0dea877cbf4b9a564566df311a3d02ea304dd0ebeb2333132
```

`GET /v2/me/notifications`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "notifications": [
    {
      "type": "CommentNotification",
      "id": 11,
      "created_at": "2016-09-22T08:05:04.491Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 47,
      "updated_at": "2016-09-22T08:05:04.606Z",
      "author_id": "545",
      "thread_subject_id": "170",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 12,
      "created_at": "2016-09-22T08:05:04.594Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 48,
      "updated_at": "2016-09-22T08:05:04.610Z",
      "author_id": "548",
      "thread_subject_id": "171",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-09-22T08:05:04.981Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-09-22T08:05:04.981Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-09-22T08:05:05.352Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-09-22T08:05:05.352Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 15,
      "created_at": "2016-09-22T08:05:05.728Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-09-22T08:05:05.728Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 16,
      "created_at": "2016-09-22T08:05:06.021Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 73,
      "updated_at": "2016-09-22T08:05:06.021Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-09-22T08:05:06.328Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 74,
      "updated_at": "2016-09-22T08:05:06.328Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-09-22T08:05:06.654Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 75,
      "updated_at": "2016-09-22T08:05:06.654Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c57d9dd81da930c0dea877cbf4b9a564566df311a3d02ea304dd0ebeb2333132"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/19
Content-Type: application/json
Authorization: Bearer 01d4b02ad7c86b66521e65646dcfe7782cbf3eef867bcdaab3782afaee5bf5a7
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-09-22T07:55:06.000Z"}}
```


| Name | Description |
|:-----|:------------|
| notification[read_at]  | Read at |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "notification": {
    "type": "CommentNotification",
    "id": 19,
    "created_at": "2016-09-22T08:05:06.860Z",
    "read_at": "2016-09-22T07:55:06.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 49,
    "updated_at": "2016-09-22T08:05:06.901Z",
    "author_id": "574",
    "thread_subject_id": "178",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/19" -d '{"notification":{"read_at":"2016-09-22T07:55:06.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01d4b02ad7c86b66521e65646dcfe7782cbf3eef867bcdaab3782afaee5bf5a7"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f40e4850375be3e7914cfce93549eea8f4c65f7f5bd509784415650fa6ed4da6
```

`GET /v2/me/user_courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_courses": [
    {
      "id": 8,
      "course_id": 288,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-22T08:05:34.598Z",
      "course_published": true,
      "updated_at": "2016-09-22T08:05:34.590Z"
    },
    {
      "id": 9,
      "course_id": 289,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-09-22T08:05:34.682Z",
      "course_published": true,
      "updated_at": "2016-09-22T08:05:34.674Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f40e4850375be3e7914cfce93549eea8f4c65f7f5bd509784415650fa6ed4da6"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/11
Content-Type: application/json
Authorization: Bearer d897e67ae17c4e2b17dbf26cad034dc57b2468e717aca852d3972ae205b7f246
```

`GET /v2/me/user_courses/:user_course_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_course": {
    "id": 11,
    "course_id": 291,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-09-22T08:05:35.050Z",
    "course_published": true,
    "updated_at": "2016-09-22T08:05:35.042Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d897e67ae17c4e2b17dbf26cad034dc57b2468e717aca852d3972ae205b7f246"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/10
Content-Type: application/json
Authorization: Bearer 6521a4cae6f1a17737e3dcbf1f9fd1e78c3b4d868629c3fb45f9780837be5222
```

`PATCH /v2/me/user_courses/:user_course_id`

#### Parameters


```json
{"user_course":{"pinned":false}}
```


| Name | Description |
|:-----|:------------|
| user_course[course_id]  | Course ID |
| user_course[pinned]  | Pinned |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_course": {
    "id": 10,
    "course_id": 290,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-09-22T08:05:34.947Z",
    "course_published": true,
    "updated_at": "2016-09-22T08:05:34.936Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/10" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6521a4cae6f1a17737e3dcbf1f9fd1e78c3b4d868629c3fb45f9780837be5222"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 085ef217ddc6a97be611da18fe32a68ba0b78976b5485d0d63d7a760275073d8
```

`GET /v2/me/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 111,
      "user_id": 793
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 112,
      "user_id": 793
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 113,
      "user_id": 793
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 114,
      "user_id": 793
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 085ef217ddc6a97be611da18fe32a68ba0b78976b5485d0d63d7a760275073d8"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/177
Content-Type: application/json
```

`GET /v2/disciplines/:discipline_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "discipline": {
    "id": 177,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 175,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 177
      },
      {
        "id": 176,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 177
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/177" -X GET \
	-H "Content-Type: application/json"
```
## Get a list of disciplines


### Request

#### Endpoint

```
GET /v2/disciplines
Content-Type: application/json
```

`GET /v2/disciplines`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "disciplines": [
    {
      "id": 175,
      "name": "Future-proofed upward-trending hardware",
      "name_translations": {
        "en": "Future-proofed upward-trending hardware"
      }
    },
    {
      "id": 176,
      "name": "Focused real-time software",
      "name_translations": {
        "en": "Focused real-time software"
      }
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/disciplines" -X GET \
	-H "Content-Type: application/json"
```
# Feedback

## Change feedback state to &#39;closed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/close
Content-Type: application/json
Authorization: Bearer a321e348fee17adfdcf53ae79a37b33f6350c5d4c97cc92590e6c24526acc7f7
```

`PATCH /v2/feedbacks/:feedback_id/close`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 13,
    "user_id": 661,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-09-22T08:05:14.957Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/13/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a321e348fee17adfdcf53ae79a37b33f6350c5d4c97cc92590e6c24526acc7f7"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/fix
Content-Type: application/json
Authorization: Bearer 2d29acb0af05c95b258d7a758ae708ab00e51545fc9cc673c356406ef0179208
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 19,
    "user_id": 691,
    "feedbackable_id": 81,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-09-22T08:05:16.670Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/19/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d29acb0af05c95b258d7a758ae708ab00e51545fc9cc673c356406ef0179208"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/11
Content-Type: application/json
Authorization: Bearer 56e7c80214ec2bcb87ef484beb2898fbf35495cac646c4543eaf385b76fe5f35
```

`GET /v2/feedbacks/:feedback_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 11,
    "user_id": 649,
    "feedbackable_id": 73,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-22T08:05:14.452Z",
    "flags": 2,
    "message": ""
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |
| feedback[message] | Message (of comment) |


```shell
curl "api.goskive.com/v2/feedbacks/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56e7c80214ec2bcb87ef484beb2898fbf35495cac646c4543eaf385b76fe5f35"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/15/close
Content-Type: application/json
Authorization: Bearer 8eb7bc535633098c6ca6e4d1231e7a0056c7d1ab4917c3a7109564f67fe17cdb
```

`PATCH /v2/feedbacks/:feedback_id/close`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "There is no event close defined for the closed state"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/15/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8eb7bc535633098c6ca6e4d1231e7a0056c7d1ab4917c3a7109564f67fe17cdb"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/fix
Content-Type: application/json
Authorization: Bearer b1ca6ca974218de4bec1a8357825be7e75d04691668dc4df48a06e71ad564038
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "Content Unit was not corrected"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/16/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1ca6ca974218de4bec1a8357825be7e75d04691668dc4df48a06e71ad564038"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/17/fix
Content-Type: application/json
Authorization: Bearer 0f907cffb03b99e46b425f32dfb642a5137af7d2c27d78536a4aaaf0896d175e
```

`PATCH /v2/feedbacks/:feedback_id/fix`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": [
    {
      "error": "undefined_error_type",
      "error_description": "There is no event fix defined for the closed state"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks/17/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f907cffb03b99e46b425f32dfb642a5137af7d2c27d78536a4aaaf0896d175e"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/12
Content-Type: application/json
Authorization: Bearer 9d4e8e47359fb8c0998184350aef567a3c4a22e04cead0906e445fdc2c428792
```

`GET /v2/feedbacks/:feedback_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedback": {
    "id": 12,
    "user_id": 654,
    "feedbackable_id": 74,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-22T08:05:14.753Z",
    "flags": 0,
    "message": "Pi equals 2"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |
| feedback[message] | Message (of comment) |


```shell
curl "api.goskive.com/v2/feedbacks/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d4e8e47359fb8c0998184350aef567a3c4a22e04cead0906e445fdc2c428792"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/71/comments
Content-Type: application/json
Authorization: Bearer 176d3d74dc2156722c8496fdba808939bb95b943a7f177dac0eebab621aa92bd
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{"comment":{"message":"This flashcard is particularly helpful!"}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 57,
    "author_id": 640,
    "reply_to_id": null,
    "created_at": "2016-09-22T08:05:13.946Z",
    "status": "published",
    "replies": [

    ],
    "message": "This flashcard is particularly helpful!",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/71/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 176d3d74dc2156722c8496fdba808939bb95b943a7f177dac0eebab621aa92bd"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/70/comments
Content-Type: application/json
Authorization: Bearer 903135834fe85ee1e106ceb9ed2f907316cd53c1cbb2f1cfd250cb86652c37b6
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 56,
    "author_id": 637,
    "reply_to_id": null,
    "created_at": "2016-09-22T08:05:13.627Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 637,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:13.624Z",
      "flags": 3,
      "message": "Hard to see the formulae."
    }
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/70/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 903135834fe85ee1e106ceb9ed2f907316cd53c1cbb2f1cfd250cb86652c37b6"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/69/comments
Content-Type: application/json
Authorization: Bearer ee0225934686857ae7ce1ef8aace26eb18987172093f69f175e75761d936ec58
```

`GET /v2/flashcards/:flashcard_id/comments`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 54,
      "author_id": 635,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:13.394Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 636,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:13.412Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/69/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee0225934686857ae7ce1ef8aace26eb18987172093f69f175e75761d936ec58"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/72/comments
Content-Type: application/json
Authorization: Bearer dbfa76bd411bb6062046cb844031fec6c450dadfb3e77acfb0db9c0af778c5bf
```

`POST /v2/flashcards/:flashcard_id/comments`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank",
      "is too short (minimum is 2 characters)"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/72/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbfa76bd411bb6062046cb844031fec6c450dadfb3e77acfb0db9c0af778c5bf"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/40/feedbacks
Content-Type: application/json
Authorization: Bearer 1105173fc78b164194985f7767cd5c423282bd28da6bcf9e0a51d7b4adc719ba
```

`POST /v2/flashcards/:flashcard_id/feedbacks`

#### Parameters


```json
{"feedback":{"message":"No comprendo","flags":0}}
```


| Name | Description |
|:-----|:------------|
| feedback[message]  | Comment message |
| feedback[flags]  | Feedback flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "feedback": {
    "id": 7,
    "user_id": 331,
    "feedbackable_id": 40,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-09-22T08:04:51.578Z",
    "flags": 0,
    "message": "No comprendo"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/40/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1105173fc78b164194985f7767cd5c423282bd28da6bcf9e0a51d7b4adc719ba"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/37/feedbacks
Content-Type: application/json
Authorization: Bearer 6064ef2ed1d7caa8684f7e77c9a8397c7d55f1f905ea65041c64857bc5e6b9f8
```

`GET /v2/flashcards/:flashcard_id/feedbacks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedbacks": [
    {
      "id": 4,
      "user_id": 322,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:04:50.952Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 321,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:04:50.940Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/37/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6064ef2ed1d7caa8684f7e77c9a8397c7d55f1f905ea65041c64857bc5e6b9f8"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/85/votes
Content-Type: application/json
Authorization: Bearer 356c8bca6e04f973112c4741f0c84babf2fd855c298d05da1296352a6ec6c086
```

`GET /v2/flashcards/:flashcard_id/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 792
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 791
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 790
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/85/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 356c8bca6e04f973112c4741f0c84babf2fd855c298d05da1296352a6ec6c086"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/62/republish
Content-Type: application/json
Authorization: Bearer 09ed4637c9d62af83fc473555da7b8d4ef2ba1b851330b42c4bb1e31454056a4
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/62/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09ed4637c9d62af83fc473555da7b8d4ef2ba1b851330b42c4bb1e31454056a4"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/bookmark
Content-Type: application/json
Authorization: Bearer 6eb19aafff1e099dc3e7d5ee0aef23b93c051c65248ce8a5cdfef4cbbaa96691
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6eb19aafff1e099dc3e7d5ee0aef23b93c051c65248ce8a5cdfef4cbbaa96691"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/61
Content-Type: application/json
Authorization: Bearer 16f22dd0b60cacc42eb39651ed39b71049143c2cf04e9062c54ada6e2f1b5c6d
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16f22dd0b60cacc42eb39651ed39b71049143c2cf04e9062c54ada6e2f1b5c6d"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/downvote
Content-Type: application/json
Authorization: Bearer 512388bbda05701a3379bc7f2a2d4892f06ae64d5beec2e5c29dc883a1e3dfae
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 512388bbda05701a3379bc7f2a2d4892f06ae64d5beec2e5c29dc883a1e3dfae"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/45
Content-Type: application/json
Authorization: Bearer ca90c6b3bf92dc1806cdb3e649b9d25bf4e2f70b1ef9bb149773f542397a396c
```

`GET /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 45,
    "obfuscated_id": "IVleRnyZemc",
    "author_id": 357,
    "chapter_id": 89,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:04:53.933Z",
    "created_at": "2016-09-22T08:04:53.933Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "Helps things *raise*",
    "front_content_html": "<p>I'm the content</p>",
    "back_content_html": "<p>I'm the content</p>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca90c6b3bf92dc1806cdb3e649b9d25bf4e2f70b1ef9bb149773f542397a396c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/report
Content-Type: application/json
Authorization: Bearer b7fe961ab9851ba76587237a70a296cba456ed90316ade722526ae9d0002cea1
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7fe961ab9851ba76587237a70a296cba456ed90316ade722526ae9d0002cea1"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/43/bookmark
Content-Type: application/json
Authorization: Bearer 3e90e83c97f63a893f549fa63630b9c81b623719cb077b909329046f956ff67b
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e90e83c97f63a893f549fa63630b9c81b623719cb077b909329046f956ff67b"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/66
Content-Type: application/json
Authorization: Bearer 556728585584e1d23d5c8229ccda15754b889a2af9330c48549628e0bc59bd46
```

`PATCH /v2/flashcards/:flashcard_id`

#### Parameters


```json
{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content]  | Front Content Markdown |
| flashcard[front_content_html]  | Front Content HTML |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[back_content_html]  | Back Content HTML |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 426,
    "chapter_id": 110,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:04:57.822Z",
    "created_at": "2016-09-22T08:04:57.477Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "Function of *eggs* in choux pastry",
    "back_content": "*rise*",
    "front_content_html": "<p>I'm the content</p>",
    "back_content_html": "<strong>rise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/66" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 556728585584e1d23d5c8229ccda15754b889a2af9330c48549628e0bc59bd46"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/67
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 13d0d44cae7765f22b4e1b408cd9dae74ceec0ebf4fdd03b78652c8a160a58aa
```

`PATCH /v2/flashcards/:flashcard_id`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

de
------------XnJLe9ZIbbGUYtzPQJ16u1--
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content]  | Front Content Markdown |
| flashcard[front_content_html]  | Front Content HTML |
| flashcard[back_content]  | Back Content Markdown |
| flashcard[back_content_html]  | Back Content HTML |
| flashcard[front_image]  | Front Image |
| flashcard[back_image]  | Back Image |
| flashcard[published]  | Published |
| flashcard[reported]  | Reported |
| flashcard[position]  | Position |
| flashcard[chapter_id]  | Chapter ID |
| flashcard[language_code]  | Language Code |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcard": {
    "id": 67,
    "obfuscated_id": "btMCNJVyvlA",
    "author_id": 429,
    "chapter_id": 111,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:04:58.290Z",
    "created_at": "2016-09-22T08:04:58.004Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/3a4d2a9ec6017861dc2aad3d1778708c10682bf3.png)",
    "back_content": "![Flashcard Image](file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/2f43518ac24f33ea5bb9717be7efac47f652b93c.png)",
    "front_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/3a4d2a9ec6017861dc2aad3d1778708c10682bf3.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///home/ubuntu/skive-backend/public/system/flashcards/medium_highdpi/2f43518ac24f33ea5bb9717be7efac47f652b93c.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/67" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[front_image]"; filename="flashcard_front.jpg"
Content-Type: image/jpeg
Content-Length: 15053

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[back_image]"; filename="flashcard_back.jpg"
Content-Type: image/jpeg
Content-Length: 16101

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[language_code]"

de
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 13d0d44cae7765f22b4e1b408cd9dae74ceec0ebf4fdd03b78652c8a160a58aa"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/upvote
Content-Type: application/json
Authorization: Bearer e89c4810eac5d5649a08c6d01f02c0e0c99b2bed23f1a165386a9cd5256e0005
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e89c4810eac5d5649a08c6d01f02c0e0c99b2bed23f1a165386a9cd5256e0005"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/flashcards/images/cache/presign
Content-Type: application/json
Authorization: Bearer 94f17c81276b1855bd4f9789483df1af61482aaffdc99f5c598d2ef3ec77b0f9
```

`GET /v2/flashcards/images/cache/presign`

#### Parameters


None known.


### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/98751cffa70da4310971112ff83c0dc9",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOS0yMlQwOTowNDo1NFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS85ODc1MWNmZmE3MGRhNDMxMDk3MTExMmZmODNjMGRjOSJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwOTIyL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDkyMlQwODA0NTRaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160922/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160922T080454Z",
    "x-amz-signature": "c4c78f7d0c70c071e7f702e019ce3473a20a51b4d74571c9e0eb38f862f69d24"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/images/cache/presign" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94f17c81276b1855bd4f9789483df1af61482aaffdc99f5c598d2ef3ec77b0f9"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/2/sign_ups
Content-Type: application/json
Authorization: Bearer 7ded7793b3b2c4b89c70763e372c0dd40d539d50a70e96349199dc68d66ab71d
```

`POST /v2/me/jobs/:job_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":"joe@megacorp.com"}}
```


| Name | Description |
|:-----|:------------|
| job_posting[email_address] *required* | Email to sign up with |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "sign_up": {
    "id": 2,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/2/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ded7793b3b2c4b89c70763e372c0dd40d539d50a70e96349199dc68d66ab71d"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer f588998553dacd968720be37742ce9fab07e74b362538708f0b950f669949f16
```

`POST /v2/me/jobs/:job_id/sign_ups`

#### Parameters


```json
{"sign_up":{"email_address":""}}
```


| Name | Description |
|:-----|:------------|
| job_posting[email_address] *required* | Email to sign up with |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "email_address": [
      "can't be blank"
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/3/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f588998553dacd968720be37742ce9fab07e74b362538708f0b950f669949f16"
```
# Password

## Change password


### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"reset_password_token":"VFNppxWyrNtVFMzoTYj_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "id": 1,
  "email": "jan.meier@hotmail.de",
  "created_at": "2016-09-22T08:04:48.070Z",
  "updated_at": "2016-09-22T08:04:48.217Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "university_id": null,
  "locale": "en",
  "phone_number": null,
  "phone_number_country_code": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "study_level": null,
  "audit_id": 4131
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"VFNppxWyrNtVFMzoTYj_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
	-H "Content-Type: application/json"
```
## Change password


### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"reset_password_token":"GdfmavCxyJXbtEBkWY-8","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "id": 300,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-09-22T08:04:49.122Z",
  "updated_at": "2016-09-22T08:04:49.997Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "university_id": null,
  "locale": "en",
  "phone_number": null,
  "phone_number_country_code": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "study_level": null,
  "audit_id": 4134
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"GdfmavCxyJXbtEBkWY-8","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
	-H "Content-Type: application/json"
```
## Request password reset email with correct email


### Request

#### Endpoint

```
POST /v2/password
Content-Type: application/json
```

`POST /v2/password`

#### Parameters


```json
{"password":{"email":"jan.turnosky@hotmail.sk"}}
```


| Name | Description |
|:-----|:------------|
| password[email] *required* | Email address |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```




```shell
curl "api.goskive.com/v2/password" -d '{"password":{"email":"jan.turnosky@hotmail.sk"}}' -X POST \
	-H "Content-Type: application/json"
```
## Request password reset email with incorrect email


### Request

#### Endpoint

```
POST /v2/password
Content-Type: application/json
```

`POST /v2/password`

#### Parameters


```json
{"password":{"email":"jan.turnosky@hotmail.com"}}
```


| Name | Description |
|:-----|:------------|
| password[email] *required* | Email address |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```




```shell
curl "api.goskive.com/v2/password" -d '{"password":{"email":"jan.turnosky@hotmail.com"}}' -X POST \
	-H "Content-Type: application/json"
```
## Validation error on password change

An incorrect `reset_password_token` gives a validation
          error.

### Request

#### Endpoint

```
PUT /v2/password
Content-Type: application/json
```

`PUT /v2/password`

#### Parameters


```json
{"password":{"password":"new-passw0rd","password_confirmation":"new-passw0rd","reset_password_token":"invalidt0ken"}}
```


| Name | Description |
|:-----|:------------|
| password[password] *required* | New password |
| password[password_confirmation] *required* | New password confirmation |
| password[reset_password_token] *required* | Reset password token |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "reset_password_token": [
      "is invalid"
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"password":"new-passw0rd","password_confirmation":"new-passw0rd","reset_password_token":"invalidt0ken"}}' -X PUT \
	-H "Content-Type: application/json"
```
# Question Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/questions/80/comments
Content-Type: application/json
Authorization: Bearer 99eba3ad0bae940a20f80e54d4216d4d29fda5154fcdb0580a4a0ceeaf078318
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{"comment":{"message":"Not sure what this question means."}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 53,
    "author_id": 590,
    "reply_to_id": null,
    "created_at": "2016-09-22T08:05:08.686Z",
    "status": "published",
    "replies": [

    ],
    "message": "Not sure what this question means.",
    "feedback": null
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/80/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99eba3ad0bae940a20f80e54d4216d4d29fda5154fcdb0580a4a0ceeaf078318"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/78/comments
Content-Type: application/json
Authorization: Bearer 24af80f3414b1044a8bc8925bf436b4d129772e0650fc3f290928e66200d973a
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "comment": {
    "id": 52,
    "author_id": 584,
    "reply_to_id": null,
    "created_at": "2016-09-22T08:05:07.908Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 584,
      "feedbackable_id": 78,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:07.905Z",
      "flags": 2,
      "message": "Really bad grammar."
    }
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/78/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24af80f3414b1044a8bc8925bf436b4d129772e0650fc3f290928e66200d973a"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/77/comments
Content-Type: application/json
Authorization: Bearer c01bd6c624b75a9be2a5b62078739f9abeb716d0d03a510a5c133bbd4810ad53
```

`GET /v2/questions/:question_id/comments`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 50,
      "author_id": 582,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:07.525Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 583,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:07.544Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/77/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c01bd6c624b75a9be2a5b62078739f9abeb716d0d03a510a5c133bbd4810ad53"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/79/comments
Content-Type: application/json
Authorization: Bearer 1cb864d504bdedb0c099ae3f267b08e5e02163a13cda999aceb70715cce1d6d2
```

`POST /v2/questions/:question_id/comments`

#### Parameters


```json
{}
```


| Name | Description |
|:-----|:------------|
| comment[message] *required* | Message |
| comment[feedback][flags] *required* | Flags |



### Response

```
Content-Type: application/json; charset=utf-8
422 Unprocessable Entity
```


```json
{
  "errors": {
    "message": [
      "can't be blank",
      "is too short (minimum is 2 characters)"
    ]
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| comment[id] | Comment ID |
| comment[author_id] | Author ID |
| comment[message] | Message |
| comment[created_at] | Created at |
| comment[reply_to_id] | Reply to Comment ID |
| comment[replies] | Replies (Array of Comments) |
| comment[feedback] | Feedback |
| [:comment, :feedback][[:comment, :feedback][id]] | Feedback ID |
| [:comment, :feedback][[:comment, :feedback][user_id]] | Creator ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_id]] | Feedbackable ID |
| [:comment, :feedback][[:comment, :feedback][feedbackable_type]] | Feedbackable Type |
| [:comment, :feedback][[:comment, :feedback][workflow_state]] | Workflow State |
| [:comment, :feedback][[:comment, :feedback][flags]] | Flags |
| [:comment, :feedback][[:comment, :feedback][updated_at]] | Updated at |


```shell
curl "api.goskive.com/v2/questions/79/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cb864d504bdedb0c099ae3f267b08e5e02163a13cda999aceb70715cce1d6d2"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/121/feedbacks
Content-Type: application/json
Authorization: Bearer d8d06787e1901f1b2fc6995abb49da7d200c1acb373ffe5df794237732ec5437
```

`POST /v2/questions/:question_id/feedbacks`

#### Parameters


```json
{"feedback":{"message":"No comprendo","flags":0}}
```


| Name | Description |
|:-----|:------------|
| feedback[message]  | Comment message |
| feedback[flags]  | Feedback flags |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "feedback": {
    "id": 45,
    "user_id": 841,
    "feedbackable_id": 121,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-09-22T08:05:28.791Z",
    "flags": 0,
    "message": "No comprendo"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| feedback[id] | Feedback ID |
| feedback[user_id] | Creator ID |
| feedback[feedbackable_id] | Feedbackable ID |
| feedback[feedbackable_type] | Feedbackable Type |
| feedback[workflow_state] | Workflow State |
| feedback[flags] | Flags |
| feedback[updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/121/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8d06787e1901f1b2fc6995abb49da7d200c1acb373ffe5df794237732ec5437"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/117/feedbacks
Content-Type: application/json
Authorization: Bearer 842d56330754009f0794e67f5cd97852dc81848cd3cdfa6356f72579182802ae
```

`GET /v2/questions/:question_id/feedbacks`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedbacks": [
    {
      "id": 42,
      "user_id": 823,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:27.345Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 822,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:27.329Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/117/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 842d56330754009f0794e67f5cd97852dc81848cd3cdfa6356f72579182802ae"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/12/votes
Content-Type: application/json
Authorization: Bearer 6a9964b2ce39b795f139d668e12f504486ebe738390e1bb8987471f1a272eeb1
```

`GET /v2/questions/:question_id/votes`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "votes": [
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 12,
      "user_id": 137
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 12,
      "user_id": 136
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 12,
      "user_id": 135
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/12/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a9964b2ce39b795f139d668e12f504486ebe738390e1bb8987471f1a272eeb1"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/49/republish
Content-Type: application/json
Authorization: Bearer 795f7950110f459f50f0a650cf966f7377b1ec1df13bf0cfaf0ff9d22ec87ece
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
403 Forbidden
```


```json
{
  "errors": [
    {
      "error": "forbidden",
      "error_description": "Your credentials do not allow access to this resource"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 795f7950110f459f50f0a650cf966f7377b1ec1df13bf0cfaf0ff9d22ec87ece"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/41/bookmark
Content-Type: application/json
Authorization: Bearer 10c30ee9fa7ed463ead63af8ce632210d4bfca3305384eb6ab2a3d1838be88cf
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/41/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10c30ee9fa7ed463ead63af8ce632210d4bfca3305384eb6ab2a3d1838be88cf"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/46
Content-Type: application/json
Authorization: Bearer 08931c7343770ba12aecf17b4f4b0b0f1824155c7976d8a685f1842002ea4582
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08931c7343770ba12aecf17b4f4b0b0f1824155c7976d8a685f1842002ea4582"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/43/downvote
Content-Type: application/json
Authorization: Bearer df358e4c6e7359ae4adbf40fe6f569b21e89dbe45db36f9be329f45e4ee42583
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/43/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df358e4c6e7359ae4adbf40fe6f569b21e89dbe45db36f9be329f45e4ee42583"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/47
Content-Type: application/json
Authorization: Bearer a7112561ae7c6d63ef8914ddb58515f312ae2a188cc1d3c16d8a86bd75647237
```

`GET /v2/questions/:question_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "question": {
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 225,
    "chapter_id": 57,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:04:35.744Z",
    "created_at": "2016-09-22T08:04:35.627Z",
    "tags": [
      {
        "id": 16,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 15,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 94,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 95,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/questions/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7112561ae7c6d63ef8914ddb58515f312ae2a188cc1d3c16d8a86bd75647237"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/42/report
Content-Type: application/json
Authorization: Bearer 92b91e6bd7a9aa276388bea1fb35949348a8417520aed50d9cc3e758150a62b3
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92b91e6bd7a9aa276388bea1fb35949348a8417520aed50d9cc3e758150a62b3"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/45/bookmark
Content-Type: application/json
Authorization: Bearer 7dd07720fb30e1e2f5a187dad5b616736ae5c06197e8b165f6c7b284028842dc
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dd07720fb30e1e2f5a187dad5b616736ae5c06197e8b165f6c7b284028842dc"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/44
Content-Type: application/json
Authorization: Bearer 72234cd38e4be9f89450c5864f4f0ed854124fda57bbc74732ac56583613221e
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":44,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-22T08:04:34.176Z","updated_at":"2016-09-22T08:04:34.294Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":54,"author_id":216,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question]  | Question Markdown |
| question[question_html]  | Question HTML |
| question[explanation]  | Explanation Markdown |
| question[explanation_html]  | Explanation HTML |
| question[answer_options]  | Answer Options |
| question[published]  | Published |
| question[reported]  | Reported |
| question[position]  | Position |
| question[chapter_id]  | Chapter ID |
| question[shuffle_answers]  | Shuffle Answers |
| question[language_code]  | Language Code |
| question[answer_options][position]  | Answer Position |
| question[answer_options][content]  | Answer Content Markdown |
| question[answer_options][content_html]  | Answer Content HTML |
| question[answer_options][correct]  | Answer Correctness |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "question": {
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 216,
    "chapter_id": 54,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-09-22T08:04:34.407Z",
    "created_at": "2016-09-22T08:04:34.176Z",
    "tags": [
      {
        "id": 10,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 9,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>44, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-09-22T08:04:34.176Z\", \"updated_at\"=>\"2016-09-22T08:04:34.294Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>54, \"author_id\"=>216, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 87,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 88,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 89,
        "position": 3,
        "content": "Choux needs baking powder.",
        "content_html": "<p>Choux needs baking powder.</p>",
        "correct": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/questions/44" -d '{"question":{"question":{"id":44,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-09-22T08:04:34.176Z","updated_at":"2016-09-22T08:04:34.294Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":54,"author_id":216,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72234cd38e4be9f89450c5864f4f0ed854124fda57bbc74732ac56583613221e"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/40/upvote
Content-Type: application/json
Authorization: Bearer c3c3f052e07df82da54e4b36265cce035925b0ee45bdc8e5cdfd98a6760e142a
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/40/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3c3f052e07df82da54e4b36265cce035925b0ee45bdc8e5cdfd98a6760e142a"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/questions/images/cache/presign
Content-Type: application/json
Authorization: Bearer 17f0c21f7903c0fda68d0e4835a67234e7dfcdac1cdaef87b949005c1b5c9d66
```

`GET /v2/questions/images/cache/presign`

#### Parameters


None known.


### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/ded944db81238726823622b34d4e9b28",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0wOS0yMlQwOTowNDozMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9kZWQ5NDRkYjgxMjM4NzI2ODIzNjIyYjM0ZDRlOWIyOCJ9LHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYwOTIyL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MDkyMlQwODA0MzJaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20160922/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20160922T080432Z",
    "x-amz-signature": "e213c84b1c1aa99039282858a3c1068ce68a74d0a8c6542858733effa5df086b"
  }
}
```



```shell
curl "api.goskive.com/v2/questions/images/cache/presign" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17f0c21f7903c0fda68d0e4835a67234e7dfcdac1cdaef87b949005c1b5c9d66"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer ed16c549fa4f8e185a207953424fd85b4f28addd1c26149d1e961f6719b6baa2
```

`GET /v2/search/courses`

#### Parameters


```json
query: Pi
```


| Name | Description |
|:-----|:------------|
| query *required* | Search query |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 198,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "topic_id": 67,
      "discipline_id": 67,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Pizza 201",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:04:31.983Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed16c549fa4f8e185a207953424fd85b4f28addd1c26149d1e961f6719b6baa2"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b2e06e7ab75c1552feef5e3c17400d3e498a9df39df322655a9fef416438216e
```

`GET /v2/search/universities`

#### Parameters


```json
query: NSP
```


| Name | Description |
|:-----|:------------|
| query *required* | Search query |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "universities": [
    {
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-64",
      "html_url": "https://goskive.com/university/uni-64",
      "slug": "uni-64",
      "name": "National School of Pizza",
      "short_name": "Uni 64",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/34ae0a587d54bcfff28a891b60e4ff558b06fe03.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/82b731c89e2f272b7201803005596c5d91004739.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-22T08:04:32.252Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-63",
      "html_url": "https://goskive.com/university/uni-63",
      "slug": "uni-63",
      "name": "National School of Pastry",
      "short_name": "Uni 63",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f0455cb406a50dfa205f9dfc8a84dec6ed607634.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ee88380d46739e088ac23d7ad0ef1eb91c7c5fb1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-22T08:04:32.235Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/universities?query=NSP" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2e06e7ab75c1552feef5e3c17400d3e498a9df39df322655a9fef416438216e"
```
# Topics

## Get a list of topics


### Request

#### Endpoint

```
GET /v2/topics
Content-Type: application/json
```

`GET /v2/topics`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "topics": [
    {
      "id": 295,
      "name": "Balanced value-added orchestration",
      "name_translations": {
        "en": "Balanced value-added orchestration"
      },
      "discipline_id": 296
    },
    {
      "id": 296,
      "name": "Triple-buffered explicit collaboration",
      "name_translations": {
        "en": "Triple-buffered explicit collaboration"
      },
      "discipline_id": 297
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/topics" -X GET \
	-H "Content-Type: application/json"
```
## Get a topic and translations


### Request

#### Endpoint

```
GET /v2/topics/294
Content-Type: application/json
```

`GET /v2/topics/:topic_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "topic": {
    "id": 294,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 295
  }
}
```



```shell
curl "api.goskive.com/v2/topics/294" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer c06df1f9bed01bbf34918a6861d4103c35efa69d10b1d8e487f760d08a3a2f86
```

`GET /v2/universities`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "universities": [
    {
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-128",
      "html_url": "https://goskive.com/university/uni-128",
      "slug": "uni-128",
      "name": "University 74",
      "short_name": "Uni 128",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2fc53ff5dd17139d68d0f07faced6ccc60096152.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/14beb69efa7713df2f56ef4d075848f934fe5299.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-22T08:04:58.433Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 129,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-129",
      "html_url": "https://goskive.com/university/uni-129",
      "slug": "uni-129",
      "name": "University 75",
      "short_name": "Uni 129",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/06d230099f8b869139a3505fd9a31831cb9d65e2.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1c92dbb32d1635f9aca651561f92e53089efbf18.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-22T08:04:58.449Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-130",
      "html_url": "https://goskive.com/university/uni-130",
      "slug": "uni-130",
      "name": "University 76",
      "short_name": "Uni 130",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/533d65a5fbfa4869f2fd5ea55f41c6a2a3233f0b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2cdcaeb16dedb8e1188c6699ecc00eae44b58249.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-09-22T08:04:58.464Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c06df1f9bed01bbf34918a6861d4103c35efa69d10b1d8e487f760d08a3a2f86"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer f901b78f762089e0164509d4bbe219b91611be086fe8b377efbdab5a417ef82d
```

`GET /v2/universities/:university_slug`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "university": {
    "id": 132,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6fe79b1498bbae607eed239641011037c14485f3.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/698454cb82409adf685ea8e628f7e6a9515f311a.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-09-22T08:04:58.594Z",
    "url": "http://www.fu-berlin.de",
    "latitude": "52.496403",
    "longitude": "13.357812",
    "published": true
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f901b78f762089e0164509d4bbe219b91611be086fe8b377efbdab5a417ef82d"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e1ee2902d9a8eda2cb0d0416da3e67774a9e6d5351f2454dbe844723a58191d7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":293,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
```


| Name | Description |
|:-----|:------------|
| course[title] *required* | Title |
| course[topic_id] *required* | Topic ID |
| course[chapters]  | Chapters |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |
| course[chapters][title]  | Chapter title |
| course[chapters][position]  | Chapter position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "course": {
    "creator_id": 891,
    "id": 284,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 269,
    "additional_university_ids": [

    ],
    "topic_id": 293,
    "discipline_id": 294,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 3,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": "2016-09-22T08:05:33.722Z",
    "updated_at": "2016-09-22T08:05:33.859Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 188,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-09-22T08:05:33.816Z",
        "course_id": 284,
        "author_id": 891,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 189,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-09-22T08:05:33.833Z",
        "course_id": 284,
        "author_id": 891,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 190,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-09-22T08:05:33.849Z",
        "course_id": 284,
        "author_id": 891,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":293,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1ee2902d9a8eda2cb0d0416da3e67774a9e6d5351f2454dbe844723a58191d7"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 06f322a7c86932178d926abf0c31e325c612d62403b6c6314f93c147a91cbb2a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":292,"published":false}}
```


| Name | Description |
|:-----|:------------|
| course[title] *required* | Title |
| course[topic_id] *required* | Topic ID |
| course[chapters]  | Chapters |
| course[instructor_name]  | Instructor name |
| course[language_code]  | Language Code |
| course[exam_months]  | Exam months |
| course[chapters]  | Chapters |
| course[organizational_identifier]  | Organizational identifier |
| course[university_id]  | University ID |
| course[degree]  | Degree |
| course[published]  | Published |
| course[course_page_url]  | Course Page URL |
| course[number_of_students]  | Number of Students |
| course[semester_min]  | Semester Min |
| course[semester_max]  | Semester Max |
| course[seconds_per_question]  | Seconds per Question |
| course[reporting_category_id]  | Reporting Category ID |
| course[additional_university_ids]  | Additional University IDs |
| course[chapters][title]  | Chapter title |
| course[chapters][position]  | Chapter position |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "course": {
    "creator_id": 890,
    "id": 283,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 268,
    "additional_university_ids": [

    ],
    "topic_id": 292,
    "discipline_id": 293,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "users_count": 0,
    "user_generated": true,
    "published": true,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-09-22T08:05:33.688Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":292,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06f322a7c86932178d926abf0c31e325c612d62403b6c6314f93c147a91cbb2a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: 
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 848,
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-188",
      "html_url": "https://goskive.com/course/fu-course-188",
      "slug": "fu-course-188",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 188",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:29.639Z",
      "shortname": "fu-course-188"
    },
    {
      "creator_id": 848,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-189",
      "html_url": "https://goskive.com/course/fu-course-189",
      "slug": "fu-course-189",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 257,
      "discipline_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 189",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-09-22T08:05:29.949Z",
      "updated_at": "2016-09-22T08:05:29.956Z",
      "shortname": "fu-course-189"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 63068c468e1f1deeb904052dfbfc5fcebfe5a5fffe51c2d23433d8bca0a8c94c
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 865,
      "id": 263,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-204",
      "html_url": "https://goskive.com/course/fu-course-204",
      "slug": "fu-course-204",
      "university_id": 258,
      "additional_university_ids": [

      ],
      "topic_id": 272,
      "discipline_id": 273,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 204",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:31.367Z",
      "shortname": "fu-course-204"
    },
    {
      "creator_id": 865,
      "id": 264,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-205",
      "html_url": "https://goskive.com/course/fu-course-205",
      "slug": "fu-course-205",
      "university_id": 258,
      "additional_university_ids": [

      ],
      "topic_id": 273,
      "discipline_id": 274,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 205",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-09-22T08:05:31.667Z",
      "updated_at": "2016-09-22T08:05:31.673Z",
      "shortname": "fu-course-205"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63068c468e1f1deeb904052dfbfc5fcebfe5a5fffe51c2d23433d8bca0a8c94c"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: 
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 853,
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 260,
      "discipline_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:30.197Z",
      "shortname": "fu-course-192"
    },
    {
      "creator_id": 853,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-193",
      "html_url": "https://goskive.com/course/fu-course-193",
      "slug": "fu-course-193",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 261,
      "discipline_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 193",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:30.238Z",
      "shortname": "fu-course-193"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a32dd77ce47426f77f8e69899cafd5f5f30e66b1f656056058006ca3c07c6aff
```

`GET /v2/universities/:university_slug/courses`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 871,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-208",
      "html_url": "https://goskive.com/course/fu-course-208",
      "slug": "fu-course-208",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "topic_id": 276,
      "discipline_id": 277,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 208",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:31.912Z",
      "shortname": "fu-course-208"
    },
    {
      "creator_id": 871,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-209",
      "html_url": "https://goskive.com/course/fu-course-209",
      "slug": "fu-course-209",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "topic_id": 277,
      "discipline_id": 278,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 209",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "users_count": 0,
      "user_generated": false,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-09-22T08:05:31.954Z",
      "shortname": "fu-course-209"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a32dd77ce47426f77f8e69899cafd5f5f30e66b1f656056058006ca3c07c6aff"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 8c34c837136f8aa6421a15629acee1c8607afcfcb2380e340612d3810ba83262
```

`POST /users`

#### Parameters


```json
{"authentication_type":"password","email":"jan.turnosky@hotmail.cz","first_name":"Jan","last_name":"Turnosky","password":"Vykupiteli"}
```


| Name | Description |
|:-----|:------------|
| authentication_type *required* | Authentication Type |
| email *required* | Email address |
| first_name *required* | First name |
| last_name *required* | Last name |
| password *required* | Password |
| locale  | Locale |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "id": 807,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-09-22T08:05:25.804Z",
  "all_access_pass": false,
  "eligible_for_first_course_purchase_discount": false,
  "email": "jan.turnosky@hotmail.cz",
  "display_name": "Jan Turnosky",
  "course_ids": [

  ]
}
```



```shell
curl "api.goskive.com/users" -d '{"authentication_type":"password","email":"jan.turnosky@hotmail.cz","first_name":"Jan","last_name":"Turnosky","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c34c837136f8aa6421a15629acee1c8607afcfcb2380e340612d3810ba83262"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/776
Content-Type: application/json
Authorization: Bearer 9390246724e9f3147051a723567f19a626878dbf8610766d3bf7f812e45dc052
```

`GET /v2/users/:user_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_profile": {
    "id": 776,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 234,
    "fields_of_study": [
      235,
      236
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-09-22T08:05:23.109Z",
    "updated_at": "2016-09-22T08:05:23.109Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/776" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9390246724e9f3147051a723567f19a626878dbf8610766d3bf7f812e45dc052"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/774
Content-Type: application/json
Authorization: Bearer ad2a704e4c51bc3a02400f06faa3b9ac363d0bcd26fad9fff98d37af0408a819
```

`GET /v2/users/:user_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_profile": {
    "id": 774,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "Magnus Ahlström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [

    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-09-22T08:05:22.946Z",
    "updated_at": "2016-09-22T08:05:22.946Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/774" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad2a704e4c51bc3a02400f06faa3b9ac363d0bcd26fad9fff98d37af0408a819"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 4162862d8c046b08048e1fcac1ada64c772859bd98315a0832e62fae813bd0d6
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4162862d8c046b08048e1fcac1ada64c772859bd98315a0832e62fae813bd0d6"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer 65cb19cd58e0ab8a3eebd5595ab1ec2f0c0d3e7ccc2859a454e5090a7c36aa91
```

`GET /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "vote": {
    "id": 13,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 89,
    "user_id": 618
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65cb19cd58e0ab8a3eebd5595ab1ec2f0c0d3e7ccc2859a454e5090a7c36aa91"
```
