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
Authorization: Basic YjJkOGYwYjI3ZWZhN2M0YTE2ODU0Y2UwYzM5OWU0YzNlZTdkYjM2YmNlODI1
YjE3OGNhNDAwYTdlNDg2NjE4YzoyYTZkZDk1NTRiN2U1YWM1YjRiODYyZmRi
ZWIxNmRmNDllMmUxYjFjYzA1OTIxNTg4YmRkNGQ2NzRjNmE0YTky

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
	-u b2d8f0b27efa7c4a16854ce0c399e4c3ee7db36bce825b178ca400a7e486618c:2a6dd9554b7e5ac5b4b862fdbeb16df49e2e1b1cc05921588bdd4d674c6a4a92
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7daa9083a48000ae18c8b040ddb285a1a9da62bf88134014405d5a7d29e76f1f","client_secret":"6bfb7631c0bd5649df66c120ba4b97abca135bc70f1fe4733953fbf0cacd2f92"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7daa9083a48000ae18c8b040ddb285a1a9da62bf88134014405d5a7d29e76f1f","client_secret":"6bfb7631c0bd5649df66c120ba4b97abca135bc70f1fe4733953fbf0cacd2f92"}' -X POST \
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
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ODQ5MzI1NTZmY2QwNjEzZDk5ZmJlNDVmYTFjZjIzMmE5YTAzYzUzZmM1NTAy
YmM3Y2Q0NjljYzUyMGRjNzdiZjo2OTg5NDFkNTM1YjA4MGYzYzA2MzQ5NjI3
NWZlNzE5MTdmYTZlY2EyM2RhZDdmM2U1ODcwN2I5NjJiNjI0NTY0

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
  "access_token": "a1a27713a477925d6fc5a01de0a84cbc3ea5eef1d9bcb8723d2ded498578d9dc",
  "token_type": "bearer",
  "created_at": 1481230355
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 84932556fcd0613d99fbe45fa1cf232a9a03c53fc5502bc7cd469cc520dc77bf:698941d535b080f3c063496275fe71917fa6eca23dad7f3e58707b962b624564
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2ff42bd79452692fc93d95da7621c9c9d9ba48404370cceae0bcc48ec9677ede","client_secret":"d9d9e1a87da6d3fd99eddadcf48ee53faf8c7ca535b3c85b96cac60b01b7dd95"}
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
  "access_token": "9429aaec96db823b5e7e5e3cc7f4038c02e9c2f1da4a9a58a971c60fc091ac1e",
  "token_type": "bearer",
  "created_at": 1481230355
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2ff42bd79452692fc93d95da7621c9c9d9ba48404370cceae0bcc48ec9677ede","client_secret":"d9d9e1a87da6d3fd99eddadcf48ee53faf8c7ca535b3c85b96cac60b01b7dd95"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"620ea6cf157d373f010e932c86b5fa4a520e9f689564d782460f6bd540d52a95","client_secret":"bf992eeb0e0a9a40ab0ed9064ff8662a740f67dbbf983a1b0268caf41ae534f9"}
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
  "access_token": "4f5611a6651a45c598219cb9460442251d10c3902736883b610b2351618a50f9",
  "token_type": "bearer",
  "created_at": 1481230355
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"620ea6cf157d373f010e932c86b5fa4a520e9f689564d782460f6bd540d52a95","client_secret":"bf992eeb0e0a9a40ab0ed9064ff8662a740f67dbbf983a1b0268caf41ae534f9"}' -X POST \
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
Authorization: Bearer 9817d7e061925eff1db13e2a7234657696d0c2816cd1a3187c0355796a2167ac
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
    "company_id": 39,
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
	-H "Authorization: Bearer 9817d7e061925eff1db13e2a7234657696d0c2816cd1a3187c0355796a2167ac"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/195/flashcards
Content-Type: application/json
Authorization: Bearer 0a7b0ab4458aab8241a5c5ed79db90ff12880a15584db60e160deb7ac117ad24
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
    "author_id": 988,
    "chapter_id": 195,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:42.323Z",
    "created_at": "2016-12-08T20:52:42.323Z",
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
curl "api.goskive.com/v2/chapters/195/flashcards" -d '{"flashcard":{"chapter_id":195,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a7b0ab4458aab8241a5c5ed79db90ff12880a15584db60e160deb7ac117ad24"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer 72052bd240c485bd81d1eb4df6de051f0ee45bb336eec6520137e44d07357cf9
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
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 983,
      "chapter_id": 194,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:42.013Z",
      "created_at": "2016-12-08T20:52:42.013Z",
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
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 983,
      "chapter_id": 194,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:42.053Z",
      "created_at": "2016-12-08T20:52:42.053Z",
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
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 983,
      "chapter_id": 194,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:42.091Z",
      "created_at": "2016-12-08T20:52:42.091Z",
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
curl "api.goskive.com/v2/chapters/194/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72052bd240c485bd81d1eb4df6de051f0ee45bb336eec6520137e44d07357cf9"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/189/questions
Content-Type: application/json
Authorization: Bearer 0a6075846c6b5e4f14375b521a97f90447dcbff4e1d96af1e56ada25c50dc967
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":189,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 131,
    "obfuscated_id": "gCw8isdgMKE",
    "author_id": 955,
    "chapter_id": 189,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:38.939Z",
    "created_at": "2016-12-08T20:52:38.939Z",
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
        "id": 263,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 264,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 265,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 266,
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
curl "api.goskive.com/v2/chapters/189/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":189,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a6075846c6b5e4f14375b521a97f90447dcbff4e1d96af1e56ada25c50dc967"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/188/questions
Content-Type: application/json
Authorization: Bearer 534ce27a5ae8864dea46a614cb87bcdca263b5bf836c5a9df31b12be3eacae31
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":188,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 130,
    "obfuscated_id": "N-qIf0IsvWM",
    "author_id": 952,
    "chapter_id": 188,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:38.441Z",
    "created_at": "2016-12-08T20:52:38.441Z",
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
        "id": 261,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 262,
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
curl "api.goskive.com/v2/chapters/188/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":188,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 534ce27a5ae8864dea46a614cb87bcdca263b5bf836c5a9df31b12be3eacae31"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/190/questions
Content-Type: application/json
Authorization: Bearer 3e32827184507c871b020e3ae799a2c278320c87a3bb22b3590b6aedc45cd2d1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":190,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 132,
    "obfuscated_id": "RECRPLqMrqE",
    "author_id": 958,
    "chapter_id": 190,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:39.519Z",
    "created_at": "2016-12-08T20:52:39.519Z",
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
        "id": 267,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 268,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/190/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":190,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e32827184507c871b020e3ae799a2c278320c87a3bb22b3590b6aedc45cd2d1"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/187/questions
Content-Type: application/json
Authorization: Bearer ad6acb11e9be18d409cac1c508db6d798691b867a7933fdc163c12416cbe7d6b
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":187,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 129,
    "obfuscated_id": "x8EyeGrWnN4",
    "author_id": 949,
    "chapter_id": 187,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:38.000Z",
    "created_at": "2016-12-08T20:52:38.000Z",
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
        "id": 258,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 259,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 260,
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
curl "api.goskive.com/v2/chapters/187/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":187,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad6acb11e9be18d409cac1c508db6d798691b867a7933fdc163c12416cbe7d6b"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/186/questions
Content-Type: application/json
Authorization: Bearer d6b09566b106cacd679ecf004ab609641c847a5034bf99b3ac51f1f0e74967e7
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
      "id": 126,
      "obfuscated_id": "fKTMLttUR-w",
      "author_id": 943,
      "chapter_id": 186,
      "position": 117,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:37.428Z",
      "created_at": "2016-12-08T20:52:37.346Z",
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
          "id": 252,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 253,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 127,
      "obfuscated_id": "E3yfRgAzssw",
      "author_id": 944,
      "chapter_id": 186,
      "position": 118,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:37.574Z",
      "created_at": "2016-12-08T20:52:37.491Z",
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
          "id": 254,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 255,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 128,
      "obfuscated_id": "Q4ODZIcqv0E",
      "author_id": 945,
      "chapter_id": 186,
      "position": 119,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:37.723Z",
      "created_at": "2016-12-08T20:52:37.638Z",
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
          "id": 256,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 257,
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
curl "api.goskive.com/v2/chapters/186/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6b09566b106cacd679ecf004ab609641c847a5034bf99b3ac51f1f0e74967e7"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/42
Content-Type: application/json
Authorization: Bearer 2564666622d54e192f1dd06814472dfd24ad0fe2410358525f8149bb4ae28c38
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
curl "api.goskive.com/v2/chapters/42" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2564666622d54e192f1dd06814472dfd24ad0fe2410358525f8149bb4ae28c38"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/43
Content-Type: application/json
Authorization: Bearer 57821147c970c48c5c9876bd4b4f4c70deabbc4d3cc2ff91f218fd2f00f01f86
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
curl "api.goskive.com/v2/chapters/43" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57821147c970c48c5c9876bd4b4f4c70deabbc4d3cc2ff91f218fd2f00f01f86"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/39
Content-Type: application/json
Authorization: Bearer 0472725476ef1576b57573c5c4438cf5002e1ff3c5eeabc35358581724e57bed
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
curl "api.goskive.com/v2/chapters/39" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0472725476ef1576b57573c5c4438cf5002e1ff3c5eeabc35358581724e57bed"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/41
Content-Type: application/json
Authorization: Bearer 9f22398017a76a55fe698a56b3b08768edb28130936a89c22e4e99c6cc4dcb47
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/41" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f22398017a76a55fe698a56b3b08768edb28130936a89c22e4e99c6cc4dcb47"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/35
Content-Type: application/json
Authorization: Bearer a3232be66dfafcadfb06fdff234ba78b952685c4e3c07b5180f3748ff1d7f633
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
    "id": 35,
    "updated_at": "2016-12-08T20:51:34.828Z",
    "course_id": 49,
    "author_id": 199,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-08T20:51:34.339Z",
    "questions_updated_at": "2016-12-08T20:51:34.339Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 203,
        "chapter_id": 35,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:34.809Z",
        "created_at": "2016-12-08T20:51:34.809Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 201,
        "chapter_id": 35,
        "position": 24,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:34.686Z",
        "created_at": "2016-12-08T20:51:34.603Z",
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
            "id": 47,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 48,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3232be66dfafcadfb06fdff234ba78b952685c4e3c07b5180f3748ff1d7f633"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/38
Content-Type: application/json
Authorization: Bearer 00f377fad28aec4828864070bb14e1fe5ba66ce9c23fc6932717b001a7633da0
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
    "id": 38,
    "updated_at": "2016-12-08T20:51:35.831Z",
    "course_id": 52,
    "author_id": 216,
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

    ],
    "title": "Eggs and Flour",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/38" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00f377fad28aec4828864070bb14e1fe5ba66ce9c23fc6932717b001a7633da0"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/59/replies
Content-Type: application/json
Authorization: Bearer 930f66953f21aac6294ca27267bc1bd47561fc2733fdc627aaf03cb81abd2f48
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
    "id": 60,
    "author_id": 979,
    "reply_to_id": 59,
    "created_at": "2016-12-08T20:52:41.566Z",
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
curl "api.goskive.com/v2/comments/59/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 930f66953f21aac6294ca27267bc1bd47561fc2733fdc627aaf03cb81abd2f48"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 9898fb9caa482137c6117a66cd4fc3b62a36f1b98bda92b2ced8ed67c68396aa
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
curl "api.goskive.com/v2/comments/58/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9898fb9caa482137c6117a66cd4fc3b62a36f1b98bda92b2ced8ed67c68396aa"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 23ead4cc905e78de223760ecb2645b27ac138076eb3ef235d70d92fe24c6bc5b
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
	-H "Authorization: Bearer 23ead4cc905e78de223760ecb2645b27ac138076eb3ef235d70d92fe24c6bc5b"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer b2b2bdeb7fa700605725c1fbc181e95af883a2e0928170afb64b39d1c756708e
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
curl "api.goskive.com/v2/comments/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2b2bdeb7fa700605725c1fbc181e95af883a2e0928170afb64b39d1c756708e"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer bafd58c8a2c13ef60a0ba899aba4063916f9ef247607dbdf67e38e76b78b9e45
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bafd58c8a2c13ef60a0ba899aba4063916f9ef247607dbdf67e38e76b78b9e45"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/44/report
Content-Type: application/json
Authorization: Bearer 58f9df333cc8496c63f49b6492bfe2f8c406bb7f267d13ffcb4f918ee42db49e
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
	-H "Authorization: Bearer 58f9df333cc8496c63f49b6492bfe2f8c406bb7f267d13ffcb4f918ee42db49e"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/35
Content-Type: application/json
Authorization: Bearer fc36c76ce7055ab194e7b82e7cc8ad4ef64ca8ad39da023d96309ebf6a466138
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
    "id": 35,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-08T20:52:40.156Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc36c76ce7055ab194e7b82e7cc8ad4ef64ca8ad39da023d96309ebf6a466138"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer ca65ed2153508d0e58e33be978a3bbf26c98d34fafced79467d81bb68591c1b9
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
      "id": 36,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T20:52:40.227Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T20:52:40.232Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T20:52:40.236Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca65ed2153508d0e58e33be978a3bbf26c98d34fafced79467d81bb68591c1b9"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/33/company_profiles
Content-Type: application/json
Authorization: Bearer 5a6ad6b06a37bf9cd85c5535b01d2d08825845b3229469508606ac94b8f5fa91
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
curl "api.goskive.com/v2/companies/33/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a6ad6b06a37bf9cd85c5535b01d2d08825845b3229469508606ac94b8f5fa91"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/32/company_profiles
Content-Type: application/json
Authorization: Bearer f4a207d527622d675c7741f8117e69b0259215049b4c472943797029ed501416
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
curl "api.goskive.com/v2/companies/32/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4a207d527622d675c7741f8117e69b0259215049b4c472943797029ed501416"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer cd67c011984f0430e1ab63f76e165170f8608be27c918410f9c60ac2db7101a0
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
	-H "Authorization: Bearer cd67c011984f0430e1ab63f76e165170f8608be27c918410f9c60ac2db7101a0"
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
Authorization: Bearer e3ffd1578ddc04763a9561c6dacc072699385a51e4642a530b02a526e09ff733
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
	-H "Authorization: Bearer e3ffd1578ddc04763a9561c6dacc072699385a51e4642a530b02a526e09ff733"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 52f04927d7a51b51dd79c56fea9ddbfb5484f0e7a441d5c4c361a4c47dc42688
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
    "id": 78,
    "updated_at": "2016-12-08T20:51:44.514Z",
    "course_id": 83,
    "author_id": 333,
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

    ],
    "title": "Preparing the oven",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52f04927d7a51b51dd79c56fea9ddbfb5484f0e7a441d5c4c361a4c47dc42688"
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
      "id": 62,
      "updated_at": "2016-12-08T20:51:42.272Z",
      "course_id": 73,
      "author_id": 297,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 53",
      "position": 1
    },
    {
      "id": 63,
      "updated_at": "2016-12-08T20:51:42.297Z",
      "course_id": 73,
      "author_id": 298,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 54",
      "position": 2
    },
    {
      "id": 64,
      "updated_at": "2016-12-08T20:51:42.520Z",
      "course_id": 73,
      "author_id": 299,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T20:51:42.173Z",
      "questions_updated_at": "2016-12-08T20:51:42.173Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 55",
      "position": 3
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
Authorization: Bearer 03677c13f3a191e572b680de74b4bc2356b942ae24d777194c5d102eb74611e0
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
      "id": 68,
      "updated_at": "2016-12-08T20:51:42.984Z",
      "course_id": 76,
      "author_id": 308,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 59",
      "position": 1
    },
    {
      "id": 69,
      "updated_at": "2016-12-08T20:51:43.009Z",
      "course_id": 76,
      "author_id": 309,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 60",
      "position": 2
    },
    {
      "id": 70,
      "updated_at": "2016-12-08T20:51:43.235Z",
      "course_id": 76,
      "author_id": 310,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T20:51:42.883Z",
      "questions_updated_at": "2016-12-08T20:51:42.883Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 61",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03677c13f3a191e572b680de74b4bc2356b942ae24d777194c5d102eb74611e0"
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
      "id": 65,
      "updated_at": "2016-12-08T20:51:42.672Z",
      "course_id": 74,
      "author_id": 303,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 56",
      "position": 1
    },
    {
      "id": 66,
      "updated_at": "2016-12-08T20:51:42.698Z",
      "course_id": 74,
      "author_id": 304,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 57",
      "position": 2
    },
    {
      "id": 67,
      "updated_at": "2016-12-08T20:51:42.723Z",
      "course_id": 74,
      "author_id": 305,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 58",
      "position": 3
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
Authorization: Bearer 6fa1a55df788d102696b4ba3cff99299270b5921b1d499d0782ea513a1d8e491
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
      "id": 71,
      "updated_at": "2016-12-08T20:51:43.431Z",
      "course_id": 77,
      "author_id": 315,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 62",
      "position": 1
    },
    {
      "id": 72,
      "updated_at": "2016-12-08T20:51:43.457Z",
      "course_id": 77,
      "author_id": 316,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 63",
      "position": 2
    },
    {
      "id": 73,
      "updated_at": "2016-12-08T20:51:43.484Z",
      "course_id": 77,
      "author_id": 317,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 64",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fa1a55df788d102696b4ba3cff99299270b5921b1d499d0782ea513a1d8e491"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer ed6451399e1f72367691f3fa75d0a31e9b09fdd166aa13d3ab5cc0e93c8ce91c
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
    "course_id": 95,
    "user_id": 364,
    "updated_at": "2016-12-08T20:51:47.353Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed6451399e1f72367691f3fa75d0a31e9b09fdd166aa13d3ab5cc0e93c8ce91c"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c100e5ad0c5ffb1469b080a5cbf88644259376314bb592d670574e9beb1e2013
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
      "course_id": 93,
      "user_id": 358,
      "updated_at": "2016-12-08T20:51:46.929Z"
    },
    {
      "id": 4,
      "course_id": 93,
      "user_id": 359,
      "updated_at": "2016-12-08T20:51:46.944Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c100e5ad0c5ffb1469b080a5cbf88644259376314bb592d670574e9beb1e2013"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/299/files
Content-Type: application/json
Authorization: Bearer 45db061a495e9e7eb0c4a20f91d847637c6293fa6cb58206bc9dd9c4a6ecc2fb
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
      "id": 19,
      "uploader": {
        "id": 909,
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
        "created_at": "2016-12-08T20:52:34.716Z",
        "updated_at": "2016-12-08T20:52:34.716Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T20:52:34.726Z",
      "updated_at": "2016-12-08T20:52:34.726Z",
      "course_id": 299,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 20,
      "uploader": {
        "id": 910,
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
        "created_at": "2016-12-08T20:52:34.736Z",
        "updated_at": "2016-12-08T20:52:34.736Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T20:52:34.745Z",
      "updated_at": "2016-12-08T20:52:34.745Z",
      "course_id": 299,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 911,
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
        "created_at": "2016-12-08T20:52:34.754Z",
        "updated_at": "2016-12-08T20:52:34.754Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T20:52:34.764Z",
      "updated_at": "2016-12-08T20:52:34.764Z",
      "course_id": 299,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/299/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45db061a495e9e7eb0c4a20f91d847637c6293fa6cb58206bc9dd9c4a6ecc2fb"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/300/files
Content-Type: application/json
Authorization: Bearer 5c2f5d5f2dea64cf96c62fc0d128185e94106159b822df50f506705eee5cfe8c
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
    "id": 22,
    "uploader": {
      "id": 914,
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
      "created_at": "2016-12-08T20:52:34.917Z",
      "updated_at": "2016-12-08T20:52:34.917Z"
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
    "created_at": "2016-12-08T20:52:34.948Z",
    "updated_at": "2016-12-08T20:52:34.948Z",
    "course_id": 300,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/300/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c2f5d5f2dea64cf96c62fc0d128185e94106159b822df50f506705eee5cfe8c"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/297/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 1ab2b603975f375e2d5714bae85902deae70cf016449f88e6289e6f2ebbdbe42
```

`GET /v2/courses/:course_id/file_upload/cache/presign`

#### Parameters


```json
extension: .jpg
```


| Name | Description |
|:-----|:------------|
| extension  | File extension |
| filename  | Filename |



### Response

```
Content-Type: application/json
200 OK
```


```json
{
  "url": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com",
  "fields": {
    "key": "cache/6f9089f7ff26d6a2452815c1d337f0d5.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQyMTo1MjozNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzZmOTA4OWY3ZmYyNmQ2YTI0NTI4MTVjMWQzMzdmMGQ1LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA4VDIwNTIzNFoifV19",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T205234Z",
    "x-amz-signature": "8a1b09b0f9cfdb7cf9ee5872b19cc538d2bfe1ecc808cf59cdbf1dce97b8e1e7"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/297/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ab2b603975f375e2d5714bae85902deae70cf016449f88e6289e6f2ebbdbe42"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer d12a150da9616779ab4aa31557f907fb1fe261c7271cb581c0cdfb221dc5898d
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
	-H "Authorization: Bearer d12a150da9616779ab4aa31557f907fb1fe261c7271cb581c0cdfb221dc5898d"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c72444d075681b3e6f12cb3280d5b756175edee3c9e0c76ce675163852774802
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
	-H "Authorization: Bearer c72444d075681b3e6f12cb3280d5b756175edee3c9e0c76ce675163852774802"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 52e9dddd78b044b06be6164b6fcd50605b29575ee827d8fdee3d34fbf6e8cfdd
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
	-H "Authorization: Bearer 52e9dddd78b044b06be6164b6fcd50605b29575ee827d8fdee3d34fbf6e8cfdd"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 14e7307ebd85d9466b7c81fb89e2ddef674d48a7db0d65c9ac28a100aa3aa7a0
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
	-H "Authorization: Bearer 14e7307ebd85d9466b7c81fb89e2ddef674d48a7db0d65c9ac28a100aa3aa7a0"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f9691c42b8000964b675ecb31974cd655ac601f3282d692b1aa1e361b6dbe7e8
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
	-H "Authorization: Bearer f9691c42b8000964b675ecb31974cd655ac601f3282d692b1aa1e361b6dbe7e8"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer c40eab0a6d34b75e61d12a3d5aae6a58bb7359d5e6e97da9aa233b441d1d3471
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
    "creator_id": 564,
    "id": 174,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "discipline_id": 182,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 4,
    "questions_count": 4,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T20:52:02.516Z",
    "updated_at": "2016-12-08T20:52:03.852Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 565,
        "chapter_id": 96,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.616Z",
        "created_at": "2016-12-08T20:52:03.616Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 565,
        "chapter_id": 97,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.697Z",
        "created_at": "2016-12-08T20:52:03.697Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 565,
        "chapter_id": 96,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.661Z",
        "created_at": "2016-12-08T20:52:03.661Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 565,
        "chapter_id": 97,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.742Z",
        "created_at": "2016-12-08T20:52:03.742Z",
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
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 565,
        "chapter_id": 96,
        "position": 61,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:02.749Z",
        "created_at": "2016-12-08T20:52:02.656Z",
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
            "id": 121,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 122,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 565,
        "chapter_id": 96,
        "position": 62,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:02.899Z",
        "created_at": "2016-12-08T20:52:02.814Z",
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
            "id": 123,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 124,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 565,
        "chapter_id": 97,
        "position": 63,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.077Z",
        "created_at": "2016-12-08T20:52:02.983Z",
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
            "id": 125,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 126,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 565,
        "chapter_id": 97,
        "position": 64,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:03.229Z",
        "created_at": "2016-12-08T20:52:03.142Z",
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
            "id": 127,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 128,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ],
    "chapters": [
      {
        "id": 96,
        "updated_at": "2016-12-08T20:52:03.796Z",
        "course_id": 174,
        "author_id": 564,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T20:52:02.516Z",
        "questions_updated_at": "2016-12-08T20:52:02.516Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 84",
        "position": 1
      },
      {
        "id": 97,
        "updated_at": "2016-12-08T20:52:03.840Z",
        "course_id": 174,
        "author_id": 564,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T20:52:02.516Z",
        "questions_updated_at": "2016-12-08T20:52:02.516Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 85",
        "position": 2
      }
    ],
    "topic_id": 182,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c40eab0a6d34b75e61d12a3d5aae6a58bb7359d5e6e97da9aa233b441d1d3471"
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
    "creator_id": 570,
    "id": 175,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "discipline_id": 183,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 2,
    "questions_count": 2,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T20:52:04.000Z",
    "updated_at": "2016-12-08T20:52:05.422Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 570,
        "chapter_id": 98,
        "position": 67,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:04.365Z",
        "created_at": "2016-12-08T20:52:04.276Z",
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
            "id": 133,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 134,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 570,
        "chapter_id": 99,
        "position": 69,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:04.678Z",
        "created_at": "2016-12-08T20:52:04.584Z",
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
          }
        ]
      }
    ],
    "chapters": [
      {
        "id": 98,
        "updated_at": "2016-12-08T20:52:05.370Z",
        "course_id": 175,
        "author_id": 570,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T20:52:04.000Z",
        "questions_updated_at": "2016-12-08T20:52:04.000Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 86",
        "position": 1
      },
      {
        "id": 99,
        "updated_at": "2016-12-08T20:52:05.411Z",
        "course_id": 175,
        "author_id": 570,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T20:52:04.000Z",
        "questions_updated_at": "2016-12-08T20:52:04.000Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 87",
        "position": 2
      }
    ],
    "topic_id": 183,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": ""
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
PUT /v2/courses/178/pin
Content-Type: application/json
Authorization: Bearer 04f12a2d21c6e1a782d94ed85a1caeb7fa82a089db06609d57138c73ce647fea
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/178/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04f12a2d21c6e1a782d94ed85a1caeb7fa82a089db06609d57138c73ce647fea"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/160/pin
Content-Type: application/json
Authorization: Bearer 0334a4e22cec259b980654a8a45f547be3121a2d35ef1280873465d6d813cfaa
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/160/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0334a4e22cec259b980654a8a45f547be3121a2d35ef1280873465d6d813cfaa"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer af7af1fb8ac85780acde49b560d0912f4c1cc9801dcb6fc15d54f9d87a7384c2
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
    "creator_id": 541,
    "id": 163,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "discipline_id": 171,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-08T20:52:00.412Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 171,
    "language_code": "fr",
    "exam_months": [

    ],
    "title": "Choux pastry 102",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af7af1fb8ac85780acde49b560d0912f4c1cc9801dcb6fc15d54f9d87a7384c2"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer c7357ee7c051f5e51ec0fdd0c1ae8883ef72512403cd62366e56c4d5796433a9
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
    "id": 375,
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
    "created_at": "2016-12-08T20:51:48.538Z",
    "updated_at": "2016-12-08T20:51:48.538Z",
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
	-H "Authorization: Bearer c7357ee7c051f5e51ec0fdd0c1ae8883ef72512403cd62366e56c4d5796433a9"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ee0a4f6d9be9a657e0d1e6a98e723279fe5d2b70d357065ee915988df5979585
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[102]}
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
    "id": 371,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      102
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T20:51:48.235Z",
    "updated_at": "2016-12-08T20:51:48.278Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[102]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee0a4f6d9be9a657e0d1e6a98e723279fe5d2b70d357065ee915988df5979585"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 32e20bdb5b89bcb01a4a3072742b73ec246fc7f1cb414523b70a3f7e8d7c8611
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
    "id": 373,
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
    "created_at": "2016-12-08T20:51:48.382Z",
    "updated_at": "2016-12-08T20:51:48.382Z",
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
	-H "Authorization: Bearer 32e20bdb5b89bcb01a4a3072742b73ec246fc7f1cb414523b70a3f7e8d7c8611"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 18a9b143deecab630c89adf52bd7c715d8893ade7e5adec0a33620684e4505da
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[105]}
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
    "id": 374,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      105
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T20:51:48.477Z",
    "updated_at": "2016-12-08T20:51:48.477Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[105]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18a9b143deecab630c89adf52bd7c715d8893ade7e5adec0a33620684e4505da"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a0a247d9a5f6b6d011289322b074bd5b3d4d7cf10132419f82b72458098e83bd
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

101
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
    "id": 370,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0e880b5fb4ee50f38c49d21f6808a4d5af67000b.jpg",
    "university_id": null,
    "fields_of_study": [
      101
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T20:51:47.885Z",
    "updated_at": "2016-12-08T20:51:48.147Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/76753bcef54e8915a42cc93d80171144e0f24e23.jpg",
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

101
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a0a247d9a5f6b6d011289322b074bd5b3d4d7cf10132419f82b72458098e83bd"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer d3a8b6f9addfe179fae718f2e5706c6173b3b0be0765b1a54dd3941584a02624
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
      "id": 4,
      "bookmarkable_id": 45,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 46,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 47,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3a8b6f9addfe179fae718f2e5706c6173b3b0be0765b1a54dd3941584a02624"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d1bdd509b98ac5cef54d14793c22d7a85af9086f35b7be4143fd040c26e903c7
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
      "creator_id": 345,
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-61",
      "html_url": "https://goskive.com/course/mit-course-61",
      "slug": "mit-course-61",
      "university_id": 89,
      "additional_university_ids": [

      ],
      "discipline_id": 92,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:51:45.884Z",
      "shortname": "mit-course-61",
      "topic_id": 92,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 346,
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-62",
      "html_url": "https://goskive.com/course/mit-course-62",
      "slug": "mit-course-62",
      "university_id": 90,
      "additional_university_ids": [

      ],
      "discipline_id": 93,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:51:45.989Z",
      "shortname": "mit-course-62",
      "topic_id": 93,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 62",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1bdd509b98ac5cef54d14793c22d7a85af9086f35b7be4143fd040c26e903c7"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 615a94d7d2fc2cded2d778f7c390edd58f57cdfe7e7466725dde9223ca28a209
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
        "id": 14,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T20:51:52.004Z",
        "updated_at": "2016-12-08T20:51:52.004Z",
        "file_url": "memory://b260ed99ffc8168ea58cf3d3996e1cf1.pdf",
        "course_id": 110,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 15,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T20:51:52.134Z",
        "updated_at": "2016-12-08T20:51:52.134Z",
        "file_url": "memory://da5e9a21b388c8e337a8981db02d443f.pdf",
        "course_id": 111,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 16,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T20:51:52.236Z",
        "updated_at": "2016-12-08T20:51:52.236Z",
        "file_url": "memory://c39977e9a8ea558218c972a656edcea4.pdf",
        "course_id": 112,
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
	-H "Authorization: Bearer 615a94d7d2fc2cded2d778f7c390edd58f57cdfe7e7466725dde9223ca28a209"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 795306970a8f3a09456d57d4e1895336b31b70bc119a76e518fd7d69f8717193
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
      "company_id": 26,
      "company": {
        "id": 26,
        "name": "Fake Company Name 26",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T20:52:13.156Z"
      },
      "created_at": "2016-12-08T20:52:13.160Z",
      "updated_at": "2016-12-08T20:52:13.160Z",
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
      "company_id": 27,
      "company": {
        "id": 27,
        "name": "Fake Company Name 27",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T20:52:13.169Z"
      },
      "created_at": "2016-12-08T20:52:13.173Z",
      "updated_at": "2016-12-08T20:52:13.173Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 795306970a8f3a09456d57d4e1895336b31b70bc119a76e518fd7d69f8717193"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer d34c0650d0d0d9903bce1643bb410e4e8b1abd6c4923a614100590f8e41b39e8
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
      "id": 9,
      "created_at": "2016-12-08T20:52:10.388Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 50,
      "updated_at": "2016-12-08T20:52:10.522Z",
      "author_id": "613",
      "thread_subject_id": "185",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 10,
      "created_at": "2016-12-08T20:52:10.510Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 51,
      "updated_at": "2016-12-08T20:52:10.525Z",
      "author_id": "616",
      "thread_subject_id": "186",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-12-08T20:52:10.911Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-12-08T20:52:10.911Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 12,
      "created_at": "2016-12-08T20:52:11.290Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-12-08T20:52:11.290Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 13,
      "created_at": "2016-12-08T20:52:11.679Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-12-08T20:52:11.679Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 14,
      "created_at": "2016-12-08T20:52:11.979Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 88,
      "updated_at": "2016-12-08T20:52:11.979Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-12-08T20:52:12.283Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 89,
      "updated_at": "2016-12-08T20:52:12.283Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 16,
      "created_at": "2016-12-08T20:52:12.589Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 90,
      "updated_at": "2016-12-08T20:52:12.589Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d34c0650d0d0d9903bce1643bb410e4e8b1abd6c4923a614100590f8e41b39e8"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/8
Content-Type: application/json
Authorization: Bearer ed15c2c815989b506bd1678233c698376ab3dd38e7cb08c6d59aa86ef28b791b
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-08T20:42:10.000Z"}}
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
    "id": 8,
    "created_at": "2016-12-08T20:52:10.125Z",
    "read_at": "2016-12-08T20:42:10.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 49,
    "updated_at": "2016-12-08T20:52:10.180Z",
    "author_id": "608",
    "thread_subject_id": "184",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/8" -d '{"notification":{"read_at":"2016-12-08T20:42:10.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed15c2c815989b506bd1678233c698376ab3dd38e7cb08c6d59aa86ef28b791b"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer cd09adb2dca97c889091d10824844c15ae58487854f3744198dfe3acd7e06eaf
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
      "id": 6,
      "course_id": 269,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T20:52:26.481Z",
      "course_published": true,
      "updated_at": "2016-12-08T20:52:26.477Z"
    },
    {
      "id": 5,
      "course_id": 268,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T20:52:26.377Z",
      "course_published": true,
      "updated_at": "2016-12-08T20:52:26.373Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd09adb2dca97c889091d10824844c15ae58487854f3744198dfe3acd7e06eaf"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer e86c8ee0930bab40e3a91fd8be691cc7eeddc5fb52ad40ebb95e75c7e44de0b8
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
    "id": 8,
    "course_id": 271,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T20:52:26.797Z",
    "course_published": true,
    "updated_at": "2016-12-08T20:52:26.793Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e86c8ee0930bab40e3a91fd8be691cc7eeddc5fb52ad40ebb95e75c7e44de0b8"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 40ed21987e5e9592446b4a0a705fe8ce91574551df558e9e62e84cfc6215b5b1
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
    "id": 7,
    "course_id": 270,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-08T20:52:26.674Z",
    "course_published": true,
    "updated_at": "2016-12-08T20:52:26.666Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40ed21987e5e9592446b4a0a705fe8ce91574551df558e9e62e84cfc6215b5b1"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 31360655b4d26bd36e5349f921979fe0194c0cd90634ab2b949ec844a71b3316
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
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 37,
      "user_id": 269
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 38,
      "user_id": 269
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 39,
      "user_id": 269
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 40,
      "user_id": 269
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31360655b4d26bd36e5349f921979fe0194c0cd90634ab2b949ec844a71b3316"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/322
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
    "id": 322,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 322,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 322
      },
      {
        "id": 323,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 322
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/322" -X GET \
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
      "id": 323,
      "name": "Persevering scalable approach",
      "name_translations": {
        "en": "Persevering scalable approach"
      }
    },
    {
      "id": 324,
      "name": "Triple-buffered 24 hour orchestration",
      "name_translations": {
        "en": "Triple-buffered 24 hour orchestration"
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
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer 63a399c1d08a5b4beeb91181be9f0aaf775a5e47e7c34bb2cba99096a48020d8
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
    "id": 27,
    "user_id": 154,
    "feedbackable_id": 11,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-08T20:51:31.432Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63a399c1d08a5b4beeb91181be9f0aaf775a5e47e7c34bb2cba99096a48020d8"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer b1a52214e4c943d038831bba70a3631b26bc01f3d4b48b901c7d915241b19e4d
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
    "id": 22,
    "user_id": 127,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-08T20:51:29.813Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/22/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1a52214e4c943d038831bba70a3631b26bc01f3d4b48b901c7d915241b19e4d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/24
Content-Type: application/json
Authorization: Bearer 68596c6ef63478f0e1bf3bb30368d1c919714ed161a76b2a436cf95da4b023c7
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
    "id": 24,
    "user_id": 137,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T20:51:30.434Z",
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
curl "api.goskive.com/v2/feedbacks/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68596c6ef63478f0e1bf3bb30368d1c919714ed161a76b2a436cf95da4b023c7"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/fix
Content-Type: application/json
Authorization: Bearer f395e6c9b478b4e63e6d429be16bb4591e74aa364436d13fed3959cbff8c598f
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
curl "api.goskive.com/v2/feedbacks/20/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f395e6c9b478b4e63e6d429be16bb4591e74aa364436d13fed3959cbff8c598f"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer d4b240a4e75e0edc4e0416c2aaa63b8525bff214d78aa7113a0b7a0a8556a8fa
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
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4b240a4e75e0edc4e0416c2aaa63b8525bff214d78aa7113a0b7a0a8556a8fa"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/close
Content-Type: application/json
Authorization: Bearer 71575d560dfc52516d3e7ed1708f82b31ded1cb49ff6ab93b7d6ca00ed93fa3c
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
curl "api.goskive.com/v2/feedbacks/28/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71575d560dfc52516d3e7ed1708f82b31ded1cb49ff6ab93b7d6ca00ed93fa3c"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/25
Content-Type: application/json
Authorization: Bearer c83010837dae0d9160707d3f8d8d4c731e49137ec918ad694dbf508763a544b2
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
    "id": 25,
    "user_id": 142,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T20:51:30.858Z",
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
curl "api.goskive.com/v2/feedbacks/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c83010837dae0d9160707d3f8d8d4c731e49137ec918ad694dbf508763a544b2"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer 4fff5773b870be1f1ec2c5ad1dc496c24b172e766592263d90da76e4739c2c7f
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
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fff5773b870be1f1ec2c5ad1dc496c24b172e766592263d90da76e4739c2c7f"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer 4f3b9fdec61eaa2f8768e3baff695b166adcfaaad50877b7c7752bd4a87aa7c6
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f3b9fdec61eaa2f8768e3baff695b166adcfaaad50877b7c7752bd4a87aa7c6"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer 1211843991aecf355b0a37728a6530686ca1fb10a3a614a7614c41a80a0fa33e
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1211843991aecf355b0a37728a6530686ca1fb10a3a614a7614c41a80a0fa33e"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/1
Content-Type: application/json
Authorization: Bearer 6c92061ff19d969049ab8fa2e284715987a517124a5df8893f455cb211289b8a
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/3ccead62c767304621db2873778d6b7c.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T205132Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b2d0210c3cb519cdbe5dde5066323da2f77a4e3916a84393967ef3a07bade07b",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c92061ff19d969049ab8fa2e284715987a517124a5df8893f455cb211289b8a"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/9/preview
Content-Type: application/json
Authorization: Bearer 268f3a57f5a7b5326783f459d3e14d0a104da71f00269bea2a5ab16b7577e640
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/aa18767994bd75b541cbe0331223b43d.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T205133Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=27356fef0d236284022c700235752efdb0312c97cf4ad767a22d13ba8807f0f9",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/9/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 268f3a57f5a7b5326783f459d3e14d0a104da71f00269bea2a5ab16b7577e640"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/4/metadata
Content-Type: application/json
Authorization: Bearer a0c67b0ebaff0c792a44d17f0d53c04ac70a20e779284fe3d6108e25cbb95f1f
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
    "id": 4,
    "uploader": {
      "id": 169,
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
      "created_at": "2016-12-08T20:51:32.781Z",
      "updated_at": "2016-12-08T20:51:32.781Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-08T20:51:32.879Z",
    "updated_at": "2016-12-08T20:51:32.879Z",
    "course_id": 39,
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
curl "api.goskive.com/v2/files/4/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0c67b0ebaff0c792a44d17f0d53c04ac70a20e779284fe3d6108e25cbb95f1f"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/18/matched_courses?required_cu_count=2
Authorization: Bearer 8cf5a95598c3965d9f3154e45e7f4aa5d56773c048851e256767efc8bbf9f97c
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
      "creator_id": 429,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 117,
      "additional_university_ids": [

      ],
      "discipline_id": 124,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T20:51:52.511Z",
      "updated_at": "2016-12-08T20:51:53.962Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 124,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 434,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-d84e7bcb-af25-49f4-8b85-3b9ee4c0fa5f",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-d84e7bcb-af25-49f4-8b85-3b9ee4c0fa5f",
      "slug": "mit-the-great-british-bake-off-d84e7bcb-af25-49f4-8b85-3b9ee4c0fa5f",
      "university_id": 118,
      "additional_university_ids": [

      ],
      "discipline_id": 125,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T20:51:52.511Z",
      "updated_at": "2016-12-08T20:51:54.457Z",
      "shortname": "mit-the-great-british-bake-off-d84e7bcb-af25-49f4-8b85-3b9ee4c0fa5f",
      "topic_id": 125,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/18/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 8cf5a95598c3965d9f3154e45e7f4aa5d56773c048851e256767efc8bbf9f97c"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/10/download
Content-Type: application/json
Authorization: Bearer 832c1a4c6ed39c80ca2cfaa28b36ae17421b6be637617d54bf2ab80a3e67eb26
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 832c1a4c6ed39c80ca2cfaa28b36ae17421b6be637617d54bf2ab80a3e67eb26"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/2/report
Content-Type: application/json
Authorization: Bearer 35f641461ded488ce2c8624eb14ac30bbf5464091dc0ed648ef7a5f6d3cdd5b8
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/2/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35f641461ded488ce2c8624eb14ac30bbf5464091dc0ed648ef7a5f6d3cdd5b8"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer d32c8b719e234f7f9a7b03b537c1b6364f4359693d48d3f601fdd5c5c4623c79
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d32c8b719e234f7f9a7b03b537c1b6364f4359693d48d3f601fdd5c5c4623c79"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/13/upvote
Content-Type: application/json
Authorization: Bearer def55bc67f65aa6b71662d691b85e58012699fdeae11b593833568348659d6c7
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer def55bc67f65aa6b71662d691b85e58012699fdeae11b593833568348659d6c7"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/51/comments
Content-Type: application/json
Authorization: Bearer e0967603d6de30a4a63838616453402aa94ee89fe50f08d1b58b22cf85072533
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
    "id": 45,
    "author_id": 589,
    "reply_to_id": null,
    "created_at": "2016-12-08T20:52:08.786Z",
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
curl "api.goskive.com/v2/flashcards/51/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0967603d6de30a4a63838616453402aa94ee89fe50f08d1b58b22cf85072533"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/53/comments
Content-Type: application/json
Authorization: Bearer 7c4453c94eed6ac47c2a1c32395a6f4ff7b350394b495cc466cc3ecdee18b830
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
    "id": 46,
    "author_id": 595,
    "reply_to_id": null,
    "created_at": "2016-12-08T20:52:09.375Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 595,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:09.372Z",
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
curl "api.goskive.com/v2/flashcards/53/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c4453c94eed6ac47c2a1c32395a6f4ff7b350394b495cc466cc3ecdee18b830"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer c4b53be3a95b905d02dc146a2adcad45f46b3246ba0ab4f16203c6d5f38dbe24
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
      "id": 47,
      "author_id": 604,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:52:09.940Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 605,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:52:09.957Z",
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
curl "api.goskive.com/v2/flashcards/55/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4b53be3a95b905d02dc146a2adcad45f46b3246ba0ab4f16203c6d5f38dbe24"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/52/comments
Content-Type: application/json
Authorization: Bearer ee373cda3944f586ac96a7d19f012d3dd1e06e953aa3c28df9b485aacc1521c7
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
curl "api.goskive.com/v2/flashcards/52/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee373cda3944f586ac96a7d19f012d3dd1e06e953aa3c28df9b485aacc1521c7"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/feedbacks
Content-Type: application/json
Authorization: Bearer 23e531238e0ca3ef18a26697175f07a67a86a416efd984fb1fbc2295f5bf38a0
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
    "id": 39,
    "user_id": 779,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T20:52:24.503Z",
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
curl "api.goskive.com/v2/flashcards/85/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23e531238e0ca3ef18a26697175f07a67a86a416efd984fb1fbc2295f5bf38a0"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/88/feedbacks
Content-Type: application/json
Authorization: Bearer 3c23dd3b77f45a19c328ffe9846a4e859f60ef7ce4755ef4ea77ce9a0dcc5bd5
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
      "id": 43,
      "user_id": 800,
      "feedbackable_id": 88,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:25.320Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 799,
      "feedbackable_id": 88,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:25.310Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/88/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c23dd3b77f45a19c328ffe9846a4e859f60ef7ce4755ef4ea77ce9a0dcc5bd5"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/2/votes
Content-Type: application/json
Authorization: Bearer db4036856e6cb989d8568f99038cff694b89e45a4f36a07f13ed45aaea9ce6ac
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
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 29
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 28
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 27
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db4036856e6cb989d8568f99038cff694b89e45a4f36a07f13ed45aaea9ce6ac"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/57/republish
Content-Type: application/json
Authorization: Bearer e40b52f1d1a220d757e8da42a1a91fe03978b6d2b466aaa1cec65c3180f5322a
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
curl "api.goskive.com/v2/flashcards/57/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e40b52f1d1a220d757e8da42a1a91fe03978b6d2b466aaa1cec65c3180f5322a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/79/bookmark
Content-Type: application/json
Authorization: Bearer d7d75593a9ddb463841b6a7bfba2f036f8c8135d402466bbc274dfd7d92ed65c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/79/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7d75593a9ddb463841b6a7bfba2f036f8c8135d402466bbc274dfd7d92ed65c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/78
Content-Type: application/json
Authorization: Bearer 4a706ee86c815983e53dc9a5f1995afc5b9b4a0e4927b5e02e69f545effbc0ed
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/78" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a706ee86c815983e53dc9a5f1995afc5b9b4a0e4927b5e02e69f545effbc0ed"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/downvote
Content-Type: application/json
Authorization: Bearer f523a950ece79d91e5e48e76ae253f0fa0bf6ff8467adf074cbccba58ddbc01f
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f523a950ece79d91e5e48e76ae253f0fa0bf6ff8467adf074cbccba58ddbc01f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/77
Content-Type: application/json
Authorization: Bearer daf0b3884df6e329593751d74c7ce10255837096b9d4c06252ad3d480f30cd6a
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 714,
    "chapter_id": 137,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:17.752Z",
    "created_at": "2016-12-08T20:52:17.752Z",
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
curl "api.goskive.com/v2/flashcards/77" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daf0b3884df6e329593751d74c7ce10255837096b9d4c06252ad3d480f30cd6a"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/75/report
Content-Type: application/json
Authorization: Bearer 5ea2640cabae0e956d3f9c4bbb2f42efd4999ddc4bd1d1ea0d9249a112d94e48
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ea2640cabae0e956d3f9c4bbb2f42efd4999ddc4bd1d1ea0d9249a112d94e48"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/76/bookmark
Content-Type: application/json
Authorization: Bearer 819753a47092b002fa435ab2a374e5114708d29a244d75ded8c439a91f4f1b65
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 819753a47092b002fa435ab2a374e5114708d29a244d75ded8c439a91f4f1b65"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/58/upvote
Content-Type: application/json
Authorization: Bearer 3e15a20108d35eee0879f47a2314ce28177f5662a1c8670c2bd00089495e20f5
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e15a20108d35eee0879f47a2314ce28177f5662a1c8670c2bd00089495e20f5"
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
    "key": "cache/6b564184dfd1375412228f5553293e2d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQyMTo1MTo0OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzZiNTY0MTg0ZGZkMTM3NTQxMjIyOGY1NTUzMjkzZTJkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDhUMjA1MTQ4WiJ9XX0=",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T205148Z",
    "x-amz-signature": "52cb5e7a3121ab089a1f36c705efa74ffc1b97872018c7da0d36054a83674e68"
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
POST /v2/me/jobs/8/sign_ups
Content-Type: application/json
Authorization: Bearer f426ba090574eee788f76784f59220dc1d1aa8ab7fb304f65a501f43591529a7
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
    "id": 1,
    "email_address": "joe@megacorp.com"
  }
}
```



```shell
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f426ba090574eee788f76784f59220dc1d1aa8ab7fb304f65a501f43591529a7"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer ac16170180c1b0129c3b174a66c46d538bec095b7de70dfcb9abb16f3426eed3
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
curl "api.goskive.com/v2/me/jobs/7/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac16170180c1b0129c3b174a66c46d538bec095b7de70dfcb9abb16f3426eed3"
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
{"password":{"reset_password_token":"uzyawH8mP9w7fszLLeCK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 15,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-08T20:51:21.292Z",
  "updated_at": "2016-12-08T20:51:21.696Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "locale": "en",
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "audit_id": 7113
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"uzyawH8mP9w7fszLLeCK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Content-Type: application/json
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
Content-Type: application/json
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
POST /v2/questions/125/comments
Content-Type: application/json
Authorization: Bearer 73088166bcd4b01d479a9e40d5feef66831fe4c67d439a966f84d4ad1dcfb9d8
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
    "id": 57,
    "author_id": 935,
    "reply_to_id": null,
    "created_at": "2016-12-08T20:52:36.865Z",
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
curl "api.goskive.com/v2/questions/125/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73088166bcd4b01d479a9e40d5feef66831fe4c67d439a966f84d4ad1dcfb9d8"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/124/comments
Content-Type: application/json
Authorization: Bearer ba9641f987833d68d82d15a0a3f36171269c533799a3985480337d4d048c65c0
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
    "id": 56,
    "author_id": 932,
    "reply_to_id": null,
    "created_at": "2016-12-08T20:52:36.408Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 932,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:36.406Z",
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
curl "api.goskive.com/v2/questions/124/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba9641f987833d68d82d15a0a3f36171269c533799a3985480337d4d048c65c0"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/121/comments
Content-Type: application/json
Authorization: Bearer a6e32c93dfbb5a68f868fb8e2f4a5f1ad0a6838c7568e326b8faf20933cd1bea
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
      "id": 54,
      "author_id": 924,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:52:35.457Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 925,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:52:35.472Z",
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
curl "api.goskive.com/v2/questions/121/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6e32c93dfbb5a68f868fb8e2f4a5f1ad0a6838c7568e326b8faf20933cd1bea"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/123/comments
Content-Type: application/json
Authorization: Bearer b3b041af8b4a22e01e616c511ede14cd2461daf18802e4b287c6e314de32bd9c
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
curl "api.goskive.com/v2/questions/123/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3b041af8b4a22e01e616c511ede14cd2461daf18802e4b287c6e314de32bd9c"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/36/feedbacks
Content-Type: application/json
Authorization: Bearer 45897114784912de0725a0b90a53b14c41e75acd45e165684f0585b7bab0d5aa
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
    "id": 36,
    "user_id": 265,
    "feedbackable_id": 36,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-08T20:51:39.702Z",
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
curl "api.goskive.com/v2/questions/36/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45897114784912de0725a0b90a53b14c41e75acd45e165684f0585b7bab0d5aa"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/31/feedbacks
Content-Type: application/json
Authorization: Bearer fa852d4004c04b7396f9507878ae62433fdade02e93eefb177e46ebfdb059a70
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
      "id": 32,
      "user_id": 244,
      "feedbackable_id": 31,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:37.848Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 243,
      "feedbackable_id": 31,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:37.837Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/31/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa852d4004c04b7396f9507878ae62433fdade02e93eefb177e46ebfdb059a70"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/1/votes
Content-Type: application/json
Authorization: Bearer fb0a779ee6c999ae6d81e38dd45a06c1c3a5e2797797a5e116d82f2096280c9a
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 6
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 5
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 4
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/1/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb0a779ee6c999ae6d81e38dd45a06c1c3a5e2797797a5e116d82f2096280c9a"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/97/republish
Content-Type: application/json
Authorization: Bearer dc1f4aa17a238e68120174f263d1c2d98618ed317cfd6c1f043ee7b03209fed3
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
curl "api.goskive.com/v2/questions/97/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc1f4aa17a238e68120174f263d1c2d98618ed317cfd6c1f043ee7b03209fed3"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/104/bookmark
Content-Type: application/json
Authorization: Bearer 5f36ba4cd1e50840704b378dbd0de5376dbb40682c77797ba21416895ddb259a
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/104/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f36ba4cd1e50840704b378dbd0de5376dbb40682c77797ba21416895ddb259a"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/99
Content-Type: application/json
Authorization: Bearer d271bf872e3ed0eed673bfaa7a447bf92c781044be0d0f7c2a2a2b21d2c1b210
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/99" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d271bf872e3ed0eed673bfaa7a447bf92c781044be0d0f7c2a2a2b21d2c1b210"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/120/downvote
Content-Type: application/json
Authorization: Bearer 9d5e0039fdc14a3ebf45ba8e9c2aabf4d6d956c64463ec6bd0bb0829fe7e0cd4
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/120/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d5e0039fdc14a3ebf45ba8e9c2aabf4d6d956c64463ec6bd0bb0829fe7e0cd4"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/103
Content-Type: application/json
Authorization: Bearer 620b4a69cabc9b990d75240b6a7ef5c4dc2d25777e0f4388e45b5ffb16454180
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
    "id": 103,
    "obfuscated_id": "AVhVflMAvL0",
    "author_id": 845,
    "chapter_id": 162,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:29.633Z",
    "created_at": "2016-12-08T20:52:29.554Z",
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
        "id": 206,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 207,
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
curl "api.goskive.com/v2/questions/103" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 620b4a69cabc9b990d75240b6a7ef5c4dc2d25777e0f4388e45b5ffb16454180"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/96/report
Content-Type: application/json
Authorization: Bearer 82561321fb28b6f18a6e52e246258e3cf7f0165ab16503f4782f2397b84dbe6d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/96/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82561321fb28b6f18a6e52e246258e3cf7f0165ab16503f4782f2397b84dbe6d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/101/bookmark
Content-Type: application/json
Authorization: Bearer 207e32b3076d0550f7c355de5e244dc27908486d37263ce4930e8646fbd2ee47
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/101/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 207e32b3076d0550f7c355de5e244dc27908486d37263ce4930e8646fbd2ee47"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/100
Content-Type: application/json
Authorization: Bearer 2b3b0317281d6284f79d68a52e5e2e8819e13c326642f66f47c2ce611c455874
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T20:52:28.470Z","updated_at":"2016-12-08T20:52:28.548Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":159,"author_id":836,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 100,
    "obfuscated_id": "erXmBhoMZFI",
    "author_id": 836,
    "chapter_id": 159,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T20:52:28.630Z",
    "created_at": "2016-12-08T20:52:28.470Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x000000110b0318>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 201,
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
curl "api.goskive.com/v2/questions/100" -d '{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T20:52:28.470Z","updated_at":"2016-12-08T20:52:28.548Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":159,"author_id":836,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b3b0317281d6284f79d68a52e5e2e8819e13c326642f66f47c2ce611c455874"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/102/upvote
Content-Type: application/json
Authorization: Bearer 9c400cd963f9f66a8c99c1738e2a5e4fd5788d338311f1cc10494ae24d6887bc
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/102/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c400cd963f9f66a8c99c1738e2a5e4fd5788d338311f1cc10494ae24d6887bc"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 9d0198e8f2dbcb35b4a9e04b71321c85e34ea5afcc3a846e807d1580091fb279
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
      "creator_id": 382,
      "id": 101,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "discipline_id": 109,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:51:49.140Z",
      "shortname": "mit-pizza-201",
      "topic_id": 109,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Pizza 201",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d0198e8f2dbcb35b4a9e04b71321c85e34ea5afcc3a846e807d1580091fb279"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 5a284cc1cb4cf03a80043519c2224381c300d2a6e7fb85b122939f3a41699445
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
      "id": 103,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-103",
      "html_url": "https://goskive.com/university/uni-103",
      "slug": "uni-103",
      "name": "National School of Pizza",
      "short_name": "Uni 103",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/3114ffbc6565f591d0e2a306f9100cfe.jpg",
      "image_thumb_url": "memory://universities/5cd39f3208306a03d12f3548f363ce98.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T20:51:49.412Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 102,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-102",
      "html_url": "https://goskive.com/university/uni-102",
      "slug": "uni-102",
      "name": "National School of Pastry",
      "short_name": "Uni 102",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/8b65f6394f8d6cc90b7175a74e6dc5f0.jpg",
      "image_thumb_url": "memory://universities/ee7c1df422c8ff5544e747814fe3a3e6.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T20:51:49.365Z",
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
	-H "Authorization: Bearer 5a284cc1cb4cf03a80043519c2224381c300d2a6e7fb85b122939f3a41699445"
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
      "id": 37,
      "name": "Programmable grid-enabled flexibility",
      "name_translations": {
        "en": "Programmable grid-enabled flexibility"
      },
      "discipline_id": 37
    },
    {
      "id": 38,
      "name": "Re-engineered even-keeled open architecture",
      "name_translations": {
        "en": "Re-engineered even-keeled open architecture"
      },
      "discipline_id": 38
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
GET /v2/topics/36
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
    "id": 36,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 36
  }
}
```



```shell
curl "api.goskive.com/v2/topics/36" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer fb93b40c8aded3905aed4b268c81c2652a8bb8f5d868023a840544108c76ac04
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
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-274",
      "html_url": "https://goskive.com/university/uni-274",
      "slug": "uni-274",
      "name": "University 214",
      "short_name": "Uni 274",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/1a8a6137c27a9f26cafe1d00eecefdfa.jpg",
      "image_thumb_url": "memory://universities/50a8e2c3ebe880391db88529a36db2d6.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T20:52:40.572Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 293,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-275",
      "html_url": "https://goskive.com/university/uni-275",
      "slug": "uni-275",
      "name": "University 215",
      "short_name": "Uni 275",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/353e562d3a6aacdbdfe85bac49f72085.jpg",
      "image_thumb_url": "memory://universities/bbff60316dffa5a648e0ed16e3b81942.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T20:52:40.617Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 294,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-276",
      "html_url": "https://goskive.com/university/uni-276",
      "slug": "uni-276",
      "name": "University 216",
      "short_name": "Uni 276",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/5c74c645b382acde88078bec3b9b9889.jpg",
      "image_thumb_url": "memory://universities/06fa5fb1f43a6eb221a605f43f3b9fd6.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T20:52:40.663Z",
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
	-H "Authorization: Bearer fb93b40c8aded3905aed4b268c81c2652a8bb8f5d868023a840544108c76ac04"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 6857787fd8d21dfe9c7f9dbff65d753b18cce18e74a4bbb76c29f25b3d706aab
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
    "id": 296,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/44f0d8f8c6c10efb0f893cd626e1f132.jpg",
    "image_thumb_url": "memory://universities/0e77b9fecb962c17235c7b1591595330.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-08T20:52:40.884Z",
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
	-H "Authorization: Bearer 6857787fd8d21dfe9c7f9dbff65d753b18cce18e74a4bbb76c29f25b3d706aab"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 074272135bcb9555b452656b7fa7fac7e0c3a9bbd068b8b3d554e472f2ebb16b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":230,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 730,
    "id": 220,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 222,
    "additional_university_ids": [

    ],
    "discipline_id": 230,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 3,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T20:52:19.078Z",
    "updated_at": "2016-12-08T20:52:19.218Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 140,
        "updated_at": "2016-12-08T20:52:19.206Z",
        "course_id": 220,
        "author_id": 730,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Etymology of Choux",
        "position": 1
      },
      {
        "id": 141,
        "updated_at": "2016-12-08T20:52:19.222Z",
        "course_id": 220,
        "author_id": 730,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Pastry Making in Medieval France",
        "position": 2
      },
      {
        "id": 142,
        "updated_at": "2016-12-08T20:52:19.236Z",
        "course_id": 220,
        "author_id": 730,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Pastry for Neophytes",
        "position": 3
      }
    ],
    "topic_id": 230,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":230,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 074272135bcb9555b452656b7fa7fac7e0c3a9bbd068b8b3d554e472f2ebb16b"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1d713cb765be32d85c6d9a15af9b91cd31aa070b9faf82c35262b9f4319cac6c
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":231,"published":false}}
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
    "creator_id": 731,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 223,
    "additional_university_ids": [

    ],
    "discipline_id": 231,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-08T20:52:19.451Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 231,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":231,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d713cb765be32d85c6d9a15af9b91cd31aa070b9faf82c35262b9f4319cac6c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f7143a06b6f2e13047ebf7d87f0b26db83628585fc7d48ca409fa9eaf12543f2
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
      "creator_id": 747,
      "id": 236,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-173",
      "html_url": "https://goskive.com/course/fu-course-173",
      "slug": "fu-course-173",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "discipline_id": 246,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:21.009Z",
      "shortname": "fu-course-173",
      "topic_id": 246,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 747,
      "id": 237,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-174",
      "html_url": "https://goskive.com/course/fu-course-174",
      "slug": "fu-course-174",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "discipline_id": 247,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T20:52:20.848Z",
      "updated_at": "2016-12-08T20:52:21.288Z",
      "shortname": "fu-course-174",
      "topic_id": 247,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 174",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7143a06b6f2e13047ebf7d87f0b26db83628585fc7d48ca409fa9eaf12543f2"
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
      "creator_id": 757,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 232,
      "additional_university_ids": [

      ],
      "discipline_id": 254,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:21.949Z",
      "shortname": "fu-course-181",
      "topic_id": 254,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 181",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 757,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 232,
      "additional_university_ids": [

      ],
      "discipline_id": 255,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T20:52:21.772Z",
      "updated_at": "2016-12-08T20:52:22.228Z",
      "shortname": "fu-course-182",
      "topic_id": 255,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 182",
      "organizational_identifier": null,
      "instructor_name": ""
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
Authorization: Bearer 4b8aee9712cfcf01a17d25486adf40d77a69679fc26b1523e1187f901d77e503
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
      "creator_id": 753,
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-177",
      "html_url": "https://goskive.com/course/fu-course-177",
      "slug": "fu-course-177",
      "university_id": 230,
      "additional_university_ids": [

      ],
      "discipline_id": 250,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:21.549Z",
      "shortname": "fu-course-177",
      "topic_id": 250,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 177",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 753,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-178",
      "html_url": "https://goskive.com/course/fu-course-178",
      "slug": "fu-course-178",
      "university_id": 230,
      "additional_university_ids": [

      ],
      "discipline_id": 251,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:21.585Z",
      "shortname": "fu-course-178",
      "topic_id": 251,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 178",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b8aee9712cfcf01a17d25486adf40d77a69679fc26b1523e1187f901d77e503"
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
      "creator_id": 762,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-185",
      "html_url": "https://goskive.com/course/fu-course-185",
      "slug": "fu-course-185",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "discipline_id": 258,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:22.427Z",
      "shortname": "fu-course-185",
      "topic_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 762,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-186",
      "html_url": "https://goskive.com/course/fu-course-186",
      "slug": "fu-course-186",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "discipline_id": 259,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T20:52:22.462Z",
      "shortname": "fu-course-186",
      "topic_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 186",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: "
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer eae02735bc297bdb67a5172453664a9a5ec77c5c4dd3c66f2ef60c70f83fafd5
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
  "id": 727,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-08T20:52:18.588Z",
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
	-H "Authorization: Bearer eae02735bc297bdb67a5172453664a9a5ec77c5c4dd3c66f2ef60c70f83fafd5"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/723
Content-Type: application/json
Authorization: Bearer b5b10c61fa88c49b0f15e96c6c28618edc8cfae95c7f92c5215325bf5e0d6e5b
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
    "id": 723,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 219,
    "fields_of_study": [
      226,
      227
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-08T20:52:18.409Z",
    "updated_at": "2016-12-08T20:52:18.409Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/723" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5b10c61fa88c49b0f15e96c6c28618edc8cfae95c7f92c5215325bf5e0d6e5b"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/725
Content-Type: application/json
Authorization: Bearer 5aa3ad871fb25387c66bb702acebcbbca6fabd989e9fdb5cba43a935d3a77701
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
    "id": 725,
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
    "created_at": "2016-12-08T20:52:18.495Z",
    "updated_at": "2016-12-08T20:52:18.495Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/725" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5aa3ad871fb25387c66bb702acebcbbca6fabd989e9fdb5cba43a935d3a77701"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/15
Content-Type: application/json
Authorization: Bearer 180b841c8bf0ccc16f126d9bf62567fa09e0d66ed2e24d010f6b22d2179eb9d9
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 180b841c8bf0ccc16f126d9bf62567fa09e0d66ed2e24d010f6b22d2179eb9d9"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/16
Content-Type: application/json
Authorization: Bearer 4d3c4750f9caf65c8da5f1ec601d4d8dc8e5f7cbd31247dd530999b2dd208610
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
    "id": 16,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 50,
    "user_id": 405
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d3c4750f9caf65c8da5f1ec601d4d8dc8e5f7cbd31247dd530999b2dd208610"
```
