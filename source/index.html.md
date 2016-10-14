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
Authorization: Basic MzAzOWFiYWU0NDY5OTQ2MDJhZDdhOTgzYWFhMDllZGQzNzIyZTA4Y2RjZmVi
OWYyMWQwNzI1MDY0Y2MwNThlMTo5YjNhM2NjNWQ1MzQyMzBjODIxYTg4Nzky
MzMwMDk4MGMyMDExNjcyYzhlMjEzZmNmMGM1MDQzYjhkODE5YjUx

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
	-u 3039abae446994602ad7a983aaa09edd3722e08cdcfeb9f21d0725064cc058e1:9b3a3cc5d534230c821a887923300980c2011672c8e213fcf0c5043b8d819b51
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2786f84f2fda6d2b29dbb7ac3fe6ed30eb4468e48dd1fcecd360a7a8aabbf678","client_secret":"c81bef348d725adc91d87577cf3f95934cd8ab5206e8f4c95b4ac684661788f0"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2786f84f2fda6d2b29dbb7ac3fe6ed30eb4468e48dd1fcecd360a7a8aabbf678","client_secret":"c81bef348d725adc91d87577cf3f95934cd8ab5206e8f4c95b4ac684661788f0"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZTczM2IzNTI5ZDQyZWNkNzJlMTM3Y2YyMTgwMTA2ZDFjNGVlYjM1ZjEwZGMx
OWJiZTNhYmEwNTQ3OGMzODg1YzpmMmNiZWU3OThiYzY5M2Q0MTlkNzI3OTM3
MjZhOTBiNDlhZmYyMmI5MTI0ZmQ3ZjNmN2YwYTNmMzQxOTFhZDY3

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
  "access_token": "2f5dc75d3c3cf6ae7c659fcd66a5bdf53d69a64c2b0ed55de333544610dac879",
  "token_type": "bearer",
  "created_at": 1476447039
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u e733b3529d42ecd72e137cf2180106d1c4eeb35f10dc19bbe3aba05478c3885c:f2cbee798bc693d419d72793726a90b49aff22b9124fd7f3f7f0a3f34191ad67
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"eb88c65d2b8357b41e99dccee9e99bf166316aca1fe5713a05c28bc9a2a9edad","client_secret":"2d2d4dd20a4a1a87306b29928fa26518a07630adc246426f2c814ba1c96ea757"}
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
  "access_token": "f1a4e17b1b163cb9f75e0f8e5d5250fc5d834c76cc0fd4bee425627484603aae",
  "token_type": "bearer",
  "created_at": 1476447039
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"eb88c65d2b8357b41e99dccee9e99bf166316aca1fe5713a05c28bc9a2a9edad","client_secret":"2d2d4dd20a4a1a87306b29928fa26518a07630adc246426f2c814ba1c96ea757"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"bd53530bf288a7483c0c0d4d36ebe6ac68784c470588eb58efbbe8a0a31cf637","client_secret":"59eb1278fedf4807bb3f76f4364257f2ffa5447996188ec13ae22759ac2d9384"}
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
  "access_token": "5be9c704816eba030832589ae281f8bd37acd87e262998c69f5dd304e7eaf632",
  "token_type": "bearer",
  "created_at": 1476447039
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"bd53530bf288a7483c0c0d4d36ebe6ac68784c470588eb58efbbe8a0a31cf637","client_secret":"59eb1278fedf4807bb3f76f4364257f2ffa5447996188ec13ae22759ac2d9384"}' -X POST \
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
Authorization: Bearer 1cf234ec6bddd36326aa0b15024b6e43e9a61872a5cf0a997ccbd4c3dfc4de5e
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
    "company_id": 31,
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
	-H "Authorization: Bearer 1cf234ec6bddd36326aa0b15024b6e43e9a61872a5cf0a997ccbd4c3dfc4de5e"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/47/flashcards
Content-Type: application/json
Authorization: Bearer 85e3b1a0b0ea954b61433d50cb2b215e0a1e8b38a4a619e14c65dbb0072197db
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":47,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 43,
    "obfuscated_id": "uapnSdBCag8",
    "author_id": 278,
    "chapter_id": 47,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:10:53.213Z",
    "created_at": "2016-10-14T12:10:53.213Z",
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
curl "api.goskive.com/v2/chapters/47/flashcards" -d '{"flashcard":{"chapter_id":47,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85e3b1a0b0ea954b61433d50cb2b215e0a1e8b38a4a619e14c65dbb0072197db"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/45/flashcards
Content-Type: application/json
Authorization: Bearer d05ec19cd20e42f59861b5ef30ab93df368ae6d5890d8a9f9276417080e9d074
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 270,
      "chapter_id": 45,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:10:52.731Z",
      "created_at": "2016-10-14T12:10:52.731Z",
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
      "author_id": 270,
      "chapter_id": 45,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:10:52.770Z",
      "created_at": "2016-10-14T12:10:52.770Z",
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 270,
      "chapter_id": 45,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:10:52.810Z",
      "created_at": "2016-10-14T12:10:52.810Z",
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
curl "api.goskive.com/v2/chapters/45/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d05ec19cd20e42f59861b5ef30ab93df368ae6d5890d8a9f9276417080e9d074"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/112/questions
Content-Type: application/json
Authorization: Bearer 9b3be8fcc49198a212b554d244c2f998133b77c5811ecf458d048dbd88238179
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":112,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 96,
    "obfuscated_id": "SEtQvXxfwHo",
    "author_id": 697,
    "chapter_id": 112,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:29.102Z",
    "created_at": "2016-10-14T12:11:29.102Z",
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
        "id": 191,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 192,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 193,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 194,
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
curl "api.goskive.com/v2/chapters/112/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":112,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b3be8fcc49198a212b554d244c2f998133b77c5811ecf458d048dbd88238179"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/111/questions
Content-Type: application/json
Authorization: Bearer 70295bae8c97184ae607f6f51ba34e5ec94b252b3866d19c651b0c6c6c99bc35
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":111,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 95,
    "obfuscated_id": "uTOhBSQK4CI",
    "author_id": 694,
    "chapter_id": 111,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:28.722Z",
    "created_at": "2016-10-14T12:11:28.722Z",
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
        "id": 189,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 190,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/111/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":111,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70295bae8c97184ae607f6f51ba34e5ec94b252b3866d19c651b0c6c6c99bc35"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/114/questions
Content-Type: application/json
Authorization: Bearer 294d9879dc53bd5570bf256e68a23edf37eded3abd24673f15ceee9f8c3e31c2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":114,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 98,
    "obfuscated_id": "icApzX10lRE",
    "author_id": 703,
    "chapter_id": 114,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:30.062Z",
    "created_at": "2016-10-14T12:11:30.062Z",
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
        "id": 198,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 199,
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
curl "api.goskive.com/v2/chapters/114/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":114,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 294d9879dc53bd5570bf256e68a23edf37eded3abd24673f15ceee9f8c3e31c2"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/113/questions
Content-Type: application/json
Authorization: Bearer 08fb6cc01ae816200615829632deaf16e373b8edf5ec546201b82a44988f8696
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":113,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 97,
    "obfuscated_id": "qdTHUgSdSV8",
    "author_id": 700,
    "chapter_id": 113,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:29.631Z",
    "created_at": "2016-10-14T12:11:29.631Z",
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
        "id": 195,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 196,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 197,
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
curl "api.goskive.com/v2/chapters/113/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":113,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08fb6cc01ae816200615829632deaf16e373b8edf5ec546201b82a44988f8696"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/110/questions
Content-Type: application/json
Authorization: Bearer 4e1abbe33f89a784754fff0fac15db6c0e8e28f61ee2d766174be4b13020e8aa
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
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 688,
      "chapter_id": 110,
      "position": 92,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:11:28.034Z",
      "created_at": "2016-10-14T12:11:27.910Z",
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
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 689,
      "chapter_id": 110,
      "position": 93,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:11:28.238Z",
      "created_at": "2016-10-14T12:11:28.113Z",
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
        }
      ]
    },
    {
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 690,
      "chapter_id": 110,
      "position": 94,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:11:28.445Z",
      "created_at": "2016-10-14T12:11:28.317Z",
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
```



```shell
curl "api.goskive.com/v2/chapters/110/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e1abbe33f89a784754fff0fac15db6c0e8e28f61ee2d766174be4b13020e8aa"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/21
Content-Type: application/json
Authorization: Bearer 6cdc42f3c5507e275b5504db251dca522731c60fcc1e13885d5e1c9ee51b7c0d
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
curl "api.goskive.com/v2/chapters/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cdc42f3c5507e275b5504db251dca522731c60fcc1e13885d5e1c9ee51b7c0d"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/22
Content-Type: application/json
Authorization: Bearer 4ce2acacab723500d6b10f9a28057343425a0a426e9d454729fe8df0cf9c7dd2
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
curl "api.goskive.com/v2/chapters/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ce2acacab723500d6b10f9a28057343425a0a426e9d454729fe8df0cf9c7dd2"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/19
Content-Type: application/json
Authorization: Bearer e3a6f0485f1fb5f7c8c7c4a9d53673072553a9a77eac8d8c6d0815ca3d95dfbe
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
curl "api.goskive.com/v2/chapters/19" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3a6f0485f1fb5f7c8c7c4a9d53673072553a9a77eac8d8c6d0815ca3d95dfbe"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/20
Content-Type: application/json
Authorization: Bearer 6b28c7782c0291407b4ac1ffd98fdc9ed874d1a429a076c18421a7c9ab352999
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b28c7782c0291407b4ac1ffd98fdc9ed874d1a429a076c18421a7c9ab352999"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/16
Content-Type: application/json
Authorization: Bearer de35ec7a8fa699de97740dba33dfba97846042d0f1429de56d8abb40bee9b528
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
    "id": 16,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T12:10:34.664Z",
    "course_id": 56,
    "author_id": 105,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-14T12:10:34.101Z",
    "questions_updated_at": "2016-10-14T12:10:34.101Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 109,
        "chapter_id": 16,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:34.646Z",
        "created_at": "2016-10-14T12:10:34.646Z",
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
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 107,
        "chapter_id": 16,
        "position": 15,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:34.534Z",
        "created_at": "2016-10-14T12:10:34.403Z",
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
            "id": 29,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 30,
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
curl "api.goskive.com/v2/chapters/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de35ec7a8fa699de97740dba33dfba97846042d0f1429de56d8abb40bee9b528"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/18
Content-Type: application/json
Authorization: Bearer df37da3e595cf3a1b28b5820faeddf69e88e6efb1f22f22f63091db16153f11b
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
    "id": 18,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T12:10:35.060Z",
    "course_id": 58,
    "author_id": 115,
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
curl "api.goskive.com/v2/chapters/18" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df37da3e595cf3a1b28b5820faeddf69e88e6efb1f22f22f63091db16153f11b"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/59/replies
Content-Type: application/json
Authorization: Bearer 9f401000b7f52acce63b209d185569b6a08cbbf22e4d11d00122dd121cfa8ffb
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
    "author_id": 964,
    "reply_to_id": 59,
    "created_at": "2016-10-14T12:11:51.769Z",
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
	-H "Authorization: Bearer 9f401000b7f52acce63b209d185569b6a08cbbf22e4d11d00122dd121cfa8ffb"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer ee7c44f90fac4632bb6e16b485218505492048ab3d462aeab2f7a53433426df6
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
	-H "Authorization: Bearer ee7c44f90fac4632bb6e16b485218505492048ab3d462aeab2f7a53433426df6"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer 021c0fc532ac86ff726db87815a666a7cf061b53ac06ffc8a4ce7af853adfb20
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
curl "api.goskive.com/v2/comments/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 021c0fc532ac86ff726db87815a666a7cf061b53ac06ffc8a4ce7af853adfb20"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/57/republish
Content-Type: application/json
Authorization: Bearer 57af912a83dcc8b979e938df878890a1e3786e776db820f58eef0870c1290c60
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
curl "api.goskive.com/v2/comments/57/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57af912a83dcc8b979e938df878890a1e3786e776db820f58eef0870c1290c60"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer 285488789bfcc14f8fd46b21057d981ada0b31786d8b310e5b11423f3f093403
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 285488789bfcc14f8fd46b21057d981ada0b31786d8b310e5b11423f3f093403"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/17/report
Content-Type: application/json
Authorization: Bearer cc416ea06677644f5b74eec2ea43da5d9f492923913c78d33dda4866b88e805e
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc416ea06677644f5b74eec2ea43da5d9f492923913c78d33dda4866b88e805e"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/9
Content-Type: application/json
Authorization: Bearer 792342551b5467e8311879019cf7be45f38dce60c9f7cddde5de07460e79b7f8
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
    "updated_at": "2016-10-14T12:10:51.610Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 792342551b5467e8311879019cf7be45f38dce60c9f7cddde5de07460e79b7f8"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer e8c17f69ef93ba9e961e8a0762bc0c604cf6bfad24c68686d97c2b2ab74f4669
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
      "updated_at": "2016-10-14T12:10:51.736Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T12:10:51.741Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T12:10:51.745Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8c17f69ef93ba9e961e8a0762bc0c604cf6bfad24c68686d97c2b2ab74f4669"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer ab117ad02f31c7e0447a57eb0a51ab38e2efb42288641c23541857e43fbdee8b
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
curl "api.goskive.com/v2/companies/27/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab117ad02f31c7e0447a57eb0a51ab38e2efb42288641c23541857e43fbdee8b"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 7ada9533fc7b8f755072c028d3e705f9b3d23cd2c5903a4b66f2da48acbb364b
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
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ada9533fc7b8f755072c028d3e705f9b3d23cd2c5903a4b66f2da48acbb364b"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer c9663339115c2c26dc2bf45001d196765f67555d0d6f012c7d782c32e36ed30d
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
      "company_id": 22,
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
	-H "Authorization: Bearer c9663339115c2c26dc2bf45001d196765f67555d0d6f012c7d782c32e36ed30d"
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
Authorization: Bearer 6221c288aabc48c06fe0eb98a76b92db0392887f9ebd0a475e27637a19747265
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
	-H "Authorization: Bearer 6221c288aabc48c06fe0eb98a76b92db0392887f9ebd0a475e27637a19747265"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 834c4ee16c2217428c5d6775a2ab8d0f29821fae11372299cddac10d14ce44cd
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
    "id": 136,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T12:11:33.329Z",
    "course_id": 241,
    "author_id": 754,
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
	-H "Authorization: Bearer 834c4ee16c2217428c5d6775a2ab8d0f29821fae11372299cddac10d14ce44cd"
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
      "id": 118,
      "title": "Clever Chapter Title 97",
      "position": 1,
      "updated_at": "2016-10-14T12:11:31.071Z",
      "course_id": 232,
      "author_id": 715,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 119,
      "title": "Clever Chapter Title 98",
      "position": 2,
      "updated_at": "2016-10-14T12:11:31.097Z",
      "course_id": 232,
      "author_id": 716,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 120,
      "title": "Clever Chapter Title 99",
      "position": 3,
      "updated_at": "2016-10-14T12:11:31.364Z",
      "course_id": 232,
      "author_id": 717,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T12:11:30.961Z",
      "questions_updated_at": "2016-10-14T12:11:30.961Z",
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
Authorization: Bearer 30a394e16b4e5e2727a5e77ca717a89afd0615f95b34374bd333495feb30bab6
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
      "title": "Clever Chapter Title 109",
      "position": 1,
      "updated_at": "2016-10-14T12:11:32.515Z",
      "course_id": 238,
      "author_id": 740,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 131,
      "title": "Clever Chapter Title 110",
      "position": 2,
      "updated_at": "2016-10-14T12:11:32.541Z",
      "course_id": 238,
      "author_id": 741,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 111",
      "position": 3,
      "updated_at": "2016-10-14T12:11:32.804Z",
      "course_id": 238,
      "author_id": 742,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T12:11:32.435Z",
      "questions_updated_at": "2016-10-14T12:11:32.435Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30a394e16b4e5e2727a5e77ca717a89afd0615f95b34374bd333495feb30bab6"
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
      "id": 121,
      "title": "Clever Chapter Title 100",
      "position": 1,
      "updated_at": "2016-10-14T12:11:31.575Z",
      "course_id": 234,
      "author_id": 722,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 122,
      "title": "Clever Chapter Title 101",
      "position": 2,
      "updated_at": "2016-10-14T12:11:31.602Z",
      "course_id": 234,
      "author_id": 723,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 123,
      "title": "Clever Chapter Title 102",
      "position": 3,
      "updated_at": "2016-10-14T12:11:31.627Z",
      "course_id": 234,
      "author_id": 724,
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
Authorization: Bearer 369757488acb28281f5f460d20b1a196fad52067fdb9ba520bf88c39537e2eb7
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
      "title": "Clever Chapter Title 112",
      "position": 1,
      "updated_at": "2016-10-14T12:11:32.970Z",
      "course_id": 239,
      "author_id": 747,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 134,
      "title": "Clever Chapter Title 113",
      "position": 2,
      "updated_at": "2016-10-14T12:11:32.997Z",
      "course_id": 239,
      "author_id": 748,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 135,
      "title": "Clever Chapter Title 114",
      "position": 3,
      "updated_at": "2016-10-14T12:11:33.024Z",
      "course_id": 239,
      "author_id": 749,
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
	-H "Authorization: Bearer 369757488acb28281f5f460d20b1a196fad52067fdb9ba520bf88c39537e2eb7"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 27a1f3a6a241141bbf87770706ea70500576d0d44efb2d9680743aa974dbe6dd
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
    "course_id": 146,
    "user_id": 427,
    "updated_at": "2016-10-14T12:11:04.903Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27a1f3a6a241141bbf87770706ea70500576d0d44efb2d9680743aa974dbe6dd"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 55f114432d505dd84d9134ba34acf606a4f93117bcbaafd5945e5850ac6efae3
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
      "course_id": 144,
      "user_id": 421,
      "updated_at": "2016-10-14T12:11:04.570Z"
    },
    {
      "id": 5,
      "course_id": 144,
      "user_id": 422,
      "updated_at": "2016-10-14T12:11:04.586Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55f114432d505dd84d9134ba34acf606a4f93117bcbaafd5945e5850ac6efae3"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/54/files
Content-Type: application/json
Authorization: Bearer 621a1dc74c017e18a385aa206d1ccd292e16a3b197d6a6aaa2d7f5fb6947f0aa
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
      "id": 2,
      "uploader": {
        "id": 93,
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
        "created_at": "2016-10-14T12:10:33.308Z",
        "updated_at": "2016-10-14T12:10:33.308Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:10:33.316Z",
      "updated_at": "2016-10-14T12:10:33.316Z",
      "course_id": 54,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 94,
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
        "created_at": "2016-10-14T12:10:33.324Z",
        "updated_at": "2016-10-14T12:10:33.324Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:10:33.331Z",
      "updated_at": "2016-10-14T12:10:33.331Z",
      "course_id": 54,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
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
        "created_at": "2016-10-14T12:10:33.339Z",
        "updated_at": "2016-10-14T12:10:33.339Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T12:10:33.346Z",
      "updated_at": "2016-10-14T12:10:33.346Z",
      "course_id": 54,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/54/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 621a1dc74c017e18a385aa206d1ccd292e16a3b197d6a6aaa2d7f5fb6947f0aa"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/51/files
Content-Type: application/json
Authorization: Bearer 02fa04398f1980d2ae0fef088eba415d5c3bd4150370137865e91e58f2665a0c
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
    "id": 1,
    "uploader": {
      "id": 87,
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
      "created_at": "2016-10-14T12:10:32.913Z",
      "updated_at": "2016-10-14T12:10:32.913Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-14T12:10:32.973Z",
    "updated_at": "2016-10-14T12:10:32.973Z",
    "course_id": 51,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/51/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02fa04398f1980d2ae0fef088eba415d5c3bd4150370137865e91e58f2665a0c"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/52/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 444356d697bb4f70ba5ac5ab90ff77ed37c6ac72e413752059a0061cea4690e0
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
    "key": "cache/55e7aee417e663cf202078f71d34de72.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMzoxMDozM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS81NWU3YWVlNDE3ZTY2M2NmMjAyMDc4ZjcxZDM0ZGU3Mi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTIxMDMzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T121033Z",
    "x-amz-signature": "5c2d99207ebb52a3a3bda4b985dc4f89b8c686466aac70e58f3c126e3a3ef22e"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/52/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 444356d697bb4f70ba5ac5ab90ff77ed37c6ac72e413752059a0061cea4690e0"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 43da45b8e1185cadd92165832b0decf4e6ae9c0fdb6c1c317858f816d0c6bf54
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
	-H "Authorization: Bearer 43da45b8e1185cadd92165832b0decf4e6ae9c0fdb6c1c317858f816d0c6bf54"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2d526330ab89c4aed31a141032fddf474d5c883cdf4528c5c2b6753f2ec2cf23
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
	-H "Authorization: Bearer 2d526330ab89c4aed31a141032fddf474d5c883cdf4528c5c2b6753f2ec2cf23"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 90fe421aa5396738bd16fba5531812ca5c538a336e1cc6292c245c5b5a44257b
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
	-H "Authorization: Bearer 90fe421aa5396738bd16fba5531812ca5c538a336e1cc6292c245c5b5a44257b"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 52f714cc3a4bcf49d68dce14e911d98390e7c3e09a6a91d47b72cc721b1db89b
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
	-H "Authorization: Bearer 52f714cc3a4bcf49d68dce14e911d98390e7c3e09a6a91d47b72cc721b1db89b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d1409f406eb7b0e955dd5b6af690ab4f8b54369316eb852eb373d8fd4163e811
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
	-H "Authorization: Bearer d1409f406eb7b0e955dd5b6af690ab4f8b54369316eb852eb373d8fd4163e811"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 02b02565285eff60b03ec4b1178cee359138a75894c1746adf2b4b6c5da28f33
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
    "creator_id": 210,
    "id": 88,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 72,
    "additional_university_ids": [

    ],
    "topic_id": 93,
    "discipline_id": 93,
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
    "chapters_updated_at": "2016-10-14T12:10:42.848Z",
    "updated_at": "2016-10-14T12:10:44.345Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 33,
        "title": "Clever Chapter Title 21",
        "position": 1,
        "updated_at": "2016-10-14T12:10:44.295Z",
        "course_id": 88,
        "author_id": 210,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:10:42.848Z",
        "questions_updated_at": "2016-10-14T12:10:42.848Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 34,
        "title": "Clever Chapter Title 22",
        "position": 2,
        "updated_at": "2016-10-14T12:10:44.337Z",
        "course_id": 88,
        "author_id": 210,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:10:42.848Z",
        "questions_updated_at": "2016-10-14T12:10:42.848Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 211,
        "chapter_id": 33,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:44.132Z",
        "created_at": "2016-10-14T12:10:44.132Z",
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
        "author_id": 211,
        "chapter_id": 34,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:44.205Z",
        "created_at": "2016-10-14T12:10:44.205Z",
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
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 211,
        "chapter_id": 33,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:44.173Z",
        "created_at": "2016-10-14T12:10:44.173Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 211,
        "chapter_id": 34,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:44.245Z",
        "created_at": "2016-10-14T12:10:44.245Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 211,
        "chapter_id": 33,
        "position": 22,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:43.102Z",
        "created_at": "2016-10-14T12:10:42.980Z",
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
      },
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 211,
        "chapter_id": 33,
        "position": 23,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:43.284Z",
        "created_at": "2016-10-14T12:10:43.166Z",
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
        "author_id": 211,
        "chapter_id": 34,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:43.495Z",
        "created_at": "2016-10-14T12:10:43.372Z",
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
      },
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 211,
        "chapter_id": 34,
        "position": 25,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:43.676Z",
        "created_at": "2016-10-14T12:10:43.561Z",
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
            "id": 49,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 50,
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
	-H "Authorization: Bearer 02b02565285eff60b03ec4b1178cee359138a75894c1746adf2b4b6c5da28f33"
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
    "creator_id": 222,
    "id": 90,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 74,
    "additional_university_ids": [

    ],
    "topic_id": 95,
    "discipline_id": 95,
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
    "chapters_updated_at": "2016-10-14T12:10:46.068Z",
    "updated_at": "2016-10-14T12:10:47.557Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 37,
        "title": "Clever Chapter Title 25",
        "position": 1,
        "updated_at": "2016-10-14T12:10:47.507Z",
        "course_id": 90,
        "author_id": 222,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:10:46.068Z",
        "questions_updated_at": "2016-10-14T12:10:46.068Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 38,
        "title": "Clever Chapter Title 26",
        "position": 2,
        "updated_at": "2016-10-14T12:10:47.550Z",
        "course_id": 90,
        "author_id": 222,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T12:10:46.068Z",
        "questions_updated_at": "2016-10-14T12:10:46.068Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 222,
        "chapter_id": 37,
        "position": 34,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:46.301Z",
        "created_at": "2016-10-14T12:10:46.177Z",
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
            "id": 67,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 68,
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
        "author_id": 222,
        "chapter_id": 38,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:10:46.692Z",
        "created_at": "2016-10-14T12:10:46.569Z",
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
            "id": 71,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 72,
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
PUT /v2/courses/83/pin
Content-Type: application/json
Authorization: Bearer b8212218d77c9a41b09014a4d13a6658885a45c9f920e3dbc90a9df2a7651f63
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/83/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8212218d77c9a41b09014a4d13a6658885a45c9f920e3dbc90a9df2a7651f63"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/82/pin
Content-Type: application/json
Authorization: Bearer 6a675343ea343e55e99548399997f064863d13e2165ebd21b17f9ba899f6be17
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/82/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a675343ea343e55e99548399997f064863d13e2165ebd21b17f9ba899f6be17"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c4293e4b36b1ae2830e2bdff5eeda74298736fb0e190f04c5bce264faec79272
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
    "creator_id": 205,
    "id": 85,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 69,
    "additional_university_ids": [

    ],
    "topic_id": 90,
    "discipline_id": 90,
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
    "updated_at": "2016-10-14T12:10:42.558Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4293e4b36b1ae2830e2bdff5eeda74298736fb0e190f04c5bce264faec79272"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 2fb24ea60dd28302d77e340c6c15cca1cb11b44ff82232b336ab9ba0b460659f
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
    "id": 253,
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
    "created_at": "2016-10-14T12:10:50.893Z",
    "updated_at": "2016-10-14T12:10:50.893Z",
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
	-H "Authorization: Bearer 2fb24ea60dd28302d77e340c6c15cca1cb11b44ff82232b336ab9ba0b460659f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7f8f0521218cb80f3bfbe56f975efb8f3d8bd3b7ea30b897cb02a85132620dc6
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[106]}
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
    "id": 254,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      106
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:10:50.994Z",
    "updated_at": "2016-10-14T12:10:51.034Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[106]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f8f0521218cb80f3bfbe56f975efb8f3d8bd3b7ea30b897cb02a85132620dc6"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0bd347ece4498f1a7cdda468c878e4aa6b9ac7c6aa6ad648349513ee5e00dd16
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
    "id": 257,
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
    "created_at": "2016-10-14T12:10:51.216Z",
    "updated_at": "2016-10-14T12:10:51.216Z",
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
	-H "Authorization: Bearer 0bd347ece4498f1a7cdda468c878e4aa6b9ac7c6aa6ad648349513ee5e00dd16"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 59abe548bf11639c1ad3080c20b445632022e103b8677c4b437d2a00bd3fb550
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[107]}
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
    "id": 255,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      107
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:10:51.080Z",
    "updated_at": "2016-10-14T12:10:51.080Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[107]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59abe548bf11639c1ad3080c20b445632022e103b8677c4b437d2a00bd3fb550"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b4044b727628dd04f187a3f7e7aad36ac6807f700908e702604d98def76641ea
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

110
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
    "id": 258,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/d19f33cc9e3467809db789512379b9129393a173.jpg",
    "university_id": null,
    "fields_of_study": [
      110
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T12:10:51.320Z",
    "updated_at": "2016-10-14T12:10:51.580Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/62c4856e46364421ed02ba5f46b3445aa53ba536.jpg",
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

110
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b4044b727628dd04f187a3f7e7aad36ac6807f700908e702604d98def76641ea"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 8eddbc8859787a0ef8b764b29739c478cd5dda5b72abf8dc63e695a58f74ce5b
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
	-H "Authorization: Bearer 8eddbc8859787a0ef8b764b29739c478cd5dda5b72abf8dc63e695a58f74ce5b"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b3db139e5f2d01db470258f04f41ef77f4c489f6729631deabc527396a4aaba4
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
	-H "Authorization: Bearer b3db139e5f2d01db470258f04f41ef77f4c489f6729631deabc527396a4aaba4"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b6aa2e07e87b59ad8839cb54b2bdf1c942c09e67072b173556203d91314af32f
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
	-H "Authorization: Bearer b6aa2e07e87b59ad8839cb54b2bdf1c942c09e67072b173556203d91314af32f"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer ec7f27cc00ca1ae0df1d5c323114a77f1d58b98b1ff80992143318211e595dd8
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
      "creator_id": 192,
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-67",
      "html_url": "https://goskive.com/course/mit-course-67",
      "slug": "mit-course-67",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 85,
      "discipline_id": 85,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
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
      "updated_at": "2016-10-14T12:10:41.558Z",
      "shortname": "mit-course-67"
    },
    {
      "creator_id": 193,
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-68",
      "html_url": "https://goskive.com/course/mit-course-68",
      "slug": "mit-course-68",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 86,
      "discipline_id": 86,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
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
      "updated_at": "2016-10-14T12:10:41.651Z",
      "shortname": "mit-course-68"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec7f27cc00ca1ae0df1d5c323114a77f1d58b98b1ff80992143318211e595dd8"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a386cd54221500f4cca443dc565850dfe8f539fcb8ea4a5b8e0951b5084b4a2d
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
        "updated_at": "2016-10-14T12:11:30.523Z"
      },
      "created_at": "2016-10-14T12:11:30.527Z",
      "updated_at": "2016-10-14T12:11:30.527Z",
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
        "updated_at": "2016-10-14T12:11:30.535Z"
      },
      "created_at": "2016-10-14T12:11:30.538Z",
      "updated_at": "2016-10-14T12:11:30.538Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a386cd54221500f4cca443dc565850dfe8f539fcb8ea4a5b8e0951b5084b4a2d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer c940364b95435ae15f236811dcadd34b0eb763c12e092a68dd8cedcbb21694f3
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
        "updated_at": "2016-10-14T12:11:30.291Z"
      },
      "created_at": "2016-10-14T12:11:30.295Z",
      "updated_at": "2016-10-14T12:11:30.295Z",
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
        "updated_at": "2016-10-14T12:11:30.309Z"
      },
      "created_at": "2016-10-14T12:11:30.313Z",
      "updated_at": "2016-10-14T12:11:30.313Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c940364b95435ae15f236811dcadd34b0eb763c12e092a68dd8cedcbb21694f3"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 78e09b7c23b5a0e0b0f8e5625b7c30e8f422e4cd45c5ccfeb42706cd67021c44
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
      "id": 1,
      "created_at": "2016-10-14T12:10:25.402Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 1,
      "updated_at": "2016-10-14T12:10:25.524Z",
      "author_id": "6",
      "thread_subject_id": "2",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 2,
      "created_at": "2016-10-14T12:10:25.511Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-14T12:10:25.528Z",
      "author_id": "9",
      "thread_subject_id": "3",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 3,
      "created_at": "2016-10-14T12:10:25.949Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-14T12:10:25.949Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-10-14T12:10:26.332Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-14T12:10:26.332Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 5,
      "created_at": "2016-10-14T12:10:26.727Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-14T12:10:26.727Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 6,
      "created_at": "2016-10-14T12:10:27.039Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 5,
      "updated_at": "2016-10-14T12:10:27.039Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 7,
      "created_at": "2016-10-14T12:10:27.347Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 6,
      "updated_at": "2016-10-14T12:10:27.347Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-10-14T12:10:27.644Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 7,
      "updated_at": "2016-10-14T12:10:27.644Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78e09b7c23b5a0e0b0f8e5625b7c30e8f422e4cd45c5ccfeb42706cd67021c44"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/9
Content-Type: application/json
Authorization: Bearer 1655dae9db8a7e02a904c46b723a7a062ec5a86d99080d7ec893b25d0d1a065d
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-14T12:00:27.000Z"}}
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
    "id": 9,
    "created_at": "2016-10-14T12:10:27.859Z",
    "read_at": "2016-10-14T12:00:27.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 3,
    "updated_at": "2016-10-14T12:10:27.901Z",
    "author_id": "35",
    "thread_subject_id": "10",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/9" -d '{"notification":{"read_at":"2016-10-14T12:00:27.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1655dae9db8a7e02a904c46b723a7a062ec5a86d99080d7ec893b25d0d1a065d"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 335f39b9092f0ed3af1602e16f7bed91fcb0ecc678c0a98d082b7a2510e65496
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
      "course_id": 276,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T12:11:41.427Z",
      "course_published": true,
      "updated_at": "2016-10-14T12:11:41.419Z"
    },
    {
      "id": 6,
      "course_id": 277,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T12:11:41.520Z",
      "course_published": true,
      "updated_at": "2016-10-14T12:11:41.511Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 335f39b9092f0ed3af1602e16f7bed91fcb0ecc678c0a98d082b7a2510e65496"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 2dca5b57c4f904725b6d9d31e4e1f9a5e6b047aa39a9e337c4ebb377de40d435
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
    "id": 7,
    "course_id": 278,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T12:11:41.707Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:11:41.699Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dca5b57c4f904725b6d9d31e4e1f9a5e6b047aa39a9e337c4ebb377de40d435"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer abbc306ea56743453a5e24904649a5048870a248aa011f63e32a320bfd034da0
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
    "course_id": 275,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-14T12:11:41.313Z",
    "course_published": true,
    "updated_at": "2016-10-14T12:11:41.301Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abbc306ea56743453a5e24904649a5048870a248aa011f63e32a320bfd034da0"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 0b112c27ad6d21ee5234702f6e348ec25076af64fceb5694e9f89b77552d38d3
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
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 18,
      "user_id": 177
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 19,
      "user_id": 177
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 20,
      "user_id": 177
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 21,
      "user_id": 177
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b112c27ad6d21ee5234702f6e348ec25076af64fceb5694e9f89b77552d38d3"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/130
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
    "id": 130,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 130,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 130
      },
      {
        "id": 131,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 130
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/130" -X GET \
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
      "id": 131,
      "name": "Object-based methodical product",
      "name_translations": {
        "en": "Object-based methodical product"
      }
    },
    {
      "id": 132,
      "name": "Sharable systematic access",
      "name_translations": {
        "en": "Sharable systematic access"
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
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer 34489550742cf6d95ecb28aa38cf13b10aa69b811251fff3cc794335214f6162
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
    "id": 20,
    "user_id": 466,
    "feedbackable_id": 60,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-14T12:11:09.790Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34489550742cf6d95ecb28aa38cf13b10aa69b811251fff3cc794335214f6162"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer a6cf30628934759f0d8ba772031481edf71332a2b9a5ced016137c538f0ecca6
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
    "user_id": 481,
    "feedbackable_id": 63,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-14T12:11:10.906Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6cf30628934759f0d8ba772031481edf71332a2b9a5ced016137c538f0ecca6"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/45
Content-Type: application/json
Authorization: Bearer f47ba081d101a070b7ca01fc320b3bec1e9232f782426157ade1b656fda3a0ae
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
    "id": 45,
    "user_id": 577,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:11:17.886Z",
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
curl "api.goskive.com/v2/feedbacks/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f47ba081d101a070b7ca01fc320b3bec1e9232f782426157ade1b656fda3a0ae"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/close
Content-Type: application/json
Authorization: Bearer eb4f119eae9e0c7cca14497f35772484fcb0eec740321a77277a32dfef2aaa1e
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
curl "api.goskive.com/v2/feedbacks/19/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb4f119eae9e0c7cca14497f35772484fcb0eec740321a77277a32dfef2aaa1e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer ede858a6ee9ae0957bc1496c5b7750b71b2cd014c5d4e8ae2696ab86d51fe15c
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
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ede858a6ee9ae0957bc1496c5b7750b71b2cd014c5d4e8ae2696ab86d51fe15c"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 9fd722c9e8d38bda12622f50c3c19eec10fda7db6c6ea8e912cba3d69f1a70c0
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
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9fd722c9e8d38bda12622f50c3c19eec10fda7db6c6ea8e912cba3d69f1a70c0"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/46
Content-Type: application/json
Authorization: Bearer a3b3fe093cb68933ab42875ccbe2314514523da35721449c7ff7eb157d03710b
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
    "id": 46,
    "user_id": 582,
    "feedbackable_id": 67,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:11:18.185Z",
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
curl "api.goskive.com/v2/feedbacks/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3b3fe093cb68933ab42875ccbe2314514523da35721449c7ff7eb157d03710b"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer b4a4fcfdbb2a0255d52be94ce370ae1065f482f0cf9539387e34e8cfbcf96a1d
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
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Authorization: Bearer b4a4fcfdbb2a0255d52be94ce370ae1065f482f0cf9539387e34e8cfbcf96a1d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Authorization: Bearer 51647ee15f74f72a0e0f76757fdd48cad1372c1db7de724ccf8cc62296a33f23
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
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Authorization: Bearer 51647ee15f74f72a0e0f76757fdd48cad1372c1db7de724ccf8cc62296a33f23" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/9
Authorization: Bearer 874a896e146c9dfa5ad67c26206c56e4bfdd37eb25baced5e40b34761e631a0b
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/db2ee0110e0fa8d5e372298201c8d5c7.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T121038Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=45d40d16021a931b096bcf05af10b15885feeac60b35bdb10f3b58aaa1c6e47a"
  }
}
```



```shell
curl "api.goskive.com/v2/files/9" -X GET \
	-H "Authorization: Bearer 874a896e146c9dfa5ad67c26206c56e4bfdd37eb25baced5e40b34761e631a0b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Authorization: Bearer 26e7cb84f6c6b615961ad225c946ead7e89ec32a93f22a90d75e3a60c8eb91d7
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
    "id": 10,
    "uploader": {
      "id": 162,
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
      "created_at": "2016-10-14T12:10:38.631Z",
      "updated_at": "2016-10-14T12:10:38.631Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-14T12:10:38.705Z",
    "updated_at": "2016-10-14T12:10:38.705Z",
    "course_id": 74,
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
	-H "Authorization: Bearer 26e7cb84f6c6b615961ad225c946ead7e89ec32a93f22a90d75e3a60c8eb91d7" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/12/matched_courses?required_cu_count=2
Authorization: Bearer c803a583a8b9cb177e7c9003b43a16bb327e3e9292ebd0baec5596781f9e07ff
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
      "creator_id": 369,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "topic_id": 142,
      "discipline_id": 143,
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
      "chapters_updated_at": "2016-10-14T12:10:59.286Z",
      "updated_at": "2016-10-14T12:11:00.936Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 374,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-e26f0531-f120-47de-908d-ca749e3351bd",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-e26f0531-f120-47de-908d-ca749e3351bd",
      "slug": "mit-the-great-british-bake-off-e26f0531-f120-47de-908d-ca749e3351bd",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 143,
      "discipline_id": 144,
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
      "chapters_updated_at": "2016-10-14T12:10:59.286Z",
      "updated_at": "2016-10-14T12:11:01.489Z",
      "shortname": "mit-the-great-british-bake-off-e26f0531-f120-47de-908d-ca749e3351bd"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/12/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer c803a583a8b9cb177e7c9003b43a16bb327e3e9292ebd0baec5596781f9e07ff"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/8/preview
Authorization: Bearer 445e0e4e5ec6b14ab75d3bf51017b2d6cb11415c6c163874f22c32478a3c061c
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/f559e2dec19d68640650a3704affc3d1.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T121038Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=75ec687808ccc3f23b410f5c4ca9d3c7c7b2a547e3be09b6aff9f8650dafe199"
  }
}
```



```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Authorization: Bearer 445e0e4e5ec6b14ab75d3bf51017b2d6cb11415c6c163874f22c32478a3c061c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/11/report
Authorization: Bearer 5108abaf8ffcea43f83c20dff834a4abea834d39ede6080f40eeb0635c4f3684
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
curl "api.goskive.com/v2/files/11/report" -d '' -X PUT \
	-H "Authorization: Bearer 5108abaf8ffcea43f83c20dff834a4abea834d39ede6080f40eeb0635c4f3684" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer 0a872d2fbcc7afd28910c8c23fd2aab157d300f23d2bbd2347e5adb650b231b0
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
    "author_id": 137,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:10:37.410Z",
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
curl "api.goskive.com/v2/flashcards/11/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a872d2fbcc7afd28910c8c23fd2aab157d300f23d2bbd2347e5adb650b231b0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer 916f01ae8f3f1ab8b73c08a0a99c85cb720f3b692db0177bff3a3d2733e720c0
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
    "author_id": 131,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:10:36.506Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 131,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:10:36.501Z",
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
curl "api.goskive.com/v2/flashcards/9/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 916f01ae8f3f1ab8b73c08a0a99c85cb720f3b692db0177bff3a3d2733e720c0"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer bd68307824d982976cf6102c927382a27f2d32818a9830a9ccd8ed00f48f751d
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
      "author_id": 143,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:10:37.723Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 144,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:10:37.741Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd68307824d982976cf6102c927382a27f2d32818a9830a9ccd8ed00f48f751d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer b3b60bb5b3571fe61624102b6b876d1ccb94a87ff910c4b70fa0acad1fa454c1
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
curl "api.goskive.com/v2/flashcards/10/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3b60bb5b3571fe61624102b6b876d1ccb94a87ff910c4b70fa0acad1fa454c1"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/51/feedbacks
Content-Type: application/json
Authorization: Bearer 4d17693cdeec7ecf6f3cd04d5f06749721020f20023fc03eedb858aa136c0690
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
    "user_id": 315,
    "feedbackable_id": 51,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:10:55.349Z",
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
curl "api.goskive.com/v2/flashcards/51/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d17693cdeec7ecf6f3cd04d5f06749721020f20023fc03eedb858aa136c0690"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/49/feedbacks
Content-Type: application/json
Authorization: Bearer 8c0b3282a81ae5ce64f5edf0cdaf78cc37f010b7603426cadd317e9180a05d5e
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
      "user_id": 311,
      "feedbackable_id": 49,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:10:54.791Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 310,
      "feedbackable_id": 49,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:10:54.778Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/49/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c0b3282a81ae5ce64f5edf0cdaf78cc37f010b7603426cadd317e9180a05d5e"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/56/votes
Content-Type: application/json
Authorization: Bearer f80103c71c293c2ca12294f36da6dde87b84d48805a464d4f5f440ce95851215
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
      "votable_id": 56,
      "user_id": 405
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 404
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 403
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f80103c71c293c2ca12294f36da6dde87b84d48805a464d4f5f440ce95851215"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/94/republish
Content-Type: application/json
Authorization: Bearer e63064a63aff01be12937772e233941e136d7dad82636744d546fc94dc0afe99
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
curl "api.goskive.com/v2/flashcards/94/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e63064a63aff01be12937772e233941e136d7dad82636744d546fc94dc0afe99"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/92/bookmark
Content-Type: application/json
Authorization: Bearer 35914214d58ccdb63c9d9baa4316d201718b518efb8d51e458366c54f788b3f6
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/92/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35914214d58ccdb63c9d9baa4316d201718b518efb8d51e458366c54f788b3f6"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/75
Content-Type: application/json
Authorization: Bearer 7cc5f62b155df7f561d9c929877923ba4678a8e3771b3fb5d363034d37ad38ff
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
	-H "Authorization: Bearer 7cc5f62b155df7f561d9c929877923ba4678a8e3771b3fb5d363034d37ad38ff"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/73/downvote
Content-Type: application/json
Authorization: Bearer 0b58d7dde536e1742d6bab439435aa0a6e56c499578b45a80a351918581ce5b8
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b58d7dde536e1742d6bab439435aa0a6e56c499578b45a80a351918581ce5b8"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/72
Content-Type: application/json
Authorization: Bearer 55a21f978a42b351e75b0ef02a39dcf89f820335d8aec3b9a84ff5d1a572400c
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
    "author_id": 773,
    "chapter_id": 142,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:35.345Z",
    "created_at": "2016-10-14T12:11:35.345Z",
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
	-H "Authorization: Bearer 55a21f978a42b351e75b0ef02a39dcf89f820335d8aec3b9a84ff5d1a572400c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/76/report
Content-Type: application/json
Authorization: Bearer 9f44536c9751a25e51632b1e1a282166c8c2931dc05bef015a571c62c4eecf2e
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f44536c9751a25e51632b1e1a282166c8c2931dc05bef015a571c62c4eecf2e"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/74/bookmark
Content-Type: application/json
Authorization: Bearer 313b5f2194505a5fed24e5995247a615d1c40658c14320ada33a6903c76c541e
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 313b5f2194505a5fed24e5995247a615d1c40658c14320ada33a6903c76c541e"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/93/upvote
Content-Type: application/json
Authorization: Bearer 00eae7e4fd2c9b89893c387200d2d879ef20d1f0af864646a2c8af2d96bac8d0
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/93/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00eae7e4fd2c9b89893c387200d2d879ef20d1f0af864646a2c8af2d96bac8d0"
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
    "key": "cache/42db333ba8cf3d46d2707dafcb22003c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMzoxMTowNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS80MmRiMzMzYmE4Y2YzZDQ2ZDI3MDdkYWZjYjIyMDAzYy5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTIxMTA0WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T121104Z",
    "x-amz-signature": "a125bf810ac9c422249fef49c56f23e2ff6c5bf8cad29cf915ffc5f7018254aa"
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
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer d79d6e0c2bd028a8b3104f546930016e9cbaac351e51ebbbd7d1dc9026bfeddd
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
curl "api.goskive.com/v2/me/jobs/1/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d79d6e0c2bd028a8b3104f546930016e9cbaac351e51ebbbd7d1dc9026bfeddd"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer b1a6c791f2189e0d3aba44b051e4438f78c6883c66d64014e5ccfa535acf1202
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
	-H "Authorization: Bearer b1a6c791f2189e0d3aba44b051e4438f78c6883c66d64014e5ccfa535acf1202"
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
{"password":{"reset_password_token":"sTL4-UK4FgamXCrd5tR7","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 450,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-14T12:11:07.591Z",
  "updated_at": "2016-10-14T12:11:08.228Z",
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
  "audit_id": 3794
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"sTL4-UK4FgamXCrd5tR7","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/72/comments
Content-Type: application/json
Authorization: Bearer c0b415948de40c093a0fd14bba634919d146167b062742472c3084a4965320c1
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
    "id": 15,
    "author_id": 447,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:11:07.431Z",
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
curl "api.goskive.com/v2/questions/72/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0b415948de40c093a0fd14bba634919d146167b062742472c3084a4965320c1"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/70/comments
Content-Type: application/json
Authorization: Bearer 0cb3447202da4b86fa860395c47728915fd1967337fa115db0bec207d44459f6
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
    "id": 14,
    "author_id": 441,
    "reply_to_id": null,
    "created_at": "2016-10-14T12:11:06.604Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 18,
      "user_id": 441,
      "feedbackable_id": 70,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:11:06.601Z",
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
curl "api.goskive.com/v2/questions/70/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cb3447202da4b86fa860395c47728915fd1967337fa115db0bec207d44459f6"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/68/comments
Content-Type: application/json
Authorization: Bearer d007c904b712542c8efb508f7daf77b12c2933035e552692624c95ab4406319e
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
      "id": 13,
      "author_id": 437,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:11:05.876Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 436,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:11:05.857Z",
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
curl "api.goskive.com/v2/questions/68/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d007c904b712542c8efb508f7daf77b12c2933035e552692624c95ab4406319e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/71/comments
Content-Type: application/json
Authorization: Bearer a185739563849d0b3b08d86456af218b043b8118b3cef510af64f43145c4804f
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
curl "api.goskive.com/v2/questions/71/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a185739563849d0b3b08d86456af218b043b8118b3cef510af64f43145c4804f"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/55/feedbacks
Content-Type: application/json
Authorization: Bearer 83c04d159bfb279aed4529fbe2678e9268ab619958529c4569fc109a034b040e
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
    "id": 17,
    "user_id": 356,
    "feedbackable_id": 55,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-14T12:10:59.130Z",
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
curl "api.goskive.com/v2/questions/55/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83c04d159bfb279aed4529fbe2678e9268ab619958529c4569fc109a034b040e"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/49/feedbacks
Content-Type: application/json
Authorization: Bearer 15f7c1449851ec2c853a02dd475917b8ea2c81fd1ff352bdad25ef08a3ec86d9
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
      "id": 11,
      "user_id": 330,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:10:56.822Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 329,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:10:56.810Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15f7c1449851ec2c853a02dd475917b8ea2c81fd1ff352bdad25ef08a3ec86d9"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/105/votes
Content-Type: application/json
Authorization: Bearer 1ee863dba557a7b6da549f26b29c97fc48f7062c9e3108c29dc0954a6a5ef855
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 856
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 855
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 854
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/105/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee863dba557a7b6da549f26b29c97fc48f7062c9e3108c29dc0954a6a5ef855"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/111/republish
Content-Type: application/json
Authorization: Bearer e1d1f7caa1dbb4005207589670c6d60aea4d462882f7957dae5adb599e037208
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
curl "api.goskive.com/v2/questions/111/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1d1f7caa1dbb4005207589670c6d60aea4d462882f7957dae5adb599e037208"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/108/bookmark
Content-Type: application/json
Authorization: Bearer 0cfc45a30a48eae3fd4adafdc851b4159d3f300f30263d8e68aaa29a9bd827cd
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/108/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cfc45a30a48eae3fd4adafdc851b4159d3f300f30263d8e68aaa29a9bd827cd"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/109
Content-Type: application/json
Authorization: Bearer 140c7e5474f3f6cb594745d979e436bf57729116fe554b17b245647a0cb7f586
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 140c7e5474f3f6cb594745d979e436bf57729116fe554b17b245647a0cb7f586"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/113/downvote
Content-Type: application/json
Authorization: Bearer a1fad718e88805f68757b9cddf5c0f438bacce84a465528fb06ab3eecb4206d1
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/113/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1fad718e88805f68757b9cddf5c0f438bacce84a465528fb06ab3eecb4206d1"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/114
Content-Type: application/json
Authorization: Bearer 103515f12782d1926d7f180cff3585b96587086e47fe3e5c164b6dd349b419be
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
    "id": 114,
    "obfuscated_id": "RwCVsRO9fcs",
    "author_id": 893,
    "chapter_id": 175,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:44.868Z",
    "created_at": "2016-10-14T12:11:44.744Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 230,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 231,
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
curl "api.goskive.com/v2/questions/114" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 103515f12782d1926d7f180cff3585b96587086e47fe3e5c164b6dd349b419be"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/112/report
Content-Type: application/json
Authorization: Bearer 8b8bf4560a276bce7b0f412b677dc0222361114b1098c976b21b7c60ac936b4d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/112/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b8bf4560a276bce7b0f412b677dc0222361114b1098c976b21b7c60ac936b4d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/132/bookmark
Content-Type: application/json
Authorization: Bearer 5720431515d0313bfc22c457bad1f279bd6f200baf6494ad32bf47fd652cfb3e
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/132/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5720431515d0313bfc22c457bad1f279bd6f200baf6494ad32bf47fd652cfb3e"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/115
Content-Type: application/json
Authorization: Bearer 23c16a228145df09bb5c055c69cd41f3df18a0057e280cdf55d1ce0c73bca3b9
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":115,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T12:11:45.108Z","updated_at":"2016-10-14T12:11:45.231Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":176,"author_id":896,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 115,
    "obfuscated_id": "tgK0VZO8yq4",
    "author_id": 896,
    "chapter_id": 176,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T12:11:45.346Z",
    "created_at": "2016-10-14T12:11:45.108Z",
    "tags": [
      {
        "id": 14,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 13,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>115, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-14T12:11:45.108Z\", \"updated_at\"=>\"2016-10-14T12:11:45.231Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>176, \"author_id\"=>896, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 232,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 233,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 234,
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
curl "api.goskive.com/v2/questions/115" -d '{"question":{"question":{"id":115,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T12:11:45.108Z","updated_at":"2016-10-14T12:11:45.231Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":176,"author_id":896,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23c16a228145df09bb5c055c69cd41f3df18a0057e280cdf55d1ce0c73bca3b9"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/131/upvote
Content-Type: application/json
Authorization: Bearer 64f9313bef18055dfc4f04912fc9610db50233037cb308c7a217e79c6f98e364
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/131/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64f9313bef18055dfc4f04912fc9610db50233037cb308c7a217e79c6f98e364"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 8a33f3a94b166dc92f77a4b1b1cf2b17d8c3f5eb9910574a1e86f9cdbde11309
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
      "creator_id": 320,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "topic_id": 127,
      "discipline_id": 127,
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
      "updated_at": "2016-10-14T12:10:55.809Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a33f3a94b166dc92f77a4b1b1cf2b17d8c3f5eb9910574a1e86f9cdbde11309"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer db48c87b2e31fce87b3c9522b07a21e4749b201a12ab459d19e5b9e82c3adb50
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
      "id": 101,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-81",
      "html_url": "https://goskive.com/university/uni-81",
      "slug": "uni-81",
      "name": "National School of Pizza",
      "short_name": "Uni 81",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/09a8b8c55ea0ce3828afc90e45c00163dfe1fb3e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ac9e3fc2db1eab104c524f7410091b20d81a9b4b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:10:55.637Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-80",
      "html_url": "https://goskive.com/university/uni-80",
      "slug": "uni-80",
      "name": "National School of Pastry",
      "short_name": "Uni 80",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/07974b03e020cb8d6a9497a0eae9d1c155bb897c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4e0d3b4fba5958832e20beba3d74112ff769384c.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:10:55.619Z",
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
	-H "Authorization: Bearer db48c87b2e31fce87b3c9522b07a21e4749b201a12ab459d19e5b9e82c3adb50"
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
      "id": 79,
      "name": "Customizable well-modulated core",
      "name_translations": {
        "en": "Customizable well-modulated core"
      },
      "discipline_id": 79
    },
    {
      "id": 80,
      "name": "Reverse-engineered scalable analyzer",
      "name_translations": {
        "en": "Reverse-engineered scalable analyzer"
      },
      "discipline_id": 80
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
GET /v2/topics/78
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
    "id": 78,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 78
  }
}
```



```shell
curl "api.goskive.com/v2/topics/78" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 246334f4e332296540d5a11f094c534d50d382b0e47be3233d88534ea2e1fbc4
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
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-43",
      "html_url": "https://goskive.com/university/uni-43",
      "slug": "uni-43",
      "name": "University 34",
      "short_name": "Uni 43",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ddc600c1a41c2c4dc4f7cb06220441f030500df1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2aac2a2154dc223f34258f90b071f2ba65516f33.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:10:41.786Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-44",
      "html_url": "https://goskive.com/university/uni-44",
      "slug": "uni-44",
      "name": "University 35",
      "short_name": "Uni 44",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/123583053f30d60d57698c0742b45baeaaeea45e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/467253d3f01c670a10060a75442205258e791570.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T12:10:41.804Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-45",
      "html_url": "https://goskive.com/university/uni-45",
      "slug": "uni-45",
      "name": "University 36",
      "short_name": "Uni 45",
      "acronym": "MIT",
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
      "updated_at": "2016-10-14T12:10:41.821Z",
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
	-H "Authorization: Bearer 246334f4e332296540d5a11f094c534d50d382b0e47be3233d88534ea2e1fbc4"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer c173ee363fc9d0ce0695ef6a783373262027df925cb9986b0a0354e61fcdcbc3
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
    "id": 64,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/34ae0a587d54bcfff28a891b60e4ff558b06fe03.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/82b731c89e2f272b7201803005596c5d91004739.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-14T12:10:41.957Z",
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
	-H "Authorization: Bearer c173ee363fc9d0ce0695ef6a783373262027df925cb9986b0a0354e61fcdcbc3"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c64533afda4ba8df18967662a5f94eb89a8e3581bc0b9ea0ff81c5e714d82d25
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":14,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 42,
    "id": 12,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 13,
    "additional_university_ids": [

    ],
    "topic_id": 14,
    "discipline_id": 14,
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
    "chapters_updated_at": "2016-10-14T12:10:28.375Z",
    "updated_at": "2016-10-14T12:10:28.520Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 8,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-14T12:10:28.475Z",
        "course_id": 12,
        "author_id": 42,
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
        "id": 9,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-14T12:10:28.493Z",
        "course_id": 12,
        "author_id": 42,
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
        "id": 10,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-14T12:10:28.510Z",
        "course_id": 12,
        "author_id": 42,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":14,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c64533afda4ba8df18967662a5f94eb89a8e3581bc0b9ea0ff81c5e714d82d25"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ed7399473621c9b5cd7ab70fe769ec669481e164e4ddffca69a26bd76e74b9d1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":13,"published":false}}
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
    "creator_id": 41,
    "id": 11,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 12,
    "additional_university_ids": [

    ],
    "topic_id": 13,
    "discipline_id": 13,
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
    "updated_at": "2016-10-14T12:10:28.266Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":13,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed7399473621c9b5cd7ab70fe769ec669481e164e4ddffca69a26bd76e74b9d1"
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
      "creator_id": 66,
      "id": 33,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-29",
      "html_url": "https://goskive.com/course/fu-course-29",
      "slug": "fu-course-29",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "topic_id": 35,
      "discipline_id": 35,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 29",
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
      "updated_at": "2016-10-14T12:10:30.959Z",
      "shortname": "fu-course-29"
    },
    {
      "creator_id": 66,
      "id": 34,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-30",
      "html_url": "https://goskive.com/course/fu-course-30",
      "slug": "fu-course-30",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "topic_id": 36,
      "discipline_id": 36,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 30",
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
      "chapters_updated_at": "2016-10-14T12:10:31.261Z",
      "updated_at": "2016-10-14T12:10:31.268Z",
      "shortname": "fu-course-30"
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
Authorization: Bearer 9714ec7a407db8ff7a11d0de191eed69b85e5a61acd00c2315739b239461d336
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
      "creator_id": 73,
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-37",
      "html_url": "https://goskive.com/course/fu-course-37",
      "slug": "fu-course-37",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 43,
      "discipline_id": 43,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 37",
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
      "updated_at": "2016-10-14T12:10:31.757Z",
      "shortname": "fu-course-37"
    },
    {
      "creator_id": 73,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-38",
      "html_url": "https://goskive.com/course/fu-course-38",
      "slug": "fu-course-38",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "topic_id": 44,
      "discipline_id": 44,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 38",
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
      "chapters_updated_at": "2016-10-14T12:10:32.069Z",
      "updated_at": "2016-10-14T12:10:32.077Z",
      "shortname": "fu-course-38"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9714ec7a407db8ff7a11d0de191eed69b85e5a61acd00c2315739b239461d336"
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
      "creator_id": 71,
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-33",
      "html_url": "https://goskive.com/course/fu-course-33",
      "slug": "fu-course-33",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 39,
      "discipline_id": 39,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 33",
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
      "updated_at": "2016-10-14T12:10:31.512Z",
      "shortname": "fu-course-33"
    },
    {
      "creator_id": 71,
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-34",
      "html_url": "https://goskive.com/course/fu-course-34",
      "slug": "fu-course-34",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 40,
      "discipline_id": 40,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 34",
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
      "updated_at": "2016-10-14T12:10:31.553Z",
      "shortname": "fu-course-34"
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
Authorization: Bearer 86d7c67420b9d46c8d07d29859bd38c3f82e488305fc792d90de5936f525ffb3
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
      "creator_id": 79,
      "id": 45,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 26,
      "additional_university_ids": [

      ],
      "topic_id": 47,
      "discipline_id": 47,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
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
      "updated_at": "2016-10-14T12:10:32.314Z",
      "shortname": "fu-course-41"
    },
    {
      "creator_id": 79,
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 26,
      "additional_university_ids": [

      ],
      "topic_id": 48,
      "discipline_id": 48,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
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
      "updated_at": "2016-10-14T12:10:32.356Z",
      "shortname": "fu-course-42"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86d7c67420b9d46c8d07d29859bd38c3f82e488305fc792d90de5936f525ffb3"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 660ebe61f1771dbef2ae04cca0bdca6a3b1952cd6ed3d9eef44cab3e9487bfeb
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
  "id": 850,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-14T12:11:39.603Z",
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
	-H "Authorization: Bearer 660ebe61f1771dbef2ae04cca0bdca6a3b1952cd6ed3d9eef44cab3e9487bfeb"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/37
Content-Type: application/json
Authorization: Bearer 39e0930dd7ff720384260c4d168b07e120b80451d1b629315365a2d2be4b5766
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
    "id": 37,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 11,
    "fields_of_study": [
      11,
      12
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-14T12:10:28.009Z",
    "updated_at": "2016-10-14T12:10:28.009Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39e0930dd7ff720384260c4d168b07e120b80451d1b629315365a2d2be4b5766"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/39
Content-Type: application/json
Authorization: Bearer f4be9cb1d0317e970b0880de4011399a994454f71c92fae941b0584993e1c189
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
    "id": 39,
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
    "created_at": "2016-10-14T12:10:28.102Z",
    "updated_at": "2016-10-14T12:10:28.102Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4be9cb1d0317e970b0880de4011399a994454f71c92fae941b0584993e1c189"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 244ab5efc84839578783648ad73f98e204db2bd1b5a3adfcd9fcdf35fe6a5386
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
	-H "Authorization: Bearer 244ab5efc84839578783648ad73f98e204db2bd1b5a3adfcd9fcdf35fe6a5386"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer 4a70a99684f58d9b491007af0e17900e14f55af148661943eafe7f9f3facad02
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
    "votable_id": 103,
    "user_id": 765
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a70a99684f58d9b491007af0e17900e14f55af148661943eafe7f9f3facad02"
```
