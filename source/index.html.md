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
Authorization: Basic NGJiNGVkOWM4ODZhZjlmY2VhZDE2Yjc3NWFmZTVlYzM4YjAyYWVjMzdjMWRh
NDM3MzBiYTk1YTNkNWE4MjkyMTo1YTdlNzU0ZmQzM2I3NTcwZTk5YjlmY2Jj
NzQxN2UyNDA2MzZiNmFjZmU5NWE4NTI0NzhiZmVkMDA5Mjg1ODFm

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
	-u 4bb4ed9c886af9fcead16b775afe5ec38b02aec37c1da43730ba95a3d5a82921:5a7e754fd33b7570e99b9fcbc7417e240636b6acfe95a852478bfed00928581f
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c0a5e07e3b36bd5222b166a00f54e99677e4cce3cfb882ec47149ac07f7f7fb6","client_secret":"2638b7039a11102eb0a86c0eddd3b5aac9e141681e0b9991f98910bed08071a0"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c0a5e07e3b36bd5222b166a00f54e99677e4cce3cfb882ec47149ac07f7f7fb6","client_secret":"2638b7039a11102eb0a86c0eddd3b5aac9e141681e0b9991f98910bed08071a0"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"2f9c0f356585abab07e890593eb11cc5fec7dd34ae4154a48d6ca93e0008205e","client_secret":"cb459f7304d8c4850874380fd7e1c25a84518a2320b335e32dfc7737fd810429"}
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
  "access_token": "835a0f7a7edfc1c81bc6691e2a3711de3286b38e40553df3a547c17db052847a",
  "token_type": "bearer",
  "created_at": 1481734093
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"2f9c0f356585abab07e890593eb11cc5fec7dd34ae4154a48d6ca93e0008205e","client_secret":"cb459f7304d8c4850874380fd7e1c25a84518a2320b335e32dfc7737fd810429"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YzFkZjI2YmVmMzQ3MzA0MzYzM2JiZjAxZTk4MTE2ZjBlNzQwNGZiMjBiNDZl
OTkyYWI2ZTJhOWIzZDY1M2M5ZTo5OTg2MGVkZDVhZDQ2YzdiNDMzNjQ5ZTll
ZmQ1MmU0ZGRjYWFkNTM5MzUzY2NkMTA5ZmIzYjQwYjgwNjhlMjBm

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
  "access_token": "b5f3ac05ad17dd7cda627f5a5aeae71171cafaa79fb179ccdc3bf3064842f219",
  "token_type": "bearer",
  "created_at": 1481734093
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u c1df26bef3473043633bbf01e98116f0e7404fb20b46e992ab6e2a9b3d653c9e:99860edd5ad46c7b433649e9efd52e4ddcaad539353ccd109fb3b40b8068e20f
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"39bc6c7bf5c06bf2357b919f15181b94704bbfd96e1e92c82d8e79ab6b678589","client_secret":"b3c8709f5770567330280370c0c83397927c0dc3119337360b942cb477882b61"}
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
  "access_token": "2df93ffe45833a874a38c829f52b1f7bbcf52795ffd786aac06aa3e300c48cad",
  "token_type": "bearer",
  "created_at": 1481734094
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"39bc6c7bf5c06bf2357b919f15181b94704bbfd96e1e92c82d8e79ab6b678589","client_secret":"b3c8709f5770567330280370c0c83397927c0dc3119337360b942cb477882b61"}' -X POST \
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
GET /v2/campaigns/4
Content-Type: application/json
Authorization: Bearer deb508f58a35a1e5b6aed53831bed064f14b343f92032e6816f0aa13cb148eb5
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
    "company_id": 16,
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
	-H "Authorization: Bearer deb508f58a35a1e5b6aed53831bed064f14b343f92032e6816f0aa13cb148eb5"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/195/flashcards
Content-Type: application/json
Authorization: Bearer 74d46e185ff6ee0dfdf4647bf782263713e7d5fe77a635a9c1e0822471b1aed5
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
    "author_id": 974,
    "chapter_id": 195,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:48:12.309Z",
    "created_at": "2016-12-14T16:48:12.309Z",
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
	-H "Authorization: Bearer 74d46e185ff6ee0dfdf4647bf782263713e7d5fe77a635a9c1e0822471b1aed5"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer 8d5250635e4bd613d745e10c43f13136b7825d36cd058a3c808ba320c619cf13
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
      "author_id": 969,
      "chapter_id": 194,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:48:12.007Z",
      "created_at": "2016-12-14T16:48:12.007Z",
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
      "author_id": 969,
      "chapter_id": 194,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:48:12.046Z",
      "created_at": "2016-12-14T16:48:12.046Z",
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
      "author_id": 969,
      "chapter_id": 194,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:48:12.085Z",
      "created_at": "2016-12-14T16:48:12.085Z",
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
	-H "Authorization: Bearer 8d5250635e4bd613d745e10c43f13136b7825d36cd058a3c808ba320c619cf13"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/66/questions
Content-Type: application/json
Authorization: Bearer d00de1d78c1026e7db7822a9e9a1c427b32a24c8a4a87968da355b49cf025a5e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":66,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 38,
    "obfuscated_id": "8_YCqPYFnsI",
    "author_id": 231,
    "chapter_id": 66,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:11.241Z",
    "created_at": "2016-12-14T16:47:11.241Z",
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
        "id": 76,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 77,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 78,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 79,
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
curl "api.goskive.com/v2/chapters/66/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":66,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d00de1d78c1026e7db7822a9e9a1c427b32a24c8a4a87968da355b49cf025a5e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/64/questions
Content-Type: application/json
Authorization: Bearer 3095fd5d3fe15f196696da817a43154f6757c318eb36f6034252088c82894e24
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":64,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 36,
    "obfuscated_id": "01Tx8eTrCOA",
    "author_id": 225,
    "chapter_id": 64,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:10.163Z",
    "created_at": "2016-12-14T16:47:10.163Z",
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
        "id": 72,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 73,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/64/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":64,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3095fd5d3fe15f196696da817a43154f6757c318eb36f6034252088c82894e24"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/65/questions
Content-Type: application/json
Authorization: Bearer 8c5f3df76b747950b6258b6847eca492e4ad054dc2b1b65d68f005bfe8ca70d8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":65,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 37,
    "obfuscated_id": "95m_4XdR9PU",
    "author_id": 228,
    "chapter_id": 65,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:10.698Z",
    "created_at": "2016-12-14T16:47:10.698Z",
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
        "id": 74,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 75,
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
curl "api.goskive.com/v2/chapters/65/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":65,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c5f3df76b747950b6258b6847eca492e4ad054dc2b1b65d68f005bfe8ca70d8"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/67/questions
Content-Type: application/json
Authorization: Bearer 8b4815cdb262584b0988fdb5483b6c8e021771416c2eb9fd116c9cd2d846543f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":67,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 234,
    "chapter_id": 67,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:11.895Z",
    "created_at": "2016-12-14T16:47:11.895Z",
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
        "id": 80,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 81,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 82,
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
curl "api.goskive.com/v2/chapters/67/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":67,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b4815cdb262584b0988fdb5483b6c8e021771416c2eb9fd116c9cd2d846543f"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/62/questions
Content-Type: application/json
Authorization: Bearer 2a4c5dacabd3d3a19454f206be7e05ae10a1ccc50a20a107ef3fbab8bd0892a7
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 216,
      "chapter_id": 62,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:09.384Z",
      "created_at": "2016-12-14T16:47:09.293Z",
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
          "id": 66,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 67,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 217,
      "chapter_id": 62,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:09.544Z",
      "created_at": "2016-12-14T16:47:09.453Z",
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
          "id": 68,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 69,
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
      "author_id": 218,
      "chapter_id": 62,
      "position": 26,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:09.716Z",
      "created_at": "2016-12-14T16:47:09.617Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/62/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a4c5dacabd3d3a19454f206be7e05ae10a1ccc50a20a107ef3fbab8bd0892a7"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/141
Content-Type: application/json
Authorization: Bearer e0b583d7950f9ab669f526ae057bd5f67ca2b1ac0fdad020a4d2352b6ea9ca80
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
curl "api.goskive.com/v2/chapters/141" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0b583d7950f9ab669f526ae057bd5f67ca2b1ac0fdad020a4d2352b6ea9ca80"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/143
Content-Type: application/json
Authorization: Bearer f21001ace6f70caa88e6b326d193e0555fa72d7e8d7f76faf6f1984bfe77e518
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
curl "api.goskive.com/v2/chapters/143" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f21001ace6f70caa88e6b326d193e0555fa72d7e8d7f76faf6f1984bfe77e518"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/147
Content-Type: application/json
Authorization: Bearer 8190f2cd51ed941940b567b3be58d190d3000ced496803b0101a428d30a39fc8
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
curl "api.goskive.com/v2/chapters/147" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8190f2cd51ed941940b567b3be58d190d3000ced496803b0101a428d30a39fc8"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/144
Content-Type: application/json
Authorization: Bearer 418fe79315058af550347cade67f16b260f03c37150cdae2c27655ddc296478e
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/144" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 418fe79315058af550347cade67f16b260f03c37150cdae2c27655ddc296478e"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/139
Content-Type: application/json
Authorization: Bearer 7620a44eb3d336638a9189f9fdcc17fb749f2725466c45005483450a6d1cb359
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
    "id": 139,
    "updated_at": "2016-12-14T16:47:42.101Z",
    "course_id": 200,
    "author_id": 617,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-14T16:47:41.514Z",
    "questions_updated_at": "2016-12-14T16:47:41.514Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 621,
        "chapter_id": 139,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:42.078Z",
        "created_at": "2016-12-14T16:47:42.078Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 619,
        "chapter_id": 139,
        "position": 67,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:41.935Z",
        "created_at": "2016-12-14T16:47:41.827Z",
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
            "id": 163,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 164,
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
curl "api.goskive.com/v2/chapters/139" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7620a44eb3d336638a9189f9fdcc17fb749f2725466c45005483450a6d1cb359"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/146
Content-Type: application/json
Authorization: Bearer 2e6e220ff69360fff17db5f955beefa339bf76f714c071ced90a0599977eb3e6
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
    "id": 146,
    "updated_at": "2016-12-14T16:47:44.162Z",
    "course_id": 207,
    "author_id": 646,
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
curl "api.goskive.com/v2/chapters/146" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e6e220ff69360fff17db5f955beefa339bf76f714c071ced90a0599977eb3e6"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/4/replies
Content-Type: application/json
Authorization: Bearer da204ab2a67d8dca59617d0bd063a67c76a3ac36321e703a520fd34e3e3d05cd
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
    "author_id": 607,
    "reply_to_id": 4,
    "created_at": "2016-12-14T16:47:40.665Z",
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
	-H "Authorization: Bearer da204ab2a67d8dca59617d0bd063a67c76a3ac36321e703a520fd34e3e3d05cd"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/6/replies
Content-Type: application/json
Authorization: Bearer 96e1aed065aae0383203f0876d311531a7f83b3f46ed9d50b6c55dd775691860
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
curl "api.goskive.com/v2/comments/6/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96e1aed065aae0383203f0876d311531a7f83b3f46ed9d50b6c55dd775691860"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/52
Content-Type: application/json
Authorization: Bearer 23481ffeec0031e09cd55505e8bd45ea66417aa2b465e3d23c1641627b9d908e
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
curl "api.goskive.com/v2/comments/52" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23481ffeec0031e09cd55505e8bd45ea66417aa2b465e3d23c1641627b9d908e"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/55/republish
Content-Type: application/json
Authorization: Bearer 9c12034743d1dd645949e45d5a07920dd526c0c6ac1d53cfa3667bff18ad54f2
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
curl "api.goskive.com/v2/comments/55/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c12034743d1dd645949e45d5a07920dd526c0c6ac1d53cfa3667bff18ad54f2"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer 1e5dce7f445b95caab2fbcc8986706246d80fd49299e74022a571b5ede7966dd
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e5dce7f445b95caab2fbcc8986706246d80fd49299e74022a571b5ede7966dd"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/16/report
Content-Type: application/json
Authorization: Bearer 890982236fe6fd913b86e37ffee706983b202e13105dd76d150849561e335ee2
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 890982236fe6fd913b86e37ffee706983b202e13105dd76d150849561e335ee2"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/12
Content-Type: application/json
Authorization: Bearer d8b539569b7c68562545749825136be42465b5c39d1dafb23aa765adfa42fbe6
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
    "id": 12,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-14T16:47:19.432Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8b539569b7c68562545749825136be42465b5c39d1dafb23aa765adfa42fbe6"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 675212ac895545b2b61f7017110176f8136938692f4a2c6656d5937d080a3d7e
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
      "name": "Fake Company Name 12",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-14T16:47:19.509Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-14T16:47:19.515Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-14T16:47:19.519Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 675212ac895545b2b61f7017110176f8136938692f4a2c6656d5937d080a3d7e"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer cc61870d67607b6195967303634692143cc427fc7908075fc37ca518a9dc479f
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
curl "api.goskive.com/v2/companies/27/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc61870d67607b6195967303634692143cc427fc7908075fc37ca518a9dc479f"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer e14e746fcdfaee387e3fd258569c40bad1b68feb8eefc617e30ee617246e4d5e
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
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e14e746fcdfaee387e3fd258569c40bad1b68feb8eefc617e30ee617246e4d5e"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer eb9e691c9b1b57155efa21450a877899411cf5c6ed4631721ee52b79971be2b0
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
      "company_id": 34,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
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
      "company_id": 37,
      "precluded_campaign_ids": [

      ],
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
	-H "Authorization: Bearer eb9e691c9b1b57155efa21450a877899411cf5c6ed4631721ee52b79971be2b0"
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
Authorization: Bearer e376af3310dcc1d8bca4c3cb39bb86be07e4fd6a557e6f8de0eb410d04365294
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
	-H "Authorization: Bearer e376af3310dcc1d8bca4c3cb39bb86be07e4fd6a557e6f8de0eb410d04365294"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e84c7cbe758718999b3209e21ae4faba84230fa46c729d7a012ab22581c10bd1
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
    "id": 56,
    "updated_at": "2016-12-14T16:47:06.725Z",
    "course_id": 57,
    "author_id": 192,
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
	-H "Authorization: Bearer e84c7cbe758718999b3209e21ae4faba84230fa46c729d7a012ab22581c10bd1"
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
      "id": 34,
      "updated_at": "2016-12-14T16:47:03.682Z",
      "course_id": 45,
      "author_id": 144,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 34",
      "position": 1
    },
    {
      "id": 35,
      "updated_at": "2016-12-14T16:47:03.709Z",
      "course_id": 45,
      "author_id": 145,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 35",
      "position": 2
    },
    {
      "id": 36,
      "updated_at": "2016-12-14T16:47:03.939Z",
      "course_id": 45,
      "author_id": 146,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-14T16:47:03.580Z",
      "questions_updated_at": "2016-12-14T16:47:03.580Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 36",
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
Authorization: Bearer ef0a2d94e029e35f16b2fb69ee75a79bfb1ef50b6b09e186963870e70ef23228
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
      "id": 40,
      "updated_at": "2016-12-14T16:47:04.416Z",
      "course_id": 48,
      "author_id": 155,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 40",
      "position": 1
    },
    {
      "id": 41,
      "updated_at": "2016-12-14T16:47:04.442Z",
      "course_id": 48,
      "author_id": 156,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 41",
      "position": 2
    },
    {
      "id": 42,
      "updated_at": "2016-12-14T16:47:04.672Z",
      "course_id": 48,
      "author_id": 157,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-14T16:47:04.313Z",
      "questions_updated_at": "2016-12-14T16:47:04.313Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 42",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef0a2d94e029e35f16b2fb69ee75a79bfb1ef50b6b09e186963870e70ef23228"
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
      "id": 37,
      "updated_at": "2016-12-14T16:47:04.209Z",
      "course_id": 47,
      "author_id": 151,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 37",
      "position": 1
    },
    {
      "id": 38,
      "updated_at": "2016-12-14T16:47:04.236Z",
      "course_id": 47,
      "author_id": 152,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 38",
      "position": 2
    },
    {
      "id": 39,
      "updated_at": "2016-12-14T16:47:04.262Z",
      "course_id": 47,
      "author_id": 153,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 39",
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
Authorization: Bearer 4f17b7a5b8e5b37fe0b1db819a77524d3bf0e56ddd1f9580a14cc2229464a648
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
      "id": 43,
      "updated_at": "2016-12-14T16:47:04.864Z",
      "course_id": 49,
      "author_id": 162,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 43",
      "position": 1
    },
    {
      "id": 44,
      "updated_at": "2016-12-14T16:47:04.887Z",
      "course_id": 49,
      "author_id": 163,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 44",
      "position": 2
    },
    {
      "id": 45,
      "updated_at": "2016-12-14T16:47:04.911Z",
      "course_id": 49,
      "author_id": 164,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 45",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f17b7a5b8e5b37fe0b1db819a77524d3bf0e56ddd1f9580a14cc2229464a648"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer edad65c4de047eeb98510d053db40a506b11ff0b5f420a49dfdc9a3624559102
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
    "course_id": 1,
    "user_id": 2,
    "updated_at": "2016-12-14T16:46:50.684Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edad65c4de047eeb98510d053db40a506b11ff0b5f420a49dfdc9a3624559102"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 42038bdb4d04e6b0a51373b3f06202e887089377c820125059cbefaf01d69b80
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
      "course_id": 4,
      "user_id": 8,
      "updated_at": "2016-12-14T16:46:51.103Z"
    },
    {
      "id": 4,
      "course_id": 4,
      "user_id": 9,
      "updated_at": "2016-12-14T16:46:51.118Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42038bdb4d04e6b0a51373b3f06202e887089377c820125059cbefaf01d69b80"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/197/files
Content-Type: application/json
Authorization: Bearer c811054a0a11a683722ffe8b642246e6efcd083de2bf0b94da9898edf5e24079
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
      "id": 17,
      "uploader": {
        "id": 599,
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
        "created_at": "2016-12-14T16:47:40.196Z",
        "updated_at": "2016-12-14T16:47:40.196Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-14T16:47:40.206Z",
      "updated_at": "2016-12-14T16:47:40.206Z",
      "course_id": 197,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 18,
      "uploader": {
        "id": 600,
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
        "created_at": "2016-12-14T16:47:40.215Z",
        "updated_at": "2016-12-14T16:47:40.215Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-14T16:47:40.224Z",
      "updated_at": "2016-12-14T16:47:40.224Z",
      "course_id": 197,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 19,
      "uploader": {
        "id": 601,
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
        "created_at": "2016-12-14T16:47:40.233Z",
        "updated_at": "2016-12-14T16:47:40.233Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-14T16:47:40.241Z",
      "updated_at": "2016-12-14T16:47:40.241Z",
      "course_id": 197,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/197/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c811054a0a11a683722ffe8b642246e6efcd083de2bf0b94da9898edf5e24079"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/194/files
Content-Type: application/json
Authorization: Bearer de9ce6a88475c81eb09044daee7d036a08fa08cfe82187c4c51f2e757b92881b
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
    "id": 16,
    "uploader": {
      "id": 593,
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
      "created_at": "2016-12-14T16:47:39.742Z",
      "updated_at": "2016-12-14T16:47:39.742Z"
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
    "created_at": "2016-12-14T16:47:39.775Z",
    "updated_at": "2016-12-14T16:47:39.775Z",
    "course_id": 194,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/194/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de9ce6a88475c81eb09044daee7d036a08fa08cfe82187c4c51f2e757b92881b"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/195/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer eba6929d18a66acba5a01df58d2e413864ae20690c7c8bf08c88bb04e63c8881
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
    "key": "cache/5ae3756dcff6aea6b37c0e541b0c5941.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNFQxNzo0NzozOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzVhZTM3NTZkY2ZmNmFlYTZiMzdjMGU1NDFiMGM1OTQxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTQvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE0VDE2NDczOVoifV19",
    "x-amz-credential": "FAKE/20161214/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161214T164739Z",
    "x-amz-signature": "d43fd679b2d8a8a118a6408c174c5b0b9117b2b6cd78886cfee01677cc13f85f"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/195/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eba6929d18a66acba5a01df58d2e413864ae20690c7c8bf08c88bb04e63c8881"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 784f9dc00b1983c2282148ea8c545ce992eefdffe31bbdfd3b92f2a03a75ab5c
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
	-H "Authorization: Bearer 784f9dc00b1983c2282148ea8c545ce992eefdffe31bbdfd3b92f2a03a75ab5c"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0e3c31a3118a71c127bbd3fed74c18b6311d09c49614e3a5a3889fee6d6a5b7c
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
	-H "Authorization: Bearer 0e3c31a3118a71c127bbd3fed74c18b6311d09c49614e3a5a3889fee6d6a5b7c"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0bc71a615c4b4a7036784206ac675bfca35f62fd2d382fc5564b758741a38fee
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
	-H "Authorization: Bearer 0bc71a615c4b4a7036784206ac675bfca35f62fd2d382fc5564b758741a38fee"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b716995406e77d25b733a86300617fbdc8d4e7cfe953128627534992bc96d1a4
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
	-H "Authorization: Bearer b716995406e77d25b733a86300617fbdc8d4e7cfe953128627534992bc96d1a4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 38a000095592182db2d55eb5af0f3fd1fb796f5d34c71660ce05579d07dd79ce
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
	-H "Authorization: Bearer 38a000095592182db2d55eb5af0f3fd1fb796f5d34c71660ce05579d07dd79ce"
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
    "creator_id": 692,
    "id": 227,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "discipline_id": 232,
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
    "chapters_updated_at": "2016-12-14T16:47:48.863Z",
    "updated_at": "2016-12-14T16:47:50.068Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 692,
        "chapter_id": 154,
        "position": 80,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:49.120Z",
        "created_at": "2016-12-14T16:47:49.041Z",
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
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 692,
        "chapter_id": 155,
        "position": 82,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:49.398Z",
        "created_at": "2016-12-14T16:47:49.319Z",
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
    ],
    "chapters": [
      {
        "id": 154,
        "updated_at": "2016-12-14T16:47:50.021Z",
        "course_id": 227,
        "author_id": 692,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-14T16:47:48.863Z",
        "questions_updated_at": "2016-12-14T16:47:48.863Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 133",
        "position": 1
      },
      {
        "id": 155,
        "updated_at": "2016-12-14T16:47:50.059Z",
        "course_id": 227,
        "author_id": 692,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-14T16:47:48.863Z",
        "questions_updated_at": "2016-12-14T16:47:48.863Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 134",
        "position": 2
      }
    ],
    "topic_id": 231,
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
Authorization: Bearer 9aa8d54e9f456683066eddcf61b1816877d12a802db56631c2ce1b902bcaee98
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
    "creator_id": 697,
    "id": 228,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 208,
    "additional_university_ids": [

    ],
    "discipline_id": 233,
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
    "chapters_updated_at": "2016-12-14T16:47:50.128Z",
    "updated_at": "2016-12-14T16:47:51.267Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 698,
        "chapter_id": 156,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:51.063Z",
        "created_at": "2016-12-14T16:47:51.063Z",
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
        "author_id": 698,
        "chapter_id": 157,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:51.131Z",
        "created_at": "2016-12-14T16:47:51.131Z",
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
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 698,
        "chapter_id": 156,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:51.101Z",
        "created_at": "2016-12-14T16:47:51.101Z",
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
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 698,
        "chapter_id": 157,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:51.170Z",
        "created_at": "2016-12-14T16:47:51.170Z",
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
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 698,
        "chapter_id": 156,
        "position": 86,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:50.325Z",
        "created_at": "2016-12-14T16:47:50.248Z",
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
            "id": 201,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 202,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 100,
        "obfuscated_id": "erXmBhoMZFI",
        "author_id": 698,
        "chapter_id": 156,
        "position": 87,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:50.449Z",
        "created_at": "2016-12-14T16:47:50.378Z",
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
            "id": 203,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 204,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 101,
        "obfuscated_id": "PprZyBVq_gc",
        "author_id": 698,
        "chapter_id": 157,
        "position": 88,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:50.606Z",
        "created_at": "2016-12-14T16:47:50.523Z",
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
            "id": 205,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 206,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 102,
        "obfuscated_id": "jFy90P7ldB4",
        "author_id": 698,
        "chapter_id": 157,
        "position": 89,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:50.736Z",
        "created_at": "2016-12-14T16:47:50.662Z",
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
            "id": 207,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 208,
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
        "id": 156,
        "updated_at": "2016-12-14T16:47:51.218Z",
        "course_id": 228,
        "author_id": 697,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-14T16:47:50.128Z",
        "questions_updated_at": "2016-12-14T16:47:50.128Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 135",
        "position": 1
      },
      {
        "id": 157,
        "updated_at": "2016-12-14T16:47:51.257Z",
        "course_id": 228,
        "author_id": 697,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-14T16:47:50.128Z",
        "questions_updated_at": "2016-12-14T16:47:50.128Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 136",
        "position": 2
      }
    ],
    "topic_id": 232,
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
	-H "Authorization: Bearer 9aa8d54e9f456683066eddcf61b1816877d12a802db56631c2ce1b902bcaee98"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/230/pin
Content-Type: application/json
Authorization: Bearer 163e682fdf1e5a649127b208338e9c1269a3dad3d472e0ee734fbb786492f202
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/230/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 163e682fdf1e5a649127b208338e9c1269a3dad3d472e0ee734fbb786492f202"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/221/pin
Content-Type: application/json
Authorization: Bearer 98e21f352208b52460b7845cc3dadacdcffd2803c6ce08bf371c4a84156fd5eb
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/221/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98e21f352208b52460b7845cc3dadacdcffd2803c6ce08bf371c4a84156fd5eb"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cd45aca5e75cde99e48f9eab2d9da44f68245d07f4fc89e2c4df80b3899aa84e
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
    "creator_id": 683,
    "id": 224,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 204,
    "additional_university_ids": [

    ],
    "discipline_id": 229,
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
    "updated_at": "2016-12-14T16:47:47.341Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 228,
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
	-H "Authorization: Bearer cd45aca5e75cde99e48f9eab2d9da44f68245d07f4fc89e2c4df80b3899aa84e"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 6ca24eea55226a38c0d8936cf301105379e922be78a725730317db2ea7f62d4a
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
    "id": 812,
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
    "created_at": "2016-12-14T16:48:01.040Z",
    "updated_at": "2016-12-14T16:48:01.040Z",
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
	-H "Authorization: Bearer 6ca24eea55226a38c0d8936cf301105379e922be78a725730317db2ea7f62d4a"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d4d0881379601ac6b63b63506500b5ed4b5c901c8f13fa8b3e34e8744413a162
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[259]}
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
    "id": 808,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      259
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-14T16:48:00.757Z",
    "updated_at": "2016-12-14T16:48:00.799Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[259]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4d0881379601ac6b63b63506500b5ed4b5c901c8f13fa8b3e34e8744413a162"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer eada646d6d6a9ea7be8570be251ee326b8cb582a308dde72caeaa13bd9a60142
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
    "id": 809,
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
    "created_at": "2016-12-14T16:48:00.825Z",
    "updated_at": "2016-12-14T16:48:00.825Z",
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
	-H "Authorization: Bearer eada646d6d6a9ea7be8570be251ee326b8cb582a308dde72caeaa13bd9a60142"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2f84b9a735223c61c7dbe65a658a140d1e6e1e6502be32722b4e7376b679df59
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[262]}
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
    "id": 811,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      262
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-14T16:48:00.984Z",
    "updated_at": "2016-12-14T16:48:00.984Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[262]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f84b9a735223c61c7dbe65a658a140d1e6e1e6502be32722b4e7376b679df59"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b119f8a610e5101ca15c9b7d975144e9b2de4351089f359b48e79794da674641
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

258
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
    "id": 807,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/b40fb0b5931c761b703c1da9fe5e63a02059f137.jpg",
    "university_id": null,
    "fields_of_study": [
      258
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-14T16:48:00.404Z",
    "updated_at": "2016-12-14T16:48:00.706Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/0b2198ab5e846a5cff38057863c4732432010e21.jpg",
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

258
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b119f8a610e5101ca15c9b7d975144e9b2de4351089f359b48e79794da674641"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 777386004e15190d486da8cefbbeb8feeb150484161b1607b76ef1cf898e2788
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
      "bookmarkable_id": 126,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 127,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 128,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 777386004e15190d486da8cefbbeb8feeb150484161b1607b76ef1cf898e2788"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer bdeb8407cad4491cf0053a0e00332a6d53b62fd4164d955a39453e32e8f93118
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
      "creator_id": 767,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-179",
      "html_url": "https://goskive.com/course/mit-course-179",
      "slug": "mit-course-179",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "discipline_id": 249,
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
      "updated_at": "2016-12-14T16:47:57.165Z",
      "shortname": "mit-course-179",
      "topic_id": 248,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 768,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-180",
      "html_url": "https://goskive.com/course/mit-course-180",
      "slug": "mit-course-180",
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
      "updated_at": "2016-12-14T16:47:57.267Z",
      "shortname": "mit-course-180",
      "topic_id": 249,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 180",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdeb8407cad4491cf0053a0e00332a6d53b62fd4164d955a39453e32e8f93118"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer f1cc05c26961d4e81bc8d664b3ae5195cd753eb9117c766be438a9f9647434a5
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
        "id": 20,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-14T16:47:44.606Z",
        "updated_at": "2016-12-14T16:47:44.606Z",
        "file_url": "memory://ede67b7332102205237e52d970af9e2c.pdf",
        "course_id": 209,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 21,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-14T16:47:44.712Z",
        "updated_at": "2016-12-14T16:47:44.712Z",
        "file_url": "memory://4937c09b7c1a51f54fd84ab286a699a9.pdf",
        "course_id": 210,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 22,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-14T16:47:44.817Z",
        "updated_at": "2016-12-14T16:47:44.817Z",
        "file_url": "memory://e3e6c6cecea742a32da5212bd99ce300.pdf",
        "course_id": 211,
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
	-H "Authorization: Bearer f1cc05c26961d4e81bc8d664b3ae5195cd753eb9117c766be438a9f9647434a5"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer f117e31a1cfdc1b0bf4ff3f8be848940ed418caebf918ba0ec445b7a9096122b
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-14T16:47:41.380Z"
      },
      "created_at": "2016-12-14T16:47:41.384Z",
      "updated_at": "2016-12-14T16:47:41.384Z",
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
      "company_id": 23,
      "company": {
        "id": 23,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-14T16:47:41.392Z"
      },
      "created_at": "2016-12-14T16:47:41.395Z",
      "updated_at": "2016-12-14T16:47:41.395Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f117e31a1cfdc1b0bf4ff3f8be848940ed418caebf918ba0ec445b7a9096122b"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer e4ee692136671ef9b978dee994964c91ca2c1cbfc591619361d74ac040854861
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
      "id": 13,
      "created_at": "2016-12-14T16:47:54.528Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-12-14T16:47:54.658Z",
      "author_id": "732",
      "thread_subject_id": "235",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 14,
      "created_at": "2016-12-14T16:47:54.647Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 8,
      "updated_at": "2016-12-14T16:47:54.661Z",
      "author_id": "735",
      "thread_subject_id": "236",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 15,
      "created_at": "2016-12-14T16:47:55.001Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-12-14T16:47:55.001Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-12-14T16:47:55.332Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-12-14T16:47:55.332Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 17,
      "created_at": "2016-12-14T16:47:55.677Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 23,
      "updated_at": "2016-12-14T16:47:55.677Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 18,
      "created_at": "2016-12-14T16:47:55.927Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 115,
      "updated_at": "2016-12-14T16:47:55.927Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 19,
      "created_at": "2016-12-14T16:47:56.190Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 116,
      "updated_at": "2016-12-14T16:47:56.190Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-12-14T16:47:56.450Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 117,
      "updated_at": "2016-12-14T16:47:56.450Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4ee692136671ef9b978dee994964c91ca2c1cbfc591619361d74ac040854861"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/21
Content-Type: application/json
Authorization: Bearer d37b5e12d758dd4efa907d757ec24aabd7f02a95a1dcc05c58c1703f1348c8fe
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-14T16:37:56.000Z"}}
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
    "id": 21,
    "created_at": "2016-12-14T16:47:56.603Z",
    "read_at": "2016-12-14T16:37:56.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 9,
    "updated_at": "2016-12-14T16:47:56.640Z",
    "author_id": "760",
    "thread_subject_id": "243",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/21" -d '{"notification":{"read_at":"2016-12-14T16:37:56.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d37b5e12d758dd4efa907d757ec24aabd7f02a95a1dcc05c58c1703f1348c8fe"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 8c9d8d450040ccb3fcd65d8f7977e7911a43137deac86e1aa2ff8f7ba1b66abe
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
      "course_id": 190,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-14T16:47:38.947Z",
      "course_published": true,
      "updated_at": "2016-12-14T16:47:38.942Z"
    },
    {
      "id": 4,
      "course_id": 191,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-14T16:47:39.054Z",
      "course_published": true,
      "updated_at": "2016-12-14T16:47:39.049Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c9d8d450040ccb3fcd65d8f7977e7911a43137deac86e1aa2ff8f7ba1b66abe"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer 7b558a33c75035d7e1052c3e05d918a7f9236f4a87d03d25df3e9881b228d2d0
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
    "course_id": 188,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-14T16:47:38.578Z",
    "course_published": true,
    "updated_at": "2016-12-14T16:47:38.572Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b558a33c75035d7e1052c3e05d918a7f9236f4a87d03d25df3e9881b228d2d0"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 28fab3a9ab89b4d0a87b9242e3531fc968d6ef44c2b66a7014a034e76272fd94
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
    "id": 2,
    "course_id": 189,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-14T16:47:38.782Z",
    "course_published": true,
    "updated_at": "2016-12-14T16:47:38.773Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28fab3a9ab89b4d0a87b9242e3531fc968d6ef44c2b66a7014a034e76272fd94"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 498a5ac31a25b512ae4804813cded2c0203886e330a049d7e316d6173bb311fb
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
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 29,
      "user_id": 200
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 30,
      "user_id": 200
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 31,
      "user_id": 200
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 200
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 498a5ac31a25b512ae4804813cded2c0203886e330a049d7e316d6173bb311fb"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/211
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
    "id": 211,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 211,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 211
      },
      {
        "id": 212,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 211
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/211" -X GET \
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
      "id": 212,
      "name": "Synergized transitional task-force",
      "name_translations": {
        "en": "Synergized transitional task-force"
      }
    },
    {
      "id": 213,
      "name": "Seamless didactic portal",
      "name_translations": {
        "en": "Seamless didactic portal"
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
PATCH /v2/feedbacks/10/close
Content-Type: application/json
Authorization: Bearer d09c5164f6ace1acc4d8edbd62bffeec7b7a44b0151337f9dc3fd3c92a496648
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
    "id": 10,
    "user_id": 443,
    "feedbackable_id": 45,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-14T16:47:28.627Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/10/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d09c5164f6ace1acc4d8edbd62bffeec7b7a44b0151337f9dc3fd3c92a496648"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/14/fix
Content-Type: application/json
Authorization: Bearer 1b9cf143b0b9b355035ab7eb45106898d250e2e96f38c630f00e528176bbd706
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
    "id": 14,
    "user_id": 463,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-14T16:47:29.921Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/14/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b9cf143b0b9b355035ab7eb45106898d250e2e96f38c630f00e528176bbd706"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/35
Content-Type: application/json
Authorization: Bearer a913cd8739d9ac91f09181b8996168f0ca9f32c17e59e7ad88b5bf411ca6aa52
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
    "id": 35,
    "user_id": 554,
    "feedbackable_id": 51,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-14T16:47:36.581Z",
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
curl "api.goskive.com/v2/feedbacks/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a913cd8739d9ac91f09181b8996168f0ca9f32c17e59e7ad88b5bf411ca6aa52"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/11/close
Content-Type: application/json
Authorization: Bearer df92d4a8cde52808b98079b9400e6ced61f15ec8d0d2484ffffb7101a73e15ae
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
	-H "Authorization: Bearer df92d4a8cde52808b98079b9400e6ced61f15ec8d0d2484ffffb7101a73e15ae"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer bb10cb00399171f0d9ef4da41a19c1137a1ffde0f05591ad74fa8b2c9622fad5
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
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb10cb00399171f0d9ef4da41a19c1137a1ffde0f05591ad74fa8b2c9622fad5"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/15/fix
Content-Type: application/json
Authorization: Bearer 718e69144fa1f51e6db017e1c08d4420a11c4f6106198e3503dc298e26fadd1b
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
curl "api.goskive.com/v2/feedbacks/15/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 718e69144fa1f51e6db017e1c08d4420a11c4f6106198e3503dc298e26fadd1b"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/36
Content-Type: application/json
Authorization: Bearer 9cff6d41db0e5c2035ba41d8ad94192157abc3acc68ff0bd31aa07726a189a0c
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
    "id": 36,
    "user_id": 559,
    "feedbackable_id": 52,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-14T16:47:36.922Z",
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
curl "api.goskive.com/v2/feedbacks/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cff6d41db0e5c2035ba41d8ad94192157abc3acc68ff0bd31aa07726a189a0c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer 4843ddc300797c9a4697bd60b331b13111d3787122a18f828a54af74a1e8c0a1
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
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4843ddc300797c9a4697bd60b331b13111d3787122a18f828a54af74a1e8c0a1"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/3/bookmark
Content-Type: application/json
Authorization: Bearer 050f24ef26d7fc652042fe12114e17dbe972b629503842a2fb5c19bb3dc3fc96
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 050f24ef26d7fc652042fe12114e17dbe972b629503842a2fb5c19bb3dc3fc96"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer af0a43a6279179ff424cab57ecaa22ffa401995db35bd828fe262c884ea2fd39
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
	-H "Authorization: Bearer af0a43a6279179ff424cab57ecaa22ffa401995db35bd828fe262c884ea2fd39"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/6
Content-Type: application/json
Authorization: Bearer a251781c21653a5cc0c74a0f3621fc9f2d14092e9fee901281455ffddbbb38f6
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/06f25a7aeeb53a1f1ef8c968d790e74b.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161214%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161214T164720Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2839f37aaa73c124eb53d772540aec12b4dd2cafc0fe8355e757253c380a1ef9",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a251781c21653a5cc0c74a0f3621fc9f2d14092e9fee901281455ffddbbb38f6"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/4/preview
Content-Type: application/json
Authorization: Bearer 9b31429f2a00d602d82ec9cfbba9d0b5f1ce14b4fd08dfdf92eda4e8ae517fcf
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/f22d3a37ed5e588ff331151ce5e33506.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161214%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161214T164719Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8dfa4f02a668692d181c8c4977e1211ee1f3cbcf62979a59adfb8c27435a7d35",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/4/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b31429f2a00d602d82ec9cfbba9d0b5f1ce14b4fd08dfdf92eda4e8ae517fcf"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer 8687c8b6374004b38cecf3f7d44acd1abae73b8f1a9c55703e19bfe9d2eb968b
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
      "id": 361,
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
      "created_at": "2016-12-14T16:47:20.761Z",
      "updated_at": "2016-12-14T16:47:20.761Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-14T16:47:20.858Z",
    "updated_at": "2016-12-14T16:47:20.858Z",
    "course_id": 107,
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
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8687c8b6374004b38cecf3f7d44acd1abae73b8f1a9c55703e19bfe9d2eb968b"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer ae527b60b8c543aeae41be295c4cd91a68ed19176064399befd8e2f15ec0f157
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
      "creator_id": 248,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "discipline_id": 73,
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
      "chapters_updated_at": "2016-12-14T16:47:12.479Z",
      "updated_at": "2016-12-14T16:47:13.984Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 253,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-0338aa76-cde0-4292-b57c-bd0de372f795",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-0338aa76-cde0-4292-b57c-bd0de372f795",
      "slug": "mit-the-great-british-bake-off-0338aa76-cde0-4292-b57c-bd0de372f795",
      "university_id": 75,
      "additional_university_ids": [

      ],
      "discipline_id": 74,
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
      "chapters_updated_at": "2016-12-14T16:47:12.479Z",
      "updated_at": "2016-12-14T16:47:14.490Z",
      "shortname": "mit-the-great-british-bake-off-0338aa76-cde0-4292-b57c-bd0de372f795",
      "topic_id": 74,
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
	-H "Authorization: Bearer ae527b60b8c543aeae41be295c4cd91a68ed19176064399befd8e2f15ec0f157"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/13/download
Content-Type: application/json
Authorization: Bearer 562d04d4e32b637ce6c17c71c28ada5a765a446cfd872e9ed40be2cd87d87284
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 562d04d4e32b637ce6c17c71c28ada5a765a446cfd872e9ed40be2cd87d87284"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/15/report
Content-Type: application/json
Authorization: Bearer 6da7a9d796cd0ef8f95d73c02176b8aef524e75f0959300548b479c07c813a17
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6da7a9d796cd0ef8f95d73c02176b8aef524e75f0959300548b479c07c813a17"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/14/bookmark
Content-Type: application/json
Authorization: Bearer 0689c7a38d8e3f1a0108d5abc43a0c5bc90f7776d61921bb8aaba3dfa01bfbf9
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0689c7a38d8e3f1a0108d5abc43a0c5bc90f7776d61921bb8aaba3dfa01bfbf9"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/5/upvote
Content-Type: application/json
Authorization: Bearer 6b02f49590e4b534e99d5058fbc74c0c11f9257ac3f096fc90aa0fdc104c3083
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b02f49590e4b534e99d5058fbc74c0c11f9257ac3f096fc90aa0fdc104c3083"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/88/comments
Content-Type: application/json
Authorization: Bearer ae82782d02d9f68352405de096cfa9234e95586823ae611fdb8c60c8ea5213e7
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
    "author_id": 832,
    "reply_to_id": null,
    "created_at": "2016-12-14T16:48:02.595Z",
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
curl "api.goskive.com/v2/flashcards/88/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae82782d02d9f68352405de096cfa9234e95586823ae611fdb8c60c8ea5213e7"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/89/comments
Content-Type: application/json
Authorization: Bearer 0de89537b6176299640697b0ba0f48482399162fd224c348975918f845a061c7
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
    "author_id": 835,
    "reply_to_id": null,
    "created_at": "2016-12-14T16:48:02.927Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 45,
      "user_id": 835,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:48:02.925Z",
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
curl "api.goskive.com/v2/flashcards/89/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0de89537b6176299640697b0ba0f48482399162fd224c348975918f845a061c7"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/86/comments
Content-Type: application/json
Authorization: Bearer c7ef4641286311e287edccbdcef7fd4126de4f0fe88273b8fc5afb52d9c16b67
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
      "author_id": 828,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:02.122Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 827,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:02.107Z",
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
curl "api.goskive.com/v2/flashcards/86/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7ef4641286311e287edccbdcef7fd4126de4f0fe88273b8fc5afb52d9c16b67"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/90/comments
Content-Type: application/json
Authorization: Bearer 23a79b81b048de09d69e88a16a8a534fe9dbce61d40f320fad8a177f5bc78de9
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
curl "api.goskive.com/v2/flashcards/90/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23a79b81b048de09d69e88a16a8a534fe9dbce61d40f320fad8a177f5bc78de9"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/7/feedbacks
Content-Type: application/json
Authorization: Bearer ad0eab75f59b452328991a1357653424ffb72499b205ab6a9159367c18aad30e
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
    "id": 7,
    "user_id": 47,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-14T16:46:53.239Z",
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
curl "api.goskive.com/v2/flashcards/7/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad0eab75f59b452328991a1357653424ffb72499b205ab6a9159367c18aad30e"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/6/feedbacks
Content-Type: application/json
Authorization: Bearer 2b30dfc0b55c44137854bfc44818ba26d6ee3bf09cd31176ca303f075da06af5
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
      "id": 6,
      "user_id": 46,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:46:52.983Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 45,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:46:52.973Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/6/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b30dfc0b55c44137854bfc44818ba26d6ee3bf09cd31176ca303f075da06af5"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/85/votes
Content-Type: application/json
Authorization: Bearer a07c83be483f3dc7f9d706a2984f3a17eaa30e1ffee005f69b05e19d52549565
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
      "id": 20,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 722
    },
    {
      "id": 19,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 721
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 720
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/85/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a07c83be483f3dc7f9d706a2984f3a17eaa30e1ffee005f69b05e19d52549565"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/38/republish
Content-Type: application/json
Authorization: Bearer 99a509c034691c17c51d013943e4d9e0f7f982a139f8c878f9a60b1851daaf3b
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
curl "api.goskive.com/v2/flashcards/38/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99a509c034691c17c51d013943e4d9e0f7f982a139f8c878f9a60b1851daaf3b"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/36/bookmark
Content-Type: application/json
Authorization: Bearer 5faaa6ec4647671d1d29a6ddad0922bce669184bd7e996cf7d4b9ab63894c94b
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/36/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5faaa6ec4647671d1d29a6ddad0922bce669184bd7e996cf7d4b9ab63894c94b"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/31
Content-Type: application/json
Authorization: Bearer ccda9cde579e41bac65560c255961806834138bd4f9bfb017369182f7c1a4892
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/31" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccda9cde579e41bac65560c255961806834138bd4f9bfb017369182f7c1a4892"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/downvote
Content-Type: application/json
Authorization: Bearer d12566b24f5af4d89adad23dd68f812b2aef447bd032ba520eff9f2a1e93faf0
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d12566b24f5af4d89adad23dd68f812b2aef447bd032ba520eff9f2a1e93faf0"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/34
Content-Type: application/json
Authorization: Bearer 79c8033762a01fca5193593db2ad066986a461cd602df723c915b04cced27ed6
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
    "id": 34,
    "obfuscated_id": "LRSQf_NrQzE",
    "author_id": 320,
    "chapter_id": 90,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:18.343Z",
    "created_at": "2016-12-14T16:47:18.343Z",
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
curl "api.goskive.com/v2/flashcards/34" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79c8033762a01fca5193593db2ad066986a461cd602df723c915b04cced27ed6"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/report
Content-Type: application/json
Authorization: Bearer 093abc5751989a18e9e9aa57aa894efcc707ba46d29382ceb8291e4f2044956c
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 093abc5751989a18e9e9aa57aa894efcc707ba46d29382ceb8291e4f2044956c"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/32/bookmark
Content-Type: application/json
Authorization: Bearer e44e44c248d71602d379e9abc27263987160457eee8ac4153116bcfbb526c3eb
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/32/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e44e44c248d71602d379e9abc27263987160457eee8ac4153116bcfbb526c3eb"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/39/upvote
Content-Type: application/json
Authorization: Bearer 035ccb221f80311acb99a2465890a5964ab993f2bf738162b9d7e4808ba3808b
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 035ccb221f80311acb99a2465890a5964ab993f2bf738162b9d7e4808ba3808b"
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
    "key": "cache/5f70e171f263041414e6e27ab55d5e7e.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNFQxNzo0Njo0OVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzVmNzBlMTcxZjI2MzA0MTQxNGU2ZTI3YWI1NWQ1ZTdlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTRUMTY0NjQ5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161214/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161214T164649Z",
    "x-amz-signature": "307f461f8c6ef0df5b13a3325177f416675860a6352a50fc7ee1f48c1509f38c"
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
Authorization: Bearer f10a9ed6b921ad3441d7fa2fe735fd5e9f1906a356e8a940a2db6d94e639303a
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
	-H "Authorization: Bearer f10a9ed6b921ad3441d7fa2fe735fd5e9f1906a356e8a940a2db6d94e639303a"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer cd543df8081ba7321cf06568687a8707efab4f99ad515542431ceed82c8206fe
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
	-H "Authorization: Bearer cd543df8081ba7321cf06568687a8707efab4f99ad515542431ceed82c8206fe"
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
{"password":{"reset_password_token":"2zhp7LZKYF-HqzJSu5zQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 975,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-14T16:48:12.458Z",
  "updated_at": "2016-12-14T16:48:13.075Z",
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
  "audit_id": 8999
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"2zhp7LZKYF-HqzJSu5zQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/133/comments
Content-Type: application/json
Authorization: Bearer 4b437b13632d424955b034fdfaa6808290970bfbd62cf3930893becfae4a35dc
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
    "id": 59,
    "author_id": 960,
    "reply_to_id": null,
    "created_at": "2016-12-14T16:48:11.119Z",
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
curl "api.goskive.com/v2/questions/133/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b437b13632d424955b034fdfaa6808290970bfbd62cf3930893becfae4a35dc"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/134/comments
Content-Type: application/json
Authorization: Bearer 6e4af8da3c30f4c8956213fe9941d86a3da3fb22de48701d44b881b97e0fd0a0
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
    "id": 60,
    "author_id": 963,
    "reply_to_id": null,
    "created_at": "2016-12-14T16:48:11.560Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 963,
      "feedbackable_id": 134,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:48:11.557Z",
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
curl "api.goskive.com/v2/questions/134/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e4af8da3c30f4c8956213fe9941d86a3da3fb22de48701d44b881b97e0fd0a0"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/131/comments
Content-Type: application/json
Authorization: Bearer 24eeed7efe2d338b216bea8396baaa95aeca8ee9240fb4c16c40c94508c22575
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
      "author_id": 956,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:10.506Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 955,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:10.491Z",
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
	-H "Authorization: Bearer 24eeed7efe2d338b216bea8396baaa95aeca8ee9240fb4c16c40c94508c22575"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/132/comments
Content-Type: application/json
Authorization: Bearer dd4ad92adea2490ec21e5f025a91ea3a57c7177b3351cb9adb4115993e090736
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
curl "api.goskive.com/v2/questions/132/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd4ad92adea2490ec21e5f025a91ea3a57c7177b3351cb9adb4115993e090736"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/118/feedbacks
Content-Type: application/json
Authorization: Bearer e3e8de59273a4bc1ae302eed4a1092b435467fe890778e45c89472b0e5b3475e
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
    "id": 37,
    "user_id": 771,
    "feedbackable_id": 118,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-14T16:47:57.883Z",
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
curl "api.goskive.com/v2/questions/118/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3e8de59273a4bc1ae302eed4a1092b435467fe890778e45c89472b0e5b3475e"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/121/feedbacks
Content-Type: application/json
Authorization: Bearer b971cdd5fd639229fb8e00d128af440aecfafb792fdf231d8ccdb182505fda9a
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
      "id": 40,
      "user_id": 784,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:59.053Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 783,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:59.043Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/121/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b971cdd5fd639229fb8e00d128af440aecfafb792fdf231d8ccdb182505fda9a"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/75/votes
Content-Type: application/json
Authorization: Bearer 0603dce5a7a3f29c6e8ef73bca233633f62489a3c5811cc047b9a2a86d93c97c
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
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 571
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 570
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 569
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/75/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0603dce5a7a3f29c6e8ef73bca233633f62489a3c5811cc047b9a2a86d93c97c"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/4/republish
Content-Type: application/json
Authorization: Bearer 1816bc1079b73bbe2144e5dedb74f7cfd80c4668ae0f3cf84a0ce8737679e5cc
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
curl "api.goskive.com/v2/questions/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1816bc1079b73bbe2144e5dedb74f7cfd80c4668ae0f3cf84a0ce8737679e5cc"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/1/bookmark
Content-Type: application/json
Authorization: Bearer 853e5b0b8c02b55f6f2255f1d4621308ffa844f0fbb247f80b76965ef2e4969a
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/1/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 853e5b0b8c02b55f6f2255f1d4621308ffa844f0fbb247f80b76965ef2e4969a"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/24
Content-Type: application/json
Authorization: Bearer 6581312705ba88703170ca7d2ae6e36b81a0b2bc0cebe086ea68c6ed47a97495
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6581312705ba88703170ca7d2ae6e36b81a0b2bc0cebe086ea68c6ed47a97495"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/23/downvote
Content-Type: application/json
Authorization: Bearer b99f69eb55beaa02756560c0eb494213502e71de2c14ecc40ed7087bf5161746
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/23/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b99f69eb55beaa02756560c0eb494213502e71de2c14ecc40ed7087bf5161746"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/5
Content-Type: application/json
Authorization: Bearer 9b267240cadd6c4768e0c11bf0f569f5c797d75e89f63e050de787851cd6645d
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 65,
    "chapter_id": 13,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:46:55.738Z",
    "created_at": "2016-12-14T16:46:55.658Z",
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
        "id": 9,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 10,
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
curl "api.goskive.com/v2/questions/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b267240cadd6c4768e0c11bf0f569f5c797d75e89f63e050de787851cd6645d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/25/report
Content-Type: application/json
Authorization: Bearer 53d2a26b435eb014a411768ab0fecfcf47b1d80d1350cc35a7e37d2effae6dac
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/25/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53d2a26b435eb014a411768ab0fecfcf47b1d80d1350cc35a7e37d2effae6dac"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/22/bookmark
Content-Type: application/json
Authorization: Bearer 66ed6c8c12157b73e1b04a6dd5c092e7f634324349edb3e10cd7d3dff315a949
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66ed6c8c12157b73e1b04a6dd5c092e7f634324349edb3e10cd7d3dff315a949"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/21
Content-Type: application/json
Authorization: Bearer 5c36daefe1f85cf244e85240ac5236147a515ff4780864412f41f7618b8fa8f2
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":21,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-14T16:47:00.281Z","updated_at":"2016-12-14T16:47:00.368Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":29,"author_id":118,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 21,
    "obfuscated_id": "XIvx1qd7-fY",
    "author_id": 118,
    "chapter_id": 29,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-14T16:47:00.458Z",
    "created_at": "2016-12-14T16:47:00.281Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x0000000d083b00>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 43,
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
curl "api.goskive.com/v2/questions/21" -d '{"question":{"question":{"id":21,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-14T16:47:00.281Z","updated_at":"2016-12-14T16:47:00.368Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":29,"author_id":118,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c36daefe1f85cf244e85240ac5236147a515ff4780864412f41f7618b8fa8f2"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/2/upvote
Content-Type: application/json
Authorization: Bearer 09ed96654d2e73c530a3999bc36ac87a870852321f3a849e6d399ea693833aa2
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/2/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09ed96654d2e73c530a3999bc36ac87a870852321f3a849e6d399ea693833aa2"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer f25725fac21563d7f97377eac7f4e99b79beae9521123655098a0839483f0765
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
      "creator_id": 136,
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "discipline_id": 41,
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
      "updated_at": "2016-12-14T16:47:02.730Z",
      "shortname": "mit-pizza-201",
      "topic_id": 41,
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
	-H "Authorization: Bearer f25725fac21563d7f97377eac7f4e99b79beae9521123655098a0839483f0765"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer c48c7de13f105d73dbc5dac8c7bec411a6ec2547cf620bbe0a4674136028a973
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
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-41",
      "html_url": "https://goskive.com/university/uni-41",
      "slug": "uni-41",
      "name": "National School of Pizza",
      "short_name": "Uni 41",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/70f816b598aa4fe360d3235c0e60128f.jpg",
      "image_thumb_url": "memory://universities/c66cce6f6c08e58245fb42cf638addd3.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-14T16:47:02.452Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 40,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-40",
      "html_url": "https://goskive.com/university/uni-40",
      "slug": "uni-40",
      "name": "National School of Pastry",
      "short_name": "Uni 40",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/f83dba65ad505f8e924a700bb71de700.jpg",
      "image_thumb_url": "memory://universities/bf73789cdc6c22ed7799b8cd1ad08b3b.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-14T16:47:02.407Z",
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
	-H "Authorization: Bearer c48c7de13f105d73dbc5dac8c7bec411a6ec2547cf620bbe0a4674136028a973"
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
      "id": 314,
      "name": "Quality-focused background moratorium",
      "name_translations": {
        "en": "Quality-focused background moratorium"
      },
      "discipline_id": 315
    },
    {
      "id": 315,
      "name": "Self-enabling 3rd generation encryption",
      "name_translations": {
        "en": "Self-enabling 3rd generation encryption"
      },
      "discipline_id": 316
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
GET /v2/topics/316
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
    "id": 316,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 317
  }
}
```



```shell
curl "api.goskive.com/v2/topics/316" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer d62ac245685078f241b063105babdfa4c98b401df8df746505474a764a9c4a2f
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
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-206",
      "html_url": "https://goskive.com/university/uni-206",
      "slug": "uni-206",
      "name": "University 150",
      "short_name": "Uni 206",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/7e899ea4c3ae688a456ea877acb6afff.jpg",
      "image_thumb_url": "memory://universities/685298e5b1732617219bdd786827f811.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-14T16:47:56.884Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-207",
      "html_url": "https://goskive.com/university/uni-207",
      "slug": "uni-207",
      "name": "University 151",
      "short_name": "Uni 207",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/3276e5bad95850d8fcb7a9081c51f3b0.jpg",
      "image_thumb_url": "memory://universities/b5c3217f5b3c5f53770187b7b5898bec.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-14T16:47:56.930Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-208",
      "html_url": "https://goskive.com/university/uni-208",
      "slug": "uni-208",
      "name": "University 152",
      "short_name": "Uni 208",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/f74fb39685f6ab8f727a5ad3ddf6545a.jpg",
      "image_thumb_url": "memory://universities/cd43e25720d51efcc7a6ce1e4b22d87c.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-14T16:47:56.977Z",
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
	-H "Authorization: Bearer d62ac245685078f241b063105babdfa4c98b401df8df746505474a764a9c4a2f"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer d7b97fddae5d125dd02b01ef02254ed792951840c175af0b4c0eee1cee6ad387
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
    "id": 224,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/67dfbc47cb3090e53eeaf62518aff7ce.jpg",
    "image_thumb_url": "memory://universities/c16fd7690b3980a3e0ba0fe5660115f1.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-14T16:47:56.697Z",
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
	-H "Authorization: Bearer d7b97fddae5d125dd02b01ef02254ed792951840c175af0b4c0eee1cee6ad387"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4cd2e6832453c45d8bf12d558ebadb206fa503bcd30122fcf154ca3397882a36
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":155,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 434,
    "id": 155,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 134,
    "additional_university_ids": [

    ],
    "discipline_id": 155,
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
    "chapters_updated_at": "2016-12-14T16:47:27.816Z",
    "updated_at": "2016-12-14T16:47:27.954Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 103,
        "updated_at": "2016-12-14T16:47:27.942Z",
        "course_id": 155,
        "author_id": 434,
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
        "id": 104,
        "updated_at": "2016-12-14T16:47:27.956Z",
        "course_id": 155,
        "author_id": 434,
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
        "id": 105,
        "updated_at": "2016-12-14T16:47:27.970Z",
        "course_id": 155,
        "author_id": 434,
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
    "topic_id": 155,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":155,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cd2e6832453c45d8bf12d558ebadb206fa503bcd30122fcf154ca3397882a36"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 542ca5c5c63f61e7221c89afc2db6cfaebf2e023f2284a45a9a00ffda45fd0ca
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":154,"published":false}}
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
    "creator_id": 433,
    "id": 154,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 133,
    "additional_university_ids": [

    ],
    "discipline_id": 154,
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
    "updated_at": "2016-12-14T16:47:27.772Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 154,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":154,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 542ca5c5c63f61e7221c89afc2db6cfaebf2e023f2284a45a9a00ffda45fd0ca"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 58c1a396004e4b34e28882a25e5e74de2ab817670de5e4a18dfbc48c5df73ae2
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
      "creator_id": 391,
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-81",
      "html_url": "https://goskive.com/course/fu-course-81",
      "slug": "fu-course-81",
      "university_id": 117,
      "additional_university_ids": [

      ],
      "discipline_id": 118,
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
      "updated_at": "2016-12-14T16:47:23.641Z",
      "shortname": "fu-course-81",
      "topic_id": 118,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 81",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 391,
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-82",
      "html_url": "https://goskive.com/course/fu-course-82",
      "slug": "fu-course-82",
      "university_id": 117,
      "additional_university_ids": [

      ],
      "discipline_id": 119,
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
      "chapters_updated_at": "2016-12-14T16:47:23.481Z",
      "updated_at": "2016-12-14T16:47:23.923Z",
      "shortname": "fu-course-82",
      "topic_id": 119,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 82",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58c1a396004e4b34e28882a25e5e74de2ab817670de5e4a18dfbc48c5df73ae2"
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
      "creator_id": 401,
      "id": 126,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-89",
      "html_url": "https://goskive.com/course/fu-course-89",
      "slug": "fu-course-89",
      "university_id": 120,
      "additional_university_ids": [

      ],
      "discipline_id": 126,
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
      "updated_at": "2016-12-14T16:47:24.537Z",
      "shortname": "fu-course-89",
      "topic_id": 126,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 401,
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-90",
      "html_url": "https://goskive.com/course/fu-course-90",
      "slug": "fu-course-90",
      "university_id": 120,
      "additional_university_ids": [

      ],
      "discipline_id": 127,
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
      "chapters_updated_at": "2016-12-14T16:47:24.381Z",
      "updated_at": "2016-12-14T16:47:24.822Z",
      "shortname": "fu-course-90",
      "topic_id": 127,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 90",
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
Authorization: Bearer 67fe846c0ebd81b7f1994230e4a25c165d870260d6cd7c3cffa31d0abbc73343
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
      "creator_id": 398,
      "id": 122,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-85",
      "html_url": "https://goskive.com/course/fu-course-85",
      "slug": "fu-course-85",
      "university_id": 119,
      "additional_university_ids": [

      ],
      "discipline_id": 122,
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
      "updated_at": "2016-12-14T16:47:24.257Z",
      "shortname": "fu-course-85",
      "topic_id": 122,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 85",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 398,
      "id": 123,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-86",
      "html_url": "https://goskive.com/course/fu-course-86",
      "slug": "fu-course-86",
      "university_id": 119,
      "additional_university_ids": [

      ],
      "discipline_id": 123,
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
      "updated_at": "2016-12-14T16:47:24.291Z",
      "shortname": "fu-course-86",
      "topic_id": 123,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 86",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67fe846c0ebd81b7f1994230e4a25c165d870260d6cd7c3cffa31d0abbc73343"
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
      "creator_id": 406,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-93",
      "html_url": "https://goskive.com/course/fu-course-93",
      "slug": "fu-course-93",
      "university_id": 122,
      "additional_university_ids": [

      ],
      "discipline_id": 130,
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
      "updated_at": "2016-12-14T16:47:25.075Z",
      "shortname": "fu-course-93",
      "topic_id": 130,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 93",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 406,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-94",
      "html_url": "https://goskive.com/course/fu-course-94",
      "slug": "fu-course-94",
      "university_id": 122,
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
      "updated_at": "2016-12-14T16:47:25.108Z",
      "shortname": "fu-course-94",
      "topic_id": 131,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 94",
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
Authorization: Bearer c2a1bcb43d5250e2c60357064e3a134b542707bdcdf499f48e7725e112652631
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
  "id": 770,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-14T16:47:57.429Z",
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
	-H "Authorization: Bearer c2a1bcb43d5250e2c60357064e3a134b542707bdcdf499f48e7725e112652631"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/590
Content-Type: application/json
Authorization: Bearer 694990d4ce0b0fc91530129e1c54830e20b2ce3932fe33d0f7d94166dac2af40
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
    "id": 590,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 173,
    "fields_of_study": [
      194,
      195
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-14T16:47:39.580Z",
    "updated_at": "2016-12-14T16:47:39.580Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/590" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 694990d4ce0b0fc91530129e1c54830e20b2ce3932fe33d0f7d94166dac2af40"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/588
Content-Type: application/json
Authorization: Bearer 0d1dd2ed82c4797a6e91d5f2fde5ca0c01291f67f64f064313c8e42b51438d27
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
    "id": 588,
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
    "created_at": "2016-12-14T16:47:39.410Z",
    "updated_at": "2016-12-14T16:47:39.410Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/588" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d1dd2ed82c4797a6e91d5f2fde5ca0c01291f67f64f064313c8e42b51438d27"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 97e1721279d70ddaa6cb67b39fdc1a516abac7f84c0bef16b8ecba44eb44fe10
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
	-H "Authorization: Bearer 97e1721279d70ddaa6cb67b39fdc1a516abac7f84c0bef16b8ecba44eb44fe10"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/11
Content-Type: application/json
Authorization: Bearer 0f6a56bd8a44253130d408c917861b938b0dcfe2de45e126a4da831aab327e4d
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
    "id": 11,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 49,
    "user_id": 382
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f6a56bd8a44253130d408c917861b938b0dcfe2de45e126a4da831aab327e4d"
```
