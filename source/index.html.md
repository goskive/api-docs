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
Authorization: Basic NjU0MGI1OGQ5NmM1MzMzYjUzMGI5Y2Q4ZTYyNjM5MTliMjc4OTk3MjgxNzQw
NjY2Yzg0YjU0MTlkODIzMmM3OTozNGNmNzFiMTAxMDc4MTg1YThlYjY4NTUw
Y2JkZjhjNmM2N2EwMmI3OTQzNzE0NTc4M2I5MjQxOTM5MDcwNTdk

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
	-u 6540b58d96c5333b530b9cd8e6263919b278997281740666c84b5419d8232c79:34cf71b101078185a8eb68550cbdf8c6c67a02b79437145783b924193907057d
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"d0ac093406110466a8386a1f8886980a1cbbd7057e3482a9df047143b71c0fc8","client_secret":"e17aceb2603326f9d41269717d693ad219d3d90492c11110a49a5f61d35945a6"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"d0ac093406110466a8386a1f8886980a1cbbd7057e3482a9df047143b71c0fc8","client_secret":"e17aceb2603326f9d41269717d693ad219d3d90492c11110a49a5f61d35945a6"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MjNmMjM5YjUxMzU0YjczZWFiOWYwM2M4YTk3ODQwMGE2M2ZlMmNkMDA1YTc5
MThlMDkzNmM2YTRkM2RjMzNiMjo1MDM5NWI0YWU2NTdkYjBkNjA0MzZmY2Fl
N2FhNzVlMTZhMzg1Y2I1ODBlNjZmY2ZhY2I5MTI4MDFjNGUzMDgy

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
  "access_token": "5822dc41b90f85e2dec873c4e4a09288346403ac4efd0e1f9ba9dc2c7e02dd95",
  "token_type": "bearer",
  "created_at": 1477428293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 23f239b51354b73eab9f03c8a978400a63fe2cd005a7918e0936c6a4d3dc33b2:50395b4ae657db0d60436fcae7aa75e16a385cb580e66fcfacb912801c4e3082
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cc6c1720937aecbd94762e2d5af6daffeeeebdc0083445216d3073aa33084456","client_secret":"15a38eee36b0b2f3d8ed9f891b391c5e5ca0af54f2b05e8e1490ccde1561ecdf"}
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
  "access_token": "62e0f1a2c3c84d4404253a3f07cfe3c06a942d4e2e82d52ed87b4538de424e31",
  "token_type": "bearer",
  "created_at": 1477428293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cc6c1720937aecbd94762e2d5af6daffeeeebdc0083445216d3073aa33084456","client_secret":"15a38eee36b0b2f3d8ed9f891b391c5e5ca0af54f2b05e8e1490ccde1561ecdf"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"aa9b8fd7a9bba83c7a99173aa1aff9ffd107c80327640c3aa9c454a07a3a690a","client_secret":"71622037c02a5d028008438613925009593204d646f92a3ba1a23cc8b6a033ca"}
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
  "access_token": "85009880a961df72d05939a538fd15651f6624365fef9a5107457ab15e7a7046",
  "token_type": "bearer",
  "created_at": 1477428293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"aa9b8fd7a9bba83c7a99173aa1aff9ffd107c80327640c3aa9c454a07a3a690a","client_secret":"71622037c02a5d028008438613925009593204d646f92a3ba1a23cc8b6a033ca"}' -X POST \
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
Authorization: Bearer 812724483f0a97ade3718e0e64222d58e81b4b0aabf9b3c491048dadf434faff
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
    "company_id": 20,
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
	-H "Authorization: Bearer 812724483f0a97ade3718e0e64222d58e81b4b0aabf9b3c491048dadf434faff"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/17/flashcards
Content-Type: application/json
Authorization: Bearer bd89b3a5121e459886774370cd9681bebcce38bfb3c5944587a7e46b6992928f
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":17,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 1,
    "obfuscated_id": "vnOJWgI0jGc",
    "author_id": 69,
    "chapter_id": 17,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:10.109Z",
    "created_at": "2016-10-25T20:44:10.109Z",
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
curl "api.goskive.com/v2/chapters/17/flashcards" -d '{"flashcard":{"chapter_id":17,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd89b3a5121e459886774370cd9681bebcce38bfb3c5944587a7e46b6992928f"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/19/flashcards
Content-Type: application/json
Authorization: Bearer 70b828fd132ca007e3c0dca25dbac2296ff4f472991a2551c91b41ed9f7b12c9
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
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 73,
      "chapter_id": 19,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:10.379Z",
      "created_at": "2016-10-25T20:44:10.379Z",
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
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 73,
      "chapter_id": 19,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:10.414Z",
      "created_at": "2016-10-25T20:44:10.414Z",
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
      "id": 4,
      "obfuscated_id": "SaV_gL1ycAY",
      "author_id": 73,
      "chapter_id": 19,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:10.448Z",
      "created_at": "2016-10-25T20:44:10.448Z",
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
curl "api.goskive.com/v2/chapters/19/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70b828fd132ca007e3c0dca25dbac2296ff4f472991a2551c91b41ed9f7b12c9"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/54/questions
Content-Type: application/json
Authorization: Bearer bdae14540cd6bc36fe0b6c5ae10969707ce6b0fe733b2eab6dbf68267665ec76
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":54,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 34,
    "obfuscated_id": "LRSQf_NrQzE",
    "author_id": 231,
    "chapter_id": 54,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:21.920Z",
    "created_at": "2016-10-25T20:44:21.920Z",
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
        "id": 68,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 69,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 70,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 71,
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
curl "api.goskive.com/v2/chapters/54/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":54,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdae14540cd6bc36fe0b6c5ae10969707ce6b0fe733b2eab6dbf68267665ec76"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/51/questions
Content-Type: application/json
Authorization: Bearer 7cd756b0080cac2b53f5451758eae9874b5499a793d416e557ffd5613c392136
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":51,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 222,
    "chapter_id": 51,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:20.853Z",
    "created_at": "2016-10-25T20:44:20.853Z",
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
        "id": 61,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 62,
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
curl "api.goskive.com/v2/chapters/51/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":51,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cd756b0080cac2b53f5451758eae9874b5499a793d416e557ffd5613c392136"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/52/questions
Content-Type: application/json
Authorization: Bearer 93ad6f75213343d3f22187bdd361a5fa92e92fc53e6859af5803693e576ca88c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":52,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 225,
    "chapter_id": 52,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:21.189Z",
    "created_at": "2016-10-25T20:44:21.189Z",
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
        "id": 63,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 64,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/52/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":52,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93ad6f75213343d3f22187bdd361a5fa92e92fc53e6859af5803693e576ca88c"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/53/questions
Content-Type: application/json
Authorization: Bearer a0a674e8215f36cc9657021ba080268226f27daf45faeac21b828236432c8c33
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":53,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 33,
    "obfuscated_id": "sjAD-GXxS8o",
    "author_id": 228,
    "chapter_id": 53,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:21.513Z",
    "created_at": "2016-10-25T20:44:21.513Z",
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
        "id": 65,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 66,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 67,
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
curl "api.goskive.com/v2/chapters/53/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":53,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0a674e8215f36cc9657021ba080268226f27daf45faeac21b828236432c8c33"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/56/questions
Content-Type: application/json
Authorization: Bearer 3c68538cfbde0bfd55918ac6f3029547c93bf957bc7a07082d2fa30737ad0814
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
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 237,
      "chapter_id": 56,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:22.693Z",
      "created_at": "2016-10-25T20:44:22.542Z",
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
          "id": 72,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 73,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 238,
      "chapter_id": 56,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:22.938Z",
      "created_at": "2016-10-25T20:44:22.783Z",
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
          "id": 74,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 75,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 37,
      "obfuscated_id": "95m_4XdR9PU",
      "author_id": 239,
      "chapter_id": 56,
      "position": 33,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:44:23.169Z",
      "created_at": "2016-10-25T20:44:23.032Z",
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
          "id": 76,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 77,
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
curl "api.goskive.com/v2/chapters/56/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c68538cfbde0bfd55918ac6f3029547c93bf957bc7a07082d2fa30737ad0814"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/106
Content-Type: application/json
Authorization: Bearer 452856403825c35d0f43e4cfd3f7b7df77f42f5a4f2fe22b2be56fcf98a59218
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
curl "api.goskive.com/v2/chapters/106" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 452856403825c35d0f43e4cfd3f7b7df77f42f5a4f2fe22b2be56fcf98a59218"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/108
Content-Type: application/json
Authorization: Bearer 72070be462ef4601de33aa64169dd06d9a8fd7f2d23107f96723ce8ed16a53a2
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
curl "api.goskive.com/v2/chapters/108" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72070be462ef4601de33aa64169dd06d9a8fd7f2d23107f96723ce8ed16a53a2"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/109
Content-Type: application/json
Authorization: Bearer 47a429392c18feb294ec56658f48421b922d78dd95c8b65f9fcb8836a25f8b67
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
curl "api.goskive.com/v2/chapters/109" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47a429392c18feb294ec56658f48421b922d78dd95c8b65f9fcb8836a25f8b67"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/107
Content-Type: application/json
Authorization: Bearer 5b196e8921be246fe4624cd484c1ea92b984144b39276cee52d7b59edfa49cbf
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/107" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b196e8921be246fe4624cd484c1ea92b984144b39276cee52d7b59edfa49cbf"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/103
Content-Type: application/json
Authorization: Bearer 808378a0877c966128c3c06652eb4648dc9413ed042d8250199adccdcd617c48
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
    "id": 103,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T20:44:40.409Z",
    "course_id": 118,
    "author_id": 452,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-25T20:44:39.742Z",
    "questions_updated_at": "2016-10-25T20:44:39.742Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 456,
        "chapter_id": 103,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:40.386Z",
        "created_at": "2016-10-25T20:44:40.386Z",
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
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 454,
        "chapter_id": 103,
        "position": 63,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:40.245Z",
        "created_at": "2016-10-25T20:44:40.085Z",
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
            "id": 136,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 137,
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
curl "api.goskive.com/v2/chapters/103" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 808378a0877c966128c3c06652eb4648dc9413ed042d8250199adccdcd617c48"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/110
Content-Type: application/json
Authorization: Bearer 8e0002ad6b980852148385938f64fd70f4709f999d01a7f4d4231a1d04c170c5
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
    "id": 110,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T20:44:42.548Z",
    "course_id": 125,
    "author_id": 481,
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
curl "api.goskive.com/v2/chapters/110" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e0002ad6b980852148385938f64fd70f4709f999d01a7f4d4231a1d04c170c5"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/4/replies
Content-Type: application/json
Authorization: Bearer cd47322d7a010ccdfd4732821e29d85982a80eda304c501ad0cb9e1a6dcd333d
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
    "id": 5,
    "author_id": 46,
    "reply_to_id": 4,
    "created_at": "2016-10-25T20:44:07.550Z",
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
curl "api.goskive.com/v2/comments/4/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd47322d7a010ccdfd4732821e29d85982a80eda304c501ad0cb9e1a6dcd333d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 4b2217a2d746213b2c13de7c46b18510872ae631bb9112ee389a1a887c5cd157
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
	-H "Authorization: Bearer 4b2217a2d746213b2c13de7c46b18510872ae631bb9112ee389a1a887c5cd157"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/20
Content-Type: application/json
Authorization: Bearer bad096c4d741a4650bd50e24ade31b2109dbde671209f7c303d7876b6380a465
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
curl "api.goskive.com/v2/comments/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bad096c4d741a4650bd50e24ade31b2109dbde671209f7c303d7876b6380a465"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/23/republish
Content-Type: application/json
Authorization: Bearer e40da25b4ddd4aeda647c2285815eccae834e5d525a24cdf0fe27d428b9e926a
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
curl "api.goskive.com/v2/comments/23/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e40da25b4ddd4aeda647c2285815eccae834e5d525a24cdf0fe27d428b9e926a"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer f97176dfd97bd6caa427ad9e3df974aafbea62aaf25475cd9a9583e911d8979c
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f97176dfd97bd6caa427ad9e3df974aafbea62aaf25475cd9a9583e911d8979c"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 9c2fcde630909bdadbbdcfe9fa40a31d490fc4341d9a8cf151b18f2a768b5747
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c2fcde630909bdadbbdcfe9fa40a31d490fc4341d9a8cf151b18f2a768b5747"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/16
Content-Type: application/json
Authorization: Bearer d128a03843210c757edddaa053004a729d0af3607ba784d16dd361aa62d7364b
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
    "updated_at": "2016-10-25T20:44:19.663Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d128a03843210c757edddaa053004a729d0af3607ba784d16dd361aa62d7364b"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 662a5bb098b1c259db102b7b04dd15601b00fd2322a9745e5cd9caa5b7d71d31
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
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:44:19.762Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:44:19.766Z"
    },
    {
      "id": 19,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:44:19.769Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 662a5bb098b1c259db102b7b04dd15601b00fd2322a9745e5cd9caa5b7d71d31"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer 4d0716bd842a434e9d8e0dd0be35a720bf0bbf34dc02152d6ea71abac98b219a
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d0716bd842a434e9d8e0dd0be35a720bf0bbf34dc02152d6ea71abac98b219a"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer f63d391821c2d7fbecdb70509a4c1099d8d97d28ff70fe6d8d1deecd6383e1d1
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f63d391821c2d7fbecdb70509a4c1099d8d97d28ff70fe6d8d1deecd6383e1d1"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 44c35d148097b0327d8824b79c9021d6adeeec51f071a91c635e796293fcaab1
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
	-H "Authorization: Bearer 44c35d148097b0327d8824b79c9021d6adeeec51f071a91c635e796293fcaab1"
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
Authorization: Bearer a1f686c4e2ef4947c9e0a883f8b7d1ac650e97d6cd2a50473fd812bde147d20e
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
	-H "Authorization: Bearer a1f686c4e2ef4947c9e0a883f8b7d1ac650e97d6cd2a50473fd812bde147d20e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer db1f66ce9188e6992528c77ca0102420a623d95013896805c708437399aa9652
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
    "id": 43,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:44:14.836Z",
    "course_id": 44,
    "author_id": 149,
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
	-H "Authorization: Bearer db1f66ce9188e6992528c77ca0102420a623d95013896805c708437399aa9652"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 09fba40af2bc6b25026a744233740446934b58e3ddcb331be48a1ea2dccc0c2a
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
      "id": 20,
      "title": "Clever Chapter Title 17",
      "position": 1,
      "updated_at": "2016-10-25T20:44:12.208Z",
      "course_id": 30,
      "author_id": 97,
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
      "position": 2,
      "updated_at": "2016-10-25T20:44:12.231Z",
      "course_id": 30,
      "author_id": 98,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 22,
      "title": "Clever Chapter Title 19",
      "position": 3,
      "updated_at": "2016-10-25T20:44:12.471Z",
      "course_id": 30,
      "author_id": 99,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T20:44:12.140Z",
      "questions_updated_at": "2016-10-25T20:44:12.140Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09fba40af2bc6b25026a744233740446934b58e3ddcb331be48a1ea2dccc0c2a"
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
      "id": 32,
      "title": "Clever Chapter Title 29",
      "position": 1,
      "updated_at": "2016-10-25T20:44:13.621Z",
      "course_id": 36,
      "author_id": 125,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 33,
      "title": "Clever Chapter Title 30",
      "position": 2,
      "updated_at": "2016-10-25T20:44:13.644Z",
      "course_id": 36,
      "author_id": 126,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 34,
      "title": "Clever Chapter Title 31",
      "position": 3,
      "updated_at": "2016-10-25T20:44:13.885Z",
      "course_id": 36,
      "author_id": 127,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T20:44:13.547Z",
      "questions_updated_at": "2016-10-25T20:44:13.547Z",
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
Authorization: Bearer ce974934956cf429ba8983579cb2ac0a7548bf2e4428d5c1331f4062957553c6
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
      "id": 23,
      "title": "Clever Chapter Title 20",
      "position": 1,
      "updated_at": "2016-10-25T20:44:12.745Z",
      "course_id": 32,
      "author_id": 106,
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
      "position": 2,
      "updated_at": "2016-10-25T20:44:12.770Z",
      "course_id": 32,
      "author_id": 107,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 25,
      "title": "Clever Chapter Title 22",
      "position": 3,
      "updated_at": "2016-10-25T20:44:12.795Z",
      "course_id": 32,
      "author_id": 108,
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
	-H "Authorization: Bearer ce974934956cf429ba8983579cb2ac0a7548bf2e4428d5c1331f4062957553c6"
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
      "id": 35,
      "title": "Clever Chapter Title 32",
      "position": 1,
      "updated_at": "2016-10-25T20:44:14.061Z",
      "course_id": 38,
      "author_id": 132,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 36,
      "title": "Clever Chapter Title 33",
      "position": 2,
      "updated_at": "2016-10-25T20:44:14.083Z",
      "course_id": 38,
      "author_id": 133,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 37,
      "title": "Clever Chapter Title 34",
      "position": 3,
      "updated_at": "2016-10-25T20:44:14.105Z",
      "course_id": 38,
      "author_id": 134,
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
Authorization: Bearer 88c2b9fd5e66094f110ef2a68ca4e31a61129f9e96264f7c0041bb486a197058
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
    "course_id": 58,
    "user_id": 204,
    "updated_at": "2016-10-25T20:44:19.535Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88c2b9fd5e66094f110ef2a68ca4e31a61129f9e96264f7c0041bb486a197058"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer b57302ee1fe6e67e66bb12b3ba8e2757a72b1c174d238e0009a0fb08689c06de
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
      "course_id": 54,
      "user_id": 192,
      "updated_at": "2016-10-25T20:44:18.985Z"
    },
    {
      "id": 2,
      "course_id": 54,
      "user_id": 193,
      "updated_at": "2016-10-25T20:44:18.999Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b57302ee1fe6e67e66bb12b3ba8e2757a72b1c174d238e0009a0fb08689c06de"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/293/files
Content-Type: application/json
Authorization: Bearer 2fbb8ada51bca4695af7812f5a2ec9ddcf605564d870ac0711ef54b7fd90a83c
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
      "id": 3,
      "uploader": {
        "id": 918,
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
        "created_at": "2016-10-25T20:45:17.508Z",
        "updated_at": "2016-10-25T20:45:17.508Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:45:17.519Z",
      "updated_at": "2016-10-25T20:45:17.519Z",
      "course_id": 293,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 919,
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
        "created_at": "2016-10-25T20:45:17.527Z",
        "updated_at": "2016-10-25T20:45:17.527Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:45:17.536Z",
      "updated_at": "2016-10-25T20:45:17.536Z",
      "course_id": 293,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 920,
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
        "created_at": "2016-10-25T20:45:17.544Z",
        "updated_at": "2016-10-25T20:45:17.544Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:45:17.554Z",
      "updated_at": "2016-10-25T20:45:17.554Z",
      "course_id": 293,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/293/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2fbb8ada51bca4695af7812f5a2ec9ddcf605564d870ac0711ef54b7fd90a83c"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/295/files
Content-Type: application/json
Authorization: Bearer 76c2f35955b03ebe39f3a863da7126cce4464c314cb17035183a773a1ea7094e
```

`POST /v2/courses/:course_id/files`

#### Parameters


```json
{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}
```


| Name | Description |
|:-----|:------------|
| file[category]  | Category: summary|assignment|exam|other |
| file[filename]  | Filename |
| file[file_url]  | URL to the file in cache on S3 |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "file": {
    "id": 6,
    "uploader": {
      "id": 925,
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
      "created_at": "2016-10-25T20:45:17.800Z",
      "updated_at": "2016-10-25T20:45:17.800Z"
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
    "created_at": "2016-10-25T20:45:17.828Z",
    "updated_at": "2016-10-25T20:45:17.828Z",
    "course_id": 295,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/295/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76c2f35955b03ebe39f3a863da7126cce4464c314cb17035183a773a1ea7094e"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/296/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 0a90f7e900dfad0a3118e715408ee364e2aa753530d10de955be13fa56853c7c
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
    "key": "cache/21c6417f63084fdc8f3fae72626c6747.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQyMTo0NToxOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzIxYzY0MTdmNjMwODRmZGM4ZjNmYWU3MjYyNmM2NzQ3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI1VDIwNDUxOFoifV19",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T204518Z",
    "x-amz-signature": "5c5e32566f8d5c4b3f286c1685fd72561f1c19ac152c037c713c4f9857b4f2bf"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/296/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a90f7e900dfad0a3118e715408ee364e2aa753530d10de955be13fa56853c7c"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 3f3a3841bce277d8187eff46dcb11e04e4baf1c687e8fdfc02f88ed9324be2ba
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
	-H "Authorization: Bearer 3f3a3841bce277d8187eff46dcb11e04e4baf1c687e8fdfc02f88ed9324be2ba"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 96548bd2bda98a0289a21d6c0f14a3f0f451177a297525b31bde5398723ce68b
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
	-H "Authorization: Bearer 96548bd2bda98a0289a21d6c0f14a3f0f451177a297525b31bde5398723ce68b"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f9b56f9d1de1d34fff00ad522fab97a05395acc1dd8f0cdc70f0a24c755ae077
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
	-H "Authorization: Bearer f9b56f9d1de1d34fff00ad522fab97a05395acc1dd8f0cdc70f0a24c755ae077"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0d7ed152cf915ebe6db7256950e7595c9f3f8b2a969197352b715af0610570d1
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
	-H "Authorization: Bearer 0d7ed152cf915ebe6db7256950e7595c9f3f8b2a969197352b715af0610570d1"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3bf45f1c1c33a1bfb180f2f186e686d5b1bfdc6a00b7d68b29f00ab8c9c46c62
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
	-H "Authorization: Bearer 3bf45f1c1c33a1bfb180f2f186e686d5b1bfdc6a00b7d68b29f00ab8c9c46c62"
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
    "creator_id": 710,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 200,
    "additional_university_ids": [

    ],
    "topic_id": 233,
    "discipline_id": 234,
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
    "chapters_updated_at": "2016-10-25T20:44:59.301Z",
    "updated_at": "2016-10-25T20:45:00.696Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 162,
        "title": "Clever Chapter Title 138",
        "position": 1,
        "updated_at": "2016-10-25T20:45:00.651Z",
        "course_id": 221,
        "author_id": 710,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:44:59.301Z",
        "questions_updated_at": "2016-10-25T20:44:59.301Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 163,
        "title": "Clever Chapter Title 139",
        "position": 2,
        "updated_at": "2016-10-25T20:45:00.689Z",
        "course_id": 221,
        "author_id": 710,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:44:59.301Z",
        "questions_updated_at": "2016-10-25T20:44:59.301Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 710,
        "chapter_id": 162,
        "position": 85,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:59.507Z",
        "created_at": "2016-10-25T20:44:59.394Z",
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
            "id": 180,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 181,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 710,
        "chapter_id": 163,
        "position": 87,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:44:59.883Z",
        "created_at": "2016-10-25T20:44:59.769Z",
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
            "id": 184,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 185,
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
Authorization: Bearer 25eacc2604cda1554702983e52edfa43baeb24277c7c7309245ffdae9286f686
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
    "creator_id": 715,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 201,
    "additional_university_ids": [

    ],
    "topic_id": 234,
    "discipline_id": 235,
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
    "chapters_updated_at": "2016-10-25T20:45:00.752Z",
    "updated_at": "2016-10-25T20:45:02.130Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 164,
        "title": "Clever Chapter Title 140",
        "position": 1,
        "updated_at": "2016-10-25T20:45:02.087Z",
        "course_id": 222,
        "author_id": 715,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:45:00.752Z",
        "questions_updated_at": "2016-10-25T20:45:00.752Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 165,
        "title": "Clever Chapter Title 141",
        "position": 2,
        "updated_at": "2016-10-25T20:45:02.123Z",
        "course_id": 222,
        "author_id": 715,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:45:00.752Z",
        "questions_updated_at": "2016-10-25T20:45:00.752Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 716,
        "chapter_id": 164,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:01.939Z",
        "created_at": "2016-10-25T20:45:01.939Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 716,
        "chapter_id": 165,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:02.003Z",
        "created_at": "2016-10-25T20:45:02.003Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 716,
        "chapter_id": 164,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:01.975Z",
        "created_at": "2016-10-25T20:45:01.975Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 716,
        "chapter_id": 165,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:02.040Z",
        "created_at": "2016-10-25T20:45:02.040Z",
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
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 716,
        "chapter_id": 164,
        "position": 91,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:00.961Z",
        "created_at": "2016-10-25T20:45:00.851Z",
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
            "id": 192,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 193,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 716,
        "chapter_id": 164,
        "position": 92,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:01.131Z",
        "created_at": "2016-10-25T20:45:01.022Z",
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
            "id": 194,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 195,
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
        "author_id": 716,
        "chapter_id": 165,
        "position": 93,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:01.331Z",
        "created_at": "2016-10-25T20:45:01.215Z",
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
            "id": 196,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 197,
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
        "author_id": 716,
        "chapter_id": 165,
        "position": 94,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:45:01.507Z",
        "created_at": "2016-10-25T20:45:01.395Z",
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
            "id": 198,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 199,
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
	-H "Authorization: Bearer 25eacc2604cda1554702983e52edfa43baeb24277c7c7309245ffdae9286f686"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/205/pin
Content-Type: application/json
Authorization: Bearer 301082b4865900f0a9959de00532af0afc9a44433ce0c2a6738f38f659908e14
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/205/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 301082b4865900f0a9959de00532af0afc9a44433ce0c2a6738f38f659908e14"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/210/pin
Content-Type: application/json
Authorization: Bearer 03b0eba2adc096da545f85ee6d8bb8febbe63e17c9a2cd6129f8c9cc8315cbe2
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/210/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03b0eba2adc096da545f85ee6d8bb8febbe63e17c9a2cd6129f8c9cc8315cbe2"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9fbc0c77ca576b446ce95dc6388782fbba8c91ba8258155c6a2c756bbb875cf6
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
    "creator_id": 681,
    "id": 209,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 188,
    "additional_university_ids": [

    ],
    "topic_id": 221,
    "discipline_id": 222,
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
    "updated_at": "2016-10-25T20:44:56.217Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9fbc0c77ca576b446ce95dc6388782fbba8c91ba8258155c6a2c756bbb875cf6"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 6f4efeb5b184d7fac9e80ebd70f02867c7a9870baa848123f525586015bd7a57
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
    "id": 219,
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
    "created_at": "2016-10-25T20:44:20.687Z",
    "updated_at": "2016-10-25T20:44:20.687Z",
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
	-H "Authorization: Bearer 6f4efeb5b184d7fac9e80ebd70f02867c7a9870baa848123f525586015bd7a57"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f219cc5de27231925e1d8ffbaf193055f5e9652e509900722c76007e80cff9d7
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[67]}
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
    "id": 214,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      67
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:44:20.104Z",
    "updated_at": "2016-10-25T20:44:20.160Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[67]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f219cc5de27231925e1d8ffbaf193055f5e9652e509900722c76007e80cff9d7"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0b1159d0f4df6fc09832888eb3b415b2e2c3aa9b434bb620eae7251e313c31c8
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
    "id": 216,
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
    "created_at": "2016-10-25T20:44:20.255Z",
    "updated_at": "2016-10-25T20:44:20.255Z",
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
	-H "Authorization: Bearer 0b1159d0f4df6fc09832888eb3b415b2e2c3aa9b434bb620eae7251e313c31c8"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7d492f58fd7c47360b8eb8a69c633792e3779edb57703f984390dcc96d4743d8
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[70]}
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
    "id": 217,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      70
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:44:20.343Z",
    "updated_at": "2016-10-25T20:44:20.343Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[70]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d492f58fd7c47360b8eb8a69c633792e3779edb57703f984390dcc96d4743d8"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 4cdaaa9f7edd1e82875470b1f389844b9b0c9bcf48931281a90532f25f574ea0
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
    "id": 218,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/b26c80f26bbbdab08d2509e919fd2ce1b4a65d6d.jpg",
    "university_id": null,
    "fields_of_study": [
      71
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:44:20.408Z",
    "updated_at": "2016-10-25T20:44:20.660Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/7dd16af6cdd72cb9a97de3f84e0254db8c9fc523.jpg",
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

71
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 4cdaaa9f7edd1e82875470b1f389844b9b0c9bcf48931281a90532f25f574ea0"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer b3a9d18c2dc1dfc3725a5c51393820a50b741e1efbb89d77f750f3f00d5b8538
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
      "bookmarkable_id": 132,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 133,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 134,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3a9d18c2dc1dfc3725a5c51393820a50b741e1efbb89d77f750f3f00d5b8538"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 26c79ac616f1ff98ddaffa5cfb89df0eea8bfe7cf5ae9e3012854014e5ccc278
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
      "id": 11,
      "title": "Campaign 10",
      "company_id": 25,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 11,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
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
      "id": 12,
      "title": "Campaign 11",
      "company_id": 26,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 12,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/cb7b53bc0db79f6fdb32fcfb3676296e2cab7797.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/bb9fd408e2885991a5d2cf387f2db8486bd6688a.png",
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
	-H "Authorization: Bearer 26c79ac616f1ff98ddaffa5cfb89df0eea8bfe7cf5ae9e3012854014e5ccc278"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a0bcb775ac2e23f7b53feb06c1298e2f56f0f4d47433f1827769a6d8815d64ef
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
      "company_id": 21,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 10,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
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
	-H "Authorization: Bearer a0bcb775ac2e23f7b53feb06c1298e2f56f0f4d47433f1827769a6d8815d64ef"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 376b9d52ecc90f6f6c82a9c3e8457a55e6f22b92cb2b75752141ab606bd9b8b0
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
      "creator_id": 211,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-26",
      "html_url": "https://goskive.com/course/mit-course-26",
      "slug": "mit-course-26",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 65,
      "discipline_id": 66,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 26",
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
      "updated_at": "2016-10-25T20:44:19.893Z",
      "shortname": "mit-course-26"
    },
    {
      "creator_id": 212,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-27",
      "html_url": "https://goskive.com/course/mit-course-27",
      "slug": "mit-course-27",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "topic_id": 66,
      "discipline_id": 67,
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
      "updated_at": "2016-10-25T20:44:19.989Z",
      "shortname": "mit-course-27"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 376b9d52ecc90f6f6c82a9c3e8457a55e6f22b92cb2b75752141ab606bd9b8b0"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer d4df616db19b455599a04ae01b35f21e25d272a3a2943f93d463fb7d1318697e
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
        "updated_at": "2016-10-25T20:45:17.290Z"
      },
      "created_at": "2016-10-25T20:45:17.294Z",
      "updated_at": "2016-10-25T20:45:17.294Z",
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
        "updated_at": "2016-10-25T20:45:17.302Z"
      },
      "created_at": "2016-10-25T20:45:17.305Z",
      "updated_at": "2016-10-25T20:45:17.305Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4df616db19b455599a04ae01b35f21e25d272a3a2943f93d463fb7d1318697e"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer ea0514902f9ebfee290aa17ff1b690072d9eca59e31c68dde3eff22f9d0d96c8
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
        "updated_at": "2016-10-25T20:45:17.119Z"
      },
      "created_at": "2016-10-25T20:45:17.122Z",
      "updated_at": "2016-10-25T20:45:17.122Z",
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
        "updated_at": "2016-10-25T20:45:17.136Z"
      },
      "created_at": "2016-10-25T20:45:17.139Z",
      "updated_at": "2016-10-25T20:45:17.139Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea0514902f9ebfee290aa17ff1b690072d9eca59e31c68dde3eff22f9d0d96c8"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 469537ef186b9d32fbee2978477a10bb70677bc213a620dc3cb475a5cccaca36
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
      "id": 7,
      "created_at": "2016-10-25T20:44:24.853Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 10,
      "updated_at": "2016-10-25T20:44:24.951Z",
      "author_id": "256",
      "thread_subject_id": "71",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 8,
      "created_at": "2016-10-25T20:44:24.941Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 11,
      "updated_at": "2016-10-25T20:44:24.954Z",
      "author_id": "259",
      "thread_subject_id": "72",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 9,
      "created_at": "2016-10-25T20:44:25.363Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-10-25T20:44:25.363Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-10-25T20:44:25.804Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-10-25T20:44:25.804Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 11,
      "created_at": "2016-10-25T20:44:26.206Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-10-25T20:44:26.206Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 12,
      "created_at": "2016-10-25T20:44:26.525Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 44,
      "updated_at": "2016-10-25T20:44:26.525Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 13,
      "created_at": "2016-10-25T20:44:26.841Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 45,
      "updated_at": "2016-10-25T20:44:26.841Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-10-25T20:44:27.154Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 46,
      "updated_at": "2016-10-25T20:44:27.154Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 469537ef186b9d32fbee2978477a10bb70677bc213a620dc3cb475a5cccaca36"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/15
Content-Type: application/json
Authorization: Bearer ffe40dccf787e2c53621527b5d6368e8bcc8c1ab552c8583738737380e015ee8
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-25T20:34:27.000Z"}}
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
    "created_at": "2016-10-25T20:44:27.301Z",
    "read_at": "2016-10-25T20:34:27.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 12,
    "updated_at": "2016-10-25T20:44:27.338Z",
    "author_id": "284",
    "thread_subject_id": "79",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/15" -d '{"notification":{"read_at":"2016-10-25T20:34:27.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffe40dccf787e2c53621527b5d6368e8bcc8c1ab552c8583738737380e015ee8"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer a03b02f3424502549a1040c513efdac9dafcd37cc72acbb8c1c8e93d735589ef
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
      "id": 2,
      "course_id": 21,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T20:44:10.756Z",
      "course_published": true,
      "updated_at": "2016-10-25T20:44:10.749Z"
    },
    {
      "id": 3,
      "course_id": 22,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T20:44:10.831Z",
      "course_published": true,
      "updated_at": "2016-10-25T20:44:10.824Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a03b02f3424502549a1040c513efdac9dafcd37cc72acbb8c1c8e93d735589ef"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer 8a847109b34444162a8556fd97201010e1b2c53a167e6714809d6d02b5e387ad
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
    "id": 1,
    "course_id": 20,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T20:44:10.617Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:44:10.609Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a847109b34444162a8556fd97201010e1b2c53a167e6714809d6d02b5e387ad"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 4b5eb51826e31a989ce750031a1086d5b24d5eeddfb2dee2317d53e8e3278328
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
    "course_id": 25,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-25T20:44:11.211Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:44:11.201Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b5eb51826e31a989ce750031a1086d5b24d5eeddfb2dee2317d53e8e3278328"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 5fdf1c05e531d6a6ad9633ebf0e537e89c9d9476f88f6c6fe68242a464fb3daf
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
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 77,
      "user_id": 656
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 78,
      "user_id": 656
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 656
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 80,
      "user_id": 656
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fdf1c05e531d6a6ad9633ebf0e537e89c9d9476f88f6c6fe68242a464fb3daf"
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
        "id": 26,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 28
      },
      {
        "id": 27,
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
      "id": 26,
      "name": "Switchable client-server functionalities",
      "name_translations": {
        "en": "Switchable client-server functionalities"
      }
    },
    {
      "id": 27,
      "name": "Devolved scalable forecast",
      "name_translations": {
        "en": "Devolved scalable forecast"
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
PATCH /v2/feedbacks/14/close
Content-Type: application/json
Authorization: Bearer 4fa5336c93d55cbfe86e6e42518dff53b12ea31eaabab5049b3e856f02d24fb5
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
    "id": 14,
    "user_id": 316,
    "feedbackable_id": 17,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-25T20:44:29.031Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/14/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fa5336c93d55cbfe86e6e42518dff53b12ea31eaabab5049b3e856f02d24fb5"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer 8d6c50fe41ccd617ae0520a76d400840397f1f4b3ab056fe868bf44371d02d04
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
    "id": 12,
    "user_id": 306,
    "feedbackable_id": 15,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-25T20:44:28.453Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d6c50fe41ccd617ae0520a76d400840397f1f4b3ab056fe868bf44371d02d04"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/17
Content-Type: application/json
Authorization: Bearer 4f3eb38b2f2c13b1e3c8dff0f3bdcb1be066fec9a1eafd3c3abea63c95772d2a
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
    "id": 17,
    "user_id": 331,
    "feedbackable_id": 20,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:44:29.865Z",
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
curl "api.goskive.com/v2/feedbacks/17" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f3eb38b2f2c13b1e3c8dff0f3bdcb1be066fec9a1eafd3c3abea63c95772d2a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/10/fix
Content-Type: application/json
Authorization: Bearer 0604b0d493472967aae3c389c29232d066325bb1ea479c4dd74e8b2fd5b6b345
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
curl "api.goskive.com/v2/feedbacks/10/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0604b0d493472967aae3c389c29232d066325bb1ea479c4dd74e8b2fd5b6b345"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/fix
Content-Type: application/json
Authorization: Bearer a4315871605cbdceae4de95662b2e522b816684e4369f1a490105f289e72f1a5
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
curl "api.goskive.com/v2/feedbacks/13/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4315871605cbdceae4de95662b2e522b816684e4369f1a490105f289e72f1a5"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/close
Content-Type: application/json
Authorization: Bearer 37774bb6e55c95561a4ae4c4f64044ca96154f4e012ce58f0e75599b584f6d01
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
curl "api.goskive.com/v2/feedbacks/16/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37774bb6e55c95561a4ae4c4f64044ca96154f4e012ce58f0e75599b584f6d01"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/18
Content-Type: application/json
Authorization: Bearer 486b4f36e8acada0266645ccbb1415b4c55dc640e76aaddc954e7e40f1e407e0
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
    "id": 18,
    "user_id": 336,
    "feedbackable_id": 21,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:44:30.153Z",
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
curl "api.goskive.com/v2/feedbacks/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 486b4f36e8acada0266645ccbb1415b4c55dc640e76aaddc954e7e40f1e407e0"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 665d3db2b67d578d1924a6132c4512950382b4b69c03cdd739b8e1d88f97a7e0
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
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 665d3db2b67d578d1924a6132c4512950382b4b69c03cdd739b8e1d88f97a7e0"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 11db34859636a0914b683bd448099c00f0423eedf8721cb7c8ddf3e6358a7b49
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11db34859636a0914b683bd448099c00f0423eedf8721cb7c8ddf3e6358a7b49"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/15
Content-Type: application/json
Authorization: Bearer 2ca1a18a79df65532a5a23a9348d96cded00e64af8967fabb64c77248e866353
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/7c2e5df6a264bff20ad3c82bd6236d7f.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T204519Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e4cf95cb14b0a72dfd64e347b499118adb42f0381fcaf6a7b19ea95bcf191920",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ca1a18a79df65532a5a23a9348d96cded00e64af8967fabb64c77248e866353"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer d2a5544c0ced54665b0ed8b8f961fd044842bb4c0913a0de5f8606524a43d008
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/41228199d1bb5fec8b1ed77ecaedeac5.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T204519Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8b24986deb7eb734d51a56ff9178214b61ed43f3f9bde108fe8c4c23b18d88b1",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/14/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2a5544c0ced54665b0ed8b8f961fd044842bb4c0913a0de5f8606524a43d008"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer f3548ba6b6f1cdda898ae6d1ab0b24fcbeba0cea5e66520019edb6bce713fa4b
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
    "id": 10,
    "uploader": {
      "id": 936,
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
      "created_at": "2016-10-25T20:45:18.377Z",
      "updated_at": "2016-10-25T20:45:18.377Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T20:45:18.450Z",
    "updated_at": "2016-10-25T20:45:18.450Z",
    "course_id": 300,
    "filename": "Pastry Making Notes.pdf",
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
| file[status] | Status |
| file[download_count] | Download count |
| file[created_at] | Created at |
| file[updated_at] | Updated at |
| file[course_id] | Course ID |
| file[category] | Category |
| file[is_anonymous] | Anonymous |


```shell
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3548ba6b6f1cdda898ae6d1ab0b24fcbeba0cea5e66520019edb6bce713fa4b"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer 4ea88f713debb2e9c00222d76e563670a8f6576132384a1647023ccb2b70dbee
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
      "creator_id": 163,
      "id": 48,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 48,
      "additional_university_ids": [

      ],
      "topic_id": 50,
      "discipline_id": 51,
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
      "chapters_updated_at": "2016-10-25T20:44:15.058Z",
      "updated_at": "2016-10-25T20:44:16.596Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 168,
      "id": 49,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-3ecb9674-87f1-4f5d-93bf-ae37c3dbebc3",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-3ecb9674-87f1-4f5d-93bf-ae37c3dbebc3",
      "slug": "mit-the-great-british-bake-off-3ecb9674-87f1-4f5d-93bf-ae37c3dbebc3",
      "university_id": 49,
      "additional_university_ids": [

      ],
      "topic_id": 51,
      "discipline_id": 52,
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
      "chapters_updated_at": "2016-10-25T20:44:15.058Z",
      "updated_at": "2016-10-25T20:44:17.121Z",
      "shortname": "mit-the-great-british-bake-off-3ecb9674-87f1-4f5d-93bf-ae37c3dbebc3"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 4ea88f713debb2e9c00222d76e563670a8f6576132384a1647023ccb2b70dbee"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/13/report
Content-Type: application/json
Authorization: Bearer 81fbfbe92c178260d3c3911e39585075903803357d2da3413a881d2af5311ef1
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81fbfbe92c178260d3c3911e39585075903803357d2da3413a881d2af5311ef1"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/25/comments
Content-Type: application/json
Authorization: Bearer dfd38ccc1ef0a03fb108f91c384f878f61282e0a508c9ca75bf5ba5da532f011
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
    "id": 17,
    "author_id": 432,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:44:38.177Z",
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
curl "api.goskive.com/v2/flashcards/25/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfd38ccc1ef0a03fb108f91c384f878f61282e0a508c9ca75bf5ba5da532f011"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/24/comments
Content-Type: application/json
Authorization: Bearer 239b12dbd798d0ea3f03111734b0e425893a830ddb7ffb2abfa34ce090c737fe
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
    "id": 16,
    "author_id": 429,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:44:37.816Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 429,
      "feedbackable_id": 24,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:37.813Z",
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
curl "api.goskive.com/v2/flashcards/24/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 239b12dbd798d0ea3f03111734b0e425893a830ddb7ffb2abfa34ce090c737fe"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/22/comments
Content-Type: application/json
Authorization: Bearer 88ceaafd98d40b4c674bf1b471354ab4297950930349987afe783a0e983a5eda
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
      "id": 15,
      "author_id": 425,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:44:37.429Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 424,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:44:37.413Z",
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
curl "api.goskive.com/v2/flashcards/22/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88ceaafd98d40b4c674bf1b471354ab4297950930349987afe783a0e983a5eda"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/26/comments
Content-Type: application/json
Authorization: Bearer 71e0c12948c9728b4da66245b3dbe13dbeb66020abff7b37d89911a4882b9f36
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
curl "api.goskive.com/v2/flashcards/26/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71e0c12948c9728b4da66245b3dbe13dbeb66020abff7b37d89911a4882b9f36"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/41/feedbacks
Content-Type: application/json
Authorization: Bearer 980949a7f2ddfdb2f22fc8b39827be5d7c395218710ae10684434636f55e7146
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
    "id": 46,
    "user_id": 518,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:44:44.469Z",
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
	-H "Authorization: Bearer 980949a7f2ddfdb2f22fc8b39827be5d7c395218710ae10684434636f55e7146"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/34/feedbacks
Content-Type: application/json
Authorization: Bearer 6a83633a7b1addfe7f6e3dc75ee243fa5cd199ef3b136324fcb0b1df6a0e177d
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
      "id": 40,
      "user_id": 489,
      "feedbackable_id": 34,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:42.909Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 488,
      "feedbackable_id": 34,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:42.898Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/34/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a83633a7b1addfe7f6e3dc75ee243fa5cd199ef3b136324fcb0b1df6a0e177d"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/28/votes
Content-Type: application/json
Authorization: Bearer 034b5da89d3b3f3a5eac718ff9b774cbe59802d190168ff5aef28d387b3c6de7
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
      "id": 13,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 447
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 446
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 445
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/28/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 034b5da89d3b3f3a5eac718ff9b774cbe59802d190168ff5aef28d387b3c6de7"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/43/republish
Content-Type: application/json
Authorization: Bearer c40fcad26aac4e4231ad27161e3a06b3d964702015cf3d657dac5ee430d8b602
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
curl "api.goskive.com/v2/flashcards/43/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c40fcad26aac4e4231ad27161e3a06b3d964702015cf3d657dac5ee430d8b602"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/48/bookmark
Content-Type: application/json
Authorization: Bearer 5772eab32a4482bc54c2817a601a4c0813dc96bbd094fdc3d5a00fb4b662f102
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/48/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5772eab32a4482bc54c2817a601a4c0813dc96bbd094fdc3d5a00fb4b662f102"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/46
Content-Type: application/json
Authorization: Bearer ffc4089da85cc26b76425877c0e08b938099648782f93d4c1e98859d8ee4039b
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffc4089da85cc26b76425877c0e08b938099648782f93d4c1e98859d8ee4039b"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/downvote
Content-Type: application/json
Authorization: Bearer 83106c036ce22b90b360be99241d26b79f75b2e2b531d1cdc9f2de579e13cccf
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83106c036ce22b90b360be99241d26b79f75b2e2b531d1cdc9f2de579e13cccf"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/45
Content-Type: application/json
Authorization: Bearer 917b27259b14800a668aab45337355be0f85f3d92710126653dc25866d32d87f
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
    "author_id": 534,
    "chapter_id": 124,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:44:45.712Z",
    "created_at": "2016-10-25T20:44:45.712Z",
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
	-H "Authorization: Bearer 917b27259b14800a668aab45337355be0f85f3d92710126653dc25866d32d87f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/47/report
Content-Type: application/json
Authorization: Bearer 9eba1b40a1e9144262f6b3edbabe22f83471fa47d05a5b1ad7b4c0a796a09a1f
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/47/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9eba1b40a1e9144262f6b3edbabe22f83471fa47d05a5b1ad7b4c0a796a09a1f"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/44/bookmark
Content-Type: application/json
Authorization: Bearer 3a0a5b4579624ee148a679a912a387096a6198f83b75dec2aae884511fd43ccf
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a0a5b4579624ee148a679a912a387096a6198f83b75dec2aae884511fd43ccf"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/upvote
Content-Type: application/json
Authorization: Bearer dc6dd2cce07d336c49aed4e67170b232dc69829db23277323f0fffd68c251c82
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc6dd2cce07d336c49aed4e67170b232dc69829db23277323f0fffd68c251c82"
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
    "key": "cache/4d99d268019ef461f683a709040bccc3.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQyMTo0NDoxOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzRkOTlkMjY4MDE5ZWY0NjFmNjgzYTcwOTA0MGJjY2MzLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjVUMjA0NDE5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T204419Z",
    "x-amz-signature": "3094efbab26368bb6e576a18ed3bd20d5bd124093424145d5fc256e20fdc64eb"
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
POST /v2/me/jobs/2/sign_ups
Content-Type: application/json
Authorization: Bearer decca72115dbf89f809815a296bf60011a15804e2687dc713074c14508b3285c
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
	-H "Authorization: Bearer decca72115dbf89f809815a296bf60011a15804e2687dc713074c14508b3285c"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 32a69b515542a6db98044d4c41e457191f339b109708f46a13da17cce4c78c0b
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
	-H "Authorization: Bearer 32a69b515542a6db98044d4c41e457191f339b109708f46a13da17cce4c78c0b"
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
{"password":{"reset_password_token":"xoGnTzmY_L9jU5gZhVLS","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 962,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-25T20:45:21.342Z",
  "updated_at": "2016-10-25T20:45:21.480Z",
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
  "audit_id": 5460
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"xoGnTzmY_L9jU5gZhVLS","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer 0a0308abf0b5715710f435a16f13db7a8ea0186809899ed7afd0792b6007d193
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
    "id": 6,
    "author_id": 50,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:44:08.413Z",
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
curl "api.goskive.com/v2/questions/12/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a0308abf0b5715710f435a16f13db7a8ea0186809899ed7afd0792b6007d193"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/13/comments
Content-Type: application/json
Authorization: Bearer 9de4c139eb066aa742b98fd82fa083d0da46abc59c5f1c173b99089395d24467
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
    "id": 7,
    "author_id": 53,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:44:08.910Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 53,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:08.907Z",
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
curl "api.goskive.com/v2/questions/13/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9de4c139eb066aa742b98fd82fa083d0da46abc59c5f1c173b99089395d24467"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/15/comments
Content-Type: application/json
Authorization: Bearer 146f44ac3406ce60cd61d0b5d38ef8da7abf9a36fb56d13d9ea0c596f3009fd5
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
      "id": 8,
      "author_id": 62,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:44:09.624Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 63,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:44:09.639Z",
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
curl "api.goskive.com/v2/questions/15/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 146f44ac3406ce60cd61d0b5d38ef8da7abf9a36fb56d13d9ea0c596f3009fd5"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/14/comments
Content-Type: application/json
Authorization: Bearer e08a8f5f23f70e268a754d8217603bf62b1b81fcf2bf128f7e4584e083619339
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
curl "api.goskive.com/v2/questions/14/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e08a8f5f23f70e268a754d8217603bf62b1b81fcf2bf128f7e4584e083619339"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/8/feedbacks
Content-Type: application/json
Authorization: Bearer 2f89e3af1a9ef496a6f0746d22a2342440a389ceec09f323cdd0088da10b9ea7
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
    "id": 8,
    "user_id": 34,
    "feedbackable_id": 8,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:44:06.703Z",
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
curl "api.goskive.com/v2/questions/8/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f89e3af1a9ef496a6f0746d22a2342440a389ceec09f323cdd0088da10b9ea7"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/2/feedbacks
Content-Type: application/json
Authorization: Bearer 215a7f8d28a41851945f5cee2a3eefd9a696f0681087a029e75eee29521e45f4
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
      "id": 2,
      "user_id": 8,
      "feedbackable_id": 2,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:04.404Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 1,
      "user_id": 7,
      "feedbackable_id": 2,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:44:04.393Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 215a7f8d28a41851945f5cee2a3eefd9a696f0681087a029e75eee29521e45f4"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/29/votes
Content-Type: application/json
Authorization: Bearer d565556fd3ae00369dcab4fe07c13039b7d2ff1e34666c70273cd5b02e8da762
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
      "votable_id": 29,
      "user_id": 187
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 29,
      "user_id": 186
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 29,
      "user_id": 185
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/29/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d565556fd3ae00369dcab4fe07c13039b7d2ff1e34666c70273cd5b02e8da762"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/112/republish
Content-Type: application/json
Authorization: Bearer 96e5a6945d1af06df66be09ecc54bfb046982ae1c8afed7716a80860e195db59
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
curl "api.goskive.com/v2/questions/112/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96e5a6945d1af06df66be09ecc54bfb046982ae1c8afed7716a80860e195db59"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/111/bookmark
Content-Type: application/json
Authorization: Bearer ba7e3c414a57e6c9370ab49d2e90f8634fb08669275e69d3444a1c440e1c4897
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba7e3c414a57e6c9370ab49d2e90f8634fb08669275e69d3444a1c440e1c4897"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/107
Content-Type: application/json
Authorization: Bearer 064064828c021935ed3f54020e05975cd14fa98690feb3caa376ca51b3a79658
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/107" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 064064828c021935ed3f54020e05975cd14fa98690feb3caa376ca51b3a79658"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/115/downvote
Content-Type: application/json
Authorization: Bearer 7f3faf83a102946cef1c9f1a10a8b51866d61aa127854503c01e8705014bcb93
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f3faf83a102946cef1c9f1a10a8b51866d61aa127854503c01e8705014bcb93"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/108
Content-Type: application/json
Authorization: Bearer a9925b129b68e57abd4441b03729b65f12f77a23d6ec9c5de65b9129079bac4e
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 826,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:45:08.891Z",
    "created_at": "2016-10-25T20:45:08.780Z",
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
        "id": 218,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 219,
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
curl "api.goskive.com/v2/questions/108" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9925b129b68e57abd4441b03729b65f12f77a23d6ec9c5de65b9129079bac4e"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/131/report
Content-Type: application/json
Authorization: Bearer 183ce427d449670878be2c7ff5ff1585106862860519a91b62d5a66d71728331
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/131/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 183ce427d449670878be2c7ff5ff1585106862860519a91b62d5a66d71728331"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/114/bookmark
Content-Type: application/json
Authorization: Bearer 9f514461055a978dcb2a55ed3216e390f016e47352c11de52d3b710ca19107a6
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f514461055a978dcb2a55ed3216e390f016e47352c11de52d3b710ca19107a6"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/109
Content-Type: application/json
Authorization: Bearer ddc7d73aa6d311d4c581914b0bfb90ec26975bc1b9b8d53808954f7a4e3d8e8c
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":109,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T20:45:09.143Z","updated_at":"2016-10-25T20:45:09.259Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":170,"author_id":829,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 109,
    "obfuscated_id": "VSPyck5c2RY",
    "author_id": 829,
    "chapter_id": 170,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:45:09.361Z",
    "created_at": "2016-10-25T20:45:09.143Z",
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
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>109, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-25T20:45:09.143Z\", \"updated_at\"=>\"2016-10-25T20:45:09.259Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>170, \"author_id\"=>829, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 220,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 221,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 222,
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
curl "api.goskive.com/v2/questions/109" -d '{"question":{"question":{"id":109,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T20:45:09.143Z","updated_at":"2016-10-25T20:45:09.259Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":170,"author_id":829,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddc7d73aa6d311d4c581914b0bfb90ec26975bc1b9b8d53808954f7a4e3d8e8c"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/110/upvote
Content-Type: application/json
Authorization: Bearer 815b704729540f2e6f0ee2ce8bebd9f844f236c74503a7c38738753c8d8aaa1f
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 815b704729540f2e6f0ee2ce8bebd9f844f236c74503a7c38738753c8d8aaa1f"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6e87b17f174139fa2b6c584a6e86a7bbbd4afbe32bee03770c21c1d398e00bbf
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
      "creator_id": 953,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 285,
      "additional_university_ids": [

      ],
      "topic_id": 319,
      "discipline_id": 320,
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
      "updated_at": "2016-10-25T20:45:19.520Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e87b17f174139fa2b6c584a6e86a7bbbd4afbe32bee03770c21c1d398e00bbf"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 7bf511503b176e43178aaaafd910e8d29378495296b7de20b6ed6d80e40faf39
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
      "id": 288,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-270",
      "html_url": "https://goskive.com/university/uni-270",
      "slug": "uni-270",
      "name": "National School of Pizza",
      "short_name": "Uni 270",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/456eae9ef6c448c1b3a29778a48892ecbfc9f665.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b28d91d39077f6205f0ef17bf61845794d14421f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:45:19.759Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 287,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-269",
      "html_url": "https://goskive.com/university/uni-269",
      "slug": "uni-269",
      "name": "National School of Pastry",
      "short_name": "Uni 269",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/149328b653f81c7e65fd887503945fa9ce98128f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/43a70809cc637caf1e4ca8f661c78d607f5a86bd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:45:19.743Z",
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
	-H "Authorization: Bearer 7bf511503b176e43178aaaafd910e8d29378495296b7de20b6ed6d80e40faf39"
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
      "id": 53,
      "name": "Re-contextualized transitional leverage",
      "name_translations": {
        "en": "Re-contextualized transitional leverage"
      },
      "discipline_id": 54
    },
    {
      "id": 54,
      "name": "Open-architected explicit productivity",
      "name_translations": {
        "en": "Open-architected explicit productivity"
      },
      "discipline_id": 55
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
GET /v2/topics/55
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
    "id": 55,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 56
  }
}
```



```shell
curl "api.goskive.com/v2/topics/55" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer f1883d833636fa9194a7b96e00e8a35e18a9b326d79594291e53164cb247d941
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
      "name": "University 211",
      "short_name": "Uni 274",
      "acronym": "MIT",
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
      "updated_at": "2016-10-25T20:45:21.565Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-273",
      "html_url": "https://goskive.com/university/uni-273",
      "slug": "uni-273",
      "name": "University 210",
      "short_name": "Uni 273",
      "acronym": "MIT",
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
      "updated_at": "2016-10-25T20:45:21.549Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 290,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-272",
      "html_url": "https://goskive.com/university/uni-272",
      "slug": "uni-272",
      "name": "University 209",
      "short_name": "Uni 272",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/1084079aa5c54cda74ccc2533b2a7fb5ed25f898.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4c5d00318fb7c537b4d2dbd3e16f01d72ba28007.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:45:21.533Z",
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
	-H "Authorization: Bearer f1883d833636fa9194a7b96e00e8a35e18a9b326d79594291e53164cb247d941"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 05603aaa0d788ea287ba18e3e7186d22c373cf977e60b4e64bab7b00c7c01b79
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
    "id": 293,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/24d3506bc78b01ae84cda49d13a88c81489eb0a3.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/31760a483210dcdae41652488f2d8ffaea633a49.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-25T20:45:21.673Z",
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
	-H "Authorization: Bearer 05603aaa0d788ea287ba18e3e7186d22c373cf977e60b4e64bab7b00c7c01b79"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6a22f9b9783c10165e54ce7127dbedf2b1ee01eda607cbcf59e37866ddd867f7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":208,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 643,
    "id": 196,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "topic_id": 208,
    "discipline_id": 209,
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
    "chapters_updated_at": "2016-10-25T20:44:52.800Z",
    "updated_at": "2016-10-25T20:44:52.934Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 149,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-25T20:44:52.893Z",
        "course_id": 196,
        "author_id": 643,
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
        "id": 150,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-25T20:44:52.909Z",
        "course_id": 196,
        "author_id": 643,
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
        "id": 151,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-25T20:44:52.925Z",
        "course_id": 196,
        "author_id": 643,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":208,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a22f9b9783c10165e54ce7127dbedf2b1ee01eda607cbcf59e37866ddd867f7"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b164af22fee16be9469199996a8cd08c573ceed859e7a549fa76b363284d4c68
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":209,"published":false}}
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
    "creator_id": 644,
    "id": 197,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "topic_id": 209,
    "discipline_id": 210,
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
    "updated_at": "2016-10-25T20:44:53.077Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":209,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b164af22fee16be9469199996a8cd08c573ceed859e7a549fa76b363284d4c68"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5bdb90ff6b9d4ea31f6b7ac564587b16b22fadd1897252e80ea59fd6293d566c
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
      "creator_id": 617,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-125",
      "html_url": "https://goskive.com/course/fu-course-125",
      "slug": "fu-course-125",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "topic_id": 186,
      "discipline_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 125",
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
      "updated_at": "2016-10-25T20:44:50.524Z",
      "shortname": "fu-course-125"
    },
    {
      "creator_id": 617,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "topic_id": 187,
      "discipline_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "chapters_updated_at": "2016-10-25T20:44:50.799Z",
      "updated_at": "2016-10-25T20:44:50.805Z",
      "shortname": "fu-course-126"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bdb90ff6b9d4ea31f6b7ac564587b16b22fadd1897252e80ea59fd6293d566c"
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
      "creator_id": 637,
      "id": 190,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 202,
      "discipline_id": 203,
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
      "updated_at": "2016-10-25T20:44:52.239Z",
      "shortname": "fu-course-141"
    },
    {
      "creator_id": 637,
      "id": 191,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 203,
      "discipline_id": 204,
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
      "chapters_updated_at": "2016-10-25T20:44:52.513Z",
      "updated_at": "2016-10-25T20:44:52.519Z",
      "shortname": "fu-course-142"
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
Authorization: Bearer 20243ea06988f859e0da8e59137c6ad80ebae63468a5ba5aaa560f2c0d766618
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
      "creator_id": 623,
      "id": 178,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-129",
      "html_url": "https://goskive.com/course/fu-course-129",
      "slug": "fu-course-129",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "topic_id": 190,
      "discipline_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 129",
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
      "updated_at": "2016-10-25T20:44:51.023Z",
      "shortname": "fu-course-129"
    },
    {
      "creator_id": 623,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "topic_id": 191,
      "discipline_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 130",
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
      "updated_at": "2016-10-25T20:44:51.062Z",
      "shortname": "fu-course-130"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20243ea06988f859e0da8e59137c6ad80ebae63468a5ba5aaa560f2c0d766618"
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
      "creator_id": 642,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 174,
      "additional_university_ids": [

      ],
      "topic_id": 206,
      "discipline_id": 207,
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
      "updated_at": "2016-10-25T20:44:52.726Z",
      "shortname": "fu-course-145"
    },
    {
      "creator_id": 642,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 174,
      "additional_university_ids": [

      ],
      "topic_id": 207,
      "discipline_id": 208,
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
      "updated_at": "2016-10-25T20:44:52.764Z",
      "shortname": "fu-course-146"
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
Authorization: Bearer 30a0ed387a66ec268850d163086dea0d7996a10b6ba4070df75c3cb652bace46
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
  "id": 438,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-25T20:44:38.598Z",
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
	-H "Authorization: Bearer 30a0ed387a66ec268850d163086dea0d7996a10b6ba4070df75c3cb652bace46"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/288
Content-Type: application/json
Authorization: Bearer ba2ac07e5db20afba58dc1ea1cd8d072a332796f0c83c8a19b7c27f47b6335ac
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
    "id": 288,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 80,
    "fields_of_study": [
      90,
      91
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-25T20:44:27.496Z",
    "updated_at": "2016-10-25T20:44:27.496Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/288" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba2ac07e5db20afba58dc1ea1cd8d072a332796f0c83c8a19b7c27f47b6335ac"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/286
Content-Type: application/json
Authorization: Bearer 5c6b9bed342c1b69da4d1e51a2587fd207df42f2fbdfcba13b4b2432ff256427
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
    "id": 286,
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
    "created_at": "2016-10-25T20:44:27.352Z",
    "updated_at": "2016-10-25T20:44:27.352Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/286" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c6b9bed342c1b69da4d1e51a2587fd207df42f2fbdfcba13b4b2432ff256427"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/7
Content-Type: application/json
Authorization: Bearer e3d01ce9363591f0e9480baa23343884776f1087c2c938a94ddd96bcab9a542f
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3d01ce9363591f0e9480baa23343884776f1087c2c938a94ddd96bcab9a542f"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/6
Content-Type: application/json
Authorization: Bearer 2059f847786a52a0a34a9ca0b55253e10c9e0aa2212b58948c22380137e713ec
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
    "id": 6,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 39,
    "user_id": 245
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2059f847786a52a0a34a9ca0b55253e10c9e0aa2212b58948c22380137e713ec"
```
