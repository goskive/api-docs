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
Authorization: Basic ZTIxODY5NGY1ZDljOTFjZTRiNmIyNjEzNmQyZTVmNTVlY2Q2MTI3ZjhjZmZj
ZTFlZDJiNmUxMDhmODYzZjhjNTo1MWJmZTE3NDE5NDYzNDM3NjQ2ZGJjMDU0
M2ZhYWM3YzQxNzg5NGEwYjRjMmU1ODAyY2JjNzQwNzUxM2FhMTJl

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
	-u e218694f5d9c91ce4b6b26136d2e5f55ecd6127f8cffce1ed2b6e108f863f8c5:51bfe17419463437646dbc0543faac7c417894a0b4c2e5802cbc7407513aa12e
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5434d9b601e5d306195f14db2623e85c2422d0b2d72acfc5fc9a04f745d41790","client_secret":"91a1c3ca6003c70e1e6ab7d4975515d1bd1396eb4bc49d65922425ebb1aff6bb"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5434d9b601e5d306195f14db2623e85c2422d0b2d72acfc5fc9a04f745d41790","client_secret":"91a1c3ca6003c70e1e6ab7d4975515d1bd1396eb4bc49d65922425ebb1aff6bb"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDNlZGEwM2M0NDMzM2UwYTk4MTVlNzZlMGViNzhjZmE2N2U2ZmZhZGJkYzIw
MjJlMjdlNjZjNmExNzQwNWZmZjo5MTBjNThlYzllNGZjNWE3ZjYwNDU5NmYw
ZjQyYzhkZjUzODQyNTVjZTRlMzVmZGJiNTc2NTIzOGFmNjc5M2Nh

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
  "access_token": "7f06f01df0e4e4392abbd266ed727975b11358700fd71a2f4511cb48a4669442",
  "token_type": "bearer",
  "created_at": 1477761784
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u d3eda03c44333e0a9815e76e0eb78cfa67e6ffadbdc2022e27e66c6a17405fff:910c58ec9e4fc5a7f604596f0f42c8df5384255ce4e35fdbb5765238af6793ca
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ab2306f7658b8c18753f72bb5b33ec0fe34357ee11cfdc89116bdaa13b12fec6","client_secret":"d64332c606a81707bcdd390a75d3dcf4a2fd223fb727a9f386176bdb858478d3"}
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
  "access_token": "d686a5cbe01ff0595c4d5cc6e36653db922df2eeeb64cc9178cb837bb479e80b",
  "token_type": "bearer",
  "created_at": 1477761784
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ab2306f7658b8c18753f72bb5b33ec0fe34357ee11cfdc89116bdaa13b12fec6","client_secret":"d64332c606a81707bcdd390a75d3dcf4a2fd223fb727a9f386176bdb858478d3"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"4364add8ffc23d4e539e87a08eeead599c5e9f80efb44c4b740da32e9ddbc91c","client_secret":"64dbba7735f60ec9c86c98ceb17c71f70905b317cb8a32632af73f4ac6fc927c"}
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
  "access_token": "4a00a9318e2dcb09dfc7f979faef7a2e47bf22053147214d673c7ebffc15aa0a",
  "token_type": "bearer",
  "created_at": 1477761784
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"4364add8ffc23d4e539e87a08eeead599c5e9f80efb44c4b740da32e9ddbc91c","client_secret":"64dbba7735f60ec9c86c98ceb17c71f70905b317cb8a32632af73f4ac6fc927c"}' -X POST \
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
GET /v2/campaigns/12
Content-Type: application/json
Authorization: Bearer bfc20b369b68d99b37848707b807d5fd4ac4d207f69407d03b2af69b9b3d418e
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
    "id": 12,
    "title": "Recruiting pastry chefs",
    "company_id": 28,
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
curl "api.goskive.com/v2/campaigns/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfc20b369b68d99b37848707b807d5fd4ac4d207f69407d03b2af69b9b3d418e"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/164/flashcards
Content-Type: application/json
Authorization: Bearer ab00a6fe40ce71a4aa515ff00bf4ff638d49584af361c3a5ee8b96677a4f07a6
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":164,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
```


| Name | Description |
|:-----|:------------|
| flashcard[front_content_html] *required* | Front Content HTML |
| flashcard[back_content_html] *required* | Back Content HTML |
| flashcard[front_content]  | Front Content Markdown |
| flashcard[back_content]  | Back Content Markdown |
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
    "id": 85,
    "obfuscated_id": "xR5KgQjIo2Y",
    "author_id": 870,
    "chapter_id": 164,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:23:03.428Z",
    "created_at": "2016-10-29T17:23:03.428Z",
    "tags": [

    ],
    "status": "draft",
    "published": false,
    "language_code": "fr",
    "front_content": null,
    "back_content": null,
    "front_content_html": "Function of <strong>eggs</strong> in choux pastry",
    "back_content_html": "Helps things <strong>raise</strong>"
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/164/flashcards" -d '{"flashcard":{"chapter_id":164,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab00a6fe40ce71a4aa515ff00bf4ff638d49584af361c3a5ee8b96677a4f07a6"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/165/flashcards
Content-Type: application/json
Authorization: Bearer c11099eccbada398b9c4b65981228fd776fe6ffab613120d9bc58665e9b31561
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
      "id": 86,
      "obfuscated_id": "7q-2LHZR3Kk",
      "author_id": 871,
      "chapter_id": 165,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:23:03.564Z",
      "created_at": "2016-10-29T17:23:03.564Z",
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
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 871,
      "chapter_id": 165,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:23:03.598Z",
      "created_at": "2016-10-29T17:23:03.598Z",
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 871,
      "chapter_id": 165,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:23:03.632Z",
      "created_at": "2016-10-29T17:23:03.632Z",
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
curl "api.goskive.com/v2/chapters/165/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c11099eccbada398b9c4b65981228fd776fe6ffab613120d9bc58665e9b31561"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/130/questions
Content-Type: application/json
Authorization: Bearer 24b6fa8a904cf798c34206139215f6a0293b06945aa269363a3bbbae21311c54
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":130,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 91,
    "obfuscated_id": "EqPpyB0JN58",
    "author_id": 692,
    "chapter_id": 130,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:48.372Z",
    "created_at": "2016-10-29T17:22:48.372Z",
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
        "id": 183,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 184,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 185,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 186,
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
curl "api.goskive.com/v2/chapters/130/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":130,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24b6fa8a904cf798c34206139215f6a0293b06945aa269363a3bbbae21311c54"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/129/questions
Content-Type: application/json
Authorization: Bearer a1bb1937fc97f614bbfe316c1cf3d4865614a31375241ddac7ae2137876f5c4d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":129,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 90,
    "obfuscated_id": "gX_ALSaJ0k4",
    "author_id": 689,
    "chapter_id": 129,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:48.052Z",
    "created_at": "2016-10-29T17:22:48.052Z",
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
        "id": 181,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 182,
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
curl "api.goskive.com/v2/chapters/129/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":129,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1bb1937fc97f614bbfe316c1cf3d4865614a31375241ddac7ae2137876f5c4d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/131/questions
Content-Type: application/json
Authorization: Bearer 1b8cc23ecdb8b4c257c8331f7921cff2d9150ab3f8e3dba0b7499b12ca95f854
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 92,
    "obfuscated_id": "__OphzZQiQY",
    "author_id": 695,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:48.846Z",
    "created_at": "2016-10-29T17:22:48.846Z",
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
        "id": 187,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 188,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/131/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b8cc23ecdb8b4c257c8331f7921cff2d9150ab3f8e3dba0b7499b12ca95f854"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/128/questions
Content-Type: application/json
Authorization: Bearer 03ef825450ecfdca1d30e55585d8c3052ea1ca5744ccdf6f428c4e4988bdcf22
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
    "id": 89,
    "obfuscated_id": "5eRHrGHLqZk",
    "author_id": 686,
    "chapter_id": 128,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:47.629Z",
    "created_at": "2016-10-29T17:22:47.629Z",
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
        "id": 178,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 179,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 180,
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
	-H "Authorization: Bearer 03ef825450ecfdca1d30e55585d8c3052ea1ca5744ccdf6f428c4e4988bdcf22"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/132/questions
Content-Type: application/json
Authorization: Bearer 11551d0e4beb6b7ee9090d8bcc655836e6e3fefe71406050c1a02905dd236c86
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
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 698,
      "chapter_id": 132,
      "position": 80,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:49.255Z",
      "created_at": "2016-10-29T17:22:49.142Z",
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
          "id": 189,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 190,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 699,
      "chapter_id": 132,
      "position": 81,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:49.438Z",
      "created_at": "2016-10-29T17:22:49.324Z",
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
          "id": 191,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 192,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 95,
      "obfuscated_id": "uTOhBSQK4CI",
      "author_id": 700,
      "chapter_id": 132,
      "position": 82,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-29T17:22:49.629Z",
      "created_at": "2016-10-29T17:22:49.510Z",
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
          "id": 193,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 194,
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
curl "api.goskive.com/v2/chapters/132/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11551d0e4beb6b7ee9090d8bcc655836e6e3fefe71406050c1a02905dd236c86"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/71
Content-Type: application/json
Authorization: Bearer 567a9794e3440ca033699df94f8441ca0140506800ed350fa927361143c961a7
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
curl "api.goskive.com/v2/chapters/71" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 567a9794e3440ca033699df94f8441ca0140506800ed350fa927361143c961a7"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/73
Content-Type: application/json
Authorization: Bearer 3f89e459f299efa6ea8ccdf14bfe3ed920ec2e3c9c025f8b5ba71dabba12b3b9
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
curl "api.goskive.com/v2/chapters/73" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f89e459f299efa6ea8ccdf14bfe3ed920ec2e3c9c025f8b5ba71dabba12b3b9"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/67
Content-Type: application/json
Authorization: Bearer 040d6a53529df8ba7c16559936d3ae2eeebb021f6e351fd0cab54d6ef8d4f0c4
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
curl "api.goskive.com/v2/chapters/67" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 040d6a53529df8ba7c16559936d3ae2eeebb021f6e351fd0cab54d6ef8d4f0c4"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/70
Content-Type: application/json
Authorization: Bearer d234edadf1bff85818fa6d334187f00c91be31b9e1ac777c7607957f2cc019d4
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/70" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d234edadf1bff85818fa6d334187f00c91be31b9e1ac777c7607957f2cc019d4"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/69
Content-Type: application/json
Authorization: Bearer 53d69d29cd28ef07b848a3922782b9d275570be2dc3952d69f1b766d58ea3767
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
    "id": 69,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-29T17:22:15.329Z",
    "course_id": 87,
    "author_id": 323,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-29T17:22:14.759Z",
    "questions_updated_at": "2016-10-29T17:22:14.759Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 327,
        "chapter_id": 69,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:15.309Z",
        "created_at": "2016-10-29T17:22:15.309Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 325,
        "chapter_id": 69,
        "position": 26,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:15.195Z",
        "created_at": "2016-10-29T17:22:15.063Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/69" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53d69d29cd28ef07b848a3922782b9d275570be2dc3952d69f1b766d58ea3767"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/65
Content-Type: application/json
Authorization: Bearer 4308c28dd9cfd72cf84b9628ff83af99bbb5316f2c3bcf78a824883d1441148f
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
    "id": 65,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-29T17:22:13.817Z",
    "course_id": 83,
    "author_id": 308,
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
curl "api.goskive.com/v2/chapters/65" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4308c28dd9cfd72cf84b9628ff83af99bbb5316f2c3bcf78a824883d1441148f"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 7e1a20153dff3077f92e83eb2c144dfea5ef9a26ec37e2bfaa43a530c78ecc75
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
    "id": 2,
    "author_id": 137,
    "reply_to_id": 1,
    "created_at": "2016-10-29T17:22:03.607Z",
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
curl "api.goskive.com/v2/comments/1/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e1a20153dff3077f92e83eb2c144dfea5ef9a26ec37e2bfaa43a530c78ecc75"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 19b8283486e5c72873656648cc92403fe2e6c6a950cfe7a3346c527f771a0146
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
curl "api.goskive.com/v2/comments/3/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19b8283486e5c72873656648cc92403fe2e6c6a950cfe7a3346c527f771a0146"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 8d7663bfc4a34f0a0f7e99388eadc9022bd2d4514ac0df3d077d34518a4270af
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
curl "api.goskive.com/v2/comments/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d7663bfc4a34f0a0f7e99388eadc9022bd2d4514ac0df3d077d34518a4270af"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/10/republish
Content-Type: application/json
Authorization: Bearer 87bf1e59e670dbbaa8c00a0a8e618de8a0e38eace02a62b3e9e78f4c1321441b
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
curl "api.goskive.com/v2/comments/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87bf1e59e670dbbaa8c00a0a8e618de8a0e38eace02a62b3e9e78f4c1321441b"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/9
Content-Type: application/json
Authorization: Bearer 5bdf9d7d18ad3b4e87c34e0adeb12f9fe01aaa0483096d2f580b10a76fe411a3
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bdf9d7d18ad3b4e87c34e0adeb12f9fe01aaa0483096d2f580b10a76fe411a3"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/47/report
Content-Type: application/json
Authorization: Bearer 918cf590d34481673a7e28ce5950b4e6ecf370f6f6db9dfe7784409d4a1e6bed
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/47/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 918cf590d34481673a7e28ce5950b4e6ecf370f6f6db9dfe7784409d4a1e6bed"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/24
Content-Type: application/json
Authorization: Bearer d3f2fa987ff7068a4bd4987ef1d14cd7d83c45d52ace70760054ad74b977dbb6
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
    "id": 24,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-29T17:22:52.257Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3f2fa987ff7068a4bd4987ef1d14cd7d83c45d52ace70760054ad74b977dbb6"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer c882e118e5923e2d3369fddca31c91629759cb3271e9693937f6a67fbf29f5a5
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
      "id": 25,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-29T17:22:52.330Z"
    },
    {
      "id": 26,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-29T17:22:52.334Z"
    },
    {
      "id": 27,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-29T17:22:52.337Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c882e118e5923e2d3369fddca31c91629759cb3271e9693937f6a67fbf29f5a5"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/31/company_profiles
Content-Type: application/json
Authorization: Bearer 5f4bbc4ebcd310f5a27b4f6d951e4657b14274307fdd3062d8547d4126147aa3
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
      "id": 12,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/cb7b53bc0db79f6fdb32fcfb3676296e2cab7797.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/bb9fd408e2885991a5d2cf387f2db8486bd6688a.png",
      "widgets": [

      ]
    },
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
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/31/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f4bbc4ebcd310f5a27b4f6d951e4657b14274307fdd3062d8547d4126147aa3"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 3192f0cff9a1a2f2acb3b707172cd07a91bd7e679c692eb6a8133c66811c6930
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
      "id": 8,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/4e8ccb4fdbb03332710724b7199bfb925ebb8588.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/1751c1fcb04de04c20e97d74547e239755abd978.png",
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
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3192f0cff9a1a2f2acb3b707172cd07a91bd7e679c692eb6a8133c66811c6930"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 849a72c5242ab2063969369aeba8722dc2a5c5819ebbb545cf27bbf332710979
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
	-H "Authorization: Bearer 849a72c5242ab2063969369aeba8722dc2a5c5819ebbb545cf27bbf332710979"
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
Authorization: Bearer 737ef3948331d25fa2f7a287b24734b28863da5f6e7756c0118a0f76d0faebc0
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
	-H "Authorization: Bearer 737ef3948331d25fa2f7a287b24734b28863da5f6e7756c0118a0f76d0faebc0"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 68d1d9cc9806b110d3920ffa7dd9c300928d088a1db181a130fd7f80f4744c69
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
    "id": 168,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-29T17:23:06.790Z",
    "course_id": 292,
    "author_id": 902,
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
	-H "Authorization: Bearer 68d1d9cc9806b110d3920ffa7dd9c300928d088a1db181a130fd7f80f4744c69"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f0282340a1805eb6d4f8e47b9bd29fc970efc64383497178a71a23e5f98dc0b1
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
      "id": 173,
      "title": "Clever Chapter Title 149",
      "position": 1,
      "updated_at": "2016-10-29T17:23:07.313Z",
      "course_id": 296,
      "author_id": 913,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 174,
      "title": "Clever Chapter Title 150",
      "position": 2,
      "updated_at": "2016-10-29T17:23:07.336Z",
      "course_id": 296,
      "author_id": 914,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 175,
      "title": "Clever Chapter Title 151",
      "position": 3,
      "updated_at": "2016-10-29T17:23:07.574Z",
      "course_id": 296,
      "author_id": 915,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-29T17:23:07.243Z",
      "questions_updated_at": "2016-10-29T17:23:07.243Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0282340a1805eb6d4f8e47b9bd29fc970efc64383497178a71a23e5f98dc0b1"
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
      "id": 179,
      "title": "Clever Chapter Title 155",
      "position": 1,
      "updated_at": "2016-10-29T17:23:08.011Z",
      "course_id": 299,
      "author_id": 927,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 180,
      "title": "Clever Chapter Title 156",
      "position": 2,
      "updated_at": "2016-10-29T17:23:08.034Z",
      "course_id": 299,
      "author_id": 928,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 181,
      "title": "Clever Chapter Title 157",
      "position": 3,
      "updated_at": "2016-10-29T17:23:08.280Z",
      "course_id": 299,
      "author_id": 929,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-29T17:23:07.938Z",
      "questions_updated_at": "2016-10-29T17:23:07.938Z",
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
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6feb5d3d8da2625f98d922949649ec0271252e9038fb1056f113fbfb3bcfeae7
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
      "id": 176,
      "title": "Clever Chapter Title 152",
      "position": 1,
      "updated_at": "2016-10-29T17:23:07.721Z",
      "course_id": 297,
      "author_id": 920,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 177,
      "title": "Clever Chapter Title 153",
      "position": 2,
      "updated_at": "2016-10-29T17:23:07.744Z",
      "course_id": 297,
      "author_id": 921,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 178,
      "title": "Clever Chapter Title 154",
      "position": 3,
      "updated_at": "2016-10-29T17:23:07.768Z",
      "course_id": 297,
      "author_id": 922,
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
	-H "Authorization: Bearer 6feb5d3d8da2625f98d922949649ec0271252e9038fb1056f113fbfb3bcfeae7"
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
      "id": 182,
      "title": "Clever Chapter Title 158",
      "position": 1,
      "updated_at": "2016-10-29T17:23:08.393Z",
      "course_id": 300,
      "author_id": 933,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 183,
      "title": "Clever Chapter Title 159",
      "position": 2,
      "updated_at": "2016-10-29T17:23:08.416Z",
      "course_id": 300,
      "author_id": 934,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 184,
      "title": "Clever Chapter Title 160",
      "position": 3,
      "updated_at": "2016-10-29T17:23:08.438Z",
      "course_id": 300,
      "author_id": 935,
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
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c262651e326fbe43c20547083996f7bb25107276908e82521864c4fc56b6aa4f
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
    "id": 5,
    "course_id": 41,
    "user_id": 121,
    "updated_at": "2016-10-29T17:22:02.054Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c262651e326fbe43c20547083996f7bb25107276908e82521864c4fc56b6aa4f"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 836d7401477b3feefa4e76c755a51f0a509cc07792af1baf9d8e7bc3c3abb1dc
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
      "id": 3,
      "course_id": 39,
      "user_id": 115,
      "updated_at": "2016-10-29T17:22:01.767Z"
    },
    {
      "id": 4,
      "course_id": 39,
      "user_id": 116,
      "updated_at": "2016-10-29T17:22:01.780Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 836d7401477b3feefa4e76c755a51f0a509cc07792af1baf9d8e7bc3c3abb1dc"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/32/files
Content-Type: application/json
Authorization: Bearer b7330805d5d16a6758adf8edd11d4eb0e09b2f0e43622980c5aae886f20c294d
```

`GET /v2/courses/:course_id/files`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "files": [
    {
      "id": 4,
      "uploader": {
        "id": 95,
        "first_name": "Kasper",
        "last_name": "Skive",
        "nickname": "Kasper Skive",
        "type": "Student",
        "avatar_thumb_url": null,
        "university_id": null,
        "fields_of_study": [

        ],
        "study_level": null,
        "graduation_year": null,
        "created_at": "2016-10-29T17:22:00.672Z",
        "updated_at": "2016-10-29T17:22:00.672Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-29T17:22:00.736Z",
      "updated_at": "2016-10-29T17:22:00.736Z",
      "course_id": 32,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 96,
        "first_name": "Kasper",
        "last_name": "Skive",
        "nickname": "Kasper Skive",
        "type": "Student",
        "avatar_thumb_url": null,
        "university_id": null,
        "fields_of_study": [

        ],
        "study_level": null,
        "graduation_year": null,
        "created_at": "2016-10-29T17:22:00.744Z",
        "updated_at": "2016-10-29T17:22:00.744Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-29T17:22:00.754Z",
      "updated_at": "2016-10-29T17:22:00.754Z",
      "course_id": 32,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 97,
        "first_name": "Kasper",
        "last_name": "Skive",
        "nickname": "Kasper Skive",
        "type": "Student",
        "avatar_thumb_url": null,
        "university_id": null,
        "fields_of_study": [

        ],
        "study_level": null,
        "graduation_year": null,
        "created_at": "2016-10-29T17:22:00.761Z",
        "updated_at": "2016-10-29T17:22:00.761Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-29T17:22:00.769Z",
      "updated_at": "2016-10-29T17:22:00.769Z",
      "course_id": 32,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/32/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7330805d5d16a6758adf8edd11d4eb0e09b2f0e43622980c5aae886f20c294d"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/35/files
Content-Type: application/json
Authorization: Bearer 84a44e943836c010d6d6f3bd2f33b79f051a363ed3ad26fb8112d55e6dd4f750
```

`POST /v2/courses/:course_id/files`

#### Parameters


```json
{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}
```


| Name | Description |
|:-----|:------------|
| file[category] *required* | Category: summary|assignment|exam|lecture_note|other |
| file[filename] *required* | Filename |
| file[file_url] *required* | URL to the file in cache on S3 |
| file[description]  | Description |
| file[is_anonymous]  | Uploader is anonymous (default: false) |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "file": {
    "id": 7,
    "uploader": {
      "id": 104,
      "first_name": "Kasper",
      "last_name": "Skive",
      "nickname": "Kasper Skive",
      "type": "Student",
      "avatar_thumb_url": null,
      "university_id": null,
      "fields_of_study": [

      ],
      "study_level": null,
      "graduation_year": null,
      "created_at": "2016-10-29T17:22:01.102Z",
      "updated_at": "2016-10-29T17:22:01.102Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [
      "update",
      "delete"
    ],
    "up_votes_count": 0,
    "created_at": "2016-10-29T17:22:01.133Z",
    "updated_at": "2016-10-29T17:22:01.133Z",
    "course_id": 35,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/35/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84a44e943836c010d6d6f3bd2f33b79f051a363ed3ad26fb8112d55e6dd4f750"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/34/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 707910d1be908effde5a0d8b2eda8c743dea52703831cb549c513da3cc328622
```

`GET /v2/courses/:course_id/file_upload/cache/presign`

#### Parameters


```json
extension: .jpg
```


| Name | Description |
|:-----|:------------|
| extension  | File extension |



### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com",
  "fields": {
    "key": "cache/a22dd2e77a35cf9179890027278c5ccc.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yOVQxODoyMjowMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2EyMmRkMmU3N2EzNWNmOTE3OTg5MDAyNzI3OGM1Y2NjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjkvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI5VDE3MjIwMVoifV19",
    "x-amz-credential": "FAKE/20161029/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161029T172201Z",
    "x-amz-signature": "eed32ef458dc0905b5298e08b3f100f6f448f5255bfd7cf1cc52677ec3966b75"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/34/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 707910d1be908effde5a0d8b2eda8c743dea52703831cb549c513da3cc328622"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer fa959dc58f17e805f34f951247cd8b525bf7cca4a3146295273f339f115be67b
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
	-H "Authorization: Bearer fa959dc58f17e805f34f951247cd8b525bf7cca4a3146295273f339f115be67b"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 77b7f40e410a222259de16abc5e295c696590792de34b09985b3db92d73f2f66
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
	-H "Authorization: Bearer 77b7f40e410a222259de16abc5e295c696590792de34b09985b3db92d73f2f66"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 02190d9d88d8d801960809948a39071ce3e7c5d13a0b1e073b6be852ffdc4dab
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
	-H "Authorization: Bearer 02190d9d88d8d801960809948a39071ce3e7c5d13a0b1e073b6be852ffdc4dab"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b7eb70473325acf9877bcfa8bc55d8895d0b15183d4345524647b0001d88a03f
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
	-H "Authorization: Bearer b7eb70473325acf9877bcfa8bc55d8895d0b15183d4345524647b0001d88a03f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c9aa2dba2dcd447e15eb2857efd12e55b532be56f140e723c2da3232a50620df
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
	-H "Authorization: Bearer c9aa2dba2dcd447e15eb2857efd12e55b532be56f140e723c2da3232a50620df"
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
    "creator_id": 501,
    "id": 179,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 157,
    "additional_university_ids": [

    ],
    "topic_id": 189,
    "discipline_id": 190,
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
    "chapters_updated_at": "2016-10-29T17:22:27.080Z",
    "updated_at": "2016-10-29T17:22:28.745Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 86,
        "title": "Clever Chapter Title 74",
        "position": 1,
        "updated_at": "2016-10-29T17:22:28.692Z",
        "course_id": 179,
        "author_id": 501,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-29T17:22:27.080Z",
        "questions_updated_at": "2016-10-29T17:22:27.080Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 87,
        "title": "Clever Chapter Title 75",
        "position": 2,
        "updated_at": "2016-10-29T17:22:28.735Z",
        "course_id": 179,
        "author_id": 501,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-29T17:22:27.080Z",
        "questions_updated_at": "2016-10-29T17:22:27.080Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 501,
        "chapter_id": 86,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:27.309Z",
        "created_at": "2016-10-29T17:22:27.172Z",
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
            "id": 75,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 76,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 501,
        "chapter_id": 87,
        "position": 40,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:27.747Z",
        "created_at": "2016-10-29T17:22:27.604Z",
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
            "id": 79,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 80,
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
Authorization: Bearer 5c0ea41b7e2e0d20c3da766a83241dd2c4ff03471e0180a5f4d9b80d4cd69069
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
    "creator_id": 506,
    "id": 180,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 158,
    "additional_university_ids": [

    ],
    "topic_id": 190,
    "discipline_id": 191,
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
    "chapters_updated_at": "2016-10-29T17:22:28.804Z",
    "updated_at": "2016-10-29T17:22:30.484Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 88,
        "title": "Clever Chapter Title 76",
        "position": 1,
        "updated_at": "2016-10-29T17:22:30.431Z",
        "course_id": 180,
        "author_id": 506,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-29T17:22:28.804Z",
        "questions_updated_at": "2016-10-29T17:22:28.804Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 89,
        "title": "Clever Chapter Title 77",
        "position": 2,
        "updated_at": "2016-10-29T17:22:30.475Z",
        "course_id": 180,
        "author_id": 506,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-29T17:22:28.804Z",
        "questions_updated_at": "2016-10-29T17:22:28.804Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 507,
        "chapter_id": 88,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:30.253Z",
        "created_at": "2016-10-29T17:22:30.253Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 507,
        "chapter_id": 89,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:30.332Z",
        "created_at": "2016-10-29T17:22:30.332Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 507,
        "chapter_id": 88,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:30.298Z",
        "created_at": "2016-10-29T17:22:30.298Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 507,
        "chapter_id": 89,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:30.376Z",
        "created_at": "2016-10-29T17:22:30.376Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 507,
        "chapter_id": 88,
        "position": 44,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:29.045Z",
        "created_at": "2016-10-29T17:22:28.903Z",
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
          }
        ]
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 507,
        "chapter_id": 88,
        "position": 45,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:29.253Z",
        "created_at": "2016-10-29T17:22:29.119Z",
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
            "id": 89,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 90,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 507,
        "chapter_id": 89,
        "position": 46,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:29.493Z",
        "created_at": "2016-10-29T17:22:29.346Z",
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
            "id": 91,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 92,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 507,
        "chapter_id": 89,
        "position": 47,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-29T17:22:29.708Z",
        "created_at": "2016-10-29T17:22:29.569Z",
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
            "id": 93,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 94,
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
	-H "Authorization: Bearer 5c0ea41b7e2e0d20c3da766a83241dd2c4ff03471e0180a5f4d9b80d4cd69069"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/196/pin
Content-Type: application/json
Authorization: Bearer f862f568244209b7c6454e802e604b87258b4dd6ba3fca4425e1721949590cee
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/196/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f862f568244209b7c6454e802e604b87258b4dd6ba3fca4425e1721949590cee"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/178/pin
Content-Type: application/json
Authorization: Bearer f06f66c8c5268cae9f578160dca7245490a5a4d5b0042bf9bee2b0acd05f5422
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/178/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f06f66c8c5268cae9f578160dca7245490a5a4d5b0042bf9bee2b0acd05f5422"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0e840b503892fc5806d828e4b9db6ed4f40c9981ed558d1c7e562fad94d1b67d
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
    "creator_id": 524,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 161,
    "additional_university_ids": [

    ],
    "topic_id": 193,
    "discipline_id": 194,
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
    "updated_at": "2016-10-29T17:22:34.339Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e840b503892fc5806d828e4b9db6ed4f40c9981ed558d1c7e562fad94d1b67d"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer d3eb6cbe107c2952e78bddc1524e4dc452cbc68e7d72ef6de54d78321299221f
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
    "id": 129,
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
    "created_at": "2016-10-29T17:22:02.744Z",
    "updated_at": "2016-10-29T17:22:02.744Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ],
    "created_content_units": 0
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3eb6cbe107c2952e78bddc1524e4dc452cbc68e7d72ef6de54d78321299221f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer fb0ddf0de4367f89e958d1f16cfe4c1ba140620fa8927cc0bb329e7c1190150e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[45]}
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
    "id": 124,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      45
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-29T17:22:02.211Z",
    "updated_at": "2016-10-29T17:22:02.262Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ],
    "created_content_units": 0
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[45]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb0ddf0de4367f89e958d1f16cfe4c1ba140620fa8927cc0bb329e7c1190150e"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f0654dc18dddd9b656aed4024590ab1d0fc616f292101cd3cecab96542dca073
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
    "id": 126,
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
    "created_at": "2016-10-29T17:22:02.365Z",
    "updated_at": "2016-10-29T17:22:02.365Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ],
    "created_content_units": 0
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0654dc18dddd9b656aed4024590ab1d0fc616f292101cd3cecab96542dca073"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 112f9563274dd798a4137ae36007c21d98400a5ab5dfdff2b05dabe79b93de6a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[48]}
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
    "id": 127,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      48
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-29T17:22:02.455Z",
    "updated_at": "2016-10-29T17:22:02.455Z",
    "email": "magnus@hotmail.sk",
    "locale": "sk",
    "avatar_url": null,
    "course_ids": [

    ],
    "created_content_units": 0
  }
}
```



```shell
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[48]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 112f9563274dd798a4137ae36007c21d98400a5ab5dfdff2b05dabe79b93de6a"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer fba270e5d380b8f0b31b63e72bf99e4ad4b39d330479bedc7cf299ec7150adb4
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

49
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
    "id": 128,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/cd515e79471e9790d738d8745961e6f3e3945090.jpg",
    "university_id": null,
    "fields_of_study": [
      49
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-29T17:22:02.522Z",
    "updated_at": "2016-10-29T17:22:02.717Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/be8f7680211b946feb97fb5b2b7da38ddf4cca9e.jpg",
    "course_ids": [

    ],
    "created_content_units": 0
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

49
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer fba270e5d380b8f0b31b63e72bf99e4ad4b39d330479bedc7cf299ec7150adb4"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer b9d6f257429dcd311ea08867dfefa4be374f1bff1ddccdad6d7f1384853da1d8
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
      "id": 7,
      "bookmarkable_id": 96,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 97,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 98,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9d6f257429dcd311ea08867dfefa4be374f1bff1ddccdad6d7f1384853da1d8"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 767a7268bfb4c9911a108f174fd819ad12a612a0f17e0f62b232955c4aa2f2cc
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
      "title": "Campaign 10",
      "company_id": 17,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 6,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/e454a32c998f7d7ac27f091147bbb511cdb6f8e8.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/0d72c01d65a8bf6733c1fdf8c672243b6d546a9e.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "id": 6,
          "image_url_absolute": "banners/8aa5bf11cc13a7de5c7089d33a8ff916dd8f8472.png",
          "target_url": "http://goskive.com",
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 11,
      "title": "Campaign 11",
      "company_id": 18,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 7,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9d765d9b895a77cd295c7f5e57af933f977bb87f.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/648481f5d8c76852bca2fea2b305e3b694878255.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "id": 7,
          "image_url_absolute": "banners/50ffd61ac4f42ad5c682c107e23dbf7769b7381c.png",
          "target_url": "http://goskive.com",
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
	-H "Authorization: Bearer 767a7268bfb4c9911a108f174fd819ad12a612a0f17e0f62b232955c4aa2f2cc"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 3caa2d77ba1a4836fd15246a4194eeba63b4c649606d1926a9377f86088a639e
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
      "id": 9,
      "title": "Campaign 9",
      "company_id": 13,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 5,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/43cd8331a2a1101475dca8b52baf14565bda8d25.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/36ab23184d8eb9448413fbe09f112b2034c6db2d.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "id": 5,
          "image_url_absolute": "banners/498551b0a405b9134839281bc158747e85383832.png",
          "target_url": "http://goskive.com",
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
	-H "Authorization: Bearer 3caa2d77ba1a4836fd15246a4194eeba63b4c649606d1926a9377f86088a639e"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer be692652f0b23851a383d15cea873dc168d625921cc1709b9997db77ab44d273
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
      "creator_id": 706,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-201",
      "html_url": "https://goskive.com/course/mit-course-201",
      "slug": "mit-course-201",
      "university_id": 223,
      "additional_university_ids": [

      ],
      "topic_id": 255,
      "discipline_id": 256,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 201",
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
      "updated_at": "2016-10-29T17:22:49.948Z",
      "shortname": "mit-course-201"
    },
    {
      "creator_id": 707,
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-202",
      "html_url": "https://goskive.com/course/mit-course-202",
      "slug": "mit-course-202",
      "university_id": 224,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 202",
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
      "updated_at": "2016-10-29T17:22:50.027Z",
      "shortname": "mit-course-202"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be692652f0b23851a383d15cea873dc168d625921cc1709b9997db77ab44d273"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer b78067fe5fce7a96bce32dba09ee343d268bdeb0e73ab0cbdd2b6ac587d0a18f
```

`GET /v2/me/files`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "user_files": {
    "uploaded_files": [
      {
        "id": 1,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-10-29T17:21:59.249Z",
        "updated_at": "2016-10-29T17:21:59.249Z",
        "file_url": "memory://8c9e6e32c260a4e05a77c9ecfa2d9ad0.pdf",
        "course_id": 25,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 2,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-10-29T17:21:59.319Z",
        "updated_at": "2016-10-29T17:21:59.319Z",
        "file_url": "memory://c0ad1e78cb5230baf2678eac8d105f10.pdf",
        "course_id": 26,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 3,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-10-29T17:21:59.393Z",
        "updated_at": "2016-10-29T17:21:59.393Z",
        "file_url": "memory://732f35d3b54eb44b039117e1c10a982e.pdf",
        "course_id": 27,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/me/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b78067fe5fce7a96bce32dba09ee343d268bdeb0e73ab0cbdd2b6ac587d0a18f"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e67125cca88ec5b55e61290425f31644b4166d34a5aa96d2fcb401357b74a1c0
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
      "id": 7,
      "title": "Job Posting7",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 37,
      "company": {
        "id": 37,
        "name": "Fake Company Name 32",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-29T17:23:06.368Z"
      },
      "created_at": "2016-10-29T17:23:06.372Z",
      "updated_at": "2016-10-29T17:23:06.372Z",
      "score": 0.0
    },
    {
      "id": 8,
      "title": "Job Posting8",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 38,
      "company": {
        "id": 38,
        "name": "Fake Company Name 33",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-29T17:23:06.379Z"
      },
      "created_at": "2016-10-29T17:23:06.383Z",
      "updated_at": "2016-10-29T17:23:06.383Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e67125cca88ec5b55e61290425f31644b4166d34a5aa96d2fcb401357b74a1c0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 02ab06a8759fe3744a7314b3dfee1ad66ed273daf823deb16d244793211fa209
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
      "company_id": 33,
      "company": {
        "id": 33,
        "name": "Fake Company Name 28",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-29T17:23:06.168Z"
      },
      "created_at": "2016-10-29T17:23:06.172Z",
      "updated_at": "2016-10-29T17:23:06.172Z",
      "score": 0.0
    },
    {
      "id": 5,
      "title": "Job Posting5",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 34,
      "company": {
        "id": 34,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-29T17:23:06.184Z"
      },
      "created_at": "2016-10-29T17:23:06.188Z",
      "updated_at": "2016-10-29T17:23:06.188Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02ab06a8759fe3744a7314b3dfee1ad66ed273daf823deb16d244793211fa209"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 2abef82ba6d625471e833313e62904b77113b246e13d81af911363792577ccdc
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
      "id": 16,
      "created_at": "2016-10-29T17:22:54.225Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-10-29T17:22:54.333Z",
      "author_id": "759",
      "thread_subject_id": "261",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-10-29T17:22:54.321Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-10-29T17:22:54.336Z",
      "author_id": "762",
      "thread_subject_id": "262",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-29T17:22:54.720Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-10-29T17:22:54.720Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-10-29T17:22:55.078Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-10-29T17:22:55.078Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-10-29T17:22:55.489Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-29T17:22:55.489Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-10-29T17:22:55.783Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 106,
      "updated_at": "2016-10-29T17:22:55.783Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-29T17:22:56.075Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 107,
      "updated_at": "2016-10-29T17:22:56.075Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-10-29T17:22:56.371Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 108,
      "updated_at": "2016-10-29T17:22:56.371Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2abef82ba6d625471e833313e62904b77113b246e13d81af911363792577ccdc"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/15
Content-Type: application/json
Authorization: Bearer 4d3608efc8266e58a4a3bfbadff147867823e1b388c806a1bd43c4c81f0f7394
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-29T17:12:53.000Z"}}
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
    "id": 15,
    "created_at": "2016-10-29T17:22:54.023Z",
    "read_at": "2016-10-29T17:12:53.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 56,
    "updated_at": "2016-10-29T17:22:54.079Z",
    "author_id": "754",
    "thread_subject_id": "260",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/15" -d '{"notification":{"read_at":"2016-10-29T17:12:53.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d3608efc8266e58a4a3bfbadff147867823e1b388c806a1bd43c4c81f0f7394"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 0bf9b7503edfeda1fdcc9fed1004c8a318798c870362d26e345207ca3cb59419
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
      "id": 7,
      "course_id": 251,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-29T17:22:50.729Z",
      "course_published": true,
      "updated_at": "2016-10-29T17:22:50.722Z"
    },
    {
      "id": 8,
      "course_id": 252,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-29T17:22:50.804Z",
      "course_published": true,
      "updated_at": "2016-10-29T17:22:50.798Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bf9b7503edfeda1fdcc9fed1004c8a318798c870362d26e345207ca3cb59419"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer e9ade7aa3fb98a386fabd778d09f5c745e0ec1dcc3b3cbbe7f4ffd44693298a6
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
    "id": 4,
    "course_id": 247,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-29T17:22:50.209Z",
    "course_published": true,
    "updated_at": "2016-10-29T17:22:50.202Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9ade7aa3fb98a386fabd778d09f5c745e0ec1dcc3b3cbbe7f4ffd44693298a6"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 7b8416a736e32daa0963995cf62a10455ebbc54a5c02264496db4d074cd9ba2e
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
    "id": 5,
    "course_id": 248,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-29T17:22:50.389Z",
    "course_published": true,
    "updated_at": "2016-10-29T17:22:50.379Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b8416a736e32daa0963995cf62a10455ebbc54a5c02264496db4d074cd9ba2e"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 7537eaedd73356bf4923b6ef29cce1c955d51cc04740af46dbf43481650ac2d9
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
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 99,
      "user_id": 739
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 739
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 101,
      "user_id": 739
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 102,
      "user_id": 739
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7537eaedd73356bf4923b6ef29cce1c955d51cc04740af46dbf43481650ac2d9"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/28
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
    "id": 28,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 28,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 28
      },
      {
        "id": 29,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 28
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/28" -X GET \
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
      "id": 29,
      "name": "Expanded solution-oriented product",
      "name_translations": {
        "en": "Expanded solution-oriented product"
      }
    },
    {
      "id": 30,
      "name": "Horizontal bandwidth-monitored implementation",
      "name_translations": {
        "en": "Horizontal bandwidth-monitored implementation"
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
PATCH /v2/feedbacks/2/close
Content-Type: application/json
Authorization: Bearer c27a7ffbd07d58e0d2605d8fc81e3eeb2eaea9834713b00c18389ef4b1d86b72
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
    "id": 2,
    "user_id": 151,
    "feedbackable_id": 27,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-29T17:22:04.554Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c27a7ffbd07d58e0d2605d8fc81e3eeb2eaea9834713b00c18389ef4b1d86b72"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/6/fix
Content-Type: application/json
Authorization: Bearer fc05a244a457318dd86313a51a717874d0d88351bc44e59c3d9e3ca0ab35fca4
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
    "id": 6,
    "user_id": 171,
    "feedbackable_id": 31,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-29T17:22:05.376Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/6/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc05a244a457318dd86313a51a717874d0d88351bc44e59c3d9e3ca0ab35fca4"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/8
Content-Type: application/json
Authorization: Bearer 8b1c2f3417300440e27fe1e4f3468e2f76ec7bbf8d3db7b08d7985cbd0877d30
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
    "id": 8,
    "user_id": 181,
    "feedbackable_id": 33,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-29T17:22:06.029Z",
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
curl "api.goskive.com/v2/feedbacks/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b1c2f3417300440e27fe1e4f3468e2f76ec7bbf8d3db7b08d7985cbd0877d30"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer f40016fdb611dcf65c831fc2aefccd27e64eb6c372c8ab6144cbe6e5d6f6334b
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
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f40016fdb611dcf65c831fc2aefccd27e64eb6c372c8ab6144cbe6e5d6f6334b"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer 0e7a48ac4cf5dc7389efeeb5c803790a69d41e6745c720b42a9331da6a10c386
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
curl "api.goskive.com/v2/feedbacks/4/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e7a48ac4cf5dc7389efeeb5c803790a69d41e6745c720b42a9331da6a10c386"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer f37e47e34f97d0cfa57f2d07b6987395de22813eb57a069a97f954fd495ea926
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
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f37e47e34f97d0cfa57f2d07b6987395de22813eb57a069a97f954fd495ea926"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/9
Content-Type: application/json
Authorization: Bearer 165c12d93c4ce3ff58a16315651597b7ca2b318a541d73cf067ba82c6c8ff037
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
    "id": 9,
    "user_id": 186,
    "feedbackable_id": 34,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-29T17:22:06.281Z",
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
curl "api.goskive.com/v2/feedbacks/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 165c12d93c4ce3ff58a16315651597b7ca2b318a541d73cf067ba82c6c8ff037"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 2f3a43bdd7baaad3917653f27b9928426c829e95817b03ad7ceef5cc49893f26
```

`DELETE /v2/files/:file_id`

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
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f3a43bdd7baaad3917653f27b9928426c829e95817b03ad7ceef5cc49893f26"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/18/bookmark
Content-Type: application/json
Authorization: Bearer 3c479938fd948d393d3d42c448adefb7a781259eb33cac03a638b71ddde88da6
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c479938fd948d393d3d42c448adefb7a781259eb33cac03a638b71ddde88da6"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer 53d222022ec92d1c7b9c8b71b931ced70667351162bff2ad2827cb6a06400d8b
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53d222022ec92d1c7b9c8b71b931ced70667351162bff2ad2827cb6a06400d8b"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/9
Content-Type: application/json
Authorization: Bearer c5a585bbbcfa3b313cf8a964a96d1cad3fd8c19b5736bac48791d2220d123bac
```

`GET /v2/files/:file_id`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "file_link": {
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5dfb109332f5c968bb83fac579b3672e.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161029%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161029T172237Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=494a0e91414c9fc102f40d8ddb70d494db2c93d46825c1434e7954ab4fb7304c",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5a585bbbcfa3b313cf8a964a96d1cad3fd8c19b5736bac48791d2220d123bac"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer 67d893f9e3d6346402901ab895a3cf1c36abb728654af6de882f5e261f3a6f46
```

`GET /v2/files/:file_id/preview`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "file_link": {
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/1444877ede61ac3c26a54a878ed9d4ba.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161029%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161029T172238Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=74e000cc480fd65850944d4db38bea30e8c199cd9cc01b3b3528fc076f63222e",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67d893f9e3d6346402901ab895a3cf1c36abb728654af6de882f5e261f3a6f46"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 532510283fa5495290e637fcd9f7700495bd97a777b6c4e44564be323e71cdd2
```

`GET /v2/files/:file_id/metadata`

#### Parameters


None known.


### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "file": {
    "id": 11,
    "uploader": {
      "id": 579,
      "first_name": "Kasper",
      "last_name": "Skive",
      "nickname": "Kasper Skive",
      "type": "Student",
      "avatar_thumb_url": null,
      "university_id": null,
      "fields_of_study": [

      ],
      "study_level": null,
      "graduation_year": null,
      "created_at": "2016-10-29T17:22:38.018Z",
      "updated_at": "2016-10-29T17:22:38.018Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-29T17:22:38.088Z",
    "updated_at": "2016-10-29T17:22:38.088Z",
    "course_id": 205,
    "filename": "Pastry Making Notes.pdf",
    "description": null,
    "category": "other",
    "is_anonymous": false
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file[id] | File ID |
| file[uploader] | Uploader |
| file[filename] | Filename |
| file[description] | Description |
| file[status] | Status |
| file[download_count] | Download count |
| file[created_at] | Created at |
| file[updated_at] | Updated at |
| file[course_id] | Course ID |
| file[category] | Category |
| file[is_anonymous] | Uploader is anonymous |


```shell
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 532510283fa5495290e637fcd9f7700495bd97a777b6c4e44564be323e71cdd2"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/20/matched_courses?required_cu_count=2
Authorization: Bearer c3096e0fae7a1da4e72d1e63794c21578ad066febc8a16d07ef13d5ee04b6cfc
```

`GET /v2/files/:file_id/matched_courses`

#### Parameters


```json
required_cu_count: 2
```


| Name | Description |
|:-----|:------------|
| required_cu_count  | Number of CUs a course must have to be matched (default: 24) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "courses": [
    {
      "creator_id": 966,
      "id": 311,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 296,
      "additional_university_ids": [

      ],
      "topic_id": 323,
      "discipline_id": 324,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": true,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-10-29T17:23:09.723Z",
      "updated_at": "2016-10-29T17:23:11.258Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 971,
      "id": 312,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-2642e161-9dee-4f51-9010-a517310b3a0f",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-2642e161-9dee-4f51-9010-a517310b3a0f",
      "slug": "mit-the-great-british-bake-off-2642e161-9dee-4f51-9010-a517310b3a0f",
      "university_id": 297,
      "additional_university_ids": [

      ],
      "topic_id": 324,
      "discipline_id": 325,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "users_count": 0,
      "user_generated": true,
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": true,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": "2016-10-29T17:23:09.723Z",
      "updated_at": "2016-10-29T17:23:11.789Z",
      "shortname": "mit-the-great-british-bake-off-2642e161-9dee-4f51-9010-a517310b3a0f"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/20/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer c3096e0fae7a1da4e72d1e63794c21578ad066febc8a16d07ef13d5ee04b6cfc"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/17/report
Content-Type: application/json
Authorization: Bearer 2112ee5f67c770eefc64b40255d3ed5d1579cc458b42276a54bdcaae80b07953
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2112ee5f67c770eefc64b40255d3ed5d1579cc458b42276a54bdcaae80b07953"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/19/bookmark
Content-Type: application/json
Authorization: Bearer 8bb3a1d6f35a2fd3900bc6d29a9712840047689673df87dba9ef9f27880dace5
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8bb3a1d6f35a2fd3900bc6d29a9712840047689673df87dba9ef9f27880dace5"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/8/upvote
Content-Type: application/json
Authorization: Bearer a6f882d5a1817b6b3ff1db5b2cd251321346d14c9333003ec29419bbf42fccd9
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6f882d5a1817b6b3ff1db5b2cd251321346d14c9333003ec29419bbf42fccd9"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/77/comments
Content-Type: application/json
Authorization: Bearer fb9d67741c52562024c2a09db61e501155de9b4accdeb519e4deb1ac05173fea
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
    "id": 52,
    "author_id": 553,
    "reply_to_id": null,
    "created_at": "2016-10-29T17:22:36.618Z",
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
curl "api.goskive.com/v2/flashcards/77/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb9d67741c52562024c2a09db61e501155de9b4accdeb519e4deb1ac05173fea"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/79/comments
Content-Type: application/json
Authorization: Bearer 7f516359828420cf9e5ada986326da0b19c1835040ffe70a8de46d3561a31077
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
    "id": 53,
    "author_id": 559,
    "reply_to_id": null,
    "created_at": "2016-10-29T17:22:37.094Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 559,
      "feedbackable_id": 79,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:37.091Z",
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
curl "api.goskive.com/v2/flashcards/79/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f516359828420cf9e5ada986326da0b19c1835040ffe70a8de46d3561a31077"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/81/comments
Content-Type: application/json
Authorization: Bearer 12e3894afa6216766e5e8464bb9deb55528f758d8df89bd0f5f3c0a611c9653c
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
      "author_id": 568,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:37.566Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 569,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:37.581Z",
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
curl "api.goskive.com/v2/flashcards/81/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12e3894afa6216766e5e8464bb9deb55528f758d8df89bd0f5f3c0a611c9653c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/78/comments
Content-Type: application/json
Authorization: Bearer d7a6a10a80d31b0be5e85aab5af017f244c0c6a1156fdd1a345f60c02c37d3fd
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
curl "api.goskive.com/v2/flashcards/78/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7a6a10a80d31b0be5e85aab5af017f244c0c6a1156fdd1a345f60c02c37d3fd"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/41/feedbacks
Content-Type: application/json
Authorization: Bearer e843064f8eb7a597939d38db9f86adbaedeb6efecf516198dd80627843134fa7
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
    "id": 35,
    "user_id": 301,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-29T17:22:13.221Z",
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
curl "api.goskive.com/v2/flashcards/41/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e843064f8eb7a597939d38db9f86adbaedeb6efecf516198dd80627843134fa7"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/36/feedbacks
Content-Type: application/json
Authorization: Bearer 37911b613552f3bdb54409a1658bd81f7909b72446e189b60e0c577371999ef3
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
      "id": 30,
      "user_id": 278,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:12.272Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 277,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:12.262Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/36/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37911b613552f3bdb54409a1658bd81f7909b72446e189b60e0c577371999ef3"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/84/votes
Content-Type: application/json
Authorization: Bearer 3fb9fe4b9edd228db617e60dc9dec528c2cf4327d00a7f722e8a909ce4b41d66
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
      "id": 23,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 84,
      "user_id": 859
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 84,
      "user_id": 858
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 84,
      "user_id": 857
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fb9fe4b9edd228db617e60dc9dec528c2cf4327d00a7f722e8a909ce4b41d66"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/24/republish
Content-Type: application/json
Authorization: Bearer 10d1ff22def5b3dfdebd89520dee8fb3b3b0ad22aafbe8ac401110ccb923ab23
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
curl "api.goskive.com/v2/flashcards/24/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10d1ff22def5b3dfdebd89520dee8fb3b3b0ad22aafbe8ac401110ccb923ab23"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/22/bookmark
Content-Type: application/json
Authorization: Bearer 57dabe8b450da3597dc6c8c7e30c87c4f2f6bac4ccea8e7ee268fbb67a80403b
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/22/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57dabe8b450da3597dc6c8c7e30c87c4f2f6bac4ccea8e7ee268fbb67a80403b"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/16
Content-Type: application/json
Authorization: Bearer 3d86d619797df7682c77773eb9b2cd3d070fb89847b40643b28a5b2dd30dcabf
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d86d619797df7682c77773eb9b2cd3d070fb89847b40643b28a5b2dd30dcabf"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/19/downvote
Content-Type: application/json
Authorization: Bearer 5a43f8ffb8a24a845ae2b997dd5fb4e149834d7542ac560117c0b9f2f9cff0d1
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a43f8ffb8a24a845ae2b997dd5fb4e149834d7542ac560117c0b9f2f9cff0d1"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/18
Content-Type: application/json
Authorization: Bearer 2297904eb40923a8f8fbd1b02adb64cb4fefdb56a06ec1d7331939f6accc30c9
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
    "id": 18,
    "obfuscated_id": "9KZ-wsvd6MY",
    "author_id": 57,
    "chapter_id": 18,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:21:57.526Z",
    "created_at": "2016-10-29T17:21:57.526Z",
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
curl "api.goskive.com/v2/flashcards/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2297904eb40923a8f8fbd1b02adb64cb4fefdb56a06ec1d7331939f6accc30c9"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/20/report
Content-Type: application/json
Authorization: Bearer ff65b12feb51f5ee01e2d3dafa41c73f36ae9e25bcc7a9a41d80328538874348
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/20/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff65b12feb51f5ee01e2d3dafa41c73f36ae9e25bcc7a9a41d80328538874348"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/17/bookmark
Content-Type: application/json
Authorization: Bearer 2d497a158b303c9f4cf156b75b503275fa13dd2f51ad0ddecaeb6df0d71a16e2
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/17/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d497a158b303c9f4cf156b75b503275fa13dd2f51ad0ddecaeb6df0d71a16e2"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/upvote
Content-Type: application/json
Authorization: Bearer 411614cf3d6401fe5ad0d54c3bdeb7538603abf90c716df636ec726b1aed6ae4
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 411614cf3d6401fe5ad0d54c3bdeb7538603abf90c716df636ec726b1aed6ae4"
```
# ImageUpload

## presigns an upload


### Request

#### Endpoint

```
GET /v2/image_upload/cache/presign?extension=.jpg

```

`GET /v2/image_upload/cache/presign`

#### Parameters


```json
extension: .jpg
```


| Name | Description |
|:-----|:------------|
| extension  | File extension |



### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com",
  "fields": {
    "key": "cache/0e48e038c7ccfb961789d076ad810b8a.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yOVQxODoyMzowOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzBlNDhlMDM4YzdjY2ZiOTYxNzg5ZDA3NmFkODEwYjhhLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyOS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjlUMTcyMzA5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161029/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161029T172309Z",
    "x-amz-signature": "2d47142fdfba1f99a170f41f87c49a5f811e4f7ba8413364faf35fce95440bda"
  }
}
```



```shell
curl "api.goskive.com/v2/image_upload/cache/presign?extension=.jpg" -X GET 
```
# Job Sign Ups

## Sign up the current user with the given email address


### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 67208840c610914421fdd870f10f365a751dc0b95b52109e75a6add88beb02c8
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
curl "api.goskive.com/v2/me/jobs/3/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67208840c610914421fdd870f10f365a751dc0b95b52109e75a6add88beb02c8"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer ad6d6435f4e80acbbc9e2f958f3886a7980c81839bf663dc4c2f771563d7b246
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
curl "api.goskive.com/v2/me/jobs/1/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad6d6435f4e80acbbc9e2f958f3886a7980c81839bf663dc4c2f771563d7b246"
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
{"password":{"reset_password_token":"aJCZqq1FZ2SDxzQgR9fY","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 890,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-29T17:23:05.944Z",
  "updated_at": "2016-10-29T17:23:06.111Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
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
  "audit_id": 4749
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"aJCZqq1FZ2SDxzQgR9fY","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/30/comments
Content-Type: application/json
Authorization: Bearer 399a985c29df73bd8afccc3ed42cf8e40ca09e0fcf7cb359a4ce36edf8113731
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
    "id": 49,
    "author_id": 440,
    "reply_to_id": null,
    "created_at": "2016-10-29T17:22:21.476Z",
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
curl "api.goskive.com/v2/questions/30/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 399a985c29df73bd8afccc3ed42cf8e40ca09e0fcf7cb359a4ce36edf8113731"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/29/comments
Content-Type: application/json
Authorization: Bearer 8b2a739b0258673a79062280331c12690bf9227005c58c8aecab1ad77cd3e16a
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
    "id": 48,
    "author_id": 437,
    "reply_to_id": null,
    "created_at": "2016-10-29T17:22:21.008Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 37,
      "user_id": 437,
      "feedbackable_id": 29,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:22:21.005Z",
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
curl "api.goskive.com/v2/questions/29/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b2a739b0258673a79062280331c12690bf9227005c58c8aecab1ad77cd3e16a"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/32/comments
Content-Type: application/json
Authorization: Bearer 0dfda5b15e2ea194e97fe753006dcb4f12531a026bb5216eadb8b71bedcc4046
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
      "author_id": 449,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:22.288Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 450,
      "reply_to_id": null,
      "created_at": "2016-10-29T17:22:22.303Z",
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
curl "api.goskive.com/v2/questions/32/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dfda5b15e2ea194e97fe753006dcb4f12531a026bb5216eadb8b71bedcc4046"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/31/comments
Content-Type: application/json
Authorization: Bearer 16a7a415bc75b77ac6e7f0045d7707f063b00a8fa4c91db634418c8de0e6794a
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
curl "api.goskive.com/v2/questions/31/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16a7a415bc75b77ac6e7f0045d7707f063b00a8fa4c91db634418c8de0e6794a"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/112/feedbacks
Content-Type: application/json
Authorization: Bearer 3797df401a4ca38e5de63589da6fb8058d10798fb6f46451447f205e3221e30f
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
    "id": 39,
    "user_id": 797,
    "feedbackable_id": 112,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-29T17:22:58.100Z",
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
curl "api.goskive.com/v2/questions/112/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3797df401a4ca38e5de63589da6fb8058d10798fb6f46451447f205e3221e30f"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/119/feedbacks
Content-Type: application/json
Authorization: Bearer 7aa6a78d27ebac5f7b6b70759c116ecb9bf46adb74e0300b5d7c25f08f10690b
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
      "id": 46,
      "user_id": 832,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:23:00.606Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 831,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-29T17:23:00.596Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/119/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7aa6a78d27ebac5f7b6b70759c116ecb9bf46adb74e0300b5d7c25f08f10690b"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/120/votes
Content-Type: application/json
Authorization: Bearer 68d92c3e498bef5bfa654532be9d6eda1f9bd0c02d0237b13b1cb43dc894128b
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
      "votable_id": 120,
      "user_id": 839
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 120,
      "user_id": 838
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 120,
      "user_id": 837
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/120/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68d92c3e498bef5bfa654532be9d6eda1f9bd0c02d0237b13b1cb43dc894128b"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/88/republish
Content-Type: application/json
Authorization: Bearer 92b31aafcb46d31015cb05217de22df123af1ecac478e91dffb1b1f75fb84e1a
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
curl "api.goskive.com/v2/questions/88/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92b31aafcb46d31015cb05217de22df123af1ecac478e91dffb1b1f75fb84e1a"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/70/bookmark
Content-Type: application/json
Authorization: Bearer 3107acbf1f7a298ac369618f477d35a140cb325a46ca3a7bfcf4e6d877818a71
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/70/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3107acbf1f7a298ac369618f477d35a140cb325a46ca3a7bfcf4e6d877818a71"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/64
Content-Type: application/json
Authorization: Bearer 1bbbc9d9ef867c1b2b1da69282c4a82686abfb39abe43ca8507274753ac7ad9f
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/64" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bbbc9d9ef867c1b2b1da69282c4a82686abfb39abe43ca8507274753ac7ad9f"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/68/downvote
Content-Type: application/json
Authorization: Bearer d44831f9985da7a2e9c6aeea845e34023651f32a36d5b2381eebebdbd50eaad0
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/68/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d44831f9985da7a2e9c6aeea845e34023651f32a36d5b2381eebebdbd50eaad0"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/86
Content-Type: application/json
Authorization: Bearer e2a38539b3df8f6af3659698547ffef37f149e918d4b6a3f938a952879cfba32
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
    "id": 86,
    "obfuscated_id": "7q-2LHZR3Kk",
    "author_id": 675,
    "chapter_id": 125,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:46.777Z",
    "created_at": "2016-10-29T17:22:46.665Z",
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
        "id": 172,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 173,
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
curl "api.goskive.com/v2/questions/86" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2a38539b3df8f6af3659698547ffef37f149e918d4b6a3f938a952879cfba32"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/66/report
Content-Type: application/json
Authorization: Bearer 7a12081726ed5b373b0ed47a012f323c32a0b9aed6250f260dfa7344f964c77a
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/66/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a12081726ed5b373b0ed47a012f323c32a0b9aed6250f260dfa7344f964c77a"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/67/bookmark
Content-Type: application/json
Authorization: Bearer 3c19de1f69e2efe556e891f5e687839645a2d001cd0da1eb2ff53c5c4dfc9f8d
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/67/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c19de1f69e2efe556e891f5e687839645a2d001cd0da1eb2ff53c5c4dfc9f8d"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/69
Content-Type: application/json
Authorization: Bearer 2ed5881dd89e7c5f35b67b5c631f77310cb700699a473374327cac1579355fcb
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":69,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-29T17:22:41.509Z","updated_at":"2016-10-29T17:22:41.619Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":108,"author_id":619,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 69,
    "obfuscated_id": "1EDi_PBgOnI",
    "author_id": 619,
    "chapter_id": 108,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-29T17:22:41.725Z",
    "created_at": "2016-10-29T17:22:41.509Z",
    "tags": [
      {
        "id": 12,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 11,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>69, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-29T17:22:41.509Z\", \"updated_at\"=>\"2016-10-29T17:22:41.619Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>108, \"author_id\"=>619, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 137,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 138,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 139,
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
curl "api.goskive.com/v2/questions/69" -d '{"question":{"question":{"id":69,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-29T17:22:41.509Z","updated_at":"2016-10-29T17:22:41.619Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":108,"author_id":619,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ed5881dd89e7c5f35b67b5c631f77310cb700699a473374327cac1579355fcb"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/65/upvote
Content-Type: application/json
Authorization: Bearer e50a34d934eb0c6dc1fec1c28496f901e28c232ca3eee4007642019a5af9ec58
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e50a34d934eb0c6dc1fec1c28496f901e28c232ca3eee4007642019a5af9ec58"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 02e8490b728d4d6d24cd71db06f084c5d74eb04bb06051e1e4b9c22d543b4105
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
      "creator_id": 952,
      "id": 306,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 289,
      "additional_university_ids": [

      ],
      "topic_id": 318,
      "discipline_id": 319,
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
      "updated_at": "2016-10-29T17:23:09.424Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02e8490b728d4d6d24cd71db06f084c5d74eb04bb06051e1e4b9c22d543b4105"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 23869b7188a65e5e9ec258d0d2b04f5540c5e03817f6071af509c3e800d39a30
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
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-272",
      "html_url": "https://goskive.com/university/uni-272",
      "slug": "uni-272",
      "name": "National School of Pizza",
      "short_name": "Uni 272",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/20e5c51187ec948e052848f3b57e570e978e8b6f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8024b910efd1a3812aea8c21604c3c62792ea5fa.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-29T17:23:09.601Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-271",
      "html_url": "https://goskive.com/university/uni-271",
      "slug": "uni-271",
      "name": "National School of Pastry",
      "short_name": "Uni 271",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/bd27ba3e14a65dc475bce92147a15b35bb84678e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f94654da13a014f55605131ca96388e79c0b329b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-29T17:23:09.585Z",
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
	-H "Authorization: Bearer 23869b7188a65e5e9ec258d0d2b04f5540c5e03817f6071af509c3e800d39a30"
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
      "id": 52,
      "name": "Reverse-engineered high-level middleware",
      "name_translations": {
        "en": "Reverse-engineered high-level middleware"
      },
      "discipline_id": 53
    },
    {
      "id": 53,
      "name": "Virtual transitional benchmark",
      "name_translations": {
        "en": "Virtual transitional benchmark"
      },
      "discipline_id": 54
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
GET /v2/topics/51
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
    "id": 51,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 52
  }
}
```



```shell
curl "api.goskive.com/v2/topics/51" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 1f79b63169ddc6514ac4c2d44433b52859622f71e6b1da5d625f793b2f0a2639
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
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-247",
      "html_url": "https://goskive.com/university/uni-247",
      "slug": "uni-247",
      "name": "University 207",
      "short_name": "Uni 247",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6cb0767d892cc8879578b821a4eb9a439587d479.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cc4bad62409aa99d1025d7305d8af9df4f0843b3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-29T17:23:02.997Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-248",
      "html_url": "https://goskive.com/university/uni-248",
      "slug": "uni-248",
      "name": "University 208",
      "short_name": "Uni 248",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0914df35f2caf4db0b883b888a57e4aa205d0cb2.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ead055e4e53075a89755412dbacadc6f3ed569cc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-29T17:23:03.013Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-249",
      "html_url": "https://goskive.com/university/uni-249",
      "slug": "uni-249",
      "name": "University 209",
      "short_name": "Uni 249",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d17c2e4a2164b62a17fa620b0e2b7b1e762dc4d5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/bc4ac250e6cea7a1fcec8d05dff47a0f5029593b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-29T17:23:03.028Z",
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
	-H "Authorization: Bearer 1f79b63169ddc6514ac4c2d44433b52859622f71e6b1da5d625f793b2f0a2639"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer d261ab60df7e631041f17527d0bda0188c3f697a194817c316344e8a03af6a8f
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
    "id": 266,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6208a3a772e527892e6a4237a00542fc37ad69ff.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ab9d27d36a3b474dc2746a2eab6daae8559768b1.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-29T17:23:02.942Z",
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
	-H "Authorization: Bearer d261ab60df7e631041f17527d0bda0188c3f697a194817c316344e8a03af6a8f"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1fb4968f585df2b70dc44ccb6eefaa042d16e85e7ac2dd7d4c3028ac5763cb0b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":151,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 457,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 141,
    "additional_university_ids": [

    ],
    "topic_id": 151,
    "discipline_id": 152,
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
    "chapters_updated_at": "2016-10-29T17:22:23.038Z",
    "updated_at": "2016-10-29T17:22:23.171Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 79,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-29T17:22:23.125Z",
        "course_id": 141,
        "author_id": 457,
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
        "id": 80,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-29T17:22:23.143Z",
        "course_id": 141,
        "author_id": 457,
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
        "id": 81,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-29T17:22:23.160Z",
        "course_id": 141,
        "author_id": 457,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":151,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fb4968f585df2b70dc44ccb6eefaa042d16e85e7ac2dd7d4c3028ac5763cb0b"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e40c5373fef6b2d7cb8b68be69e958dea9149267ea50490d93d04fcc40cdd76a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":150,"published":false}}
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
    "creator_id": 456,
    "id": 140,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 140,
    "additional_university_ids": [

    ],
    "topic_id": 150,
    "discipline_id": 151,
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
    "updated_at": "2016-10-29T17:22:23.005Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":150,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e40c5373fef6b2d7cb8b68be69e958dea9149267ea50490d93d04fcc40cdd76a"
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
      "creator_id": 473,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-133",
      "html_url": "https://goskive.com/course/fu-course-133",
      "slug": "fu-course-133",
      "university_id": 147,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 167,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 133",
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
      "updated_at": "2016-10-29T17:22:24.623Z",
      "shortname": "fu-course-133"
    },
    {
      "creator_id": 473,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 147,
      "additional_university_ids": [

      ],
      "topic_id": 167,
      "discipline_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
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
      "chapters_updated_at": "2016-10-29T17:22:24.952Z",
      "updated_at": "2016-10-29T17:22:24.961Z",
      "shortname": "fu-course-134"
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
Authorization: Bearer dfdcf8c8c27ab1ed9fd76656326ee75b3ad660a9b40daad4603668e79a3420c2
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
      "creator_id": 480,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 174,
      "discipline_id": 175,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
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
      "updated_at": "2016-10-29T17:22:25.388Z",
      "shortname": "fu-course-141"
    },
    {
      "creator_id": 480,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 175,
      "discipline_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "chapters_updated_at": "2016-10-29T17:22:25.708Z",
      "updated_at": "2016-10-29T17:22:25.716Z",
      "shortname": "fu-course-142"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfdcf8c8c27ab1ed9fd76656326ee75b3ad660a9b40daad4603668e79a3420c2"
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
      "creator_id": 478,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 170,
      "discipline_id": 171,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
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
      "updated_at": "2016-10-29T17:22:25.172Z",
      "shortname": "fu-course-137"
    },
    {
      "creator_id": 478,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 171,
      "discipline_id": 172,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
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
      "updated_at": "2016-10-29T17:22:25.211Z",
      "shortname": "fu-course-138"
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
Authorization: Bearer 13d3d3ee96d84a8ee6b3613e6f9150bc405081505a81f42fe6c7b6561f7af927
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
      "creator_id": 487,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
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
      "updated_at": "2016-10-29T17:22:25.990Z",
      "shortname": "fu-course-145"
    },
    {
      "creator_id": 487,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
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
      "updated_at": "2016-10-29T17:22:26.032Z",
      "shortname": "fu-course-146"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13d3d3ee96d84a8ee6b3613e6f9150bc405081505a81f42fe6c7b6561f7af927"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer a0f325e5c646278b1e4547bff2a359034786408f30d875b2f84139f4652ee7ac
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
  "id": 93,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-29T17:22:00.406Z",
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
	-H "Authorization: Bearer a0f325e5c646278b1e4547bff2a359034786408f30d875b2f84139f4652ee7ac"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/864
Content-Type: application/json
Authorization: Bearer f76ef7e64ab9d7f6628c19761772f9576afab86c52ced4527653b059e3db13e1
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
    "id": 864,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 270,
    "fields_of_study": [
      297,
      298
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-29T17:23:03.181Z",
    "updated_at": "2016-10-29T17:23:03.181Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/864" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f76ef7e64ab9d7f6628c19761772f9576afab86c52ced4527653b059e3db13e1"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/866
Content-Type: application/json
Authorization: Bearer 6011165792c9b3d74e55fe473625ab115a033cf01e1ac0d6e3b80fe537a9447c
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
    "id": 866,
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
    "created_at": "2016-10-29T17:23:03.263Z",
    "updated_at": "2016-10-29T17:23:03.263Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/866" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6011165792c9b3d74e55fe473625ab115a033cf01e1ac0d6e3b80fe537a9447c"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/13
Content-Type: application/json
Authorization: Bearer f06d55e2e0e3320cbd4c872948c947df85dad7df80641d980b70bd257db031cf
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f06d55e2e0e3320cbd4c872948c947df85dad7df80641d980b70bd257db031cf"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer ff26e3cfb99d3e7e057f94f6d538aacce7d1aef9315749d933ade194ec26b408
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
    "id": 14,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 110,
    "user_id": 789
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff26e3cfb99d3e7e057f94f6d538aacce7d1aef9315749d933ade194ec26b408"
```
