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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"eab2a2b8fc4635f6e6dd4531145084c9a28a0c63598342b6c9beb5e52c256fa9","client_secret":"2797094527e1444fefeb111d886fb3fbd8371da1f16c34f1283cf7e7bb4a7679"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"eab2a2b8fc4635f6e6dd4531145084c9a28a0c63598342b6c9beb5e52c256fa9","client_secret":"2797094527e1444fefeb111d886fb3fbd8371da1f16c34f1283cf7e7bb4a7679"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NDIyYzE4ZWFmOTZhZGI3MDExYTBjYTZhZjZjZWYxOWRhMzE1Zjk1NDA2OWQ0
YWI3MDc5NzkwMDNlNWJiODM4ZjpjOTQ4N2UxZGVmOGEwN2M5NjRlNDllNDY4
MmFlYzRmMGNmYzQzYTNkMDEwOGI5YWE4ZmM0ODI2MjIzZjA5MjU0

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
	-u 422c18eaf96adb7011a0ca6af6cef19da315f954069d4ab707979003e5bb838f:c9487e1def8a07c964e49e4682aec4f0cfc43a3d0108b9aa8fc4826223f09254
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"4ec913a4019d26e247129af6add0d4079dbbb6499ed89d5af3c1ad28982d7746","client_secret":"d2923faf4da26d2cb4946d4fc4ccb71bd3191fd588398903f5d1137974c237d4"}
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
  "access_token": "74bd0bd4fecdd4707bcca084c558ef48c3f10d7044f6b206b3feb6f1f6406fb0",
  "token_type": "bearer",
  "created_at": 1478638001
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"4ec913a4019d26e247129af6add0d4079dbbb6499ed89d5af3c1ad28982d7746","client_secret":"d2923faf4da26d2cb4946d4fc4ccb71bd3191fd588398903f5d1137974c237d4"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MzhkZDk1OTlmNjAyZjUzNWFmMGE0OTdhZTRkZTJkMzcwMjJlYzIxZTE2MjI1
ZDk5YTk4ZTVlODRmZWQ4YjQ1Nzo3MThmMDhhZWUzOTFjNjEwMDBhZmE5OWEy
MWZmNjY3YzViNWZhNGYwODQxNDQ3M2JkOTk0NDU1NGNkNjJlMmM3

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
  "access_token": "1f24a9ec9804804d7e0cb5523a50b196177cdf5e095336dad147cd9b3ab3c05c",
  "token_type": "bearer",
  "created_at": 1478638001
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 38dd9599f602f535af0a497ae4de2d37022ec21e16225d99a98e5e84fed8b457:718f08aee391c61000afa99a21ff667c5b5fa4f08414473bd9944554cd62e2c7
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
{"grant_type":"client_credentials","client_id":"af3550b45e2895a764fc01a1da7cc870c96151b1ef4e2ac4c61502d4437e5ddd","client_secret":"5197e840a9ed19d8fa719d70b4287ecbdab056b87c8e3a3e8393d8b38efbe551"}
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
  "access_token": "23015c9ef23667eff586cd9123be2fbd43f6a97fbf1ceb17057cc3f39bec9a99",
  "token_type": "bearer",
  "created_at": 1478638001
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"af3550b45e2895a764fc01a1da7cc870c96151b1ef4e2ac4c61502d4437e5ddd","client_secret":"5197e840a9ed19d8fa719d70b4287ecbdab056b87c8e3a3e8393d8b38efbe551"}' -X POST \
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
Authorization: Bearer d64f874227e823e1b44030bd5383d2c25814c6a65d3cc107e7238b499a372f4e
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
    "company_id": 21,
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
	-H "Authorization: Bearer d64f874227e823e1b44030bd5383d2c25814c6a65d3cc107e7238b499a372f4e"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/138/flashcards
Content-Type: application/json
Authorization: Bearer a10ff3ade0b1ef4ea0d1c9d73aed8b78ec79cd78703ce303b2ace842ad01e831
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":138,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 711,
    "chapter_id": 138,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:36.544Z",
    "created_at": "2016-11-08T20:47:36.544Z",
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
curl "api.goskive.com/v2/chapters/138/flashcards" -d '{"flashcard":{"chapter_id":138,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a10ff3ade0b1ef4ea0d1c9d73aed8b78ec79cd78703ce303b2ace842ad01e831"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/136/flashcards
Content-Type: application/json
Authorization: Bearer 6d56b63a5cfde85f4bc3d404e8090542d7b5491d36772c531499059f05cde6a5
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 703,
      "chapter_id": 136,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:35.997Z",
      "created_at": "2016-11-08T20:47:35.997Z",
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 703,
      "chapter_id": 136,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:36.039Z",
      "created_at": "2016-11-08T20:47:36.039Z",
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 703,
      "chapter_id": 136,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:36.085Z",
      "created_at": "2016-11-08T20:47:36.085Z",
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
curl "api.goskive.com/v2/chapters/136/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d56b63a5cfde85f4bc3d404e8090542d7b5491d36772c531499059f05cde6a5"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/160/questions
Content-Type: application/json
Authorization: Bearer fdedf7502eb3bdbcf93df15cc25b9cb671c14c4ee9f11cd62cb01c81cdfb9eba
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":160,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 99,
    "obfuscated_id": "5fPQ9k37GTc",
    "author_id": 859,
    "chapter_id": 160,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:52.379Z",
    "created_at": "2016-11-08T20:47:52.379Z",
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
        "id": 197,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 198,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 199,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 200,
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
curl "api.goskive.com/v2/chapters/160/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":160,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdedf7502eb3bdbcf93df15cc25b9cb671c14c4ee9f11cd62cb01c81cdfb9eba"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/159/questions
Content-Type: application/json
Authorization: Bearer 3f4651f280f8eff64979618326f1903b954c9ab859a40379753ea8085a57cfee
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":159,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 856,
    "chapter_id": 159,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:51.780Z",
    "created_at": "2016-11-08T20:47:51.780Z",
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
        "id": 195,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 196,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/159/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":159,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f4651f280f8eff64979618326f1903b954c9ab859a40379753ea8085a57cfee"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/162/questions
Content-Type: application/json
Authorization: Bearer f1cfb462c51c33a1a105b94c8f0b0c9dab20552a2dacae4de7ef3e0898aaa709
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":162,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 101,
    "obfuscated_id": "PprZyBVq_gc",
    "author_id": 865,
    "chapter_id": 162,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:53.727Z",
    "created_at": "2016-11-08T20:47:53.727Z",
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
        "id": 204,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 205,
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
curl "api.goskive.com/v2/chapters/162/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":162,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1cfb462c51c33a1a105b94c8f0b0c9dab20552a2dacae4de7ef3e0898aaa709"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/161/questions
Content-Type: application/json
Authorization: Bearer b63db7fbb0351081056377322752d1167903c72d5444222f5e183bd568156931
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":161,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 100,
    "obfuscated_id": "erXmBhoMZFI",
    "author_id": 862,
    "chapter_id": 161,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:53.155Z",
    "created_at": "2016-11-08T20:47:53.155Z",
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
        "id": 201,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 202,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 203,
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
curl "api.goskive.com/v2/chapters/161/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":161,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b63db7fbb0351081056377322752d1167903c72d5444222f5e183bd568156931"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/158/questions
Content-Type: application/json
Authorization: Bearer b6da854e285ddbde57d23e7ef51f13ae84b814a4d553251c43c772cda1aac409
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
      "id": 95,
      "obfuscated_id": "uTOhBSQK4CI",
      "author_id": 850,
      "chapter_id": 158,
      "position": 95,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:51.095Z",
      "created_at": "2016-11-08T20:47:50.966Z",
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
      "id": 96,
      "obfuscated_id": "SEtQvXxfwHo",
      "author_id": 851,
      "chapter_id": 158,
      "position": 96,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:51.306Z",
      "created_at": "2016-11-08T20:47:51.173Z",
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
          "id": 191,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 192,
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
      "author_id": 852,
      "chapter_id": 158,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T20:47:51.518Z",
      "created_at": "2016-11-08T20:47:51.382Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/158/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6da854e285ddbde57d23e7ef51f13ae84b814a4d553251c43c772cda1aac409"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/43
Content-Type: application/json
Authorization: Bearer f4fb78c8ae8973f8b4c2c042e377b39173b96e7d4643cd53f7e1de1e6542dadb
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
	-H "Authorization: Bearer f4fb78c8ae8973f8b4c2c042e377b39173b96e7d4643cd53f7e1de1e6542dadb"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/45
Content-Type: application/json
Authorization: Bearer e467b545fa62819a1f0f961543fa8f750782a6380ea429f87b6e8c81383223d9
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
curl "api.goskive.com/v2/chapters/45" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e467b545fa62819a1f0f961543fa8f750782a6380ea429f87b6e8c81383223d9"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/48
Content-Type: application/json
Authorization: Bearer 286372ea72987007def21aa48e9ecab9784e35740dc7c2f4420cecde559663d7
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
curl "api.goskive.com/v2/chapters/48" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 286372ea72987007def21aa48e9ecab9784e35740dc7c2f4420cecde559663d7"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/44
Content-Type: application/json
Authorization: Bearer 6b2f13397b116de73c5601eab5e609e52c2cd4c6e8f2b7284d3c4eec442cd580
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b2f13397b116de73c5601eab5e609e52c2cd4c6e8f2b7284d3c4eec442cd580"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/46
Content-Type: application/json
Authorization: Bearer e5d9bc156d766cec7da555886ee9842b36d880c15de8f7b3ec3967a6233e17f0
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
    "id": 46,
    "updated_at": "2016-11-08T20:46:58.267Z",
    "course_id": 86,
    "author_id": 191,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-08T20:46:57.750Z",
    "questions_updated_at": "2016-11-08T20:46:57.750Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 195,
        "chapter_id": 46,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.250Z",
        "created_at": "2016-11-08T20:46:58.250Z",
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
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 193,
        "chapter_id": 46,
        "position": 21,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:46:58.148Z",
        "created_at": "2016-11-08T20:46:58.032Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5d9bc156d766cec7da555886ee9842b36d880c15de8f7b3ec3967a6233e17f0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/49
Content-Type: application/json
Authorization: Bearer cd26da0cb4488beba93b91e747f3a1ec55d4bb5d6df18879c49fdfc890da1194
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
    "id": 49,
    "updated_at": "2016-11-08T20:46:59.193Z",
    "course_id": 89,
    "author_id": 208,
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
curl "api.goskive.com/v2/chapters/49" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd26da0cb4488beba93b91e747f3a1ec55d4bb5d6df18879c49fdfc890da1194"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/57/replies
Content-Type: application/json
Authorization: Bearer 4ca91670e00f02ca7e999c41aa2da5051392d5547b769ac39c4f2d2359ae625d
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
    "id": 58,
    "author_id": 828,
    "reply_to_id": 57,
    "created_at": "2016-11-08T20:47:49.707Z",
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
curl "api.goskive.com/v2/comments/57/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ca91670e00f02ca7e999c41aa2da5051392d5547b769ac39c4f2d2359ae625d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer cb1d0b3f4e829ce04e36b92684973bba9b28e433451683a073f2fdea7c97c7c7
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
curl "api.goskive.com/v2/comments/56/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb1d0b3f4e829ce04e36b92684973bba9b28e433451683a073f2fdea7c97c7c7"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/45
Content-Type: application/json
Authorization: Bearer 7667e47d7b0fa9d62a675d4400c63f7dacb40c8b97828bec5240068036f695e6
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
curl "api.goskive.com/v2/comments/45" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7667e47d7b0fa9d62a675d4400c63f7dacb40c8b97828bec5240068036f695e6"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/42/republish
Content-Type: application/json
Authorization: Bearer 9a69fe3c31a617dc201dae918e623087594b00ad39e9b2cf1e84673575e6e182
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
curl "api.goskive.com/v2/comments/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a69fe3c31a617dc201dae918e623087594b00ad39e9b2cf1e84673575e6e182"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/46
Content-Type: application/json
Authorization: Bearer 3d2324c4d189352c4fcfdc21124d429e0a0d90560b1f6646756fe9bd0a659c87
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
	-H "Authorization: Bearer 3d2324c4d189352c4fcfdc21124d429e0a0d90560b1f6646756fe9bd0a659c87"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/43/report
Content-Type: application/json
Authorization: Bearer 2a78ad2ce61e0ae8191abd171dcda20c046d3714b94dc387238b344997618cd8
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/43/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a78ad2ce61e0ae8191abd171dcda20c046d3714b94dc387238b344997618cd8"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 6ba0de96ee6b10e46954c5c7c1830e5ee76ec9675f4a3c413857980d2080119b
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
    "id": 36,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-08T20:47:30.222Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ba0de96ee6b10e46954c5c7c1830e5ee76ec9675f4a3c413857980d2080119b"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 5e46e70d4b9127d6c6f2fb00550d785c4498d46ca84899b6fcc4cb141cebda05
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
      "id": 37,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T20:47:30.334Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T20:47:30.338Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T20:47:30.342Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e46e70d4b9127d6c6f2fb00550d785c4498d46ca84899b6fcc4cb141cebda05"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/35/company_profiles
Content-Type: application/json
Authorization: Bearer cfbcc822cf0c50c610f50736ca3b5c132254c19d60fe0c47185578a8cecd350d
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
	-H "Authorization: Bearer cfbcc822cf0c50c610f50736ca3b5c132254c19d60fe0c47185578a8cecd350d"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/33/company_profiles
Content-Type: application/json
Authorization: Bearer 3350474893a26bdddf14c49d3bd64274ffa8c8f1d1b4ad167337d454264ec5ae
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
curl "api.goskive.com/v2/companies/33/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3350474893a26bdddf14c49d3bd64274ffa8c8f1d1b4ad167337d454264ec5ae"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer a5c5e400613414b9b80ba99982716f8ce1030dfe75e0f5497ee34adb59bf036e
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
      "id": 4,
      "title": "Campaign 4",
      "company_id": 9,
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
    },
    {
      "id": 7,
      "title": "Campaign 7",
      "company_id": 12,
      "precluded_campaign_ids": [

      ],
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
	-H "Authorization: Bearer a5c5e400613414b9b80ba99982716f8ce1030dfe75e0f5497ee34adb59bf036e"
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
Authorization: Bearer abb5036d770ec5e91c78a6f0d7875205f3200b19283f9bc163a3ca6b3f3cd9b6
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
	-H "Authorization: Bearer abb5036d770ec5e91c78a6f0d7875205f3200b19283f9bc163a3ca6b3f3cd9b6"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5568c0ff5e8a21449eb3cb3031b415acb01ff4661298e7f240a1d7df91a1e5a8
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
    "id": 24,
    "updated_at": "2016-11-08T20:46:44.766Z",
    "course_id": 14,
    "author_id": 58,
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
	-H "Authorization: Bearer 5568c0ff5e8a21449eb3cb3031b415acb01ff4661298e7f240a1d7df91a1e5a8"
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
      "id": 7,
      "updated_at": "2016-11-08T20:46:42.589Z",
      "course_id": 4,
      "author_id": 22,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 7",
      "position": 1
    },
    {
      "id": 8,
      "updated_at": "2016-11-08T20:46:42.612Z",
      "course_id": 4,
      "author_id": 23,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 8",
      "position": 2
    },
    {
      "id": 9,
      "updated_at": "2016-11-08T20:46:42.856Z",
      "course_id": 4,
      "author_id": 24,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T20:46:42.516Z",
      "questions_updated_at": "2016-11-08T20:46:42.516Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 9",
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
Authorization: Bearer d14bf1b3077457d3cc0501467971d3edde59223509db591fd893dfbf50a67b25
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
      "id": 13,
      "updated_at": "2016-11-08T20:46:43.214Z",
      "course_id": 7,
      "author_id": 33,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 13",
      "position": 1
    },
    {
      "id": 14,
      "updated_at": "2016-11-08T20:46:43.237Z",
      "course_id": 7,
      "author_id": 34,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 14",
      "position": 2
    },
    {
      "id": 15,
      "updated_at": "2016-11-08T20:46:43.486Z",
      "course_id": 7,
      "author_id": 35,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T20:46:43.141Z",
      "questions_updated_at": "2016-11-08T20:46:43.141Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 15",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d14bf1b3077457d3cc0501467971d3edde59223509db591fd893dfbf50a67b25"
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
      "id": 10,
      "updated_at": "2016-11-08T20:46:43.050Z",
      "course_id": 6,
      "author_id": 29,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 10",
      "position": 1
    },
    {
      "id": 11,
      "updated_at": "2016-11-08T20:46:43.074Z",
      "course_id": 6,
      "author_id": 30,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 11",
      "position": 2
    },
    {
      "id": 12,
      "updated_at": "2016-11-08T20:46:43.098Z",
      "course_id": 6,
      "author_id": 31,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 12",
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
Authorization: Bearer b17fc9edff7bb07e3edba8220fe5cd4bee091a2a41ecff13d88fb126b9bd3d3d
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
      "id": 16,
      "updated_at": "2016-11-08T20:46:43.748Z",
      "course_id": 9,
      "author_id": 42,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 16",
      "position": 1
    },
    {
      "id": 17,
      "updated_at": "2016-11-08T20:46:43.770Z",
      "course_id": 9,
      "author_id": 43,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 17",
      "position": 2
    },
    {
      "id": 18,
      "updated_at": "2016-11-08T20:46:43.793Z",
      "course_id": 9,
      "author_id": 44,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 18",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b17fc9edff7bb07e3edba8220fe5cd4bee091a2a41ecff13d88fb126b9bd3d3d"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d8f085845d3b8b037f6c9567726f5dd9a847c3ee37ec84cf4ce80417165b1e19
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
    "course_id": 273,
    "user_id": 842,
    "updated_at": "2016-11-08T20:47:50.565Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8f085845d3b8b037f6c9567726f5dd9a847c3ee37ec84cf4ce80417165b1e19"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 41dfbe2091e54fa441b95b8f4c445b70bd6b3bf3d3ac5f8549297f02e3c8ee80
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
      "id": 2,
      "course_id": 269,
      "user_id": 830,
      "updated_at": "2016-11-08T20:47:49.936Z"
    },
    {
      "id": 3,
      "course_id": 269,
      "user_id": 831,
      "updated_at": "2016-11-08T20:47:49.952Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41dfbe2091e54fa441b95b8f4c445b70bd6b3bf3d3ac5f8549297f02e3c8ee80"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/64/files
Content-Type: application/json
Authorization: Bearer 0e4c8a631520b3ffc03b58ef814760fbaa8d7714e40bad2a5acb0e984ea00afc
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
        "id": 123,
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
        "created_at": "2016-11-08T20:46:50.853Z",
        "updated_at": "2016-11-08T20:46:50.853Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T20:46:50.866Z",
      "updated_at": "2016-11-08T20:46:50.866Z",
      "course_id": 64,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 124,
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
        "created_at": "2016-11-08T20:46:50.873Z",
        "updated_at": "2016-11-08T20:46:50.873Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T20:46:50.883Z",
      "updated_at": "2016-11-08T20:46:50.883Z",
      "course_id": 64,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 125,
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
        "created_at": "2016-11-08T20:46:50.890Z",
        "updated_at": "2016-11-08T20:46:50.890Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T20:46:50.899Z",
      "updated_at": "2016-11-08T20:46:50.899Z",
      "course_id": 64,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/64/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e4c8a631520b3ffc03b58ef814760fbaa8d7714e40bad2a5acb0e984ea00afc"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/63/files
Content-Type: application/json
Authorization: Bearer acabb39dffcbeee5675c129df492e396d7a4db8f79bb855724486e5808bd6195
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
    "id": 1,
    "uploader": {
      "id": 121,
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
      "created_at": "2016-11-08T20:46:50.611Z",
      "updated_at": "2016-11-08T20:46:50.611Z"
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
    "created_at": "2016-11-08T20:46:50.667Z",
    "updated_at": "2016-11-08T20:46:50.667Z",
    "course_id": 63,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/63/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer acabb39dffcbeee5675c129df492e396d7a4db8f79bb855724486e5808bd6195"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/62/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 9c06cf42ae8f8aaf5b1ffcd4a2cd827cab019ce4726e544b3124719fb0259acf
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
    "key": "cache/08a89a06cd39676b38ea432f3ad7fb9f.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQyMTo0Njo1MFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzA4YTg5YTA2Y2QzOTY3NmIzOGVhNDMyZjNhZDdmYjlmLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA4VDIwNDY1MFoifV19",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T204650Z",
    "x-amz-signature": "7cbd57d7886631c68e99db503faeb50f10a401cb17d3f9791bcdb43022bb7664"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/62/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c06cf42ae8f8aaf5b1ffcd4a2cd827cab019ce4726e544b3124719fb0259acf"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer ae2f4526382d7b0153798e20a6e47177584340fc54b0f5e3aa70db8667c0a0aa
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
	-H "Authorization: Bearer ae2f4526382d7b0153798e20a6e47177584340fc54b0f5e3aa70db8667c0a0aa"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a01d6356e82d5545ccf39b76ea8ce53236b7c74a0da66b70cf28c1b6de1520b5
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
	-H "Authorization: Bearer a01d6356e82d5545ccf39b76ea8ce53236b7c74a0da66b70cf28c1b6de1520b5"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6c6b92d89e62ad306674521b26905672dc6bb1c432cb99b376932dfe046d6f5c
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
	-H "Authorization: Bearer 6c6b92d89e62ad306674521b26905672dc6bb1c432cb99b376932dfe046d6f5c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1b98b7cb2527e3b5d1bce327988fa643ca5c44e7a6eebc32938ae23f1b014ea8
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
	-H "Authorization: Bearer 1b98b7cb2527e3b5d1bce327988fa643ca5c44e7a6eebc32938ae23f1b014ea8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b81ece3606462ef1502dd3d0060e3e6a1e5f1717134e4fdd3732fd0931f04240
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
	-H "Authorization: Bearer b81ece3606462ef1502dd3d0060e3e6a1e5f1717134e4fdd3732fd0931f04240"
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
    "creator_id": 761,
    "id": 247,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 232,
    "additional_university_ids": [

    ],
    "discipline_id": 260,
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
    "chapters_updated_at": "2016-11-08T20:47:40.715Z",
    "updated_at": "2016-11-08T20:47:42.293Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 761,
        "chapter_id": 142,
        "position": 73,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:40.939Z",
        "created_at": "2016-11-08T20:47:40.810Z",
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
            "id": 145,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 146,
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
        "author_id": 761,
        "chapter_id": 143,
        "position": 75,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:41.352Z",
        "created_at": "2016-11-08T20:47:41.217Z",
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
            "id": 149,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 150,
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
        "id": 142,
        "updated_at": "2016-11-08T20:47:42.242Z",
        "course_id": 247,
        "author_id": 761,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T20:47:40.715Z",
        "questions_updated_at": "2016-11-08T20:47:40.715Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 124",
        "position": 1
      },
      {
        "id": 143,
        "updated_at": "2016-11-08T20:47:42.285Z",
        "course_id": 247,
        "author_id": 761,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T20:47:40.715Z",
        "questions_updated_at": "2016-11-08T20:47:40.715Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 125",
        "position": 2
      }
    ],
    "topic_id": 259,
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
Authorization: Bearer a168e25d502f09d4527aaa728782b75731bda1f305c33d285e790c2213aaae27
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
    "creator_id": 766,
    "id": 248,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 233,
    "additional_university_ids": [

    ],
    "discipline_id": 261,
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
    "chapters_updated_at": "2016-11-08T20:47:42.353Z",
    "updated_at": "2016-11-08T20:47:43.914Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 767,
        "chapter_id": 144,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:43.694Z",
        "created_at": "2016-11-08T20:47:43.694Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 767,
        "chapter_id": 145,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:43.770Z",
        "created_at": "2016-11-08T20:47:43.770Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 767,
        "chapter_id": 144,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:43.737Z",
        "created_at": "2016-11-08T20:47:43.737Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 767,
        "chapter_id": 145,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:43.812Z",
        "created_at": "2016-11-08T20:47:43.812Z",
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
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 767,
        "chapter_id": 144,
        "position": 79,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:42.584Z",
        "created_at": "2016-11-08T20:47:42.456Z",
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
            "id": 157,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 158,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 767,
        "chapter_id": 144,
        "position": 80,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:42.775Z",
        "created_at": "2016-11-08T20:47:42.653Z",
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
            "id": 159,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 160,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 767,
        "chapter_id": 145,
        "position": 81,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:42.999Z",
        "created_at": "2016-11-08T20:47:42.864Z",
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
            "id": 161,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 162,
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
        "author_id": 767,
        "chapter_id": 145,
        "position": 82,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T20:47:43.198Z",
        "created_at": "2016-11-08T20:47:43.067Z",
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
    "chapters": [
      {
        "id": 144,
        "updated_at": "2016-11-08T20:47:43.865Z",
        "course_id": 248,
        "author_id": 766,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T20:47:42.353Z",
        "questions_updated_at": "2016-11-08T20:47:42.353Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 126",
        "position": 1
      },
      {
        "id": 145,
        "updated_at": "2016-11-08T20:47:43.906Z",
        "course_id": 248,
        "author_id": 766,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T20:47:42.353Z",
        "questions_updated_at": "2016-11-08T20:47:42.353Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 127",
        "position": 2
      }
    ],
    "topic_id": 260,
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
	-H "Authorization: Bearer a168e25d502f09d4527aaa728782b75731bda1f305c33d285e790c2213aaae27"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/245/pin
Content-Type: application/json
Authorization: Bearer a5ca47d95c8c8b8d4bed23153591580c30df77a88a384c103af93201e0d946ff
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/245/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5ca47d95c8c8b8d4bed23153591580c30df77a88a384c103af93201e0d946ff"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/250/pin
Content-Type: application/json
Authorization: Bearer 84c08e8c203f590f2ba25798f2b5b30aa54d32ee68930262879433929a9fc2c5
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/250/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84c08e8c203f590f2ba25798f2b5b30aa54d32ee68930262879433929a9fc2c5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1f7ef707c87dad7ecdc3c5d1c5bc832dee39013e75bbd86835982386d7e784a5
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
    "creator_id": 800,
    "id": 260,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 245,
    "additional_university_ids": [

    ],
    "discipline_id": 273,
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
    "updated_at": "2016-11-08T20:47:47.606Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 272,
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
	-H "Authorization: Bearer 1f7ef707c87dad7ecdc3c5d1c5bc832dee39013e75bbd86835982386d7e784a5"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 56fc146eed11347ed30288e88859b1cac254659d960642773157006ea61bb5fd
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
    "id": 591,
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
    "created_at": "2016-11-08T20:47:27.510Z",
    "updated_at": "2016-11-08T20:47:27.510Z",
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
	-H "Authorization: Bearer 56fc146eed11347ed30288e88859b1cac254659d960642773157006ea61bb5fd"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 629b9bc03cd59f6e7691bda1769b160db909af0657e57d934924b9a9d46c0a1b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[206]}
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
    "id": 586,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      206
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T20:47:26.896Z",
    "updated_at": "2016-11-08T20:47:26.946Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[206]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 629b9bc03cd59f6e7691bda1769b160db909af0657e57d934924b9a9d46c0a1b"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 37ea383092638d0362ff3e3af36f4ffe9e5294c59dea7342d04aaabba548a96b
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
    "id": 589,
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
    "created_at": "2016-11-08T20:47:27.126Z",
    "updated_at": "2016-11-08T20:47:27.126Z",
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
	-H "Authorization: Bearer 37ea383092638d0362ff3e3af36f4ffe9e5294c59dea7342d04aaabba548a96b"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2e202e0ca67f3e35677cc4eaf1965f2f84f611ec14e03f64af0d1bcb5d5ffe63
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[208]}
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
    "id": 588,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      208
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T20:47:27.076Z",
    "updated_at": "2016-11-08T20:47:27.076Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[208]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e202e0ca67f3e35677cc4eaf1965f2f84f611ec14e03f64af0d1bcb5d5ffe63"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 8bfa7754d695fc17331a7ba8e678e0901a6ca75ac82604d31944a348599e6eac
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

210
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
    "id": 590,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9eef34dffd629e3546e70e06cd502e0866167482.jpg",
    "university_id": null,
    "fields_of_study": [
      210
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T20:47:27.220Z",
    "updated_at": "2016-11-08T20:47:27.479Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/7852e92f1b9d9250927c3d89ee433295616feb1e.jpg",
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

210
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 8bfa7754d695fc17331a7ba8e678e0901a6ca75ac82604d31944a348599e6eac"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer b3c760ab9f7499880732a092826717d25e29633471ca29717a0b0ac884dd6a30
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
      "bookmarkable_id": 57,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 58,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 59,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3c760ab9f7499880732a092826717d25e29633471ca29717a0b0ac884dd6a30"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8bb78c5624ae7a44bc0c87d68130f3d3b844effd5402672472e6710fa29a9d5a
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
	-H "Authorization: Bearer 8bb78c5624ae7a44bc0c87d68130f3d3b844effd5402672472e6710fa29a9d5a"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer dce72f4aab2ba256c6eee852627e071d21fb435798806f992e9d3ff0256339d7
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
	-H "Authorization: Bearer dce72f4aab2ba256c6eee852627e071d21fb435798806f992e9d3ff0256339d7"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer c3fcc4dd8ecf2e9800863460b7fd0e03409fc6c0e4f82b6fdb0887e588b142fa
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
      "creator_id": 130,
      "id": 66,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-47",
      "html_url": "https://goskive.com/course/mit-course-47",
      "slug": "mit-course-47",
      "university_id": 44,
      "additional_university_ids": [

      ],
      "discipline_id": 69,
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
      "updated_at": "2016-11-08T20:46:51.154Z",
      "shortname": "mit-course-47",
      "topic_id": 68,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 131,
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-48",
      "html_url": "https://goskive.com/course/mit-course-48",
      "slug": "mit-course-48",
      "university_id": 45,
      "additional_university_ids": [

      ],
      "discipline_id": 70,
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
      "updated_at": "2016-11-08T20:46:51.230Z",
      "shortname": "mit-course-48",
      "topic_id": 69,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 48",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3fcc4dd8ecf2e9800863460b7fd0e03409fc6c0e4f82b6fdb0887e588b142fa"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 8d1658a87450d85797c0645ca9b7b1b901598ca9e5922129e496fcd2274651f3
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
        "created_at": "2016-11-08T20:47:54.300Z",
        "updated_at": "2016-11-08T20:47:54.300Z",
        "file_url": "memory://37b2c79bc3ac2f8c57060446f9c624ed.pdf",
        "course_id": 281,
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
        "created_at": "2016-11-08T20:47:54.376Z",
        "updated_at": "2016-11-08T20:47:54.376Z",
        "file_url": "memory://ebdc15a5e41b61c0ffce517ad2523517.pdf",
        "course_id": 282,
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
        "created_at": "2016-11-08T20:47:54.455Z",
        "updated_at": "2016-11-08T20:47:54.455Z",
        "file_url": "memory://2304f62ce2d3fd7f85356071a609f7f0.pdf",
        "course_id": 283,
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
	-H "Authorization: Bearer 8d1658a87450d85797c0645ca9b7b1b901598ca9e5922129e496fcd2274651f3"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 384c48edd6ff1bccc87d40c4acf5bcb712e7a8fc1f4f618a15b8d25d117fe451
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
      "company_id": 27,
      "company": {
        "id": 27,
        "name": "Fake Company Name 26",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T20:47:12.579Z"
      },
      "created_at": "2016-11-08T20:47:12.582Z",
      "updated_at": "2016-11-08T20:47:12.582Z",
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
      "company_id": 28,
      "company": {
        "id": 28,
        "name": "Fake Company Name 27",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T20:47:12.590Z"
      },
      "created_at": "2016-11-08T20:47:12.593Z",
      "updated_at": "2016-11-08T20:47:12.593Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 384c48edd6ff1bccc87d40c4acf5bcb712e7a8fc1f4f618a15b8d25d117fe451"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 3c42ee7b21545144704ed54d2cd69f9d66cea102e702eb0432d02b124e637ccd
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
      "company_id": 23,
      "company": {
        "id": 23,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T20:47:12.371Z"
      },
      "created_at": "2016-11-08T20:47:12.376Z",
      "updated_at": "2016-11-08T20:47:12.376Z",
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
      "company_id": 24,
      "company": {
        "id": 24,
        "name": "Fake Company Name 23",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T20:47:12.390Z"
      },
      "created_at": "2016-11-08T20:47:12.394Z",
      "updated_at": "2016-11-08T20:47:12.394Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c42ee7b21545144704ed54d2cd69f9d66cea102e702eb0432d02b124e637ccd"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 69bddb3af812ed51f97471e1700624c3589f04be7c1b5f9f9a2af4387ae7070f
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
      "created_at": "2016-11-08T20:47:24.634Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 50,
      "updated_at": "2016-11-08T20:47:24.768Z",
      "author_id": "560",
      "thread_subject_id": "191",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 8,
      "created_at": "2016-11-08T20:47:24.756Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 51,
      "updated_at": "2016-11-08T20:47:24.771Z",
      "author_id": "563",
      "thread_subject_id": "192",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 9,
      "created_at": "2016-11-08T20:47:25.155Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-11-08T20:47:25.155Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-11-08T20:47:25.528Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-11-08T20:47:25.528Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 11,
      "created_at": "2016-11-08T20:47:25.912Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-11-08T20:47:25.912Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 12,
      "created_at": "2016-11-08T20:47:26.220Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 63,
      "updated_at": "2016-11-08T20:47:26.220Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 13,
      "created_at": "2016-11-08T20:47:26.525Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 64,
      "updated_at": "2016-11-08T20:47:26.525Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-11-08T20:47:26.827Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 65,
      "updated_at": "2016-11-08T20:47:26.827Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69bddb3af812ed51f97471e1700624c3589f04be7c1b5f9f9a2af4387ae7070f"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/6
Content-Type: application/json
Authorization: Bearer 7ba7488e55042070bd93c7887228344b09d4ad0f8ad6a168c3a21fd5929d0b18
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-08T20:37:24.000Z"}}
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
    "id": 6,
    "created_at": "2016-11-08T20:47:24.436Z",
    "read_at": "2016-11-08T20:37:24.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 49,
    "updated_at": "2016-11-08T20:47:24.490Z",
    "author_id": "555",
    "thread_subject_id": "190",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/6" -d '{"notification":{"read_at":"2016-11-08T20:37:24.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ba7488e55042070bd93c7887228344b09d4ad0f8ad6a168c3a21fd5929d0b18"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer bcbb831e04dbed0d1ce5fe6015b7fc58c74ab3160041358ed4792486ef1244d5
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
      "course_id": 58,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T20:46:50.087Z",
      "course_published": true,
      "updated_at": "2016-11-08T20:46:50.080Z"
    },
    {
      "id": 3,
      "course_id": 59,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T20:46:50.163Z",
      "course_published": true,
      "updated_at": "2016-11-08T20:46:50.156Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcbb831e04dbed0d1ce5fe6015b7fc58c74ab3160041358ed4792486ef1244d5"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 95052c137cee94df4de1641a0e5d8aaa54e1db3e7eb0840e3be3e09ec964c35c
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
    "course_id": 60,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T20:46:50.283Z",
    "course_published": true,
    "updated_at": "2016-11-08T20:46:50.275Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95052c137cee94df4de1641a0e5d8aaa54e1db3e7eb0840e3be3e09ec964c35c"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer ebb8e4bf3bb80bcc7dd14a5abcd527feb770ea5d48dd2d22472d39e23de986a4
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
    "course_id": 61,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-08T20:46:50.443Z",
    "course_published": true,
    "updated_at": "2016-11-08T20:46:50.431Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebb8e4bf3bb80bcc7dd14a5abcd527feb770ea5d48dd2d22472d39e23de986a4"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 39ee683df7eb197a0ff9f46553e262821de90aeb462f914a89cec5af06791082
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
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 13,
      "user_id": 150
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 14,
      "user_id": 150
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 15,
      "user_id": 150
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 16,
      "user_id": 150
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39ee683df7eb197a0ff9f46553e262821de90aeb462f914a89cec5af06791082"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/16
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
    "id": 16,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 16,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 16
      },
      {
        "id": 17,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 16
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/16" -X GET \
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
      "id": 17,
      "name": "Phased upward-trending hardware",
      "name_translations": {
        "en": "Phased upward-trending hardware"
      }
    },
    {
      "id": 18,
      "name": "Self-enabling bandwidth-monitored workforce",
      "name_translations": {
        "en": "Self-enabling bandwidth-monitored workforce"
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
PATCH /v2/feedbacks/6/close
Content-Type: application/json
Authorization: Bearer 560eafa8c17e449a1913dd3b4134371e20cd7f8722c2a22dab4906dd67827bb6
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
    "id": 6,
    "user_id": 246,
    "feedbackable_id": 17,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-08T20:47:01.607Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/6/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 560eafa8c17e449a1913dd3b4134371e20cd7f8722c2a22dab4906dd67827bb6"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/fix
Content-Type: application/json
Authorization: Bearer 906e2d846967449bbda953a6e5811a56f93af7474d1035ce150a0e1a42639c0b
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
    "id": 3,
    "user_id": 231,
    "feedbackable_id": 14,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-08T20:47:00.640Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/3/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 906e2d846967449bbda953a6e5811a56f93af7474d1035ce150a0e1a42639c0b"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer 3c5654448a537c6833dcdbf0c469a569f364abd35389f202cdc7d3abb9e66470
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
    "user_id": 342,
    "feedbackable_id": 20,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T20:47:08.747Z",
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
curl "api.goskive.com/v2/feedbacks/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c5654448a537c6833dcdbf0c469a569f364abd35389f202cdc7d3abb9e66470"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/2/fix
Content-Type: application/json
Authorization: Bearer 4085d4b814c378ea9aa61cf35814209d0e4e0b67b9ddb0fe9259c3c1c89ecc4a
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
curl "api.goskive.com/v2/feedbacks/2/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4085d4b814c378ea9aa61cf35814209d0e4e0b67b9ddb0fe9259c3c1c89ecc4a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer a76ab3a2781b21b83221ad7f30d910b95bd8d38dc1c112071c815079abe7a8b9
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
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a76ab3a2781b21b83221ad7f30d910b95bd8d38dc1c112071c815079abe7a8b9"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/8/close
Content-Type: application/json
Authorization: Bearer e970f23a29529289c84f88386a7d5c206747d790191dfd27e105e1391b0f8a70
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
curl "api.goskive.com/v2/feedbacks/8/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e970f23a29529289c84f88386a7d5c206747d790191dfd27e105e1391b0f8a70"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/29
Content-Type: application/json
Authorization: Bearer c74a86eb4a362aa8e25f03f4c2cf9493f0e25b5760822eb4f035a7d28de291fd
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
    "id": 29,
    "user_id": 347,
    "feedbackable_id": 21,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T20:47:09.021Z",
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
curl "api.goskive.com/v2/feedbacks/29" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c74a86eb4a362aa8e25f03f4c2cf9493f0e25b5760822eb4f035a7d28de291fd"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer 8f953fcf7bdd07d13cb9648ef4f4d465dbaedcb69a0887378b75dfd65a7779b7
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
curl "api.goskive.com/v2/files/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f953fcf7bdd07d13cb9648ef4f4d465dbaedcb69a0887378b75dfd65a7779b7"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/7/bookmark
Content-Type: application/json
Authorization: Bearer d06486113f7b7cd533d75a120323de11b75108561e5cafdca5c411aa5adba2ee
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d06486113f7b7cd533d75a120323de11b75108561e5cafdca5c411aa5adba2ee"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer 218fccef31712f31dd299a5cb1115afcfeb63388f8a6489277718e5fdc2405e6
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 218fccef31712f31dd299a5cb1115afcfeb63388f8a6489277718e5fdc2405e6"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/15
Content-Type: application/json
Authorization: Bearer 71dc0eac63cd6e00c2c478fde922875338d5c430901a733838c2c6cd02c1c36f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/d59e853537e5cdc9dde38109f140066e.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T204737Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e006298b0b274a49577d997d7aa25d68a46e7ca1d7d3a59c17982fe0b45e702c",
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
	-H "Authorization: Bearer 71dc0eac63cd6e00c2c478fde922875338d5c430901a733838c2c6cd02c1c36f"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/11/preview
Content-Type: application/json
Authorization: Bearer f3ef31815c59b5dfc0004aa00cf4b578edb78ae0b248b50413a6e7bdbc8e0dae
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/f05f0fd60979f6e1f17738866fc9b9cb.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T204737Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=0040c31e17160b9af2c0f59b9426e2abb865d13d45aa91581552247bf6b489d9",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/11/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3ef31815c59b5dfc0004aa00cf4b578edb78ae0b248b50413a6e7bdbc8e0dae"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 8b921e4e162c8388d5b0ba906cfbfc75f366a87dc0230eda790fb0124076a4e8
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
    "id": 8,
    "uploader": {
      "id": 715,
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
      "created_at": "2016-11-08T20:47:36.846Z",
      "updated_at": "2016-11-08T20:47:36.846Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-08T20:47:36.921Z",
    "updated_at": "2016-11-08T20:47:36.921Z",
    "course_id": 232,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b921e4e162c8388d5b0ba906cfbfc75f366a87dc0230eda790fb0124076a4e8"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/5/matched_courses?required_cu_count=2
Authorization: Bearer 3c269b265693b1b073cde203ebd5690d20370b66e270c49a7df3b0291891ad81
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
      "creator_id": 391,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 114,
      "additional_university_ids": [

      ],
      "discipline_id": 138,
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
      "chapters_updated_at": "2016-11-08T20:47:12.685Z",
      "updated_at": "2016-11-08T20:47:14.967Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 137,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 396,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-71488294-268b-47fe-89e0-ffc0f80e72f3",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-71488294-268b-47fe-89e0-ffc0f80e72f3",
      "slug": "mit-the-great-british-bake-off-71488294-268b-47fe-89e0-ffc0f80e72f3",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "discipline_id": 139,
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
      "chapters_updated_at": "2016-11-08T20:47:12.685Z",
      "updated_at": "2016-11-08T20:47:15.554Z",
      "shortname": "mit-the-great-british-bake-off-71488294-268b-47fe-89e0-ffc0f80e72f3",
      "topic_id": 138,
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
curl "api.goskive.com/v2/files/5/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 3c269b265693b1b073cde203ebd5690d20370b66e270c49a7df3b0291891ad81"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/17/download
Content-Type: application/json
Authorization: Bearer 572093e8fb6ee7b31272ac85983839e011c135ceb2627973f5ac83782e5e3c92
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 572093e8fb6ee7b31272ac85983839e011c135ceb2627973f5ac83782e5e3c92"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/18/report
Content-Type: application/json
Authorization: Bearer d6b9b3dd010172a38e32ee4b458ed30e5401e2a297efa1c35cff4e22a0952a15
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6b9b3dd010172a38e32ee4b458ed30e5401e2a297efa1c35cff4e22a0952a15"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/19/bookmark
Content-Type: application/json
Authorization: Bearer ac2bc043973a5c0a229aa6a621f97d58c973694f07ef98fb8085fd96a0520af4
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac2bc043973a5c0a229aa6a621f97d58c973694f07ef98fb8085fd96a0520af4"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/16/upvote
Content-Type: application/json
Authorization: Bearer e58c3f9d3119634face407419e08eb21c774d8be9ac970170cc5c75e28a21ba2
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
	-H "Authorization: Bearer e58c3f9d3119634face407419e08eb21c774d8be9ac970170cc5c75e28a21ba2"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/37/comments
Content-Type: application/json
Authorization: Bearer 4f51820bf333b20bede7afc16cc183b7ee8fa7b4e671ac15c315a29f427e1305
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
    "id": 54,
    "author_id": 620,
    "reply_to_id": null,
    "created_at": "2016-11-08T20:47:31.156Z",
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
curl "api.goskive.com/v2/flashcards/37/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f51820bf333b20bede7afc16cc183b7ee8fa7b4e671ac15c315a29f427e1305"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/38/comments
Content-Type: application/json
Authorization: Bearer 22acde5e4de5fac273366c82effdf04f35171e9256fdb3818a53f69b57351364
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
    "id": 55,
    "author_id": 623,
    "reply_to_id": null,
    "created_at": "2016-11-08T20:47:31.466Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 623,
      "feedbackable_id": 38,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:31.462Z",
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
curl "api.goskive.com/v2/flashcards/38/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22acde5e4de5fac273366c82effdf04f35171e9256fdb3818a53f69b57351364"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/34/comments
Content-Type: application/json
Authorization: Bearer 678e4ecef87980bef7520fb3eaebe6cfcefc791084468e755f264c7ac36ee585
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
      "id": 53,
      "author_id": 613,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:30.560Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 612,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:47:30.544Z",
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
curl "api.goskive.com/v2/flashcards/34/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 678e4ecef87980bef7520fb3eaebe6cfcefc791084468e755f264c7ac36ee585"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/36/comments
Content-Type: application/json
Authorization: Bearer a4e66fed14c5fa9f7dc8452d2e9112f353a434f2827acf580145773090646208
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
curl "api.goskive.com/v2/flashcards/36/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4e66fed14c5fa9f7dc8452d2e9112f353a434f2827acf580145773090646208"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/26/feedbacks
Content-Type: application/json
Authorization: Bearer 736e6ee641ddefea5a3c18f6015a42c2012b1d9df80bb4725deeccd8d4f19db0
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
    "id": 30,
    "user_id": 506,
    "feedbackable_id": 26,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T20:47:21.781Z",
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
curl "api.goskive.com/v2/flashcards/26/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 736e6ee641ddefea5a3c18f6015a42c2012b1d9df80bb4725deeccd8d4f19db0"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/29/feedbacks
Content-Type: application/json
Authorization: Bearer fa9cb3fd7d5c1beb5f55ecd9064d8832730d753add9cafb4b73074ccd5b5c558
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
      "id": 33,
      "user_id": 519,
      "feedbackable_id": 29,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:22.556Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 518,
      "feedbackable_id": 29,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:47:22.546Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/29/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa9cb3fd7d5c1beb5f55ecd9064d8832730d753add9cafb4b73074ccd5b5c558"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/95/votes
Content-Type: application/json
Authorization: Bearer 43d420e569f72eb97734628ef2a563b3fcce89ebcc890d41eea92f6cca542331
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
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 95,
      "user_id": 818
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 95,
      "user_id": 817
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 95,
      "user_id": 816
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/95/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43d420e569f72eb97734628ef2a563b3fcce89ebcc890d41eea92f6cca542331"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/58/republish
Content-Type: application/json
Authorization: Bearer 28ab61226d2274c62ad6cb34316bb5cb56aa48ae733c98297dae6d3d57a1777a
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
curl "api.goskive.com/v2/flashcards/58/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28ab61226d2274c62ad6cb34316bb5cb56aa48ae733c98297dae6d3d57a1777a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/bookmark
Content-Type: application/json
Authorization: Bearer 48a32680b5fe7a298c56a07a225c6417be8bad4382093a72805fbdc478baa539
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48a32680b5fe7a298c56a07a225c6417be8bad4382093a72805fbdc478baa539"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/60
Content-Type: application/json
Authorization: Bearer c832854c9dd864bfadb59a0b7a821df8f213ddb7337eb7a703ec240294193375
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/60" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c832854c9dd864bfadb59a0b7a821df8f213ddb7337eb7a703ec240294193375"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/57/downvote
Content-Type: application/json
Authorization: Bearer 50fe8bc195f2ccbd8afdec60de1c2ea35d08b3273a20b40f0dc8ab4998d085de
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/57/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50fe8bc195f2ccbd8afdec60de1c2ea35d08b3273a20b40f0dc8ab4998d085de"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/62
Content-Type: application/json
Authorization: Bearer 9f91c7223e97c3a443110c7286681d438099de0c7666d0864c4fdcf9087b38c9
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
    "id": 62,
    "obfuscated_id": "fj_KMGohXD4",
    "author_id": 700,
    "chapter_id": 135,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:47:35.795Z",
    "created_at": "2016-11-08T20:47:35.795Z",
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
curl "api.goskive.com/v2/flashcards/62" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f91c7223e97c3a443110c7286681d438099de0c7666d0864c4fdcf9087b38c9"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/report
Content-Type: application/json
Authorization: Bearer ad9907e57c138af5b73adcfee121524426c9d15f4112d9f86511c8271c868be1
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad9907e57c138af5b73adcfee121524426c9d15f4112d9f86511c8271c868be1"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/39/bookmark
Content-Type: application/json
Authorization: Bearer 94a8a3bf7cd145fa5ca57ab91f314138ebd5c8bb8235ff0f982fe2a9f95ecf7e
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94a8a3bf7cd145fa5ca57ab91f314138ebd5c8bb8235ff0f982fe2a9f95ecf7e"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/61/upvote
Content-Type: application/json
Authorization: Bearer be0551b5dec845cc133217cf415b9ebc5e591f388604c4cdb37ff20841e13e36
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
	-H "Authorization: Bearer be0551b5dec845cc133217cf415b9ebc5e591f388604c4cdb37ff20841e13e36"
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
    "key": "cache/00ca0c282924bb54db2278d735c49b4d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQyMTo0Njo0OVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzAwY2EwYzI4MjkyNGJiNTRkYjIyNzhkNzM1YzQ5YjRkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDhUMjA0NjQ5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T204649Z",
    "x-amz-signature": "13481b286f427f6f64108811537faaa6053c4292469939d925bb5a41c085a3c0"
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
Authorization: Bearer 97ce44ced964b788be12e1bff1f8e3e85be41a3108a7578f65f1a35fd0a3e9b9
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
	-H "Authorization: Bearer 97ce44ced964b788be12e1bff1f8e3e85be41a3108a7578f65f1a35fd0a3e9b9"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer fd4ac5bf6f378e2aa972bb7e59efa16ebfe5003edcedb0a9c8ae4c88ae17a10b
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
	-H "Authorization: Bearer fd4ac5bf6f378e2aa972bb7e59efa16ebfe5003edcedb0a9c8ae4c88ae17a10b"
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
{"password":{"reset_password_token":"4tSnyeyzKETAyTx3YDcV","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 596,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-08T20:47:29.298Z",
  "updated_at": "2016-11-08T20:47:29.427Z",
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
  "audit_id": 5254
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"4tSnyeyzKETAyTx3YDcV","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Authorization: Bearer 6a90eeae4cb85f511d09bd426dbc299b103333ed557e20210f027576f186d28c
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
    "author_id": 147,
    "reply_to_id": null,
    "created_at": "2016-11-08T20:46:53.448Z",
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
	-H "Authorization: Bearer 6a90eeae4cb85f511d09bd426dbc299b103333ed557e20210f027576f186d28c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer 665ea1ec52fef15526a768f7dca2ee07bcbb8e6ae712aac630d4f0901a5ee2fe
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
    "author_id": 144,
    "reply_to_id": null,
    "created_at": "2016-11-08T20:46:52.712Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 144,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:46:52.708Z",
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
curl "api.goskive.com/v2/questions/11/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 665ea1ec52fef15526a768f7dca2ee07bcbb8e6ae712aac630d4f0901a5ee2fe"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/9/comments
Content-Type: application/json
Authorization: Bearer 609737be76b9eec3192641f80e5d5092f5e0156e3af33085e61b0c75bb767b57
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
      "author_id": 139,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:46:51.986Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 140,
      "reply_to_id": null,
      "created_at": "2016-11-08T20:46:52.020Z",
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
curl "api.goskive.com/v2/questions/9/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 609737be76b9eec3192641f80e5d5092f5e0156e3af33085e61b0c75bb767b57"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/10/comments
Content-Type: application/json
Authorization: Bearer 61b6636ecd1d1df9a04849e0416c9f0c046fc9f6c2b7a64c4514fe12d8f2f07f
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
curl "api.goskive.com/v2/questions/10/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61b6636ecd1d1df9a04849e0416c9f0c046fc9f6c2b7a64c4514fe12d8f2f07f"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/127/feedbacks
Content-Type: application/json
Authorization: Bearer 7c03232bc8a1af1bdaf86503b96ece4ef923ca45e6b2884e5043383df4253e30
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
    "user_id": 953,
    "feedbackable_id": 127,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-08T20:48:03.740Z",
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
	-H "Authorization: Bearer 7c03232bc8a1af1bdaf86503b96ece4ef923ca45e6b2884e5043383df4253e30"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/134/feedbacks
Content-Type: application/json
Authorization: Bearer 0bc210350a70ec1fd54eab8d25248c46f639e7c9b44588b3a8832db5fd7dc920
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
      "user_id": 988,
      "feedbackable_id": 134,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:48:06.327Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 987,
      "feedbackable_id": 134,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T20:48:06.317Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/134/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bc210350a70ec1fd54eab8d25248c46f639e7c9b44588b3a8832db5fd7dc920"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/44/votes
Content-Type: application/json
Authorization: Bearer efba6a7484d64c4916ff5ede390ee71d70aae7555df72bdc4a7a67343cd39948
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
      "votable_id": 44,
      "user_id": 359
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 358
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 357
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/44/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer efba6a7484d64c4916ff5ede390ee71d70aae7555df72bdc4a7a67343cd39948"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/124/republish
Content-Type: application/json
Authorization: Bearer 87d46d2dffa7a244fe597b0baad687ff61149080987dcfc9ecfbb316d463ab80
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
curl "api.goskive.com/v2/questions/124/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87d46d2dffa7a244fe597b0baad687ff61149080987dcfc9ecfbb316d463ab80"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/102/bookmark
Content-Type: application/json
Authorization: Bearer fdd0351284e1f2d7b3fc6f2582e7125b6e6f021d6123dd19e611765787d78d20
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/102/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdd0351284e1f2d7b3fc6f2582e7125b6e6f021d6123dd19e611765787d78d20"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/125
Content-Type: application/json
Authorization: Bearer c56b4a6003a5f6f854daad7b9ddac833d77d04a293ffcafa41f02aacd849f497
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/125" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c56b4a6003a5f6f854daad7b9ddac833d77d04a293ffcafa41f02aacd849f497"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/122/downvote
Content-Type: application/json
Authorization: Bearer 0b2b6f94a095110a38568c68872e9e9e06e1b68f617ff548b7a7fd39c8640311
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/122/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b2b6f94a095110a38568c68872e9e9e06e1b68f617ff548b7a7fd39c8640311"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/119
Content-Type: application/json
Authorization: Bearer 98022a201806c98afbe7b88a769b5203f0f3fb31eab2fcaa0997a7cebd87d33a
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
    "id": 119,
    "obfuscated_id": "JRh8sWka24Y",
    "author_id": 929,
    "chapter_id": 180,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:48:00.224Z",
    "created_at": "2016-11-08T20:48:00.108Z",
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
        "id": 240,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 241,
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
curl "api.goskive.com/v2/questions/119" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98022a201806c98afbe7b88a769b5203f0f3fb31eab2fcaa0997a7cebd87d33a"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/120/report
Content-Type: application/json
Authorization: Bearer 4272f102a40e1e83e496db6c4afb346dba19055bb960b65595fe669a67a4155e
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/120/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4272f102a40e1e83e496db6c4afb346dba19055bb960b65595fe669a67a4155e"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/121/bookmark
Content-Type: application/json
Authorization: Bearer 024c7fad0f517957aea7bf9e7597a5e3b06cfb28c8a9438b1ebd011841dfdeab
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/121/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 024c7fad0f517957aea7bf9e7597a5e3b06cfb28c8a9438b1ebd011841dfdeab"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/126
Content-Type: application/json
Authorization: Bearer 9f18efb332c93cc2683e22a114e0c5b29857a56717efb884d5dab1eed7911f66
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":126,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T20:48:02.954Z","updated_at":"2016-11-08T20:48:03.068Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":187,"author_id":950,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 126,
    "obfuscated_id": "fKTMLttUR-w",
    "author_id": 950,
    "chapter_id": 187,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T20:48:03.176Z",
    "created_at": "2016-11-08T20:48:02.954Z",
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
    "question": "{\"id\"=>126, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-08T20:48:02.954Z\", \"updated_at\"=>\"2016-11-08T20:48:03.068Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>187, \"author_id\"=>950, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 256,
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
curl "api.goskive.com/v2/questions/126" -d '{"question":{"question":{"id":126,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T20:48:02.954Z","updated_at":"2016-11-08T20:48:03.068Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":187,"author_id":950,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f18efb332c93cc2683e22a114e0c5b29857a56717efb884d5dab1eed7911f66"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/118/upvote
Content-Type: application/json
Authorization: Bearer 35b902f38155e9d9957ab42736dd09a8e2e24ff5f339c5fad06c2c238f52a25e
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/118/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35b902f38155e9d9957ab42736dd09a8e2e24ff5f339c5fad06c2c238f52a25e"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 81f3bb2058a4928afac2b684983d6151e3354668a127cf7c77d0b175438fc9e5
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
      "creator_id": 406,
      "id": 134,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 117,
      "additional_university_ids": [

      ],
      "discipline_id": 142,
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
      "updated_at": "2016-11-08T20:47:17.083Z",
      "shortname": "mit-pizza-201",
      "topic_id": 141,
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
	-H "Authorization: Bearer 81f3bb2058a4928afac2b684983d6151e3354668a127cf7c77d0b175438fc9e5"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 2413b4fd08bf03c2c543ff0aaadaab4dae8a16b0bd67ad257d044739ba78ed64
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
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-100",
      "html_url": "https://goskive.com/university/uni-100",
      "slug": "uni-100",
      "name": "National School of Pizza",
      "short_name": "Uni 100",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b5c059d79ca15ef51a64141885c41356b7eb6d7f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2ad2f4c4aa6e2cd2c784d7880241d6c1b55f4863.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T20:47:17.373Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-99",
      "html_url": "https://goskive.com/university/uni-99",
      "slug": "uni-99",
      "name": "National School of Pastry",
      "short_name": "Uni 99",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/18b3243e0496f81e57c0841ffc50d1ffea7771fc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8235339619085a5aaf31c8771d17b1288f8e8a68.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T20:47:17.356Z",
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
	-H "Authorization: Bearer 2413b4fd08bf03c2c543ff0aaadaab4dae8a16b0bd67ad257d044739ba78ed64"
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
      "id": 95,
      "name": "Diverse maximized methodology",
      "name_translations": {
        "en": "Diverse maximized methodology"
      },
      "discipline_id": 96
    },
    {
      "id": 96,
      "name": "Function-based maximized product",
      "name_translations": {
        "en": "Function-based maximized product"
      },
      "discipline_id": 97
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
GET /v2/topics/94
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
    "id": 94,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 95
  }
}
```



```shell
curl "api.goskive.com/v2/topics/94" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer be1d04095a9e49d95c78cde40d3244c37c439043f9cdf672ed9aba883946245c
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
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-55",
      "html_url": "https://goskive.com/university/uni-55",
      "slug": "uni-55",
      "name": "University 27",
      "short_name": "Uni 55",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5ea26c0fe407ac9aecae4409b94b03910c0208ce.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9af5cde7ee37bf1949b95d1335e8e2a4af7a4bf8.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T20:47:00.025Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-54",
      "html_url": "https://goskive.com/university/uni-54",
      "slug": "uni-54",
      "name": "University 26",
      "short_name": "Uni 54",
      "acronym": "MIT",
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
      "updated_at": "2016-11-08T20:47:00.009Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-53",
      "html_url": "https://goskive.com/university/uni-53",
      "slug": "uni-53",
      "name": "University 25",
      "short_name": "Uni 53",
      "acronym": "MIT",
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
      "updated_at": "2016-11-08T20:46:59.993Z",
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
	-H "Authorization: Bearer be1d04095a9e49d95c78cde40d3244c37c439043f9cdf672ed9aba883946245c"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 87a858e2fcfd7806d6e8e0480fc47ab91e54342dfe3a6a3724966beae918a390
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
    "id": 75,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2f8af7cfd34b79907d70212c94decefc62b88ac5.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8c7d639ffdd2f7c4104668f024cac41bcabf5f59.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-08T20:47:00.197Z",
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
	-H "Authorization: Bearer 87a858e2fcfd7806d6e8e0480fc47ab91e54342dfe3a6a3724966beae918a390"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 388383fbcf8a029801caf3fa47483ac6b0f270c33fecf3f1844acec3e6ff6b3b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":19,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 62,
    "id": 17,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 17,
    "additional_university_ids": [

    ],
    "discipline_id": 20,
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
    "chapters_updated_at": "2016-11-08T20:46:45.406Z",
    "updated_at": "2016-11-08T20:46:45.565Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 25,
        "updated_at": "2016-11-08T20:46:45.520Z",
        "course_id": 17,
        "author_id": 62,
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
        "id": 26,
        "updated_at": "2016-11-08T20:46:45.538Z",
        "course_id": 17,
        "author_id": 62,
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
        "id": 27,
        "updated_at": "2016-11-08T20:46:45.555Z",
        "course_id": 17,
        "author_id": 62,
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
    "topic_id": 19,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":19,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 388383fbcf8a029801caf3fa47483ac6b0f270c33fecf3f1844acec3e6ff6b3b"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 88b0cdf2c84fc5822262e0d18fcae444b406605d78c5d09d039e229e6723b508
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":20,"published":false}}
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
    "creator_id": 63,
    "id": 18,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 18,
    "additional_university_ids": [

    ],
    "discipline_id": 21,
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
    "updated_at": "2016-11-08T20:46:45.783Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 20,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":20,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88b0cdf2c84fc5822262e0d18fcae444b406605d78c5d09d039e229e6723b508"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2ca1bede4d53ef98621d1bdfdda71d0d9981e9dc6f52f9b5d2d79980d42a7afc
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
      "creator_id": 80,
      "id": 34,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "discipline_id": 37,
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
      "updated_at": "2016-11-08T20:46:47.336Z",
      "shortname": "fu-course-15",
      "topic_id": 36,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 80,
      "id": 35,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "discipline_id": 38,
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
      "chapters_updated_at": "2016-11-08T20:46:47.203Z",
      "updated_at": "2016-11-08T20:46:47.625Z",
      "shortname": "fu-course-16",
      "topic_id": 37,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ca1bede4d53ef98621d1bdfdda71d0d9981e9dc6f52f9b5d2d79980d42a7afc"
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
      "creator_id": 90,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 28,
      "additional_university_ids": [

      ],
      "discipline_id": 45,
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
      "updated_at": "2016-11-08T20:46:48.161Z",
      "shortname": "fu-course-23",
      "topic_id": 44,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 90,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 28,
      "additional_university_ids": [

      ],
      "discipline_id": 46,
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
      "chapters_updated_at": "2016-11-08T20:46:48.022Z",
      "updated_at": "2016-11-08T20:46:48.577Z",
      "shortname": "fu-course-24",
      "topic_id": 45,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
Authorization: Bearer 814114146f3c1a1b32aaeec7939982dc381d22bd289de5d6376464810a08cd1d
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
      "creator_id": 87,
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 27,
      "additional_university_ids": [

      ],
      "discipline_id": 41,
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
      "updated_at": "2016-11-08T20:46:47.879Z",
      "shortname": "fu-course-19",
      "topic_id": 40,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 87,
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 27,
      "additional_university_ids": [

      ],
      "discipline_id": 42,
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
      "updated_at": "2016-11-08T20:46:47.915Z",
      "shortname": "fu-course-20",
      "topic_id": 41,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 814114146f3c1a1b32aaeec7939982dc381d22bd289de5d6376464810a08cd1d"
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
      "creator_id": 95,
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 29,
      "additional_university_ids": [

      ],
      "discipline_id": 49,
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
      "updated_at": "2016-11-08T20:46:48.751Z",
      "shortname": "fu-course-27",
      "topic_id": 48,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 95,
      "id": 47,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 29,
      "additional_university_ids": [

      ],
      "discipline_id": 50,
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
      "updated_at": "2016-11-08T20:46:48.789Z",
      "shortname": "fu-course-28",
      "topic_id": 49,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
Authorization: Bearer e4ce5bb72e46894577588df0be7e7eea9aaa83be4f1693a4fb94ea39a9c4aeef
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
  "id": 363,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-08T20:47:10.437Z",
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
	-H "Authorization: Bearer e4ce5bb72e46894577588df0be7e7eea9aaa83be4f1693a4fb94ea39a9c4aeef"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/217
Content-Type: application/json
Authorization: Bearer b2018375bdd818924b30123e2d65554f340b78a8cd485c9a68e954d53b5bed3c
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
    "id": 217,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 70,
    "fields_of_study": [
      97,
      98
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-08T20:46:59.924Z",
    "updated_at": "2016-11-08T20:46:59.924Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/217" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2018375bdd818924b30123e2d65554f340b78a8cd485c9a68e954d53b5bed3c"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/215
Content-Type: application/json
Authorization: Bearer bd6c255c5fb6ffb37ee8425f66fbc3d1f24303c97958f1b20b0ef9deb880d577
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
    "id": 215,
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
    "created_at": "2016-11-08T20:46:59.771Z",
    "updated_at": "2016-11-08T20:46:59.771Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/215" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd6c255c5fb6ffb37ee8425f66fbc3d1f24303c97958f1b20b0ef9deb880d577"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/11
Content-Type: application/json
Authorization: Bearer e896f15824ca841f93dfbcf53b8b761a2ff332de5ad120432915159445ed4c95
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
	-H "Authorization: Bearer e896f15824ca841f93dfbcf53b8b761a2ff332de5ad120432915159445ed4c95"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/9
Content-Type: application/json
Authorization: Bearer 1cec3c64c370cfd121324d59748f88413d3ca655153ad73c9a30714c7b7a7f74
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
    "id": 9,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 46,
    "user_id": 365
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cec3c64c370cfd121324d59748f88413d3ca655153ad73c9a30714c7b7a7f74"
```
