---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

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

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MTgzODZmNDc3NmM1OGM3MDJjZDdhYjhlNTFmOGE4NDI5ZTgxZWFiNjk2OGJh
NTAwNGZkMWQyMDM3ODRmYzMwOTo5Yjg2NjYzZDM1MGYxZmFiZTI5YmM1ZDA4
Y2ExZDdkY2Y1YWM2YWMxMmRjODIwN2MzZWJiNWQ0N2QxMmY2M2Ux

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
	-u 18386f4776c58c702cd7ab8e51f8a8429e81eab6968ba5004fd1d203784fc309:9b86663d350f1fabe29bc5d08ca1d7dcf5ac6ac12dc8207c3ebb5d47d12f63e1
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7548e368a22915b9f8d79bb05e5f98ca0e134f1f6f697aab0948af81c31e1956","client_secret":"352f8dfc1626725263a73d5ff3b8306213a5311868f40e6538cfdd8dc5582596"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7548e368a22915b9f8d79bb05e5f98ca0e134f1f6f697aab0948af81c31e1956","client_secret":"352f8dfc1626725263a73d5ff3b8306213a5311868f40e6538cfdd8dc5582596"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OWU5NzBkYTg0NjM2ZDY5MDYxZDIxZDBkMThlYTNlYmE3NDg1ZmIzZTIxMGMx
M2E3OWVmN2I2NGZiYTZkNWE5MzpmNjEwYTIyYjY4NzFkOTk0ZjQ3N2YxYzM3
ODRmZTVmYWE2MDczZTdiNTljZDRjYjMxNDQ0NTdlZmUyYjMxYWVj

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
	-u 9e970da84636d69061d21d0d18ea3eba7485fb3e210c13a79ef7b64fba6d5a93:f610a22b6871d994f477f1c3784fe5faa6073e7b59cd4cb3144457efe2b31aec
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1bacbf000ad74954546f0a2ca4d97fcccca8256cd96d0a5105ce353229539698","client_secret":"20640ac889b8c94ab5df57884ff284fce23bd0ffff7b44157e2511755dcde444"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1bacbf000ad74954546f0a2ca4d97fcccca8256cd96d0a5105ce353229539698","client_secret":"20640ac889b8c94ab5df57884ff284fce23bd0ffff7b44157e2511755dcde444"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7f0d2eba5aa188ea124fcae1946e1b64098f8e17b00c80a0d84ec905b93abcae","client_secret":"bf79c6c5b18bf017bb15ce36d20eac626b572cd69b47c23f9f509927ff12cd38"}
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
  "access_token": "3eab91e1ac5d0c51af2a966987a5f77f5e2499fe9a090a11137c2f8edf1ef345",
  "token_type": "bearer",
  "created_at": 1468852713
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7f0d2eba5aa188ea124fcae1946e1b64098f8e17b00c80a0d84ec905b93abcae","client_secret":"bf79c6c5b18bf017bb15ce36d20eac626b572cd69b47c23f9f509927ff12cd38"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NmE3YTE4MTVmYWM1NDBlZDgyZGJjYmQ4YmVlMjFiNjlkNjRhNWU3MzU4MDdi
NDAwMDVjMTBjODU0ZjQwMzc5Njo5ZmU5NTExYzJhZWI1MjI2YzQ5NWNjYzNl
MTY1NTI5ZDdjNTA5ZGIxNDMxM2ZmYWEwYWQzODYwMmJjMTdhZGYx

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
  "access_token": "3a7aa4ced133873564c92ad1055e12a7fb937e43a4ec7d634b04fcdc93099ff5",
  "token_type": "bearer",
  "created_at": 1468852712
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 6a7a1815fac540ed82dbcbd8bee21b69d64a5e735807b40005c10c854f403796:9fe9511c2aeb5226c495ccc3e165529d7c509db14313ffaa0ad38602bc17adf1
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
{"grant_type":"client_credentials","client_id":"743a05b2c9b8c00afa16e38bac42c753932f71ae339a6ca3870cac8ce58a1206","client_secret":"aeed481874b236d017fbb483a24f7e60f95e3bbc0be366a793bdcf270b234089"}
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
  "access_token": "e02013995500450483e3d9affb89d02672ba57fef72f1f9fc6c64eaac79f2d4b",
  "token_type": "bearer",
  "created_at": 1468852712
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"743a05b2c9b8c00afa16e38bac42c753932f71ae339a6ca3870cac8ce58a1206","client_secret":"aeed481874b236d017fbb483a24f7e60f95e3bbc0be366a793bdcf270b234089"}' -X POST \
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
GET /v2/campaigns/1
Content-Type: application/json
Authorization: Bearer c0f24378af776732ae56e6083210ed2196b92fd73fc5720a7449d81cfcc3e76f
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
    "id": 1,
    "title": "Recruiting pastry chefs",
    "company_id": 5,
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
curl "api.goskive.com/v2/campaigns/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0f24378af776732ae56e6083210ed2196b92fd73fc5720a7449d81cfcc3e76f"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/16/flashcards
Content-Type: application/json
Authorization: Bearer 804fb43f4beb0bb0e7105ba609eb911c751b364fe48f60e4b016e6429a47d0c3
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":16,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content] *required* | Front Content Markdown |
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content] *required* | Back Content Markdown |
| flashcard[back_content_html] *required* | Back Content HTML |
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 87,
    "chapter_id": 16,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:32.615Z",
    "created_at": "2016-07-18T14:37:32.615Z",
    "tags": [

    ],
    "reported": false,
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
curl "api.goskive.com/v2/chapters/16/flashcards" -d '{"flashcard":{"chapter_id":16,"front_content":"Function of *eggs* in choux pastry","front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content":"Helps things *raise*","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 804fb43f4beb0bb0e7105ba609eb911c751b364fe48f60e4b016e6429a47d0c3"
```
## Create a flashcard with images


### Request

#### Endpoint

```
POST /v2/chapters/17/flashcards
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 51f27bcf69454607d27dbfff43b7e4daf94c9f4a1ab4ba9f2f9ea40a3e5257a8
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

17
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
| flashcard[front_content] *required* | Front Content Markdown |
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content] *required* | Back Content Markdown |
| flashcard[back_content_html] *required* | Back Content HTML |
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
    "id": 14,
    "obfuscated_id": "gbKzjBR_8tw",
    "author_id": 90,
    "chapter_id": 17,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:33.202Z",
    "created_at": "2016-07-18T14:37:33.202Z",
    "tags": [

    ],
    "reported": false,
    "published": false,
    "language_code": "fr",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/fb9eca73d5ca70238c11cab38851fce8992132e3.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/e1ca4904d6ed4d028d256c87bae13b6d8411ce9c.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/fb9eca73d5ca70238c11cab38851fce8992132e3.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/e1ca4904d6ed4d028d256c87bae13b6d8411ce9c.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/17/flashcards" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="flashcard[chapter_id]"

17
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
	-H "Authorization: Bearer 51f27bcf69454607d27dbfff43b7e4daf94c9f4a1ab4ba9f2f9ea40a3e5257a8"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/18/flashcards
Content-Type: application/json
Authorization: Bearer 3befd296d68bbf1776146f3d46fd3234cfe7900060381dccbcc71f63efb88fd0
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 91,
      "chapter_id": 18,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:33.421Z",
      "created_at": "2016-07-18T14:37:33.421Z",
      "tags": [

      ],
      "reported": false,
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 91,
      "chapter_id": 18,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:33.443Z",
      "created_at": "2016-07-18T14:37:33.443Z",
      "tags": [

      ],
      "reported": false,
      "published": true,
      "language_code": "de",
      "front_content": "So we have a weird question here…  with *weird* **markup**!",
      "back_content": "This is **nice** back content!",
      "front_content_html": "<p>I'm the content</p>",
      "back_content_html": "<p>I'm the content</p>"
    },
    {
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 91,
      "chapter_id": 18,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:33.466Z",
      "created_at": "2016-07-18T14:37:33.466Z",
      "tags": [

      ],
      "reported": false,
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
curl "api.goskive.com/v2/chapters/18/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3befd296d68bbf1776146f3d46fd3234cfe7900060381dccbcc71f63efb88fd0"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/27/questions
Content-Type: application/json
Authorization: Bearer 4c4e70aff0ec849db991061687acab0cc1d6d2d2400bf361a3b660e31368d516
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":27,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 12,
    "obfuscated_id": "4vzz6KHlMwo",
    "author_id": 130,
    "chapter_id": 27,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:47.839Z",
    "created_at": "2016-07-18T14:37:47.839Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 24,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 25,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 26,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 27,
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
curl "api.goskive.com/v2/chapters/27/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":27,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c4e70aff0ec849db991061687acab0cc1d6d2d2400bf361a3b660e31368d516"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/25/questions
Content-Type: application/json
Authorization: Bearer 19007c50ed5166d134e9fdba46c8414056ef25f20e5246789075ae5d74036577
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":25,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 10,
    "obfuscated_id": "aY5v9ahzH5c",
    "author_id": 124,
    "chapter_id": 25,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:47.226Z",
    "created_at": "2016-07-18T14:37:47.226Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 19,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 20,
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
curl "api.goskive.com/v2/chapters/25/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":25,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19007c50ed5166d134e9fdba46c8414056ef25f20e5246789075ae5d74036577"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/26/questions
Content-Type: application/json
Authorization: Bearer b05d79ea8ad73eefa728d19b0a9626739a26b1973650ea780bfe5a81c4f134a8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":26,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
```


| Name | Description |
|:-----|:------------|
| question[question] *required* | Question Markdown |
| question[question_html] *required* | Question HTML |
| question[explanation] *required* | Explanation Markdown |
| question[explanation_html] *required* | Explanation HTML |
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
    "id": 11,
    "obfuscated_id": "KS_N8rRWCuE",
    "author_id": 127,
    "chapter_id": 26,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:47.481Z",
    "created_at": "2016-07-18T14:37:47.481Z",
    "tags": [

    ],
    "reported": false,
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
        "id": 21,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 22,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 23,
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
curl "api.goskive.com/v2/chapters/26/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":26,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b05d79ea8ad73eefa728d19b0a9626739a26b1973650ea780bfe5a81c4f134a8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/29/questions
Content-Type: application/json
Authorization: Bearer d48cc1adf8fe98ccc7da7cd18ce82b1378df89563d38b8a32b57e426c5531a82
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 136,
      "chapter_id": 29,
      "position": 10,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:48.327Z",
      "created_at": "2016-07-18T14:37:48.295Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 28,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 29,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 137,
      "chapter_id": 29,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:48.405Z",
      "created_at": "2016-07-18T14:37:48.374Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 30,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 31,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 138,
      "chapter_id": 29,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-07-18T14:37:48.485Z",
      "created_at": "2016-07-18T14:37:48.453Z",
      "tags": [

      ],
      "reported": false,
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
          "id": 32,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 33,
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
curl "api.goskive.com/v2/chapters/29/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d48cc1adf8fe98ccc7da7cd18ce82b1378df89563d38b8a32b57e426c5531a82"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/80
Content-Type: application/json
Authorization: Bearer c7020d6aad0c1b29c498f0589b5b7bf3246c55eed7ebad5019776bdd78273c88
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
curl "api.goskive.com/v2/chapters/80" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7020d6aad0c1b29c498f0589b5b7bf3246c55eed7ebad5019776bdd78273c88"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/81
Content-Type: application/json
Authorization: Bearer bd76ab468d85cad1858542ea0fdabdda00f290928439427de6acba7ec38b89ee
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
curl "api.goskive.com/v2/chapters/81" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd76ab468d85cad1858542ea0fdabdda00f290928439427de6acba7ec38b89ee"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/76
Content-Type: application/json
Authorization: Bearer b1954093ca81c569f68e556290ff2498061eb8aeb233538ea25de4a80a2e8419
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
curl "api.goskive.com/v2/chapters/76" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1954093ca81c569f68e556290ff2498061eb8aeb233538ea25de4a80a2e8419"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/79
Content-Type: application/json
Authorization: Bearer d238c7ecd7ba3f54efd8a83164219d8163398e1e455257c498e1972bca1ef450
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/79" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d238c7ecd7ba3f54efd8a83164219d8163398e1e455257c498e1972bca1ef450"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/83
Content-Type: application/json
Authorization: Bearer 8f7f6f8cfc1220232e81ee25c54ef6c808813d077ca7196338d663fb76c29a3c
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
    "id": 83,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-07-18T14:38:10.046Z",
    "course_id": 167,
    "author_id": 464,
    "permissions": [

    ],
    "flashcards_updated_at": "2015-03-12T13:59:00.000Z",
    "questions_updated_at": "2015-04-12T13:59:00.000Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 468,
        "chapter_id": 83,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-07-18T14:38:10.040Z",
        "tags": [

        ],
        "reported": false,
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 466,
        "chapter_id": 83,
        "position": 23,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-07-18T14:38:09.900Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 54,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 55,
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
curl "api.goskive.com/v2/chapters/83" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f7f6f8cfc1220232e81ee25c54ef6c808813d077ca7196338d663fb76c29a3c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/77
Content-Type: application/json
Authorization: Bearer 0777af8a7d3d917abf592e3e5f4a43182d86f8ff96ae1362797979c3132d1994
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
    "id": 77,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-07-18T14:38:08.323Z",
    "course_id": 161,
    "author_id": 447,
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
curl "api.goskive.com/v2/chapters/77" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0777af8a7d3d917abf592e3e5f4a43182d86f8ff96ae1362797979c3132d1994"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/48/replies
Content-Type: application/json
Authorization: Bearer 9ac5435a66515ec5fe02d3aa7dd906b421611264a6f224a3ffbecf327ef8f843
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
    "id": 49,
    "author_id": 506,
    "reply_to_id": 48,
    "created_at": "2016-07-18T14:38:13.358Z",
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
curl "api.goskive.com/v2/comments/48/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ac5435a66515ec5fe02d3aa7dd906b421611264a6f224a3ffbecf327ef8f843"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/50/replies
Content-Type: application/json
Authorization: Bearer b4dbcd8d17ffd064636ee784b7cc689a225eb01013bab674ced4af326ac5da91
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
curl "api.goskive.com/v2/comments/50/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4dbcd8d17ffd064636ee784b7cc689a225eb01013bab674ced4af326ac5da91"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 846e7ccc8f4d8a00b718954a424a5c50bc8184bbf7c9eff3a07a1fa5501e1e33
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
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 846e7ccc8f4d8a00b718954a424a5c50bc8184bbf7c9eff3a07a1fa5501e1e33"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/7/republish
Content-Type: application/json
Authorization: Bearer b4d87c10d524d04965efee6d05a00b277b1c51b82dd87607a87aac4fe4498db6
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
	-H "Authorization: Bearer b4d87c10d524d04965efee6d05a00b277b1c51b82dd87607a87aac4fe4498db6"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer 52162731452ee28fe99df5ff79ff5ed7585306555e8482c197c650149ce1c91b
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
	-H "Authorization: Bearer 52162731452ee28fe99df5ff79ff5ed7585306555e8482c197c650149ce1c91b"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/44/report
Content-Type: application/json
Authorization: Bearer a8f919dcdcde03ca9b5ca8bd29aba515e60507c14128922aa6bfd02f91356ad3
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8f919dcdcde03ca9b5ca8bd29aba515e60507c14128922aa6bfd02f91356ad3"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer 7bf875491b44f5b5068a35a1d22d1703fc72d84c603512cc385f4fbea345a80b
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
    "id": 4,
    "name": "Pastry Corp",
    "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-07-18T14:37:27.079Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7bf875491b44f5b5068a35a1d22d1703fc72d84c603512cc385f4fbea345a80b"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 9cf0d78809bf34e36b8ad19585071958ce06a6cbcd741ba11966faaddfa2e84e
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
      "id": 1,
      "name": "Fake Company Name 1",
      "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
      "brand_color": "#000000",
      "updated_at": "2016-07-18T14:37:26.896Z"
    },
    {
      "id": 2,
      "name": "Fake Company Name 2",
      "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-07-18T14:37:26.903Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 3",
      "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-07-18T14:37:26.910Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cf0d78809bf34e36b8ad19585071958ce06a6cbcd741ba11966faaddfa2e84e"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 2174340bac8982e8d8465e7a5bb633688c8bf3724d607ae52bd02bc5f3477d36
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
      "id": 11,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/6557160cf523e6b44ee9eac06061463b0fcbd3b1.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/f4961300e395cd3802066da84ade8e1cdd20826f.png",
      "widgets": [

      ]
    },
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
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/653938ceeed87e42b62d7feeca02cd82da1acb27.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/d204067fe9ed5e993ed4b1188ce57016fdd8b991.png",
      "widgets": [

      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2174340bac8982e8d8465e7a5bb633688c8bf3724d607ae52bd02bc5f3477d36"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/28/company_profiles
Content-Type: application/json
Authorization: Bearer d52dce042e7ab5e4ecd015e2020190b5ef8e5b3b1d9368992a8d9afcce5c8d92
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
      "id": 7,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/9d765d9b895a77cd295c7f5e57af933f977bb87f.png",
      "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/648481f5d8c76852bca2fea2b305e3b694878255.png",
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
curl "api.goskive.com/v2/companies/28/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d52dce042e7ab5e4ecd015e2020190b5ef8e5b3b1d9368992a8d9afcce5c8d92"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer c851585201921aa8ff9159aa759d7bfca9be44789f91338b9716ad789cdc0f4f
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 16,
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
          "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/3e3de85f9259343d03d531c0557570e70612c274.png",
          "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/9df145d07eb8d34190b3b56db5884a14a6e7644c.png",
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
      "id": 7,
      "title": "Campaign 6",
      "company_id": 19,
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
          "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/b7227ba08020eaf424f385a68712e11390fe76a3.png",
          "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/15a47e0f0d046fb9c95772f170325321f8fb4d6d.png",
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
	-H "Authorization: Bearer c851585201921aa8ff9159aa759d7bfca9be44789f91338b9716ad789cdc0f4f"
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
Authorization: Bearer 0b1a10992614782d88e269615ae7344309ca73689478d44af784edd6939d9121
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
	-H "Authorization: Bearer 0b1a10992614782d88e269615ae7344309ca73689478d44af784edd6939d9121"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 349148230d6a9e4280e2a4e014569896ca800c0bde9b0fbf35cedd836637545b
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
    "id": 119,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-07-18T14:38:23.972Z",
    "course_id": 218,
    "author_id": 622,
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
	-H "Authorization: Bearer 349148230d6a9e4280e2a4e014569896ca800c0bde9b0fbf35cedd836637545b"
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
      "id": 130,
      "title": "Clever Chapter Title 106",
      "position": 1,
      "updated_at": "2016-07-18T14:38:25.487Z",
      "course_id": 225,
      "author_id": 647,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 131,
      "title": "Clever Chapter Title 107",
      "position": 2,
      "updated_at": "2016-07-18T14:38:25.519Z",
      "course_id": 225,
      "author_id": 648,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 108",
      "position": 3,
      "updated_at": "2016-07-18T14:38:25.685Z",
      "course_id": 225,
      "author_id": 649,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-07-18T14:38:25.671Z",
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
Authorization: Bearer d256fa26bd4dfca6389fde0510ff7c165374bb5efb0dffcfd8fda93738cee4f8
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
      "id": 136,
      "title": "Clever Chapter Title 112",
      "position": 1,
      "updated_at": "2016-07-18T14:38:26.141Z",
      "course_id": 228,
      "author_id": 658,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 137,
      "title": "Clever Chapter Title 113",
      "position": 2,
      "updated_at": "2016-07-18T14:38:26.169Z",
      "course_id": 228,
      "author_id": 659,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 138,
      "title": "Clever Chapter Title 114",
      "position": 3,
      "updated_at": "2016-07-18T14:38:26.330Z",
      "course_id": 228,
      "author_id": 660,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": "2016-07-18T14:38:26.316Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d256fa26bd4dfca6389fde0510ff7c165374bb5efb0dffcfd8fda93738cee4f8"
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
      "id": 133,
      "title": "Clever Chapter Title 109",
      "position": 1,
      "updated_at": "2016-07-18T14:38:25.926Z",
      "course_id": 227,
      "author_id": 654,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 134,
      "title": "Clever Chapter Title 110",
      "position": 2,
      "updated_at": "2016-07-18T14:38:25.954Z",
      "course_id": 227,
      "author_id": 655,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 135,
      "title": "Clever Chapter Title 111",
      "position": 3,
      "updated_at": "2016-07-18T14:38:25.982Z",
      "course_id": 227,
      "author_id": 656,
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
Authorization: Bearer 929121d6170c2e62f0e224f5c1928082dd0f9f088f41623170c0060442791d88
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
      "id": 139,
      "title": "Clever Chapter Title 115",
      "position": 1,
      "updated_at": "2016-07-18T14:38:26.553Z",
      "course_id": 229,
      "author_id": 665,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 140,
      "title": "Clever Chapter Title 116",
      "position": 2,
      "updated_at": "2016-07-18T14:38:26.583Z",
      "course_id": 229,
      "author_id": 666,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 141,
      "title": "Clever Chapter Title 117",
      "position": 3,
      "updated_at": "2016-07-18T14:38:26.613Z",
      "course_id": 229,
      "author_id": 667,
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
	-H "Authorization: Bearer 929121d6170c2e62f0e224f5c1928082dd0f9f088f41623170c0060442791d88"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d4edd6faf745ded3631fec214e5b9f50f604533fad8da94528cfa65f637c313e
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
    "id": 7,
    "course_id": 250,
    "user_id": 749,
    "updated_at": "2016-07-18T14:38:36.770Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4edd6faf745ded3631fec214e5b9f50f604533fad8da94528cfa65f637c313e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer bcb4b1ff95715a9ad9e6090c4e2663d766458b5349c20bf6fcd0d7ee0c5d5f3d
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
      "id": 4,
      "course_id": 248,
      "user_id": 743,
      "updated_at": "2016-07-18T14:38:36.333Z"
    },
    {
      "id": 5,
      "course_id": 248,
      "user_id": 744,
      "updated_at": "2016-07-18T14:38:36.353Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcb4b1ff95715a9ad9e6090c4e2663d766458b5349c20bf6fcd0d7ee0c5d5f3d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer c25800c27ba8d3e730ccf4729d29b95ce770b664f8df6b124292915f0d8c2d98
```

`DELETE /v2/course_requests/:course_request_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/course_requests/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c25800c27ba8d3e730ccf4729d29b95ce770b664f8df6b124292915f0d8c2d98"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e8173c9f662a483d17a4d54333fbf49b3497dcfbf9e7b0aac72c4557ef5321db
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
	-H "Authorization: Bearer e8173c9f662a483d17a4d54333fbf49b3497dcfbf9e7b0aac72c4557ef5321db"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ad4ad34649820bb8efaebecda5634dd90e73d284eb774859d72774dbb911fa7e
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
	-H "Authorization: Bearer ad4ad34649820bb8efaebecda5634dd90e73d284eb774859d72774dbb911fa7e"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 702156c35b7e2871239ab4ff1a492606b7b7d033c62f55f2e163e38f35933150
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
	-H "Authorization: Bearer 702156c35b7e2871239ab4ff1a492606b7b7d033c62f55f2e163e38f35933150"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 827a5cc0d170df9669bd9d2d55026b6bf9850f099e0aec1aaa0670fa9fb20939
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
	-H "Authorization: Bearer 827a5cc0d170df9669bd9d2d55026b6bf9850f099e0aec1aaa0670fa9fb20939"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer f9ce0ff90cd9dee5f30aaf555620ecea4ee80b63b7d34c80aebdb3bb63d715df
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
    "creator_id": 784,
    "id": 259,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 244,
    "additional_university_ids": [

    ],
    "topic_id": 271,
    "discipline_id": 272,
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
    "chapters_updated_at": "2016-07-18T14:38:41.958Z",
    "updated_at": "2016-07-18T14:38:41.961Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 166,
        "title": "Clever Chapter Title 142",
        "position": 1,
        "updated_at": "2016-07-18T14:38:41.917Z",
        "course_id": 259,
        "author_id": 784,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-07-18T14:38:41.815Z",
        "questions_updated_at": "2016-07-18T14:38:41.410Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 167,
        "title": "Clever Chapter Title 143",
        "position": 2,
        "updated_at": "2016-07-18T14:38:41.958Z",
        "course_id": 259,
        "author_id": 784,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-07-18T14:38:41.869Z",
        "questions_updated_at": "2016-07-18T14:38:41.576Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 785,
        "chapter_id": 166,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.784Z",
        "created_at": "2016-07-18T14:38:41.784Z",
        "tags": [

        ],
        "reported": false,
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 785,
        "chapter_id": 167,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.838Z",
        "created_at": "2016-07-18T14:38:41.838Z",
        "tags": [

        ],
        "reported": false,
        "published": true,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 785,
        "chapter_id": 166,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.815Z",
        "created_at": "2016-07-18T14:38:41.815Z",
        "tags": [

        ],
        "reported": false,
        "published": false,
        "language_code": "de",
        "front_content": "So we have a weird question here…  with *weird* **markup**!",
        "back_content": "This is **nice** back content!",
        "front_content_html": "<p>I'm the content</p>",
        "back_content_html": "<p>I'm the content</p>"
      },
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 785,
        "chapter_id": 167,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.869Z",
        "created_at": "2016-07-18T14:38:41.869Z",
        "tags": [

        ],
        "reported": false,
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
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 785,
        "chapter_id": 166,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.334Z",
        "created_at": "2016-07-18T14:38:41.300Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 195,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 196,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 97,
        "obfuscated_id": "qdTHUgSdSV8",
        "author_id": 785,
        "chapter_id": 166,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.410Z",
        "created_at": "2016-07-18T14:38:41.377Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 197,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 198,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 98,
        "obfuscated_id": "icApzX10lRE",
        "author_id": 785,
        "chapter_id": 167,
        "position": 86,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.500Z",
        "created_at": "2016-07-18T14:38:41.466Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 199,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 200,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 785,
        "chapter_id": 167,
        "position": 87,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:41.576Z",
        "created_at": "2016-07-18T14:38:41.542Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 201,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 202,
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
	-H "Authorization: Bearer f9ce0ff90cd9dee5f30aaf555620ecea4ee80b63b7d34c80aebdb3bb63d715df"
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
    "creator_id": 779,
    "id": 258,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 243,
    "additional_university_ids": [

    ],
    "topic_id": 270,
    "discipline_id": 271,
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
    "chapters_updated_at": "2016-07-18T14:38:41.101Z",
    "updated_at": "2016-07-18T14:38:41.104Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 164,
        "title": "Clever Chapter Title 140",
        "position": 1,
        "updated_at": "2016-07-18T14:38:41.060Z",
        "course_id": 258,
        "author_id": 779,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-07-18T14:38:40.927Z",
        "questions_updated_at": "2016-07-18T14:38:40.475Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 165,
        "title": "Clever Chapter Title 141",
        "position": 2,
        "updated_at": "2016-07-18T14:38:41.101Z",
        "course_id": 258,
        "author_id": 779,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-07-18T14:38:40.982Z",
        "questions_updated_at": "2016-07-18T14:38:40.640Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 779,
        "chapter_id": 164,
        "position": 78,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:40.475Z",
        "created_at": "2016-07-18T14:38:40.440Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 183,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 184,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 779,
        "chapter_id": 165,
        "position": 80,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-07-18T14:38:40.640Z",
        "created_at": "2016-07-18T14:38:40.608Z",
        "tags": [

        ],
        "reported": false,
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
            "id": 187,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 188,
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
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/274/pin
Content-Type: application/json
Authorization: Bearer 8347c9771edaeed88d767e841bd220a221b435baf73f2e53064602e254c74321
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/274/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8347c9771edaeed88d767e841bd220a221b435baf73f2e53064602e254c74321"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/273/pin
Content-Type: application/json
Authorization: Bearer 2d2f94c4890c7afb62c0f797249d826fbbf1ff5d308be9a0f86e7f919e5452f8
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/273/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d2f94c4890c7afb62c0f797249d826fbbf1ff5d308be9a0f86e7f919e5452f8"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 44de557228a7e7af0b8332b8c3cc63c352147f22f856ceede7f443ec913b0e8b
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
    "creator_id": 796,
    "id": 263,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 248,
    "additional_university_ids": [

    ],
    "topic_id": 275,
    "discipline_id": 276,
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
    "updated_at": "2016-07-18T14:38:42.746Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44de557228a7e7af0b8332b8c3cc63c352147f22f856ceede7f443ec913b0e8b"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1282390455c02e3cb52721749cd0afbe3cbc0fdbd2def645c0208ad670f9b7eb
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
    "id": 157,
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
    "created_at": "2016-07-18T14:37:50.757Z",
    "updated_at": "2016-07-18T14:37:50.757Z",
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
	-H "Authorization: Bearer 1282390455c02e3cb52721749cd0afbe3cbc0fdbd2def645c0208ad670f9b7eb"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c804572441dd67f03063c321de34a593fed8a5b744b4a5a0778bb53e5bc031f2
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[72]}
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
    "id": 153,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      72
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-07-18T14:37:50.400Z",
    "updated_at": "2016-07-18T14:37:50.453Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[72]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c804572441dd67f03063c321de34a593fed8a5b744b4a5a0778bb53e5bc031f2"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f7c88659b2b59078784ff415ebd2b3fae34617802d39f12c1475da5ff68ac285
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
    "id": 156,
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
    "created_at": "2016-07-18T14:37:50.666Z",
    "updated_at": "2016-07-18T14:37:50.666Z",
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
	-H "Authorization: Bearer f7c88659b2b59078784ff415ebd2b3fae34617802d39f12c1475da5ff68ac285"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d31f05166708207a4bc33967847e4123ba7402a8a3c149fb397a066a89133000
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[74]}
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
    "id": 155,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      74
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-07-18T14:37:50.601Z",
    "updated_at": "2016-07-18T14:37:50.601Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[74]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d31f05166708207a4bc33967847e4123ba7402a8a3c149fb397a066a89133000"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a645bdc44c0735e6abc9e3df9ac18114a1dc7ad61ab11cd64f71240705682dbe
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

71
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
    "id": 152,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/thumb/a534a0653fa5fa2d35490d342d01de8fad81c6c9.jpg",
    "university_id": null,
    "fields_of_study": [
      71
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-07-18T14:37:49.947Z",
    "updated_at": "2016-07-18T14:37:50.308Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/students/original/b7023da0ea3de0b4a25b2a989b782f6ec4f3679f.jpg",
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

71
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a645bdc44c0735e6abc9e3df9ac18114a1dc7ad61ab11cd64f71240705682dbe"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 638189fe8ea5e2af678a298490527bb2620fdbe7f4e0fe814f846cb78d9f195b
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
      "id": 6,
      "bookmarkable_id": 104,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 105,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 106,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 638189fe8ea5e2af678a298490527bb2620fdbe7f4e0fe814f846cb78d9f195b"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 4ac61597db006281747c07c94dc70a1880a3675a86b855d8e88a40bd2c71b5d5
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
      "id": 2,
      "title": "Campaign 1",
      "company_id": 6,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 1,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/0adf1955ecfb39ff0d02f85dd384e7aeaf694927.png",
          "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/39195f7a12fa003c1584dcee68597ed4a180cb4b.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/8dbf7d28f3cbdc6d654d6324af20a11fe3653b85.png",
          "target_url": "http://goskive.com",
          "id": 1,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 3,
      "title": "Campaign 2",
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
          "id": 2,
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/9eceef98bbb4cbbf925777c91787755d8353de98.png",
          "header_image_hires_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/company_profiles/original/a56a082a30d2de9bc36364cd610c75501bd3b7d5.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/889019b341716d48f4f28718872d4f688cd18499.png",
          "target_url": "http://goskive.com",
          "id": 2,
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
	-H "Authorization: Bearer 4ac61597db006281747c07c94dc70a1880a3675a86b855d8e88a40bd2c71b5d5"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer bff2e0bfb46732f713f331a361bc3410ede8f65fe7993a826fdc4518662ec8b0
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
      "creator_id": 159,
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-54",
      "html_url": "https://goskive.com/course/mit-course-54",
      "slug": "mit-course-54",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 77,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 54",
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
      "updated_at": "2016-07-18T14:37:50.924Z",
      "shortname": "mit-course-54"
    },
    {
      "creator_id": 160,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-55",
      "html_url": "https://goskive.com/course/mit-course-55",
      "slug": "mit-course-55",
      "university_id": 47,
      "additional_university_ids": [

      ],
      "topic_id": 77,
      "discipline_id": 78,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 55",
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
      "updated_at": "2016-07-18T14:37:51.017Z",
      "shortname": "mit-course-55"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bff2e0bfb46732f713f331a361bc3410ede8f65fe7993a826fdc4518662ec8b0"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer eac7ff5472d6fc40be4b1a360f3f99113910b5dcf019edf618e782637952ea65
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
      "id": 1,
      "title": "Job Posting1",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 8",
        "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-07-18T14:37:49.654Z"
      },
      "created_at": "2016-07-18T14:37:49.659Z",
      "updated_at": "2016-07-18T14:37:49.659Z"
    },
    {
      "id": 1,
      "title": "Job Posting1",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 8",
        "logo_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-07-18T14:37:49.654Z"
      },
      "created_at": "2016-07-18T14:37:49.659Z",
      "updated_at": "2016-07-18T14:37:49.659Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eac7ff5472d6fc40be4b1a360f3f99113910b5dcf019edf618e782637952ea65"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer c1858a4d2178561572a6338b0d584f5517d278929cd1031f1d6373b6287e8864
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
      "id": 6,
      "created_at": "2016-07-18T14:38:05.076Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 45,
      "updated_at": "2016-07-18T14:38:05.202Z",
      "author_id": "397",
      "thread_subject_id": "148",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 7,
      "created_at": "2016-07-18T14:38:05.187Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 46,
      "updated_at": "2016-07-18T14:38:05.207Z",
      "author_id": "400",
      "thread_subject_id": "149",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-07-18T14:38:05.431Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-07-18T14:38:05.431Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 9,
      "created_at": "2016-07-18T14:38:05.658Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-07-18T14:38:05.658Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 10,
      "created_at": "2016-07-18T14:38:05.885Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-07-18T14:38:05.885Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 11,
      "created_at": "2016-07-18T14:38:06.080Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-07-18T14:38:06.080Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-07-18T14:38:06.274Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 21,
      "updated_at": "2016-07-18T14:38:06.274Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 13,
      "created_at": "2016-07-18T14:38:06.466Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 22,
      "updated_at": "2016-07-18T14:38:06.466Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1858a4d2178561572a6338b0d584f5517d278929cd1031f1d6373b6287e8864"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer 3f0a8f07e73ea3ca04c5451e2fd7167f87bb4bfad5b9be472396a3f15d808ab0
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-07-18T14:28:06.000Z"}}
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
    "id": 14,
    "created_at": "2016-07-18T14:38:06.734Z",
    "read_at": "2016-07-18T14:28:06.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 47,
    "updated_at": "2016-07-18T14:38:06.782Z",
    "author_id": "426",
    "thread_subject_id": "156",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-07-18T14:28:06.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f0a8f07e73ea3ca04c5451e2fd7167f87bb4bfad5b9be472396a3f15d808ab0"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0567dcb0f90606b734bd917483607cbaeed4f8bcfe7e8ea6ce70fa84d097b510
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
      "course_id": 175,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-07-18T14:38:12.006Z",
      "course_published": true,
      "updated_at": "2016-07-18T14:38:11.993Z"
    },
    {
      "id": 9,
      "course_id": 176,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-07-18T14:38:12.102Z",
      "course_published": true,
      "updated_at": "2016-07-18T14:38:12.089Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0567dcb0f90606b734bd917483607cbaeed4f8bcfe7e8ea6ce70fa84d097b510"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/10
Content-Type: application/json
Authorization: Bearer 49d902d04605b614d136b92f0231bb14f38a6037fe5ca9cb404da046b5527361
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
    "id": 10,
    "course_id": 177,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-07-18T14:38:12.248Z",
    "course_published": true,
    "updated_at": "2016-07-18T14:38:12.236Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49d902d04605b614d136b92f0231bb14f38a6037fe5ca9cb404da046b5527361"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/11
Content-Type: application/json
Authorization: Bearer a4f64cd5c4fb9aea2a22a6c8f847a39c4280bdf849b88d81ff218f2fc0084603
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
    "id": 11,
    "course_id": 178,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-07-18T14:38:12.447Z",
    "course_published": true,
    "updated_at": "2016-07-18T14:38:12.439Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/11" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4f64cd5c4fb9aea2a22a6c8f847a39c4280bdf849b88d81ff218f2fc0084603"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 9a74231b52dde00db9657a17c34ed13f3e2334a6ed50500ea789193ae2c0145a
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
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 6,
      "user_id": 109
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 7,
      "user_id": 109
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 8,
      "user_id": 109
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 9,
      "user_id": 109
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a74231b52dde00db9657a17c34ed13f3e2334a6ed50500ea789193ae2c0145a"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/53
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
    "id": 53,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 53,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 53
      },
      {
        "id": 54,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 53
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/53" -X GET \
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
      "id": 54,
      "name": "De-engineered dynamic software",
      "name_translations": {
        "en": "De-engineered dynamic software"
      }
    },
    {
      "id": 55,
      "name": "Inverse optimal conglomeration",
      "name_translations": {
        "en": "Inverse optimal conglomeration"
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
PATCH /v2/feedbacks/11/close
Content-Type: application/json
Authorization: Bearer a659ac1ef45ce3c39083843baa1915dea3c8839d491ae42e35f9a41375095518
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
    "id": 11,
    "user_id": 175,
    "feedbackable_id": 20,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-07-18T14:37:51.896Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/11/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a659ac1ef45ce3c39083843baa1915dea3c8839d491ae42e35f9a41375095518"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/14/fix
Content-Type: application/json
Authorization: Bearer 8fdb104045a76778929d41409f452a2962c97587e42fd79870fbddd7e418b033
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
    "id": 14,
    "user_id": 192,
    "feedbackable_id": 23,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-07-18T14:37:52.738Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/14/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fdb104045a76778929d41409f452a2962c97587e42fd79870fbddd7e418b033"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/12
Content-Type: application/json
Authorization: Bearer e0e620b9016c6b339193e0f485f782e7bae38d0c2b4323d44b77e861a2a6dd4a
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
    "user_id": 180,
    "feedbackable_id": 21,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-07-18T14:37:52.215Z",
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
curl "api.goskive.com/v2/feedbacks/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0e620b9016c6b339193e0f485f782e7bae38d0c2b4323d44b77e861a2a6dd4a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/17/fix
Content-Type: application/json
Authorization: Bearer 7c6e0d14668010844e931eefe63d506048b0bfa365f7a68a7dc5a99c49f61f5c
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
curl "api.goskive.com/v2/feedbacks/17/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c6e0d14668010844e931eefe63d506048b0bfa365f7a68a7dc5a99c49f61f5c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/9/close
Content-Type: application/json
Authorization: Bearer 10ef42407ad0d61c93d07a1717ab640348cae70ea34c11ebe457a37bfc9c5510
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
curl "api.goskive.com/v2/feedbacks/9/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10ef42407ad0d61c93d07a1717ab640348cae70ea34c11ebe457a37bfc9c5510"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/fix
Content-Type: application/json
Authorization: Bearer bfe692760aa0850703d067e408d89610dc70afd0cff7ac9de431883e1a8bc3ce
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
curl "api.goskive.com/v2/feedbacks/16/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfe692760aa0850703d067e408d89610dc70afd0cff7ac9de431883e1a8bc3ce"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/13
Content-Type: application/json
Authorization: Bearer 29adef3ec0a7a96679dcec1f66487240e74c676206116bafda90b66fd49ebe4f
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
    "id": 13,
    "user_id": 185,
    "feedbackable_id": 22,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-07-18T14:37:52.529Z",
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
curl "api.goskive.com/v2/feedbacks/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29adef3ec0a7a96679dcec1f66487240e74c676206116bafda90b66fd49ebe4f"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/68/comments
Content-Type: application/json
Authorization: Bearer 5625e3f898336fedc75563cd1374c811193860383a55d6bafbc7cf0b90499d90
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
    "id": 56,
    "author_id": 723,
    "reply_to_id": null,
    "created_at": "2016-07-18T14:38:31.903Z",
    "status": "published",
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
curl "api.goskive.com/v2/flashcards/68/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5625e3f898336fedc75563cd1374c811193860383a55d6bafbc7cf0b90499d90"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/67/comments
Content-Type: application/json
Authorization: Bearer 5ccd086cd919a28b0b1fce62ee47b43895c6dbc1eb399f8aa92c1ec9ae6e348a
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
    "id": 55,
    "author_id": 720,
    "reply_to_id": null,
    "created_at": "2016-07-18T14:38:31.377Z",
    "status": "published",
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 26,
      "user_id": 720,
      "feedbackable_id": 67,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:38:31.374Z",
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
curl "api.goskive.com/v2/flashcards/67/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ccd086cd919a28b0b1fce62ee47b43895c6dbc1eb399f8aa92c1ec9ae6e348a"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/64/comments
Content-Type: application/json
Authorization: Bearer e7ae977b8a04195f7d9808d200205897f97b437bfd8e8f2da371818ee21b5cae
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
      "author_id": 713,
      "reply_to_id": null,
      "created_at": "2016-07-18T14:38:30.747Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 712,
      "reply_to_id": null,
      "created_at": "2016-07-18T14:38:30.720Z",
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
curl "api.goskive.com/v2/flashcards/64/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7ae977b8a04195f7d9808d200205897f97b437bfd8e8f2da371818ee21b5cae"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/66/comments
Content-Type: application/json
Authorization: Bearer 0f77e4fb1c5bccab4bf248cf7ecc6f14e7afbc67bda2cc9d84471600b3be9ae6
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
curl "api.goskive.com/v2/flashcards/66/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f77e4fb1c5bccab4bf248cf7ecc6f14e7afbc67bda2cc9d84471600b3be9ae6"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/feedbacks
Content-Type: application/json
Authorization: Bearer 948086d34f3b3c86071d5f76cdf4c9fa91dd27682c57df86c46f0bdba7c27206
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
    "id": 1,
    "user_id": 1,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-07-18T14:37:24.209Z",
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
curl "api.goskive.com/v2/flashcards/1/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 948086d34f3b3c86071d5f76cdf4c9fa91dd27682c57df86c46f0bdba7c27206"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/5/feedbacks
Content-Type: application/json
Authorization: Bearer 0eac54fa8d81042d8295e95a90192ec484a269f43304b6a33792c9ef78d39d3a
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
      "id": 6,
      "user_id": 19,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:37:26.106Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 18,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:37:26.092Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0eac54fa8d81042d8295e95a90192ec484a269f43304b6a33792c9ef78d39d3a"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/54/votes
Content-Type: application/json
Authorization: Bearer 947804f76ca27bdf543f70b6434ca3d90e21830776451d6c78fd91cf6bb2c66d
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
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 54,
      "user_id": 436
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 54,
      "user_id": 435
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 54,
      "user_id": 434
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/54/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 947804f76ca27bdf543f70b6434ca3d90e21830776451d6c78fd91cf6bb2c66d"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/51/republish
Content-Type: application/json
Authorization: Bearer d35e550658264f1c2f2bdac23cf254f8075eba7352c509e07171448ddf66d247
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
curl "api.goskive.com/v2/flashcards/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d35e550658264f1c2f2bdac23cf254f8075eba7352c509e07171448ddf66d247"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/49/bookmark
Content-Type: application/json
Authorization: Bearer 50218e323a8673df3443b275dbe4ba684e7bbe04f3a6038214b682b0f5c7c9d0
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50218e323a8673df3443b275dbe4ba684e7bbe04f3a6038214b682b0f5c7c9d0"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50
Content-Type: application/json
Authorization: Bearer fda1c9acd3cfd276d7f2568a67e77a5afa5d06f3d5e0ee7f76c0056d7f39edd0
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fda1c9acd3cfd276d7f2568a67e77a5afa5d06f3d5e0ee7f76c0056d7f39edd0"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/downvote
Content-Type: application/json
Authorization: Bearer be47a7427e380cb4cf5524de6d1faa48f6e1fef8bb34671405ddaf68daa707e2
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be47a7427e380cb4cf5524de6d1faa48f6e1fef8bb34671405ddaf68daa707e2"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/30
Content-Type: application/json
Authorization: Bearer e0d2d08a56d034c1373ab58038b9b7ce950767396822fe62df1694c2b803451d
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 222,
    "chapter_id": 42,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:54.969Z",
    "created_at": "2016-07-18T14:37:54.969Z",
    "tags": [

    ],
    "reported": false,
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
curl "api.goskive.com/v2/flashcards/30" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0d2d08a56d034c1373ab58038b9b7ce950767396822fe62df1694c2b803451d"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/27/report
Content-Type: application/json
Authorization: Bearer 069e2e5de41fcd3fb7327d81085c8892add194d7030af5f678286c68fa12fc08
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/27/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 069e2e5de41fcd3fb7327d81085c8892add194d7030af5f678286c68fa12fc08"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/28/bookmark
Content-Type: application/json
Authorization: Bearer a6a31c1d51a60dd67fb83b7dff87cff78f836dcbea2f5a355aa6460c7ca57774
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6a31c1d51a60dd67fb83b7dff87cff78f836dcbea2f5a355aa6460c7ca57774"
```
## Update a flashcard


### Request

#### Endpoint

```
PATCH /v2/flashcards/32
Content-Type: application/json
Authorization: Bearer a927c65579cf18eca6c4c8101f8cf3d03ae5e4d0a5938ce52b0e55e826f61aba
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 228,
    "chapter_id": 44,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:56.037Z",
    "created_at": "2016-07-18T14:37:55.713Z",
    "tags": [

    ],
    "reported": false,
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
curl "api.goskive.com/v2/flashcards/32" -d '{"flashcard":{"back_content":"*rise*","back_content_html":"\u003cstrong\u003erise\u003c/strong\u003e","language_code":"de"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a927c65579cf18eca6c4c8101f8cf3d03ae5e4d0a5938ce52b0e55e826f61aba"
```
## Update a flashcard with images


### Request

#### Endpoint

```
PATCH /v2/flashcards/31
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer e98bed34ff4a694748d2bf0b0b215f0feaee1e41549084bdd4ebedd04e3c9ed5
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 225,
    "chapter_id": 43,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:37:55.517Z",
    "created_at": "2016-07-18T14:37:55.153Z",
    "tags": [

    ],
    "reported": false,
    "published": true,
    "language_code": "de",
    "front_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/9dd4915ff120f758cde497a05e13d256cbb844db.png)",
    "back_content": "![Flashcard Image](file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/1f5bc6d13ce7ba4f700c3746e95b9b1e7ec3e22f.png)",
    "front_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/9dd4915ff120f758cde497a05e13d256cbb844db.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>",
    "back_content_html": "<img src=\"file:///Users/alexbcoles/git-repos/skive-backend/public/system/flashcards/medium_highdpi/1f5bc6d13ce7ba4f700c3746e95b9b1e7ec3e22f.png\" style=\"display: block; margin: 0 auto; max-width: 100%; max-height: 270px;\"/>"
  }
}
```



```shell
curl "api.goskive.com/v2/flashcards/31" -d '------------XnJLe9ZIbbGUYtzPQJ16u1
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
	-H "Authorization: Bearer e98bed34ff4a694748d2bf0b0b215f0feaee1e41549084bdd4ebedd04e3c9ed5"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/29/upvote
Content-Type: application/json
Authorization: Bearer 6f84ed0233f9a00f3034f78c227c207a225b2ebf295cd825632023c4891c47ab
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/29/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f84ed0233f9a00f3034f78c227c207a225b2ebf295cd825632023c4891c47ab"
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/5/sign_ups
Content-Type: application/json
Authorization: Bearer 9d1c1c739ee41092f49403b71d6019b6015946cef150ff93a6658faab8adc50f
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
curl "api.goskive.com/v2/me/jobs/5/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d1c1c739ee41092f49403b71d6019b6015946cef150ff93a6658faab8adc50f"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/6/sign_ups
Content-Type: application/json
Authorization: Bearer c67d3471843c29167a884038f446a77fbcc67f76e3cde363a397028454c11bdf
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
curl "api.goskive.com/v2/me/jobs/6/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c67d3471843c29167a884038f446a77fbcc67f76e3cde363a397028454c11bdf"
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
{"password":{"reset_password_token":"Ycp8UB_xfyvxy9ncvZT1","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "created_at": "2016-07-18T14:37:35.348Z",
  "updated_at": "2016-07-18T14:37:35.795Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "downloaded_courses_count": 0,
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
  "audit_id": 10218
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"Ycp8UB_xfyvxy9ncvZT1","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
{"password":{"reset_password_token":"xob1UCRJ8TrJYbZQsvFx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 99,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-07-18T14:37:35.864Z",
  "updated_at": "2016-07-18T14:37:37.497Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "course_purchases_count": 0,
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "downloaded_courses_count": 0,
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
  "audit_id": 10219
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"xob1UCRJ8TrJYbZQsvFx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/75/comments
Content-Type: application/json
Authorization: Bearer 367c00e474876f401532e29e920438fd9197414af6ba4c9e678e1460fbec9a61
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
    "id": 59,
    "author_id": 758,
    "reply_to_id": null,
    "created_at": "2016-07-18T14:38:37.591Z",
    "status": "published",
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
curl "api.goskive.com/v2/questions/75/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 367c00e474876f401532e29e920438fd9197414af6ba4c9e678e1460fbec9a61"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/76/comments
Content-Type: application/json
Authorization: Bearer f5584fc3ac8b3f04d2be5181ac33d3afd8742a4599f594376864c8f01420d443
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
    "id": 60,
    "author_id": 761,
    "reply_to_id": null,
    "created_at": "2016-07-18T14:38:38.011Z",
    "status": "published",
    "message": "Really bad grammar.",
    "feedback": {
      "id": 27,
      "user_id": 761,
      "feedbackable_id": 76,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:38:38.004Z",
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
curl "api.goskive.com/v2/questions/76/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5584fc3ac8b3f04d2be5181ac33d3afd8742a4599f594376864c8f01420d443"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/74/comments
Content-Type: application/json
Authorization: Bearer 2bfd1e97e85d906d3e9d59bf70b43280f2a158f9b5bdaa8feaffb0e8c1592cc2
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
      "id": 58,
      "author_id": 757,
      "reply_to_id": null,
      "created_at": "2016-07-18T14:38:37.303Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 756,
      "reply_to_id": null,
      "created_at": "2016-07-18T14:38:37.279Z",
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
curl "api.goskive.com/v2/questions/74/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bfd1e97e85d906d3e9d59bf70b43280f2a158f9b5bdaa8feaffb0e8c1592cc2"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/77/comments
Content-Type: application/json
Authorization: Bearer 5864fd71581591266b618e2a5bc51deb713890d34082a03a289a0b4e172a2b20
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
curl "api.goskive.com/v2/questions/77/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5864fd71581591266b618e2a5bc51deb713890d34082a03a289a0b4e172a2b20"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/72/feedbacks
Content-Type: application/json
Authorization: Bearer 530bdc66fc4753f23242dcc04421f86bd4a13428f3e1bb9b7331402a5de537df
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
    "id": 25,
    "user_id": 706,
    "feedbackable_id": 72,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-07-18T14:38:30.342Z",
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
curl "api.goskive.com/v2/questions/72/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 530bdc66fc4753f23242dcc04421f86bd4a13428f3e1bb9b7331402a5de537df"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/70/feedbacks
Content-Type: application/json
Authorization: Bearer aedf852a5b8b5b5b0ca4f1ac9095f998f080b73d676c260965834691f76b2c29
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
      "id": 23,
      "user_id": 702,
      "feedbackable_id": 70,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:38:29.580Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 701,
      "feedbackable_id": 70,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-07-18T14:38:29.558Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/70/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aedf852a5b8b5b5b0ca4f1ac9095f998f080b73d676c260965834691f76b2c29"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/57/votes
Content-Type: application/json
Authorization: Bearer cf415a310fa4f0e15d701714d7282b86c04dc7b674dbcae1f4726bfcc6a48643
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
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 601
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 600
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 599
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/57/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf415a310fa4f0e15d701714d7282b86c04dc7b674dbcae1f4726bfcc6a48643"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/54/republish
Content-Type: application/json
Authorization: Bearer 60dddb8ded142af1c2ae7ab24398f6fe15244830b210a3a1f55198c8551657d2
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
curl "api.goskive.com/v2/questions/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60dddb8ded142af1c2ae7ab24398f6fe15244830b210a3a1f55198c8551657d2"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/50/bookmark
Content-Type: application/json
Authorization: Bearer 0062917f7f4fc45a12cb4a8e46978f8a80b2e08bfc3cad5e5eb0bc205894b505
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0062917f7f4fc45a12cb4a8e46978f8a80b2e08bfc3cad5e5eb0bc205894b505"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/51
Content-Type: application/json
Authorization: Bearer 39253a9a5ee9538d10dc326d4821315d20c1f4ddafcb93c5f8851731f6140cb5
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39253a9a5ee9538d10dc326d4821315d20c1f4ddafcb93c5f8851731f6140cb5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/49/downvote
Content-Type: application/json
Authorization: Bearer 9b7eacb799fdcea11c5fbfe585f2b3ba154892165756560bdb15add3147ba628
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b7eacb799fdcea11c5fbfe585f2b3ba154892165756560bdb15add3147ba628"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/33
Content-Type: application/json
Authorization: Bearer 4968c678f670cd9a368b7d24c0c36fe10e23c6e6cc6a8a438dd2aba2eb6b9b79
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
    "id": 33,
    "obfuscated_id": "sjAD-GXxS8o",
    "author_id": 519,
    "chapter_id": 89,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:38:15.293Z",
    "created_at": "2016-07-18T14:38:15.255Z",
    "tags": [
      {
        "id": 6,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 5,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "reported": false,
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
        "id": 69,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 70,
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
curl "api.goskive.com/v2/questions/33" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4968c678f670cd9a368b7d24c0c36fe10e23c6e6cc6a8a438dd2aba2eb6b9b79"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/52/report
Content-Type: application/json
Authorization: Bearer 5565445200d15700e56da474e064c1dd0b870e559ead1fd75c41df5d762e0489
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5565445200d15700e56da474e064c1dd0b870e559ead1fd75c41df5d762e0489"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/53/bookmark
Content-Type: application/json
Authorization: Bearer a27171d3f74f92d711adcfa1454b843e35770e1f9219acd0fa112eb9f1113393
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/53/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a27171d3f74f92d711adcfa1454b843e35770e1f9219acd0fa112eb9f1113393"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/32
Content-Type: application/json
Authorization: Bearer 4fe4670a8c378d2f8d2d7b202367146d83baabe69a6c6d72fc7f3359ece7eff3
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-07-18T14:38:14.887Z","updated_at":"2016-07-18T14:38:14.921Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":88,"author_id":516,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 516,
    "chapter_id": 88,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-07-18T14:38:15.014Z",
    "created_at": "2016-07-18T14:38:14.887Z",
    "tags": [
      {
        "id": 4,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 3,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "reported": false,
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>32, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-07-18T14:38:14.887Z\", \"updated_at\"=>\"2016-07-18T14:38:14.921Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>88, \"author_id\"=>516, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 66,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 67,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 68,
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
curl "api.goskive.com/v2/questions/32" -d '{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-07-18T14:38:14.887Z","updated_at":"2016-07-18T14:38:14.921Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":88,"author_id":516,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fe4670a8c378d2f8d2d7b202367146d83baabe69a6c6d72fc7f3359ece7eff3"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/31/upvote
Content-Type: application/json
Authorization: Bearer a0c287bcfe5348c464c8ac07acee47cac1ff78edf541fe375dbf9306093b7d2a
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0c287bcfe5348c464c8ac07acee47cac1ff78edf541fe375dbf9306093b7d2a"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer fe70c8bd52d0bf0cec8ad7f8bdfd74dfbb377ada48d4030bdc3980c11d1913cf
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
      "creator_id": 497,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 190,
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
      "updated_at": "2016-07-18T14:38:12.575Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe70c8bd52d0bf0cec8ad7f8bdfd74dfbb377ada48d4030bdc3980c11d1913cf"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 0cb56cc2e3a083cecb89ecdcb82c3efd07a1e4b7e2f5435dab0909758a9b43c9
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
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-146",
      "html_url": "https://goskive.com/university/uni-146",
      "slug": "uni-146",
      "name": "National School of Pizza",
      "short_name": "Uni 146",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/21e377db908ec820a6a5d74f189877b51d0fc45f.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/afdca0056119c90458fa88325a87772fa59363cf.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-07-18T14:38:12.879Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-145",
      "html_url": "https://goskive.com/university/uni-145",
      "slug": "uni-145",
      "name": "National School of Pastry",
      "short_name": "Uni 145",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/d42ffac50a87c2f5f95462aa80d7eef46b931fdc.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/4b22ef9138b10be2b344bf80993382e2349656fe.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-07-18T14:38:12.856Z",
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
	-H "Authorization: Bearer 0cb56cc2e3a083cecb89ecdcb82c3efd07a1e4b7e2f5435dab0909758a9b43c9"
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
      "id": 194,
      "name": "Secured motivating initiative",
      "name_translations": {
        "en": "Secured motivating initiative"
      },
      "discipline_id": 195
    },
    {
      "id": 195,
      "name": "Fundamental needs-based encoding",
      "name_translations": {
        "en": "Fundamental needs-based encoding"
      },
      "discipline_id": 196
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
GET /v2/topics/196
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
    "id": 196,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 197
  }
}
```



```shell
curl "api.goskive.com/v2/topics/196" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer e86ed16cbdd76fda63c44e5377ef00e0d4331006e2b6ce4c5aba024f91ae0990
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
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-40",
      "html_url": "https://goskive.com/university/uni-40",
      "slug": "uni-40",
      "name": "University 31",
      "short_name": "Uni 40",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/27410d0ec0ebad41a0b92764fee58f02682122eb.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/b6020270ac48e3e0eb7dfc5a4a7346976b139c7e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-07-18T14:37:53.958Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-41",
      "html_url": "https://goskive.com/university/uni-41",
      "slug": "uni-41",
      "name": "University 32",
      "short_name": "Uni 41",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/ddc600c1a41c2c4dc4f7cb06220441f030500df1.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/2aac2a2154dc223f34258f90b071f2ba65516f33.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-07-18T14:37:53.975Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-42",
      "html_url": "https://goskive.com/university/uni-42",
      "slug": "uni-42",
      "name": "University 33",
      "short_name": "Uni 42",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/123583053f30d60d57698c0742b45baeaaeea45e.png",
      "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/467253d3f01c670a10060a75442205258e791570.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-07-18T14:37:53.994Z",
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
	-H "Authorization: Bearer e86ed16cbdd76fda63c44e5377ef00e0d4331006e2b6ce4c5aba024f91ae0990"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1d8efd43780eea57351400d67823146868b9aa4a9f981fae5190670aa39adbab
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
    "id": 59,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/original/8c1892a7833be9197de94e38b43c671374a64b54.png",
    "image_thumb_url": "file:///Users/alexbcoles/git-repos/skive-backend/public/system/universities/thumb/2b75f7c2258319815d34dc05c5b66e628e795a7f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-07-18T14:37:53.891Z",
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
	-H "Authorization: Bearer 1d8efd43780eea57351400d67823146868b9aa4a9f981fae5190670aa39adbab"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4281cff1046410026e6e42ea8028e6797300e0f41d079d7f0fdd4340ea95860a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":47,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 83,
    "id": 47,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 25,
    "additional_university_ids": [

    ],
    "topic_id": 47,
    "discipline_id": 47,
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
    "chapters_updated_at": "2016-07-18T14:37:31.895Z",
    "updated_at": "2016-07-18T14:37:31.908Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 13,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-07-18T14:37:31.843Z",
        "course_id": 47,
        "author_id": 83,
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
        "id": 14,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-07-18T14:37:31.871Z",
        "course_id": 47,
        "author_id": 83,
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
        "id": 15,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-07-18T14:37:31.895Z",
        "course_id": 47,
        "author_id": 83,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":47,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4281cff1046410026e6e42ea8028e6797300e0f41d079d7f0fdd4340ea95860a"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 35453489cf2ddd7943f5cf2612f0113c0cd103ba61eb670e8e631bffff826621
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":48,"published":false}}
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
    "creator_id": 84,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 26,
    "additional_university_ids": [

    ],
    "topic_id": 48,
    "discipline_id": 48,
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
    "updated_at": "2016-07-18T14:37:32.110Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":48,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35453489cf2ddd7943f5cf2612f0113c0cd103ba61eb670e8e631bffff826621"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0bf2c901f58c3f205e36cd6843933d70e150eede503f9ed2c2477fe2fc197132
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
      "creator_id": 58,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 27,
      "discipline_id": 27,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
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
      "updated_at": "2016-07-18T14:37:28.997Z",
      "shortname": "fu-course-27"
    },
    {
      "creator_id": 58,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 28,
      "discipline_id": 28,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
      "chapters_updated_at": "2016-07-18T14:37:29.197Z",
      "updated_at": "2016-07-18T14:37:29.199Z",
      "shortname": "fu-course-28"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bf2c901f58c3f205e36cd6843933d70e150eede503f9ed2c2477fe2fc197132"
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
      "creator_id": 51,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "topic_id": 19,
      "discipline_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
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
      "updated_at": "2016-07-18T14:37:28.289Z",
      "shortname": "fu-course-19"
    },
    {
      "creator_id": 51,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
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
      "chapters_updated_at": "2016-07-18T14:37:28.485Z",
      "updated_at": "2016-07-18T14:37:28.488Z",
      "shortname": "fu-course-20"
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
      "creator_id": 56,
      "id": 23,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 23,
      "discipline_id": 23,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
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
      "updated_at": "2016-07-18T14:37:28.706Z",
      "shortname": "fu-course-23"
    },
    {
      "creator_id": 56,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 24,
      "discipline_id": 24,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
      "updated_at": "2016-07-18T14:37:28.752Z",
      "shortname": "fu-course-24"
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
Authorization: Bearer e2f12090042e4a0616a4cc6c2e5bbfd4b6e38e870605349a1eb40bd5677b18b1
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
      "creator_id": 64,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 31,
      "discipline_id": 31,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 31",
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
      "updated_at": "2016-07-18T14:37:29.480Z",
      "shortname": "fu-course-31"
    },
    {
      "creator_id": 64,
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 32,
      "discipline_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
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
      "updated_at": "2016-07-18T14:37:29.525Z",
      "shortname": "fu-course-32"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2f12090042e4a0616a4cc6c2e5bbfd4b6e38e870605349a1eb40bd5677b18b1"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer e74abea7daa0bf44f206cc0eedf88b69d9347b0a5373c61345861c1eb7e6bedc
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
  "id": 512,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-07-18T14:38:14.074Z",
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
	-H "Authorization: Bearer e74abea7daa0bf44f206cc0eedf88b69d9347b0a5373c61345861c1eb7e6bedc"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/142
Content-Type: application/json
Authorization: Bearer 6f3bd9c5f886de365c3f1921dd573bad0ad86c1579c5cf59981a60a69612f961
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
    "id": 142,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 41,
    "fields_of_study": [
      65,
      66
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-07-18T14:37:48.792Z",
    "updated_at": "2016-07-18T14:37:48.792Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/142" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f3bd9c5f886de365c3f1921dd573bad0ad86c1579c5cf59981a60a69612f961"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/140
Content-Type: application/json
Authorization: Bearer bd3e9aea9857a4243cd72f6c6d68eced40fe63df539b25e84e5f4b9efc2fa2c4
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
    "id": 140,
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
    "created_at": "2016-07-18T14:37:48.583Z",
    "updated_at": "2016-07-18T14:37:48.583Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/140" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd3e9aea9857a4243cd72f6c6d68eced40fe63df539b25e84e5f4b9efc2fa2c4"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer 2979b06886ebaad936a5da16986b51f16bdf6588fbcf2fdff21260f2b743b60c
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2979b06886ebaad936a5da16986b51f16bdf6588fbcf2fdff21260f2b743b60c"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/20
Content-Type: application/json
Authorization: Bearer 6bb81708ba22c82b449e0f3f0126f0d5af020fcba0b7f6ae5e1bc444fe564c93
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
    "id": 20,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 59,
    "user_id": 605
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bb81708ba22c82b449e0f3f0126f0d5af020fcba0b7f6ae5e1bc444fe564c93"
```
