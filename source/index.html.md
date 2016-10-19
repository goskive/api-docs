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
Authorization: Basic MWI5OTIxZmRhMDdmMjNmZTU5MDAzMzQ3MDRhN2NkNmM5NmE0OGVlMTg1Yzkx
NGRkNjJhYTMxNGE1MmI1ODY5NzowMjlkNjEyYzk5NzI1MzNhM2U3MjQxYTdl
MzczMTI4ODYzOWU3Njk1NTk4OWI1YWY2OTk1MDZhZDYxOGIzY2Fi

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
	-u 1b9921fda07f23fe5900334704a7cd6c96a48ee185c914dd62aa314a52b58697:029d612c9972533a3e7241a7e3731288639e76955989b5af699506ad618b3cab
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e4b6255e91104f8da78dca76d1aec48ec6194793dc60f592d2ae556250016d6b","client_secret":"fd9ac6ea34d5d9ea58c3b2fd5f2da32511bb012a709de0b6307ad0feae04cf85"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e4b6255e91104f8da78dca76d1aec48ec6194793dc60f592d2ae556250016d6b","client_secret":"fd9ac6ea34d5d9ea58c3b2fd5f2da32511bb012a709de0b6307ad0feae04cf85"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"88aff8c7e68a0ddd6fac3b2a843d007ea1d7d1e0365695d100ca94d387550d42","client_secret":"5f90af49388d98b81102af1efee8802995841eb2ad04f2f99d3ecb27312f2dcf"}
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
  "access_token": "5da15d48674af1256404738731844900ad4de23867e5be19d8d166e81662b111",
  "token_type": "bearer",
  "created_at": 1476864322
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"88aff8c7e68a0ddd6fac3b2a843d007ea1d7d1e0365695d100ca94d387550d42","client_secret":"5f90af49388d98b81102af1efee8802995841eb2ad04f2f99d3ecb27312f2dcf"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZTAyNDdmN2ZjNzZjODBkZjgyMjg1ODI3NzQ2NzcxMTkwNzMxMmNmOTgzYWUz
M2UwNmU2ODAwZGNiNzQ0NTE5ZTo4NDdlZjM2MGIwOTdmMDVhMWJiNmVjYmIx
NDRmZmQ5NTNkM2QyNGU2ZjkyNzk3MjdmOWU0NjFlNmQwNTg3YzY2

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
  "access_token": "86e35aeaffdffb9ec2c60a61ecc3e1621eaff368ab7eb41dce8023af5bbcabc8",
  "token_type": "bearer",
  "created_at": 1476864322
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u e0247f7fc76c80df822858277467711907312cf983ae33e06e6800dcb744519e:847ef360b097f05a1bb6ecbb144ffd953d3d24e6f9279727f9e461e6d0587c66
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"3baa19a00bbd46e12cac9909fc5a01d94e411a4886fec8b695fc9a41b3cd0b02","client_secret":"d2ae0e3b93480860f067accede1aff374755610c43823d086607064169209211"}
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
  "access_token": "f803fda9b4ca09593d8f79dca67377541f8205a6f26969443a68b087d488e170",
  "token_type": "bearer",
  "created_at": 1476864322
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"3baa19a00bbd46e12cac9909fc5a01d94e411a4886fec8b695fc9a41b3cd0b02","client_secret":"d2ae0e3b93480860f067accede1aff374755610c43823d086607064169209211"}' -X POST \
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
Authorization: Bearer bfd4284645aa7bd0e9c7feb6737d31be299a9081a4390a3e21b0ebe3ec43ac1d
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
    "company_id": 17,
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
	-H "Authorization: Bearer bfd4284645aa7bd0e9c7feb6737d31be299a9081a4390a3e21b0ebe3ec43ac1d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/150/flashcards
Content-Type: application/json
Authorization: Bearer 8bcd61de055b67bf4c03510df54839fdee19c9160911610f837aaa08b7f46b87
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":150,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 90,
    "obfuscated_id": "gX_ALSaJ0k4",
    "author_id": 650,
    "chapter_id": 150,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:59.809Z",
    "created_at": "2016-10-19T08:04:59.809Z",
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
curl "api.goskive.com/v2/chapters/150/flashcards" -d '{"flashcard":{"chapter_id":150,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8bcd61de055b67bf4c03510df54839fdee19c9160911610f837aaa08b7f46b87"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/149/flashcards
Content-Type: application/json
Authorization: Bearer dc3b94558e91189f71289b11dfe77899aef81ca31342a11786cd746b180c03fc
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
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 645,
      "chapter_id": 149,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:59.557Z",
      "created_at": "2016-10-19T08:04:59.557Z",
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
      "author_id": 645,
      "chapter_id": 149,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:59.590Z",
      "created_at": "2016-10-19T08:04:59.590Z",
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 645,
      "chapter_id": 149,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:59.623Z",
      "created_at": "2016-10-19T08:04:59.623Z",
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
curl "api.goskive.com/v2/chapters/149/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc3b94558e91189f71289b11dfe77899aef81ca31342a11786cd746b180c03fc"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/54/questions
Content-Type: application/json
Authorization: Bearer 064d96e966c0c49bef7563b0659245a7704af2b24f91ca1bfb72cc630fd98692
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
    "id": 43,
    "obfuscated_id": "uapnSdBCag8",
    "author_id": 268,
    "chapter_id": 54,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:28.344Z",
    "created_at": "2016-10-19T08:04:28.344Z",
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
        "id": 85,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 86,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 87,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 88,
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
	-H "Authorization: Bearer 064d96e966c0c49bef7563b0659245a7704af2b24f91ca1bfb72cc630fd98692"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/52/questions
Content-Type: application/json
Authorization: Bearer 1813f078b3352286b81ec6736e3bd4a1014e852bd5dc4a78656cad240af8d16e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":52,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 41,
    "obfuscated_id": "11qbskrctUU",
    "author_id": 262,
    "chapter_id": 52,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:27.600Z",
    "created_at": "2016-10-19T08:04:27.600Z",
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
        "id": 81,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 82,
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
curl "api.goskive.com/v2/chapters/52/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":52,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1813f078b3352286b81ec6736e3bd4a1014e852bd5dc4a78656cad240af8d16e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/53/questions
Content-Type: application/json
Authorization: Bearer aa54cf49c80e4a54a7e9e6daedce8fe546be58fb1652d5804f54f239f0c7c5f5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":53,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 42,
    "obfuscated_id": "6gppIIjkzlA",
    "author_id": 265,
    "chapter_id": 53,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:27.965Z",
    "created_at": "2016-10-19T08:04:27.965Z",
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
        "id": 83,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 84,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/53/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":53,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa54cf49c80e4a54a7e9e6daedce8fe546be58fb1652d5804f54f239f0c7c5f5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/55/questions
Content-Type: application/json
Authorization: Bearer ac8f7c7b5c83a993fd9f58e1eb8edd2e7db29b2fa954ab0b6f23f22e908b8920
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":55,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 271,
    "chapter_id": 55,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:28.883Z",
    "created_at": "2016-10-19T08:04:28.883Z",
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
        "id": 89,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 90,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 91,
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
curl "api.goskive.com/v2/chapters/55/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":55,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac8f7c7b5c83a993fd9f58e1eb8edd2e7db29b2fa954ab0b6f23f22e908b8920"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/50/questions
Content-Type: application/json
Authorization: Bearer d3d5fb7ed9aa36970ff377196031fcbaf9438ee4287c189c4c2c623349ef0b0e
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
      "id": 38,
      "obfuscated_id": "8_YCqPYFnsI",
      "author_id": 253,
      "chapter_id": 50,
      "position": 38,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:26.748Z",
      "created_at": "2016-10-19T08:04:26.613Z",
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 254,
      "chapter_id": 50,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:26.965Z",
      "created_at": "2016-10-19T08:04:26.827Z",
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
          "id": 77,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 78,
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
      "author_id": 255,
      "chapter_id": 50,
      "position": 40,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:04:27.192Z",
      "created_at": "2016-10-19T08:04:27.049Z",
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
```



```shell
curl "api.goskive.com/v2/chapters/50/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3d5fb7ed9aa36970ff377196031fcbaf9438ee4287c189c4c2c623349ef0b0e"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/12
Content-Type: application/json
Authorization: Bearer c040e72fdc1f41c7d0fe9d6f691a260c5996a7572959ca1af25fd47c0d89b7e7
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
curl "api.goskive.com/v2/chapters/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c040e72fdc1f41c7d0fe9d6f691a260c5996a7572959ca1af25fd47c0d89b7e7"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/14
Content-Type: application/json
Authorization: Bearer b68dbd4dfb65852a9fab03f7e1dad05f192a8e0af5570aee19bce7a82c65e73c
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
curl "api.goskive.com/v2/chapters/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b68dbd4dfb65852a9fab03f7e1dad05f192a8e0af5570aee19bce7a82c65e73c"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 8a2903d81fe01e577a8786f30fcdf62c059b294fb57a7957fdbfb6fc61d382c4
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
curl "api.goskive.com/v2/chapters/7" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a2903d81fe01e577a8786f30fcdf62c059b294fb57a7957fdbfb6fc61d382c4"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/15
Content-Type: application/json
Authorization: Bearer 621495b00513c9eb3b4a4bf8b1475dc6224160718a47495d600896a259f71558
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 621495b00513c9eb3b4a4bf8b1475dc6224160718a47495d600896a259f71558"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/11
Content-Type: application/json
Authorization: Bearer 0a9895e02c92b995aee8912f2e696cb3f9b756d3ed1830282ac31959f8a2334b
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
    "id": 11,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T08:04:12.098Z",
    "course_id": 15,
    "author_id": 50,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-19T08:04:11.565Z",
    "questions_updated_at": "2016-10-19T08:04:11.565Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 54,
        "chapter_id": 11,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:12.080Z",
        "created_at": "2016-10-19T08:04:12.080Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 52,
        "chapter_id": 11,
        "position": 10,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:11.975Z",
        "created_at": "2016-10-19T08:04:11.855Z",
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
          }
        ]
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a9895e02c92b995aee8912f2e696cb3f9b756d3ed1830282ac31959f8a2334b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 6024803437412a73ec7dee09394c1c6837aad3ca2f2d262e39a2d2a9ba64e477
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
    "id": 9,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T08:04:10.893Z",
    "course_id": 13,
    "author_id": 41,
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
curl "api.goskive.com/v2/chapters/9" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6024803437412a73ec7dee09394c1c6837aad3ca2f2d262e39a2d2a9ba64e477"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/10/replies
Content-Type: application/json
Authorization: Bearer 35eb639939a2792cba753dabe02ce9c4274b874505de1a1b2d74ed5adda46dd7
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
    "id": 11,
    "author_id": 349,
    "reply_to_id": 10,
    "created_at": "2016-10-19T08:04:38.840Z",
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
curl "api.goskive.com/v2/comments/10/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35eb639939a2792cba753dabe02ce9c4274b874505de1a1b2d74ed5adda46dd7"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/9/replies
Content-Type: application/json
Authorization: Bearer a52d76a816a4e33ad3a296bde37d56e9557d22847a95718d2b3eb5f2ade7dd31
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
curl "api.goskive.com/v2/comments/9/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a52d76a816a4e33ad3a296bde37d56e9557d22847a95718d2b3eb5f2ade7dd31"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/56
Content-Type: application/json
Authorization: Bearer fa0f2849a6ea03fc5a24e1d8664c8aa04011723f045e1291b7a46942db23b65c
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
curl "api.goskive.com/v2/comments/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa0f2849a6ea03fc5a24e1d8664c8aa04011723f045e1291b7a46942db23b65c"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/59/republish
Content-Type: application/json
Authorization: Bearer 762e9c602fbf26ad6bd8a20b43b8f0d7a69430e000d4ca76a7cf76ee5e6b4886
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
curl "api.goskive.com/v2/comments/59/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 762e9c602fbf26ad6bd8a20b43b8f0d7a69430e000d4ca76a7cf76ee5e6b4886"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/57
Content-Type: application/json
Authorization: Bearer 84a6b4b8536e6f0c20dde2acd7b49d1e86d281a6dbb3966b5e45c6fc2183dee3
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84a6b4b8536e6f0c20dde2acd7b49d1e86d281a6dbb3966b5e45c6fc2183dee3"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 3c87201bbd20f9f1b93519617d6891d0fd0a93d25f711455186e6b9f9c106fa5
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
	-H "Authorization: Bearer 3c87201bbd20f9f1b93519617d6891d0fd0a93d25f711455186e6b9f9c106fa5"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/16
Content-Type: application/json
Authorization: Bearer cd10552d312d94e867099df4f1a564a86a8c0457dd12acff9b3cccabc38a0fd4
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
    "updated_at": "2016-10-19T08:04:26.402Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd10552d312d94e867099df4f1a564a86a8c0457dd12acff9b3cccabc38a0fd4"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 5abf91fff589ae8b5358c9e2127a0471a6785aeb5f5e00b920ed77e3c7643753
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
      "id": 13,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:04:26.283Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:04:26.287Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:04:26.291Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5abf91fff589ae8b5358c9e2127a0471a6785aeb5f5e00b920ed77e3c7643753"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer a9eb924c742ae350dba17e87edb06d1f0b77551587c59195ad16a9140b7e20e4
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
	-H "Authorization: Bearer a9eb924c742ae350dba17e87edb06d1f0b77551587c59195ad16a9140b7e20e4"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 18052d4fac7c2c25a5557ad76973188f7b5f23482efb5da52032de7835924e77
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
curl "api.goskive.com/v2/companies/26/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18052d4fac7c2c25a5557ad76973188f7b5f23482efb5da52032de7835924e77"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer ecba7999b8ef79e83110037204b1dae10f855189eec20e05cf2caff4a767c062
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
	-H "Authorization: Bearer ecba7999b8ef79e83110037204b1dae10f855189eec20e05cf2caff4a767c062"
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
Authorization: Bearer 3d18cf98b65bd7bffaac56fabf57c5ea214ebfe999cd2266c70f3da8a7524c5c
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
	-H "Authorization: Bearer 3d18cf98b65bd7bffaac56fabf57c5ea214ebfe999cd2266c70f3da8a7524c5c"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 87246222003dca584474436e619f98279af586ed311d3c729912eb5195b78f14
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
    "id": 94,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T08:04:42.633Z",
    "course_id": 102,
    "author_id": 414,
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
	-H "Authorization: Bearer 87246222003dca584474436e619f98279af586ed311d3c729912eb5195b78f14"
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
      "id": 77,
      "title": "Clever Chapter Title 62",
      "position": 1,
      "updated_at": "2016-10-19T08:04:40.702Z",
      "course_id": 91,
      "author_id": 376,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 78,
      "title": "Clever Chapter Title 63",
      "position": 2,
      "updated_at": "2016-10-19T08:04:40.725Z",
      "course_id": 91,
      "author_id": 377,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 79,
      "title": "Clever Chapter Title 64",
      "position": 3,
      "updated_at": "2016-10-19T08:04:40.956Z",
      "course_id": 91,
      "author_id": 378,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T08:04:40.632Z",
      "questions_updated_at": "2016-10-19T08:04:40.632Z",
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
Authorization: Bearer 20e25b07dc2f7e90ace2224d2d7bb3df907eeb4ad317b8dc9660323d88ca9371
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
      "id": 83,
      "title": "Clever Chapter Title 68",
      "position": 1,
      "updated_at": "2016-10-19T08:04:41.293Z",
      "course_id": 94,
      "author_id": 387,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 84,
      "title": "Clever Chapter Title 69",
      "position": 2,
      "updated_at": "2016-10-19T08:04:41.316Z",
      "course_id": 94,
      "author_id": 388,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 85,
      "title": "Clever Chapter Title 70",
      "position": 3,
      "updated_at": "2016-10-19T08:04:41.546Z",
      "course_id": 94,
      "author_id": 389,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T08:04:41.223Z",
      "questions_updated_at": "2016-10-19T08:04:41.223Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20e25b07dc2f7e90ace2224d2d7bb3df907eeb4ad317b8dc9660323d88ca9371"
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
      "id": 80,
      "title": "Clever Chapter Title 65",
      "position": 1,
      "updated_at": "2016-10-19T08:04:41.068Z",
      "course_id": 92,
      "author_id": 382,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 81,
      "title": "Clever Chapter Title 66",
      "position": 2,
      "updated_at": "2016-10-19T08:04:41.091Z",
      "course_id": 92,
      "author_id": 383,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 82,
      "title": "Clever Chapter Title 67",
      "position": 3,
      "updated_at": "2016-10-19T08:04:41.113Z",
      "course_id": 92,
      "author_id": 384,
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
Authorization: Bearer 3443a29c6581afe618e304678b0266d7e8e77910c73ef9cb01ff00adb354fcb1
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
      "id": 86,
      "title": "Clever Chapter Title 71",
      "position": 1,
      "updated_at": "2016-10-19T08:04:41.692Z",
      "course_id": 95,
      "author_id": 394,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 87,
      "title": "Clever Chapter Title 72",
      "position": 2,
      "updated_at": "2016-10-19T08:04:41.715Z",
      "course_id": 95,
      "author_id": 395,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 88,
      "title": "Clever Chapter Title 73",
      "position": 3,
      "updated_at": "2016-10-19T08:04:41.737Z",
      "course_id": 95,
      "author_id": 396,
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
	-H "Authorization: Bearer 3443a29c6581afe618e304678b0266d7e8e77910c73ef9cb01ff00adb354fcb1"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 6396ea4dad285a1f80d800a7d81e8226bf1465f60d19dcc4445fb338eceabf9e
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
    "course_id": 149,
    "user_id": 562,
    "updated_at": "2016-10-19T08:04:55.494Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6396ea4dad285a1f80d800a7d81e8226bf1465f60d19dcc4445fb338eceabf9e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f56441e85ac6b5607d9a8d930c226b9b55d8b7b25cd4acef0ea7bff35dd74520
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
      "course_id": 147,
      "user_id": 556,
      "updated_at": "2016-10-19T08:04:55.205Z"
    },
    {
      "id": 5,
      "course_id": 147,
      "user_id": 557,
      "updated_at": "2016-10-19T08:04:55.218Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f56441e85ac6b5607d9a8d930c226b9b55d8b7b25cd4acef0ea7bff35dd74520"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/253/files
Content-Type: application/json
Authorization: Bearer 55b1951343c03526ec40ebb08a38d9d87a426800ad939d8ec23404c6c458be5f
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
      "id": 12,
      "uploader": {
        "id": 805,
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
        "created_at": "2016-10-19T08:05:13.032Z",
        "updated_at": "2016-10-19T08:05:13.032Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T08:05:13.038Z",
      "updated_at": "2016-10-19T08:05:13.038Z",
      "course_id": 253,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 806,
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
        "created_at": "2016-10-19T08:05:13.045Z",
        "updated_at": "2016-10-19T08:05:13.045Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T08:05:13.050Z",
      "updated_at": "2016-10-19T08:05:13.050Z",
      "course_id": 253,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 807,
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
        "created_at": "2016-10-19T08:05:13.057Z",
        "updated_at": "2016-10-19T08:05:13.057Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T08:05:13.063Z",
      "updated_at": "2016-10-19T08:05:13.063Z",
      "course_id": 253,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/253/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55b1951343c03526ec40ebb08a38d9d87a426800ad939d8ec23404c6c458be5f"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/256/files
Content-Type: application/json
Authorization: Bearer 6cbae7628112bca667551d0786d83d5209f99fd114ed3ab770fb8394b47f2fcf
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
    "id": 15,
    "uploader": {
      "id": 814,
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
      "created_at": "2016-10-19T08:05:13.381Z",
      "updated_at": "2016-10-19T08:05:13.381Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [

    ],
    "created_at": "2016-10-19T08:05:13.407Z",
    "updated_at": "2016-10-19T08:05:13.407Z",
    "course_id": 256,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/256/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cbae7628112bca667551d0786d83d5209f99fd114ed3ab770fb8394b47f2fcf"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/255/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 713949673836f8df185ebc7d6382c583ddc34f345d814a36d24523037f12f25f
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
    "key": "cache/52682b8b0e583f13e39640fe37d6dbc3.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQwOTowNToxM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS81MjY4MmI4YjBlNTgzZjEzZTM5NjQwZmUzN2Q2ZGJjMy5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTlUMDgwNTEzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T080513Z",
    "x-amz-signature": "6378634055990a98da45e53f61ffdcc70b097d6a43584bf8ab39596f924160d9"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/255/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 713949673836f8df185ebc7d6382c583ddc34f345d814a36d24523037f12f25f"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer c0a87f90473807adc1696a636483f9fdd0d34e204720c535d01233b712d13ba2
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
	-H "Authorization: Bearer c0a87f90473807adc1696a636483f9fdd0d34e204720c535d01233b712d13ba2"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5fa9ef9eabf1734d0d0d1a5e07f576bee021e8786e69ad69f2e5d49c7bf7d1b4
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
	-H "Authorization: Bearer 5fa9ef9eabf1734d0d0d1a5e07f576bee021e8786e69ad69f2e5d49c7bf7d1b4"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 25f124ccd645265d19bdb15fee12f855f1a9d2b2648ef96e583b8190c16e6cd7
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
	-H "Authorization: Bearer 25f124ccd645265d19bdb15fee12f855f1a9d2b2648ef96e583b8190c16e6cd7"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d27ff9f9c06a750ef44fd03829600c0644b24ed247be97245d456951fa803e3f
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
	-H "Authorization: Bearer d27ff9f9c06a750ef44fd03829600c0644b24ed247be97245d456951fa803e3f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 922cee98c63db52003f24de5872f541aee7523f2ed4525ba84f281a4f6310516
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
	-H "Authorization: Bearer 922cee98c63db52003f24de5872f541aee7523f2ed4525ba84f281a4f6310516"
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
    "creator_id": 523,
    "id": 137,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 144,
    "additional_university_ids": [

    ],
    "topic_id": 149,
    "discipline_id": 150,
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
    "chapters_updated_at": "2016-10-19T08:04:50.105Z",
    "updated_at": "2016-10-19T08:04:51.411Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 118,
        "title": "Clever Chapter Title 100",
        "position": 1,
        "updated_at": "2016-10-19T08:04:51.369Z",
        "course_id": 137,
        "author_id": 523,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:04:50.105Z",
        "questions_updated_at": "2016-10-19T08:04:50.105Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 119,
        "title": "Clever Chapter Title 101",
        "position": 2,
        "updated_at": "2016-10-19T08:04:51.404Z",
        "course_id": 137,
        "author_id": 523,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:04:50.105Z",
        "questions_updated_at": "2016-10-19T08:04:50.105Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 523,
        "chapter_id": 118,
        "position": 72,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:50.301Z",
        "created_at": "2016-10-19T08:04:50.193Z",
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
            "id": 154,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 155,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 523,
        "chapter_id": 119,
        "position": 74,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:50.650Z",
        "created_at": "2016-10-19T08:04:50.537Z",
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
            "id": 158,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 159,
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
Authorization: Bearer fdd7519feb786351b71fc062c28ad161596f31230c61c4b9129af58693219a0d
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
    "creator_id": 528,
    "id": 138,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 145,
    "additional_university_ids": [

    ],
    "topic_id": 150,
    "discipline_id": 151,
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
    "chapters_updated_at": "2016-10-19T08:04:51.463Z",
    "updated_at": "2016-10-19T08:04:52.772Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 120,
        "title": "Clever Chapter Title 102",
        "position": 1,
        "updated_at": "2016-10-19T08:04:52.730Z",
        "course_id": 138,
        "author_id": 528,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:04:51.463Z",
        "questions_updated_at": "2016-10-19T08:04:51.463Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 121,
        "title": "Clever Chapter Title 103",
        "position": 2,
        "updated_at": "2016-10-19T08:04:52.765Z",
        "course_id": 138,
        "author_id": 528,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:04:51.463Z",
        "questions_updated_at": "2016-10-19T08:04:51.463Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 529,
        "chapter_id": 120,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.587Z",
        "created_at": "2016-10-19T08:04:52.587Z",
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
        "author_id": 529,
        "chapter_id": 121,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.650Z",
        "created_at": "2016-10-19T08:04:52.650Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 529,
        "chapter_id": 120,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.622Z",
        "created_at": "2016-10-19T08:04:52.622Z",
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
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 529,
        "chapter_id": 121,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.686Z",
        "created_at": "2016-10-19T08:04:52.686Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 529,
        "chapter_id": 120,
        "position": 78,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:51.665Z",
        "created_at": "2016-10-19T08:04:51.558Z",
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
      },
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 529,
        "chapter_id": 120,
        "position": 79,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:51.826Z",
        "created_at": "2016-10-19T08:04:51.724Z",
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
            "id": 168,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 169,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 529,
        "chapter_id": 121,
        "position": 80,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.013Z",
        "created_at": "2016-10-19T08:04:51.903Z",
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
            "id": 170,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 171,
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
        "author_id": 529,
        "chapter_id": 121,
        "position": 81,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:04:52.178Z",
        "created_at": "2016-10-19T08:04:52.074Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdd7519feb786351b71fc062c28ad161596f31230c61c4b9129af58693219a0d"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/126/pin
Content-Type: application/json
Authorization: Bearer dd483cf1d7966b95f8a12cef95aa4dcd5e0bc688c34bb32d083bdee8fe4dd301
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/126/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd483cf1d7966b95f8a12cef95aa4dcd5e0bc688c34bb32d083bdee8fe4dd301"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/140/pin
Content-Type: application/json
Authorization: Bearer a78db58653c44ac599cf097ff8eea01a5824a13540a155e750d9e8b2a6452438
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/140/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a78db58653c44ac599cf097ff8eea01a5824a13540a155e750d9e8b2a6452438"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 65563381300995184f26d48641ac8c2e9f72c31fd50e0e22e08ab7b8c037ba85
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
    "creator_id": 542,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 148,
    "additional_university_ids": [

    ],
    "topic_id": 153,
    "discipline_id": 154,
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
    "updated_at": "2016-10-19T08:04:54.500Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65563381300995184f26d48641ac8c2e9f72c31fd50e0e22e08ab7b8c037ba85"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 65564fdab26d3da86d301a97242b52b1889b701fb4a643c945e205a1802e02a1
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
    "id": 238,
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
    "created_at": "2016-10-19T08:04:25.433Z",
    "updated_at": "2016-10-19T08:04:25.433Z",
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
	-H "Authorization: Bearer 65564fdab26d3da86d301a97242b52b1889b701fb4a643c945e205a1802e02a1"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer daaf24dab3bca9a16153a7cda1d7a59a4d9ff7dd813b0cab998a250479eec951
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[64]}
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
    "id": 234,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      64
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:04:25.171Z",
    "updated_at": "2016-10-19T08:04:25.207Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[64]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daaf24dab3bca9a16153a7cda1d7a59a4d9ff7dd813b0cab998a250479eec951"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 68b64c99b3401551d0de90a1b2abd5c34ca8f2a692e5398f8bdd47e22e0ccc00
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
    "id": 235,
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
    "created_at": "2016-10-19T08:04:25.227Z",
    "updated_at": "2016-10-19T08:04:25.227Z",
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
	-H "Authorization: Bearer 68b64c99b3401551d0de90a1b2abd5c34ca8f2a692e5398f8bdd47e22e0ccc00"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0324368a2d5094fd68e896fd0176174bae55d7aa2805d6d685df34da53582d24
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[66]}
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
    "id": 236,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      66
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:04:25.316Z",
    "updated_at": "2016-10-19T08:04:25.316Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[66]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0324368a2d5094fd68e896fd0176174bae55d7aa2805d6d685df34da53582d24"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a7f5549aaf3cb0d6cbe858580b080a363207553beb0d54457950bc23656a824f
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

63
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
    "id": 233,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9712dc601dda0d6620b9aa27455f7e90f3659908.jpg",
    "university_id": null,
    "fields_of_study": [
      63
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:04:24.789Z",
    "updated_at": "2016-10-19T08:04:25.115Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/97807af057309419a5a4846a2327643eeb0b9efb.jpg",
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

63
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a7f5549aaf3cb0d6cbe858580b080a363207553beb0d54457950bc23656a824f"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 79fa2c5ad62a28a3d27769822833c41eb61e09429b4300b2c40c719ec5981bee
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
      "id": 1,
      "bookmarkable_id": 58,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 59,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 60,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79fa2c5ad62a28a3d27769822833c41eb61e09429b4300b2c40c719ec5981bee"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer aae90aa89fad0e31342d459f76613e1724d506074dcb83c9528b90e69114da66
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
      "company_id": 22,
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
      "id": 12,
      "title": "Campaign 11",
      "company_id": 23,
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
	-H "Authorization: Bearer aae90aa89fad0e31342d459f76613e1724d506074dcb83c9528b90e69114da66"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 18ae130ad79b6ae36d883d45a1a12203f1516fdddce1faaa456d080d3af181f5
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
      "company_id": 18,
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
	-H "Authorization: Bearer 18ae130ad79b6ae36d883d45a1a12203f1516fdddce1faaa456d080d3af181f5"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer b30fcb8a5352d57d69759f47b95ac23c22c3ded0a3009445ed0f53a5c2c7cc83
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
      "creator_id": 351,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-56",
      "html_url": "https://goskive.com/course/mit-course-56",
      "slug": "mit-course-56",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 97,
      "discipline_id": 98,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
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
      "updated_at": "2016-10-19T08:04:39.069Z",
      "shortname": "mit-course-56"
    },
    {
      "creator_id": 352,
      "id": 86,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-57",
      "html_url": "https://goskive.com/course/mit-course-57",
      "slug": "mit-course-57",
      "university_id": 93,
      "additional_university_ids": [

      ],
      "topic_id": 98,
      "discipline_id": 99,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
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
      "updated_at": "2016-10-19T08:04:39.151Z",
      "shortname": "mit-course-57"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b30fcb8a5352d57d69759f47b95ac23c22c3ded0a3009445ed0f53a5c2c7cc83"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e5282c77c6fb2bfc89d86ec2cf6b8e9c0638f552ce48af3e7c6b88eee7f6f8e7
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
        "updated_at": "2016-10-19T08:05:22.020Z"
      },
      "created_at": "2016-10-19T08:05:22.024Z",
      "updated_at": "2016-10-19T08:05:22.024Z",
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
        "updated_at": "2016-10-19T08:05:22.031Z"
      },
      "created_at": "2016-10-19T08:05:22.035Z",
      "updated_at": "2016-10-19T08:05:22.035Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5282c77c6fb2bfc89d86ec2cf6b8e9c0638f552ce48af3e7c6b88eee7f6f8e7"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer dc3aef29b65decc01ce7b8a7b897b2141302472e018ad673db3524185818cd1b
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
        "updated_at": "2016-10-19T08:05:21.819Z"
      },
      "created_at": "2016-10-19T08:05:21.822Z",
      "updated_at": "2016-10-19T08:05:21.822Z",
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
        "updated_at": "2016-10-19T08:05:21.836Z"
      },
      "created_at": "2016-10-19T08:05:21.839Z",
      "updated_at": "2016-10-19T08:05:21.839Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc3aef29b65decc01ce7b8a7b897b2141302472e018ad673db3524185818cd1b"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 00c97d824e7d15a9ecd7d7552f24360841ea4187c17e3c731c7cda11727d0455
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
      "created_at": "2016-10-19T08:04:13.692Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-19T08:04:13.793Z",
      "author_id": "79",
      "thread_subject_id": "21",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 4,
      "created_at": "2016-10-19T08:04:13.782Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-10-19T08:04:13.796Z",
      "author_id": "82",
      "thread_subject_id": "22",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-10-19T08:04:14.193Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-10-19T08:04:14.193Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-19T08:04:14.562Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-10-19T08:04:14.562Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 7,
      "created_at": "2016-10-19T08:04:14.942Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-10-19T08:04:14.942Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 8,
      "created_at": "2016-10-19T08:04:15.246Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 16,
      "updated_at": "2016-10-19T08:04:15.246Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-10-19T08:04:15.543Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 17,
      "updated_at": "2016-10-19T08:04:15.543Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-19T08:04:15.838Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 18,
      "updated_at": "2016-10-19T08:04:15.838Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00c97d824e7d15a9ecd7d7552f24360841ea4187c17e3c731c7cda11727d0455"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/2
Content-Type: application/json
Authorization: Bearer 83ae3f0d02b5503ddd44a046d29bb779227499c97d7d534074aaefb2bec03bd9
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-19T07:54:13.000Z"}}
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
    "created_at": "2016-10-19T08:04:13.492Z",
    "read_at": "2016-10-19T07:54:13.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-10-19T08:04:13.552Z",
    "author_id": "74",
    "thread_subject_id": "20",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/2" -d '{"notification":{"read_at":"2016-10-19T07:54:13.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83ae3f0d02b5503ddd44a046d29bb779227499c97d7d534074aaefb2bec03bd9"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 60e307f290b3b985bc999e1abebbed4117041022fd2bf61a40f2cc7947bcc455
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
      "course_id": 121,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T08:04:46.319Z",
      "course_published": true,
      "updated_at": "2016-10-19T08:04:46.313Z"
    },
    {
      "id": 7,
      "course_id": 122,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T08:04:46.391Z",
      "course_published": true,
      "updated_at": "2016-10-19T08:04:46.385Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60e307f290b3b985bc999e1abebbed4117041022fd2bf61a40f2cc7947bcc455"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 55c2bec6e9035bedd7595458744baeeb731a40ced281e383aaf2b0bf032dc4ca
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
    "course_id": 117,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T08:04:45.832Z",
    "course_published": true,
    "updated_at": "2016-10-19T08:04:45.825Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55c2bec6e9035bedd7595458744baeeb731a40ced281e383aaf2b0bf032dc4ca"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 8e0715b364c682416e0a231e335f42af3c4ec5f44a381b2139930109d6b4f066
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
    "course_id": 120,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-19T08:04:46.198Z",
    "course_published": true,
    "updated_at": "2016-10-19T08:04:46.188Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e0715b364c682416e0a231e335f42af3c4ec5f44a381b2139930109d6b4f066"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3cf3b91cba1aef115920229acea9c89493864dce7f82bc72dc65944bf0b1b1f3
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
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 818
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 124,
      "user_id": 818
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 125,
      "user_id": 818
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 126,
      "user_id": 818
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3cf3b91cba1aef115920229acea9c89493864dce7f82bc72dc65944bf0b1b1f3"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/78
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
    "id": 78,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 78,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 78
      },
      {
        "id": 79,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 78
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/78" -X GET \
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
      "id": 79,
      "name": "Cross-group fresh-thinking superstructure",
      "name_translations": {
        "en": "Cross-group fresh-thinking superstructure"
      }
    },
    {
      "id": 80,
      "name": "Future-proofed multi-state conglomeration",
      "name_translations": {
        "en": "Future-proofed multi-state conglomeration"
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
Authorization: Bearer 762054435b39d137ae625941bedb6cf7d0b8bdced82fc3664af9e0243b7e1569
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
    "user_id": 113,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-19T08:04:16.607Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 762054435b39d137ae625941bedb6cf7d0b8bdced82fc3664af9e0243b7e1569"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer 563d85eb285a6c458388c788a9411011f22061c3f7ed0580990a8436a08be115
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
    "id": 5,
    "user_id": 128,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-19T08:04:17.286Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 563d85eb285a6c458388c788a9411011f22061c3f7ed0580990a8436a08be115"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/27
Content-Type: application/json
Authorization: Bearer e73ad1ae23084386835308879b43e2551fe0fb81c69772e60261e0a6ea0fa434
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
    "id": 27,
    "user_id": 224,
    "feedbackable_id": 12,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T08:04:24.435Z",
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
curl "api.goskive.com/v2/feedbacks/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e73ad1ae23084386835308879b43e2551fe0fb81c69772e60261e0a6ea0fa434"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer e97ec36922171f01c98b08af02de5b48e19cd8b82a16ed94ad4e7c48eb21f280
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
	-H "Authorization: Bearer e97ec36922171f01c98b08af02de5b48e19cd8b82a16ed94ad4e7c48eb21f280"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer ef1d21fc80595e333c0bda0a23ccf21a89411c04b5e0e5e294129ec641164ae7
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
	-H "Authorization: Bearer ef1d21fc80595e333c0bda0a23ccf21a89411c04b5e0e5e294129ec641164ae7"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/7/fix
Content-Type: application/json
Authorization: Bearer d923b46e5ded761fec97ca0ab916f1b4ec8abee5421948bc9c66dfcfd8a1dc16
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
curl "api.goskive.com/v2/feedbacks/7/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d923b46e5ded761fec97ca0ab916f1b4ec8abee5421948bc9c66dfcfd8a1dc16"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer eb5370f02510e8d6772d34b1c10a4b4ffae8f59d5f9b680ca6097c41d0245e89
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
    "id": 28,
    "user_id": 229,
    "feedbackable_id": 13,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T08:04:24.721Z",
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
curl "api.goskive.com/v2/feedbacks/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb5370f02510e8d6772d34b1c10a4b4ffae8f59d5f9b680ca6097c41d0245e89"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 28e4bfbec8a4f12ca31c93af484fe55c34b0a065fa971d084fa1b54328f5d1e1
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
	-H "Authorization: Bearer 28e4bfbec8a4f12ca31c93af484fe55c34b0a065fa971d084fa1b54328f5d1e1" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer ccba1c48b023e89a62aa47711177c334b625547ba6f7ab824ddec221b278f6d6
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
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Authorization: Bearer ccba1c48b023e89a62aa47711177c334b625547ba6f7ab824ddec221b278f6d6" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/3
Authorization: Bearer f72e7072beaa17e84405190c871ba4af269b745a19e392b1f33f62d72ecc8d49
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/efcbdd30f2f1e01f2f5c6358f7877612.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T080459Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=713bea93d711c9f381c39d1701d39f934f60073838867becd703303d3a37a060"
  }
}
```



```shell
curl "api.goskive.com/v2/files/3" -X GET \
	-H "Authorization: Bearer f72e7072beaa17e84405190c871ba4af269b745a19e392b1f33f62d72ecc8d49"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Authorization: Bearer 8d393fdb2cd7de0fe5202b22f11d8c528afd6f6ef9d9cbb412b9536919e91df4
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
    "id": 9,
    "uploader": {
      "id": 667,
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
      "created_at": "2016-10-19T08:05:00.560Z",
      "updated_at": "2016-10-19T08:05:00.560Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-19T08:05:00.626Z",
    "updated_at": "2016-10-19T08:05:00.626Z",
    "course_id": 184,
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
curl "api.goskive.com/v2/files/9/metadata" -X GET \
	-H "Authorization: Bearer 8d393fdb2cd7de0fe5202b22f11d8c528afd6f6ef9d9cbb412b9536919e91df4" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer 0ee4adc0a60464dc29786e6a1fdb32b131a5bbb822c6ea99f7a31a25b7bf85d5
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
      "creator_id": 285,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 78,
      "additional_university_ids": [

      ],
      "topic_id": 83,
      "discipline_id": 84,
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
      "chapters_updated_at": "2016-10-19T08:04:29.695Z",
      "updated_at": "2016-10-19T08:04:31.506Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 290,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-90e9dd54-5c67-4937-bd5b-a35216fb29c2",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-90e9dd54-5c67-4937-bd5b-a35216fb29c2",
      "slug": "mit-the-great-british-bake-off-90e9dd54-5c67-4937-bd5b-a35216fb29c2",
      "university_id": 79,
      "additional_university_ids": [

      ],
      "topic_id": 84,
      "discipline_id": 85,
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
      "chapters_updated_at": "2016-10-19T08:04:29.695Z",
      "updated_at": "2016-10-19T08:04:32.149Z",
      "shortname": "mit-the-great-british-bake-off-90e9dd54-5c67-4937-bd5b-a35216fb29c2"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 0ee4adc0a60464dc29786e6a1fdb32b131a5bbb822c6ea99f7a31a25b7bf85d5"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/10/preview
Authorization: Bearer 4254e4f97d2a08b34a43f2e8575fcd7c40974d83a5e28c0c7b42e017958ec348
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/c9b172fc02a8aa7a5807bd1930c62676.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T080500Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=4a4cc9d8c2713a00d4ca8fe87f80e7e591d4b39e157f1c6155defd38dbdf3335"
  }
}
```



```shell
curl "api.goskive.com/v2/files/10/preview" -X GET \
	-H "Authorization: Bearer 4254e4f97d2a08b34a43f2e8575fcd7c40974d83a5e28c0c7b42e017958ec348"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/11/report
Authorization: Bearer 4e8208a5e2dbb0228082b7b590f6349c19fa8304f31d3906e490c6e770974bc2
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
	-H "Authorization: Bearer 4e8208a5e2dbb0228082b7b590f6349c19fa8304f31d3906e490c6e770974bc2" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/23/comments
Content-Type: application/json
Authorization: Bearer 76834a9c2dbc8114a684e0dcf282ea68937af1b747cde722bc9dd2d76aebe562
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
    "id": 14,
    "author_id": 423,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:04:43.191Z",
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
curl "api.goskive.com/v2/flashcards/23/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76834a9c2dbc8114a684e0dcf282ea68937af1b747cde722bc9dd2d76aebe562"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/25/comments
Content-Type: application/json
Authorization: Bearer 02e2ca5e409a91beea58b8b47818b18bbdd6438ef7c7450cfef60cca34a1e076
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
    "author_id": 429,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:04:43.643Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 30,
      "user_id": 429,
      "feedbackable_id": 25,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:43.640Z",
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
curl "api.goskive.com/v2/flashcards/25/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02e2ca5e409a91beea58b8b47818b18bbdd6438ef7c7450cfef60cca34a1e076"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/22/comments
Content-Type: application/json
Authorization: Bearer cbba5d387e3005164823ba0665ab48c386ce5821c5bc263e88de912ede28842f
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
      "author_id": 422,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:04:42.975Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 421,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:04:42.959Z",
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
	-H "Authorization: Bearer cbba5d387e3005164823ba0665ab48c386ce5821c5bc263e88de912ede28842f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/24/comments
Content-Type: application/json
Authorization: Bearer 7337d842afe41d6fb0515150012f0eb27ebf44a2fe93b677bae71185addee05c
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
curl "api.goskive.com/v2/flashcards/24/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7337d842afe41d6fb0515150012f0eb27ebf44a2fe93b677bae71185addee05c"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/32/feedbacks
Content-Type: application/json
Authorization: Bearer cc4d63e8aa9892119072cd8d8fff72089acf9960f62ff4b90e62f20f0ebbb82e
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
    "user_id": 465,
    "feedbackable_id": 32,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T08:04:45.298Z",
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
curl "api.goskive.com/v2/flashcards/32/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc4d63e8aa9892119072cd8d8fff72089acf9960f62ff4b90e62f20f0ebbb82e"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/30/feedbacks
Content-Type: application/json
Authorization: Bearer 0593441f6286c6e585d1a5acd409ed0a6a8cefdfa80da18f6859594bd11a06fe
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
      "id": 36,
      "user_id": 461,
      "feedbackable_id": 30,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:44.952Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 460,
      "feedbackable_id": 30,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:44.942Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/30/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0593441f6286c6e585d1a5acd409ed0a6a8cefdfa80da18f6859594bd11a06fe"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/35/votes
Content-Type: application/json
Authorization: Bearer b0d4e66a67d10036263e9c785476dcbe82ff37dbc85c09bfae8c314335d18143
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
      "votable_id": 35,
      "user_id": 491
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 35,
      "user_id": 490
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 35,
      "user_id": 489
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/35/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0d4e66a67d10036263e9c785476dcbe82ff37dbc85c09bfae8c314335d18143"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/67/republish
Content-Type: application/json
Authorization: Bearer 10904cbce2fc876bdad5a1f49d202674e7bc35e8157ce7f9dae5172f12cb4b89
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
curl "api.goskive.com/v2/flashcards/67/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10904cbce2fc876bdad5a1f49d202674e7bc35e8157ce7f9dae5172f12cb4b89"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/86/bookmark
Content-Type: application/json
Authorization: Bearer 71acf4d05bd2d8fde8b924cd343dce3333567028556461e85bf59e4eba19cbd7
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/86/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71acf4d05bd2d8fde8b924cd343dce3333567028556461e85bf59e4eba19cbd7"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/69
Content-Type: application/json
Authorization: Bearer 9f20a0b167e34d2805a86ede202492c19ac85636479f2f42694932cce9f61394
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f20a0b167e34d2805a86ede202492c19ac85636479f2f42694932cce9f61394"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/66/downvote
Content-Type: application/json
Authorization: Bearer e96ae1839e576c4414a444bc83e925407e547a81789e80c64ef2925736fd1b5c
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e96ae1839e576c4414a444bc83e925407e547a81789e80c64ef2925736fd1b5c"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/85
Content-Type: application/json
Authorization: Bearer f4f62481684560b0499a7373f46cde41e649cd126290d266646ae7cd1864e602
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
    "id": 85,
    "obfuscated_id": "xR5KgQjIo2Y",
    "author_id": 636,
    "chapter_id": 146,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:04:59.125Z",
    "created_at": "2016-10-19T08:04:59.125Z",
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
curl "api.goskive.com/v2/flashcards/85" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4f62481684560b0499a7373f46cde41e649cd126290d266646ae7cd1864e602"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/report
Content-Type: application/json
Authorization: Bearer 68767664ceece58953d6475361a9ba217ccd3f2aaacebed4ddb545fe02d7daff
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
	-H "Authorization: Bearer 68767664ceece58953d6475361a9ba217ccd3f2aaacebed4ddb545fe02d7daff"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/63/bookmark
Content-Type: application/json
Authorization: Bearer b6279ba1b165380958a9a6bbd3e610777ea8534aaeea70b671d0c33f6e89ca48
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6279ba1b165380958a9a6bbd3e610777ea8534aaeea70b671d0c33f6e89ca48"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/upvote
Content-Type: application/json
Authorization: Bearer 61bf78980e93c3a6c80401add7bb2ecd04f26f171d12a743bee96994005428ee
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61bf78980e93c3a6c80401add7bb2ecd04f26f171d12a743bee96994005428ee"
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
    "key": "cache/4d3e3459e07e8d181bb64b6e0347cd1d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQwOTowNDoyNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS80ZDNlMzQ1OWUwN2U4ZDE4MWJiNjRiNmUwMzQ3Y2QxZC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE5L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOVQwODA0MjZaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T080426Z",
    "x-amz-signature": "f40d700914adb161ceaafa28a21cc9df2ca3a8f3df7c140b3898b11e26d5185e"
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
Authorization: Bearer a98a2d399ddcb3a600e22520325698ece510ea9cd3c85153167158f3046103f0
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
curl "api.goskive.com/v2/me/jobs/2/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a98a2d399ddcb3a600e22520325698ece510ea9cd3c85153167158f3046103f0"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 0d6dfa41abb9c5314aef8a28ee7edb694a6c46f1cd76042617e7cc7c1ecf7045
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
	-H "Authorization: Bearer 0d6dfa41abb9c5314aef8a28ee7edb694a6c46f1cd76042617e7cc7c1ecf7045"
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
{"password":{"reset_password_token":"SVCVL5q_i47KYxixpwTz","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 324,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-19T08:04:36.420Z",
  "updated_at": "2016-10-19T08:04:36.556Z",
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
  "audit_id": 3311
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"SVCVL5q_i47KYxixpwTz","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Authorization: Bearer 2b83f5dd4b9c5926d95901d18e9fe22a5d10c49b359e1f0e53ca667ce9dc1be8
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
    "author_id": 304,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:04:33.388Z",
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
	-H "Authorization: Bearer 2b83f5dd4b9c5926d95901d18e9fe22a5d10c49b359e1f0e53ca667ce9dc1be8"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/53/comments
Content-Type: application/json
Authorization: Bearer 3040a069e57e0f17a2d621df1af1d4b58078e547eaadd0fb105ad026fd400c7c
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
    "id": 5,
    "author_id": 301,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:04:32.878Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 29,
      "user_id": 301,
      "feedbackable_id": 53,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:04:32.875Z",
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
	-H "Authorization: Bearer 3040a069e57e0f17a2d621df1af1d4b58078e547eaadd0fb105ad026fd400c7c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/56/comments
Content-Type: application/json
Authorization: Bearer 3fe91119aa540b3a71c61af98643f28ae49b321c11b45506570c34cc75bf9c86
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
      "author_id": 314,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:04:34.217Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 313,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:04:34.201Z",
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
curl "api.goskive.com/v2/questions/56/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fe91119aa540b3a71c61af98643f28ae49b321c11b45506570c34cc75bf9c86"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/55/comments
Content-Type: application/json
Authorization: Bearer 3feb1224e09161a800ab0dc6470b657b7e258e4b6a46aee327ae03d3f4fbd6d2
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
	-H "Authorization: Bearer 3feb1224e09161a800ab0dc6470b657b7e258e4b6a46aee327ae03d3f4fbd6d2"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/127/feedbacks
Content-Type: application/json
Authorization: Bearer 8db9b72947c3396fad7818721c64927e730902a4a98dea8141c7115d7ee1a1a4
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
    "user_id": 832,
    "feedbackable_id": 127,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-19T08:05:15.550Z",
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
curl "api.goskive.com/v2/questions/127/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8db9b72947c3396fad7818721c64927e730902a4a98dea8141c7115d7ee1a1a4"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/133/feedbacks
Content-Type: application/json
Authorization: Bearer 001cf82c0d841bfc1292beac4d2a955f46b8370f74c44992427e5ed03dad241d
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
      "user_id": 864,
      "feedbackable_id": 133,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:05:17.667Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 863,
      "feedbackable_id": 133,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:05:17.656Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/133/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 001cf82c0d841bfc1292beac4d2a955f46b8370f74c44992427e5ed03dad241d"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/1/votes
Content-Type: application/json
Authorization: Bearer 923e3334e7d2f0cd22b1ba2eeea3775a1baa2898b999d6f83a4f6a4689a0a835
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
      "user_id": 11
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 10
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 9
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/1/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 923e3334e7d2f0cd22b1ba2eeea3775a1baa2898b999d6f83a4f6a4689a0a835"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/116/republish
Content-Type: application/json
Authorization: Bearer 07871b89f4b40e0e84f2fe41d1ce02bd2f9a188041b9374b1e460477e32b5c04
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
curl "api.goskive.com/v2/questions/116/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07871b89f4b40e0e84f2fe41d1ce02bd2f9a188041b9374b1e460477e32b5c04"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/114/bookmark
Content-Type: application/json
Authorization: Bearer 08d7d4b4653a71d0a326268411f45a18f781eb1682fc21ed46f25183c4969eeb
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08d7d4b4653a71d0a326268411f45a18f781eb1682fc21ed46f25183c4969eeb"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/113
Content-Type: application/json
Authorization: Bearer 4bc8210bbce494ad9a2e6e96a5170ea0207aa34fd2c094fa21e91e77f8a42418
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/113" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4bc8210bbce494ad9a2e6e96a5170ea0207aa34fd2c094fa21e91e77f8a42418"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/118/downvote
Content-Type: application/json
Authorization: Bearer d5bb2cf85fac02e97a9173dcac5b5ddd2fc6d5ec321a88b995d18af5bc84be96
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/118/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5bb2cf85fac02e97a9173dcac5b5ddd2fc6d5ec321a88b995d18af5bc84be96"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/120
Content-Type: application/json
Authorization: Bearer 9a1db302694ae86321f2385ccb2011b40c394ffa0db50230341914496496f977
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
    "id": 120,
    "obfuscated_id": "vEr9LtFjURM",
    "author_id": 795,
    "chapter_id": 181,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:05:12.086Z",
    "created_at": "2016-10-19T08:05:11.978Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 242,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 243,
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
curl "api.goskive.com/v2/questions/120" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a1db302694ae86321f2385ccb2011b40c394ffa0db50230341914496496f977"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/119/report
Content-Type: application/json
Authorization: Bearer 456e31581341f376db5956979b019218f1fcf52697c7a894f604ac274c4ab383
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/119/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 456e31581341f376db5956979b019218f1fcf52697c7a894f604ac274c4ab383"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/115/bookmark
Content-Type: application/json
Authorization: Bearer 6c4973ba2c89e182ce8a024a4cb4dd4f3387930ba14c9a3dd856953639b68100
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c4973ba2c89e182ce8a024a4cb4dd4f3387930ba14c9a3dd856953639b68100"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/121
Content-Type: application/json
Authorization: Bearer 45d8021ba36b8756e52685781b2c470547d6edf4bdfee893fbe10a97ecbc4136
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":121,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T08:05:12.291Z","updated_at":"2016-10-19T08:05:12.399Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":182,"author_id":798,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 121,
    "obfuscated_id": "LQhaXfRg6ZA",
    "author_id": 798,
    "chapter_id": 182,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:05:12.499Z",
    "created_at": "2016-10-19T08:05:12.291Z",
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
    "question": "{\"id\"=>121, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-19T08:05:12.291Z\", \"updated_at\"=>\"2016-10-19T08:05:12.399Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>182, \"author_id\"=>798, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 244,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 245,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 246,
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
curl "api.goskive.com/v2/questions/121" -d '{"question":{"question":{"id":121,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T08:05:12.291Z","updated_at":"2016-10-19T08:05:12.399Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":182,"author_id":798,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45d8021ba36b8756e52685781b2c470547d6edf4bdfee893fbe10a97ecbc4136"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/122/upvote
Content-Type: application/json
Authorization: Bearer 164fb9386bf37b6b190cb030c2fdf1b1cb528757fa2ff3cda382e7b235d6e569
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/122/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 164fb9386bf37b6b190cb030c2fdf1b1cb528757fa2ff3cda382e7b235d6e569"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer ad37000971ede7184c115a3e965a3bcf428c691335669f18337368e04fb23d7c
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
      "creator_id": 3,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "topic_id": 2,
      "discipline_id": 2,
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
      "updated_at": "2016-10-19T08:04:07.154Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad37000971ede7184c115a3e965a3bcf428c691335669f18337368e04fb23d7c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer eaae3b4e0b9a9fbe95f5194deca24c752bd88bc55fb8895f27a2fab0dbf06589
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
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "National School of Pizza",
      "short_name": "Uni 2",
      "acronym": "NSPI",
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
      "updated_at": "2016-10-19T08:04:06.862Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 1,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-1",
      "html_url": "https://goskive.com/university/uni-1",
      "slug": "uni-1",
      "name": "National School of Pastry",
      "short_name": "Uni 1",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/38802f33528ba3ba141b3ec7e7bce0a2b851ee78.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51291693f690a69f7677e03637596dc7709b266f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:04:06.844Z",
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
	-H "Authorization: Bearer eaae3b4e0b9a9fbe95f5194deca24c752bd88bc55fb8895f27a2fab0dbf06589"
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
      "id": 8,
      "name": "Future-proofed demand-driven capacity",
      "name_translations": {
        "en": "Future-proofed demand-driven capacity"
      },
      "discipline_id": 8
    },
    {
      "id": 9,
      "name": "Robust demand-driven time-frame",
      "name_translations": {
        "en": "Robust demand-driven time-frame"
      },
      "discipline_id": 9
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
GET /v2/topics/10
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
    "id": 10,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 10
  }
}
```



```shell
curl "api.goskive.com/v2/topics/10" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer e9552c0a5956b99c05b1ebe8c4b121a3ee6a27238c13b8ea818f79b47d2f41be
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
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-9",
      "html_url": "https://goskive.com/university/uni-9",
      "slug": "uni-9",
      "name": "University 4",
      "short_name": "Uni 9",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/87ba84ab1107072a961e4e0676ef38b11ea6bc3e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b1af93f712353ded5aa14b0defbbe8f407c0d997.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:04:08.884Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 12,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-10",
      "html_url": "https://goskive.com/university/uni-10",
      "slug": "uni-10",
      "name": "University 5",
      "short_name": "Uni 10",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5bcbb5f32f57a2edaadd2dbcddd13bce2e6da770.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/35e26355049fa64a351bfa2fbc72aee98aac48f5.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:04:08.899Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 13,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-11",
      "html_url": "https://goskive.com/university/uni-11",
      "slug": "uni-11",
      "name": "University 6",
      "short_name": "Uni 11",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0807ab42117f07e0ba6d1aca79325e2f65ec600d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1203abbdb8e1c4445cac833cf83747bef4ae8006.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:04:08.915Z",
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
	-H "Authorization: Bearer e9552c0a5956b99c05b1ebe8c4b121a3ee6a27238c13b8ea818f79b47d2f41be"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 0697bb22dede247f1243662fa977f00ffa4107bd2a8c536cc85d0377059ce799
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
    "id": 10,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/907b97acad454546ae110f7cad7c8a133f868482.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/590c7f8b9d9c518ab5b695e676ac1e98a5606cc2.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-19T08:04:08.795Z",
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
	-H "Authorization: Bearer 0697bb22dede247f1243662fa977f00ffa4107bd2a8c536cc85d0377059ce799"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 30208a2a53f866f00c5b9cead48c9c1e639add6f9113fbc0873ad49c2b967ea5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":236,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 720,
    "id": 224,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 209,
    "additional_university_ids": [

    ],
    "topic_id": 236,
    "discipline_id": 237,
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
    "chapters_updated_at": "2016-10-19T08:05:04.683Z",
    "updated_at": "2016-10-19T08:05:04.811Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 156,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-19T08:05:04.770Z",
        "course_id": 224,
        "author_id": 720,
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
        "id": 157,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-19T08:05:04.786Z",
        "course_id": 224,
        "author_id": 720,
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
        "id": 158,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-19T08:05:04.802Z",
        "course_id": 224,
        "author_id": 720,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":236,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30208a2a53f866f00c5b9cead48c9c1e639add6f9113fbc0873ad49c2b967ea5"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cafc27b4dce849a3dab2584edc7e69eb0e95053241d3fe56ee36175981665aaa
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":237,"published":false}}
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
    "creator_id": 721,
    "id": 225,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 210,
    "additional_university_ids": [

    ],
    "topic_id": 237,
    "discipline_id": 238,
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
    "updated_at": "2016-10-19T08:05:04.961Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":237,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cafc27b4dce849a3dab2584edc7e69eb0e95053241d3fe56ee36175981665aaa"
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
      "creator_id": 684,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 197,
      "additional_university_ids": [

      ],
      "topic_id": 206,
      "discipline_id": 207,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "updated_at": "2016-10-19T08:05:01.768Z",
      "shortname": "fu-course-126"
    },
    {
      "creator_id": 684,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 197,
      "additional_university_ids": [

      ],
      "topic_id": 207,
      "discipline_id": 208,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "chapters_updated_at": "2016-10-19T08:05:02.032Z",
      "updated_at": "2016-10-19T08:05:02.038Z",
      "shortname": "fu-course-127"
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
Authorization: Bearer bef880b50458ecf09633f5d6fcc8b89abaed429e23cb14d08d6a6a009e77fabd
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
      "creator_id": 701,
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 203,
      "additional_university_ids": [

      ],
      "topic_id": 222,
      "discipline_id": 223,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "updated_at": "2016-10-19T08:05:03.244Z",
      "shortname": "fu-course-142"
    },
    {
      "creator_id": 701,
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-143",
      "html_url": "https://goskive.com/course/fu-course-143",
      "slug": "fu-course-143",
      "university_id": 203,
      "additional_university_ids": [

      ],
      "topic_id": 223,
      "discipline_id": 224,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
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
      "chapters_updated_at": "2016-10-19T08:05:03.507Z",
      "updated_at": "2016-10-19T08:05:03.513Z",
      "shortname": "fu-course-143"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bef880b50458ecf09633f5d6fcc8b89abaed429e23cb14d08d6a6a009e77fabd"
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
      "creator_id": 689,
      "id": 198,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 198,
      "additional_university_ids": [

      ],
      "topic_id": 210,
      "discipline_id": 211,
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
      "updated_at": "2016-10-19T08:05:02.202Z",
      "shortname": "fu-course-130"
    },
    {
      "creator_id": 689,
      "id": 199,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 198,
      "additional_university_ids": [

      ],
      "topic_id": 211,
      "discipline_id": 212,
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
      "updated_at": "2016-10-19T08:05:02.238Z",
      "shortname": "fu-course-131"
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
Authorization: Bearer af57baf8736623e481ff516a9cced1f605a97054d833e37bf4e961269e4616e8
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
      "creator_id": 707,
      "id": 214,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 204,
      "additional_university_ids": [

      ],
      "topic_id": 226,
      "discipline_id": 227,
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
      "updated_at": "2016-10-19T08:05:03.713Z",
      "shortname": "fu-course-146"
    },
    {
      "creator_id": 707,
      "id": 215,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 204,
      "additional_university_ids": [

      ],
      "topic_id": 227,
      "discipline_id": 228,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
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
      "updated_at": "2016-10-19T08:05:03.749Z",
      "shortname": "fu-course-147"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af57baf8736623e481ff516a9cced1f605a97054d833e37bf4e961269e4616e8"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 059ae9b03dd15e4594549ee13ee915df7db8a02620a6bf9db5ef8a1c814c9f76
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
  "id": 272,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-19T08:04:29.361Z",
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
	-H "Authorization: Bearer 059ae9b03dd15e4594549ee13ee915df7db8a02620a6bf9db5ef8a1c814c9f76"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/70
Content-Type: application/json
Authorization: Bearer 44fb218278b4c8673ea6d8adb764c5b65a2baf32a2b683bdbd16a680f9dd2d62
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
    "id": 70,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 26,
    "fields_of_study": [
      23,
      24
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-19T08:04:13.302Z",
    "updated_at": "2016-10-19T08:04:13.302Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/70" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44fb218278b4c8673ea6d8adb764c5b65a2baf32a2b683bdbd16a680f9dd2d62"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/68
Content-Type: application/json
Authorization: Bearer a915f5627fe7652540300af42c95cc6ad3e88e6051ccf2e372796c0175a05949
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
    "id": 68,
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
    "created_at": "2016-10-19T08:04:13.136Z",
    "updated_at": "2016-10-19T08:04:13.136Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/68" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a915f5627fe7652540300af42c95cc6ad3e88e6051ccf2e372796c0175a05949"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/6
Content-Type: application/json
Authorization: Bearer 115c48f8b8b4998584e457a6d2c46c3cf16e11677d9e50129db4e2780a648452
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 115c48f8b8b4998584e457a6d2c46c3cf16e11677d9e50129db4e2780a648452"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/7
Content-Type: application/json
Authorization: Bearer 5aa149d8715a94826a2adf79f17d73da541eecc3e24962d66d836411e4a9c7f7
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
    "id": 7,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 6,
    "user_id": 30
  }
}
```



```shell
curl "api.goskive.com/v2/votes/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5aa149d8715a94826a2adf79f17d73da541eecc3e24962d66d836411e4a9c7f7"
```
