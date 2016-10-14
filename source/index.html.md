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
Authorization: Basic MTUwNjI1MWU0N2E0ZTU1ZWI5ZGFhNjIxYzZjNzU3NGMxNGMzZDdhZGY3ZDUw
OTM2ZTgzYTg5NzIwOTc3NjQ1MjoyYTE3MzA1NGRjZmRlOTc0NGUyNzQ1YjBk
NTI2NTQwYTc3MjhlMmYzZGJhYTNhOTc2OTFlMTVhNTJmMGUxMDNm

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
	-u 1506251e47a4e55eb9daa621c6c7574c14c3d7adf7d50936e83a897209776452:2a173054dcfde9744e2745b0d526540a7728e2f3dbaa3a97691e15a52f0e103f
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a9c0f50a4f723b0c33be125d56a8d4ec9b54e1d1b3c238bb69d79ad4b16436af","client_secret":"49cac811d04d27babe3c97200f59cd0413be771ffaec3c02ced15aeab660b89a"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a9c0f50a4f723b0c33be125d56a8d4ec9b54e1d1b3c238bb69d79ad4b16436af","client_secret":"49cac811d04d27babe3c97200f59cd0413be771ffaec3c02ced15aeab660b89a"}' -X POST \
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
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"client_credentials","client_id":"d8c0bba88945cca182850fce25d86b5f6adf7ef7551a342f509a1126f7590ba5","client_secret":"ea9ebec02e347503b53f87c2591d88faa898fbb239257b96807b8a42354c7ecb"}
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
  "access_token": "bb8694693b4ae89ac594fa65e85f24e583bb6239b1580cc1f153fed7accd3d48",
  "token_type": "bearer",
  "created_at": 1476446546
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"d8c0bba88945cca182850fce25d86b5f6adf7ef7551a342f509a1126f7590ba5","client_secret":"ea9ebec02e347503b53f87c2591d88faa898fbb239257b96807b8a42354c7ecb"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ODUxN2I1YjE0YzlhZjhlMWU5YTJiYWVjZThmNDVjZWFhZjc2OWU5MjJhYzZl
M2M5ZjM1YzBhZjAyZDAxODc1YzozNjA4MjI4NTM5MmIwZDFmZjk3NWQzMzIy
OWM5MjRlNTJlMWNhODAzYTVmZGM3ZWVmMGFlNzllYjVjMTEwZGM2

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
  "access_token": "3bc144946d8b781eaa216c82ac4824d35e5051e61c4ab385118db689b06d211c",
  "token_type": "bearer",
  "created_at": 1476446546
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 8517b5b14c9af8e1e9a2baece8f45ceaaf769e922ac6e3c9f35c0af02d01875c:36082285392b0d1ff975d33229c924e52e1ca803a5fdc7eef0ae79eb5c110dc6
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"649773c51b51a11762f25bce63fe17f1276fbfe16d3e7399e60c3d363f1bc7db","client_secret":"819902229d21bc89c2a36ebb29b3b45d2562837146dc08cfc64156d3f35f3f10"}
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
  "access_token": "2278f2bd2a5757bcfa96a26de526507b6f1c301e634a3fa149998e68ad44c423",
  "token_type": "bearer",
  "created_at": 1476446546
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"649773c51b51a11762f25bce63fe17f1276fbfe16d3e7399e60c3d363f1bc7db","client_secret":"819902229d21bc89c2a36ebb29b3b45d2562837146dc08cfc64156d3f35f3f10"}' -X POST \
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
Authorization: Bearer 7ce753b718eb43a5d79a37331518eace30010bb2019905c33b7c3162a012007c
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
    "company_id": 1,
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
	-H "Authorization: Bearer 7ce753b718eb43a5d79a37331518eace30010bb2019905c33b7c3162a012007c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/10/flashcards
Content-Type: application/json
Authorization: Bearer c02b323447e340f040febbcdb8f3b155e4d12c78151c78ae10996641209cbc49
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":10,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 49,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:01:26.409Z",
    "created_at": "2016-10-14T12:01:26.409Z",
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
curl "api.goskive.com/v2/chapters/10/flashcards" -d '{"flashcard":{"chapter_id":10,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c02b323447e340f040febbcdb8f3b155e4d12c78151c78ae10996641209cbc49"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/9/flashcards
Content-Type: application/json
Authorization: Bearer c0c7806f095fc29799b9f858a5fbd337742c400a5a5f205eb3c90a800a46e5c3
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
      "id": 1,
      "obfuscated_id": "vnOJWgI0jGc",
      "author_id": 44,
      "chapter_id": 9,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:01:26.099Z",
      "created_at": "2016-10-14T12:01:26.099Z",
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
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 44,
      "chapter_id": 9,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:01:26.140Z",
      "created_at": "2016-10-14T12:01:26.140Z",
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
      "author_id": 44,
      "chapter_id": 9,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:01:26.178Z",
      "created_at": "2016-10-14T12:01:26.178Z",
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
curl "api.goskive.com/v2/chapters/9/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0c7806f095fc29799b9f858a5fbd337742c400a5a5f205eb3c90a800a46e5c3"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/145/questions
Content-Type: application/json
Authorization: Bearer 4cebb560366c102877f27b30c46e7db1162ae5e22809f8078e865ed789f334fe
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 114,
    "obfuscated_id": "RwCVsRO9fcs",
    "author_id": 736,
    "chapter_id": 145,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:24.709Z",
    "created_at": "2016-10-14T12:02:24.709Z",
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
        "id": 228,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 229,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 230,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 231,
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
curl "api.goskive.com/v2/chapters/145/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cebb560366c102877f27b30c46e7db1162ae5e22809f8078e865ed789f334fe"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/144/questions
Content-Type: application/json
Authorization: Bearer 7c8ea64fd41b81e68a544f41db6d703f9fa41a4463aab7a45f17cfa76afe36e7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":144,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 113,
    "obfuscated_id": "pcyz_ZHBlMU",
    "author_id": 733,
    "chapter_id": 144,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:24.355Z",
    "created_at": "2016-10-14T12:02:24.355Z",
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
        "id": 226,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 227,
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
curl "api.goskive.com/v2/chapters/144/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":144,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c8ea64fd41b81e68a544f41db6d703f9fa41a4463aab7a45f17cfa76afe36e7"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/146/questions
Content-Type: application/json
Authorization: Bearer 5d79cd9eb971297dad283162b5ca217612447e4777b889f133a0d76e2085ee80
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":146,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 115,
    "obfuscated_id": "tgK0VZO8yq4",
    "author_id": 739,
    "chapter_id": 146,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:25.224Z",
    "created_at": "2016-10-14T12:02:25.224Z",
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
        "id": 232,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 233,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/146/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":146,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d79cd9eb971297dad283162b5ca217612447e4777b889f133a0d76e2085ee80"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/147/questions
Content-Type: application/json
Authorization: Bearer 38409cf522dcd8aee8bfe069053505519054963fc374886c2983056263ddc4db
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":147,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 116,
    "obfuscated_id": "PhHGVKqnHFA",
    "author_id": 742,
    "chapter_id": 147,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:25.598Z",
    "created_at": "2016-10-14T12:02:25.598Z",
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
        "id": 234,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 235,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 236,
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
curl "api.goskive.com/v2/chapters/147/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":147,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38409cf522dcd8aee8bfe069053505519054963fc374886c2983056263ddc4db"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/149/questions
Content-Type: application/json
Authorization: Bearer 4df6a16c600e8695c8ac7efc5eaf9a39e36c972e00c08a3820b8d79e32b5de19
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
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 748,
      "chapter_id": 149,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:26.252Z",
      "created_at": "2016-10-14T12:02:26.129Z",
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
          "id": 237,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 238,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 749,
      "chapter_id": 149,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:26.451Z",
      "created_at": "2016-10-14T12:02:26.328Z",
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
          "id": 239,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 240,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 119,
      "obfuscated_id": "JRh8sWka24Y",
      "author_id": 750,
      "chapter_id": 149,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:26.653Z",
      "created_at": "2016-10-14T12:02:26.527Z",
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
          "id": 241,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 242,
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
curl "api.goskive.com/v2/chapters/149/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4df6a16c600e8695c8ac7efc5eaf9a39e36c972e00c08a3820b8d79e32b5de19"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/46
Content-Type: application/json
Authorization: Bearer c5642da4cf3f9a0dd26cf72a214d941f0c96f006bdc32522db56ca3995473f7d
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
curl "api.goskive.com/v2/chapters/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5642da4cf3f9a0dd26cf72a214d941f0c96f006bdc32522db56ca3995473f7d"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/48
Content-Type: application/json
Authorization: Bearer 44e37b5c1a5d9a0e92433193bbdd5a0afe32e23d4d9168820c770dc59dda0ca3
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
curl "api.goskive.com/v2/chapters/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44e37b5c1a5d9a0e92433193bbdd5a0afe32e23d4d9168820c770dc59dda0ca3"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/43
Content-Type: application/json
Authorization: Bearer cf55e7c2c08af453ef9fc873b8ef9bebb118dfd9089c39e51693c80e1bcaf784
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
curl "api.goskive.com/v2/chapters/43" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf55e7c2c08af453ef9fc873b8ef9bebb118dfd9089c39e51693c80e1bcaf784"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/47
Content-Type: application/json
Authorization: Bearer 3b0e0528f49e0abe08a258f5a01841fc3ca295f1061f49fdc4b24f7756144e04
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b0e0528f49e0abe08a258f5a01841fc3ca295f1061f49fdc4b24f7756144e04"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/49
Content-Type: application/json
Authorization: Bearer 329c642c78669476ef4aeb3766908259e8599c7dd62f5e684f1d66b089bd35d2
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
    "id": 49,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T12:01:46.614Z",
    "course_id": 65,
    "author_id": 217,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-14T12:01:46.068Z",
    "questions_updated_at": "2016-10-14T12:01:46.068Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 221,
        "chapter_id": 49,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:46.596Z",
        "created_at": "2016-10-14T12:01:46.596Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 219,
        "chapter_id": 49,
        "position": 48,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:46.487Z",
        "created_at": "2016-10-14T12:01:46.366Z",
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
            "id": 95,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 96,
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
curl "api.goskive.com/v2/chapters/49" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 329c642c78669476ef4aeb3766908259e8599c7dd62f5e684f1d66b089bd35d2"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/42
Content-Type: application/json
Authorization: Bearer 599ec2e0e8be1c6f15a8db4791d928ee000dd9be7f3013da13b354292e928c6b
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
    "id": 42,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T12:01:44.787Z",
    "course_id": 58,
    "author_id": 197,
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
curl "api.goskive.com/v2/chapters/42" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 599ec2e0e8be1c6f15a8db4791d928ee000dd9be7f3013da13b354292e928c6b"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/53/replies
Content-Type: application/json
Authorization: Bearer f517f8208cb50e0117810cc6d06a5849d64a90c6da57d8077d18c11b404fb519
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
    "id": 54,
    "author_id": 406,
    "reply_to_id": 53,
    "created_at": "2016-10-14T12:01:58.532Z",
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
curl "api.goskive.com/v2/comments/53/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f517f8208cb50e0117810cc6d06a5849d64a90c6da57d8077d18c11b404fb519"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/55/replies
Content-Type: application/json
Authorization: Bearer 22f87d7437c0c73057bc824babddc11e2d56d29660d1988ef6d95ef28b5ce7e9
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
curl "api.goskive.com/v2/comments/55/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22f87d7437c0c73057bc824babddc11e2d56d29660d1988ef6d95ef28b5ce7e9"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer 7f507613d9940eac8ed852489b3a72a7dd9a4d4445056c6845205f58aba810ae
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
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f507613d9940eac8ed852489b3a72a7dd9a4d4445056c6845205f58aba810ae"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/50/republish
Content-Type: application/json
Authorization: Bearer a27d1d846c1757dffe13c53354faae2ee878046486b3ec2f6cbf75c4749c5223
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
	-H "Authorization: Bearer a27d1d846c1757dffe13c53354faae2ee878046486b3ec2f6cbf75c4749c5223"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 7516270722803e69f33f8731daa529541f3ed92445dd0f7008420602931c8c99
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7516270722803e69f33f8731daa529541f3ed92445dd0f7008420602931c8c99"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/52/report
Content-Type: application/json
Authorization: Bearer 0c3b35316696a1e98d0d6e268e17144df186e72b039d553025ef632710eac66b
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c3b35316696a1e98d0d6e268e17144df186e72b039d553025ef632710eac66b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/10
Content-Type: application/json
Authorization: Bearer 58cd2dbda50cbe2cac90c3f345578d55a76cacc37c13631cef30173a130dc8ac
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
    "id": 10,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-14T12:01:33.965Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58cd2dbda50cbe2cac90c3f345578d55a76cacc37c13631cef30173a130dc8ac"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer e0eab50457528067f7c0e002edf883ab4051ac6054f77871653d5577279df0d7
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
      "id": 11,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T12:01:34.043Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T12:01:34.048Z"
    },
    {
      "id": 13,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T12:01:34.052Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0eab50457528067f7c0e002edf883ab4051ac6054f77871653d5577279df0d7"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/31/company_profiles
Content-Type: application/json
Authorization: Bearer 7e1ad59eb12a1c4e7e17e89535303f618ad16aea868f3c697c2e82f614a065ea
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
curl "api.goskive.com/v2/companies/31/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e1ad59eb12a1c4e7e17e89535303f618ad16aea868f3c697c2e82f614a065ea"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 1ecbe927e98808d4760b12ec3fc71a80c2bdaea919f276c3eeefe89298901592
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
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ecbe927e98808d4760b12ec3fc71a80c2bdaea919f276c3eeefe89298901592"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 130523240f0c99909824fdd672a48de7a0ab3857afd14960c9ad5c5303fb0079
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
      "id": 6,
      "title": "Campaign 5",
      "company_id": 20,
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
	-H "Authorization: Bearer 130523240f0c99909824fdd672a48de7a0ab3857afd14960c9ad5c5303fb0079"
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
Authorization: Bearer 33551271ebeb3b45722c0fc1e492826ee84e3475fb13c7e0ac2c1c391902a40b
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
	-H "Authorization: Bearer 33551271ebeb3b45722c0fc1e492826ee84e3475fb13c7e0ac2c1c391902a40b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6522a88ec5329693531cf15749b6212e8f2e8ecb15b83a7d1dbb7c81a9caca65
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
    "id": 96,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T12:02:12.581Z",
    "course_id": 182,
    "author_id": 600,
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
	-H "Authorization: Bearer 6522a88ec5329693531cf15749b6212e8f2e8ecb15b83a7d1dbb7c81a9caca65"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 17c7adfc2e2d39194d937557ff493838090a1f50d2180e419056252126dec61e
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
      "id": 104,
      "title": "Clever Chapter Title 89",
      "position": 1,
      "updated_at": "2016-10-14T12:02:13.715Z",
      "course_id": 188,
      "author_id": 620,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 105,
      "title": "Clever Chapter Title 90",
      "position": 2,
      "updated_at": "2016-10-14T12:02:13.741Z",
      "course_id": 188,
      "author_id": 621,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 106,
      "title": "Clever Chapter Title 91",
      "position": 3,
      "updated_at": "2016-10-14T12:02:14.005Z",
      "course_id": 188,
      "author_id": 622,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T12:02:13.635Z",
      "questions_updated_at": "2016-10-14T12:02:13.635Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17c7adfc2e2d39194d937557ff493838090a1f50d2180e419056252126dec61e"
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
      "id": 110,
      "title": "Clever Chapter Title 95",
      "position": 1,
      "updated_at": "2016-10-14T12:02:14.488Z",
      "course_id": 191,
      "author_id": 634,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 111,
      "title": "Clever Chapter Title 96",
      "position": 2,
      "updated_at": "2016-10-14T12:02:14.513Z",
      "course_id": 191,
      "author_id": 635,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 112,
      "title": "Clever Chapter Title 97",
      "position": 3,
      "updated_at": "2016-10-14T12:02:14.770Z",
      "course_id": 191,
      "author_id": 636,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T12:02:14.410Z",
      "questions_updated_at": "2016-10-14T12:02:14.410Z",
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
Authorization: Bearer 0af094ac2b091ab47fb7de80249f820c8989dd59da2564f0d950fe28b3fd1123
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
      "id": 107,
      "title": "Clever Chapter Title 92",
      "position": 1,
      "updated_at": "2016-10-14T12:02:14.168Z",
      "course_id": 189,
      "author_id": 627,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 108,
      "title": "Clever Chapter Title 93",
      "position": 2,
      "updated_at": "2016-10-14T12:02:14.194Z",
      "course_id": 189,
      "author_id": 628,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 109,
      "title": "Clever Chapter Title 94",
      "position": 3,
      "updated_at": "2016-10-14T12:02:14.219Z",
      "course_id": 189,
      "author_id": 629,
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
	-H "Authorization: Bearer 0af094ac2b091ab47fb7de80249f820c8989dd59da2564f0d950fe28b3fd1123"
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
      "id": 113,
      "title": "Clever Chapter Title 98",
      "position": 1,
      "updated_at": "2016-10-14T12:02:14.973Z",
      "course_id": 193,
      "author_id": 641,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 114,
      "title": "Clever Chapter Title 99",
      "position": 2,
      "updated_at": "2016-10-14T12:02:14.998Z",
      "course_id": 193,
      "author_id": 642,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 115,
      "title": "Clever Chapter Title 100",
      "position": 3,
      "updated_at": "2016-10-14T12:02:15.024Z",
      "course_id": 193,
      "author_id": 643,
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
Authorization: Bearer b73ccd96e496bbbf3f74236cb33d4cc65387a60bf5e713863c9f922602c3c8f6
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
    "course_id": 86,
    "user_id": 278,
    "updated_at": "2016-10-14T12:01:51.998Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b73ccd96e496bbbf3f74236cb33d4cc65387a60bf5e713863c9f922602c3c8f6"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7604863a372e90b8feaa893ef0f52ac0bb625c5dbfe62af81373bc30e34a17e4
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
      "course_id": 83,
      "user_id": 270,
      "updated_at": "2016-10-14T12:01:51.542Z"
    },
    {
      "id": 5,
      "course_id": 83,
      "user_id": 271,
      "updated_at": "2016-10-14T12:01:51.558Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7604863a372e90b8feaa893ef0f52ac0bb625c5dbfe62af81373bc30e34a17e4"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/148/files
Content-Type: application/json
Authorization: Bearer af0432b5937cb2f3310dedb66df7fde5cbde55c4298ca4f73f6e3c339a44c898
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
      "id": 8,
      "uploader": {
        "id": 455,
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
        "created_at": "2016-10-14T12:02:02.914Z",
        "updated_at": "2016-10-14T12:02:02.914Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:02:02.921Z",
      "updated_at": "2016-10-14T12:02:02.921Z",
      "course_id": 148,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 456,
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
        "created_at": "2016-10-14T12:02:02.928Z",
        "updated_at": "2016-10-14T12:02:02.928Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:02:02.936Z",
      "updated_at": "2016-10-14T12:02:02.936Z",
      "course_id": 148,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 10,
      "uploader": {
        "id": 457,
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
        "created_at": "2016-10-14T12:02:02.943Z",
        "updated_at": "2016-10-14T12:02:02.943Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:02:02.950Z",
      "updated_at": "2016-10-14T12:02:02.950Z",
      "course_id": 148,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/148/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af0432b5937cb2f3310dedb66df7fde5cbde55c4298ca4f73f6e3c339a44c898"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/151/files
Content-Type: application/json
Authorization: Bearer 78993560a54f711049fd41afbc1f59a6647fe5588769a9710f4355ba078e9942
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
    "id": 11,
    "uploader": {
      "id": 464,
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
      "created_at": "2016-10-14T12:02:03.286Z",
      "updated_at": "2016-10-14T12:02:03.286Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-14T12:02:03.316Z",
    "updated_at": "2016-10-14T12:02:03.316Z",
    "course_id": 151,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/151/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78993560a54f711049fd41afbc1f59a6647fe5588769a9710f4355ba078e9942"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/150/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 288021861e7ac497e822967a2f2b769da3e3cde2a3a23dee3f69dccf6a06e6f7
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
    "key": "cache/4833000d2a666b7b497c3988b7e881b5.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMzowMjowM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS80ODMzMDAwZDJhNjY2YjdiNDk3YzM5ODhiN2U4ODFiNS5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTIwMjAzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T120203Z",
    "x-amz-signature": "5f841f4498e0a49cf93a345ff6ef0e122052e49711e6c91062a38cc956d906d3"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/150/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 288021861e7ac497e822967a2f2b769da3e3cde2a3a23dee3f69dccf6a06e6f7"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer ee062747cad2c46eed9954cbd3bab3b1199fd4fdf21a9768a9c42e4cc29f60ed
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
	-H "Authorization: Bearer ee062747cad2c46eed9954cbd3bab3b1199fd4fdf21a9768a9c42e4cc29f60ed"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3fac98efae6981fbda8ee2c1827b6ec561da53a08081e9f542455951ab33dbd3
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
	-H "Authorization: Bearer 3fac98efae6981fbda8ee2c1827b6ec561da53a08081e9f542455951ab33dbd3"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 57dcacc9cf0ede82dd7c28a145a03894c77bea9b5a25a379bf115c89c080d8dc
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
	-H "Authorization: Bearer 57dcacc9cf0ede82dd7c28a145a03894c77bea9b5a25a379bf115c89c080d8dc"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9841acf9989b631a0916c21228aaa270491042f66f5fe7db00c26acfd9cbe004
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
	-H "Authorization: Bearer 9841acf9989b631a0916c21228aaa270491042f66f5fe7db00c26acfd9cbe004"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0a3ca67d1341a8950c7c09d9eff96523f8be6185d1d54747cbbae78765699e00
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
	-H "Authorization: Bearer 0a3ca67d1341a8950c7c09d9eff96523f8be6185d1d54747cbbae78765699e00"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer d4baf5d20686441d25da589ecbcbfe22a1cf17aa80ac4b9da404f9d7ad67f501
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
    "creator_id": 162,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 48,
    "additional_university_ids": [

    ],
    "topic_id": 56,
    "discipline_id": 56,
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
    "chapters_updated_at": "2016-10-14T12:01:36.951Z",
    "updated_at": "2016-10-14T12:01:38.573Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 34,
        "title": "Clever Chapter Title 31",
        "position": 1,
        "updated_at": "2016-10-14T12:01:38.524Z",
        "course_id": 48,
        "author_id": 162,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:01:36.951Z",
        "questions_updated_at": "2016-10-14T12:01:36.951Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 35,
        "title": "Clever Chapter Title 32",
        "position": 2,
        "updated_at": "2016-10-14T12:01:38.565Z",
        "course_id": 48,
        "author_id": 162,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:01:36.951Z",
        "questions_updated_at": "2016-10-14T12:01:36.951Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 163,
        "chapter_id": 34,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:38.352Z",
        "created_at": "2016-10-14T12:01:38.352Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 163,
        "chapter_id": 35,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:38.429Z",
        "created_at": "2016-10-14T12:01:38.429Z",
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
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 163,
        "chapter_id": 34,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:38.395Z",
        "created_at": "2016-10-14T12:01:38.395Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 163,
        "chapter_id": 35,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:38.472Z",
        "created_at": "2016-10-14T12:01:38.472Z",
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
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 163,
        "chapter_id": 34,
        "position": 21,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:37.195Z",
        "created_at": "2016-10-14T12:01:37.051Z",
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
            "id": 41,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 42,
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
        "author_id": 163,
        "chapter_id": 34,
        "position": 22,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:37.396Z",
        "created_at": "2016-10-14T12:01:37.266Z",
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
      },
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 163,
        "chapter_id": 35,
        "position": 23,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:37.629Z",
        "created_at": "2016-10-14T12:01:37.487Z",
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
            "id": 45,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 46,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 163,
        "chapter_id": 35,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:37.836Z",
        "created_at": "2016-10-14T12:01:37.703Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4baf5d20686441d25da589ecbcbfe22a1cf17aa80ac4b9da404f9d7ad67f501"
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
    "creator_id": 174,
    "id": 50,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 50,
    "additional_university_ids": [

    ],
    "topic_id": 58,
    "discipline_id": 58,
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
    "chapters_updated_at": "2016-10-14T12:01:40.469Z",
    "updated_at": "2016-10-14T12:01:42.186Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 38,
        "title": "Clever Chapter Title 35",
        "position": 1,
        "updated_at": "2016-10-14T12:01:42.129Z",
        "course_id": 50,
        "author_id": 174,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:01:40.469Z",
        "questions_updated_at": "2016-10-14T12:01:40.469Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 39,
        "title": "Clever Chapter Title 36",
        "position": 2,
        "updated_at": "2016-10-14T12:01:42.177Z",
        "course_id": 50,
        "author_id": 174,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:01:40.469Z",
        "questions_updated_at": "2016-10-14T12:01:40.469Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 174,
        "chapter_id": 38,
        "position": 33,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.706Z",
        "created_at": "2016-10-14T12:01:40.564Z",
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
            "id": 65,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 66,
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
        "author_id": 174,
        "chapter_id": 39,
        "position": 35,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:41.158Z",
        "created_at": "2016-10-14T12:01:41.010Z",
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
PUT /v2/courses/57/pin
Content-Type: application/json
Authorization: Bearer 65a9c4a8cbff27c273a05e8fc5b455837191064f450f46fcb29f82717788483a
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/57/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65a9c4a8cbff27c273a05e8fc5b455837191064f450f46fcb29f82717788483a"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/56/pin
Content-Type: application/json
Authorization: Bearer 2236f02431930e5cc925ba0a8d3617047e7c5a5fdeceb1ae17d6eb230b070969
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/56/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2236f02431930e5cc925ba0a8d3617047e7c5a5fdeceb1ae17d6eb230b070969"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fb1ae46ac64385b2ef1f19c17ca42bd8fe493361230bb8f2a06467bbc3d94659
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
    "creator_id": 187,
    "id": 53,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 53,
    "additional_university_ids": [

    ],
    "topic_id": 61,
    "discipline_id": 61,
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
    "updated_at": "2016-10-14T12:01:44.124Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb1ae46ac64385b2ef1f19c17ca42bd8fe493361230bb8f2a06467bbc3d94659"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 6507b75fe9e3cf26af03798161f6da622fa8cd8cea0c4f17d5776885ed0db491
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
    "id": 133,
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
    "created_at": "2016-10-14T12:01:34.164Z",
    "updated_at": "2016-10-14T12:01:34.164Z",
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
	-H "Authorization: Bearer 6507b75fe9e3cf26af03798161f6da622fa8cd8cea0c4f17d5776885ed0db491"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0bbb01d7c6062677cf7f38ce841ed63a0e148fa41e282f73e9cd48c08e2d9541
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[42]}
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
    "id": 135,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      42
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:01:34.669Z",
    "updated_at": "2016-10-14T12:01:34.705Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[42]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bbb01d7c6062677cf7f38ce841ed63a0e148fa41e282f73e9cd48c08e2d9541"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer e863e158250e8f603504f3e444b38ce250f8f1de70680fbc2fb99d34288ac72c
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
    "id": 138,
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
    "created_at": "2016-10-14T12:01:34.875Z",
    "updated_at": "2016-10-14T12:01:34.875Z",
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
	-H "Authorization: Bearer e863e158250e8f603504f3e444b38ce250f8f1de70680fbc2fb99d34288ac72c"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 24753d8580e58f223228f87a9461b6655551710af4ef917c287d124cd4f702cc
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[44]}
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
    "id": 137,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      44
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:01:34.824Z",
    "updated_at": "2016-10-14T12:01:34.824Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[44]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24753d8580e58f223228f87a9461b6655551710af4ef917c287d124cd4f702cc"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 27ebba21a7c2d55d4219ba03ccc636b4692e739baf394fbf1970e8ac96908b4c
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

41
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
    "id": 134,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/7f451bf4c59c29a30f6b18013c4bc01800e2ccb1.jpg",
    "university_id": null,
    "fields_of_study": [
      41
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:01:34.263Z",
    "updated_at": "2016-10-14T12:01:34.616Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/88bf60262bb1454abbb303efe96df9043d867070.jpg",
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

41
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 27ebba21a7c2d55d4219ba03ccc636b4692e739baf394fbf1970e8ac96908b4c"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 5f3c9044e1f5cc00e5a60dc07b75cfd848f93772c8b0db8c521fb2d724319fb0
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
      "bookmarkable_id": 128,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 129,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 130,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f3c9044e1f5cc00e5a60dc07b75cfd848f93772c8b0db8c521fb2d724319fb0"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer de04ec34e29f668e9a892910b464f0cc470c46f4d34d2440ec690fad82489c80
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
      "company_id": 36,
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
      "company_id": 37,
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
	-H "Authorization: Bearer de04ec34e29f668e9a892910b464f0cc470c46f4d34d2440ec690fad82489c80"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer affde6d6f7d6506956fb5f51fbd9a81989975f3c2affc725f78fb6162f46daf9
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
      "company_id": 32,
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
	-H "Authorization: Bearer affde6d6f7d6506956fb5f51fbd9a81989975f3c2affc725f78fb6162f46daf9"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 3bac949ae8794076e5304b2ad3e0371865505dd2ceeb35a375102684b2e381d9
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
      "creator_id": 379,
      "id": 129,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-88",
      "html_url": "https://goskive.com/course/mit-course-88",
      "slug": "mit-course-88",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 139,
      "discipline_id": 140,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 88",
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
      "updated_at": "2016-10-14T12:01:57.009Z",
      "shortname": "mit-course-88"
    },
    {
      "creator_id": 380,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-89",
      "html_url": "https://goskive.com/course/mit-course-89",
      "slug": "mit-course-89",
      "university_id": 131,
      "additional_university_ids": [

      ],
      "topic_id": 140,
      "discipline_id": 141,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
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
      "updated_at": "2016-10-14T12:01:57.093Z",
      "shortname": "mit-course-89"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bac949ae8794076e5304b2ad3e0371865505dd2ceeb35a375102684b2e381d9"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cf36d135e9740e4e261c9bb9dfbec872e6045d9eef05647db4d5c95e220f65f3
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T12:01:33.676Z"
      },
      "created_at": "2016-10-14T12:01:33.680Z",
      "updated_at": "2016-10-14T12:01:33.680Z",
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
      "company_id": 8,
      "company": {
        "id": 8,
        "name": "Fake Company Name 7",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T12:01:33.689Z"
      },
      "created_at": "2016-10-14T12:01:33.693Z",
      "updated_at": "2016-10-14T12:01:33.693Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf36d135e9740e4e261c9bb9dfbec872e6045d9eef05647db4d5c95e220f65f3"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e6c159006102a9a49343228fb654cc174f9a6555ddb9c8f6b7ee8af00da52cec
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
      "company_id": 3,
      "company": {
        "id": 3,
        "name": "Fake Company Name 2",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T12:01:33.378Z"
      },
      "created_at": "2016-10-14T12:01:33.384Z",
      "updated_at": "2016-10-14T12:01:33.384Z",
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
      "company_id": 4,
      "company": {
        "id": 4,
        "name": "Fake Company Name 3",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-14T12:01:33.400Z"
      },
      "created_at": "2016-10-14T12:01:33.404Z",
      "updated_at": "2016-10-14T12:01:33.404Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6c159006102a9a49343228fb654cc174f9a6555ddb9c8f6b7ee8af00da52cec"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer f2ea68e5a8a57b5ff23b9b7f6e34eb3dc37d9a9ee2acf4ba16b60f294f9645d7
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
      "created_at": "2016-10-14T12:01:30.045Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-10-14T12:01:30.157Z",
      "author_id": "88",
      "thread_subject_id": "27",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 6,
      "created_at": "2016-10-14T12:01:30.145Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-10-14T12:01:30.160Z",
      "author_id": "91",
      "thread_subject_id": "28",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-14T12:01:30.560Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-14T12:01:30.560Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-10-14T12:01:30.952Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-10-14T12:01:30.952Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 9,
      "created_at": "2016-10-14T12:01:31.344Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-14T12:01:31.344Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 10,
      "created_at": "2016-10-14T12:01:31.684Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 15,
      "updated_at": "2016-10-14T12:01:31.684Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-14T12:01:32.005Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 16,
      "updated_at": "2016-10-14T12:01:32.005Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-10-14T12:01:32.323Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 17,
      "updated_at": "2016-10-14T12:01:32.323Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2ea68e5a8a57b5ff23b9b7f6e34eb3dc37d9a9ee2acf4ba16b60f294f9645d7"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/4
Content-Type: application/json
Authorization: Bearer e7216dc2efdfbedcfb5657b5fc8f040ff48a5d8b86fecffee3c52a4963f724dd
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-14T11:51:29.000Z"}}
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
    "created_at": "2016-10-14T12:01:29.876Z",
    "read_at": "2016-10-14T11:51:29.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 5,
    "updated_at": "2016-10-14T12:01:29.933Z",
    "author_id": "84",
    "thread_subject_id": "26",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/4" -d '{"notification":{"read_at":"2016-10-14T11:51:29.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7216dc2efdfbedcfb5657b5fc8f040ff48a5d8b86fecffee3c52a4963f724dd"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 140b206b6cd0c2a7b81af1f5c3c5637d59f2b6d16d7e29a9c3d6a76f2bee9eab
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
      "id": 3,
      "course_id": 11,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T12:01:25.418Z",
      "course_published": true,
      "updated_at": "2016-10-14T12:01:25.410Z"
    },
    {
      "id": 4,
      "course_id": 12,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T12:01:25.504Z",
      "course_published": true,
      "updated_at": "2016-10-14T12:01:25.496Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 140b206b6cd0c2a7b81af1f5c3c5637d59f2b6d16d7e29a9c3d6a76f2bee9eab"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer c525a6f6241038683649438fd5a253cff6c08cd9ebb70eaa26b45ba2b8dbe300
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
    "course_id": 8,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T12:01:25.043Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:01:25.034Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c525a6f6241038683649438fd5a253cff6c08cd9ebb70eaa26b45ba2b8dbe300"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 5f0fb26ddf28440b0e395cacded376b19eed0af5c33988871aaf198205c302d6
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
    "course_id": 13,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-14T12:01:25.726Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:01:25.714Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f0fb26ddf28440b0e395cacded376b19eed0af5c33988871aaf198205c302d6"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 9d0f8e9bbf865d33ea53ed5aee807c1648f0f8ec8639f4aa3b83e605b40aaae7
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
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 8,
      "user_id": 51
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 9,
      "user_id": 51
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 10,
      "user_id": 51
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 11,
      "user_id": 51
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d0f8e9bbf865d33ea53ed5aee807c1648f0f8ec8639f4aa3b83e605b40aaae7"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/90
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
    "id": 90,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 88,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 90
      },
      {
        "id": 89,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 90
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/90" -X GET \
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
      "id": 88,
      "name": "Grass-roots 4th generation utilisation",
      "name_translations": {
        "en": "Grass-roots 4th generation utilisation"
      }
    },
    {
      "id": 89,
      "name": "Open-architected grid-enabled customer loyalty",
      "name_translations": {
        "en": "Open-architected grid-enabled customer loyalty"
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
Authorization: Bearer 1ca1e2e4e90a4b7676707a7f9eefdc725318debf69eb8e98c4b15b8c458f4f2f
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
    "user_id": 477,
    "feedbackable_id": 45,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-14T12:02:04.115Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ca1e2e4e90a4b7676707a7f9eefdc725318debf69eb8e98c4b15b8c458f4f2f"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/fix
Content-Type: application/json
Authorization: Bearer a57920f51be3b179284f581140237a6537b63fbe5361656854c202e32f0c3b5d
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
    "id": 35,
    "user_id": 578,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-14T12:02:11.408Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/35/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a57920f51be3b179284f581140237a6537b63fbe5361656854c202e32f0c3b5d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/37
Content-Type: application/json
Authorization: Bearer 70c6a250cbdaa70d4d9ef9ccaa3a6293ea79c7646aed0fc2691b8741132c2669
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
    "id": 37,
    "user_id": 588,
    "feedbackable_id": 51,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:02:11.999Z",
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
curl "api.goskive.com/v2/feedbacks/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70c6a250cbdaa70d4d9ef9ccaa3a6293ea79c7646aed0fc2691b8741132c2669"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/close
Content-Type: application/json
Authorization: Bearer 3eaf311a6aed83e328ebfd02608b85ecd0b21e5f23956605fc90f10f3546a250
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
curl "api.goskive.com/v2/feedbacks/13/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eaf311a6aed83e328ebfd02608b85ecd0b21e5f23956605fc90f10f3546a250"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/33/fix
Content-Type: application/json
Authorization: Bearer 452dafeb3a40272dbe1ccab5bc258cd2b75d79d3c6425f57036a9a88f081321c
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
curl "api.goskive.com/v2/feedbacks/33/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 452dafeb3a40272dbe1ccab5bc258cd2b75d79d3c6425f57036a9a88f081321c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/36/fix
Content-Type: application/json
Authorization: Bearer cdaeb04998e5e6281df3d5f294345fd63f4f0ba98cdcbc6fd19330ef47549bd7
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
	-H "Authorization: Bearer cdaeb04998e5e6281df3d5f294345fd63f4f0ba98cdcbc6fd19330ef47549bd7"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/38
Content-Type: application/json
Authorization: Bearer 03cb8d2e98933c1ac68c0a5507bb1cc1f6f6241499c04af61b1c65e445523387
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
    "id": 38,
    "user_id": 593,
    "feedbackable_id": 52,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:02:12.290Z",
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
curl "api.goskive.com/v2/feedbacks/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03cb8d2e98933c1ac68c0a5507bb1cc1f6f6241499c04af61b1c65e445523387"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 6718733095db41f4aa5caddb318c64c6e38fb2d5de578cfcf25596e47f848a33
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
curl "api.goskive.com/v2/files/4" -d '' -X DELETE \
	-H "Authorization: Bearer 6718733095db41f4aa5caddb318c64c6e38fb2d5de578cfcf25596e47f848a33" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer 68c3b7da1c5a27471c5f51a1c6de3f2cd7dd858c88d0daa419e26db4992e71df
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
	-H "Authorization: Bearer 68c3b7da1c5a27471c5f51a1c6de3f2cd7dd858c88d0daa419e26db4992e71df" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/3
Authorization: Bearer 7a120726771d88455e01f41411346b1103ea94304390736a7bbc5aadb2ed8aa3
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/1ea8344eac64d512ea012bc95a36d878.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T120157Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=7de9301403641bfabe6cc2b03e5634740bf235b26784c41bb7145f4e931323b7"
  }
}
```



```shell
curl "api.goskive.com/v2/files/3" -X GET \
	-H "Authorization: Bearer 7a120726771d88455e01f41411346b1103ea94304390736a7bbc5aadb2ed8aa3"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/2/metadata
Authorization: Bearer a65863a8aea1692cb775dae38c7431358bc06707e904dafd5100cdffdebdf59d
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
    "id": 2,
    "uploader": {
      "id": 385,
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
      "created_at": "2016-10-14T12:01:57.428Z",
      "updated_at": "2016-10-14T12:01:57.428Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-14T12:01:57.504Z",
    "updated_at": "2016-10-14T12:01:57.504Z",
    "course_id": 132,
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
curl "api.goskive.com/v2/files/2/metadata" -X GET \
	-H "Authorization: Bearer a65863a8aea1692cb775dae38c7431358bc06707e904dafd5100cdffdebdf59d" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/13/matched_courses?required_cu_count=2
Authorization: Bearer acbbca6aab7955f14ed21ed9490524fada994860ff18258ac94a22738dedf4da
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
      "creator_id": 771,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 232,
      "additional_university_ids": [

      ],
      "topic_id": 242,
      "discipline_id": 243,
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
      "chapters_updated_at": "2016-10-14T12:02:27.108Z",
      "updated_at": "2016-10-14T12:02:28.777Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 776,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-cd61f906-dd47-4f6a-b421-51feffdec080",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-cd61f906-dd47-4f6a-b421-51feffdec080",
      "slug": "mit-the-great-british-bake-off-cd61f906-dd47-4f6a-b421-51feffdec080",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "topic_id": 243,
      "discipline_id": 244,
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
      "chapters_updated_at": "2016-10-14T12:02:27.108Z",
      "updated_at": "2016-10-14T12:02:29.358Z",
      "shortname": "mit-the-great-british-bake-off-cd61f906-dd47-4f6a-b421-51feffdec080"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/13/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer acbbca6aab7955f14ed21ed9490524fada994860ff18258ac94a22738dedf4da"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/1/preview
Authorization: Bearer 790bb81235ad60302d166d586339f6ac5c40c02d4fe95b15b4cb2d85d80dc22f
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/b81802387946b40f0a1103397e9cc17a.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T120157Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=28819897b98d44dd2ca4b03e7954b8fe663d75d57c03bf072719f0ecbb95c7c1"
  }
}
```



```shell
curl "api.goskive.com/v2/files/1/preview" -X GET \
	-H "Authorization: Bearer 790bb81235ad60302d166d586339f6ac5c40c02d4fe95b15b4cb2d85d80dc22f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/7/report
Authorization: Bearer 8d261d4cb755f25e48aa410c6bf9ca2b05f379893b74cc573ce1c26f92fa3eaf
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
curl "api.goskive.com/v2/files/7/report" -d '' -X PUT \
	-H "Authorization: Bearer 8d261d4cb755f25e48aa410c6bf9ca2b05f379893b74cc573ce1c26f92fa3eaf" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/5/comments
Content-Type: application/json
Authorization: Bearer cdb5f9841cb81809ebb971e33676fbaec9e9d108b711b73d80b514b34281433e
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
    "id": 1,
    "author_id": 65,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:01:28.418Z",
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
curl "api.goskive.com/v2/flashcards/5/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdb5f9841cb81809ebb971e33676fbaec9e9d108b711b73d80b514b34281433e"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/6/comments
Content-Type: application/json
Authorization: Bearer 58627920125309dde87633d6059f4c65c1c29a1eafb1ed0a496730e1fd8c96b6
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
    "id": 2,
    "author_id": 68,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:01:29.039Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 68,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:01:29.034Z",
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
curl "api.goskive.com/v2/flashcards/6/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58627920125309dde87633d6059f4c65c1c29a1eafb1ed0a496730e1fd8c96b6"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer f9ef9f6ab207dae682fb3d9ae5c407d7d3769b3fe3bdea162962083fd713a0d5
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
      "id": 4,
      "author_id": 81,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:29.732Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 80,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:29.715Z",
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
curl "api.goskive.com/v2/flashcards/9/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9ef9f6ab207dae682fb3d9ae5c407d7d3769b3fe3bdea162962083fd713a0d5"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/7/comments
Content-Type: application/json
Authorization: Bearer f4c3e4e0e2cdd0d8a8cf0505f709002d43ec7ddfdb3caa49e3faade8a4188b28
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
curl "api.goskive.com/v2/flashcards/7/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4c3e4e0e2cdd0d8a8cf0505f709002d43ec7ddfdb3caa49e3faade8a4188b28"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/61/feedbacks
Content-Type: application/json
Authorization: Bearer 635e2194b7b64bfedf0672b7dd9f8fca4977e35df624bfa423d29672a09ec26f
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
    "id": 40,
    "user_id": 802,
    "feedbackable_id": 61,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:02:31.332Z",
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
curl "api.goskive.com/v2/flashcards/61/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 635e2194b7b64bfedf0672b7dd9f8fca4977e35df624bfa423d29672a09ec26f"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/67/feedbacks
Content-Type: application/json
Authorization: Bearer a5b02c4f23817f5b1658f0c4ba67244259519b5be88e76e4ae695188366c6b7c
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
      "id": 46,
      "user_id": 834,
      "feedbackable_id": 67,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:32.628Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 833,
      "feedbackable_id": 67,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:32.617Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/67/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5b02c4f23817f5b1658f0c4ba67244259519b5be88e76e4ae695188366c6b7c"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/11/votes
Content-Type: application/json
Authorization: Bearer 453a303c03a1b90f3bbb4ea3060a9e55dbb99367cee71bac7b3645a849df5e8f
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
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 11,
      "user_id": 123
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 11,
      "user_id": 122
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 11,
      "user_id": 121
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/11/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 453a303c03a1b90f3bbb4ea3060a9e55dbb99367cee71bac7b3645a849df5e8f"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/70/republish
Content-Type: application/json
Authorization: Bearer e1dea95d112e260f9347c06db1d2d9067706b414be4e26109f7881d04ff45e10
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
curl "api.goskive.com/v2/flashcards/70/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1dea95d112e260f9347c06db1d2d9067706b414be4e26109f7881d04ff45e10"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/76/bookmark
Content-Type: application/json
Authorization: Bearer 54d0716f66f7d7ed73d60f5ad5b2712838eabe19a17d021ff8e42154f6670995
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54d0716f66f7d7ed73d60f5ad5b2712838eabe19a17d021ff8e42154f6670995"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/75
Content-Type: application/json
Authorization: Bearer f518a42efa9d1e77f902510be543dad2f3082d1c3706e674de7e7e3356783db8
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f518a42efa9d1e77f902510be543dad2f3082d1c3706e674de7e7e3356783db8"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/68/downvote
Content-Type: application/json
Authorization: Bearer 4710264f837ac96381b31be5a13921e1d3600614b6c401d632d057d470f3fd8a
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/68/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4710264f837ac96381b31be5a13921e1d3600614b6c401d632d057d470f3fd8a"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/72
Content-Type: application/json
Authorization: Bearer 3f2b33866f41ec6ae11d3e5ac4a70adec26b117e57b3f720fcf11f4ec4f6a263
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
    "id": 72,
    "obfuscated_id": "oqzxOzwzIgw",
    "author_id": 847,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:33.516Z",
    "created_at": "2016-10-14T12:02:33.516Z",
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
curl "api.goskive.com/v2/flashcards/72" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f2b33866f41ec6ae11d3e5ac4a70adec26b117e57b3f720fcf11f4ec4f6a263"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/report
Content-Type: application/json
Authorization: Bearer aa5928bd1b70377b18c61389d24f8829afc42a74093fadf92fc93c364398cd5b
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa5928bd1b70377b18c61389d24f8829afc42a74093fadf92fc93c364398cd5b"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/71/bookmark
Content-Type: application/json
Authorization: Bearer d810f84eb350e1a94512befde083292ea5d169b07aa1c4aee28efa2ac6dcb403
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/71/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d810f84eb350e1a94512befde083292ea5d169b07aa1c4aee28efa2ac6dcb403"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/73/upvote
Content-Type: application/json
Authorization: Bearer d67a736d284066ef0d0dca991eb6961d912afbeec0181af3b391538a2a23c108
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d67a736d284066ef0d0dca991eb6961d912afbeec0181af3b391538a2a23c108"
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
    "key": "cache/827dc88b3d9830e548ce5f58d3b40041.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMzowMTozM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS84MjdkYzg4YjNkOTgzMGU1NDhjZTVmNThkM2I0MDA0MS5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTIwMTMzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T120133Z",
    "x-amz-signature": "ba7f20582f849288befe588b0b3addf4b3fc6c8c2b6a5a4744ed523cd233e1a9"
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
Authorization: Bearer d703989b5c1f4a43833205b72d9739721799e1f25487a3f950818d4671e5d72e
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
	-H "Authorization: Bearer d703989b5c1f4a43833205b72d9739721799e1f25487a3f950818d4671e5d72e"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer c52ea9e9e7c443014dc033386cadae642b421a733abe6ac57336e7c5d4831422
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
	-H "Authorization: Bearer c52ea9e9e7c443014dc033386cadae642b421a733abe6ac57336e7c5d4831422"
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
{"password":{"reset_password_token":"YW9biz9r1PoVF4Z9Cser","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 916,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-14T12:02:38.429Z",
  "updated_at": "2016-10-14T12:02:38.598Z",
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
  "audit_id": 4663
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"YW9biz9r1PoVF4Z9Cser","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/54/comments
Content-Type: application/json
Authorization: Bearer b6b901b5e7176902874638610345b796b5aa3ee20b64185c80a1b2bfd74aaddf
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
    "id": 11,
    "author_id": 255,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:01:50.357Z",
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
curl "api.goskive.com/v2/questions/54/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6b901b5e7176902874638610345b796b5aa3ee20b64185c80a1b2bfd74aaddf"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/53/comments
Content-Type: application/json
Authorization: Bearer 11e9e9e5758a704c65f70e74883dd7dfba75dc56075d79cce0a1166f8cd0e38f
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
    "id": 10,
    "author_id": 252,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:01:49.883Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 2,
      "user_id": 252,
      "feedbackable_id": 53,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:01:49.879Z",
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
curl "api.goskive.com/v2/questions/53/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11e9e9e5758a704c65f70e74883dd7dfba75dc56075d79cce0a1166f8cd0e38f"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/51/comments
Content-Type: application/json
Authorization: Bearer b645a10ac8e7624f09e4addc65f994983df5ab949471d8f6702232c25b4b790d
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
      "author_id": 247,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:49.189Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 248,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:49.208Z",
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
curl "api.goskive.com/v2/questions/51/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b645a10ac8e7624f09e4addc65f994983df5ab949471d8f6702232c25b4b790d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/55/comments
Content-Type: application/json
Authorization: Bearer 69be723bd4ae728a1e998240ba199f444adcaaaa64f7a39f365bac65f137a80f
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
curl "api.goskive.com/v2/questions/55/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69be723bd4ae728a1e998240ba199f444adcaaaa64f7a39f365bac65f137a80f"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/65/feedbacks
Content-Type: application/json
Authorization: Bearer 44e1dfc617bad0a9206b34fd0c07ddab06dc34e93143ca277a838a781e8977fe
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
    "id": 10,
    "user_id": 448,
    "feedbackable_id": 65,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:02:02.255Z",
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
curl "api.goskive.com/v2/questions/65/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44e1dfc617bad0a9206b34fd0c07ddab06dc34e93143ca277a838a781e8977fe"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/58/feedbacks
Content-Type: application/json
Authorization: Bearer 2b21b5a2b89ecb5d5e61f2214d090e28476d032f1a61016b8f54811e1f80aeaa
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
      "id": 4,
      "user_id": 419,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:01:59.665Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 418,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:01:59.653Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/58/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b21b5a2b89ecb5d5e61f2214d090e28476d032f1a61016b8f54811e1f80aeaa"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/4/votes
Content-Type: application/json
Authorization: Bearer 1f5c18007580a353bbe4bb2028e9db4aea53dc1a42f7035315439464fd93e0e0
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
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 4,
      "user_id": 18
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 4,
      "user_id": 17
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 4,
      "user_id": 16
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/4/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f5c18007580a353bbe4bb2028e9db4aea53dc1a42f7035315439464fd93e0e0"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/92/republish
Content-Type: application/json
Authorization: Bearer 7f3e08a38e189bfdd99c330ddf7df02cb1f068bf9320317332aa2637f167238f
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
curl "api.goskive.com/v2/questions/92/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f3e08a38e189bfdd99c330ddf7df02cb1f068bf9320317332aa2637f167238f"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/88/bookmark
Content-Type: application/json
Authorization: Bearer 673620e14d2b9669a52437e8ce1cf270c7063264e62f2a2316db2b25f1e1f60d
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/88/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 673620e14d2b9669a52437e8ce1cf270c7063264e62f2a2316db2b25f1e1f60d"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/112
Content-Type: application/json
Authorization: Bearer 901e450e26f1758c9fdaaf8269d5cc4fa20f7e81619763b1162e995796fd61fa
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/112" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 901e450e26f1758c9fdaaf8269d5cc4fa20f7e81619763b1162e995796fd61fa"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/110/downvote
Content-Type: application/json
Authorization: Bearer 396ab4f914f7b7ff45b001f0cfcd351c871b6f86e2413a3e69eea616f2b0a9b5
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 396ab4f914f7b7ff45b001f0cfcd351c871b6f86e2413a3e69eea616f2b0a9b5"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/89
Content-Type: application/json
Authorization: Bearer dbfbe4773c7c7b0d46681e166ae1b1566d943b2e64a2c72435e0e514eab2ad23
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
    "id": 89,
    "obfuscated_id": "5eRHrGHLqZk",
    "author_id": 654,
    "chapter_id": 120,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:16.008Z",
    "created_at": "2016-10-14T12:02:15.888Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/89" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbfbe4773c7c7b0d46681e166ae1b1566d943b2e64a2c72435e0e514eab2ad23"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/90/report
Content-Type: application/json
Authorization: Bearer 191e59ee9dd364d772d665404c2a1eb2a91326bf0c7512996b4e3f1a3df40c27
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/90/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 191e59ee9dd364d772d665404c2a1eb2a91326bf0c7512996b4e3f1a3df40c27"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/109/bookmark
Content-Type: application/json
Authorization: Bearer f189d46cd76c7805d0b4e7a56f41344b25914f8c084b6f09746b28e06fef243a
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f189d46cd76c7805d0b4e7a56f41344b25914f8c084b6f09746b28e06fef243a"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/93
Content-Type: application/json
Authorization: Bearer 2c80e7a8833d0632544e5bbc2042a566e49fb2c38aa072dde801fa7f3d981b5d
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":93,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T12:02:17.489Z","updated_at":"2016-10-14T12:02:17.609Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":124,"author_id":666,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 666,
    "chapter_id": 124,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:02:17.722Z",
    "created_at": "2016-10-14T12:02:17.489Z",
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
    "question": "{\"id\"=>93, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-14T12:02:17.489Z\", \"updated_at\"=>\"2016-10-14T12:02:17.609Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>124, \"author_id\"=>666, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 185,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 186,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 187,
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
curl "api.goskive.com/v2/questions/93" -d '{"question":{"question":{"id":93,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T12:02:17.489Z","updated_at":"2016-10-14T12:02:17.609Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":124,"author_id":666,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c80e7a8833d0632544e5bbc2042a566e49fb2c38aa072dde801fa7f3d981b5d"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/111/upvote
Content-Type: application/json
Authorization: Bearer 8e66b77b8efa7226e1723e877bf3c459bf2afd4c19ae287709d242c90b94c1ec
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e66b77b8efa7226e1723e877bf3c459bf2afd4c19ae287709d242c90b94c1ec"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 00a628a140d23a2dc5f833d2eabbafb945a4fa627d7b74a415d94e99519ced21
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
      "creator_id": 242,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "topic_id": 80,
      "discipline_id": 80,
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
      "updated_at": "2016-10-14T12:01:48.734Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00a628a140d23a2dc5f833d2eabbafb945a4fa627d7b74a415d94e99519ced21"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 60ff2d67d45ee728be35f89c4d0263d3255643edf65fa3648268904ac37df88e
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
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-72",
      "html_url": "https://goskive.com/university/uni-72",
      "slug": "uni-72",
      "name": "National School of Pizza",
      "short_name": "Uni 72",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/eb17af409208ca654f585bc4d7642861365b7674.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a2acc3b39b369b62935ab17303fbc0d252cb6b91.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:01:48.504Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-71",
      "html_url": "https://goskive.com/university/uni-71",
      "slug": "uni-71",
      "name": "National School of Pastry",
      "short_name": "Uni 71",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6815e8d7e9cbcb148f1da5faa12acfad6db49257.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b48f9d0cebdb7956f7b23dc7411c7261eca3d96a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:01:48.461Z",
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
	-H "Authorization: Bearer 60ff2d67d45ee728be35f89c4d0263d3255643edf65fa3648268904ac37df88e"
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
      "name": "Cross-platform composite algorithm",
      "name_translations": {
        "en": "Cross-platform composite algorithm"
      },
      "discipline_id": 38
    },
    {
      "id": 39,
      "name": "Expanded eco-centric intranet",
      "name_translations": {
        "en": "Expanded eco-centric intranet"
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
GET /v2/topics/40
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
    "id": 40,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 40
  }
}
```



```shell
curl "api.goskive.com/v2/topics/40" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer c0edad15113d86ba4489c7e25ea9007986cdc4a13c182e00dcc212dbb0ba10a1
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
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-240",
      "html_url": "https://goskive.com/university/uni-240",
      "slug": "uni-240",
      "name": "University 177",
      "short_name": "Uni 240",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cff67873362ee3a29d561042c7facb3260161ded.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/92aec2a9b06ccfdaec1185e21c9f1b64ee851392.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:02:30.735Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-238",
      "html_url": "https://goskive.com/university/uni-238",
      "slug": "uni-238",
      "name": "University 175",
      "short_name": "Uni 238",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cc8c1bd4bd1d61da3756102e429ffda134c94210.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8bcd38c77c90580d88b3e155e39aad65f49060cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:02:30.702Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-239",
      "html_url": "https://goskive.com/university/uni-239",
      "slug": "uni-239",
      "name": "University 176",
      "short_name": "Uni 239",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/48a2378f71bf32b4659c203b40668d09183285f6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6167303c927184e4d13783875ec6336736353ae3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:02:30.719Z",
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
	-H "Authorization: Bearer c0edad15113d86ba4489c7e25ea9007986cdc4a13c182e00dcc212dbb0ba10a1"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 8ee13e756dc2e2633651c9ad0d82773e63ce68ab5297d1c0c577fd96ed8844fd
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
    "id": 238,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fa483c5edea94000bf08c410dcc2c1e508040ead.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/893681a5b52f73e766cb781feb727bd6b6546942.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-14T12:02:30.559Z",
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
	-H "Authorization: Bearer 8ee13e756dc2e2633651c9ad0d82773e63ce68ab5297d1c0c577fd96ed8844fd"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5a6627d2b19572dd94ed2a834fee997394b62b58833be735b385d25d5b4c8df9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":280,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 920,
    "id": 268,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 275,
    "additional_university_ids": [

    ],
    "topic_id": 280,
    "discipline_id": 281,
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
    "chapters_updated_at": "2016-10-14T12:02:38.641Z",
    "updated_at": "2016-10-14T12:02:38.791Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 189,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-14T12:02:38.745Z",
        "course_id": 268,
        "author_id": 920,
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
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-14T12:02:38.763Z",
        "course_id": 268,
        "author_id": 920,
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
        "id": 191,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-14T12:02:38.781Z",
        "course_id": 268,
        "author_id": 920,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":280,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a6627d2b19572dd94ed2a834fee997394b62b58833be735b385d25d5b4c8df9"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b263f95e8a994573d4eb5d5dda33c1e12b6506abbd6d16399781c7d608236656
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":281,"published":false}}
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
    "creator_id": 921,
    "id": 269,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 276,
    "additional_university_ids": [

    ],
    "topic_id": 281,
    "discipline_id": 282,
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
    "updated_at": "2016-10-14T12:02:38.982Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":281,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b263f95e8a994573d4eb5d5dda33c1e12b6506abbd6d16399781c7d608236656"
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
      "creator_id": 939,
      "id": 286,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 284,
      "additional_university_ids": [

      ],
      "topic_id": 298,
      "discipline_id": 299,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
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
      "updated_at": "2016-10-14T12:02:40.706Z",
      "shortname": "fu-course-214"
    },
    {
      "creator_id": 939,
      "id": 287,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 284,
      "additional_university_ids": [

      ],
      "topic_id": 299,
      "discipline_id": 300,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
      "chapters_updated_at": "2016-10-14T12:02:41.009Z",
      "updated_at": "2016-10-14T12:02:41.016Z",
      "shortname": "fu-course-215"
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
Authorization: Bearer 13109bbcacd3b395c9f0cf3455ebb314e2159a59226831075ac94792c4b224d8
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
      "creator_id": 956,
      "id": 302,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-230",
      "html_url": "https://goskive.com/course/fu-course-230",
      "slug": "fu-course-230",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "topic_id": 314,
      "discipline_id": 315,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 230",
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
      "updated_at": "2016-10-14T12:02:42.469Z",
      "shortname": "fu-course-230"
    },
    {
      "creator_id": 956,
      "id": 303,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-231",
      "html_url": "https://goskive.com/course/fu-course-231",
      "slug": "fu-course-231",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "topic_id": 315,
      "discipline_id": 316,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 231",
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
      "chapters_updated_at": "2016-10-14T12:02:42.774Z",
      "updated_at": "2016-10-14T12:02:42.781Z",
      "shortname": "fu-course-231"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13109bbcacd3b395c9f0cf3455ebb314e2159a59226831075ac94792c4b224d8"
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
      "creator_id": 944,
      "id": 290,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-218",
      "html_url": "https://goskive.com/course/fu-course-218",
      "slug": "fu-course-218",
      "university_id": 286,
      "additional_university_ids": [

      ],
      "topic_id": 302,
      "discipline_id": 303,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 218",
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
      "updated_at": "2016-10-14T12:02:41.246Z",
      "shortname": "fu-course-218"
    },
    {
      "creator_id": 944,
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-219",
      "html_url": "https://goskive.com/course/fu-course-219",
      "slug": "fu-course-219",
      "university_id": 286,
      "additional_university_ids": [

      ],
      "topic_id": 303,
      "discipline_id": 304,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 219",
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
      "updated_at": "2016-10-14T12:02:41.292Z",
      "shortname": "fu-course-219"
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
Authorization: Bearer a4b0e3f7b04fd60a1f0a35ee71847961d7b246030382b41cc7771471d019f710
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
      "creator_id": 962,
      "id": 306,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-234",
      "html_url": "https://goskive.com/course/fu-course-234",
      "slug": "fu-course-234",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "topic_id": 318,
      "discipline_id": 319,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 234",
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
      "updated_at": "2016-10-14T12:02:43.025Z",
      "shortname": "fu-course-234"
    },
    {
      "creator_id": 962,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-235",
      "html_url": "https://goskive.com/course/fu-course-235",
      "slug": "fu-course-235",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "topic_id": 319,
      "discipline_id": 320,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 235",
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
      "updated_at": "2016-10-14T12:02:43.070Z",
      "shortname": "fu-course-235"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4b0e3f7b04fd60a1f0a35ee71847961d7b246030382b41cc7771471d019f710"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer fc00955de3bd2e08ec1414a8609f64d1dd1045edce007b93f7abe7401890dca8
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
  "id": 238,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-14T12:01:48.189Z",
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
	-H "Authorization: Bearer fc00955de3bd2e08ec1414a8609f64d1dd1045edce007b93f7abe7401890dca8"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/467
Content-Type: application/json
Authorization: Bearer 688a63e2ad38b05d7c18d04c012392b1904142f2c250935418888423c2b76f05
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
    "id": 467,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 153,
    "fields_of_study": [
      162,
      163
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-14T12:02:03.522Z",
    "updated_at": "2016-10-14T12:02:03.522Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/467" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 688a63e2ad38b05d7c18d04c012392b1904142f2c250935418888423c2b76f05"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/465
Content-Type: application/json
Authorization: Bearer adaff3de68da2c6ac91ff7de961caa8dba1613409786e243ee0aeeb978659f37
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
    "id": 465,
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
    "created_at": "2016-10-14T12:02:03.353Z",
    "updated_at": "2016-10-14T12:02:03.353Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/465" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adaff3de68da2c6ac91ff7de961caa8dba1613409786e243ee0aeeb978659f37"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/1
Content-Type: application/json
Authorization: Bearer 8a6d65f47ba00b6e7f405aaee56c586db20b6d23fb170b2d9008650442078524
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a6d65f47ba00b6e7f405aaee56c586db20b6d23fb170b2d9008650442078524"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/3
Content-Type: application/json
Authorization: Bearer 3c5aeaaf81a827235f6181f13002a73253e30bd26a1685e6494f9227be62876b
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
    "id": 3,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 3,
    "user_id": 9
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c5aeaaf81a827235f6181f13002a73253e30bd26a1685e6494f9227be62876b"
```
