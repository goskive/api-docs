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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1e5fcee945bf5565ad0e8f45b41ab01e879753b4b4e308b3f720dc4adb66f0f1","client_secret":"c6a41036f0387a9d83f22ef371e6a3ff32c41615fb1bbb17dfb80cbc8e8086ae"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1e5fcee945bf5565ad0e8f45b41ab01e879753b4b4e308b3f720dc4adb66f0f1","client_secret":"c6a41036f0387a9d83f22ef371e6a3ff32c41615fb1bbb17dfb80cbc8e8086ae"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NjgxZTZhYmY3YTk0NDkyZGFhYWFiOTNiMjc5MzczN2ViOGYxM2Q4M2JkZDMw
YzVmMjYwMjFiOTU1YjdiNmFlNzo1MzMwMDYwMTc2MDM0ZDY4OTFhZWI0ZTZl
NTdlMzRkMzU4ZGIwOWZlNTQ2YjZkMWEwMjhhNzYwZTBjY2MxMTZl

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
	-u 681e6abf7a94492daaaab93b2793737eb8f13d83bdd30c5f26021b955b7b6ae7:5330060176034d6891aeb4e6e57e34d358db09fe546b6d1a028a760e0ccc116e
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
{"grant_type":"client_credentials","client_id":"b8e1d881dc3165d2f1c342931c0958386aaccb7f4db7d87499af401236e81ccc","client_secret":"d8246ecbcc01a69e98eb98f2007d19ca0a9f444ba62272c00ebe63ab711655d1"}
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
  "access_token": "0529ecf45b5f5ed3934971c88cf791b46b29b748692fd1643d93c24a8bfc4c32",
  "token_type": "bearer",
  "created_at": 1478690298
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"b8e1d881dc3165d2f1c342931c0958386aaccb7f4db7d87499af401236e81ccc","client_secret":"d8246ecbcc01a69e98eb98f2007d19ca0a9f444ba62272c00ebe63ab711655d1"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"132ba892e2a036ed4e5257b402f2b470de5f6c4141f1940ee153538c64ed7f46","client_secret":"0621d229d09fad02b1f9250a7e15a14e7bd52a1ca81f7a8d61a8b8b4fc9293bc"}
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
  "access_token": "88b1b0a597e9a2099028d5af304a905ab371af52aae227d057b76a731d8fa17c",
  "token_type": "bearer",
  "created_at": 1478690298
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"132ba892e2a036ed4e5257b402f2b470de5f6c4141f1940ee153538c64ed7f46","client_secret":"0621d229d09fad02b1f9250a7e15a14e7bd52a1ca81f7a8d61a8b8b4fc9293bc"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTBiMDA5N2IzZTcyOTljMDMwOGYyNDk3MjU4NzcyZmIxYjZmMGRiMzNlOTYw
YjA0ZGEyMjU0YTU5NDliNTQ1NjpmN2E4OGY5OGMzZjNiY2M4YTA5OWJkMzY3
N2YzOWZiMGI4MzM1Y2IyODBlNzM4ZmNhNGI0NGU3ODhhOGZlZDU1

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
  "access_token": "d39d7b86e8e41f5e27a26adfdd0337bdd2f8f6b762d817b8f2a829523e10312e",
  "token_type": "bearer",
  "created_at": 1478690298
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 90b0097b3e7299c0308f2497258772fb1b6f0db33e960b04da2254a5949b5456:f7a88f98c3f3bcc8a099bd3677f39fb0b8335cb280e738fca4b44e788a8fed55
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
GET /v2/campaigns/4
Content-Type: application/json
Authorization: Bearer da22958cc944ec57a44d6b073f79c8d0bf2a90522b89ebdc22d050dc945f6404
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
    "id": 4,
    "title": "Recruiting pastry chefs",
    "company_id": 27,
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
curl "api.goskive.com/v2/campaigns/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da22958cc944ec57a44d6b073f79c8d0bf2a90522b89ebdc22d050dc945f6404"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/88/flashcards
Content-Type: application/json
Authorization: Bearer 05837bc79c7344b8574cd70ce95b9a96b3b1d43d6efc8d85d31c34d47e0ca261
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":88,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 38,
    "obfuscated_id": "8_YCqPYFnsI",
    "author_id": 426,
    "chapter_id": 88,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:31.974Z",
    "created_at": "2016-11-09T11:18:31.974Z",
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
curl "api.goskive.com/v2/chapters/88/flashcards" -d '{"flashcard":{"chapter_id":88,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05837bc79c7344b8574cd70ce95b9a96b3b1d43d6efc8d85d31c34d47e0ca261"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/90/flashcards
Content-Type: application/json
Authorization: Bearer 9201b01a9af1ac6f04bd4b9d845b2b4efb9543edd822727299fb7836732b560b
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 430,
      "chapter_id": 90,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:32.374Z",
      "created_at": "2016-11-09T11:18:32.374Z",
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 430,
      "chapter_id": 90,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:32.414Z",
      "created_at": "2016-11-09T11:18:32.414Z",
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
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 430,
      "chapter_id": 90,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:32.452Z",
      "created_at": "2016-11-09T11:18:32.452Z",
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
curl "api.goskive.com/v2/chapters/90/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9201b01a9af1ac6f04bd4b9d845b2b4efb9543edd822727299fb7836732b560b"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/97/questions
Content-Type: application/json
Authorization: Bearer 91747ef7e72a254ed5c7a1faccc16b1c529e625768ff576f604de2a6ac9d6ff3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":97,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 57,
    "obfuscated_id": "mCV2FECTNQs",
    "author_id": 470,
    "chapter_id": 97,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:36.645Z",
    "created_at": "2016-11-09T11:18:36.645Z",
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
        "id": 115,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 116,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 117,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 118,
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
curl "api.goskive.com/v2/chapters/97/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":97,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91747ef7e72a254ed5c7a1faccc16b1c529e625768ff576f604de2a6ac9d6ff3"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/96/questions
Content-Type: application/json
Authorization: Bearer ef33a2a39f3417db612fb8f45c2dea37b24b95902711dffed13c43681c2fc467
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":96,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 56,
    "obfuscated_id": "PgrpyPCfpqo",
    "author_id": 467,
    "chapter_id": 96,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:36.075Z",
    "created_at": "2016-11-09T11:18:36.075Z",
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
        "id": 113,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 114,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/96/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":96,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef33a2a39f3417db612fb8f45c2dea37b24b95902711dffed13c43681c2fc467"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/98/questions
Content-Type: application/json
Authorization: Bearer 7c86b73cdf86743729900b034f478da9c3190f931d006a327cadb63ba8c74613
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":98,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 58,
    "obfuscated_id": "_S2mxc1kfck",
    "author_id": 473,
    "chapter_id": 98,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:37.382Z",
    "created_at": "2016-11-09T11:18:37.382Z",
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
        "id": 119,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 120,
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
curl "api.goskive.com/v2/chapters/98/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":98,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c86b73cdf86743729900b034f478da9c3190f931d006a327cadb63ba8c74613"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/95/questions
Content-Type: application/json
Authorization: Bearer f45af5ae7f8652d2cd0d1cc29ea68d5e822c393da938b1c4b0e8808fefb46ddb
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":95,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 55,
    "obfuscated_id": "VX19tR4fHZ8",
    "author_id": 464,
    "chapter_id": 95,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:35.497Z",
    "created_at": "2016-11-09T11:18:35.497Z",
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
        "id": 110,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 111,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 112,
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
curl "api.goskive.com/v2/chapters/95/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":95,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f45af5ae7f8652d2cd0d1cc29ea68d5e822c393da938b1c4b0e8808fefb46ddb"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/100/questions
Content-Type: application/json
Authorization: Bearer 98d5987170c97329b593c26dfc1e0bf7730b9a36d5b32cc0411ab46d3fc33f25
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 479,
      "chapter_id": 100,
      "position": 46,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:38.225Z",
      "created_at": "2016-11-09T11:18:38.096Z",
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
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 480,
      "chapter_id": 100,
      "position": 47,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:38.438Z",
      "created_at": "2016-11-09T11:18:38.304Z",
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 481,
      "chapter_id": 100,
      "position": 48,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T11:18:38.655Z",
      "created_at": "2016-11-09T11:18:38.519Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/100/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98d5987170c97329b593c26dfc1e0bf7730b9a36d5b32cc0411ab46d3fc33f25"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/159
Content-Type: application/json
Authorization: Bearer ebf22571a3315c2e3d799f597b83ec4503b62ce7f2dda07e7cf9102e413d54aa
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
curl "api.goskive.com/v2/chapters/159" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebf22571a3315c2e3d799f597b83ec4503b62ce7f2dda07e7cf9102e413d54aa"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/162
Content-Type: application/json
Authorization: Bearer fb0e6423bab7fe2a62f9c8b053b4dd22e1de1f57d8463cb2cedff343a25dc951
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
curl "api.goskive.com/v2/chapters/162" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb0e6423bab7fe2a62f9c8b053b4dd22e1de1f57d8463cb2cedff343a25dc951"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/166
Content-Type: application/json
Authorization: Bearer ebfe451da8d574b69fb4c898c468070f1c70c44aa08af741fd2d726aa9df9317
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
curl "api.goskive.com/v2/chapters/166" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebfe451da8d574b69fb4c898c468070f1c70c44aa08af741fd2d726aa9df9317"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/161
Content-Type: application/json
Authorization: Bearer aea76e5ec46bdb5da42c8c8f8f2b317dafc946acaf1026f0f2e398f29f976f42
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/161" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aea76e5ec46bdb5da42c8c8f8f2b317dafc946acaf1026f0f2e398f29f976f42"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/163
Content-Type: application/json
Authorization: Bearer 2a7be2eac0bd3b64eb4c0b2466fd56773cb041e7eb85a7451248fd7605f94685
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
    "id": 163,
    "updated_at": "2016-11-09T11:19:08.838Z",
    "course_id": 238,
    "author_id": 736,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-09T11:19:08.246Z",
    "questions_updated_at": "2016-11-09T11:19:08.246Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 740,
        "chapter_id": 163,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:08.818Z",
        "created_at": "2016-11-09T11:19:08.818Z",
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
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 738,
        "chapter_id": 163,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:08.699Z",
        "created_at": "2016-11-09T11:19:08.564Z",
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
            "id": 229,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 230,
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
curl "api.goskive.com/v2/chapters/163" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a7be2eac0bd3b64eb4c0b2466fd56773cb041e7eb85a7451248fd7605f94685"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/167
Content-Type: application/json
Authorization: Bearer bd16d1d3793bb56c14aebc5a9f876846b40aba3bb0b3df92ecceb40d40191f18
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
    "id": 167,
    "updated_at": "2016-11-09T11:19:10.122Z",
    "course_id": 242,
    "author_id": 756,
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
curl "api.goskive.com/v2/chapters/167" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd16d1d3793bb56c14aebc5a9f876846b40aba3bb0b3df92ecceb40d40191f18"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/16/replies
Content-Type: application/json
Authorization: Bearer 42e08ac8ac72189cb05c87db3fe7ae8b45e40577cfda2bdbcbd5c7d07d8592d8
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
    "id": 17,
    "author_id": 338,
    "reply_to_id": 16,
    "created_at": "2016-11-09T11:18:26.302Z",
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
curl "api.goskive.com/v2/comments/16/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42e08ac8ac72189cb05c87db3fe7ae8b45e40577cfda2bdbcbd5c7d07d8592d8"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/18/replies
Content-Type: application/json
Authorization: Bearer 28a064c4f46c8e812f9e728184433f716ca331f8a4d6ff41bc09ecee661c925b
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
curl "api.goskive.com/v2/comments/18/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28a064c4f46c8e812f9e728184433f716ca331f8a4d6ff41bc09ecee661c925b"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/24
Content-Type: application/json
Authorization: Bearer 41f11ca03433dd382ae43b55a06999271cb21b37770c242584f364c67ea995b7
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
curl "api.goskive.com/v2/comments/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41f11ca03433dd382ae43b55a06999271cb21b37770c242584f364c67ea995b7"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/21/republish
Content-Type: application/json
Authorization: Bearer 26ff4eccc8fa4a5ae4d7a59ddcdb92b5cd349c26cc894b3aaf4ff585b47dea4b
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
curl "api.goskive.com/v2/comments/21/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26ff4eccc8fa4a5ae4d7a59ddcdb92b5cd349c26cc894b3aaf4ff585b47dea4b"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/23
Content-Type: application/json
Authorization: Bearer 4f89eff58107e99f4b6378e8a0dc2ec0b628227ae78ebc43f39e543abb77405d
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f89eff58107e99f4b6378e8a0dc2ec0b628227ae78ebc43f39e543abb77405d"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/22/report
Content-Type: application/json
Authorization: Bearer 1f64cdeaf4a592a3c2666f25ad89327f3f84616b113eb49cc4873091a3a32305
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f64cdeaf4a592a3c2666f25ad89327f3f84616b113eb49cc4873091a3a32305"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/23
Content-Type: application/json
Authorization: Bearer a3951e8e5d68643d016419706e64a3f869e8f77f78f7ff6e1dcf59c399df7f93
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
    "id": 23,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-09T11:18:33.070Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3951e8e5d68643d016419706e64a3f869e8f77f78f7ff6e1dcf59c399df7f93"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f4253470f505e4070e48cae36247be90b0fdf4c544f089b4b26ca02c3087fbe2
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
      "id": 20,
      "name": "Fake Company Name 20",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T11:18:32.918Z"
    },
    {
      "id": 21,
      "name": "Fake Company Name 21",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T11:18:32.922Z"
    },
    {
      "id": 22,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T11:18:32.927Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4253470f505e4070e48cae36247be90b0fdf4c544f089b4b26ca02c3087fbe2"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 79057c1d535903dfb438577a1462f1f0a7ec1dab56a0ac97a2bcf2086a752a8d
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

      ]
    },
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
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79057c1d535903dfb438577a1462f1f0a7ec1dab56a0ac97a2bcf2086a752a8d"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/24/company_profiles
Content-Type: application/json
Authorization: Bearer e3b29b89970c986a04c7e4e362cb16ee0b4ec992c2df4d7cd046ed8a1bc1c519
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
      "id": 4,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/b7227ba08020eaf424f385a68712e11390fe76a3.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/15a47e0f0d046fb9c95772f170325321f8fb4d6d.png",
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
curl "api.goskive.com/v2/companies/24/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3b29b89970c986a04c7e4e362cb16ee0b4ec992c2df4d7cd046ed8a1bc1c519"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 7f18fa176c0b383ae0fdca6872cd995a5eceac786390eb32bdc47300cf100cb4
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
      "title": "Campaign 4",
      "company_id": 28,
      "precluded_campaign_ids": [

      ],
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
    },
    {
      "id": 8,
      "title": "Campaign 7",
      "company_id": 31,
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f18fa176c0b383ae0fdca6872cd995a5eceac786390eb32bdc47300cf100cb4"
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
Authorization: Bearer 5d600a59438fd0a1623e86182cde1be57ff9d9468e84157ec1a0fb5e62c9daef
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
	-H "Authorization: Bearer 5d600a59438fd0a1623e86182cde1be57ff9d9468e84157ec1a0fb5e62c9daef"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6688a5bde0fd6c87fa1e27714a21e46a7e61be2c43938237b159cc5d22a5fb6a
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
    "id": 135,
    "updated_at": "2016-11-09T11:18:48.601Z",
    "course_id": 197,
    "author_id": 596,
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
	-H "Authorization: Bearer 6688a5bde0fd6c87fa1e27714a21e46a7e61be2c43938237b159cc5d22a5fb6a"
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
      "id": 121,
      "updated_at": "2016-11-09T11:18:46.566Z",
      "course_id": 188,
      "author_id": 565,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 109",
      "position": 1
    },
    {
      "id": 122,
      "updated_at": "2016-11-09T11:18:46.594Z",
      "course_id": 188,
      "author_id": 566,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 110",
      "position": 2
    },
    {
      "id": 123,
      "updated_at": "2016-11-09T11:18:46.862Z",
      "course_id": 188,
      "author_id": 567,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-09T11:18:46.479Z",
      "questions_updated_at": "2016-11-09T11:18:46.479Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 111",
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
Authorization: Bearer a2ab90a176b575818b770aa378458c47df0f310ba7b497f54bd4d022ce0f3155
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
      "id": 127,
      "updated_at": "2016-11-09T11:18:47.251Z",
      "course_id": 191,
      "author_id": 576,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 115",
      "position": 1
    },
    {
      "id": 128,
      "updated_at": "2016-11-09T11:18:47.276Z",
      "course_id": 191,
      "author_id": 577,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 116",
      "position": 2
    },
    {
      "id": 129,
      "updated_at": "2016-11-09T11:18:47.555Z",
      "course_id": 191,
      "author_id": 578,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-09T11:18:47.173Z",
      "questions_updated_at": "2016-11-09T11:18:47.173Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 117",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2ab90a176b575818b770aa378458c47df0f310ba7b497f54bd4d022ce0f3155"
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
      "id": 124,
      "updated_at": "2016-11-09T11:18:47.075Z",
      "course_id": 190,
      "author_id": 572,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 112",
      "position": 1
    },
    {
      "id": 125,
      "updated_at": "2016-11-09T11:18:47.100Z",
      "course_id": 190,
      "author_id": 573,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 113",
      "position": 2
    },
    {
      "id": 126,
      "updated_at": "2016-11-09T11:18:47.125Z",
      "course_id": 190,
      "author_id": 574,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 114",
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
Authorization: Bearer 290974e0cc49ac0b7f5f241caf51ff63f2e6d6893594f80a697a2673965a93e9
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
      "updated_at": "2016-11-09T11:18:47.745Z",
      "course_id": 192,
      "author_id": 583,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 118",
      "position": 1
    },
    {
      "id": 131,
      "updated_at": "2016-11-09T11:18:47.773Z",
      "course_id": 192,
      "author_id": 584,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 119",
      "position": 2
    },
    {
      "id": 132,
      "updated_at": "2016-11-09T11:18:47.801Z",
      "course_id": 192,
      "author_id": 585,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 120",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 290974e0cc49ac0b7f5f241caf51ff63f2e6d6893594f80a697a2673965a93e9"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 21933b5edb6768995604818a2d58398539db87a795490155d6364ea164063323
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
    "course_id": 76,
    "user_id": 260,
    "updated_at": "2016-11-09T11:18:20.518Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21933b5edb6768995604818a2d58398539db87a795490155d6364ea164063323"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 9e7bf02c00db27cfd6259d554230c9ffeb969ade980b665dde0825beed3301ac
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
      "course_id": 74,
      "user_id": 254,
      "updated_at": "2016-11-09T11:18:20.180Z"
    },
    {
      "id": 5,
      "course_id": 74,
      "user_id": 255,
      "updated_at": "2016-11-09T11:18:20.195Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e7bf02c00db27cfd6259d554230c9ffeb969ade980b665dde0825beed3301ac"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/243/files
Content-Type: application/json
Authorization: Bearer e87fa17612499c291ed86587b7b8a2f4ce977fc7fcc86e853db46036b2cf85ed
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
        "id": 758,
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
        "created_at": "2016-11-09T11:19:10.289Z",
        "updated_at": "2016-11-09T11:19:10.289Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T11:19:10.301Z",
      "updated_at": "2016-11-09T11:19:10.301Z",
      "course_id": 243,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 20,
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
        "created_at": "2016-11-09T11:19:10.310Z",
        "updated_at": "2016-11-09T11:19:10.310Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T11:19:10.320Z",
      "updated_at": "2016-11-09T11:19:10.320Z",
      "course_id": 243,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 760,
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
        "created_at": "2016-11-09T11:19:10.329Z",
        "updated_at": "2016-11-09T11:19:10.329Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T11:19:10.340Z",
      "updated_at": "2016-11-09T11:19:10.340Z",
      "course_id": 243,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/243/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e87fa17612499c291ed86587b7b8a2f4ce977fc7fcc86e853db46036b2cf85ed"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/246/files
Content-Type: application/json
Authorization: Bearer b4b86cc147c4b2e824583926003070f4baf2ae1ca7f6798767d14f7068a9b74e
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
      "id": 767,
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
      "created_at": "2016-11-09T11:19:10.708Z",
      "updated_at": "2016-11-09T11:19:10.708Z"
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
    "created_at": "2016-11-09T11:19:10.743Z",
    "updated_at": "2016-11-09T11:19:10.743Z",
    "course_id": 246,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/246/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4b86cc147c4b2e824583926003070f4baf2ae1ca7f6798767d14f7068a9b74e"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/245/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 04dc61f008dc859828731c893b20fc7a76cf68ca4c4bdff1554ff3c6b1e6b020
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
    "key": "cache/165783002c43b7db99cc329bac906f1e.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOVQxMjoxOToxMFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzE2NTc4MzAwMmM0M2I3ZGI5OWNjMzI5YmFjOTA2ZjFlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDkvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA5VDExMTkxMFoifV19",
    "x-amz-credential": "FAKE/20161109/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161109T111910Z",
    "x-amz-signature": "e064bb9d238508326152fa955a68f46371270c20250cd1d8d608fc4ea3743641"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/245/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04dc61f008dc859828731c893b20fc7a76cf68ca4c4bdff1554ff3c6b1e6b020"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer e4368690765e2241199e551a6b32b787910669db0c85b8f679ca993624aaeaff
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
	-H "Authorization: Bearer e4368690765e2241199e551a6b32b787910669db0c85b8f679ca993624aaeaff"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 03701855f396edac24a3b01ee89b7a992d30972ae5278a5599b0763b95aeb864
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
	-H "Authorization: Bearer 03701855f396edac24a3b01ee89b7a992d30972ae5278a5599b0763b95aeb864"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c7c20e0242988247515ee10abf5ee42f24d50abf80fe82cec8fe596f6ae10247
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
	-H "Authorization: Bearer c7c20e0242988247515ee10abf5ee42f24d50abf80fe82cec8fe596f6ae10247"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 576cbab9675fdb8c9cdb530b3de6c3e78eb446d917d31f6615d04c43117baa32
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
	-H "Authorization: Bearer 576cbab9675fdb8c9cdb530b3de6c3e78eb446d917d31f6615d04c43117baa32"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ae249f103980994f7dd61d620ed1bdb63598bf8357c422752eb5b40838828c82
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
	-H "Authorization: Bearer ae249f103980994f7dd61d620ed1bdb63598bf8357c422752eb5b40838828c82"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 46bdb03952450d51f07f31e4d33f7c0d5af15e9e7bc56d27d89335a1a505b420
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
    "creator_id": 674,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 206,
    "additional_university_ids": [

    ],
    "discipline_id": 229,
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
    "chapters_updated_at": "2016-11-09T11:18:57.517Z",
    "updated_at": "2016-11-09T11:18:59.142Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 675,
        "chapter_id": 147,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:58.899Z",
        "created_at": "2016-11-09T11:18:58.899Z",
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
        "author_id": 675,
        "chapter_id": 148,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:58.983Z",
        "created_at": "2016-11-09T11:18:58.983Z",
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
        "author_id": 675,
        "chapter_id": 147,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:58.945Z",
        "created_at": "2016-11-09T11:18:58.945Z",
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
        "author_id": 675,
        "chapter_id": 148,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:59.030Z",
        "created_at": "2016-11-09T11:18:59.030Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 675,
        "chapter_id": 147,
        "position": 71,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:57.747Z",
        "created_at": "2016-11-09T11:18:57.623Z",
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
            "id": 171,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 172,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 675,
        "chapter_id": 147,
        "position": 72,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:57.941Z",
        "created_at": "2016-11-09T11:18:57.817Z",
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
        "author_id": 675,
        "chapter_id": 148,
        "position": 73,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:58.167Z",
        "created_at": "2016-11-09T11:18:58.031Z",
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
        "author_id": 675,
        "chapter_id": 148,
        "position": 74,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:18:58.375Z",
        "created_at": "2016-11-09T11:18:58.242Z",
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
    ],
    "chapters": [
      {
        "id": 147,
        "updated_at": "2016-11-09T11:18:59.088Z",
        "course_id": 221,
        "author_id": 674,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T11:18:57.517Z",
        "questions_updated_at": "2016-11-09T11:18:57.517Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 132",
        "position": 1
      },
      {
        "id": 148,
        "updated_at": "2016-11-09T11:18:59.133Z",
        "course_id": 221,
        "author_id": 674,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T11:18:57.517Z",
        "questions_updated_at": "2016-11-09T11:18:57.517Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 133",
        "position": 2
      }
    ],
    "topic_id": 228,
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
	-H "Authorization: Bearer 46bdb03952450d51f07f31e4d33f7c0d5af15e9e7bc56d27d89335a1a505b420"
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
    "creator_id": 686,
    "id": 223,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 208,
    "additional_university_ids": [

    ],
    "discipline_id": 231,
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
    "chapters_updated_at": "2016-11-09T11:19:01.023Z",
    "updated_at": "2016-11-09T11:19:02.672Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 686,
        "chapter_id": 151,
        "position": 83,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:01.253Z",
        "created_at": "2016-11-09T11:19:01.124Z",
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
        "id": 98,
        "obfuscated_id": "icApzX10lRE",
        "author_id": 686,
        "chapter_id": 152,
        "position": 85,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T11:19:01.683Z",
        "created_at": "2016-11-09T11:19:01.547Z",
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
      }
    ],
    "chapters": [
      {
        "id": 151,
        "updated_at": "2016-11-09T11:19:02.620Z",
        "course_id": 223,
        "author_id": 686,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T11:19:01.023Z",
        "questions_updated_at": "2016-11-09T11:19:01.023Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 136",
        "position": 1
      },
      {
        "id": 152,
        "updated_at": "2016-11-09T11:19:02.664Z",
        "course_id": 223,
        "author_id": 686,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T11:19:01.023Z",
        "questions_updated_at": "2016-11-09T11:19:01.023Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 137",
        "position": 2
      }
    ],
    "topic_id": 230,
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
PUT /v2/courses/220/pin
Content-Type: application/json
Authorization: Bearer 217a8ea7701e29e2c79548c321adbb436c37b6d75b1e1aba017c1ca273acca37
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/220/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 217a8ea7701e29e2c79548c321adbb436c37b6d75b1e1aba017c1ca273acca37"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/219/pin
Content-Type: application/json
Authorization: Bearer 0a655052b0cbd04365e13ead498de8d7171b1c05ba6421addb0e8674f966371b
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/219/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a655052b0cbd04365e13ead498de8d7171b1c05ba6421addb0e8674f966371b"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2293d8999ca5ebf88399a176d8d2fa5095b3ffe0b1ec6452517a8dc03e55d093
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
    "creator_id": 663,
    "id": 215,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 200,
    "additional_university_ids": [

    ],
    "discipline_id": 223,
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
    "updated_at": "2016-11-09T11:18:56.714Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 222,
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
	-H "Authorization: Bearer 2293d8999ca5ebf88399a176d8d2fa5095b3ffe0b1ec6452517a8dc03e55d093"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 72ddb9a105c97979bdd5f2650baa3131dbb7c7298b17206793bfd12f564827f8
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
    "id": 717,
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
    "created_at": "2016-11-09T11:19:06.316Z",
    "updated_at": "2016-11-09T11:19:06.316Z",
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
	-H "Authorization: Bearer 72ddb9a105c97979bdd5f2650baa3131dbb7c7298b17206793bfd12f564827f8"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2108f2ef8137fc95746b3a3214864a0111472b3dc91011f48dfa09f750fd782e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[241]}
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
    "id": 718,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      241
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T11:19:06.421Z",
    "updated_at": "2016-11-09T11:19:06.459Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[241]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2108f2ef8137fc95746b3a3214864a0111472b3dc91011f48dfa09f750fd782e"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 48fb3969683ab985ea5a49e678b927912231e7ce67f47e44f553615413d5959c
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
    "id": 720,
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
    "created_at": "2016-11-09T11:19:06.564Z",
    "updated_at": "2016-11-09T11:19:06.564Z",
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
	-H "Authorization: Bearer 48fb3969683ab985ea5a49e678b927912231e7ce67f47e44f553615413d5959c"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0d27bd1a3043a44b6c5048d6076ff91fca5a9ce54b28839770f6adf230fde953
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[242]}
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
    "id": 719,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      242
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T11:19:06.508Z",
    "updated_at": "2016-11-09T11:19:06.508Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[242]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d27bd1a3043a44b6c5048d6076ff91fca5a9ce54b28839770f6adf230fde953"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 1b512e36a0c9c7f17c6bf7cd294a55e0813c8368a9512fec399ec19c65021c08
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

245
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
    "id": 722,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/f686b91463b8c22aa57cd5aec647a53e8941d81d.jpg",
    "university_id": null,
    "fields_of_study": [
      245
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T11:19:06.759Z",
    "updated_at": "2016-11-09T11:19:07.014Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/742fcbb2f2e26c494dc4136f93b96c87c5236e6e.jpg",
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

245
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 1b512e36a0c9c7f17c6bf7cd294a55e0813c8368a9512fec399ec19c65021c08"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer d03317312ec607588f7b778b21e3fd69c7cd51022143986d323c5acdf017bc80
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
      "bookmarkable_id": 38,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 39,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 40,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d03317312ec607588f7b778b21e3fd69c7cd51022143986d323c5acdf017bc80"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 34a6a3a546cd7164476cfaa5a8cbed75ebbd83bb5a3899e5f5f8b4595944b374
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
      "company_id": 16,
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
      "company_id": 17,
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
	-H "Authorization: Bearer 34a6a3a546cd7164476cfaa5a8cbed75ebbd83bb5a3899e5f5f8b4595944b374"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 17a7115165c1a487233016afd00d6f7f0c16130d334a6dc0c7c2bfa8242ea3dc
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
      "company_id": 12,
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
	-H "Authorization: Bearer 17a7115165c1a487233016afd00d6f7f0c16130d334a6dc0c7c2bfa8242ea3dc"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer f1fc3241c8a583a4c16c26f1f9b901b6702535e5f9ed67315e55177ca63740ed
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
      "creator_id": 128,
      "id": 36,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-36",
      "html_url": "https://goskive.com/course/mit-course-36",
      "slug": "mit-course-36",
      "university_id": 41,
      "additional_university_ids": [

      ],
      "discipline_id": 36,
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
      "updated_at": "2016-11-09T11:18:08.791Z",
      "shortname": "mit-course-36",
      "topic_id": 36,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 36",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 129,
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-37",
      "html_url": "https://goskive.com/course/mit-course-37",
      "slug": "mit-course-37",
      "university_id": 42,
      "additional_university_ids": [

      ],
      "discipline_id": 37,
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
      "updated_at": "2016-11-09T11:18:08.887Z",
      "shortname": "mit-course-37",
      "topic_id": 37,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 37",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1fc3241c8a583a4c16c26f1f9b901b6702535e5f9ed67315e55177ca63740ed"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 092da3664313ec23201a6a529db0a37fabdae702b3892ac6331184899aeeebc1
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
        "created_at": "2016-11-09T11:18:32.686Z",
        "updated_at": "2016-11-09T11:18:32.686Z",
        "file_url": "memory://8ce327f6a606d44c73e065abbe0f4330.pdf",
        "course_id": 122,
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
        "created_at": "2016-11-09T11:18:32.767Z",
        "updated_at": "2016-11-09T11:18:32.767Z",
        "file_url": "memory://5fd832da1df5565ab2da3f5b5f05d8a2.pdf",
        "course_id": 123,
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
        "created_at": "2016-11-09T11:18:32.852Z",
        "updated_at": "2016-11-09T11:18:32.852Z",
        "file_url": "memory://5200caa30c5acba8a55e1b87704568d0.pdf",
        "course_id": 124,
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
	-H "Authorization: Bearer 092da3664313ec23201a6a529db0a37fabdae702b3892ac6331184899aeeebc1"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer c77650a41bb6b49d40c4381d8a84960ddf296b31bea84eb73a2293ebf091755d
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
      "company_id": 9,
      "company": {
        "id": 9,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T11:18:05.131Z"
      },
      "created_at": "2016-11-09T11:18:05.134Z",
      "updated_at": "2016-11-09T11:18:05.134Z",
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T11:18:05.143Z"
      },
      "created_at": "2016-11-09T11:18:05.146Z",
      "updated_at": "2016-11-09T11:18:05.146Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c77650a41bb6b49d40c4381d8a84960ddf296b31bea84eb73a2293ebf091755d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8672db0f5b0fca360b5b73ec4fac2e4cbb99c0944294ed402bcdbc7c2f144bc5
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
      "company_id": 5,
      "company": {
        "id": 5,
        "name": "Fake Company Name 5",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T11:18:04.897Z"
      },
      "created_at": "2016-11-09T11:18:04.901Z",
      "updated_at": "2016-11-09T11:18:04.901Z",
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T11:18:04.915Z"
      },
      "created_at": "2016-11-09T11:18:04.918Z",
      "updated_at": "2016-11-09T11:18:04.918Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8672db0f5b0fca360b5b73ec4fac2e4cbb99c0944294ed402bcdbc7c2f144bc5"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer cbdd85cdb258e61c0ab425b4d4ac337afc5697bfc2bd62fe9a9f71ed804b45b2
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
      "id": 5,
      "created_at": "2016-11-09T11:18:06.323Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-11-09T11:18:06.440Z",
      "author_id": "100",
      "thread_subject_id": "28",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 6,
      "created_at": "2016-11-09T11:18:06.429Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-11-09T11:18:06.443Z",
      "author_id": "103",
      "thread_subject_id": "29",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-11-09T11:18:06.835Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-11-09T11:18:06.835Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-11-09T11:18:07.227Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-11-09T11:18:07.227Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 9,
      "created_at": "2016-11-09T11:18:07.624Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-11-09T11:18:07.624Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 10,
      "created_at": "2016-11-09T11:18:07.937Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 30,
      "updated_at": "2016-11-09T11:18:07.937Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-11-09T11:18:08.267Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 31,
      "updated_at": "2016-11-09T11:18:08.267Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-11-09T11:18:08.594Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 32,
      "updated_at": "2016-11-09T11:18:08.594Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbdd85cdb258e61c0ab425b4d4ac337afc5697bfc2bd62fe9a9f71ed804b45b2"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/4
Content-Type: application/json
Authorization: Bearer 0b34fa65e77db9967eba92139ab370b781ca25abfcecb4da0a3edb47887c1a72
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-09T11:08:05.000Z"}}
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
    "id": 4,
    "created_at": "2016-11-09T11:18:06.100Z",
    "read_at": "2016-11-09T11:08:05.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-11-09T11:18:06.162Z",
    "author_id": "96",
    "thread_subject_id": "27",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/4" -d '{"notification":{"read_at":"2016-11-09T11:08:05.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b34fa65e77db9967eba92139ab370b781ca25abfcecb4da0a3edb47887c1a72"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 60cbcfc25fcf6abda28623f730a343a8b4294c64ab8edc050fc51aef78839057
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
      "course_id": 60,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-09T11:18:15.535Z",
      "course_published": true,
      "updated_at": "2016-11-09T11:18:15.528Z"
    },
    {
      "id": 7,
      "course_id": 61,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-09T11:18:15.617Z",
      "course_published": true,
      "updated_at": "2016-11-09T11:18:15.610Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60cbcfc25fcf6abda28623f730a343a8b4294c64ab8edc050fc51aef78839057"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 7eacd50a4bf47d1fc741c41279ef711154f79900f9103500d75b858644da5d86
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
    "course_id": 57,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-09T11:18:15.174Z",
    "course_published": true,
    "updated_at": "2016-11-09T11:18:15.167Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7eacd50a4bf47d1fc741c41279ef711154f79900f9103500d75b858644da5d86"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer da9ae5fe62fa94ad3aa2c1057b925b2178bdee832fb85d7ddb25626910d5de5e
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
    "course_id": 56,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-09T11:18:15.068Z",
    "course_published": true,
    "updated_at": "2016-11-09T11:18:15.057Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da9ae5fe62fa94ad3aa2c1057b925b2178bdee832fb85d7ddb25626910d5de5e"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 29df84910b8b57efa1c452c2264ee71299e5c8c8a48db8072070e02cc0a16841
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
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 51,
      "user_id": 444
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 52,
      "user_id": 444
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 53,
      "user_id": 444
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 444
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29df84910b8b57efa1c452c2264ee71299e5c8c8a48db8072070e02cc0a16841"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/76
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
    "id": 76,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 76,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 76
      },
      {
        "id": 77,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 76
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/76" -X GET \
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
      "id": 77,
      "name": "Cloned bottom-line alliance",
      "name_translations": {
        "en": "Cloned bottom-line alliance"
      }
    },
    {
      "id": 78,
      "name": "Public-key zero tolerance function",
      "name_translations": {
        "en": "Public-key zero tolerance function"
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
PATCH /v2/feedbacks/39/close
Content-Type: application/json
Authorization: Bearer 56692613a157e19ef72babece99c5ca52e5d87c31ce771d90015660032e13c31
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
    "id": 39,
    "user_id": 857,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-09T11:19:17.800Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/39/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56692613a157e19ef72babece99c5ca52e5d87c31ce771d90015660032e13c31"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/45/fix
Content-Type: application/json
Authorization: Bearer b7f4e97d86a06a364bc9e8f999a1335aec8cd4703a56a09b8daccdc96a654e3c
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
    "id": 45,
    "user_id": 889,
    "feedbackable_id": 94,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-09T11:19:19.479Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/45/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7f4e97d86a06a364bc9e8f999a1335aec8cd4703a56a09b8daccdc96a654e3c"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/41
Content-Type: application/json
Authorization: Bearer a875e82f4c4eacf6053e1215d0925bdcb1f75985d56c7e3b83f0e78904e2f5da
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
    "id": 41,
    "user_id": 867,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T11:19:18.487Z",
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
curl "api.goskive.com/v2/feedbacks/41" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a875e82f4c4eacf6053e1215d0925bdcb1f75985d56c7e3b83f0e78904e2f5da"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/38/close
Content-Type: application/json
Authorization: Bearer 7cf8ed4427322016004c0efb3b35abe75ac956181766f9e8476aba5187b452a8
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
curl "api.goskive.com/v2/feedbacks/38/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cf8ed4427322016004c0efb3b35abe75ac956181766f9e8476aba5187b452a8"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 925031e79ca97f4169a9887ec8af0f56918a2ac5a1c1db51d1dc5c0e29b238ee
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
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 925031e79ca97f4169a9887ec8af0f56918a2ac5a1c1db51d1dc5c0e29b238ee"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/fix
Content-Type: application/json
Authorization: Bearer 3d4eba337a157b7b319cbd6a4473a1a31d739675672d88c67b51d14b65c62682
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
curl "api.goskive.com/v2/feedbacks/44/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d4eba337a157b7b319cbd6a4473a1a31d739675672d88c67b51d14b65c62682"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/42
Content-Type: application/json
Authorization: Bearer a42c8737b598b722755d8b4907f7a577f7097f4b4686a2672da2b1ed982eaea9
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
    "id": 42,
    "user_id": 872,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T11:19:18.789Z",
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
curl "api.goskive.com/v2/feedbacks/42" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a42c8737b598b722755d8b4907f7a577f7097f4b4686a2672da2b1ed982eaea9"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 67e18b82b1b4f593e3d95d272e78335596d73f6eb3d8827aa08e4d3798c47610
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67e18b82b1b4f593e3d95d272e78335596d73f6eb3d8827aa08e4d3798c47610"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/5/bookmark
Content-Type: application/json
Authorization: Bearer bcc236d63c144660cd1640e8dd2af8b5176c1044bf5690ca249ba15ac2655fd6
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcc236d63c144660cd1640e8dd2af8b5176c1044bf5690ca249ba15ac2655fd6"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer c943bdd5d6820f8bc406d8b68211082daaf8e5e672059c50bd4c134d41cb1ede
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
	-H "Authorization: Bearer c943bdd5d6820f8bc406d8b68211082daaf8e5e672059c50bd4c134d41cb1ede"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/13
Content-Type: application/json
Authorization: Bearer bd842fc3f3451833a83f98b933c85f1f6594df2dd89b148f260b5ae66d13e4c9
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/bc629d45be4fb4a55ca0e7f297825d26.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161109%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161109T111811Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=0fec6caf5166529ccc9f52b1a98ef1044887922a81cdfab3197aba196abde44e",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd842fc3f3451833a83f98b933c85f1f6594df2dd89b148f260b5ae66d13e4c9"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer e5033774db4fe5c70f00b8bd38eaa60da3b1ca353f8b0bb42cb5e3d332f69d3a
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/c0ff6532aa253eda4b47de34fa96e15f.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161109%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161109T111810Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=13e90f8e7ba0c28e5673626d922e307705aaa90a863cfe9337348c3e79a0238b",
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
	-H "Authorization: Bearer e5033774db4fe5c70f00b8bd38eaa60da3b1ca353f8b0bb42cb5e3d332f69d3a"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/1/metadata
Content-Type: application/json
Authorization: Bearer ee42fb507afc70b762e5538251e66f876305968eb059a75b8864aa32146c7bc8
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
    "id": 1,
    "uploader": {
      "id": 131,
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
      "created_at": "2016-11-09T11:18:09.033Z",
      "updated_at": "2016-11-09T11:18:09.033Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-09T11:18:09.214Z",
    "updated_at": "2016-11-09T11:18:09.214Z",
    "course_id": 38,
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
curl "api.goskive.com/v2/files/1/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee42fb507afc70b762e5538251e66f876305968eb059a75b8864aa32146c7bc8"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/17/matched_courses?required_cu_count=2
Authorization: Bearer 6c03992f35f62757f8f3417f09b6b83019fbb70ae6d3859007e7c60c8cf410ca
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
      "creator_id": 613,
      "id": 202,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-31c2d690-3d75-49de-b637-401b73753490",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-31c2d690-3d75-49de-b637-401b73753490",
      "slug": "mit-the-great-british-bake-off-31c2d690-3d75-49de-b637-401b73753490",
      "university_id": 187,
      "additional_university_ids": [

      ],
      "discipline_id": 210,
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
      "chapters_updated_at": "2016-11-09T11:18:48.800Z",
      "updated_at": "2016-11-09T11:18:51.742Z",
      "shortname": "mit-the-great-british-bake-off-31c2d690-3d75-49de-b637-401b73753490",
      "topic_id": 209,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 608,
      "id": 201,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "discipline_id": 209,
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
      "chapters_updated_at": "2016-11-09T11:18:48.800Z",
      "updated_at": "2016-11-09T11:18:51.089Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 208,
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
curl "api.goskive.com/v2/files/17/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 6c03992f35f62757f8f3417f09b6b83019fbb70ae6d3859007e7c60c8cf410ca"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/12/download
Content-Type: application/json
Authorization: Bearer fee2eb79c7cd394d6e7681e51ba5046cdb8ee0870b8155d35c18c4e140b55ffc
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fee2eb79c7cd394d6e7681e51ba5046cdb8ee0870b8155d35c18c4e140b55ffc"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 8c58ed8cdcb90e518242507fc9dfb055d1ef3a6b924a3032c1bc708352436936
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c58ed8cdcb90e518242507fc9dfb055d1ef3a6b924a3032c1bc708352436936"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/4/bookmark
Content-Type: application/json
Authorization: Bearer 9a2f9a7335a3616c5c7ac5af304289b02d384206bfc5cd04e71512ae92c07b26
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a2f9a7335a3616c5c7ac5af304289b02d384206bfc5cd04e71512ae92c07b26"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/6/upvote
Content-Type: application/json
Authorization: Bearer a172870153afc3cb4576b6a0cc385eaef6c18e5ce97b18e50a154367472965a1
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a172870153afc3cb4576b6a0cc385eaef6c18e5ce97b18e50a154367472965a1"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/2/comments
Content-Type: application/json
Authorization: Bearer af564e1be446d4ea2c683b46d8c717d78ddcb77092c356a2922f43e904b525f8
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
    "id": 5,
    "author_id": 171,
    "reply_to_id": null,
    "created_at": "2016-11-09T11:18:12.037Z",
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
curl "api.goskive.com/v2/flashcards/2/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af564e1be446d4ea2c683b46d8c717d78ddcb77092c356a2922f43e904b525f8"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/comments
Content-Type: application/json
Authorization: Bearer 2d4824085ff6ea2b11fe8b834ec2af69a4b48a42bc943aa3f360173a536aa165
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
    "id": 4,
    "author_id": 168,
    "reply_to_id": null,
    "created_at": "2016-11-09T11:18:11.699Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 168,
      "feedbackable_id": 1,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:11.694Z",
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
curl "api.goskive.com/v2/flashcards/1/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d4824085ff6ea2b11fe8b834ec2af69a4b48a42bc943aa3f360173a536aa165"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/4/comments
Content-Type: application/json
Authorization: Bearer 47978ad59dfd45b028cf54856beb7f25e47a591925b4cfccc55de6ac7a7bb4f9
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
      "id": 6,
      "author_id": 180,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:18:12.540Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 181,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:18:12.588Z",
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
curl "api.goskive.com/v2/flashcards/4/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47978ad59dfd45b028cf54856beb7f25e47a591925b4cfccc55de6ac7a7bb4f9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/3/comments
Content-Type: application/json
Authorization: Bearer 3a86d4a9b479288bd36ec80732917d08c5bfbb39e0bbd35253f44bb8faba6b25
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
curl "api.goskive.com/v2/flashcards/3/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a86d4a9b479288bd36ec80732917d08c5bfbb39e0bbd35253f44bb8faba6b25"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/12/feedbacks
Content-Type: application/json
Authorization: Bearer bc670ee98a5f452668473c4d9aba8bfd029fecdff769c171e16b84e93a5efaed
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
    "id": 9,
    "user_id": 292,
    "feedbackable_id": 12,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T11:18:22.290Z",
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
curl "api.goskive.com/v2/flashcards/12/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc670ee98a5f452668473c4d9aba8bfd029fecdff769c171e16b84e93a5efaed"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/11/feedbacks
Content-Type: application/json
Authorization: Bearer 4db26cf7a1de3bc562ea2caa0be4016b102489f830ef6627adf820b28655c4c1
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
      "id": 8,
      "user_id": 291,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:22.076Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 290,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:22.063Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/11/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4db26cf7a1de3bc562ea2caa0be4016b102489f830ef6627adf820b28655c4c1"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/56/votes
Content-Type: application/json
Authorization: Bearer f45c85b02e6821587e03de65492fcaf3ef26d63d593b9d14a6f5405f741d598f
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 634
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 633
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 632
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f45c85b02e6821587e03de65492fcaf3ef26d63d593b9d14a6f5405f741d598f"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/14/republish
Content-Type: application/json
Authorization: Bearer e9e0cf5aaa47b5a5303000e2aa8d3ef743d097299664ac44cde2fbcc4e1ef94d
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
curl "api.goskive.com/v2/flashcards/14/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9e0cf5aaa47b5a5303000e2aa8d3ef743d097299664ac44cde2fbcc4e1ef94d"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/16/bookmark
Content-Type: application/json
Authorization: Bearer e7dfcdc257ec9a593357aa829ba1fe4dbf1ed1f5ed8380e275fe69e4ac5b35f2
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7dfcdc257ec9a593357aa829ba1fe4dbf1ed1f5ed8380e275fe69e4ac5b35f2"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/19
Content-Type: application/json
Authorization: Bearer dc2a8004ad2d80a9ef072f2e0b5d62159e6827248aad4beb1b9c3f571106c3b6
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc2a8004ad2d80a9ef072f2e0b5d62159e6827248aad4beb1b9c3f571106c3b6"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/downvote
Content-Type: application/json
Authorization: Bearer c7ea3abe59a5f716066127a4cde47f6a2a01ea4ce9e921c8cccef875cbbe3535
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7ea3abe59a5f716066127a4cde47f6a2a01ea4ce9e921c8cccef875cbbe3535"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/20
Content-Type: application/json
Authorization: Bearer 03049a4b7f73a0fab6dc0d91247d103c581c3251b93ab7c48250816a8193813c
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
    "id": 20,
    "obfuscated_id": "4DFpearSrHk",
    "author_id": 365,
    "chapter_id": 70,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:18:28.964Z",
    "created_at": "2016-11-09T11:18:28.964Z",
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
curl "api.goskive.com/v2/flashcards/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03049a4b7f73a0fab6dc0d91247d103c581c3251b93ab7c48250816a8193813c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/18/report
Content-Type: application/json
Authorization: Bearer c1f4b50cd9be07790882cd94e3d6e09e68b4ac42cdd827dd10a4fc64eb88efad
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/18/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1f4b50cd9be07790882cd94e3d6e09e68b4ac42cdd827dd10a4fc64eb88efad"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/17/bookmark
Content-Type: application/json
Authorization: Bearer 8c8f2b1ee2213b00aa51c1f3854dc441d3eca681cc42598d31968f150a0b3b69
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
	-H "Authorization: Bearer 8c8f2b1ee2213b00aa51c1f3854dc441d3eca681cc42598d31968f150a0b3b69"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/upvote
Content-Type: application/json
Authorization: Bearer cb0554c81d45608e7dd8ec004f5dda3d04e838dc46f322460b7eca5e6fe41ed7
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
	-H "Authorization: Bearer cb0554c81d45608e7dd8ec004f5dda3d04e838dc46f322460b7eca5e6fe41ed7"
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
    "key": "cache/e23c8adc4afa67da45105e20273b8074.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOVQxMjoxODoxOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2UyM2M4YWRjNGFmYTY3ZGE0NTEwNWUyMDI3M2I4MDc0LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwOS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDlUMTExODE5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161109/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161109T111819Z",
    "x-amz-signature": "cf92f8bf4ace6df677e36b724e31a160800bd1004295d683f97c16b80b4b7cce"
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
Authorization: Bearer 6649bf2121b3e627148ec801faa1477b29c9a54b25be33c519c042b0e65a6ffe
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
	-H "Authorization: Bearer 6649bf2121b3e627148ec801faa1477b29c9a54b25be33c519c042b0e65a6ffe"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 99bcc487df739ce853b6f0ca4b29f22bd14e60b54e525407fb72cdbb73f22e5d
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
	-H "Authorization: Bearer 99bcc487df739ce853b6f0ca4b29f22bd14e60b54e525407fb72cdbb73f22e5d"
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
{"password":{"reset_password_token":"JPKzjcDaYvyzszM2XgJ_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 191,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-09T11:18:14.761Z",
  "updated_at": "2016-11-09T11:18:14.905Z",
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
  "audit_id": 4309
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"JPKzjcDaYvyzszM2XgJ_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/33/comments
Content-Type: application/json
Authorization: Bearer 6b3aaf0f49421e5919f93c877339035595f21fffd769a49e638bb1d3c9c4b479
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
    "id": 8,
    "author_id": 205,
    "reply_to_id": null,
    "created_at": "2016-11-09T11:18:16.031Z",
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
curl "api.goskive.com/v2/questions/33/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b3aaf0f49421e5919f93c877339035595f21fffd769a49e638bb1d3c9c4b479"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/35/comments
Content-Type: application/json
Authorization: Bearer fee513632d26854d14bf10d6f2ac936fee4b570cde7cbfa71b4b373b7ba24ab3
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
    "id": 9,
    "author_id": 211,
    "reply_to_id": null,
    "created_at": "2016-11-09T11:18:16.858Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 2,
      "user_id": 211,
      "feedbackable_id": 35,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:16.854Z",
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
curl "api.goskive.com/v2/questions/35/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fee513632d26854d14bf10d6f2ac936fee4b570cde7cbfa71b4b373b7ba24ab3"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/36/comments
Content-Type: application/json
Authorization: Bearer dca0a68de57a833bf34538001fce11dfca6c3ae374a8cea58709721a785b9529
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
      "id": 11,
      "author_id": 218,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:18:17.396Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 217,
      "reply_to_id": null,
      "created_at": "2016-11-09T11:18:17.377Z",
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
curl "api.goskive.com/v2/questions/36/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dca0a68de57a833bf34538001fce11dfca6c3ae374a8cea58709721a785b9529"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/34/comments
Content-Type: application/json
Authorization: Bearer 7b06fb732025d21ff20b1b38b84e99c27a6f50c0506f85bfc4480ddbbbda21ac
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
curl "api.goskive.com/v2/questions/34/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b06fb732025d21ff20b1b38b84e99c27a6f50c0506f85bfc4480ddbbbda21ac"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/41/feedbacks
Content-Type: application/json
Authorization: Bearer 71b7526da236e37b585ab5e289004b0ee25e8b7d4fe7d6010d554cd9909b222c
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
    "id": 11,
    "user_id": 298,
    "feedbackable_id": 41,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-09T11:18:23.081Z",
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
curl "api.goskive.com/v2/questions/41/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71b7526da236e37b585ab5e289004b0ee25e8b7d4fe7d6010d554cd9909b222c"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/47/feedbacks
Content-Type: application/json
Authorization: Bearer df22eea128b72e9527308f71819be0ca2276a01472ae19b79765bdc1f99ba7f8
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
      "id": 18,
      "user_id": 330,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:25.563Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 329,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T11:18:25.552Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/47/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df22eea128b72e9527308f71819be0ca2276a01472ae19b79765bdc1f99ba7f8"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/81/votes
Content-Type: application/json
Authorization: Bearer db490136e574a81866840e15cb7bebad6211742a35ac140e8eb8a06b1f31c110
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 643
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 642
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 641
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/81/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db490136e574a81866840e15cb7bebad6211742a35ac140e8eb8a06b1f31c110"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/5/republish
Content-Type: application/json
Authorization: Bearer 89a7561351e66caea164d8508c4af87652f98bdf4f8456d206f1e9af9e79a8d5
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
curl "api.goskive.com/v2/questions/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89a7561351e66caea164d8508c4af87652f98bdf4f8456d206f1e9af9e79a8d5"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/9/bookmark
Content-Type: application/json
Authorization: Bearer eef767813cf714fcc1dced81d33cab7e61e81f07cdf214d1eef286ae90e0b2c0
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/9/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eef767813cf714fcc1dced81d33cab7e61e81f07cdf214d1eef286ae90e0b2c0"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/4
Content-Type: application/json
Authorization: Bearer c76e4bad625ccf4877916646eb5211eeb21ec5270b4f21159729062ae077e0e3
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c76e4bad625ccf4877916646eb5211eeb21ec5270b4f21159729062ae077e0e3"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/8/downvote
Content-Type: application/json
Authorization: Bearer 2145749783be838b3f10c2f3c8b988fced2ec20169c747622458b770ff8942c5
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/8/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2145749783be838b3f10c2f3c8b988fced2ec20169c747622458b770ff8942c5"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/1
Content-Type: application/json
Authorization: Bearer 355af26964f5cecb96494d4bb930f9090cfcaf850b602c427f29c6f2b016dbf3
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
    "id": 1,
    "obfuscated_id": "vnOJWgI0jGc",
    "author_id": 4,
    "chapter_id": 1,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:17:55.240Z",
    "created_at": "2016-11-09T11:17:55.101Z",
    "tags": [
      {
        "id": 2,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 1,
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
        "id": 1,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 2,
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
curl "api.goskive.com/v2/questions/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 355af26964f5cecb96494d4bb930f9090cfcaf850b602c427f29c6f2b016dbf3"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/7/report
Content-Type: application/json
Authorization: Bearer 094347e9788ea669471dd13dea9aa1abe0490307828b59a49e66d9dd026be3dd
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/7/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 094347e9788ea669471dd13dea9aa1abe0490307828b59a49e66d9dd026be3dd"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/2/bookmark
Content-Type: application/json
Authorization: Bearer a0bb52f5034be0257a33b0e6956623b3cc661c5624e4dda4d7ebbafc51442f76
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/2/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0bb52f5034be0257a33b0e6956623b3cc661c5624e4dda4d7ebbafc51442f76"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/10
Content-Type: application/json
Authorization: Bearer 20063595ecef79002755aa6e98901935d9a25b01bd18719cf095d230a8e8f742
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":10,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-09T11:17:59.305Z","updated_at":"2016-11-09T11:17:59.438Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":10,"author_id":31,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 10,
    "obfuscated_id": "aY5v9ahzH5c",
    "author_id": 31,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T11:17:59.554Z",
    "created_at": "2016-11-09T11:17:59.305Z",
    "tags": [
      {
        "id": 18,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 17,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>10, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-09T11:17:59.305Z\", \"updated_at\"=>\"2016-11-09T11:17:59.438Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>10, \"author_id\"=>31, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 19,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 20,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 21,
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
curl "api.goskive.com/v2/questions/10" -d '{"question":{"question":{"id":10,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-09T11:17:59.305Z","updated_at":"2016-11-09T11:17:59.438Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":10,"author_id":31,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20063595ecef79002755aa6e98901935d9a25b01bd18719cf095d230a8e8f742"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/3/upvote
Content-Type: application/json
Authorization: Bearer adf18c6a3d1054dc307e1c943dc4ad6c85e5d9b1f301643b166f60c05d09d0d7
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/3/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adf18c6a3d1054dc307e1c943dc4ad6c85e5d9b1f301643b166f60c05d09d0d7"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 9644f5f92f2c15dbda4671624691e43fd872408bd6fef5545e5be4d19318459f
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
      "creator_id": 457,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 135,
      "additional_university_ids": [

      ],
      "discipline_id": 138,
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
      "updated_at": "2016-11-09T11:18:34.942Z",
      "shortname": "mit-pizza-201",
      "topic_id": 137,
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
	-H "Authorization: Bearer 9644f5f92f2c15dbda4671624691e43fd872408bd6fef5545e5be4d19318459f"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer f656b3dd2c70e87c9de83f030b02fe1e7da0f1d76181795a7522bffce3416638
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
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-136",
      "html_url": "https://goskive.com/university/uni-136",
      "slug": "uni-136",
      "name": "National School of Pizza",
      "short_name": "Uni 136",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/22e0271fa1a95a3ebd21004566ca006480a29fb7.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ec51f7234cf2cad1e88020d64b782980e5730a00.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T11:18:35.274Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 137,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-135",
      "html_url": "https://goskive.com/university/uni-135",
      "slug": "uni-135",
      "name": "National School of Pastry",
      "short_name": "Uni 135",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dd1a4853cc7ebf29f1612ba69af39b3047aec5e9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1e9d020786692e45c632b798b71094eff5410a21.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T11:18:35.255Z",
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
	-H "Authorization: Bearer f656b3dd2c70e87c9de83f030b02fe1e7da0f1d76181795a7522bffce3416638"
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
      "id": 72,
      "name": "Fundamental intangible info-mediaries",
      "name_translations": {
        "en": "Fundamental intangible info-mediaries"
      },
      "discipline_id": 72
    },
    {
      "id": 73,
      "name": "Upgradable intermediate architecture",
      "name_translations": {
        "en": "Upgradable intermediate architecture"
      },
      "discipline_id": 73
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
GET /v2/topics/71
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
    "id": 71,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 71
  }
}
```



```shell
curl "api.goskive.com/v2/topics/71" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer bd7052659c13b496f7963d8987913ad038d4bea846e6db99b99bcef23625a9a0
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
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-27",
      "html_url": "https://goskive.com/university/uni-27",
      "slug": "uni-27",
      "name": "University 27",
      "short_name": "Uni 27",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e52f886204f3c268b5bc9c997ace9d06b6d5e0ed.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6cf2910b81a03d0b5a18d72f6ff8a336bcef109e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T11:18:05.871Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-28",
      "html_url": "https://goskive.com/university/uni-28",
      "slug": "uni-28",
      "name": "University 28",
      "short_name": "Uni 28",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3adf5d55dded610e239dbe397ff5334d61b93651.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a67816d1339855338bf38430f591ca8e9be6e8d1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T11:18:05.889Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-29",
      "html_url": "https://goskive.com/university/uni-29",
      "slug": "uni-29",
      "name": "University 29",
      "short_name": "Uni 29",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0b535ca5da2e9b29b5fbc2937a72466afa2de998.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f2aa41db8d47b411c27b0c58cd6fdb58f76e09ba.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T11:18:05.907Z",
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
	-H "Authorization: Bearer bd7052659c13b496f7963d8987913ad038d4bea846e6db99b99bcef23625a9a0"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 96091a6664ab9cd1af9c5dcc2e0dd3cd2bb754e43a9f7cfc8d12ce3e26130c85
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
    "id": 27,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/304ae157986dd569dea48362e51bee432e419196.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cf72c04ee41f93c5e3de90878b17dec10f89dee7.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-09T11:18:05.672Z",
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
	-H "Authorization: Bearer 96091a6664ab9cd1af9c5dcc2e0dd3cd2bb754e43a9f7cfc8d12ce3e26130c85"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 47ab7c9aee03c8e2344828f9711476fe3f5bb08d3c3b15ada781ddb95a209c15
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
    "creator_id": 499,
    "id": 144,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 151,
    "additional_university_ids": [

    ],
    "discipline_id": 152,
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
    "chapters_updated_at": "2016-11-09T11:18:40.818Z",
    "updated_at": "2016-11-09T11:18:40.968Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 105,
        "updated_at": "2016-11-09T11:18:40.922Z",
        "course_id": 144,
        "author_id": 499,
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
        "id": 106,
        "updated_at": "2016-11-09T11:18:40.939Z",
        "course_id": 144,
        "author_id": 499,
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
        "id": 107,
        "updated_at": "2016-11-09T11:18:40.957Z",
        "course_id": 144,
        "author_id": 499,
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
    "topic_id": 151,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":151,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47ab7c9aee03c8e2344828f9711476fe3f5bb08d3c3b15ada781ddb95a209c15"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3a1ec5ee06e5c88ac113080b4de2dc4af25c6036bb560f372fb5c230daa432b0
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":152,"published":false}}
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
    "creator_id": 500,
    "id": 145,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 152,
    "additional_university_ids": [

    ],
    "discipline_id": 153,
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
    "updated_at": "2016-11-09T11:18:41.175Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 152,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":152,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a1ec5ee06e5c88ac113080b4de2dc4af25c6036bb560f372fb5c230daa432b0"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer dd2c33dbc4edf82de449d816de5001714cffb5309f12682b5e1bc16d8cdc0861
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
      "creator_id": 507,
      "id": 153,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "discipline_id": 161,
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
      "updated_at": "2016-11-09T11:18:41.866Z",
      "shortname": "fu-course-130",
      "topic_id": 160,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 130",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 507,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "discipline_id": 162,
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
      "chapters_updated_at": "2016-11-09T11:18:41.712Z",
      "updated_at": "2016-11-09T11:18:42.187Z",
      "shortname": "fu-course-131",
      "topic_id": 161,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd2c33dbc4edf82de449d816de5001714cffb5309f12682b5e1bc16d8cdc0861"
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
      "creator_id": 527,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "discipline_id": 177,
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
      "updated_at": "2016-11-09T11:18:43.762Z",
      "shortname": "fu-course-146",
      "topic_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 527,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "discipline_id": 178,
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
      "chapters_updated_at": "2016-11-09T11:18:43.608Z",
      "updated_at": "2016-11-09T11:18:44.084Z",
      "shortname": "fu-course-147",
      "topic_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
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
Authorization: Bearer 9627213ed77e2d20150101eca2ab2c4ae114d3b080e33236289cf33d16dae122
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
      "creator_id": 513,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "discipline_id": 165,
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
      "updated_at": "2016-11-09T11:18:42.450Z",
      "shortname": "fu-course-134",
      "topic_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 513,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "discipline_id": 166,
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
      "updated_at": "2016-11-09T11:18:42.493Z",
      "shortname": "fu-course-135",
      "topic_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9627213ed77e2d20150101eca2ab2c4ae114d3b080e33236289cf33d16dae122"
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
      "creator_id": 532,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 181,
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
      "updated_at": "2016-11-09T11:18:44.271Z",
      "shortname": "fu-course-150",
      "topic_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 532,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 182,
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
      "updated_at": "2016-11-09T11:18:44.314Z",
      "shortname": "fu-course-151",
      "topic_id": 181,
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
	-H "Authorization: "
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 8616561a9a222c758249bb96da19bdf6710bdb29a59269d12f761272dce0405a
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
  "id": 261,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-09T11:18:20.573Z",
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
	-H "Authorization: Bearer 8616561a9a222c758249bb96da19bdf6710bdb29a59269d12f761272dce0405a"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/241
Content-Type: application/json
Authorization: Bearer 3ed538b33ac4f88fa3c01e229498f2fb669aa7d6112d332a024c7e90888445b8
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
    "id": 241,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 76,
    "fields_of_study": [
      74,
      75
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-09T11:18:19.404Z",
    "updated_at": "2016-11-09T11:18:19.404Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/241" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ed538b33ac4f88fa3c01e229498f2fb669aa7d6112d332a024c7e90888445b8"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/243
Content-Type: application/json
Authorization: Bearer debe1e88c7921f3ef48b9ebc6f55ee0c1fe604daa7f4853ed3085ac3fb3ad4ff
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
    "id": 243,
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
    "created_at": "2016-11-09T11:18:19.495Z",
    "updated_at": "2016-11-09T11:18:19.495Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/243" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer debe1e88c7921f3ef48b9ebc6f55ee0c1fe604daa7f4853ed3085ac3fb3ad4ff"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/15
Content-Type: application/json
Authorization: Bearer 2f35eb959f523523ca8e998a95a22d69806f0b3dd91e19b6cefe94b65286b75b
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
	-H "Authorization: Bearer 2f35eb959f523523ca8e998a95a22d69806f0b3dd91e19b6cefe94b65286b75b"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer 64d9cd507bc7323d5b3e6eae9bb70999cf2206430867ce5f6cd70104de5cb663
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
    "votable_id": 62,
    "user_id": 486
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64d9cd507bc7323d5b3e6eae9bb70999cf2206430867ce5f6cd70104de5cb663"
```
