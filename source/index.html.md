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
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"25133b077b665e6d6c4febde6317783bbddfe59c3459d74838b0e3deeedcee9e","client_secret":"80f70135610570dbe894feda82d12ac1245d818561b4f73dfdbf3c5e68edb941"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"25133b077b665e6d6c4febde6317783bbddfe59c3459d74838b0e3deeedcee9e","client_secret":"80f70135610570dbe894feda82d12ac1245d818561b4f73dfdbf3c5e68edb941"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTRkZjdmMWM4NWQ0NGIxYmJiMTY5M2Y3ZGI2ZDFmYTEwMjkwYTYxMDg2MjJk
ZGIzMGM3MWU0NTQ1N2IzNDE4Njo1ZjI2ZmRiNWM5ODVkMGIxNmQ3ZDIxMGMw
NzVhN2NlMjA1ODQ0MjU4MGE3ODI1YTJmNWU3ZDNhNWExM2YxMjIz

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
	-u a4df7f1c85d44b1bbb1693f7db6d1fa10290a6108622ddb30c71e45457b34186:5f26fdb5c985d0b16d7d210c075a7ce2058442580a7825a2f5e7d3a5a13f1223
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7b22038f0b1beb498ee26ddbf6e5e98eb29510be72df93f7fd581c59c5f644d3","client_secret":"db1c9050a8b401bb37702b2c119d2aada4cecd604ce6b2460bba1f4151ec2f59"}
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
  "access_token": "b3a407fc2b7787a27329c2ab50be778feaa3e40b4f62b5548d9ba80536e1101b",
  "token_type": "bearer",
  "created_at": 1479389166
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7b22038f0b1beb498ee26ddbf6e5e98eb29510be72df93f7fd581c59c5f644d3","client_secret":"db1c9050a8b401bb37702b2c119d2aada4cecd604ce6b2460bba1f4151ec2f59"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDkxMzAzYjJmNDU4NzgzNDE2MGUzZmIxYmUxZDJmYjQ5YTExMTNkYTExZjZm
ZTJmYjhlNWQ2Y2I0NmNmMGE5Zjo0OGFiZTYyMmQ3NmU2ODVhNGY4NjNhMWU5
OTgzYjdkNGMyZmNlOGUzNTU1MGRkMjJlY2Q2ZjFiNjI1YTE4NjBk

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
  "access_token": "24a23f9a7b187e469cd2829e41f4f9928ec87d6bcd6d46eb30354988329943f2",
  "token_type": "bearer",
  "created_at": 1479389166
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u d91303b2f4587834160e3fb1be1d2fb49a1113da11f6fe2fb8e5d6cb46cf0a9f:48abe622d76e685a4f863a1e9983b7d4c2fce8e35550dd22ecd6f1b625a1860d
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
{"grant_type":"client_credentials","client_id":"50967fcad008010288fb71f6080baaf1c7a2dc8a46c7446daf800da54b07f203","client_secret":"438b8463537f5e9ee3488a9b599ddb30e410ac0a3ad93a97bc8810ae661f4738"}
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
  "access_token": "d37766777563dd98dea800eca41d01e429fcc9b3db6dfd4c0400c14019e6737c",
  "token_type": "bearer",
  "created_at": 1479389166
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"50967fcad008010288fb71f6080baaf1c7a2dc8a46c7446daf800da54b07f203","client_secret":"438b8463537f5e9ee3488a9b599ddb30e410ac0a3ad93a97bc8810ae661f4738"}' -X POST \
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
Authorization: Bearer abb09116a90a3ef08a133c7be1732c51ef37bc88d50e031f987a9f9c2c529cc1
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
    "company_id": 33,
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
	-H "Authorization: Bearer abb09116a90a3ef08a133c7be1732c51ef37bc88d50e031f987a9f9c2c529cc1"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/190/flashcards
Content-Type: application/json
Authorization: Bearer db3573cdc652b050b89a4988fe93102e2fcc44f6d6cd909d186660f8505b4bf7
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":190,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 971,
    "chapter_id": 190,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:26:54.048Z",
    "created_at": "2016-11-17T13:26:54.048Z",
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
curl "api.goskive.com/v2/chapters/190/flashcards" -d '{"flashcard":{"chapter_id":190,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db3573cdc652b050b89a4988fe93102e2fcc44f6d6cd909d186660f8505b4bf7"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/189/flashcards
Content-Type: application/json
Authorization: Bearer 94780c7520c61def658b0af342ab17734cfd550cc39ceff00259711dc9037e6d
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
      "author_id": 966,
      "chapter_id": 189,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:53.778Z",
      "created_at": "2016-11-17T13:26:53.778Z",
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
      "author_id": 966,
      "chapter_id": 189,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:53.815Z",
      "created_at": "2016-11-17T13:26:53.815Z",
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
      "author_id": 966,
      "chapter_id": 189,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:53.851Z",
      "created_at": "2016-11-17T13:26:53.851Z",
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
curl "api.goskive.com/v2/chapters/189/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94780c7520c61def658b0af342ab17734cfd550cc39ceff00259711dc9037e6d"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/35/questions
Content-Type: application/json
Authorization: Bearer ec51aa71f43c0104965708fe3a52a3a4d0d8b902779a24522bae613503e28e66
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":35,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 200,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:25:47.876Z",
    "created_at": "2016-11-17T13:25:47.876Z",
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
        "id": 59,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 60,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 61,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 62,
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
curl "api.goskive.com/v2/chapters/35/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":35,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec51aa71f43c0104965708fe3a52a3a4d0d8b902779a24522bae613503e28e66"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/36/questions
Content-Type: application/json
Authorization: Bearer f89c89ba0498c729eb864c0f0b7d11241227c1113e976693cdd0b7c2a4e9f2a5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 203,
    "chapter_id": 36,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:25:48.570Z",
    "created_at": "2016-11-17T13:25:48.570Z",
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
curl "api.goskive.com/v2/chapters/36/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f89c89ba0498c729eb864c0f0b7d11241227c1113e976693cdd0b7c2a4e9f2a5"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/38/questions
Content-Type: application/json
Authorization: Bearer 75731ec7a0830006793ad474c5919b5febae31396da43be8e3236071f4856c4d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 209,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:25:49.578Z",
    "created_at": "2016-11-17T13:25:49.578Z",
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
        "id": 68,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 69,
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
curl "api.goskive.com/v2/chapters/38/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75731ec7a0830006793ad474c5919b5febae31396da43be8e3236071f4856c4d"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/37/questions
Content-Type: application/json
Authorization: Bearer f9c871965047db0bd378999e1015ecc8bdc0e3ea5bbc2f775bec937e17bb3c82
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":37,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 206,
    "chapter_id": 37,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:25:49.074Z",
    "created_at": "2016-11-17T13:25:49.074Z",
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
curl "api.goskive.com/v2/chapters/37/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":37,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9c871965047db0bd378999e1015ecc8bdc0e3ea5bbc2f775bec937e17bb3c82"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/40/questions
Content-Type: application/json
Authorization: Bearer 140bf8709399bdb005aa351674c95a03e8ca6d199649d8b38566fd36b7f251e9
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 215,
      "chapter_id": 40,
      "position": 30,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:25:50.313Z",
      "created_at": "2016-11-17T13:25:50.195Z",
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
          "id": 70,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 71,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 216,
      "chapter_id": 40,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:25:50.499Z",
      "created_at": "2016-11-17T13:25:50.380Z",
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
      "author_id": 217,
      "chapter_id": 40,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:25:50.693Z",
      "created_at": "2016-11-17T13:25:50.569Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/40/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 140bf8709399bdb005aa351674c95a03e8ca6d199649d8b38566fd36b7f251e9"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/49
Content-Type: application/json
Authorization: Bearer bfcd006faaa02b959f02fac57615b78296d5d12216585e23ad6c8a47ff0c5a2e
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
curl "api.goskive.com/v2/chapters/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfcd006faaa02b959f02fac57615b78296d5d12216585e23ad6c8a47ff0c5a2e"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/50
Content-Type: application/json
Authorization: Bearer 53fc502ef728be5ccaf745e2923dd87e2a6ee687835b334377d3272889858d6f
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
curl "api.goskive.com/v2/chapters/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53fc502ef728be5ccaf745e2923dd87e2a6ee687835b334377d3272889858d6f"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/45
Content-Type: application/json
Authorization: Bearer e0ebf3474d3ef00eff625317ed3a0af221b55850813faab85a8d908bbdfccf56
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
curl "api.goskive.com/v2/chapters/45" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0ebf3474d3ef00eff625317ed3a0af221b55850813faab85a8d908bbdfccf56"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/48
Content-Type: application/json
Authorization: Bearer aa218cb57d34897680482350763d5f800ed15dc647293434a5bd7cc411de63eb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa218cb57d34897680482350763d5f800ed15dc647293434a5bd7cc411de63eb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/52
Content-Type: application/json
Authorization: Bearer 23f84261ff7056ddeeb00d6f773ed5d6bec94ea8884a5e2ecd5d43499e73c4ce
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
    "id": 52,
    "updated_at": "2016-11-17T13:25:55.544Z",
    "course_id": 69,
    "author_id": 273,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-17T13:25:54.954Z",
    "questions_updated_at": "2016-11-17T13:25:54.954Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 277,
        "chapter_id": 52,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:55.526Z",
        "created_at": "2016-11-17T13:25:55.526Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 275,
        "chapter_id": 52,
        "position": 40,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:55.382Z",
        "created_at": "2016-11-17T13:25:55.256Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/52" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23f84261ff7056ddeeb00d6f773ed5d6bec94ea8884a5e2ecd5d43499e73c4ce"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/47
Content-Type: application/json
Authorization: Bearer 0bd124840ec69c270a506ade01a3b166c1fa365fc4c71fd877b9256d00b95520
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
    "id": 47,
    "updated_at": "2016-11-17T13:25:53.880Z",
    "course_id": 64,
    "author_id": 259,
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
curl "api.goskive.com/v2/chapters/47" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bd124840ec69c270a506ade01a3b166c1fa365fc4c71fd877b9256d00b95520"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 374023abac86f9ef2279a62b576aa15c76898a204911d13e9381655f328ded64
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
    "id": 4,
    "author_id": 163,
    "reply_to_id": 3,
    "created_at": "2016-11-17T13:25:41.294Z",
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
curl "api.goskive.com/v2/comments/3/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 374023abac86f9ef2279a62b576aa15c76898a204911d13e9381655f328ded64"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 67c9bd863a4005664f078aa8663f9d30df3b858a29652596a5bcf96f7ff35c18
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
curl "api.goskive.com/v2/comments/2/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67c9bd863a4005664f078aa8663f9d30df3b858a29652596a5bcf96f7ff35c18"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer fa8a351354635f451486f5a10deaa50904beb848f4168ed543c7f02f3a949324
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
curl "api.goskive.com/v2/comments/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa8a351354635f451486f5a10deaa50904beb848f4168ed543c7f02f3a949324"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/50/republish
Content-Type: application/json
Authorization: Bearer d77cf5770fcf905fd8008ff58ebe743e306528ab9a6a73af950d1ac16f71a27a
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
curl "api.goskive.com/v2/comments/50/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d77cf5770fcf905fd8008ff58ebe743e306528ab9a6a73af950d1ac16f71a27a"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/46
Content-Type: application/json
Authorization: Bearer b340296888a83c098f8524b7258f4baf670518411b72d582a38c7d6636ae258e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b340296888a83c098f8524b7258f4baf670518411b72d582a38c7d6636ae258e"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/45/report
Content-Type: application/json
Authorization: Bearer b2d806c589aa0a544efbd8105350e2ac1c6ab7ea84d1c9711f4cd43f0d7a831b
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/45/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2d806c589aa0a544efbd8105350e2ac1c6ab7ea84d1c9711f4cd43f0d7a831b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/9
Content-Type: application/json
Authorization: Bearer bdec400e075336eace242c120cc6a81056fa3c8f76c59d1bb0ca7f71e069efd9
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
    "id": 9,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-17T13:26:03.461Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdec400e075336eace242c120cc6a81056fa3c8f76c59d1bb0ca7f71e069efd9"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 7e9d9146489099e3400737c2f2f61223f41afb326e1e0b89132385959b212f71
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
      "id": 10,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-17T13:26:03.536Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-17T13:26:03.540Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-17T13:26:03.544Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e9d9146489099e3400737c2f2f61223f41afb326e1e0b89132385959b212f71"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/35/company_profiles
Content-Type: application/json
Authorization: Bearer 03ccec93fe2e3e71e54e93c02fa6bee8a19bb7cccdd0df2eab45b1bf870fc025
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
curl "api.goskive.com/v2/companies/35/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03ccec93fe2e3e71e54e93c02fa6bee8a19bb7cccdd0df2eab45b1bf870fc025"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/34/company_profiles
Content-Type: application/json
Authorization: Bearer 89126c9bdf84511c5ff6fb80756b6c6f79af6e0a514fb4aed335e8b795915d2a
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
curl "api.goskive.com/v2/companies/34/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89126c9bdf84511c5ff6fb80756b6c6f79af6e0a514fb4aed335e8b795915d2a"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 81154078d00019d1b096f6fae3707109013664391cf3f5be41089df00822d80b
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
      "id": 8,
      "title": "Campaign 8",
      "company_id": 27,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 30,
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
	-H "Authorization: Bearer 81154078d00019d1b096f6fae3707109013664391cf3f5be41089df00822d80b"
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
Authorization: Bearer 9325a2707edcdb0eee8406c63ce84e64416428a146f158e26f87f86b39c87219
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
	-H "Authorization: Bearer 9325a2707edcdb0eee8406c63ce84e64416428a146f158e26f87f86b39c87219"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0a7147a918c1ea7b4eaf75338268ad547d55655bc507a28070d93d4235a8107b
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
    "id": 160,
    "updated_at": "2016-11-17T13:26:42.086Z",
    "course_id": 281,
    "author_id": 865,
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
	-H "Authorization: Bearer 0a7147a918c1ea7b4eaf75338268ad547d55655bc507a28070d93d4235a8107b"
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
      "id": 142,
      "updated_at": "2016-11-17T13:26:39.533Z",
      "course_id": 271,
      "author_id": 824,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 124",
      "position": 1
    },
    {
      "id": 143,
      "updated_at": "2016-11-17T13:26:39.560Z",
      "course_id": 271,
      "author_id": 825,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 125",
      "position": 2
    },
    {
      "id": 144,
      "updated_at": "2016-11-17T13:26:39.892Z",
      "course_id": 271,
      "author_id": 826,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-17T13:26:39.459Z",
      "questions_updated_at": "2016-11-17T13:26:39.459Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 126",
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
Authorization: Bearer 3772a54fdead4d8c4827b8cc2224a921900d860b3db3cfde4be53a8e0b7d7aba
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
      "id": 148,
      "updated_at": "2016-11-17T13:26:40.277Z",
      "course_id": 274,
      "author_id": 835,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 130",
      "position": 1
    },
    {
      "id": 149,
      "updated_at": "2016-11-17T13:26:40.306Z",
      "course_id": 274,
      "author_id": 836,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 131",
      "position": 2
    },
    {
      "id": 150,
      "updated_at": "2016-11-17T13:26:40.676Z",
      "course_id": 274,
      "author_id": 837,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-17T13:26:40.201Z",
      "questions_updated_at": "2016-11-17T13:26:40.201Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 132",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3772a54fdead4d8c4827b8cc2224a921900d860b3db3cfde4be53a8e0b7d7aba"
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
      "id": 145,
      "updated_at": "2016-11-17T13:26:40.019Z",
      "course_id": 272,
      "author_id": 830,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 127",
      "position": 1
    },
    {
      "id": 146,
      "updated_at": "2016-11-17T13:26:40.046Z",
      "course_id": 272,
      "author_id": 831,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 128",
      "position": 2
    },
    {
      "id": 147,
      "updated_at": "2016-11-17T13:26:40.073Z",
      "course_id": 272,
      "author_id": 832,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 129",
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
Authorization: Bearer 9eb519ca7d76ec0225f344e2d973727f6e51a92e15336cebdf9ea204963a3409
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
      "id": 151,
      "updated_at": "2016-11-17T13:26:40.936Z",
      "course_id": 276,
      "author_id": 844,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 133",
      "position": 1
    },
    {
      "id": 152,
      "updated_at": "2016-11-17T13:26:40.964Z",
      "course_id": 276,
      "author_id": 845,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 134",
      "position": 2
    },
    {
      "id": 153,
      "updated_at": "2016-11-17T13:26:40.990Z",
      "course_id": 276,
      "author_id": 846,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 135",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9eb519ca7d76ec0225f344e2d973727f6e51a92e15336cebdf9ea204963a3409"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f7f96342f85c7a8fa43b027cc034b0f27a59a08da62e2afbb921f3f8a118f647
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
    "course_id": 194,
    "user_id": 597,
    "updated_at": "2016-11-17T13:26:17.764Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7f96342f85c7a8fa43b027cc034b0f27a59a08da62e2afbb921f3f8a118f647"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer fd31aae0ca4903b3c3952de322454c54bebdc93316349f08650c94af06100beb
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
      "course_id": 191,
      "user_id": 589,
      "updated_at": "2016-11-17T13:26:17.343Z"
    },
    {
      "id": 5,
      "course_id": 191,
      "user_id": 590,
      "updated_at": "2016-11-17T13:26:17.357Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd31aae0ca4903b3c3952de322454c54bebdc93316349f08650c94af06100beb"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/59/files
Content-Type: application/json
Authorization: Bearer dd9629ee55e4d633aae46ce09948fe974689cf51cee146810e0f0665e2c14e12
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
      "id": 7,
      "uploader": {
        "id": 239,
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
        "created_at": "2016-11-17T13:25:52.331Z",
        "updated_at": "2016-11-17T13:25:52.331Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T13:25:52.341Z",
      "updated_at": "2016-11-17T13:25:52.341Z",
      "course_id": 59,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 8,
      "uploader": {
        "id": 240,
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
        "created_at": "2016-11-17T13:25:52.348Z",
        "updated_at": "2016-11-17T13:25:52.348Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T13:25:52.357Z",
      "updated_at": "2016-11-17T13:25:52.357Z",
      "course_id": 59,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 241,
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
        "created_at": "2016-11-17T13:25:52.365Z",
        "updated_at": "2016-11-17T13:25:52.365Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T13:25:52.381Z",
      "updated_at": "2016-11-17T13:25:52.381Z",
      "course_id": 59,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/59/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd9629ee55e4d633aae46ce09948fe974689cf51cee146810e0f0665e2c14e12"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/58/files
Content-Type: application/json
Authorization: Bearer 8c570539ead333761663f70bceec9b151a0d6f3fbc59d675e1b97b0d1f895f75
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
    "id": 6,
    "uploader": {
      "id": 237,
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
      "created_at": "2016-11-17T13:25:52.149Z",
      "updated_at": "2016-11-17T13:25:52.149Z"
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
    "created_at": "2016-11-17T13:25:52.194Z",
    "updated_at": "2016-11-17T13:25:52.194Z",
    "course_id": 58,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/58/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c570539ead333761663f70bceec9b151a0d6f3fbc59d675e1b97b0d1f895f75"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/57/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer d3e95928b50f3cc793a5997142df92e996020fad5952949befe2c00506f89a9e
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
    "key": "cache/2222ba48f76bec4a6ad23ca312fec671.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xN1QxNDoyNTo1MloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzIyMjJiYTQ4Zjc2YmVjNGE2YWQyM2NhMzEyZmVjNjcxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTcvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE3VDEzMjU1MloifV19",
    "x-amz-credential": "FAKE/20161117/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161117T132552Z",
    "x-amz-signature": "2b04b73b948a74a3f7d77d42bc865fae39709144f045d87eaecf333ba5ff402f"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/57/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3e95928b50f3cc793a5997142df92e996020fad5952949befe2c00506f89a9e"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer c8f9c8c701f4b0a1cb64454a688e1ea781c5f5059d8a6dc3093a3ffcc4e20e65
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
	-H "Authorization: Bearer c8f9c8c701f4b0a1cb64454a688e1ea781c5f5059d8a6dc3093a3ffcc4e20e65"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8d723efc18ea02b6c313da4e8d21c2c2e30a2d0bc97c781fd0e702130793a098
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
	-H "Authorization: Bearer 8d723efc18ea02b6c313da4e8d21c2c2e30a2d0bc97c781fd0e702130793a098"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3ba3954ee0a1f701e8e5fd6851ea89b7010965ce746d8031ecc6ee916a44316c
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
	-H "Authorization: Bearer 3ba3954ee0a1f701e8e5fd6851ea89b7010965ce746d8031ecc6ee916a44316c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6ed9cb4241c34a0680b49cdc5e28b947fbecf632b0585f23323262c07977260c
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
	-H "Authorization: Bearer 6ed9cb4241c34a0680b49cdc5e28b947fbecf632b0585f23323262c07977260c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2a1f7baf7a1568463d3808949c7348ae382805e6d8d69d359d2725db3a856e66
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
	-H "Authorization: Bearer 2a1f7baf7a1568463d3808949c7348ae382805e6d8d69d359d2725db3a856e66"
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
    "creator_id": 768,
    "id": 257,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 242,
    "additional_university_ids": [

    ],
    "discipline_id": 265,
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
    "chapters_updated_at": "2016-11-17T13:26:30.235Z",
    "updated_at": "2016-11-17T13:26:32.014Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 768,
        "chapter_id": 124,
        "position": 76,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:30.480Z",
        "created_at": "2016-11-17T13:26:30.327Z",
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
            "id": 162,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 163,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 768,
        "chapter_id": 125,
        "position": 78,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:30.965Z",
        "created_at": "2016-11-17T13:26:30.806Z",
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
            "id": 166,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 167,
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
        "id": 124,
        "updated_at": "2016-11-17T13:26:31.959Z",
        "course_id": 257,
        "author_id": 768,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T13:26:30.235Z",
        "questions_updated_at": "2016-11-17T13:26:30.235Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 106",
        "position": 1
      },
      {
        "id": 125,
        "updated_at": "2016-11-17T13:26:32.004Z",
        "course_id": 257,
        "author_id": 768,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T13:26:30.235Z",
        "questions_updated_at": "2016-11-17T13:26:30.235Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 107",
        "position": 2
      }
    ],
    "topic_id": 264,
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
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 26cf79aacc8e7bffcb227185505887f7338cb5042134eec8ca07bd2070a6712a
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
    "creator_id": 773,
    "id": 258,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 243,
    "additional_university_ids": [

    ],
    "discipline_id": 266,
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
    "chapters_updated_at": "2016-11-17T13:26:32.070Z",
    "updated_at": "2016-11-17T13:26:33.878Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 774,
        "chapter_id": 126,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:33.638Z",
        "created_at": "2016-11-17T13:26:33.638Z",
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
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 774,
        "chapter_id": 127,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:33.720Z",
        "created_at": "2016-11-17T13:26:33.720Z",
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
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 774,
        "chapter_id": 126,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:33.685Z",
        "created_at": "2016-11-17T13:26:33.685Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 774,
        "chapter_id": 127,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:33.766Z",
        "created_at": "2016-11-17T13:26:33.766Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 774,
        "chapter_id": 126,
        "position": 82,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:32.329Z",
        "created_at": "2016-11-17T13:26:32.170Z",
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
            "id": 174,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 175,
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
        "author_id": 774,
        "chapter_id": 126,
        "position": 83,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:32.565Z",
        "created_at": "2016-11-17T13:26:32.410Z",
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
            "id": 176,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 177,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 774,
        "chapter_id": 127,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:32.827Z",
        "created_at": "2016-11-17T13:26:32.666Z",
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
            "id": 178,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 179,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 774,
        "chapter_id": 127,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:33.061Z",
        "created_at": "2016-11-17T13:26:32.909Z",
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
      }
    ],
    "chapters": [
      {
        "id": 126,
        "updated_at": "2016-11-17T13:26:33.823Z",
        "course_id": 258,
        "author_id": 773,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T13:26:32.070Z",
        "questions_updated_at": "2016-11-17T13:26:32.070Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 108",
        "position": 1
      },
      {
        "id": 127,
        "updated_at": "2016-11-17T13:26:33.868Z",
        "course_id": 258,
        "author_id": 773,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T13:26:32.070Z",
        "questions_updated_at": "2016-11-17T13:26:32.070Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 109",
        "position": 2
      }
    ],
    "topic_id": 265,
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
	-H "Authorization: Bearer 26cf79aacc8e7bffcb227185505887f7338cb5042134eec8ca07bd2070a6712a"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/255/pin
Content-Type: application/json
Authorization: Bearer e3864e8c7ddf8fe02882d104aec5b66d59ecb6cdcab10c3d647f3498822644fb
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/255/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3864e8c7ddf8fe02882d104aec5b66d59ecb6cdcab10c3d647f3498822644fb"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/254/pin
Content-Type: application/json
Authorization: Bearer 9e5dd816afa73de97e3d1c81d7948d123c50334d1e604832a717bf953be89443
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/254/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e5dd816afa73de97e3d1c81d7948d123c50334d1e604832a717bf953be89443"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9aaaf60b1183ab4ed4c55b1c66849e6cc83802ac2597a4a23c2b68df211145b4
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
    "creator_id": 751,
    "id": 250,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 235,
    "additional_university_ids": [

    ],
    "discipline_id": 258,
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
    "updated_at": "2016-11-17T13:26:27.675Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 257,
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
	-H "Authorization: Bearer 9aaaf60b1183ab4ed4c55b1c66849e6cc83802ac2597a4a23c2b68df211145b4"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 62952ac0730459b3c962840725e9e1e47b0839ed3fe5a5a11923c3d53e04cb51
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
    "id": 956,
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
    "created_at": "2016-11-17T13:26:52.789Z",
    "updated_at": "2016-11-17T13:26:52.789Z",
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
	-H "Authorization: Bearer 62952ac0730459b3c962840725e9e1e47b0839ed3fe5a5a11923c3d53e04cb51"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c18831bda7659763368dc3ce732650752bbd4b46d4d15222cf7cd468e7e665c6
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[317]}
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
    "id": 952,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      317
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-17T13:26:52.530Z",
    "updated_at": "2016-11-17T13:26:52.564Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[317]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c18831bda7659763368dc3ce732650752bbd4b46d4d15222cf7cd468e7e665c6"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 31920d4389c383d72eb09c4aa43b70c62f04caa3a7b204e4654e526df40e0413
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
    "id": 955,
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
    "created_at": "2016-11-17T13:26:52.721Z",
    "updated_at": "2016-11-17T13:26:52.721Z",
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
	-H "Authorization: Bearer 31920d4389c383d72eb09c4aa43b70c62f04caa3a7b204e4654e526df40e0413"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 24f036fa8fcffd7d308fce44367f1c6d45d598048fd0dee15b40276ddfe56225
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[318]}
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
    "id": 953,
    "first_name": "Magnus",
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
    "created_at": "2016-11-17T13:26:52.603Z",
    "updated_at": "2016-11-17T13:26:52.603Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[318]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24f036fa8fcffd7d308fce44367f1c6d45d598048fd0dee15b40276ddfe56225"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 9a14210ee20abd000fe77302f369a26f6bedfe4c35c3dd65bb854f8fc6226bd5
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

316
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
    "id": 951,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9e00d517ecd522cf0cb8cd668e08c19515f40779.jpg",
    "university_id": null,
    "fields_of_study": [
      316
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-17T13:26:52.194Z",
    "updated_at": "2016-11-17T13:26:52.474Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/18eebe194de1df1f46f0f9d4ec1d14f86de436eb.jpg",
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

316
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 9a14210ee20abd000fe77302f369a26f6bedfe4c35c3dd65bb854f8fc6226bd5"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer b6be14b66a5011f16e537d157c481573255c8f80a9b1ccf12196b5d0c6cdcc6a
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
      "id": 2,
      "bookmarkable_id": 37,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 38,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 39,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6be14b66a5011f16e537d157c481573255c8f80a9b1ccf12196b5d0c6cdcc6a"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 38a6ca5f540b69cc967f33b679ccedf6ad1398ae23d14cdf3f5f39f777335d8a
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
      "title": "Campaign 2",
      "company_id": 5,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 2,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/9eceef98bbb4cbbf925777c91787755d8353de98.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/a56a082a30d2de9bc36364cd610c75501bd3b7d5.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "id": 2,
          "image_url_absolute": "banners/889019b341716d48f4f28718872d4f688cd18499.png",
          "target_url": "http://goskive.com",
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 3,
      "title": "Campaign 3",
      "company_id": 6,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 3,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
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
          "id": 3,
          "image_url_absolute": "banners/69ad62d43dc80a20595b9668db2a008bef68d956.png",
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
	-H "Authorization: Bearer 38a6ca5f540b69cc967f33b679ccedf6ad1398ae23d14cdf3f5f39f777335d8a"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 4c85e56f1351c47db3b030ea4dd78c95c3039161c8c2f7cee4142ea6dbc46d27
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 1,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 1,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/0adf1955ecfb39ff0d02f85dd384e7aeaf694927.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/39195f7a12fa003c1584dcee68597ed4a180cb4b.png",
          "widgets": [

          ]
        }
      ],
      "banners": [
        {
          "id": 1,
          "image_url_absolute": "banners/8dbf7d28f3cbdc6d654d6324af20a11fe3653b85.png",
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
	-H "Authorization: Bearer 4c85e56f1351c47db3b030ea4dd78c95c3039161c8c2f7cee4142ea6dbc46d27"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer e5bce703314df8e6e887d3d415e5e14ea8d7c55940261dcdf2069d0c17fc9a72
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
      "creator_id": 534,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-126",
      "html_url": "https://goskive.com/course/mit-course-126",
      "slug": "mit-course-126",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "discipline_id": 155,
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
      "updated_at": "2016-11-17T13:26:12.225Z",
      "shortname": "mit-course-126",
      "topic_id": 154,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 535,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-127",
      "html_url": "https://goskive.com/course/mit-course-127",
      "slug": "mit-course-127",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "discipline_id": 156,
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
      "updated_at": "2016-11-17T13:26:12.334Z",
      "shortname": "mit-course-127",
      "topic_id": 155,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5bce703314df8e6e887d3d415e5e14ea8d7c55940261dcdf2069d0c17fc9a72"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 10b720cd81b49cbee9259fe1eab5ec123581912cb472efece087ffb5eececcc3
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
        "created_at": "2016-11-17T13:25:40.321Z",
        "updated_at": "2016-11-17T13:25:40.321Z",
        "file_url": "memory://d3e1c600b0df384e70adf7aa5de3a707.pdf",
        "course_id": 37,
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
        "created_at": "2016-11-17T13:25:40.394Z",
        "updated_at": "2016-11-17T13:25:40.394Z",
        "file_url": "memory://b1137ed2b9b6ed58d76c3474edf77eb0.pdf",
        "course_id": 38,
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
        "created_at": "2016-11-17T13:25:40.464Z",
        "updated_at": "2016-11-17T13:25:40.464Z",
        "file_url": "memory://c87daa83d98ac41e1bcbf20a6ce2e3c6.pdf",
        "course_id": 39,
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
	-H "Authorization: Bearer 10b720cd81b49cbee9259fe1eab5ec123581912cb472efece087ffb5eececcc3"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 9e895f05831fca5c774c6dbb83425937d2074864de40b0b5e88617edef266b39
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T13:26:19.877Z"
      },
      "created_at": "2016-11-17T13:26:19.880Z",
      "updated_at": "2016-11-17T13:26:19.880Z",
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
      "company_id": 19,
      "company": {
        "id": 19,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T13:26:19.888Z"
      },
      "created_at": "2016-11-17T13:26:19.891Z",
      "updated_at": "2016-11-17T13:26:19.891Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e895f05831fca5c774c6dbb83425937d2074864de40b0b5e88617edef266b39"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a539753e9d25d2f5b4e85f002df56b437243eb111a20d63a3598e0c69ed353d9
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 13",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T13:26:19.713Z"
      },
      "created_at": "2016-11-17T13:26:19.718Z",
      "updated_at": "2016-11-17T13:26:19.718Z",
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T13:26:19.732Z"
      },
      "created_at": "2016-11-17T13:26:19.735Z",
      "updated_at": "2016-11-17T13:26:19.735Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a539753e9d25d2f5b4e85f002df56b437243eb111a20d63a3598e0c69ed353d9"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 88cb895877a2bb5aac84ceb50519df32490b613019f2c46f25882badf8c12cd0
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
      "id": 3,
      "created_at": "2016-11-17T13:25:56.501Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-11-17T13:25:56.604Z",
      "author_id": "292",
      "thread_subject_id": "72",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 4,
      "created_at": "2016-11-17T13:25:56.592Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-11-17T13:25:56.607Z",
      "author_id": "295",
      "thread_subject_id": "73",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-11-17T13:25:56.999Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-11-17T13:25:56.999Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-11-17T13:25:57.379Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-11-17T13:25:57.379Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 7,
      "created_at": "2016-11-17T13:25:57.775Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-11-17T13:25:57.775Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 8,
      "created_at": "2016-11-17T13:25:58.076Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 50,
      "updated_at": "2016-11-17T13:25:58.076Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-11-17T13:25:58.384Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 51,
      "updated_at": "2016-11-17T13:25:58.384Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-11-17T13:25:58.684Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 52,
      "updated_at": "2016-11-17T13:25:58.684Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88cb895877a2bb5aac84ceb50519df32490b613019f2c46f25882badf8c12cd0"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/2
Content-Type: application/json
Authorization: Bearer 3b45392bbebc076ce6f864bcd8ce11d6482d8c90a693dac6a2ea9013fca8166f
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-17T13:15:56.000Z"}}
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
    "id": 2,
    "created_at": "2016-11-17T13:25:56.345Z",
    "read_at": "2016-11-17T13:15:56.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 5,
    "updated_at": "2016-11-17T13:25:56.398Z",
    "author_id": "288",
    "thread_subject_id": "71",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/2" -d '{"notification":{"read_at":"2016-11-17T13:15:56.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b45392bbebc076ce6f864bcd8ce11d6482d8c90a693dac6a2ea9013fca8166f"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 2866c57b85ea15f2307048759a0d8849110ec571e501d4f494c681d0ab1ad463
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
      "id": 4,
      "course_id": 35,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-17T13:25:39.962Z",
      "course_published": true,
      "updated_at": "2016-11-17T13:25:39.955Z"
    },
    {
      "id": 5,
      "course_id": 36,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-17T13:25:40.040Z",
      "course_published": true,
      "updated_at": "2016-11-17T13:25:40.032Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2866c57b85ea15f2307048759a0d8849110ec571e501d4f494c681d0ab1ad463"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer 001bc602f151a1f94026f3a1847ee08b05b1acfe6157c5d12184760c6d7796bf
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
    "course_id": 31,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-17T13:25:39.473Z",
    "course_published": true,
    "updated_at": "2016-11-17T13:25:39.464Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 001bc602f151a1f94026f3a1847ee08b05b1acfe6157c5d12184760c6d7796bf"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 72e1791b37a43b12858cf3ff255eeef8acc4ef4350c065a72c3f3455d9283bfa
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
    "id": 3,
    "course_id": 34,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-17T13:25:39.869Z",
    "course_published": true,
    "updated_at": "2016-11-17T13:25:39.858Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72e1791b37a43b12858cf3ff255eeef8acc4ef4350c065a72c3f3455d9283bfa"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f457151dd81247d151ee0755a3767cdc875d463d523e0bb73516dc33a6dbf7dc
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
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 98,
      "user_id": 802
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 99,
      "user_id": 802
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 802
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 101,
      "user_id": 802
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f457151dd81247d151ee0755a3767cdc875d463d523e0bb73516dc33a6dbf7dc"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/97
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
    "id": 97,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 97,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 97
      },
      {
        "id": 98,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 97
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/97" -X GET \
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
      "id": 98,
      "name": "Persevering 24/7 matrices",
      "name_translations": {
        "en": "Persevering 24/7 matrices"
      }
    },
    {
      "id": 99,
      "name": "Switchable maximized knowledge user",
      "name_translations": {
        "en": "Switchable maximized knowledge user"
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
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer 54bb6e9ff1c1375766af57007cf7882d5ac29a856a1613b66258e5fb30128bc8
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
    "id": 1,
    "user_id": 10,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-17T13:25:31.280Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/1/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54bb6e9ff1c1375766af57007cf7882d5ac29a856a1613b66258e5fb30128bc8"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/6/fix
Content-Type: application/json
Authorization: Bearer 09f1db51e07b64f7e3e5d34d018fa7a9cb697009e4b3bd93c3436f3fa5f77a1b
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
    "user_id": 35,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-17T13:25:32.724Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/6/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09f1db51e07b64f7e3e5d34d018fa7a9cb697009e4b3bd93c3436f3fa5f77a1b"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/8
Content-Type: application/json
Authorization: Bearer 7d90b27c1775c0dec914d7e2bcf164c2d2e5eaa38ae16d5f1370be9a222b9943
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
    "user_id": 45,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T13:25:33.378Z",
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
	-H "Authorization: Bearer 7d90b27c1775c0dec914d7e2bcf164c2d2e5eaa38ae16d5f1370be9a222b9943"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer a3583a54d0ae7f4b68230ee526c14e799ebc768471541d330308c5aead5ed3a0
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
	-H "Authorization: Bearer a3583a54d0ae7f4b68230ee526c14e799ebc768471541d330308c5aead5ed3a0"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer 5a277b1faee07fa4e0cfacb15050ff63f98f4db1c4931da1f93483162523df69
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
	-H "Authorization: Bearer 5a277b1faee07fa4e0cfacb15050ff63f98f4db1c4931da1f93483162523df69"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer 6b8a43051e8fd5a2d019f57c505668f5d4a001b6bcb366ea53edc777443ce900
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
	-H "Authorization: Bearer 6b8a43051e8fd5a2d019f57c505668f5d4a001b6bcb366ea53edc777443ce900"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/9
Content-Type: application/json
Authorization: Bearer cd0cdf8419979c905d5428f004cf6c2fa57bf61512a156eb23a6370fd5a68afb
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
    "user_id": 50,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T13:25:33.676Z",
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
	-H "Authorization: Bearer cd0cdf8419979c905d5428f004cf6c2fa57bf61512a156eb23a6370fd5a68afb"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer c207ae504530b9d3143a365df8e00397adf64f33194fcd95840a836a6b1fd5f6
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
curl "api.goskive.com/v2/files/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c207ae504530b9d3143a365df8e00397adf64f33194fcd95840a836a6b1fd5f6"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/22/bookmark
Content-Type: application/json
Authorization: Bearer 82aae71df9f99bd47a3dcf4d40e52b5618ce13ce08a18a4d235759480a80f121
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/22/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82aae71df9f99bd47a3dcf4d40e52b5618ce13ce08a18a4d235759480a80f121"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer a1ff16b70559046080b62a1bdafce028907017383ee42bad38ee1883c78b6dbd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1ff16b70559046080b62a1bdafce028907017383ee42bad38ee1883c78b6dbd"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/20
Content-Type: application/json
Authorization: Bearer b9d51a8bd5c2eb87acd0a523700bcdff6e4c78f03653df60d11b4965a0c767aa
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/d65d260a285dce36063e05348a59634a.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161117%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161117T132619Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f4bd6a2af194522018d1fdfd0c2dd71d66693ceb96b5003d59b78a4fd56c3075",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9d51a8bd5c2eb87acd0a523700bcdff6e4c78f03653df60d11b4965a0c767aa"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/13/preview
Content-Type: application/json
Authorization: Bearer b7458160dc714f20e78b000dcef01b3c76252e85f76e14159df88a47bb34ecd0
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/c512e5324e136482645db9629dfc44ab.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161117%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161117T132618Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=496e292e4439976ff75899ad2cfbd3673533a1375aaa8dc670067282505aa960",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/13/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7458160dc714f20e78b000dcef01b3c76252e85f76e14159df88a47bb34ecd0"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/17/metadata
Content-Type: application/json
Authorization: Bearer ffab609fa035aa235d6acbb130bd31e1af96c5de508960a413e9b6eda04844ff
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
    "id": 17,
    "uploader": {
      "id": 618,
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
      "created_at": "2016-11-17T13:26:18.919Z",
      "updated_at": "2016-11-17T13:26:18.919Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-17T13:26:18.992Z",
    "updated_at": "2016-11-17T13:26:18.992Z",
    "course_id": 202,
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
curl "api.goskive.com/v2/files/17/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffab609fa035aa235d6acbb130bd31e1af96c5de508960a413e9b6eda04844ff"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/4/matched_courses?required_cu_count=2
Authorization: Bearer 0673d3c7bda52d52440fcf4fce20c864a8fb62f525d7f0d9c4c418ad9000cc43
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
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-0de3ddd5-1f43-4d79-9cd7-006aaa2dc6d0",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-0de3ddd5-1f43-4d79-9cd7-006aaa2dc6d0",
      "slug": "mit-the-great-british-bake-off-0de3ddd5-1f43-4d79-9cd7-006aaa2dc6d0",
      "university_id": 51,
      "additional_university_ids": [

      ],
      "discipline_id": 49,
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
      "chapters_updated_at": "2016-11-17T13:25:43.246Z",
      "updated_at": "2016-11-17T13:25:46.510Z",
      "shortname": "mit-the-great-british-bake-off-0de3ddd5-1f43-4d79-9cd7-006aaa2dc6d0",
      "topic_id": 49,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 183,
      "id": 45,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 50,
      "additional_university_ids": [

      ],
      "discipline_id": 48,
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
      "chapters_updated_at": "2016-11-17T13:25:43.246Z",
      "updated_at": "2016-11-17T13:25:45.959Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 48,
      "language_code": "en",
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
curl "api.goskive.com/v2/files/4/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 0673d3c7bda52d52440fcf4fce20c864a8fb62f525d7f0d9c4c418ad9000cc43"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/11/download
Content-Type: application/json
Authorization: Bearer f7be99a9a720cc48627f2aa298ee076ad5889fd7fa88d9cdab6094ca2cdc8fa3
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7be99a9a720cc48627f2aa298ee076ad5889fd7fa88d9cdab6094ca2cdc8fa3"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/10/report
Content-Type: application/json
Authorization: Bearer 80d5bc5136652b0581e34ef5e415c5c27d2242d971e587cbcd09968e59c2f9a9
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80d5bc5136652b0581e34ef5e415c5c27d2242d971e587cbcd09968e59c2f9a9"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer c601516dd9ab6671d24bf18d8923053306f5475b1eff25b5d36d0f9fa5e698f8
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
	-H "Authorization: Bearer c601516dd9ab6671d24bf18d8923053306f5475b1eff25b5d36d0f9fa5e698f8"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/21/upvote
Content-Type: application/json
Authorization: Bearer 4c2a6041660477b3890bab68330c0f1637df37774fec6b4edd16ba4260a6c6e5
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c2a6041660477b3890bab68330c0f1637df37774fec6b4edd16ba4260a6c6e5"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/84/comments
Content-Type: application/json
Authorization: Bearer b32edb8fbab92dad843864dede4947d4e2f3c5bc9453b735c9ceec0d491b8978
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
    "id": 53,
    "author_id": 785,
    "reply_to_id": null,
    "created_at": "2016-11-17T13:26:36.131Z",
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
curl "api.goskive.com/v2/flashcards/84/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b32edb8fbab92dad843864dede4947d4e2f3c5bc9453b735c9ceec0d491b8978"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/comments
Content-Type: application/json
Authorization: Bearer a9ad7f6d0af33edfb3cd00ee6ab477183651d728320882a5c24cca707e034191
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
    "id": 54,
    "author_id": 788,
    "reply_to_id": null,
    "created_at": "2016-11-17T13:26:36.492Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 45,
      "user_id": 788,
      "feedbackable_id": 85,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:36.489Z",
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
curl "api.goskive.com/v2/flashcards/85/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9ad7f6d0af33edfb3cd00ee6ab477183651d728320882a5c24cca707e034191"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/87/comments
Content-Type: application/json
Authorization: Bearer dbf2e5c007f1790fe463afcd65a537ffba99d16d0e7886bce0def4a675f8105d
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
      "id": 56,
      "author_id": 798,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:36.991Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 797,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:36.974Z",
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
curl "api.goskive.com/v2/flashcards/87/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbf2e5c007f1790fe463afcd65a537ffba99d16d0e7886bce0def4a675f8105d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/86/comments
Content-Type: application/json
Authorization: Bearer d022eeee2a4bf70ec82327eb0cf7b067ff56c9c00c3de57e5155abe29146f587
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
curl "api.goskive.com/v2/flashcards/86/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d022eeee2a4bf70ec82327eb0cf7b067ff56c9c00c3de57e5155abe29146f587"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/22/feedbacks
Content-Type: application/json
Authorization: Bearer e4ed82705629168769e27b7f3841bef514bce301b520e959dc5f5840756ac45f
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
    "id": 37,
    "user_id": 497,
    "feedbackable_id": 22,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T13:26:10.576Z",
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
curl "api.goskive.com/v2/flashcards/22/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4ed82705629168769e27b7f3841bef514bce301b520e959dc5f5840756ac45f"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/29/feedbacks
Content-Type: application/json
Authorization: Bearer 6b6eedb40c937626cd1e3bbaecff66ea45691d9a5659ecb0bfdf1788dc5688f1
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
      "user_id": 532,
      "feedbackable_id": 29,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:12.111Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 531,
      "feedbackable_id": 29,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:12.101Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b6eedb40c937626cd1e3bbaecff66ea45691d9a5659ecb0bfdf1788dc5688f1"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/20/votes
Content-Type: application/json
Authorization: Bearer 1b0a53e646f8857e5dfb3cd2c119a2b3597903718d4eeae9cd71b5341458a41d
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
      "votable_id": 20,
      "user_id": 382
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 20,
      "user_id": 381
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 20,
      "user_id": 380
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/20/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b0a53e646f8857e5dfb3cd2c119a2b3597903718d4eeae9cd71b5341458a41d"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/35/republish
Content-Type: application/json
Authorization: Bearer 8a1f7bfc3874cd38c7de036beffb5be5ad1dbe9cb4c5e86d500d6cdf7eb7d6fc
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
curl "api.goskive.com/v2/flashcards/35/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a1f7bfc3874cd38c7de036beffb5be5ad1dbe9cb4c5e86d500d6cdf7eb7d6fc"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/38/bookmark
Content-Type: application/json
Authorization: Bearer dd98c20b6d030b39b003b5a71127191fad7d7942853d4dd2a2b63b145c119203
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd98c20b6d030b39b003b5a71127191fad7d7942853d4dd2a2b63b145c119203"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/37
Content-Type: application/json
Authorization: Bearer abe70ad0394f6aca01646cf42a3adf0e9034ad8e6870ea0fff511b7a9b52ffe6
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abe70ad0394f6aca01646cf42a3adf0e9034ad8e6870ea0fff511b7a9b52ffe6"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/downvote
Content-Type: application/json
Authorization: Bearer 978fbadc9e09ebcd9315fe62a20deec12a9ce1525f81656b9ef38b926647ef28
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 978fbadc9e09ebcd9315fe62a20deec12a9ce1525f81656b9ef38b926647ef28"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/39
Content-Type: application/json
Authorization: Bearer 3217a7ed6e48e6430be2fed8c604eba7ca6e45733d7bb1241fbd330e53cc4ef2
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 669,
    "chapter_id": 99,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:26:22.720Z",
    "created_at": "2016-11-17T13:26:22.720Z",
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
curl "api.goskive.com/v2/flashcards/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3217a7ed6e48e6430be2fed8c604eba7ca6e45733d7bb1241fbd330e53cc4ef2"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/report
Content-Type: application/json
Authorization: Bearer c4c96233f68af7da1de85a87aa6ca2e729fb0956c1b3489df9acf6210e14bfe8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4c96233f68af7da1de85a87aa6ca2e729fb0956c1b3489df9acf6210e14bfe8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/36/bookmark
Content-Type: application/json
Authorization: Bearer 073c1b4dc2fd9d798b44454df9b7cadf074cb4c4b13dea3790e45064d7d5c4d8
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/36/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 073c1b4dc2fd9d798b44454df9b7cadf074cb4c4b13dea3790e45064d7d5c4d8"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/upvote
Content-Type: application/json
Authorization: Bearer 497e46d197797b9a828a2e7a46fb84839b574b03e42bc75e970e5b7688ef3a4d
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 497e46d197797b9a828a2e7a46fb84839b574b03e42bc75e970e5b7688ef3a4d"
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
    "key": "cache/b36ec24bd816af27de2a6339ef5d144b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xN1QxNDoyNjozOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2IzNmVjMjRiZDgxNmFmMjdkZTJhNjMzOWVmNWQxNDRiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExNy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMTdUMTMyNjM5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161117/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161117T132639Z",
    "x-amz-signature": "55f6139de2e15b91a4153747fbb677fe9eb8c7432d564600fa9b2835e711a8e0"
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
Authorization: Bearer aa9a44795a130ca728d498a517abcc54d12bae3f9e6042bc4f816e7633f49d63
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
	-H "Authorization: Bearer aa9a44795a130ca728d498a517abcc54d12bae3f9e6042bc4f816e7633f49d63"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer e495335d4d123dea3143f451d3c0d1cc8ebc48389fbe86130b51c70db94f59df
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
	-H "Authorization: Bearer e495335d4d123dea3143f451d3c0d1cc8ebc48389fbe86130b51c70db94f59df"
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
{"password":{"reset_password_token":"S9D-eE5eMVvxocertPoF","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 170,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-17T13:25:43.096Z",
  "updated_at": "2016-11-17T13:25:43.229Z",
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
  "audit_id": 4478
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"S9D-eE5eMVvxocertPoF","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/134/comments
Content-Type: application/json
Authorization: Bearer 2b6bdfeb8b33086bc098e63f566d86107b930fc962b0fb55a57275e8588c5a92
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
    "id": 60,
    "author_id": 986,
    "reply_to_id": null,
    "created_at": "2016-11-17T13:26:55.866Z",
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
curl "api.goskive.com/v2/questions/134/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b6bdfeb8b33086bc098e63f566d86107b930fc962b0fb55a57275e8588c5a92"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/133/comments
Content-Type: application/json
Authorization: Bearer fb90a4583b6e68d3f8cec3c5d28872435de41100cb291cbe5cb8bdd6473adb92
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
    "id": 59,
    "author_id": 983,
    "reply_to_id": null,
    "created_at": "2016-11-17T13:26:55.426Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 983,
      "feedbackable_id": 133,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:55.423Z",
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
curl "api.goskive.com/v2/questions/133/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb90a4583b6e68d3f8cec3c5d28872435de41100cb291cbe5cb8bdd6473adb92"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/131/comments
Content-Type: application/json
Authorization: Bearer 22a1ccc3396295b664ef48d279fb5fac032f2d56681c6d031c8337f920a4f4f0
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
      "author_id": 979,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:54.781Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 978,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:54.765Z",
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
curl "api.goskive.com/v2/questions/131/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22a1ccc3396295b664ef48d279fb5fac032f2d56681c6d031c8337f920a4f4f0"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/132/comments
Content-Type: application/json
Authorization: Bearer 46d945d48d7d597b2426461cdea30269cd993ce890203b5d7f9b9c7e88186290
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
curl "api.goskive.com/v2/questions/132/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46d945d48d7d597b2426461cdea30269cd993ce890203b5d7f9b9c7e88186290"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/57/feedbacks
Content-Type: application/json
Authorization: Bearer 85df45a9d5b717c2d5c820dba40892c90717d4140913ec623c05c1554203b33b
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
    "id": 30,
    "user_id": 335,
    "feedbackable_id": 57,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-17T13:26:01.174Z",
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
curl "api.goskive.com/v2/questions/57/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85df45a9d5b717c2d5c820dba40892c90717d4140913ec623c05c1554203b33b"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/61/feedbacks
Content-Type: application/json
Authorization: Bearer 0c64d2e9891ba6a058c6f4d1878bbff2a778923bb5c0e2eeb3aa829ecb3534c2
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
      "id": 34,
      "user_id": 353,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:02.653Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 352,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:02.643Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/61/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c64d2e9891ba6a058c6f4d1878bbff2a778923bb5c0e2eeb3aa829ecb3534c2"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/54/votes
Content-Type: application/json
Authorization: Bearer de3d19ddbde2602db044ec554b51557fa2f6e54a4d61dac634962f5fd0ed4c80
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
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 328
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 327
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 326
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/54/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de3d19ddbde2602db044ec554b51557fa2f6e54a4d61dac634962f5fd0ed4c80"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/108/republish
Content-Type: application/json
Authorization: Bearer 671f7d33f72379ad60e4661d584279a24cc6e6e3ed0c88b875b669261f6679de
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
curl "api.goskive.com/v2/questions/108/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 671f7d33f72379ad60e4661d584279a24cc6e6e3ed0c88b875b669261f6679de"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/110/bookmark
Content-Type: application/json
Authorization: Bearer ee5be42a08f6df3318a84cc68f818f7424b915eff9a29cf40357371281ef35fd
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee5be42a08f6df3318a84cc68f818f7424b915eff9a29cf40357371281ef35fd"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/106
Content-Type: application/json
Authorization: Bearer 11b21798483b11c32719eae1d784290d610762c80633d7646ce672642051ddd3
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/106" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11b21798483b11c32719eae1d784290d610762c80633d7646ce672642051ddd3"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/112/downvote
Content-Type: application/json
Authorization: Bearer 5a878edb52dbe442180c62fe464b96c9b614a2c0653dfbf781ea8073c4500d17
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/112/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a878edb52dbe442180c62fe464b96c9b614a2c0653dfbf781ea8073c4500d17"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/107
Content-Type: application/json
Authorization: Bearer d3cf3e8fbef4c311ff2c337145df82e5280c7c0ea56cc10c717a981accd24a2d
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
    "id": 107,
    "obfuscated_id": "_2rgp7tgq8o",
    "author_id": 877,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:26:44.138Z",
    "created_at": "2016-11-17T13:26:43.968Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 216,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 217,
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
curl "api.goskive.com/v2/questions/107" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3cf3e8fbef4c311ff2c337145df82e5280c7c0ea56cc10c717a981accd24a2d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/129/report
Content-Type: application/json
Authorization: Bearer c9589a9a9dcc33e050e328e88b3645bf0ce7a6f76ae8801cd8dbf624ac06eb55
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/129/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9589a9a9dcc33e050e328e88b3645bf0ce7a6f76ae8801cd8dbf624ac06eb55"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/128/bookmark
Content-Type: application/json
Authorization: Bearer 39a54203024fa4591bf728371b6e207d39b29a0fd13150c71c2b8b48da7b9c0c
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/128/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39a54203024fa4591bf728371b6e207d39b29a0fd13150c71c2b8b48da7b9c0c"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/111
Content-Type: application/json
Authorization: Bearer 9d9481417e7cb83d963e64caf40f64a2470311831b7fe2eeef93d6a049c4ad12
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":111,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-17T13:26:45.614Z","updated_at":"2016-11-17T13:26:45.784Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":169,"author_id":889,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 111,
    "obfuscated_id": "G-D-sgMUtTw",
    "author_id": 889,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T13:26:45.913Z",
    "created_at": "2016-11-17T13:26:45.614Z",
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
    "question": "{\"id\"=>111, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-17T13:26:45.614Z\", \"updated_at\"=>\"2016-11-17T13:26:45.784Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>169, \"author_id\"=>889, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 224,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 225,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 226,
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
curl "api.goskive.com/v2/questions/111" -d '{"question":{"question":{"id":111,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-17T13:26:45.614Z","updated_at":"2016-11-17T13:26:45.784Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":169,"author_id":889,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d9481417e7cb83d963e64caf40f64a2470311831b7fe2eeef93d6a049c4ad12"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/105/upvote
Content-Type: application/json
Authorization: Bearer 5e1769b3fabccc3097fa5fb9a51b244905c900f40ff904f3e921b16bbaad6c1d
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/105/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e1769b3fabccc3097fa5fb9a51b244905c900f40ff904f3e921b16bbaad6c1d"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer d7d4b3744225b5dbd54789310a13fac11795f4d58d0d525dfe2f9fe6bb584413
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
      "creator_id": 649,
      "id": 213,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 199,
      "additional_university_ids": [

      ],
      "discipline_id": 221,
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
      "updated_at": "2016-11-17T13:26:21.102Z",
      "shortname": "mit-pizza-201",
      "topic_id": 220,
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
	-H "Authorization: Bearer d7d4b3744225b5dbd54789310a13fac11795f4d58d0d525dfe2f9fe6bb584413"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 5288488fc15aea49c83c809085083b9ba84950a56234aa071dd713a6c4303269
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
      "id": 197,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-177",
      "html_url": "https://goskive.com/university/uni-177",
      "slug": "uni-177",
      "name": "National School of Pizza",
      "short_name": "Uni 177",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/50972f911c8fb0a0bb1619f6e718267a6cd23b42.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51d8573844e06df03da73ce266c4ec618bc3d315.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T13:26:20.890Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 196,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-176",
      "html_url": "https://goskive.com/university/uni-176",
      "slug": "uni-176",
      "name": "National School of Pastry",
      "short_name": "Uni 176",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/691708776e2a02229b737f1b2a92b7e25e6e7c3c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a9f145362449dba2911e7ea22ea755d720905381.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T13:26:20.872Z",
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
	-H "Authorization: Bearer 5288488fc15aea49c83c809085083b9ba84950a56234aa071dd713a6c4303269"
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
      "id": 38,
      "name": "Robust composite concept",
      "name_translations": {
        "en": "Robust composite concept"
      },
      "discipline_id": 38
    },
    {
      "id": 39,
      "name": "Fully-configurable discrete ability",
      "name_translations": {
        "en": "Fully-configurable discrete ability"
      },
      "discipline_id": 39
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
GET /v2/topics/37
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
    "id": 37,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 37
  }
}
```



```shell
curl "api.goskive.com/v2/topics/37" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer f00a3ae28d34b7a969e89656033c7363875076e766771e36562a839a57c118e7
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
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "University 2",
      "short_name": "Uni 2",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2a89a9c79d6373cf1f5ef1c3a160f560b4b8d6a3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d16dc82a00061731dd68a80b60fdd432c556966d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T13:25:30.784Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-3",
      "html_url": "https://goskive.com/university/uni-3",
      "slug": "uni-3",
      "name": "University 3",
      "short_name": "Uni 3",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0178e4c1b8a1e0379f3158851027049f94ddc463.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51e7a1f572cf9347372a35d5e9ae2cc89f48eb30.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T13:25:30.798Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-4",
      "html_url": "https://goskive.com/university/uni-4",
      "slug": "uni-4",
      "name": "University 4",
      "short_name": "Uni 4",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T13:25:30.830Z",
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
	-H "Authorization: Bearer f00a3ae28d34b7a969e89656033c7363875076e766771e36562a839a57c118e7"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer fc17563662d047538a9975cf4a7e376a51dbc0c4f53c3801f791ec630cc0a2a6
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
    "id": 6,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe1a82f0ac557b999bf5a6b1a0cb87e1a6833cb0.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/dc7090e68b98e4b6195de2af1177270dca8a9cfc.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-17T13:25:31.007Z",
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
	-H "Authorization: Bearer fc17563662d047538a9975cf4a7e376a51dbc0c4f53c3801f791ec630cc0a2a6"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 83095a714d3b5a2d0ee7cd09e2b24aaaa9a955a9828e106dc774f6a36169d845
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":158,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 539,
    "id": 151,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 157,
    "additional_university_ids": [

    ],
    "discipline_id": 159,
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
    "chapters_updated_at": "2016-11-17T13:26:12.759Z",
    "updated_at": "2016-11-17T13:26:12.914Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 86,
        "updated_at": "2016-11-17T13:26:12.866Z",
        "course_id": 151,
        "author_id": 539,
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
        "id": 87,
        "updated_at": "2016-11-17T13:26:12.885Z",
        "course_id": 151,
        "author_id": 539,
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
        "id": 88,
        "updated_at": "2016-11-17T13:26:12.904Z",
        "course_id": 151,
        "author_id": 539,
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
    "topic_id": 158,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":158,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83095a714d3b5a2d0ee7cd09e2b24aaaa9a955a9828e106dc774f6a36169d845"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer db14fecf9deee14983fcaa9c47152cdfc46f1c7e1f61527a63fb983bb36bd2a5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":159,"published":false}}
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
    "creator_id": 540,
    "id": 152,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 158,
    "additional_university_ids": [

    ],
    "discipline_id": 160,
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
    "updated_at": "2016-11-17T13:26:13.112Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 159,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":159,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db14fecf9deee14983fcaa9c47152cdfc46f1c7e1f61527a63fb983bb36bd2a5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 26775df3931ed2a36d3e4965265d238e263a6c4f24be3c39e6d69975fca74c5f
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
      "creator_id": 566,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 183,
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
      "updated_at": "2016-11-17T13:26:15.550Z",
      "shortname": "fu-course-150",
      "topic_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 566,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 184,
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
      "chapters_updated_at": "2016-11-17T13:26:15.409Z",
      "updated_at": "2016-11-17T13:26:15.872Z",
      "shortname": "fu-course-151",
      "topic_id": 183,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26775df3931ed2a36d3e4965265d238e263a6c4f24be3c39e6d69975fca74c5f"
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
      "creator_id": 576,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-158",
      "html_url": "https://goskive.com/course/fu-course-158",
      "slug": "fu-course-158",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "discipline_id": 191,
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
      "updated_at": "2016-11-17T13:26:16.388Z",
      "shortname": "fu-course-158",
      "topic_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 158",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 576,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-159",
      "html_url": "https://goskive.com/course/fu-course-159",
      "slug": "fu-course-159",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "discipline_id": 192,
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
      "chapters_updated_at": "2016-11-17T13:26:16.252Z",
      "updated_at": "2016-11-17T13:26:16.720Z",
      "shortname": "fu-course-159",
      "topic_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 159",
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
Authorization: Bearer 4cb0760256799670bfb3ac41a36735918385b2b43dfd823124156072f726ab43
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
      "creator_id": 572,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-154",
      "html_url": "https://goskive.com/course/fu-course-154",
      "slug": "fu-course-154",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 187,
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
      "updated_at": "2016-11-17T13:26:16.084Z",
      "shortname": "fu-course-154",
      "topic_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 154",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 572,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-155",
      "html_url": "https://goskive.com/course/fu-course-155",
      "slug": "fu-course-155",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "discipline_id": 188,
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
      "updated_at": "2016-11-17T13:26:16.123Z",
      "shortname": "fu-course-155",
      "topic_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cb0760256799670bfb3ac41a36735918385b2b43dfd823124156072f726ab43"
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
      "creator_id": 581,
      "id": 187,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "discipline_id": 195,
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
      "updated_at": "2016-11-17T13:26:16.916Z",
      "shortname": "fu-course-162",
      "topic_id": 194,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 162",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 581,
      "id": 188,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "discipline_id": 196,
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
      "updated_at": "2016-11-17T13:26:16.960Z",
      "shortname": "fu-course-163",
      "topic_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
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
Authorization: Bearer 6bf047ac0dca7c56b487a2e5fc86c59c3380dec7261e8029d927f35d0f151e4f
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
  "id": 319,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-17T13:25:58.799Z",
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
	-H "Authorization: Bearer 6bf047ac0dca7c56b487a2e5fc86c59c3380dec7261e8029d927f35d0f151e4f"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/219
Content-Type: application/json
Authorization: Bearer 0d8499a133fa8cee2ecb8632a6102f6e4459a51eca36b8c5f7a63bc606ded796
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
    "id": 219,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 59,
    "fields_of_study": [
      57,
      58
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-17T13:25:50.898Z",
    "updated_at": "2016-11-17T13:25:50.898Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/219" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d8499a133fa8cee2ecb8632a6102f6e4459a51eca36b8c5f7a63bc606ded796"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/221
Content-Type: application/json
Authorization: Bearer a228b28e5ade12bfc0e872590e9f76cc67f188ed4e391e1b29d4efa25d28ece1
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
    "id": 221,
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
    "created_at": "2016-11-17T13:25:50.983Z",
    "updated_at": "2016-11-17T13:25:50.983Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/221" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a228b28e5ade12bfc0e872590e9f76cc67f188ed4e391e1b29d4efa25d28ece1"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 79b16a10a1c20b4ea5e1397b523442b3af430e6ed200ad882d01787700e0a613
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
	-H "Authorization: Bearer 79b16a10a1c20b4ea5e1397b523442b3af430e6ed200ad882d01787700e0a613"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer 791611dfe4a822b489c227a5f65cc4bacdd13b4493e69e08c0af1133ffe176da
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
    "votable_id": 66,
    "user_id": 394
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 791611dfe4a822b489c227a5f65cc4bacdd13b4493e69e08c0af1133ffe176da"
```
