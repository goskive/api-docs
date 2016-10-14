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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7d45efe3c2c9083de2397d4edbdbf93a84d14567ac209967e7523806a21d4493","client_secret":"5a8b607f6e5c6e09933eac43ab27fd410857920d8f7b027b711e80a6c3bdfe63"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7d45efe3c2c9083de2397d4edbdbf93a84d14567ac209967e7523806a21d4493","client_secret":"5a8b607f6e5c6e09933eac43ab27fd410857920d8f7b027b711e80a6c3bdfe63"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YzdjYmZlYWI0Yzc4MDM0OGIxNjhhYWJiODc0YjQwZjZhN2Q5NmNmOWMzZjE1
OTIxM2I2NjRjOTYzNWVjNzFiZDowOWUxMWNkZmMwYTllMWQwN2ExOTgzZmFh
ODc3Yzg3YzNiOGJmZjBhNjViMGUxM2NkYTIxMTIzNzIwMjRkYzNh

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
	-u c7cbfeab4c780348b168aabb874b40f6a7d96cf9c3f159213b664c9635ec71bd:09e11cdfc0a9e1d07a1983faa877c87c3b8bff0a65b0e13cda2112372024dc3a
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
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"client_credentials","client_id":"dc83d5adca9bdc077cae43c307e1824c9404f14dac68761bc8dd83ec228d3e19","client_secret":"cbb65141a13e0e38eb0aa77b20e3fdfceceabb9dc2caba58a2e86e9c6e6255b3"}
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
  "access_token": "c582ffa96088107bad47cb69fd590bc3c4538d8dd25c505588c16b1f2f0c7fb3",
  "token_type": "bearer",
  "created_at": 1476470632
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"dc83d5adca9bdc077cae43c307e1824c9404f14dac68761bc8dd83ec228d3e19","client_secret":"cbb65141a13e0e38eb0aa77b20e3fdfceceabb9dc2caba58a2e86e9c6e6255b3"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"b00d8d6c7f5d86cd73a23ca9a5d032afcf4c612d6d59ccca8030aa8977f23421","client_secret":"2749a95f518bba349eebeaf860f3b2a63fff5ca5ce3962c2f9698e6f64e59d08"}
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
  "access_token": "b7cd4f8b8c73d13fa1cf64a9a0e29cd439290b360cef917348f11238cce353da",
  "token_type": "bearer",
  "created_at": 1476470632
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"b00d8d6c7f5d86cd73a23ca9a5d032afcf4c612d6d59ccca8030aa8977f23421","client_secret":"2749a95f518bba349eebeaf860f3b2a63fff5ca5ce3962c2f9698e6f64e59d08"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MTk5NGU2ZmYwNGM3NDk4ZmI4ZjIyNWExMzgxNTJlOWVhN2QyNWRhNTBmYTNh
YjllOTdiYzkxMGRmNGEwYzY5Yzo2OGFiN2Y4MTJiODE5MzgwMTViYzEzZGE3
ODdkZjg4MjZhY2IyYzhjZDRiYjkxYThiZmZmZTk3MzllN2EyYzhl

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
  "access_token": "3fb523f75b0ea27766e839af69e44e1273fa64c0765f1a22b6e0b39bcb536d13",
  "token_type": "bearer",
  "created_at": 1476470632
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 1994e6ff04c7498fb8f225a138152e9ea7d25da50fa3ab9e97bc910df4a0c69c:68ab7f812b81938015bc13da787df8826acb2c8cd4bb91a8bfffe9739e7a2c8e
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
Authorization: Bearer 848c2a2b681402543d9ee9bbfe11b312ebede48b17cd39d109fd41018b166bde
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
	-H "Authorization: Bearer 848c2a2b681402543d9ee9bbfe11b312ebede48b17cd39d109fd41018b166bde"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/42/flashcards
Content-Type: application/json
Authorization: Bearer 110e44c87f74f43d92909840ee980a6d055f2d1fcf3560ad21d32d84a992bdbd
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":42,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 9,
    "obfuscated_id": "DMbUb8tMXMw",
    "author_id": 160,
    "chapter_id": 42,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:43:40.245Z",
    "created_at": "2016-10-14T18:43:40.245Z",
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
curl "api.goskive.com/v2/chapters/42/flashcards" -d '{"flashcard":{"chapter_id":42,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 110e44c87f74f43d92909840ee980a6d055f2d1fcf3560ad21d32d84a992bdbd"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/43/flashcards
Content-Type: application/json
Authorization: Bearer da23b9b06acbf0dcdd9162286e4523e83d02a17a1c8ecd27a235b2411cf63ff7
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
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 161,
      "chapter_id": 43,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:40.401Z",
      "created_at": "2016-10-14T18:43:40.401Z",
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 161,
      "chapter_id": 43,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:40.441Z",
      "created_at": "2016-10-14T18:43:40.441Z",
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
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 161,
      "chapter_id": 43,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:40.481Z",
      "created_at": "2016-10-14T18:43:40.481Z",
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
curl "api.goskive.com/v2/chapters/43/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da23b9b06acbf0dcdd9162286e4523e83d02a17a1c8ecd27a235b2411cf63ff7"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/81/questions
Content-Type: application/json
Authorization: Bearer bcb099a97d97b045e0f6db3b7465749c13f14a45eb8de2245018d1d9a1d85404
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":81,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 387,
    "chapter_id": 81,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:44:05.522Z",
    "created_at": "2016-10-14T18:44:05.522Z",
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
        "id": 159,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 160,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 161,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 162,
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
curl "api.goskive.com/v2/chapters/81/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":81,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcb099a97d97b045e0f6db3b7465749c13f14a45eb8de2245018d1d9a1d85404"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/79/questions
Content-Type: application/json
Authorization: Bearer f4e1443ac4d642b9442ba2c8632e19330d9f0d5800c964c42cd24f97fde96d05
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":79,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 381,
    "chapter_id": 79,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:44:04.858Z",
    "created_at": "2016-10-14T18:44:04.858Z",
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
        "id": 155,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 156,
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
curl "api.goskive.com/v2/chapters/79/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":79,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4e1443ac4d642b9442ba2c8632e19330d9f0d5800c964c42cd24f97fde96d05"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/80/questions
Content-Type: application/json
Authorization: Bearer 14d960efaff1f71e694e4cabe9d50e3ccb54c75336f76ed96bc68b2183567cce
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":80,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 78,
    "obfuscated_id": "-wsYNe2w7uo",
    "author_id": 384,
    "chapter_id": 80,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:44:05.184Z",
    "created_at": "2016-10-14T18:44:05.184Z",
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
        "id": 157,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 158,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/80/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":80,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14d960efaff1f71e694e4cabe9d50e3ccb54c75336f76ed96bc68b2183567cce"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/78/questions
Content-Type: application/json
Authorization: Bearer 65ea800d5d046294c14f5fb86623f0398676ffc026fae1f02225c1f78fdddbf2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":78,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 76,
    "obfuscated_id": "oK0h_-4yfUk",
    "author_id": 378,
    "chapter_id": 78,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:44:04.445Z",
    "created_at": "2016-10-14T18:44:04.445Z",
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
        "id": 152,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 153,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 154,
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
curl "api.goskive.com/v2/chapters/78/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":78,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65ea800d5d046294c14f5fb86623f0398676ffc026fae1f02225c1f78fdddbf2"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/77/questions
Content-Type: application/json
Authorization: Bearer 74aacb8ba78d5d5b58e140e79a7e488936b6aa205dd94ba6a684a87055b411ec
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 372,
      "chapter_id": 77,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:03.802Z",
      "created_at": "2016-10-14T18:44:03.689Z",
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
          "id": 146,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 147,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 373,
      "chapter_id": 77,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:03.988Z",
      "created_at": "2016-10-14T18:44:03.873Z",
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
          "id": 148,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 149,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 374,
      "chapter_id": 77,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:04.184Z",
      "created_at": "2016-10-14T18:44:04.062Z",
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
          "id": 150,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 151,
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
curl "api.goskive.com/v2/chapters/77/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74aacb8ba78d5d5b58e140e79a7e488936b6aa205dd94ba6a684a87055b411ec"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/187
Content-Type: application/json
Authorization: Bearer c08f921733338cb5a333f0e77ea4e4b46fc197fbe113226c5cb438df6bfea682
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
curl "api.goskive.com/v2/chapters/187" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c08f921733338cb5a333f0e77ea4e4b46fc197fbe113226c5cb438df6bfea682"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 3a9fec551fe92293712a5a8be8e502ed2cc3b7cb2ca8309b915724c7e48b531a
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
curl "api.goskive.com/v2/chapters/189" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a9fec551fe92293712a5a8be8e502ed2cc3b7cb2ca8309b915724c7e48b531a"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 1c496e14ba6b089ab7e5c3281cd50f15313dcd27ad7867f3adb812bf7d16fce0
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
curl "api.goskive.com/v2/chapters/190" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c496e14ba6b089ab7e5c3281cd50f15313dcd27ad7867f3adb812bf7d16fce0"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/188
Content-Type: application/json
Authorization: Bearer f0befda88592dd766ff2f806cf75bc047ea7d93b66364efc69fc7730ac18ea62
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/188" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0befda88592dd766ff2f806cf75bc047ea7d93b66364efc69fc7730ac18ea62"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/185
Content-Type: application/json
Authorization: Bearer 5ea9ee44f775a435ea3ebf87eaf78b2914f4d7d96d038c1694b708ed34ab661c
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
    "id": 185,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T18:44:42.947Z",
    "course_id": 297,
    "author_id": 928,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-14T18:44:42.399Z",
    "questions_updated_at": "2016-10-14T18:44:42.399Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 932,
        "chapter_id": 185,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.930Z",
        "created_at": "2016-10-14T18:44:42.930Z",
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
        "id": 129,
        "obfuscated_id": "x8EyeGrWnN4",
        "author_id": 930,
        "chapter_id": 185,
        "position": 116,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.825Z",
        "created_at": "2016-10-14T18:44:42.707Z",
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
            "id": 261,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 262,
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
curl "api.goskive.com/v2/chapters/185" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ea9ee44f775a435ea3ebf87eaf78b2914f4d7d96d038c1694b708ed34ab661c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/192
Content-Type: application/json
Authorization: Bearer 391882fb7a1159b878c4695646b138a6a18e0214ee7ebbf720fdae30e9e307ea
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
    "id": 192,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T18:44:44.367Z",
    "course_id": 304,
    "author_id": 953,
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
curl "api.goskive.com/v2/chapters/192" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 391882fb7a1159b878c4695646b138a6a18e0214ee7ebbf720fdae30e9e307ea"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 23b350d38cebfb6d623ee3a87164599e8a487d90041f97bd71ab5f9b6ed20966
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
    "id": 59,
    "author_id": 897,
    "reply_to_id": 58,
    "created_at": "2016-10-14T18:44:40.426Z",
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
curl "api.goskive.com/v2/comments/58/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23b350d38cebfb6d623ee3a87164599e8a487d90041f97bd71ab5f9b6ed20966"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer a186609969ad71acacb125dc258edc50fb975c66ae0b8ad9311f74395a120e17
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
curl "api.goskive.com/v2/comments/60/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a186609969ad71acacb125dc258edc50fb975c66ae0b8ad9311f74395a120e17"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/16
Content-Type: application/json
Authorization: Bearer e14debb306215dccd7fde51f2fc11557887d45d6abc5a6be43038fd5cce31882
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
curl "api.goskive.com/v2/comments/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e14debb306215dccd7fde51f2fc11557887d45d6abc5a6be43038fd5cce31882"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/15/republish
Content-Type: application/json
Authorization: Bearer 9ae46bf746c5aa655bb48ea01d51023dd2a99a11652c8065277b86d19d77e5f6
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
curl "api.goskive.com/v2/comments/15/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ae46bf746c5aa655bb48ea01d51023dd2a99a11652c8065277b86d19d77e5f6"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/18
Content-Type: application/json
Authorization: Bearer 541a72f7d8706c1afc50bf70ff97796d06a264a90ea4ffdfaef0e5b90645b7f0
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 541a72f7d8706c1afc50bf70ff97796d06a264a90ea4ffdfaef0e5b90645b7f0"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/19/report
Content-Type: application/json
Authorization: Bearer c1aa0ed1fdd2a444066df88d2d07093e3c19922055cec0f63de0e9a435079165
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/19/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1aa0ed1fdd2a444066df88d2d07093e3c19922055cec0f63de0e9a435079165"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/24
Content-Type: application/json
Authorization: Bearer e731bd3cb228ece1f4f685fd53c6430e30c0154001ff07079627100e4d7cce51
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
    "updated_at": "2016-10-14T18:43:57.599Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e731bd3cb228ece1f4f685fd53c6430e30c0154001ff07079627100e4d7cce51"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 36dc9d4ed583ed695f8d47f8c04064704af1fdf0d5782906dc8a5bc94f12c79d
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
      "name": "Fake Company Name 21",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T18:43:57.679Z"
    },
    {
      "id": 26,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T18:43:57.684Z"
    },
    {
      "id": 27,
      "name": "Fake Company Name 23",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T18:43:57.688Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36dc9d4ed583ed695f8d47f8c04064704af1fdf0d5782906dc8a5bc94f12c79d"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/23/company_profiles
Content-Type: application/json
Authorization: Bearer fee8ecd35b90ddababf6068918ef7bc5d1dd40205f00da37891ed572feb2cee1
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
curl "api.goskive.com/v2/companies/23/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fee8ecd35b90ddababf6068918ef7bc5d1dd40205f00da37891ed572feb2cee1"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/21/company_profiles
Content-Type: application/json
Authorization: Bearer 432c6c4898ced709ae22c6509780acf37fe1b759e05fba44af19da76fc3f94f9
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
curl "api.goskive.com/v2/companies/21/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 432c6c4898ced709ae22c6509780acf37fe1b759e05fba44af19da76fc3f94f9"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 7be245fe1b0830dde03add71dff1eebf0c0a3bb53678cc4d04b75c3b25049e04
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
	-H "Authorization: Bearer 7be245fe1b0830dde03add71dff1eebf0c0a3bb53678cc4d04b75c3b25049e04"
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
Authorization: Bearer 4f5c970e8a6424244f7b04483759b96dc0e60bfe580daf8f79d50490e2bdeef5
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
	-H "Authorization: Bearer 4f5c970e8a6424244f7b04483759b96dc0e60bfe580daf8f79d50490e2bdeef5"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7e8d7fa23a989b7c49dc9ffa4cf4da454f5a2990b099b9256a271176a872ec4c
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
    "id": 149,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T18:44:28.101Z",
    "course_id": 213,
    "author_id": 687,
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
	-H "Authorization: Bearer 7e8d7fa23a989b7c49dc9ffa4cf4da454f5a2990b099b9256a271176a872ec4c"
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
      "id": 154,
      "title": "Clever Chapter Title 139",
      "position": 1,
      "updated_at": "2016-10-14T18:44:28.698Z",
      "course_id": 217,
      "author_id": 698,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 155,
      "title": "Clever Chapter Title 140",
      "position": 2,
      "updated_at": "2016-10-14T18:44:28.723Z",
      "course_id": 217,
      "author_id": 699,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 156,
      "title": "Clever Chapter Title 141",
      "position": 3,
      "updated_at": "2016-10-14T18:44:28.980Z",
      "course_id": 217,
      "author_id": 700,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T18:44:28.622Z",
      "questions_updated_at": "2016-10-14T18:44:28.622Z",
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
Authorization: Bearer bf56ac194a946201beaf4cbb3ff41900cc6481b1f37b70def8bb54e8d45d8758
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
      "id": 160,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-14T18:44:29.358Z",
      "course_id": 220,
      "author_id": 709,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 161,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-14T18:44:29.383Z",
      "course_id": 220,
      "author_id": 710,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 162,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-14T18:44:29.642Z",
      "course_id": 220,
      "author_id": 711,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T18:44:29.278Z",
      "questions_updated_at": "2016-10-14T18:44:29.278Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf56ac194a946201beaf4cbb3ff41900cc6481b1f37b70def8bb54e8d45d8758"
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
      "id": 157,
      "title": "Clever Chapter Title 142",
      "position": 1,
      "updated_at": "2016-10-14T18:44:29.103Z",
      "course_id": 218,
      "author_id": 704,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 158,
      "title": "Clever Chapter Title 143",
      "position": 2,
      "updated_at": "2016-10-14T18:44:29.129Z",
      "course_id": 218,
      "author_id": 705,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 159,
      "title": "Clever Chapter Title 144",
      "position": 3,
      "updated_at": "2016-10-14T18:44:29.154Z",
      "course_id": 218,
      "author_id": 706,
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
Authorization: Bearer 58ebe66f81146e7401fc75a81ea8b468032f6f57ee30d859be5fe9b9f9503a40
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
      "id": 163,
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-14T18:44:29.803Z",
      "course_id": 221,
      "author_id": 716,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 164,
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-14T18:44:29.829Z",
      "course_id": 221,
      "author_id": 717,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 165,
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-14T18:44:29.855Z",
      "course_id": 221,
      "author_id": 718,
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
	-H "Authorization: Bearer 58ebe66f81146e7401fc75a81ea8b468032f6f57ee30d859be5fe9b9f9503a40"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 344ff0a97db44d4df6a4feb07545c58c4ae7c235f89e5bdddfa4295d22aa45b7
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
    "id": 3,
    "course_id": 291,
    "user_id": 906,
    "updated_at": "2016-10-14T18:44:41.161Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 344ff0a97db44d4df6a4feb07545c58c4ae7c235f89e5bdddfa4295d22aa45b7"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 6908fd0d84667a9fbecb3da6ac3637a78f037421eda1dca57db6f30195e66a6b
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
      "id": 6,
      "course_id": 295,
      "user_id": 916,
      "updated_at": "2016-10-14T18:44:41.648Z"
    },
    {
      "id": 7,
      "course_id": 295,
      "user_id": 917,
      "updated_at": "2016-10-14T18:44:41.664Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6908fd0d84667a9fbecb3da6ac3637a78f037421eda1dca57db6f30195e66a6b"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/237/files
Content-Type: application/json
Authorization: Bearer 1353ee4814a0e3151735e5ee1db592ec973c9a6d37e5e105f57e0a5136f1e0b9
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
      "id": 11,
      "uploader": {
        "id": 763,
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
        "created_at": "2016-10-14T18:44:32.954Z",
        "updated_at": "2016-10-14T18:44:32.954Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T18:44:32.961Z",
      "updated_at": "2016-10-14T18:44:32.961Z",
      "course_id": 237,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 12,
      "uploader": {
        "id": 764,
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
        "created_at": "2016-10-14T18:44:32.969Z",
        "updated_at": "2016-10-14T18:44:32.969Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T18:44:32.976Z",
      "updated_at": "2016-10-14T18:44:32.976Z",
      "course_id": 237,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 765,
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
        "created_at": "2016-10-14T18:44:32.984Z",
        "updated_at": "2016-10-14T18:44:32.984Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T18:44:32.991Z",
      "updated_at": "2016-10-14T18:44:32.991Z",
      "course_id": 237,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/237/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1353ee4814a0e3151735e5ee1db592ec973c9a6d37e5e105f57e0a5136f1e0b9"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/235/files
Content-Type: application/json
Authorization: Bearer 1be20727ee1373194b6941c5628a52cf4b39daaba5c135783471f444073f6c47
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
    "id": 10,
    "uploader": {
      "id": 759,
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
      "created_at": "2016-10-14T18:44:32.701Z",
      "updated_at": "2016-10-14T18:44:32.701Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-14T18:44:32.734Z",
    "updated_at": "2016-10-14T18:44:32.734Z",
    "course_id": 235,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/235/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1be20727ee1373194b6941c5628a52cf4b39daaba5c135783471f444073f6c47"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/234/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer ebb5c024b8f72fdb3fdbfd12cb9512bed85db2927170a2070df0563cbbdde91d
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
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/25d5f282d3682c31f26830e4ff369e28.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxOTo0NDozMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8yNWQ1ZjI4MmQzNjgyYzMxZjI2ODMwZTRmZjM2OWUyOC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE0L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxNFQxODQ0MzJaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T184432Z",
    "x-amz-signature": "9b18d88595bf7596aaf397a60e13645b31a6a1cf1ec164b4516b9574beaeffe5"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/234/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebb5c024b8f72fdb3fdbfd12cb9512bed85db2927170a2070df0563cbbdde91d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 0a095321f9d738ac540bc8aa505d7779515e04059cde796eaf48ebf78908e7cf
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
	-H "Authorization: Bearer 0a095321f9d738ac540bc8aa505d7779515e04059cde796eaf48ebf78908e7cf"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e7c4d95cf6ec25ff48ec5a600bb17924ab7e7a23c4c26e0910930c7bb63c29d2
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
	-H "Authorization: Bearer e7c4d95cf6ec25ff48ec5a600bb17924ab7e7a23c4c26e0910930c7bb63c29d2"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e2d8931faed2e066f37e62017d685ca1302a326808ab1561ac0fe727f3593db5
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
	-H "Authorization: Bearer e2d8931faed2e066f37e62017d685ca1302a326808ab1561ac0fe727f3593db5"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4295b65c73f75b29bad70dd36cf18e4f847a0bcc9338e028509e620d61e07156
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
	-H "Authorization: Bearer 4295b65c73f75b29bad70dd36cf18e4f847a0bcc9338e028509e620d61e07156"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fe1d30ed51c725425150bebf9c20465aec8903ba67eff9cba17b3fccb6ceac35
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
	-H "Authorization: Bearer fe1d30ed51c725425150bebf9c20465aec8903ba67eff9cba17b3fccb6ceac35"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 11fae93c4ff1379432b4d153bde1265271318bdb96c95c989372cdf7f60d67b8
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
    "creator_id": 229,
    "id": 70,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 76,
    "additional_university_ids": [

    ],
    "topic_id": 77,
    "discipline_id": 77,
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
    "chapters_updated_at": "2016-10-14T18:43:45.556Z",
    "updated_at": "2016-10-14T18:43:47.192Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 55,
        "title": "Clever Chapter Title 52",
        "position": 1,
        "updated_at": "2016-10-14T18:43:47.139Z",
        "course_id": 70,
        "author_id": 229,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T18:43:45.556Z",
        "questions_updated_at": "2016-10-14T18:43:45.556Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 56,
        "title": "Clever Chapter Title 53",
        "position": 2,
        "updated_at": "2016-10-14T18:43:47.183Z",
        "course_id": 70,
        "author_id": 229,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T18:43:45.556Z",
        "questions_updated_at": "2016-10-14T18:43:45.556Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 230,
        "chapter_id": 55,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:46.963Z",
        "created_at": "2016-10-14T18:43:46.963Z",
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
        "author_id": 230,
        "chapter_id": 56,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:47.041Z",
        "created_at": "2016-10-14T18:43:47.041Z",
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
        "author_id": 230,
        "chapter_id": 55,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:47.008Z",
        "created_at": "2016-10-14T18:43:47.008Z",
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
        "author_id": 230,
        "chapter_id": 56,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:47.085Z",
        "created_at": "2016-10-14T18:43:47.085Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 230,
        "chapter_id": 55,
        "position": 28,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:45.794Z",
        "created_at": "2016-10-14T18:43:45.659Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 230,
        "chapter_id": 55,
        "position": 29,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:45.995Z",
        "created_at": "2016-10-14T18:43:45.866Z",
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
      },
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 230,
        "chapter_id": 56,
        "position": 30,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:46.228Z",
        "created_at": "2016-10-14T18:43:46.087Z",
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
            "id": 78,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 79,
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
        "author_id": 230,
        "chapter_id": 56,
        "position": 31,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:46.436Z",
        "created_at": "2016-10-14T18:43:46.302Z",
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
            "id": 80,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 81,
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
	-H "Authorization: Bearer 11fae93c4ff1379432b4d153bde1265271318bdb96c95c989372cdf7f60d67b8"
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
    "creator_id": 235,
    "id": 71,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 77,
    "additional_university_ids": [

    ],
    "topic_id": 78,
    "discipline_id": 78,
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
    "chapters_updated_at": "2016-10-14T18:43:47.317Z",
    "updated_at": "2016-10-14T18:43:49.016Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 57,
        "title": "Clever Chapter Title 54",
        "position": 1,
        "updated_at": "2016-10-14T18:43:48.964Z",
        "course_id": 71,
        "author_id": 235,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T18:43:47.317Z",
        "questions_updated_at": "2016-10-14T18:43:47.317Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 58,
        "title": "Clever Chapter Title 55",
        "position": 2,
        "updated_at": "2016-10-14T18:43:49.007Z",
        "course_id": 71,
        "author_id": 235,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T18:43:47.317Z",
        "questions_updated_at": "2016-10-14T18:43:47.317Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 235,
        "chapter_id": 57,
        "position": 34,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:47.551Z",
        "created_at": "2016-10-14T18:43:47.411Z",
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
            "id": 86,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 87,
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
        "author_id": 235,
        "chapter_id": 58,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:48.017Z",
        "created_at": "2016-10-14T18:43:47.868Z",
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
            "id": 90,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 91,
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
PUT /v2/courses/69/pin
Content-Type: application/json
Authorization: Bearer c20c98c426fcb60381716471317af372f9fb9b63de53dcab73acd52947747257
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/69/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c20c98c426fcb60381716471317af372f9fb9b63de53dcab73acd52947747257"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/68/pin
Content-Type: application/json
Authorization: Bearer 425ed587fc500d8cd133fd423fb81069dea21bbb7d517f5f0765b02f61918c3e
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/68/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 425ed587fc500d8cd133fd423fb81069dea21bbb7d517f5f0765b02f61918c3e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 238346f7fe38be2337ff3caadea3ad078b325248f0758000ebf3e1695a6065cb
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
    "creator_id": 200,
    "id": 56,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 62,
    "additional_university_ids": [

    ],
    "topic_id": 63,
    "discipline_id": 63,
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
    "updated_at": "2016-10-14T18:43:43.461Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 238346f7fe38be2337ff3caadea3ad078b325248f0758000ebf3e1695a6065cb"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 8b2096ebef887c9871972d199e175ce7813f90f6db60732ce0a8a1aa1dbcc7d1
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
    "id": 188,
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
    "created_at": "2016-10-14T18:43:42.260Z",
    "updated_at": "2016-10-14T18:43:42.260Z",
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
	-H "Authorization: Bearer 8b2096ebef887c9871972d199e175ce7813f90f6db60732ce0a8a1aa1dbcc7d1"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2f92b7de2d9bb84ef413adf52a8dc286a31de61a28c9d9f217fdcecd0a58a097
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[55]}
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
    "id": 189,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      55
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T18:43:42.362Z",
    "updated_at": "2016-10-14T18:43:42.428Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[55]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f92b7de2d9bb84ef413adf52a8dc286a31de61a28c9d9f217fdcecd0a58a097"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer efe6036b12a6cbe4e7fa15530474091f7596a39fa2a35a12eb5261be468f3598
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
    "id": 190,
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
    "created_at": "2016-10-14T18:43:42.450Z",
    "updated_at": "2016-10-14T18:43:42.450Z",
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
	-H "Authorization: Bearer efe6036b12a6cbe4e7fa15530474091f7596a39fa2a35a12eb5261be468f3598"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a4ecb5741bcd114a00a76f5c21b891d7729a7478571963e126f40e7964cae0f2
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[57]}
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
    "id": 191,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      57
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T18:43:42.546Z",
    "updated_at": "2016-10-14T18:43:42.546Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[57]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4ecb5741bcd114a00a76f5c21b891d7729a7478571963e126f40e7964cae0f2"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b753f455a238f08043829214358445809fc83934e4708c74c0ad72a4ad9847c2
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

59
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
    "id": 193,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/116d6e6473721306d7bd971744f0a276e571e026.jpg",
    "university_id": null,
    "fields_of_study": [
      59
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T18:43:42.696Z",
    "updated_at": "2016-10-14T18:43:42.975Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/040f241fb71378fc74f12235b8530cce6a73dbde.jpg",
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

59
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b753f455a238f08043829214358445809fc83934e4708c74c0ad72a4ad9847c2"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 0ece358d852e80f551755b0b938c6a5de805967638f650d216f8c675375624b1
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
	-H "Authorization: Bearer 0ece358d852e80f551755b0b938c6a5de805967638f650d216f8c675375624b1"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 77f42ab25fff4f4ef919d9653c9e04f1a645c6b80ff4328f7a980576474b4afc
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
	-H "Authorization: Bearer 77f42ab25fff4f4ef919d9653c9e04f1a645c6b80ff4328f7a980576474b4afc"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a133fb11701f03f2ef28934ca5178bc32039bbc1f14e37979b8817b7edf5f5d4
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
	-H "Authorization: Bearer a133fb11701f03f2ef28934ca5178bc32039bbc1f14e37979b8817b7edf5f5d4"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 4b70197854e61c20b38bfc4b1c567fba039e58a94dbc25897c48b2bd383fb3f7
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
      "creator_id": 302,
      "id": 82,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-60",
      "html_url": "https://goskive.com/course/mit-course-60",
      "slug": "mit-course-60",
      "university_id": 88,
      "additional_university_ids": [

      ],
      "topic_id": 89,
      "discipline_id": 89,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 60",
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
      "updated_at": "2016-10-14T18:43:57.454Z",
      "shortname": "mit-course-60"
    },
    {
      "creator_id": 303,
      "id": 83,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-61",
      "html_url": "https://goskive.com/course/mit-course-61",
      "slug": "mit-course-61",
      "university_id": 89,
      "additional_university_ids": [

      ],
      "topic_id": 90,
      "discipline_id": 90,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
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
      "updated_at": "2016-10-14T18:43:57.544Z",
      "shortname": "mit-course-61"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b70197854e61c20b38bfc4b1c567fba039e58a94dbc25897c48b2bd383fb3f7"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer c47966ea26f843ccfe17dc5ae16876157aa7a12eeecc2eea9780d4c0d49cd847
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
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T18:44:06.144Z"
      },
      "created_at": "2016-10-14T18:44:06.147Z",
      "updated_at": "2016-10-14T18:44:06.147Z",
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
        "name": "Fake Company Name 30",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T18:44:06.156Z"
      },
      "created_at": "2016-10-14T18:44:06.159Z",
      "updated_at": "2016-10-14T18:44:06.159Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c47966ea26f843ccfe17dc5ae16876157aa7a12eeecc2eea9780d4c0d49cd847"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 122efe742a57b6837aac4ed0f1e80ce29264211b16e3dab690d8b97de4cafa5e
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
      "company_id": 29,
      "company": {
        "id": 29,
        "name": "Fake Company Name 25",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/eb30fd9939333e805126ba26a8736769f7ca2ba6.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T18:44:05.918Z"
      },
      "created_at": "2016-10-14T18:44:05.923Z",
      "updated_at": "2016-10-14T18:44:05.923Z",
      "score": 0.0
    },
    {
      "id": 2,
      "title": "Job Posting2",
      "description": "A Dream Job at a Dream Company!",
      "category": "Dream Jobs",
      "department": "Dream Department",
      "city_name": null,
      "image_url": "http://company.com/dream_job.jpg",
      "target_url": "http://company.com/dream_job",
      "pdf_url": "http://company.com/dream_job.pdf",
      "screens": [

      ],
      "company_id": 30,
      "company": {
        "id": 30,
        "name": "Fake Company Name 26",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T18:44:05.936Z"
      },
      "created_at": "2016-10-14T18:44:05.939Z",
      "updated_at": "2016-10-14T18:44:05.939Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 122efe742a57b6837aac4ed0f1e80ce29264211b16e3dab690d8b97de4cafa5e"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer b05f35b4bc40011e7e3062ec706efeb6d5475538e7f385065cfe5d27b2d2b89d
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
      "id": 17,
      "created_at": "2016-10-14T18:44:37.578Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-10-14T18:44:37.697Z",
      "author_id": "863",
      "thread_subject_id": "279",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 18,
      "created_at": "2016-10-14T18:44:37.684Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-10-14T18:44:37.701Z",
      "author_id": "866",
      "thread_subject_id": "280",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-10-14T18:44:38.104Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 20,
      "updated_at": "2016-10-14T18:44:38.104Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-10-14T18:44:38.545Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-10-14T18:44:38.545Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 21,
      "created_at": "2016-10-14T18:44:38.966Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-10-14T18:44:38.966Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 22,
      "created_at": "2016-10-14T18:44:39.282Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 121,
      "updated_at": "2016-10-14T18:44:39.282Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-10-14T18:44:39.590Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 122,
      "updated_at": "2016-10-14T18:44:39.590Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-10-14T18:44:39.891Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 123,
      "updated_at": "2016-10-14T18:44:39.891Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b05f35b4bc40011e7e3062ec706efeb6d5475538e7f385065cfe5d27b2d2b89d"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/25
Content-Type: application/json
Authorization: Bearer 2f175083f372fee1c6e41359355d549cd98b485adec28cae096eda13ae6338ed
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-14T18:34:39.000Z"}}
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
    "id": 25,
    "created_at": "2016-10-14T18:44:40.027Z",
    "read_at": "2016-10-14T18:34:39.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 57,
    "updated_at": "2016-10-14T18:44:40.067Z",
    "author_id": "891",
    "thread_subject_id": "287",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/25" -d '{"notification":{"read_at":"2016-10-14T18:34:39.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f175083f372fee1c6e41359355d549cd98b485adec28cae096eda13ae6338ed"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b6615ef05a1d23406d5b6385ad24a5c5214c1ec1d1231e1f8f4b6b81159fefca
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
      "id": 5,
      "course_id": 90,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T18:44:01.532Z",
      "course_published": true,
      "updated_at": "2016-10-14T18:44:01.523Z"
    },
    {
      "id": 6,
      "course_id": 91,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T18:44:01.622Z",
      "course_published": true,
      "updated_at": "2016-10-14T18:44:01.614Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6615ef05a1d23406d5b6385ad24a5c5214c1ec1d1231e1f8f4b6b81159fefca"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 2964e10c308efa7652d90458e87a9c34c5463d4ebfe41b28c48fda0e0c1f9058
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
    "course_id": 94,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T18:44:01.992Z",
    "course_published": true,
    "updated_at": "2016-10-14T18:44:01.984Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2964e10c308efa7652d90458e87a9c34c5463d4ebfe41b28c48fda0e0c1f9058"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer d832cdf58ecdfbf3e487d28e3cbbe0fc80e5e737a2eea5ff94d106b0451d45b0
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
    "id": 4,
    "course_id": 89,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-14T18:44:01.369Z",
    "course_published": true,
    "updated_at": "2016-10-14T18:44:01.357Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d832cdf58ecdfbf3e487d28e3cbbe0fc80e5e737a2eea5ff94d106b0451d45b0"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f31d80aad2829219dc80cd7ca886e9a8375d6674288b69cddafa12deba14ae98
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
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 69,
      "user_id": 307
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 70,
      "user_id": 307
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 71,
      "user_id": 307
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 72,
      "user_id": 307
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f31d80aad2829219dc80cd7ca886e9a8375d6674288b69cddafa12deba14ae98"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/121
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
    "id": 121,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 119,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 121
      },
      {
        "id": 120,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 121
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/121" -X GET \
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
      "id": 119,
      "name": "Front-line uniform challenge",
      "name_translations": {
        "en": "Front-line uniform challenge"
      }
    },
    {
      "id": 120,
      "name": "Visionary clear-thinking adapter",
      "name_translations": {
        "en": "Visionary clear-thinking adapter"
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
PATCH /v2/feedbacks/25/close
Content-Type: application/json
Authorization: Bearer 5fe56754b38a38395fd5ebe0b99d24141a88d91573a1375b1ae3bdd0438d4b7d
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
    "id": 25,
    "user_id": 441,
    "feedbackable_id": 51,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-14T18:44:10.086Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fe56754b38a38395fd5ebe0b99d24141a88d91573a1375b1ae3bdd0438d4b7d"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer 72621d1e42dc0e4876e5fc486ffc1a2d416213a51170b4cd6de5eecc11304c12
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
    "id": 23,
    "user_id": 431,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-14T18:44:09.354Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72621d1e42dc0e4876e5fc486ffc1a2d416213a51170b4cd6de5eecc11304c12"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer bc50b3680a35048130eb1b97ed57270140047a589bde981a7c52e86c18183d6d
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
    "id": 19,
    "user_id": 409,
    "feedbackable_id": 45,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T18:44:08.454Z",
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
curl "api.goskive.com/v2/feedbacks/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc50b3680a35048130eb1b97ed57270140047a589bde981a7c52e86c18183d6d"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer d8b89dca1f19d76e662d68b970eb7c7a8fe6d218ef4deda2be8e3432e5d54379
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
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8b89dca1f19d76e662d68b970eb7c7a8fe6d218ef4deda2be8e3432e5d54379"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer db8753c4bb368f4a7a08f9768ba6a9b0005f2ded0a003b0d4ce56c86c11309f2
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
curl "api.goskive.com/v2/feedbacks/22/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db8753c4bb368f4a7a08f9768ba6a9b0005f2ded0a003b0d4ce56c86c11309f2"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer bde17a3ee037c5fe5b5a2c0818ed6a9673a10935b42be1e247cea49b6f84b569
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
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bde17a3ee037c5fe5b5a2c0818ed6a9673a10935b42be1e247cea49b6f84b569"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 8bc550c8ea8f1b77163b751b99078766d80bfb1bdf0b443c65f266a9e5203796
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
    "id": 20,
    "user_id": 414,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T18:44:08.742Z",
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
curl "api.goskive.com/v2/feedbacks/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8bc550c8ea8f1b77163b751b99078766d80bfb1bdf0b443c65f266a9e5203796"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/3
Authorization: Bearer 271c8ffbee50aece406aef64ebae1734613f402ab4c01edd10f68fcff04bdbed
Content-Type: application/x-www-form-urlencoded
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
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Authorization: Bearer 271c8ffbee50aece406aef64ebae1734613f402ab4c01edd10f68fcff04bdbed" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer c5866b8f7ead3edbf72be0e62ea9f3f1db3c941166d7f085349e8840ccd21c86
Content-Type: application/x-www-form-urlencoded
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Authorization: Bearer c5866b8f7ead3edbf72be0e62ea9f3f1db3c941166d7f085349e8840ccd21c86" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/6
Authorization: Bearer 89895f698dbd3c2d8d45db33b7ae24f429d5d2be677c15001a028d6c0a7c7c45
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/48f7e2061e0251f1a88d13480acdf3a2.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T184403Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=dc90dde91c6bed9864be1fc944dc46b3752a9da092d277a114ad5819bf0ccafa"
  }
}
```



```shell
curl "api.goskive.com/v2/files/6" -X GET \
	-H "Authorization: Bearer 89895f698dbd3c2d8d45db33b7ae24f429d5d2be677c15001a028d6c0a7c7c45"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer bcac4ce769f827a3875f705bad6e49e5028fa204abc804fc2e6f9fc220bba6fd
Content-Type: application/json
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
    "id": 7,
    "uploader": {
      "id": 363,
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
      "created_at": "2016-10-14T18:44:03.100Z",
      "updated_at": "2016-10-14T18:44:03.100Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-14T18:44:03.174Z",
    "updated_at": "2016-10-14T18:44:03.174Z",
    "course_id": 102,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Authorization: Bearer bcac4ce769f827a3875f705bad6e49e5028fa204abc804fc2e6f9fc220bba6fd" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer 27bbf9f2cd6407f769a4f821ed5e44f38cfb91091a6120edfa28c171248a5279
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
      "creator_id": 666,
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "topic_id": 219,
      "discipline_id": 220,
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
      "chapters_updated_at": "2016-10-14T18:44:25.158Z",
      "updated_at": "2016-10-14T18:44:26.853Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 671,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-ce1ccedc-04ae-4ee2-b5af-3342d3579d30",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-ce1ccedc-04ae-4ee2-b5af-3342d3579d30",
      "slug": "mit-the-great-british-bake-off-ce1ccedc-04ae-4ee2-b5af-3342d3579d30",
      "university_id": 192,
      "additional_university_ids": [

      ],
      "topic_id": 220,
      "discipline_id": 221,
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
      "chapters_updated_at": "2016-10-14T18:44:25.158Z",
      "updated_at": "2016-10-14T18:44:27.424Z",
      "shortname": "mit-the-great-british-bake-off-ce1ccedc-04ae-4ee2-b5af-3342d3579d30"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/8/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 27bbf9f2cd6407f769a4f821ed5e44f38cfb91091a6120edfa28c171248a5279"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/1/preview
Authorization: Bearer 3632ffcd6f1c47ff974e6117ee27374003b014fde022c5e3d6f5fe2018919534
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/863a3676a4edf9c3260feb9720d47061.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T184402Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=ac40ad374e94d2f2c49792f448beb79b2e3f17da58594ab09ca6c12fde0c2166"
  }
}
```



```shell
curl "api.goskive.com/v2/files/1/preview" -X GET \
	-H "Authorization: Bearer 3632ffcd6f1c47ff974e6117ee27374003b014fde022c5e3d6f5fe2018919534"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/2/report
Authorization: Bearer 7a0e70e56e52698fc5a99cbabbb7ffb663bcd62da1370e9f877db40150931d5d
Content-Type: application/x-www-form-urlencoded
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
	-H "Authorization: Bearer 7a0e70e56e52698fc5a99cbabbb7ffb663bcd62da1370e9f877db40150931d5d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/14/comments
Content-Type: application/json
Authorization: Bearer a16b69e06203c4d11f3760a4fd6564eb68cbd24c30616869e7a7b05fdaf494ed
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
    "id": 8,
    "author_id": 174,
    "reply_to_id": null,
    "created_at": "2016-10-14T18:43:41.555Z",
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
curl "api.goskive.com/v2/flashcards/14/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a16b69e06203c4d11f3760a4fd6564eb68cbd24c30616869e7a7b05fdaf494ed"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer 83e2f33007067a4a1ba62a401973a9c675a8482f08f15ffb2b02f5a5a9252fb9
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
    "id": 7,
    "author_id": 171,
    "reply_to_id": null,
    "created_at": "2016-10-14T18:43:41.238Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 171,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:41.235Z",
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
curl "api.goskive.com/v2/flashcards/13/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83e2f33007067a4a1ba62a401973a9c675a8482f08f15ffb2b02f5a5a9252fb9"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/16/comments
Content-Type: application/json
Authorization: Bearer f899abaf6125892dd6c7503d2599d2ae1dead9f7bd02c9fa38d1712f99ac4c56
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
      "id": 10,
      "author_id": 184,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:43:42.045Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 183,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:43:42.030Z",
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
curl "api.goskive.com/v2/flashcards/16/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f899abaf6125892dd6c7503d2599d2ae1dead9f7bd02c9fa38d1712f99ac4c56"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/15/comments
Content-Type: application/json
Authorization: Bearer 51d135facd997f05f71b81342879ce92124be3f44cc98ee13584a6653630ba0b
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
curl "api.goskive.com/v2/flashcards/15/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51d135facd997f05f71b81342879ce92124be3f44cc98ee13584a6653630ba0b"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/feedbacks
Content-Type: application/json
Authorization: Bearer cc8b33fade3c0209ab537b0fe1984c9b26a14c634f3d15e02e0ec70599f0e59a
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
    "id": 2,
    "user_id": 42,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T18:43:29.710Z",
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
	-H "Authorization: Bearer cc8b33fade3c0209ab537b0fe1984c9b26a14c634f3d15e02e0ec70599f0e59a"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/6/feedbacks
Content-Type: application/json
Authorization: Bearer 89e93b7adb327679e3adfd6037597edb921ddf4c56db4ec7f30b7e304b758e2e
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
      "id": 7,
      "user_id": 69,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:31.037Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 68,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:31.026Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/6/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89e93b7adb327679e3adfd6037597edb921ddf4c56db4ec7f30b7e304b758e2e"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/90/votes
Content-Type: application/json
Authorization: Bearer 69e4c56a8f3e1fccdbed313cb4cadfb5bfd06704cb94f3641320a19b66970359
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
      "votable_id": 90,
      "user_id": 747
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 90,
      "user_id": 746
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 90,
      "user_id": 745
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/90/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69e4c56a8f3e1fccdbed313cb4cadfb5bfd06704cb94f3641320a19b66970359"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/59/republish
Content-Type: application/json
Authorization: Bearer c44e00799882cf1179f27f19f569506ce47ea6b1c667a66c4398f33aa6c599f2
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
curl "api.goskive.com/v2/flashcards/59/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c44e00799882cf1179f27f19f569506ce47ea6b1c667a66c4398f33aa6c599f2"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/bookmark
Content-Type: application/json
Authorization: Bearer 0269a9724b98c0cfd1c87a08b65b64ecd1eff989f12e276375e450b609f44986
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0269a9724b98c0cfd1c87a08b65b64ecd1eff989f12e276375e450b609f44986"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/58
Content-Type: application/json
Authorization: Bearer 5ee47989f65870077916a67de6d7ca4443f5d3d314cbff35f6f0cce47bafe0b1
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ee47989f65870077916a67de6d7ca4443f5d3d314cbff35f6f0cce47bafe0b1"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/downvote
Content-Type: application/json
Authorization: Bearer 20796d8fdfca70d3e3824c81b78ca43840de96c34b5c0b1bfc764da9d0a90cb4
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
	-H "Authorization: Bearer 20796d8fdfca70d3e3824c81b78ca43840de96c34b5c0b1bfc764da9d0a90cb4"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/66
Content-Type: application/json
Authorization: Bearer 02d13dc6b2fc8f52e91aa20bbdac939be9510696b1305d17d2de61206b77aa05
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 603,
    "chapter_id": 128,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:44:22.785Z",
    "created_at": "2016-10-14T18:44:22.785Z",
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
curl "api.goskive.com/v2/flashcards/66" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02d13dc6b2fc8f52e91aa20bbdac939be9510696b1305d17d2de61206b77aa05"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/report
Content-Type: application/json
Authorization: Bearer 877c14b327e099ce99ffe488a66737a9ca86e2b7cadb54f116b757341c0621bf
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 877c14b327e099ce99ffe488a66737a9ca86e2b7cadb54f116b757341c0621bf"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/62/bookmark
Content-Type: application/json
Authorization: Bearer 349bf0a1690fd7987e19619dd7498e2dd985acefc34558180278d55e56ee7a04
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/62/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 349bf0a1690fd7987e19619dd7498e2dd985acefc34558180278d55e56ee7a04"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/61/upvote
Content-Type: application/json
Authorization: Bearer e4efe98250fa50dc70ffb4ac5569b0a61bb89e04bb3e56e23c59f8a825a8b921
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4efe98250fa50dc70ffb4ac5569b0a61bb89e04bb3e56e23c59f8a825a8b921"
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
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/83c12eb138d06412bf0433104ab6a40c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxOTo0Mzo0MloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS84M2MxMmViMTM4ZDA2NDEyYmYwNDMzMTA0YWI2YTQwYy5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE0L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxNFQxODQzNDJaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T184342Z",
    "x-amz-signature": "d1c8463177b6c53e66978aceeb2d8527e26d56a9119e2a0cd52f2556c050e075"
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
Authorization: Bearer 61671f2e68312f05759a26de3fc69278e776f4ba005b2f22641d5f15282ffa62
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
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61671f2e68312f05759a26de3fc69278e776f4ba005b2f22641d5f15282ffa62"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer ca1834aee31f9ad1d05fa56330e666152abc211302fb4d56a4650c080ff14df5
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
curl "api.goskive.com/v2/me/jobs/9/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca1834aee31f9ad1d05fa56330e666152abc211302fb4d56a4650c080ff14df5"
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
{"password":{"reset_password_token":"9nz5qFFqNVTQQgrzCwj5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 328,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-14T18:44:01.013Z",
  "updated_at": "2016-10-14T18:44:01.176Z",
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
  "audit_id": 3771
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"9nz5qFFqNVTQQgrzCwj5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/6/comments
Content-Type: application/json
Authorization: Bearer fe9f1718c159327c6b8244dd55e8931a44d5f672e2801cc639a1934f3698fd6f
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
    "id": 3,
    "author_id": 25,
    "reply_to_id": null,
    "created_at": "2016-10-14T18:43:27.521Z",
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
curl "api.goskive.com/v2/questions/6/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe9f1718c159327c6b8244dd55e8931a44d5f672e2801cc639a1934f3698fd6f"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/7/comments
Content-Type: application/json
Authorization: Bearer eebdd58a57327c15a9f1bdce5f80a9de310be74b234df8b62e431f215528030b
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
    "id": 4,
    "author_id": 28,
    "reply_to_id": null,
    "created_at": "2016-10-14T18:43:28.224Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 28,
      "feedbackable_id": 7,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:28.220Z",
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
curl "api.goskive.com/v2/questions/7/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eebdd58a57327c15a9f1bdce5f80a9de310be74b234df8b62e431f215528030b"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/5/comments
Content-Type: application/json
Authorization: Bearer f00bdfa4dda29ea601bb0bacbfbada9774d62c9837f4b3bcdd098dacfca5a2d1
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
      "id": 1,
      "author_id": 23,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:43:27.150Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 24,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:43:27.181Z",
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
curl "api.goskive.com/v2/questions/5/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f00bdfa4dda29ea601bb0bacbfbada9774d62c9837f4b3bcdd098dacfca5a2d1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/8/comments
Content-Type: application/json
Authorization: Bearer 883b8ad332686c6210ca0999ca8ad361a5abbfeba652edfc9608f0f491b6f036
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
curl "api.goskive.com/v2/questions/8/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 883b8ad332686c6210ca0999ca8ad361a5abbfeba652edfc9608f0f491b6f036"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/68/feedbacks
Content-Type: application/json
Authorization: Bearer 862421e4a339fb12ef90abc40d01ce79c73aeebf9637fe7cda30c48e565459cd
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
    "id": 18,
    "user_id": 294,
    "feedbackable_id": 68,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-14T18:43:56.831Z",
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
curl "api.goskive.com/v2/questions/68/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 862421e4a339fb12ef90abc40d01ce79c73aeebf9637fe7cda30c48e565459cd"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/64/feedbacks
Content-Type: application/json
Authorization: Bearer 2f9bd7945c4c6127b0be99cb849eaaafba2ac8c2fa13e4bafe461e20f5261779
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
      "id": 14,
      "user_id": 282,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:55.047Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 281,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:55.035Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/64/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f9bd7945c4c6127b0be99cb849eaaafba2ac8c2fa13e4bafe461e20f5261779"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/1/votes
Content-Type: application/json
Authorization: Bearer 4fb405f0e8bae7811d8f3f016ac8f6f216b4152f29b3602e448714d4f170d33a
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
	-H "Authorization: Bearer 4fb405f0e8bae7811d8f3f016ac8f6f216b4152f29b3602e448714d4f170d33a"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/11/republish
Content-Type: application/json
Authorization: Bearer 1b2bfc4b0e9d27b3b9248b72c3a6018ad859acc6658f465d6b6072ad96cf2ee7
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
curl "api.goskive.com/v2/questions/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b2bfc4b0e9d27b3b9248b72c3a6018ad859acc6658f465d6b6072ad96cf2ee7"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/31/bookmark
Content-Type: application/json
Authorization: Bearer f1a0b231ff128ef5f7eec022013400a1addf1fb47cb5f34b6753460ad81a1bfa
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1a0b231ff128ef5f7eec022013400a1addf1fb47cb5f34b6753460ad81a1bfa"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/12
Content-Type: application/json
Authorization: Bearer 73e6de9e96d0e420323eb72ad0c5b70bb4af6586215d69f5269216a390cc0245
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73e6de9e96d0e420323eb72ad0c5b70bb4af6586215d69f5269216a390cc0245"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/33/downvote
Content-Type: application/json
Authorization: Bearer 45920f4a465077591e7064ae7b9ec2637733c09fb5871e253ca97b19a6cfd02e
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/33/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45920f4a465077591e7064ae7b9ec2637733c09fb5871e253ca97b19a6cfd02e"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/13
Content-Type: application/json
Authorization: Bearer 316cd70f6264d0069291c98b54d8fb1dd2207f20385f7e8bdaaeb6f8a13657be
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 90,
    "chapter_id": 21,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:43:33.305Z",
    "created_at": "2016-10-14T18:43:33.185Z",
    "tags": [
      {
        "id": 8,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 7,
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
        "id": 25,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 26,
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
curl "api.goskive.com/v2/questions/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 316cd70f6264d0069291c98b54d8fb1dd2207f20385f7e8bdaaeb6f8a13657be"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/29/report
Content-Type: application/json
Authorization: Bearer 698cbf3e5a742507c25402ea9279350a359e40ceb72ae7092407ad4218a8509c
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/29/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 698cbf3e5a742507c25402ea9279350a359e40ceb72ae7092407ad4218a8509c"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/9/bookmark
Content-Type: application/json
Authorization: Bearer d01892078a451200cec90f3313084cf3ae1370ae9865df2dfaab419ee243e214
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/9/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d01892078a451200cec90f3313084cf3ae1370ae9865df2dfaab419ee243e214"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/32
Content-Type: application/json
Authorization: Bearer 48b9afce902a24b3835cd73c9a1cd2193244aa53a6327f45ee6e1414f0705252
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T18:43:39.349Z","updated_at":"2016-10-14T18:43:39.479Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":40,"author_id":152,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 152,
    "chapter_id": 40,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T18:43:39.590Z",
    "created_at": "2016-10-14T18:43:39.349Z",
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
    "question": "{\"id\"=>32, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-14T18:43:39.349Z\", \"updated_at\"=>\"2016-10-14T18:43:39.479Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>40, \"author_id\"=>152, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 63,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 64,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 65,
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
curl "api.goskive.com/v2/questions/32" -d '{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T18:43:39.349Z","updated_at":"2016-10-14T18:43:39.479Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":40,"author_id":152,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48b9afce902a24b3835cd73c9a1cd2193244aa53a6327f45ee6e1414f0705252"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/30/upvote
Content-Type: application/json
Authorization: Bearer f17eba340dd31e8f536f8c7d92fee9388638428405b5c54679b96b26d4e121c9
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/30/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f17eba340dd31e8f536f8c7d92fee9388638428405b5c54679b96b26d4e121c9"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7f117a7e52fa9beffafa3282e2c2699a4dd9c6de85e9899dfc86ac29035ccea0
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
      "creator_id": 753,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "topic_id": 243,
      "discipline_id": 244,
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
      "updated_at": "2016-10-14T18:44:32.282Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f117a7e52fa9beffafa3282e2c2699a4dd9c6de85e9899dfc86ac29035ccea0"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer eb9a7277b93ca57abdc1e0b2722108d85d191e70b71afe02c5cd576a9baa7f31
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
      "id": 215,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-195",
      "html_url": "https://goskive.com/university/uni-195",
      "slug": "uni-195",
      "name": "National School of Pizza",
      "short_name": "Uni 195",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/01fa4d063f9dcdd8de74fbee940bd3d5be1e97eb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/899bdee5fe1909868aae15fc75d04a4125a1dead.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T18:44:32.110Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 214,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-194",
      "html_url": "https://goskive.com/university/uni-194",
      "slug": "uni-194",
      "name": "National School of Pastry",
      "short_name": "Uni 194",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8efdb8264c7f4a28df19e2f795afb7290e8efd49.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ad9fd4421755460f2afe46727848c3fa475fafa0.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T18:44:32.092Z",
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
	-H "Authorization: Bearer eb9a7277b93ca57abdc1e0b2722108d85d191e70b71afe02c5cd576a9baa7f31"
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
      "id": 117,
      "name": "Upgradable empowering hub",
      "name_translations": {
        "en": "Upgradable empowering hub"
      },
      "discipline_id": 117
    },
    {
      "id": 118,
      "name": "Balanced analyzing framework",
      "name_translations": {
        "en": "Balanced analyzing framework"
      },
      "discipline_id": 118
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
GET /v2/topics/116
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
    "id": 116,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 116
  }
}
```



```shell
curl "api.goskive.com/v2/topics/116" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer b72cebd8942fb425c0698b7492bf06205de6bd6b8fba4d2c449e4dd43c16dcfc
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
      "id": 6,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-4",
      "html_url": "https://goskive.com/university/uni-4",
      "slug": "uni-4",
      "name": "University 4",
      "short_name": "Uni 4",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe1a82f0ac557b999bf5a6b1a0cb87e1a6833cb0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/dc7090e68b98e4b6195de2af1177270dca8a9cfc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T18:43:26.469Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 7,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-5",
      "html_url": "https://goskive.com/university/uni-5",
      "slug": "uni-5",
      "name": "University 5",
      "short_name": "Uni 5",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/78bc87f167212793f65ef23fb795957bf12d7279.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/72904deab5c9c5f628bf957d93b468b0ce156dff.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T18:43:26.485Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 8,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-6",
      "html_url": "https://goskive.com/university/uni-6",
      "slug": "uni-6",
      "name": "University 6",
      "short_name": "Uni 6",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dfe35e4e2ca3912e737667f9f1b65820be0620bd.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c9be80ebafe25e4b31c8faf14a17ae62999885f7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T18:43:26.502Z",
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
	-H "Authorization: Bearer b72cebd8942fb425c0698b7492bf06205de6bd6b8fba4d2c449e4dd43c16dcfc"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1b1d951017aa9085489d5d52c5b77981986537be7ed76bdb3b7cd95af7a3fe3a
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
    "id": 4,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-14T18:43:26.294Z",
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
	-H "Authorization: Bearer 1b1d951017aa9085489d5d52c5b77981986537be7ed76bdb3b7cd95af7a3fe3a"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c96dd7c20bf8648412dd83e2556ac2b0c96dfcc5e6f126174dbc270b57496813
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":154,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 535,
    "id": 142,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 148,
    "additional_university_ids": [

    ],
    "topic_id": 154,
    "discipline_id": 155,
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
    "chapters_updated_at": "2016-10-14T18:44:16.790Z",
    "updated_at": "2016-10-14T18:44:16.928Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 113,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-14T18:44:16.882Z",
        "course_id": 142,
        "author_id": 535,
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
        "id": 114,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-14T18:44:16.901Z",
        "course_id": 142,
        "author_id": 535,
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
        "id": 115,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-14T18:44:16.918Z",
        "course_id": 142,
        "author_id": 535,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":154,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c96dd7c20bf8648412dd83e2556ac2b0c96dfcc5e6f126174dbc270b57496813"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 04ca45493da86674cbabd7506b0e52735888bb7fa55e78bd55c91ba1b0495082
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":155,"published":false}}
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
    "creator_id": 536,
    "id": 143,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 149,
    "additional_university_ids": [

    ],
    "topic_id": 155,
    "discipline_id": 156,
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
    "updated_at": "2016-10-14T18:44:17.077Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":155,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04ca45493da86674cbabd7506b0e52735888bb7fa55e78bd55c91ba1b0495082"
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
      "creator_id": 543,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 163,
      "discipline_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
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
      "updated_at": "2016-10-14T18:44:17.741Z",
      "shortname": "fu-course-119"
    },
    {
      "creator_id": 543,
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 164,
      "discipline_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 120",
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
      "chapters_updated_at": "2016-10-14T18:44:18.035Z",
      "updated_at": "2016-10-14T18:44:18.041Z",
      "shortname": "fu-course-120"
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
Authorization: Bearer 200298af03e6330938c3da5ffbe2d3020b1056bd40819a0999f2eb4887ad10d6
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
      "creator_id": 550,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 171,
      "discipline_id": 172,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-10-14T18:44:18.480Z",
      "shortname": "fu-course-127"
    },
    {
      "creator_id": 550,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 172,
      "discipline_id": 173,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
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
      "chapters_updated_at": "2016-10-14T18:44:18.770Z",
      "updated_at": "2016-10-14T18:44:18.777Z",
      "shortname": "fu-course-128"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 200298af03e6330938c3da5ffbe2d3020b1056bd40819a0999f2eb4887ad10d6"
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
      "creator_id": 548,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 167,
      "discipline_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "updated_at": "2016-10-14T18:44:18.256Z",
      "shortname": "fu-course-123"
    },
    {
      "creator_id": 548,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-124",
      "html_url": "https://goskive.com/course/fu-course-124",
      "slug": "fu-course-124",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 168,
      "discipline_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 124",
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
      "updated_at": "2016-10-14T18:44:18.298Z",
      "shortname": "fu-course-124"
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
Authorization: Bearer 6a0c458cd63e9844552800c4183b9860d15d2db02f16d132225bd80196bd4a0e
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
      "creator_id": 556,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "topic_id": 175,
      "discipline_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
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
      "updated_at": "2016-10-14T18:44:19.009Z",
      "shortname": "fu-course-131"
    },
    {
      "creator_id": 556,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "updated_at": "2016-10-14T18:44:19.061Z",
      "shortname": "fu-course-132"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a0c458cd63e9844552800c4183b9860d15d2db02f16d132225bd80196bd4a0e"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 22e79996652768b6a617fef2ae1fd8d0dbaef9927b1bba74b9dc28d1c397ce7d
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
  "id": 366,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-14T18:44:03.266Z",
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
	-H "Authorization: Bearer 22e79996652768b6a617fef2ae1fd8d0dbaef9927b1bba74b9dc28d1c397ce7d"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/196
Content-Type: application/json
Authorization: Bearer 18a8b194aaeb5cb14c60e8456f768c1120f1748efcefd197ac207f210ef60ef7
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
    "id": 196,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 60,
    "fields_of_study": [
      60,
      61
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-14T18:43:43.147Z",
    "updated_at": "2016-10-14T18:43:43.147Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/196" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18a8b194aaeb5cb14c60e8456f768c1120f1748efcefd197ac207f210ef60ef7"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/194
Content-Type: application/json
Authorization: Bearer 8f303dd25391ef6c78f5767057e8613cd42951574886cccc264c80278569f585
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
    "id": 194,
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
    "created_at": "2016-10-14T18:43:43.003Z",
    "updated_at": "2016-10-14T18:43:43.003Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/194" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f303dd25391ef6c78f5767057e8613cd42951574886cccc264c80278569f585"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/11
Content-Type: application/json
Authorization: Bearer c7378b8915263d432a7cb2d0fbb1817e9fa0c9ab7596b528610df66cc19f407c
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7378b8915263d432a7cb2d0fbb1817e9fa0c9ab7596b528610df66cc19f407c"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer cc52304c5d6414a43db27fd313bc72e72cab3e606ff036a6001029c5416cf20c
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
    "votable_id": 82,
    "user_id": 399
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc52304c5d6414a43db27fd313bc72e72cab3e606ff036a6001029c5416cf20c"
```
