---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"f684b8152cfb1b4b963a6c2c68ca41bbf34a2d555dd82b9fae9b25c1775e0565","client_secret":"feaeeda6c1dfb45417a3889bb26104bac73c907b97e3e728ea228581181d950e"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"f684b8152cfb1b4b963a6c2c68ca41bbf34a2d555dd82b9fae9b25c1775e0565","client_secret":"feaeeda6c1dfb45417a3889bb26104bac73c907b97e3e728ea228581181d950e"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MGUwODBhYjNhOGMwZDQyYWUyYzQwYWQ5ZmVjMTYzNWVkM2MzZDdmNmUzNGFm
YjkzNjhiOWY4MDkwNzBmMjgxZjowMmE1YmMyODk3YWIxMzllNmEyMzU1NmE5
NWFlMTVhNzgxZWMwOWU1NWQ1NWVhZWJlZjRmODA4ODA0MTEyN2Yx

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
	-u 0e080ab3a8c0d42ae2c40ad9fec1635ed3c3d7f6e34afb9368b9f809070f281f:02a5bc2897ab139e6a23556a95ae15a781ec09e55d55eaebef4f8088041127f1
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
{"grant_type":"client_credentials","client_id":"27a5ae6ea5c266759152858b475e9e292346a1d6dbfc06a89bcdb381482efe18","client_secret":"2bc05ce5fa5f6d8e954609a6809c4b3e19d2b3fa630f1783d7ee24e1c07e5a59"}
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
  "access_token": "e92a8cfe998f39c71c833d1e0fd1f0d8b100dd20efcfe4d963f7a3951e87279c",
  "token_type": "bearer",
  "created_at": 1481822388
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"27a5ae6ea5c266759152858b475e9e292346a1d6dbfc06a89bcdb381482efe18","client_secret":"2bc05ce5fa5f6d8e954609a6809c4b3e19d2b3fa630f1783d7ee24e1c07e5a59"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e20d3878405dea19837e2d1a1e9de097e6da17f4c11d5684398c6363ce2b5db0","client_secret":"10cc9cd6bbc2e70af50e4ef6ae7d440e220be7b1cbb53f96a9309f7d2d7e3b11"}
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
  "access_token": "50c949bc42045a081a35abe9c261177ec68f27640ad4537171c1ad437da7fc47",
  "token_type": "bearer",
  "created_at": 1481822388
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e20d3878405dea19837e2d1a1e9de097e6da17f4c11d5684398c6363ce2b5db0","client_secret":"10cc9cd6bbc2e70af50e4ef6ae7d440e220be7b1cbb53f96a9309f7d2d7e3b11"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NzdjNzY0NGZhNWMzZDJiODZkNzgyZWI1YmRhYWMwMmQ1ZjlmZDU2NTE1YjM0
ZjQyZDRjNDEyNGU2MDZjNWY3ZjoyN2M3OTM3MzYxOTZkODYxY2QxYjZhNTgx
NjNjYWI1OWQxZmI3ZDJiNDEzZDA1MDI3MTA1ZGQyY2NkMmI3Nzg5

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
  "access_token": "6b45919563df979d147d529fb168214a974eca452330ce77278430688bd5e8ef",
  "token_type": "bearer",
  "created_at": 1481822388
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 77c7644fa5c3d2b86d782eb5bdaac02d5f9fd56515b34f42d4c4124e606c5f7f:27c793736196d861cd1b6a58163cab59d1fb7d2b413d05027105dd2ccd2b7789
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
Authorization: Bearer 2d1146b0165e5c5b8c4f5832f1a93b1ea2d7f78aff20cce674eedd04cc55203c
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
    "company_id": 8,
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
	-H "Authorization: Bearer 2d1146b0165e5c5b8c4f5832f1a93b1ea2d7f78aff20cce674eedd04cc55203c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/108/flashcards
Content-Type: application/json
Authorization: Bearer 231c243cb15c11aa8132d7e74e99a3cf1fbe98be0de7247b212c347ef5448d88
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":108,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 55,
    "obfuscated_id": "VX19tR4fHZ8",
    "author_id": 505,
    "chapter_id": 108,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:14.063Z",
    "created_at": "2016-12-15T17:20:14.063Z",
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
curl "api.goskive.com/v2/chapters/108/flashcards" -d '{"flashcard":{"chapter_id":108,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 231c243cb15c11aa8132d7e74e99a3cf1fbe98be0de7247b212c347ef5448d88"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/107/flashcards
Content-Type: application/json
Authorization: Bearer f9338a0802d6e9c4217d7c94ed4dd5ee1cd79feef95334b767025b027e268490
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 500,
      "chapter_id": 107,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:13.691Z",
      "created_at": "2016-12-15T17:20:13.691Z",
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 500,
      "chapter_id": 107,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:13.738Z",
      "created_at": "2016-12-15T17:20:13.738Z",
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 500,
      "chapter_id": 107,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:13.784Z",
      "created_at": "2016-12-15T17:20:13.784Z",
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
curl "api.goskive.com/v2/chapters/107/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9338a0802d6e9c4217d7c94ed4dd5ee1cd79feef95334b767025b027e268490"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/186/questions
Content-Type: application/json
Authorization: Bearer 0badd1686d2e28dae046c384d028275a76868f488af77594a8ab39d8288b9056
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":186,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 120,
    "obfuscated_id": "vEr9LtFjURM",
    "author_id": 832,
    "chapter_id": 186,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:47.830Z",
    "created_at": "2016-12-15T17:20:47.830Z",
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
        "id": 241,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 242,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 243,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 244,
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
curl "api.goskive.com/v2/chapters/186/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":186,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0badd1686d2e28dae046c384d028275a76868f488af77594a8ab39d8288b9056"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/183/questions
Content-Type: application/json
Authorization: Bearer 4fff622163839c857150acb49b8b1ba8f3aa077e72e8068d599953dff837b9f9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 117,
    "obfuscated_id": "BsA8mEPn8aM",
    "author_id": 823,
    "chapter_id": 183,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:46.194Z",
    "created_at": "2016-12-15T17:20:46.194Z",
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
        "id": 234,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 235,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/183/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fff622163839c857150acb49b8b1ba8f3aa077e72e8068d599953dff837b9f9"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/184/questions
Content-Type: application/json
Authorization: Bearer 1b8b2c856eea7699ce5ff4ae6e09faee6a3884aec2da4dfb53d52ded1d721c9d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 118,
    "obfuscated_id": "ET3wO26jBck",
    "author_id": 826,
    "chapter_id": 184,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:46.773Z",
    "created_at": "2016-12-15T17:20:46.773Z",
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
        "id": 236,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 237,
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
curl "api.goskive.com/v2/chapters/184/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b8b2c856eea7699ce5ff4ae6e09faee6a3884aec2da4dfb53d52ded1d721c9d"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/185/questions
Content-Type: application/json
Authorization: Bearer 824e6fbe18572eb13773462bd184cd442f8122c872b0b61ae1181ec4a9720b12
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":185,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 119,
    "obfuscated_id": "JRh8sWka24Y",
    "author_id": 829,
    "chapter_id": 185,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:47.330Z",
    "created_at": "2016-12-15T17:20:47.330Z",
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
        "id": 238,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 239,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 240,
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
curl "api.goskive.com/v2/chapters/185/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":185,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 824e6fbe18572eb13773462bd184cd442f8122c872b0b61ae1181ec4a9720b12"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/187/questions
Content-Type: application/json
Authorization: Bearer 1963672ce5319cea5f6ae315504a086e44cb1813ccfdcb28a24fc02be54d2c6f
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
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 835,
      "chapter_id": 187,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:48.531Z",
      "created_at": "2016-12-15T17:20:48.446Z",
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
          "id": 245,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 246,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 836,
      "chapter_id": 187,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:48.684Z",
      "created_at": "2016-12-15T17:20:48.597Z",
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
          "id": 247,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 248,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 837,
      "chapter_id": 187,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T17:20:48.848Z",
      "created_at": "2016-12-15T17:20:48.758Z",
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
          "id": 249,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 250,
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
curl "api.goskive.com/v2/chapters/187/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1963672ce5319cea5f6ae315504a086e44cb1813ccfdcb28a24fc02be54d2c6f"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/35
Content-Type: application/json
Authorization: Bearer 7a1a70a7a43a0f6f1bf2b86f6bea637f3aa97f4ef0a789beafeac46a89b6df66
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
curl "api.goskive.com/v2/chapters/35" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a1a70a7a43a0f6f1bf2b86f6bea637f3aa97f4ef0a789beafeac46a89b6df66"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/37
Content-Type: application/json
Authorization: Bearer 2b378a625f36e8efbebf0d0094fb85c0ae3a0f64a368bdac70651303463bda9f
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
curl "api.goskive.com/v2/chapters/37" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b378a625f36e8efbebf0d0094fb85c0ae3a0f64a368bdac70651303463bda9f"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/32
Content-Type: application/json
Authorization: Bearer 26210dacbef012ae745c16174c8ab691018ea2a0b435a48888dd8c49b5d49ed8
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
curl "api.goskive.com/v2/chapters/32" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26210dacbef012ae745c16174c8ab691018ea2a0b435a48888dd8c49b5d49ed8"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/36
Content-Type: application/json
Authorization: Bearer 1281e164b53d98162e8717515707f0e9e5c01db8c612aa7f441e30ca2750f5f1
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/36" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1281e164b53d98162e8717515707f0e9e5c01db8c612aa7f441e30ca2750f5f1"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/30
Content-Type: application/json
Authorization: Bearer a00f167368e9e7d77f76f56db0dfcaa2acdeb10b4498112a73c632fbab30d43f
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
    "id": 30,
    "updated_at": "2016-12-15T17:19:37.503Z",
    "course_id": 32,
    "author_id": 106,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T17:19:36.972Z",
    "questions_updated_at": "2016-12-15T17:19:36.972Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 110,
        "chapter_id": 30,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:37.484Z",
        "created_at": "2016-12-15T17:19:37.484Z",
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
        "author_id": 108,
        "chapter_id": 30,
        "position": 8,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:19:37.376Z",
        "created_at": "2016-12-15T17:19:37.283Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/30" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a00f167368e9e7d77f76f56db0dfcaa2acdeb10b4498112a73c632fbab30d43f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/33
Content-Type: application/json
Authorization: Bearer 75f6a74dbe278643a199231b40d7c9122e252def66c2c85d31a1bf59e72bb641
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
    "id": 33,
    "updated_at": "2016-12-15T17:19:38.178Z",
    "course_id": 35,
    "author_id": 119,
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
curl "api.goskive.com/v2/chapters/33" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75f6a74dbe278643a199231b40d7c9122e252def66c2c85d31a1bf59e72bb641"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/11/replies
Content-Type: application/json
Authorization: Bearer a9e9a73fe03d24d49564a4cba9abff698243e106e2aa64543f8e79d983a472bf
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
    "id": 12,
    "author_id": 326,
    "reply_to_id": 11,
    "created_at": "2016-12-15T17:19:57.967Z",
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
curl "api.goskive.com/v2/comments/11/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9e9a73fe03d24d49564a4cba9abff698243e106e2aa64543f8e79d983a472bf"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/10/replies
Content-Type: application/json
Authorization: Bearer edb28d39d49332c8d8ef1fd6d6b4dcb5d930e20b2b3a9b7d920fb5ecbe9acfee
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
curl "api.goskive.com/v2/comments/10/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edb28d39d49332c8d8ef1fd6d6b4dcb5d930e20b2b3a9b7d920fb5ecbe9acfee"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/58
Content-Type: application/json
Authorization: Bearer 6ea603c048e824c37298144c650e2383f1aaf21bb7a63cae61d60ebec1e9b020
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
curl "api.goskive.com/v2/comments/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ea603c048e824c37298144c650e2383f1aaf21bb7a63cae61d60ebec1e9b020"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/60/republish
Content-Type: application/json
Authorization: Bearer c2f2dc77cd3b4bd292b8f8aa2afcdce8cd7d3447e019a763622026e0456eae33
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
curl "api.goskive.com/v2/comments/60/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2f2dc77cd3b4bd292b8f8aa2afcdce8cd7d3447e019a763622026e0456eae33"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/56
Content-Type: application/json
Authorization: Bearer e97e449c16bc732b4f9a4e640a8ed0505c4ea33ef7c9809ee24700ea343f71a8
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e97e449c16bc732b4f9a4e640a8ed0505c4ea33ef7c9809ee24700ea343f71a8"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/55/report
Content-Type: application/json
Authorization: Bearer 9e2dacded3c0ddfcac335833d6587c6bda5d64abf73dbcf1bc514a7a081b7594
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e2dacded3c0ddfcac335833d6587c6bda5d64abf73dbcf1bc514a7a081b7594"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer f3f57b57d338fb107bd5f842df6c39e7745a1594f217d2e7a6c02b9a34f674ab
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
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T17:19:39.516Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3f57b57d338fb107bd5f842df6c39e7745a1594f217d2e7a6c02b9a34f674ab"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer dd87cce8fde0ee8bbc783efe68c47a40ebb3bbfcfc228aceea37237d1154cad0
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
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T17:19:39.447Z"
    },
    {
      "id": 2,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T17:19:39.452Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T17:19:39.456Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd87cce8fde0ee8bbc783efe68c47a40ebb3bbfcfc228aceea37237d1154cad0"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/30/company_profiles
Content-Type: application/json
Authorization: Bearer 16a9236bd4694ff6f286ad9f105b7581fc1993482b4821622ddf6098090245a8
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
curl "api.goskive.com/v2/companies/30/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16a9236bd4694ff6f286ad9f105b7581fc1993482b4821622ddf6098090245a8"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 53dded9cfbfe0400b9f58a12a6a61f2fa966a8ef0e0a15c3bf138835a2d7df52
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
	-H "Authorization: Bearer 53dded9cfbfe0400b9f58a12a6a61f2fa966a8ef0e0a15c3bf138835a2d7df52"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer cb3a0b5c5efe9a5b5ef315ffbfbc1bc5766fd2031e1630313a9890106e7e6431
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
      "id": 9,
      "title": "Campaign 8",
      "company_id": 23,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 6,
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
          "image_url_absolute": "banners/8aa5bf11cc13a7de5c7089d33a8ff916dd8f8472.png",
          "target_url": "http://goskive.com",
          "id": 6,
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
      "precluded_campaign_ids": [

      ],
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
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9d765d9b895a77cd295c7f5e57af933f977bb87f.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/648481f5d8c76852bca2fea2b305e3b694878255.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/50ffd61ac4f42ad5c682c107e23dbf7769b7381c.png",
          "target_url": "http://goskive.com",
          "id": 7,
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
	-H "Authorization: Bearer cb3a0b5c5efe9a5b5ef315ffbfbc1bc5766fd2031e1630313a9890106e7e6431"
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
Authorization: Bearer 1eb5c9e9737560e2a0013a864a5c5cfcffbbd162422ee534ea0f0c9b5c70681f
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
	-H "Authorization: Bearer 1eb5c9e9737560e2a0013a864a5c5cfcffbbd162422ee534ea0f0c9b5c70681f"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8639e953c9e311941492a8241454db1d6f411d6ecdb8d37f13830b6950ec029b
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
    "id": 92,
    "updated_at": "2016-12-15T17:20:02.036Z",
    "course_id": 99,
    "author_id": 378,
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
	-H "Authorization: Bearer 8639e953c9e311941492a8241454db1d6f411d6ecdb8d37f13830b6950ec029b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a67615e981ee1aafcaf1ca87f3e1589f067a074e31d7e5ea515d9ab35594b9a8
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
      "id": 79,
      "updated_at": "2016-12-15T17:19:59.730Z",
      "course_id": 91,
      "author_id": 349,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 70",
      "position": 1
    },
    {
      "id": 80,
      "updated_at": "2016-12-15T17:19:59.758Z",
      "course_id": 91,
      "author_id": 350,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 71",
      "position": 2
    },
    {
      "id": 81,
      "updated_at": "2016-12-15T17:20:00.015Z",
      "course_id": 91,
      "author_id": 351,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T17:19:59.600Z",
      "questions_updated_at": "2016-12-15T17:19:59.600Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 72",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a67615e981ee1aafcaf1ca87f3e1589f067a074e31d7e5ea515d9ab35594b9a8"
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
      "id": 85,
      "updated_at": "2016-12-15T17:20:00.741Z",
      "course_id": 94,
      "author_id": 363,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 76",
      "position": 1
    },
    {
      "id": 86,
      "updated_at": "2016-12-15T17:20:00.770Z",
      "course_id": 94,
      "author_id": 364,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 77",
      "position": 2
    },
    {
      "id": 87,
      "updated_at": "2016-12-15T17:20:01.096Z",
      "course_id": 94,
      "author_id": 365,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T17:20:00.618Z",
      "questions_updated_at": "2016-12-15T17:20:00.618Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 78",
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
Authorization: Bearer 313319a6e2eb84ec758a017a733003b542eefdf92e0cc56e3e1c539bda186101
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
      "id": 82,
      "updated_at": "2016-12-15T17:20:00.256Z",
      "course_id": 92,
      "author_id": 356,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 73",
      "position": 1
    },
    {
      "id": 83,
      "updated_at": "2016-12-15T17:20:00.285Z",
      "course_id": 92,
      "author_id": 357,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 74",
      "position": 2
    },
    {
      "id": 84,
      "updated_at": "2016-12-15T17:20:00.318Z",
      "course_id": 92,
      "author_id": 358,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 75",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 313319a6e2eb84ec758a017a733003b542eefdf92e0cc56e3e1c539bda186101"
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
      "id": 88,
      "updated_at": "2016-12-15T17:20:01.276Z",
      "course_id": 95,
      "author_id": 369,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 79",
      "position": 1
    },
    {
      "id": 89,
      "updated_at": "2016-12-15T17:20:01.305Z",
      "course_id": 95,
      "author_id": 370,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 80",
      "position": 2
    },
    {
      "id": 90,
      "updated_at": "2016-12-15T17:20:01.334Z",
      "course_id": 95,
      "author_id": 371,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 81",
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
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer ae83d18e695a3d840d8a73fe96119776cc93b1dd77c2a4b8d55cae70579da226
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
    "id": 1,
    "course_id": 69,
    "user_id": 269,
    "updated_at": "2016-12-15T17:19:53.381Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae83d18e695a3d840d8a73fe96119776cc93b1dd77c2a4b8d55cae70579da226"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 445fb8a8f2fd24c8254623a294cc91d1502544958f7273b53a8195e1055cf5de
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
      "id": 5,
      "course_id": 74,
      "user_id": 281,
      "updated_at": "2016-12-15T17:19:54.299Z"
    },
    {
      "id": 6,
      "course_id": 74,
      "user_id": 282,
      "updated_at": "2016-12-15T17:19:54.315Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 445fb8a8f2fd24c8254623a294cc91d1502544958f7273b53a8195e1055cf5de"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/267/files
Content-Type: application/json
Authorization: Bearer 0f9194ddcfc0a996af4c8fd02a4bf73abe2c25b36d47d28b485919a1cb13bbb5
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
      "id": 20,
      "uploader": {
        "id": 861,
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
        "created_at": "2016-12-15T17:20:51.287Z",
        "updated_at": "2016-12-15T17:20:51.287Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T17:20:51.297Z",
      "updated_at": "2016-12-15T17:20:51.297Z",
      "course_id": 267,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 862,
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
        "created_at": "2016-12-15T17:20:51.307Z",
        "updated_at": "2016-12-15T17:20:51.307Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T17:20:51.316Z",
      "updated_at": "2016-12-15T17:20:51.316Z",
      "course_id": 267,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 22,
      "uploader": {
        "id": 863,
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
        "created_at": "2016-12-15T17:20:51.325Z",
        "updated_at": "2016-12-15T17:20:51.325Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T17:20:51.334Z",
      "updated_at": "2016-12-15T17:20:51.334Z",
      "course_id": 267,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/267/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f9194ddcfc0a996af4c8fd02a4bf73abe2c25b36d47d28b485919a1cb13bbb5"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/265/files
Content-Type: application/json
Authorization: Bearer 17e09accb1d1bb1a4c72b4c443c1df6707076e8eb9a4d329a282c7bd02769b6a
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
    "id": 19,
    "uploader": {
      "id": 857,
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
      "created_at": "2016-12-15T17:20:50.874Z",
      "updated_at": "2016-12-15T17:20:50.874Z"
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
    "created_at": "2016-12-15T17:20:50.908Z",
    "updated_at": "2016-12-15T17:20:50.908Z",
    "course_id": 265,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/265/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17e09accb1d1bb1a4c72b4c443c1df6707076e8eb9a4d329a282c7bd02769b6a"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/264/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 962d763e78909141967acbbdfde00fa182148df725f8cb8841f0f48fd289c96d
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
    "key": "cache/2befb9c964c410627989722e393261ec.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxODoyMDo1MFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzJiZWZiOWM5NjRjNDEwNjI3OTg5NzIyZTM5MzI2MWVjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDE3MjA1MFoifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T172050Z",
    "x-amz-signature": "9f6b87b6d970507790c993b61543ad675bcd915c54994c5e13aa20accc2655d4"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/264/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 962d763e78909141967acbbdfde00fa182148df725f8cb8841f0f48fd289c96d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 98404cb28dfe08410bcbf1685bf5838716a2e8d072247211c4a3f29c2595c6cb
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
	-H "Authorization: Bearer 98404cb28dfe08410bcbf1685bf5838716a2e8d072247211c4a3f29c2595c6cb"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 13c87918f091a5923cb7a13852629f625fc7d9e4aaeec3feedde042b73f2f868
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
	-H "Authorization: Bearer 13c87918f091a5923cb7a13852629f625fc7d9e4aaeec3feedde042b73f2f868"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f3e8de0080edc0309fce3ae9f359a56cc60f8254a9066ffe7d1c46a65adb400f
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
	-H "Authorization: Bearer f3e8de0080edc0309fce3ae9f359a56cc60f8254a9066ffe7d1c46a65adb400f"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3e57cfd90b2ceb5f804e7e5007cf29f5018e7ff21c8a4cd318e855f550d694ef
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
	-H "Authorization: Bearer 3e57cfd90b2ceb5f804e7e5007cf29f5018e7ff21c8a4cd318e855f550d694ef"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 90545a8f35ee4e08f320f60a2f1d75be60c8274d16e4c288c8368706b1490021
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
	-H "Authorization: Bearer 90545a8f35ee4e08f320f60a2f1d75be60c8274d16e4c288c8368706b1490021"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer a14b180c8944f491498bf928725f692488c41508487f44c99b2ee5b2a210db7d
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
    "creator_id": 774,
    "id": 240,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 224,
    "additional_university_ids": [

    ],
    "discipline_id": 242,
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
    "chapters_updated_at": "2016-12-15T17:20:38.131Z",
    "updated_at": "2016-12-15T17:20:39.426Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 775,
        "chapter_id": 171,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:39.195Z",
        "created_at": "2016-12-15T17:20:39.195Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 775,
        "chapter_id": 172,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:39.272Z",
        "created_at": "2016-12-15T17:20:39.272Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 775,
        "chapter_id": 171,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:39.240Z",
        "created_at": "2016-12-15T17:20:39.240Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 775,
        "chapter_id": 172,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:39.315Z",
        "created_at": "2016-12-15T17:20:39.315Z",
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
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 775,
        "chapter_id": 171,
        "position": 82,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:38.377Z",
        "created_at": "2016-12-15T17:20:38.290Z",
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
            "id": 182,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 183,
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
        "author_id": 775,
        "chapter_id": 171,
        "position": 83,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:38.514Z",
        "created_at": "2016-12-15T17:20:38.436Z",
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
      },
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 775,
        "chapter_id": 172,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:38.684Z",
        "created_at": "2016-12-15T17:20:38.595Z",
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
            "id": 186,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 187,
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
        "author_id": 775,
        "chapter_id": 172,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:38.828Z",
        "created_at": "2016-12-15T17:20:38.747Z",
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
            "id": 188,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 189,
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
        "id": 171,
        "updated_at": "2016-12-15T17:20:39.371Z",
        "course_id": 240,
        "author_id": 774,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T17:20:38.131Z",
        "questions_updated_at": "2016-12-15T17:20:38.131Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 153",
        "position": 1
      },
      {
        "id": 172,
        "updated_at": "2016-12-15T17:20:39.415Z",
        "course_id": 240,
        "author_id": 774,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T17:20:38.131Z",
        "questions_updated_at": "2016-12-15T17:20:38.131Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 154",
        "position": 2
      }
    ],
    "topic_id": 242,
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
	-H "Authorization: Bearer a14b180c8944f491498bf928725f692488c41508487f44c99b2ee5b2a210db7d"
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
    "creator_id": 780,
    "id": 241,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 225,
    "additional_university_ids": [

    ],
    "discipline_id": 243,
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
    "chapters_updated_at": "2016-12-15T17:20:39.584Z",
    "updated_at": "2016-12-15T17:20:40.851Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 97,
        "obfuscated_id": "qdTHUgSdSV8",
        "author_id": 780,
        "chapter_id": 173,
        "position": 88,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:39.812Z",
        "created_at": "2016-12-15T17:20:39.728Z",
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
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 780,
        "chapter_id": 174,
        "position": 90,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T17:20:40.115Z",
        "created_at": "2016-12-15T17:20:40.027Z",
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
    ],
    "chapters": [
      {
        "id": 173,
        "updated_at": "2016-12-15T17:20:40.798Z",
        "course_id": 241,
        "author_id": 780,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T17:20:39.584Z",
        "questions_updated_at": "2016-12-15T17:20:39.584Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 155",
        "position": 1
      },
      {
        "id": 174,
        "updated_at": "2016-12-15T17:20:40.841Z",
        "course_id": 241,
        "author_id": 780,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T17:20:39.584Z",
        "questions_updated_at": "2016-12-15T17:20:39.584Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 156",
        "position": 2
      }
    ],
    "topic_id": 243,
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
PUT /v2/courses/244/pin
Content-Type: application/json
Authorization: Bearer 3722bea603466a82353c60982ee34a71f018462953ad6ed6da2773edb1ae74e2
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/244/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3722bea603466a82353c60982ee34a71f018462953ad6ed6da2773edb1ae74e2"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/245/pin
Content-Type: application/json
Authorization: Bearer dc6915f41a4202480146c60121c55dec2fd5f9f22677cb7734f6760a2e9d1c46
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/245/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc6915f41a4202480146c60121c55dec2fd5f9f22677cb7734f6760a2e9d1c46"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 45dcc46ad59f4f964e4ea1ff5fe848f43e967c91d46bf0fc577c43cf8aa9f4b8
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
    "creator_id": 769,
    "id": 237,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 221,
    "additional_university_ids": [

    ],
    "discipline_id": 239,
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
    "updated_at": "2016-12-15T17:20:37.701Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 239,
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
	-H "Authorization: Bearer 45dcc46ad59f4f964e4ea1ff5fe848f43e967c91d46bf0fc577c43cf8aa9f4b8"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 9f3d9e1ffcef8beab2ba79b721c4acecf66d2584f8295fed43c60ee2f4e3c894
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
    "id": 975,
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
    "created_at": "2016-12-15T17:20:59.608Z",
    "updated_at": "2016-12-15T17:20:59.608Z",
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
	-H "Authorization: Bearer 9f3d9e1ffcef8beab2ba79b721c4acecf66d2584f8295fed43c60ee2f4e3c894"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 59fae3750e9666c922a9ff54f302b6d55e9d8e306aaf698d8a3e4e55e0610b0a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[318]}
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
    "id": 977,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      318
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T17:21:00.012Z",
    "updated_at": "2016-12-15T17:21:00.051Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[318]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59fae3750e9666c922a9ff54f302b6d55e9d8e306aaf698d8a3e4e55e0610b0a"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c5d88d728da8241a16e42298f8cfe6c15692611ca0fde8bf766dd957802e2278
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
    "id": 978,
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
    "created_at": "2016-12-15T17:21:00.077Z",
    "updated_at": "2016-12-15T17:21:00.077Z",
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
	-H "Authorization: Bearer c5d88d728da8241a16e42298f8cfe6c15692611ca0fde8bf766dd957802e2278"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 88748a539649ca350dd3aae458d47f04fb0089554cc44434898013a3cb1814d6
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[320]}
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
    "id": 979,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      320
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T17:21:00.169Z",
    "updated_at": "2016-12-15T17:21:00.169Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[320]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88748a539649ca350dd3aae458d47f04fb0089554cc44434898013a3cb1814d6"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 2685e13c1c5c5f7e4e83b85427d913d867446294245a73b9df670c8f40861003
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

317
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
    "id": 976,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/ce347d6a4f245eaed5907731997cb7ae969d04c2.jpg",
    "university_id": null,
    "fields_of_study": [
      317
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T17:20:59.692Z",
    "updated_at": "2016-12-15T17:20:59.961Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/3c7fce7deb06f616226f8dbda8ff8659e8463564.jpg",
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

317
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 2685e13c1c5c5f7e4e83b85427d913d867446294245a73b9df670c8f40861003"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 03fd6424004d753623874bb948052d139af474e3312ed28c3d909d2a4525b353
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
      "id": 5,
      "bookmarkable_id": 24,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 25,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 26,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03fd6424004d753623874bb948052d139af474e3312ed28c3d909d2a4525b353"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer eb1763a93be1276d211020e082c515bfcd8053058168295c21a789e481130e8b
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
      "creator_id": 16,
      "id": 5,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-5",
      "html_url": "https://goskive.com/course/mit-course-5",
      "slug": "mit-course-5",
      "university_id": 5,
      "additional_university_ids": [

      ],
      "discipline_id": 5,
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
      "updated_at": "2016-12-15T17:19:29.833Z",
      "shortname": "mit-course-5",
      "topic_id": 5,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 15,
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-4",
      "html_url": "https://goskive.com/course/mit-course-4",
      "slug": "mit-course-4",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "discipline_id": 4,
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
      "updated_at": "2016-12-15T17:19:29.706Z",
      "shortname": "mit-course-4",
      "topic_id": 4,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 4",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb1763a93be1276d211020e082c515bfcd8053058168295c21a789e481130e8b"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 86ef5f05d94e65a7f6a3887be8e9feab0df0dc9c931b53c82ee598ba7dafb83d
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
        "id": 3,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T17:19:46.379Z",
        "updated_at": "2016-12-15T17:19:46.379Z",
        "file_url": "memory://b3cfafe9a86c3530c1e28f7e9c55954f.pdf",
        "course_id": 55,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 4,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T17:19:46.510Z",
        "updated_at": "2016-12-15T17:19:46.510Z",
        "file_url": "memory://abd37b0bcb9968dc805bc4f1c3169973.pdf",
        "course_id": 56,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 5,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T17:19:46.638Z",
        "updated_at": "2016-12-15T17:19:46.638Z",
        "file_url": "memory://4085cb2e02a9debef4ea7a99ecc3ab08.pdf",
        "course_id": 57,
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
	-H "Authorization: Bearer 86ef5f05d94e65a7f6a3887be8e9feab0df0dc9c931b53c82ee598ba7dafb83d"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e42e6fc912ae808e52a597aaee5eda3de55159dbd97688f6f1b2b15bfdc976ca
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
        "updated_at": "2016-12-15T17:21:00.603Z"
      },
      "created_at": "2016-12-15T17:21:00.607Z",
      "updated_at": "2016-12-15T17:21:00.607Z",
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
        "updated_at": "2016-12-15T17:21:00.615Z"
      },
      "created_at": "2016-12-15T17:21:00.618Z",
      "updated_at": "2016-12-15T17:21:00.618Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e42e6fc912ae808e52a597aaee5eda3de55159dbd97688f6f1b2b15bfdc976ca"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer e8cf6c94b3db0215c5edd92d36bc882971efd372d4c3023126955f37041996f7
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
      "created_at": "2016-12-15T17:19:54.734Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 8,
      "updated_at": "2016-12-15T17:19:54.891Z",
      "author_id": "290",
      "thread_subject_id": "76",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 12,
      "created_at": "2016-12-15T17:19:54.879Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 9,
      "updated_at": "2016-12-15T17:19:54.894Z",
      "author_id": "293",
      "thread_subject_id": "77",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-12-15T17:19:55.319Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-12-15T17:19:55.319Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-12-15T17:19:55.736Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-12-15T17:19:55.736Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 15,
      "created_at": "2016-12-15T17:19:56.152Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-12-15T17:19:56.152Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 16,
      "created_at": "2016-12-15T17:19:56.460Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 35,
      "updated_at": "2016-12-15T17:19:56.460Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-12-15T17:19:56.783Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 36,
      "updated_at": "2016-12-15T17:19:56.783Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-12-15T17:19:57.097Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 37,
      "updated_at": "2016-12-15T17:19:57.097Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8cf6c94b3db0215c5edd92d36bc882971efd372d4c3023126955f37041996f7"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/10
Content-Type: application/json
Authorization: Bearer 32afabcf9914b39a5419875a989fa1212aec997f25908e2586fe3be68f4a6dce
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T17:09:54.000Z"}}
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
    "id": 10,
    "created_at": "2016-12-15T17:19:54.527Z",
    "read_at": "2016-12-15T17:09:54.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 7,
    "updated_at": "2016-12-15T17:19:54.578Z",
    "author_id": "286",
    "thread_subject_id": "75",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/10" -d '{"notification":{"read_at":"2016-12-15T17:09:54.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32afabcf9914b39a5419875a989fa1212aec997f25908e2586fe3be68f4a6dce"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer e9da66bc31b3f4b82b82a6a40f2398b2c9329f7ebf33673625aa77be40229bfb
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
      "course_id": 148,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T17:20:09.798Z",
      "course_published": true,
      "updated_at": "2016-12-15T17:20:09.793Z"
    },
    {
      "id": 6,
      "course_id": 149,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T17:20:09.926Z",
      "course_published": true,
      "updated_at": "2016-12-15T17:20:09.921Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9da66bc31b3f4b82b82a6a40f2398b2c9329f7ebf33673625aa77be40229bfb"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 1f35e440e54a2318f9d8d06aadcc93698be38996ea17ba96bf8c3051ee3ef949
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
    "id": 3,
    "course_id": 146,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T17:20:09.407Z",
    "course_published": true,
    "updated_at": "2016-12-15T17:20:09.401Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f35e440e54a2318f9d8d06aadcc93698be38996ea17ba96bf8c3051ee3ef949"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 64fccf28715ad3878941aafc8f0efccb30021aebb20c37151fc58a15252e516c
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
    "course_id": 147,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T17:20:09.648Z",
    "course_published": true,
    "updated_at": "2016-12-15T17:20:09.639Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64fccf28715ad3878941aafc8f0efccb30021aebb20c37151fc58a15252e516c"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer d6612da11a14dadb4b94f1c90700816cda159379cfd9008995502e37773f3e5d
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
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 127,
      "user_id": 961
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 961
    },
    {
      "id": 22,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 129,
      "user_id": 961
    },
    {
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 961
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6612da11a14dadb4b94f1c90700816cda159379cfd9008995502e37773f3e5d"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/311
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
    "id": 311,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 311,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 311
      },
      {
        "id": 312,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 311
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/311" -X GET \
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
      "id": 312,
      "name": "Phased dedicated firmware",
      "name_translations": {
        "en": "Phased dedicated firmware"
      }
    },
    {
      "id": 313,
      "name": "Object-based value-added support",
      "name_translations": {
        "en": "Object-based value-added support"
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
PATCH /v2/feedbacks/12/close
Content-Type: application/json
Authorization: Bearer 24a4095caff5fbbec970230f551c1e3fb00a53dd2815ad8b53e1d6437c4005f8
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
    "id": 12,
    "user_id": 599,
    "feedbackable_id": 58,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T17:20:24.636Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24a4095caff5fbbec970230f551c1e3fb00a53dd2815ad8b53e1d6437c4005f8"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/37/fix
Content-Type: application/json
Authorization: Bearer 1bfa62aacaede1b979e13af3bcf515a1c7993e1f13a1228267df29775b37dbbb
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
    "id": 37,
    "user_id": 712,
    "feedbackable_id": 64,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T17:20:32.789Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/37/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bfa62aacaede1b979e13af3bcf515a1c7993e1f13a1228267df29775b37dbbb"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/33
Content-Type: application/json
Authorization: Bearer 8c5360d6eae19dde72b38a3f65bbcd666dbc74256ce8c0e6d530ae7f7294ef2b
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
    "id": 33,
    "user_id": 690,
    "feedbackable_id": 60,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T17:20:31.636Z",
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
curl "api.goskive.com/v2/feedbacks/33" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c5360d6eae19dde72b38a3f65bbcd666dbc74256ce8c0e6d530ae7f7294ef2b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/11/close
Content-Type: application/json
Authorization: Bearer 2bc8b4063df4acf2f50e530e98ffe4cfbeea1a34cc7a3e3b97b30d0d31351208
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
curl "api.goskive.com/v2/feedbacks/11/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bc8b4063df4acf2f50e530e98ffe4cfbeea1a34cc7a3e3b97b30d0d31351208"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/fix
Content-Type: application/json
Authorization: Bearer 52eb3bb14f626bca1934a8ae0155fff06913f14f6c7e220e38bacbc0ec50ebb6
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
curl "api.goskive.com/v2/feedbacks/35/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52eb3bb14f626bca1934a8ae0155fff06913f14f6c7e220e38bacbc0ec50ebb6"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/36/fix
Content-Type: application/json
Authorization: Bearer ebc968c07edcad5e03e8455fc0a62cefd7f44be93ece459b134174027cea5ed8
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
curl "api.goskive.com/v2/feedbacks/36/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebc968c07edcad5e03e8455fc0a62cefd7f44be93ece459b134174027cea5ed8"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/34
Content-Type: application/json
Authorization: Bearer 0adef910c689de549027f83b53924b74b91d27522527d97cc7bfbff2d28060ce
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
    "id": 34,
    "user_id": 695,
    "feedbackable_id": 61,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T17:20:32.019Z",
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
curl "api.goskive.com/v2/feedbacks/34" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0adef910c689de549027f83b53924b74b91d27522527d97cc7bfbff2d28060ce"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 0f8a831c1ccf2363944de28f21836889de83c6002437f97b8a8dc37c1e7751fd
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
	-H "Authorization: Bearer 0f8a831c1ccf2363944de28f21836889de83c6002437f97b8a8dc37c1e7751fd"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer 7ce361393de2bf25991c96bb135b1d29ac0e4c50e9e5107f17df3f28f52168e9
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
	-H "Authorization: Bearer 7ce361393de2bf25991c96bb135b1d29ac0e4c50e9e5107f17df3f28f52168e9"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 627cde38cc227bd4dc2ce9badb11b21a864521835b9c89b6103688a7f1207dfb
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
	-H "Authorization: Bearer 627cde38cc227bd4dc2ce9badb11b21a864521835b9c89b6103688a7f1207dfb"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer a61ce7e3cc2047eddd64a5a69d7329144b25cea04071618249998ebe43ef96ed
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/300d8e5e70bf24a3a36b1fe1a6632675.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T172011Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=50026fcc409652892ea0787378fb6dcf58537d99d1ee4a8ebee9ed121c029667",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a61ce7e3cc2047eddd64a5a69d7329144b25cea04071618249998ebe43ef96ed"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/12/preview
Content-Type: application/json
Authorization: Bearer 40a2b348bba88e483fbaaee084a5ac7528cd7e1e9dde6ef7de5f84d4b67e9f3b
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/4424713ec9b2ba834dbaa3d3674f7331.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T172011Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6bc1c08af61e50d1cd1243e1a9d97a78abca5d17077bf32135af56f62bed7891",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/12/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40a2b348bba88e483fbaaee084a5ac7528cd7e1e9dde6ef7de5f84d4b67e9f3b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 85c159ab9856faee52071ba4aae2405d1822a5b7c16929d2ca06b2efe66cb1ce
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
    "id": 14,
    "uploader": {
      "id": 482,
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
      "created_at": "2016-12-15T17:20:12.111Z",
      "updated_at": "2016-12-15T17:20:12.111Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T17:20:12.236Z",
    "updated_at": "2016-12-15T17:20:12.236Z",
    "course_id": 160,
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
curl "api.goskive.com/v2/files/14/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85c159ab9856faee52071ba4aae2405d1822a5b7c16929d2ca06b2efe66cb1ce"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer cb38c43d9652b42783b8a03cc2de7069059310cdafa81aea48bdad6cd1bc7cea
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
      "creator_id": 188,
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 51,
      "additional_university_ids": [

      ],
      "discipline_id": 51,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 2,
      "questions_count": 1,
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
      "chapters_updated_at": "2016-12-15T17:19:43.918Z",
      "updated_at": "2016-12-15T17:19:45.168Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 51,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 193,
      "id": 52,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-9b8eed6a-6cd0-4b87-ab73-3f4d990a0610",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-9b8eed6a-6cd0-4b87-ab73-3f4d990a0610",
      "slug": "mit-the-great-british-bake-off-9b8eed6a-6cd0-4b87-ab73-3f4d990a0610",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "discipline_id": 52,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 2,
      "questions_count": 1,
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
      "chapters_updated_at": "2016-12-15T17:19:43.918Z",
      "updated_at": "2016-12-15T17:19:45.591Z",
      "shortname": "mit-the-great-british-bake-off-9b8eed6a-6cd0-4b87-ab73-3f4d990a0610",
      "topic_id": 52,
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
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer cb38c43d9652b42783b8a03cc2de7069059310cdafa81aea48bdad6cd1bc7cea"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/6/download
Content-Type: application/json
Authorization: Bearer 14512b74cfc19d9b08e1eac66a1b4fd91122e7bfee1fd98349ae05042532da92
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14512b74cfc19d9b08e1eac66a1b4fd91122e7bfee1fd98349ae05042532da92"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/17/report
Content-Type: application/json
Authorization: Bearer 16ba007fecf1a847134120142417ac4146f07e80800930d11322280524ad3086
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
	-H "Authorization: Bearer 16ba007fecf1a847134120142417ac4146f07e80800930d11322280524ad3086"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/18/bookmark
Content-Type: application/json
Authorization: Bearer dc29aca2426c36b2ce36a70120871341d2a37d6c82d965fe3a138f6649185784
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc29aca2426c36b2ce36a70120871341d2a37d6c82d965fe3a138f6649185784"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/16/upvote
Content-Type: application/json
Authorization: Bearer dbee7b689231a7f9f9a2a448efaef995e486455dded69f3f7c535d23729bbce7
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbee7b689231a7f9f9a2a448efaef995e486455dded69f3f7c535d23729bbce7"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/51/comments
Content-Type: application/json
Authorization: Bearer 63bad1724b885ba1e4f180af7c3f769c7a97702052be985d406f861d1345581c
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
    "id": 16,
    "author_id": 444,
    "reply_to_id": null,
    "created_at": "2016-12-15T17:20:09.104Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/51/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63bad1724b885ba1e4f180af7c3f769c7a97702052be985d406f861d1345581c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/50/comments
Content-Type: application/json
Authorization: Bearer 96922ff38f164062d7137a7c0ea9ae2fe95eed29cc595e7197b2859c9b99a5a5
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
    "id": 15,
    "author_id": 441,
    "reply_to_id": null,
    "created_at": "2016-12-15T17:20:08.701Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 441,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:08.699Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/50/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96922ff38f164062d7137a7c0ea9ae2fe95eed29cc595e7197b2859c9b99a5a5"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/48/comments
Content-Type: application/json
Authorization: Bearer fb378f8bdff1bf8ad5b634887f1fb20dd4199f291eb9b3deb573fa9fcc213439
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
      "id": 13,
      "author_id": 436,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:08.180Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 437,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:20:08.196Z",
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
curl "api.goskive.com/v2/flashcards/48/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb378f8bdff1bf8ad5b634887f1fb20dd4199f291eb9b3deb573fa9fcc213439"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/49/comments
Content-Type: application/json
Authorization: Bearer 350a308f346bbf940677d0d6f76f4926e8deae521fd83bd384aaf28079a286c4
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/49/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 350a308f346bbf940677d0d6f76f4926e8deae521fd83bd384aaf28079a286c4"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer 4fe596c65a5ab919df996276dde582da014af2c726b5edf59c6e5b3ea055ee1e
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
    "user_id": 719,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T17:20:33.693Z",
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
curl "api.goskive.com/v2/flashcards/66/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fe596c65a5ab919df996276dde582da014af2c726b5edf59c6e5b3ea055ee1e"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/71/feedbacks
Content-Type: application/json
Authorization: Bearer 31cdc361e49594ce22a860bf2e58df2e69870c9fbf93d87382f49861a8fa2dfa
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
      "id": 44,
      "user_id": 740,
      "feedbackable_id": 71,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:35.248Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 739,
      "feedbackable_id": 71,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:20:35.238Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/71/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31cdc361e49594ce22a860bf2e58df2e69870c9fbf93d87382f49861a8fa2dfa"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/38/votes
Content-Type: application/json
Authorization: Bearer 901539e5b3a819412286ec8f56e3c7207c7b7d43af03c310fd2b22bd81b7d854
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
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 38,
      "user_id": 264
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 38,
      "user_id": 263
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 38,
      "user_id": 262
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/38/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 901539e5b3a819412286ec8f56e3c7207c7b7d43af03c310fd2b22bd81b7d854"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/8/republish
Content-Type: application/json
Authorization: Bearer c9f729a6899941a18fd2e7ce88bef9a71280f7710c07245e64e51a0ae65bc835
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
curl "api.goskive.com/v2/flashcards/8/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9f729a6899941a18fd2e7ce88bef9a71280f7710c07245e64e51a0ae65bc835"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/24/bookmark
Content-Type: application/json
Authorization: Bearer 1231683aca8cc855437028f3c3006bcda3100908f3f2deb891df0e8e6273079c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1231683aca8cc855437028f3c3006bcda3100908f3f2deb891df0e8e6273079c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/5
Content-Type: application/json
Authorization: Bearer 2532a6824f8676e2fb069820aecf6ef50efbf7022b070e5889edec3e581a1dcd
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2532a6824f8676e2fb069820aecf6ef50efbf7022b070e5889edec3e581a1dcd"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/4/downvote
Content-Type: application/json
Authorization: Bearer 2f6e6bf3e1ca1fb1345ee1e67607ec1fc7d7ab30cf8fccbc69929024471bad10
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/4/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f6e6bf3e1ca1fb1345ee1e67607ec1fc7d7ab30cf8fccbc69929024471bad10"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/6
Content-Type: application/json
Authorization: Bearer c52a7c98a3f36222da05128d4908fbc923c56d7922013f733a129d055b4a23bf
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
    "id": 6,
    "obfuscated_id": "eyxYPTvoIb8",
    "author_id": 36,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:19:32.429Z",
    "created_at": "2016-12-15T17:19:32.429Z",
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
curl "api.goskive.com/v2/flashcards/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c52a7c98a3f36222da05128d4908fbc923c56d7922013f733a129d055b4a23bf"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/2/report
Content-Type: application/json
Authorization: Bearer 3e331ff641aba84aa28eaf588e53ecbeaae998c0ce6bbc3bb28bc8b6b6c8ccb1
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/2/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e331ff641aba84aa28eaf588e53ecbeaae998c0ce6bbc3bb28bc8b6b6c8ccb1"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/3/bookmark
Content-Type: application/json
Authorization: Bearer a024dd996a795edc37d3f29a3795f85ca35ae68fcc37d7507ba854b2b0322d23
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/3/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a024dd996a795edc37d3f29a3795f85ca35ae68fcc37d7507ba854b2b0322d23"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/1/upvote
Content-Type: application/json
Authorization: Bearer 4ed651604f9542bd8e29bade774e240681faa26085e4cfc89ee691d7b698b91f
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/1/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ed651604f9542bd8e29bade774e240681faa26085e4cfc89ee691d7b698b91f"
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
    "key": "cache/060e27f84c60acd7d8677519e1f27168.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxODoyMTowMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzA2MGUyN2Y4NGM2MGFjZDdkODY3NzUxOWUxZjI3MTY4LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTcyMTAxWiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T172101Z",
    "x-amz-signature": "2ffd8a0489f94a66933d3847cd64915f0e024252f428e8e0708505809f0af8e4"
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
Authorization: Bearer eedd0effa2bc5eb9de8b428fe2dfedc2fe8f471b0969a1afb934c11e34ed2e54
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
	-H "Authorization: Bearer eedd0effa2bc5eb9de8b428fe2dfedc2fe8f471b0969a1afb934c11e34ed2e54"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 959ff93dae45e17a7d89426d0d94ff6acddc8ede9bdbc277a423c6963466e193
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
	-H "Authorization: Bearer 959ff93dae45e17a7d89426d0d94ff6acddc8ede9bdbc277a423c6963466e193"
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
{"password":{"reset_password_token":"GT-xJxrbrG44ztx8XyZs","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 211,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T17:19:46.713Z",
  "updated_at": "2016-12-15T17:19:47.336Z",
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
  "audit_id": 7493
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"GT-xJxrbrG44ztx8XyZs","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/29/comments
Content-Type: application/json
Authorization: Bearer 784a3053e6fc2bc74d0e4c6a8d1d1e3279243fee7cea4b9d2e12ebc2041ea274
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
    "id": 4,
    "author_id": 245,
    "reply_to_id": null,
    "created_at": "2016-12-15T17:19:51.090Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/29/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 784a3053e6fc2bc74d0e4c6a8d1d1e3279243fee7cea4b9d2e12ebc2041ea274"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer b325d9c580e8f402df4acc42cc2e3e28225931c593970fcf209c55a34235d503
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
    "id": 3,
    "author_id": 239,
    "reply_to_id": null,
    "created_at": "2016-12-15T17:19:50.209Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 239,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:19:50.206Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/27/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b325d9c580e8f402df4acc42cc2e3e28225931c593970fcf209c55a34235d503"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/30/comments
Content-Type: application/json
Authorization: Bearer b2e91b2dcbb386c51aeb0dc767675f17cd92e32ebae011a1a497480f966b4c44
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
      "id": 5,
      "author_id": 251,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:19:51.586Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 252,
      "reply_to_id": null,
      "created_at": "2016-12-15T17:19:51.604Z",
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
curl "api.goskive.com/v2/questions/30/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2e91b2dcbb386c51aeb0dc767675f17cd92e32ebae011a1a497480f966b4c44"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/28/comments
Content-Type: application/json
Authorization: Bearer c371e9006d82fe1e3789bad346c677f5186644f78f16f06c282b73d8c9a4a435
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/28/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c371e9006d82fe1e3789bad346c677f5186644f78f16f06c282b73d8c9a4a435"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/12/feedbacks
Content-Type: application/json
Authorization: Bearer b25af2944b1d12d97d0c5d135dbeb22d652cf65a8700d74838eadd97bcf25c8a
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
    "id": 2,
    "user_id": 142,
    "feedbackable_id": 12,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T17:19:41.198Z",
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
curl "api.goskive.com/v2/questions/12/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b25af2944b1d12d97d0c5d135dbeb22d652cf65a8700d74838eadd97bcf25c8a"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/18/feedbacks
Content-Type: application/json
Authorization: Bearer 602f4be27bf6549864b2f4fe29ed54e7916f83d5fb9c2c288a8fc1e68456cd71
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
      "id": 8,
      "user_id": 174,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:19:43.591Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 173,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T17:19:43.581Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/18/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 602f4be27bf6549864b2f4fe29ed54e7916f83d5fb9c2c288a8fc1e68456cd71"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/2/votes
Content-Type: application/json
Authorization: Bearer a44edb73d634937af4381f96766b6da214f0db1d117651ecf8564d10696fd7f4
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
      "votable_id": 2,
      "user_id": 9
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 8
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 7
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a44edb73d634937af4381f96766b6da214f0db1d117651ecf8564d10696fd7f4"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/66/republish
Content-Type: application/json
Authorization: Bearer 21b31ede127ffeb600b8689641e691ef117cac1c713c66c5e9d840c3cad21ea8
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
curl "api.goskive.com/v2/questions/66/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21b31ede127ffeb600b8689641e691ef117cac1c713c66c5e9d840c3cad21ea8"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/71/bookmark
Content-Type: application/json
Authorization: Bearer cb9066cf7f60ba7f298d39746ba4fb7e0930989f4cf14aa65510dfa443415b5d
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/71/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb9066cf7f60ba7f298d39746ba4fb7e0930989f4cf14aa65510dfa443415b5d"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/69
Content-Type: application/json
Authorization: Bearer 19c6548af7074f531536f95fb14221ce72ec92b7867dba383eb4dae0367ebeb3
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/69" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19c6548af7074f531536f95fb14221ce72ec92b7867dba383eb4dae0367ebeb3"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/62/downvote
Content-Type: application/json
Authorization: Bearer b695e053ab9fa7584ad57da2b7b1f5a3926d50617bfcb6e5dba21d0aa7c0ceab
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/62/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b695e053ab9fa7584ad57da2b7b1f5a3926d50617bfcb6e5dba21d0aa7c0ceab"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/68
Content-Type: application/json
Authorization: Bearer cadc2a8964f97a9f473275e3f15bc6bb918ca3360b18e70a48c89acfb9e27209
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 579,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:22.732Z",
    "created_at": "2016-12-15T17:20:22.642Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/68" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cadc2a8964f97a9f473275e3f15bc6bb918ca3360b18e70a48c89acfb9e27209"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/70/report
Content-Type: application/json
Authorization: Bearer ed6f7d647c9408f0ccf8259f103c74a888e659ec41c5311ce00a81e1076484e6
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/70/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed6f7d647c9408f0ccf8259f103c74a888e659ec41c5311ce00a81e1076484e6"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/63/bookmark
Content-Type: application/json
Authorization: Bearer c837e7130521d1bba7ca07b1b9e000e99aed1160e70e959cb99a4bb70e4d4075
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/63/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c837e7130521d1bba7ca07b1b9e000e99aed1160e70e959cb99a4bb70e4d4075"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/64
Content-Type: application/json
Authorization: Bearer 88b993e4186498de2841cf4f9c6a3dd78ebe15f96d1205bb5ae0402cb20309e7
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":64,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T17:20:20.775Z","updated_at":"2016-12-15T17:20:20.884Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":127,"author_id":567,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 64,
    "obfuscated_id": "H-V851w7HZg",
    "author_id": 567,
    "chapter_id": 127,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T17:20:21.021Z",
    "created_at": "2016-12-15T17:20:20.775Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x0000001141ee78>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 129,
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
curl "api.goskive.com/v2/questions/64" -d '{"question":{"question":{"id":64,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T17:20:20.775Z","updated_at":"2016-12-15T17:20:20.884Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":127,"author_id":567,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88b993e4186498de2841cf4f9c6a3dd78ebe15f96d1205bb5ae0402cb20309e7"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/67/upvote
Content-Type: application/json
Authorization: Bearer 9c9f2b7bfe256318f14390934df2d1b6583e26af9bbde6551ca6fd4ae541b5e3
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/67/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c9f2b7bfe256318f14390934df2d1b6583e26af9bbde6551ca6fd4ae541b5e3"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 12f53bb24052c32d7e182cf7c8e0053d492887c4e57bdfef609d144c4be4ebf9
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
      "creator_id": 986,
      "id": 314,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 300,
      "additional_university_ids": [

      ],
      "discipline_id": 327,
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
      "updated_at": "2016-12-15T17:21:01.256Z",
      "shortname": "mit-pizza-201",
      "topic_id": 326,
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
	-H "Authorization: Bearer 12f53bb24052c32d7e182cf7c8e0053d492887c4e57bdfef609d144c4be4ebf9"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b1bec5a7cb845a6892188aee6a23fbff2ce54621161ef3abb26de8e531b38f3e
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
      "id": 298,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-278",
      "html_url": "https://goskive.com/university/uni-278",
      "slug": "uni-278",
      "name": "National School of Pizza",
      "short_name": "Uni 278",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/aec37fb345499adc0586b02dda4ad32f.jpg",
      "image_url_small": "memory://universities/d60b73103b05025baf604dfbcd91dbd7.jpg",
      "image_thumb_url": "memory://universities/5405536eeb4db3ef3d5a92388ad56b08.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T17:21:00.929Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 297,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-277",
      "html_url": "https://goskive.com/university/uni-277",
      "slug": "uni-277",
      "name": "National School of Pastry",
      "short_name": "Uni 277",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/30c1071f3b3446a847c56a64d8c3a9d7.jpg",
      "image_url_small": "memory://universities/87a27e21824067c415c3921665fe15e7.jpg",
      "image_thumb_url": "memory://universities/e27158f8f5cf4941f66f2358ddb47a2a.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T17:21:00.862Z",
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
	-H "Authorization: Bearer b1bec5a7cb845a6892188aee6a23fbff2ce54621161ef3abb26de8e531b38f3e"
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
      "id": 322,
      "name": "Versatile client-server budgetary management",
      "name_translations": {
        "en": "Versatile client-server budgetary management"
      },
      "discipline_id": 323
    },
    {
      "id": 323,
      "name": "Optimized global task-force",
      "name_translations": {
        "en": "Optimized global task-force"
      },
      "discipline_id": 324
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
GET /v2/topics/324
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
    "id": 324,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 325
  }
}
```



```shell
curl "api.goskive.com/v2/topics/324" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer ad93004d6a980f7e0e98749669483bbc46e3b49b20645589f5889a1c787f8979
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
      "id": 218,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-198",
      "html_url": "https://goskive.com/university/uni-198",
      "slug": "uni-198",
      "name": "University 161",
      "short_name": "Uni 198",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/24268143f82b8e42da0fb6e24c629c79.jpg",
      "image_url_small": "memory://universities/a807ab21b281467847e7af07225889c8.jpg",
      "image_thumb_url": "memory://universities/13a2f20568fe74761d8f6045ef123e69.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T17:20:37.223Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 217,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-197",
      "html_url": "https://goskive.com/university/uni-197",
      "slug": "uni-197",
      "name": "University 160",
      "short_name": "Uni 197",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/b1f4e002b66d62462851b40532acabd2.jpg",
      "image_url_small": "memory://universities/91fae6f4d468217065cd8649cb368734.jpg",
      "image_thumb_url": "memory://universities/e4e9320ace1428f28d27669e4c4be05b.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T17:20:37.157Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-199",
      "html_url": "https://goskive.com/university/uni-199",
      "slug": "uni-199",
      "name": "University 162",
      "short_name": "Uni 199",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/360d6d83d043fdc4218a804b765a4702.jpg",
      "image_url_small": "memory://universities/319378b56e1cc9f2e2695d628d936ce9.jpg",
      "image_thumb_url": "memory://universities/7045abb6a368878fef76d678f0a36c1d.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T17:20:37.293Z",
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
	-H "Authorization: Bearer ad93004d6a980f7e0e98749669483bbc46e3b49b20645589f5889a1c787f8979"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 642b0f1d0a69e191eaabdb7e0b5529c15c4eb3ecdaf2a55461640347a8984519
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
    "id": 216,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/9a28ccf38a275b6d1ad2342b25885537.jpg",
    "image_url_small": "memory://universities/f27aa142e9320ce49a05bde9e1f20238.jpg",
    "image_thumb_url": "memory://universities/e11d4b5caac99abdaa473713f2408b12.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T17:20:37.010Z",
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
	-H "Authorization: Bearer 642b0f1d0a69e191eaabdb7e0b5529c15c4eb3ecdaf2a55461640347a8984519"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7a63abf36a4c2ea9b1d3bc04629c7989de16f08e08dba2e291b7997e93229e24
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":138,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 423,
    "id": 138,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 116,
    "additional_university_ids": [

    ],
    "discipline_id": 138,
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
    "chapters_updated_at": "2016-12-15T17:20:06.789Z",
    "updated_at": "2016-12-15T17:20:06.959Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 98,
        "updated_at": "2016-12-15T17:20:06.946Z",
        "course_id": 138,
        "author_id": 423,
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
        "id": 99,
        "updated_at": "2016-12-15T17:20:06.962Z",
        "course_id": 138,
        "author_id": 423,
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
        "id": 100,
        "updated_at": "2016-12-15T17:20:06.977Z",
        "course_id": 138,
        "author_id": 423,
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
    "topic_id": 138,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":138,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a63abf36a4c2ea9b1d3bc04629c7989de16f08e08dba2e291b7997e93229e24"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b7b050dc0d1fe6a6397bd85dfd45a6e422bf56df358b7f9e6cb79a160a25dfd3
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":137,"published":false}}
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
    "creator_id": 422,
    "id": 137,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "discipline_id": 137,
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
    "updated_at": "2016-12-15T17:20:06.738Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 137,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":137,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7b050dc0d1fe6a6397bd85dfd45a6e422bf56df358b7f9e6cb79a160a25dfd3"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 077ee460a4a11ba94a01719b3dfd82169b294c298d6f8823968203f65daa333c
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
      "creator_id": 396,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-79",
      "html_url": "https://goskive.com/course/fu-course-79",
      "slug": "fu-course-79",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "discipline_id": 115,
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
      "updated_at": "2016-12-15T17:20:03.910Z",
      "shortname": "fu-course-79",
      "topic_id": 115,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 79",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 396,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-80",
      "html_url": "https://goskive.com/course/fu-course-80",
      "slug": "fu-course-80",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "discipline_id": 116,
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
      "chapters_updated_at": "2016-12-15T17:20:03.728Z",
      "updated_at": "2016-12-15T17:20:04.197Z",
      "shortname": "fu-course-80",
      "topic_id": 116,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 80",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 077ee460a4a11ba94a01719b3dfd82169b294c298d6f8823968203f65daa333c"
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
      "creator_id": 416,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-95",
      "html_url": "https://goskive.com/course/fu-course-95",
      "slug": "fu-course-95",
      "university_id": 112,
      "additional_university_ids": [

      ],
      "discipline_id": 131,
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
      "updated_at": "2016-12-15T17:20:05.928Z",
      "shortname": "fu-course-95",
      "topic_id": 131,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 95",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 416,
      "id": 132,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-96",
      "html_url": "https://goskive.com/course/fu-course-96",
      "slug": "fu-course-96",
      "university_id": 112,
      "additional_university_ids": [

      ],
      "discipline_id": 132,
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
      "chapters_updated_at": "2016-12-15T17:20:05.748Z",
      "updated_at": "2016-12-15T17:20:06.210Z",
      "shortname": "fu-course-96",
      "topic_id": 132,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 96",
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
Authorization: Bearer 56d585cf3dd8c54c0f2727d0c2177a8c6bb0fe86681de651bc83c650b5b4199e
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
      "creator_id": 402,
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-83",
      "html_url": "https://goskive.com/course/fu-course-83",
      "slug": "fu-course-83",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "discipline_id": 119,
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
      "updated_at": "2016-12-15T17:20:04.491Z",
      "shortname": "fu-course-83",
      "topic_id": 119,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 83",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 402,
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-84",
      "html_url": "https://goskive.com/course/fu-course-84",
      "slug": "fu-course-84",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "discipline_id": 120,
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
      "updated_at": "2016-12-15T17:20:04.529Z",
      "shortname": "fu-course-84",
      "topic_id": 120,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 84",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56d585cf3dd8c54c0f2727d0c2177a8c6bb0fe86681de651bc83c650b5b4199e"
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
      "creator_id": 421,
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-99",
      "html_url": "https://goskive.com/course/fu-course-99",
      "slug": "fu-course-99",
      "university_id": 113,
      "additional_university_ids": [

      ],
      "discipline_id": 135,
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
      "updated_at": "2016-12-15T17:20:06.431Z",
      "shortname": "fu-course-99",
      "topic_id": 135,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 99",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 421,
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-100",
      "html_url": "https://goskive.com/course/fu-course-100",
      "slug": "fu-course-100",
      "university_id": 113,
      "additional_university_ids": [

      ],
      "discipline_id": 136,
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
      "updated_at": "2016-12-15T17:20:06.466Z",
      "shortname": "fu-course-100",
      "topic_id": 136,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 100",
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
Authorization: Bearer 698f3754a01154e5d8109a96dffa5c9ba3e55e3e4dac91c1b1792d4c595a3163
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
  "id": 459,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T17:20:10.408Z",
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
	-H "Authorization: Bearer 698f3754a01154e5d8109a96dffa5c9ba3e55e3e4dac91c1b1792d4c595a3163"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/426
Content-Type: application/json
Authorization: Bearer 7275d0d674e074b96ffbd599c2a4143633bbeae8c9ae6761d3d301a6eef74c6c
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
    "id": 426,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 119,
    "fields_of_study": [
      141,
      142
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T17:20:07.598Z",
    "updated_at": "2016-12-15T17:20:07.598Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/426" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7275d0d674e074b96ffbd599c2a4143633bbeae8c9ae6761d3d301a6eef74c6c"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/428
Content-Type: application/json
Authorization: Bearer c206056ae3c2e6f4c136b3aac81b49a1878bff42339e6939d8327d2d14e36cd2
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
    "id": 428,
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
    "created_at": "2016-12-15T17:20:07.689Z",
    "updated_at": "2016-12-15T17:20:07.689Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/428" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c206056ae3c2e6f4c136b3aac81b49a1878bff42339e6939d8327d2d14e36cd2"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/17
Content-Type: application/json
Authorization: Bearer fad09b063b8d919b551d44c6cc51f2e9cc0ca11571aa092ad412fcc2eb007e10
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fad09b063b8d919b551d44c6cc51f2e9cc0ca11571aa092ad412fcc2eb007e10"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/18
Content-Type: application/json
Authorization: Bearer ae2acfe98f643ba36cb01d93f1c26b8702bc9f616c33cb8e3c277ca30b0a9380
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
    "id": 18,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 125,
    "user_id": 846
  }
}
```



```shell
curl "api.goskive.com/v2/votes/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae2acfe98f643ba36cb01d93f1c26b8702bc9f616c33cb8e3c277ca30b0a9380"
```
