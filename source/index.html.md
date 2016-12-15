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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0b680d4be6cbf4a8606d189a95d6effc7ebedc11223f9c01db31d82ab6e8db6c","client_secret":"9d58d1cb0bcea43d3521e5c1343ad17d90bf3104ba0bc6509eb901b8ba302595"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0b680d4be6cbf4a8606d189a95d6effc7ebedc11223f9c01db31d82ab6e8db6c","client_secret":"9d58d1cb0bcea43d3521e5c1343ad17d90bf3104ba0bc6509eb901b8ba302595"}' -X POST \
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
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZjhhYjAxNmFhNDM5MjIwNzYyNmZjNmMwN2NmZTVhNjA5MWYzNzViZDgzMjA5
N2EzMTQxMjJiNDFkOTRiY2FkODo1ZDM2NjYwZmE3YjQ1YTM4ZDlmZTg2NDYz
MTQwNTg2ZjI1YWViNGZkOTZjZTFkM2MwYjY2Mjk2YmI5ZmY1OWRh

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
	-u f8ab016aa4392207626fc6c07cfe5a6091f375bd832097a314122b41d94bcad8:5d36660fa7b45a38d9fe86463140586f25aeb4fd96ce1d3c0b66296bb9ff59da
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"66ee22745d31af762c1f5df54dab29723a06bb5f55e46900c58fd6a57415964f","client_secret":"928bd8ead2782725a9dbb661253a8bbba7e2dc0062a06b9cf453c4a8801aeb93"}
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
  "access_token": "533afc6b0da7d3d2ffecc69108118c205e4db0e1f3efb01fb478b68280984568",
  "token_type": "bearer",
  "created_at": 1481811998
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"66ee22745d31af762c1f5df54dab29723a06bb5f55e46900c58fd6a57415964f","client_secret":"928bd8ead2782725a9dbb661253a8bbba7e2dc0062a06b9cf453c4a8801aeb93"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MzRkYjU5NTM3ODFlZGEzMWZiODMyNWViNzZjYTRlMjQ2ZWRjNzhlMTdkZGFj
ZjdmNTlmMTRlZDU1YmZhY2NlMjpkYjU2NWEzODhlYWYzMTAxN2QyNzIwM2Fk
MTNhNzdmM2JkZWIxMTg3Y2UzYjY2MmY3MjRlMzZjZTVjNDg2NzFl

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
  "access_token": "9b25f40c1d6aa8ae96a21ec22672809a583239ac5547c44ec7dabc591f799d8c",
  "token_type": "bearer",
  "created_at": 1481811998
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 34db5953781eda31fb8325eb76ca4e246edc78e17ddacf7f59f14ed55bfacce2:db565a388eaf31017d27203ad13a77f3bdeb1187ce3b662f724e36ce5c48671e
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
{"grant_type":"client_credentials","client_id":"98cb9189717e5ec25cac6a1aeabc9a5c6a1bb821e5d8dd3b904c92199a428d28","client_secret":"c699b7faec744435841d35378c97cd2f3bcc8a4707ac9a0f9f3fe68eafc6bdf8"}
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
  "access_token": "00d14e13e2120906236f2734c7a6e31e9d04088107df86a1cd62e55ce06ea662",
  "token_type": "bearer",
  "created_at": 1481811998
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"98cb9189717e5ec25cac6a1aeabc9a5c6a1bb821e5d8dd3b904c92199a428d28","client_secret":"c699b7faec744435841d35378c97cd2f3bcc8a4707ac9a0f9f3fe68eafc6bdf8"}' -X POST \
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
Authorization: Bearer 291950992ee3daf975be224026a16139f715a192d50ad88db6b26d3d74251edf
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
	-H "Authorization: Bearer 291950992ee3daf975be224026a16139f715a192d50ad88db6b26d3d74251edf"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/45/flashcards
Content-Type: application/json
Authorization: Bearer 9f9719d7fa75596b621863aa0b795549692e35e484ea86318553acc0dc19fb43
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":45,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 57,
    "obfuscated_id": "mCV2FECTNQs",
    "author_id": 246,
    "chapter_id": 45,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:01.487Z",
    "created_at": "2016-12-15T14:27:01.487Z",
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
curl "api.goskive.com/v2/chapters/45/flashcards" -d '{"flashcard":{"chapter_id":45,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f9719d7fa75596b621863aa0b795549692e35e484ea86318553acc0dc19fb43"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/44/flashcards
Content-Type: application/json
Authorization: Bearer a0f03cd09b43ab584315b847cea8f39a1adfd955ff4e50e9a22b2e3461c5cdd6
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 241,
      "chapter_id": 44,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:01.113Z",
      "created_at": "2016-12-15T14:27:01.113Z",
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
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 241,
      "chapter_id": 44,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:01.157Z",
      "created_at": "2016-12-15T14:27:01.157Z",
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
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 241,
      "chapter_id": 44,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:01.200Z",
      "created_at": "2016-12-15T14:27:01.200Z",
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
curl "api.goskive.com/v2/chapters/44/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0f03cd09b43ab584315b847cea8f39a1adfd955ff4e50e9a22b2e3461c5cdd6"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/89/questions
Content-Type: application/json
Authorization: Bearer d4884ceda253f578d91fff17a9fd160b5e666ab9ea5cf99a9bc2ed207662e23f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":89,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 64,
    "obfuscated_id": "H-V851w7HZg",
    "author_id": 421,
    "chapter_id": 89,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:20.674Z",
    "created_at": "2016-12-15T14:27:20.674Z",
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
        "id": 128,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 129,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 130,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 131,
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
curl "api.goskive.com/v2/chapters/89/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":89,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4884ceda253f578d91fff17a9fd160b5e666ab9ea5cf99a9bc2ed207662e23f"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/90/questions
Content-Type: application/json
Authorization: Bearer ebfad546e4f4eaf9ef4a603372518d4226b8f300b7f70eba0722588c4925fcdc
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":90,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 65,
    "obfuscated_id": "Pu1fo5_Q1vk",
    "author_id": 424,
    "chapter_id": 90,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:21.431Z",
    "created_at": "2016-12-15T14:27:21.431Z",
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
        "id": 132,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 133,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/90/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":90,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebfad546e4f4eaf9ef4a603372518d4226b8f300b7f70eba0722588c4925fcdc"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/92/questions
Content-Type: application/json
Authorization: Bearer 77541cddfa91210efc01a5a2ff8a4e0044fd883bb2a3e5a211288fbf512e8b37
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":92,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 67,
    "obfuscated_id": "btMCNJVyvlA",
    "author_id": 430,
    "chapter_id": 92,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:22.558Z",
    "created_at": "2016-12-15T14:27:22.558Z",
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
        "id": 137,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 138,
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
curl "api.goskive.com/v2/chapters/92/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":92,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77541cddfa91210efc01a5a2ff8a4e0044fd883bb2a3e5a211288fbf512e8b37"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/91/questions
Content-Type: application/json
Authorization: Bearer 866d7e9581fdcee92a379ef026e8c3b2f5c05c42374ee7d9bfed8bd19295e582
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":91,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 427,
    "chapter_id": 91,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:22.031Z",
    "created_at": "2016-12-15T14:27:22.031Z",
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
        "id": 134,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 135,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 136,
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
curl "api.goskive.com/v2/chapters/91/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":91,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 866d7e9581fdcee92a379ef026e8c3b2f5c05c42374ee7d9bfed8bd19295e582"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/93/questions
Content-Type: application/json
Authorization: Bearer 48a0486340bc2833a4d1afe510cfccd3e1d44d816094b7897fb5c5d83286cbbe
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 433,
      "chapter_id": 93,
      "position": 55,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:23.228Z",
      "created_at": "2016-12-15T14:27:23.132Z",
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
          "id": 139,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 140,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 434,
      "chapter_id": 93,
      "position": 56,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:23.399Z",
      "created_at": "2016-12-15T14:27:23.302Z",
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
          "id": 141,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 142,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 435,
      "chapter_id": 93,
      "position": 57,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T14:27:23.570Z",
      "created_at": "2016-12-15T14:27:23.471Z",
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
          "id": 143,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 144,
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
curl "api.goskive.com/v2/chapters/93/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48a0486340bc2833a4d1afe510cfccd3e1d44d816094b7897fb5c5d83286cbbe"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/131
Content-Type: application/json
Authorization: Bearer cc9238af1703923430f61d1fee246f7a3e5bb1dd5b7fc6d1e47fc2118becaf54
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
curl "api.goskive.com/v2/chapters/131" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc9238af1703923430f61d1fee246f7a3e5bb1dd5b7fc6d1e47fc2118becaf54"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/134
Content-Type: application/json
Authorization: Bearer bf0d868c2f83741071d015209eb640c7cd84e3b461f40a7429398253475b5706
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
curl "api.goskive.com/v2/chapters/134" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf0d868c2f83741071d015209eb640c7cd84e3b461f40a7429398253475b5706"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/126
Content-Type: application/json
Authorization: Bearer 3d0ea8b677cedc9d402d22893632f7e31df44d197fe5b4784355cde6e1a45bdf
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
curl "api.goskive.com/v2/chapters/126" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d0ea8b677cedc9d402d22893632f7e31df44d197fe5b4784355cde6e1a45bdf"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/133
Content-Type: application/json
Authorization: Bearer e49dd33951f810b04ad876263f03e5d2d00d3e975d5deba4454a09ac43c673fb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/133" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e49dd33951f810b04ad876263f03e5d2d00d3e975d5deba4454a09ac43c673fb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/130
Content-Type: application/json
Authorization: Bearer 688ca0b9d636a738bcfaa8b8d94b4edff4d4a5441ecc645df9758220427ca544
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
    "id": 130,
    "updated_at": "2016-12-15T14:27:35.416Z",
    "course_id": 189,
    "author_id": 558,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T14:27:34.846Z",
    "questions_updated_at": "2016-12-15T14:27:34.846Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 562,
        "chapter_id": 130,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:27:35.395Z",
        "created_at": "2016-12-15T14:27:35.395Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 560,
        "chapter_id": 130,
        "position": 68,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:27:35.280Z",
        "created_at": "2016-12-15T14:27:35.180Z",
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
            "id": 165,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 166,
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
curl "api.goskive.com/v2/chapters/130" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 688ca0b9d636a738bcfaa8b8d94b4edff4d4a5441ecc645df9758220427ca544"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/128
Content-Type: application/json
Authorization: Bearer 22ca2aeaf923155f77707333ca5a2aabbe4ed5ceffcdb903a9f1070a7a4021c6
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
    "id": 128,
    "updated_at": "2016-12-15T14:27:34.126Z",
    "course_id": 187,
    "author_id": 549,
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
curl "api.goskive.com/v2/chapters/128" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22ca2aeaf923155f77707333ca5a2aabbe4ed5ceffcdb903a9f1070a7a4021c6"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/4/replies
Content-Type: application/json
Authorization: Bearer f3e6d272e11d792dd9e22ee1bfe0b9506f49a8104c39e503332d1031d8558196
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
    "author_id": 407,
    "reply_to_id": 4,
    "created_at": "2016-12-15T14:27:19.116Z",
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
	-H "Authorization: Bearer f3e6d272e11d792dd9e22ee1bfe0b9506f49a8104c39e503332d1031d8558196"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 8e8aa3f9f57216afbf6f509bf9c578c6a3f7e7aae63d659ffa35421ae3da4971
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
	-H "Authorization: Bearer 8e8aa3f9f57216afbf6f509bf9c578c6a3f7e7aae63d659ffa35421ae3da4971"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/21
Content-Type: application/json
Authorization: Bearer 77ad2c14d0c886207bc4b5b13b6bca089848072d61d9c3dd79ff761dcb97ecba
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
curl "api.goskive.com/v2/comments/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77ad2c14d0c886207bc4b5b13b6bca089848072d61d9c3dd79ff761dcb97ecba"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/58/republish
Content-Type: application/json
Authorization: Bearer 76caa74c42d741d9d47449de970d3ceddbe7fbd16fb60feb64c702638dcd662a
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
curl "api.goskive.com/v2/comments/58/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76caa74c42d741d9d47449de970d3ceddbe7fbd16fb60feb64c702638dcd662a"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer eee54466976b0e2d22f088cc029982c458c4c144560cb8cd72bef8b145c9aaf6
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
	-H "Authorization: Bearer eee54466976b0e2d22f088cc029982c458c4c144560cb8cd72bef8b145c9aaf6"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 281c6d6f05fe89150fb032177ca586bb9204bc183f9c6f27475ed8dbad348b47
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
	-H "Authorization: Bearer 281c6d6f05fe89150fb032177ca586bb9204bc183f9c6f27475ed8dbad348b47"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/7
Content-Type: application/json
Authorization: Bearer 7273479626e292cc127f502ae83c0dc9a49b46bd78e6b47faa276c277ddc4a91
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
    "id": 7,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T14:26:44.257Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7273479626e292cc127f502ae83c0dc9a49b46bd78e6b47faa276c277ddc4a91"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 2bf23d7f9ab13fd1df0e7d0acfdf53bc5f254bb2e982985ea00d9b242577452b
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
      "id": 4,
      "name": "Fake Company Name 4",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T14:26:44.088Z"
    },
    {
      "id": 5,
      "name": "Fake Company Name 5",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T14:26:44.092Z"
    },
    {
      "id": 6,
      "name": "Fake Company Name 6",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T14:26:44.097Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bf23d7f9ab13fd1df0e7d0acfdf53bc5f254bb2e982985ea00d9b242577452b"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/31/company_profiles
Content-Type: application/json
Authorization: Bearer 48e46b62d7a6f946d4e1b4f0450496c37dc073719975c7b030f831a9370a8dd3
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
	-H "Authorization: Bearer 48e46b62d7a6f946d4e1b4f0450496c37dc073719975c7b030f831a9370a8dd3"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer 81f2187b3224c4805e13fcacc9df4e02b1d09a79c030d63cc1e4ca2445a75acb
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
	-H "Authorization: Bearer 81f2187b3224c4805e13fcacc9df4e02b1d09a79c030d63cc1e4ca2445a75acb"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 8d857d41af3d03549ee6a1272566c4555190d0d602e705727aac5299e0c0fdc9
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
	-H "Authorization: Bearer 8d857d41af3d03549ee6a1272566c4555190d0d602e705727aac5299e0c0fdc9"
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
Authorization: Bearer 8da255175a5980b0cf2a3453b95bb3d811773aab8de0be1a1ee81133ead89d0f
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
	-H "Authorization: Bearer 8da255175a5980b0cf2a3453b95bb3d811773aab8de0be1a1ee81133ead89d0f"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 40ea5d8aed78646e89ee020398b9a7ed1d27bb355c07e3cdfdad83085bb493f0
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
    "id": 102,
    "updated_at": "2016-12-15T14:27:29.441Z",
    "course_id": 171,
    "author_id": 488,
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
	-H "Authorization: Bearer 40ea5d8aed78646e89ee020398b9a7ed1d27bb355c07e3cdfdad83085bb493f0"
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
      "id": 105,
      "updated_at": "2016-12-15T14:27:30.039Z",
      "course_id": 174,
      "author_id": 494,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 90",
      "position": 1
    },
    {
      "id": 106,
      "updated_at": "2016-12-15T14:27:30.067Z",
      "course_id": 174,
      "author_id": 495,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 91",
      "position": 2
    },
    {
      "id": 107,
      "updated_at": "2016-12-15T14:27:30.306Z",
      "course_id": 174,
      "author_id": 496,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T14:27:29.878Z",
      "questions_updated_at": "2016-12-15T14:27:29.878Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 92",
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
Authorization: Bearer ea7e0c598296a57f532456fd85dc3a0d5cd2d42f9f7b7f6891bae849351e4cb7
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
      "id": 117,
      "updated_at": "2016-12-15T14:27:31.786Z",
      "course_id": 180,
      "author_id": 519,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 102",
      "position": 1
    },
    {
      "id": 118,
      "updated_at": "2016-12-15T14:27:31.815Z",
      "course_id": 180,
      "author_id": 520,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 103",
      "position": 2
    },
    {
      "id": 119,
      "updated_at": "2016-12-15T14:27:32.063Z",
      "course_id": 180,
      "author_id": 521,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T14:27:31.657Z",
      "questions_updated_at": "2016-12-15T14:27:31.657Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 104",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea7e0c598296a57f532456fd85dc3a0d5cd2d42f9f7b7f6891bae849351e4cb7"
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
      "id": 108,
      "updated_at": "2016-12-15T14:27:30.624Z",
      "course_id": 176,
      "author_id": 501,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 93",
      "position": 1
    },
    {
      "id": 109,
      "updated_at": "2016-12-15T14:27:30.653Z",
      "course_id": 176,
      "author_id": 502,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 94",
      "position": 2
    },
    {
      "id": 110,
      "updated_at": "2016-12-15T14:27:30.680Z",
      "course_id": 176,
      "author_id": 503,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 95",
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
Authorization: Bearer 82d9867971b290d5d800e941fcd34b3f3a3ac8f7d9287fae067f6dee86f77f1b
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
      "id": 120,
      "updated_at": "2016-12-15T14:27:32.297Z",
      "course_id": 181,
      "author_id": 526,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 105",
      "position": 1
    },
    {
      "id": 121,
      "updated_at": "2016-12-15T14:27:32.326Z",
      "course_id": 181,
      "author_id": 527,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 106",
      "position": 2
    },
    {
      "id": 122,
      "updated_at": "2016-12-15T14:27:32.355Z",
      "course_id": 181,
      "author_id": 528,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 107",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82d9867971b290d5d800e941fcd34b3f3a3ac8f7d9287fae067f6dee86f77f1b"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 6eb174efeb2fa638579af5ae328f5b1779a220056945a162ced135e0b3af3b5a
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
    "course_id": 39,
    "user_id": 137,
    "updated_at": "2016-12-15T14:26:47.564Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6eb174efeb2fa638579af5ae328f5b1779a220056945a162ced135e0b3af3b5a"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 369ea0365a36868602df1a2c0f484974da1cb7d4b6e5e023c22f3da3f4dbf6f2
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
      "course_id": 42,
      "user_id": 143,
      "updated_at": "2016-12-15T14:26:48.083Z"
    },
    {
      "id": 4,
      "course_id": 42,
      "user_id": 144,
      "updated_at": "2016-12-15T14:26:48.099Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 369ea0365a36868602df1a2c0f484974da1cb7d4b6e5e023c22f3da3f4dbf6f2"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/11/files
Content-Type: application/json
Authorization: Bearer 0aa44acea332b00656d84fbdf286beaf231d38a0498ad3e70bfb3a312c5055ea
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
      "id": 5,
      "uploader": {
        "id": 23,
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
        "created_at": "2016-12-15T14:26:38.153Z",
        "updated_at": "2016-12-15T14:26:38.153Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T14:26:38.170Z",
      "updated_at": "2016-12-15T14:26:38.170Z",
      "course_id": 11,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 24,
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
        "created_at": "2016-12-15T14:26:38.183Z",
        "updated_at": "2016-12-15T14:26:38.183Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T14:26:38.195Z",
      "updated_at": "2016-12-15T14:26:38.195Z",
      "course_id": 11,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 7,
      "uploader": {
        "id": 25,
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
        "created_at": "2016-12-15T14:26:38.208Z",
        "updated_at": "2016-12-15T14:26:38.208Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T14:26:38.220Z",
      "updated_at": "2016-12-15T14:26:38.220Z",
      "course_id": 11,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/11/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aa44acea332b00656d84fbdf286beaf231d38a0498ad3e70bfb3a312c5055ea"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/8/files
Content-Type: application/json
Authorization: Bearer cdfbf6fcaa9a32714500268d77f42a34a708f7f71c32636fa36531fa4854322b
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
    "id": 4,
    "uploader": {
      "id": 17,
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
      "created_at": "2016-12-15T14:26:37.423Z",
      "updated_at": "2016-12-15T14:26:37.423Z"
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
    "created_at": "2016-12-15T14:26:37.473Z",
    "updated_at": "2016-12-15T14:26:37.473Z",
    "course_id": 8,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/8/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdfbf6fcaa9a32714500268d77f42a34a708f7f71c32636fa36531fa4854322b"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/9/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer a22a02867ad53089ce6446717c1103310d10ca3b65bc72221e31c860537c98a0
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
    "key": "cache/d8c7eb537d22720687266f37206bc8be.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNToyNjozN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Q4YzdlYjUzN2QyMjcyMDY4NzI2NmYzNzIwNmJjOGJlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDE0MjYzN1oifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T142637Z",
    "x-amz-signature": "c0abe57e9aed7af5032d52919801d79f5ff2e4c04325d1a960fa06c64cd62432"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/9/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a22a02867ad53089ce6446717c1103310d10ca3b65bc72221e31c860537c98a0"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer aa03f2d896d4dbc1957d6cb1ca88e03ae72ef1e633ff539113f94548316fd3bc
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
	-H "Authorization: Bearer aa03f2d896d4dbc1957d6cb1ca88e03ae72ef1e633ff539113f94548316fd3bc"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9c8a5b5faca05162919cdee90038863b6a46e12e3a42cdb41a80c735d0ca5a4d
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
	-H "Authorization: Bearer 9c8a5b5faca05162919cdee90038863b6a46e12e3a42cdb41a80c735d0ca5a4d"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6dc65043e357ea4018826e4cf07fa9dcbd11306963050fc15889ab43ab0bbf10
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
	-H "Authorization: Bearer 6dc65043e357ea4018826e4cf07fa9dcbd11306963050fc15889ab43ab0bbf10"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fd8c00e34261855d2e4d64db362b274b3bbdb1cd327514186a68f8f420aa71b7
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
	-H "Authorization: Bearer fd8c00e34261855d2e4d64db362b274b3bbdb1cd327514186a68f8f420aa71b7"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 39f335487ff5f26f61e18e3efdb0b687c50531fa7a2e1437ec3f214c629a4d37
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
	-H "Authorization: Bearer 39f335487ff5f26f61e18e3efdb0b687c50531fa7a2e1437ec3f214c629a4d37"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 10a05610c9ef319ef492a4a2013340de6fb0302b569b5aef6f670a5bdef0628b
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
    "creator_id": 188,
    "id": 58,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 59,
    "additional_university_ids": [

    ],
    "discipline_id": 66,
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
    "chapters_updated_at": "2016-12-15T14:26:53.870Z",
    "updated_at": "2016-12-15T14:26:55.206Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 189,
        "chapter_id": 36,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:54.968Z",
        "created_at": "2016-12-15T14:26:54.968Z",
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
        "author_id": 189,
        "chapter_id": 37,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:55.051Z",
        "created_at": "2016-12-15T14:26:55.051Z",
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
        "author_id": 189,
        "chapter_id": 36,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:55.014Z",
        "created_at": "2016-12-15T14:26:55.014Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 189,
        "chapter_id": 37,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:55.096Z",
        "created_at": "2016-12-15T14:26:55.096Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 189,
        "chapter_id": 36,
        "position": 18,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:54.119Z",
        "created_at": "2016-12-15T14:26:54.024Z",
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
            "id": 35,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 36,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 189,
        "chapter_id": 36,
        "position": 19,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:54.267Z",
        "created_at": "2016-12-15T14:26:54.185Z",
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
            "id": 37,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 38,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 189,
        "chapter_id": 37,
        "position": 20,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:54.441Z",
        "created_at": "2016-12-15T14:26:54.349Z",
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
            "id": 39,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 40,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 189,
        "chapter_id": 37,
        "position": 21,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:54.587Z",
        "created_at": "2016-12-15T14:26:54.504Z",
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
    "chapters": [
      {
        "id": 36,
        "updated_at": "2016-12-15T14:26:55.151Z",
        "course_id": 58,
        "author_id": 188,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T14:26:53.870Z",
        "questions_updated_at": "2016-12-15T14:26:53.870Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 36",
        "position": 1
      },
      {
        "id": 37,
        "updated_at": "2016-12-15T14:26:55.195Z",
        "course_id": 58,
        "author_id": 188,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T14:26:53.870Z",
        "questions_updated_at": "2016-12-15T14:26:53.870Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 37",
        "position": 2
      }
    ],
    "topic_id": 65,
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
	-H "Authorization: Bearer 10a05610c9ef319ef492a4a2013340de6fb0302b569b5aef6f670a5bdef0628b"
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
    "creator_id": 194,
    "id": 59,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 60,
    "additional_university_ids": [

    ],
    "discipline_id": 67,
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
    "chapters_updated_at": "2016-12-15T14:26:55.372Z",
    "updated_at": "2016-12-15T14:26:56.727Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 194,
        "chapter_id": 38,
        "position": 24,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:55.638Z",
        "created_at": "2016-12-15T14:26:55.549Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 194,
        "chapter_id": 39,
        "position": 26,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T14:26:55.959Z",
        "created_at": "2016-12-15T14:26:55.865Z",
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
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
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
        "id": 38,
        "updated_at": "2016-12-15T14:26:56.672Z",
        "course_id": 59,
        "author_id": 194,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T14:26:55.372Z",
        "questions_updated_at": "2016-12-15T14:26:55.372Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 38",
        "position": 1
      },
      {
        "id": 39,
        "updated_at": "2016-12-15T14:26:56.715Z",
        "course_id": 59,
        "author_id": 194,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T14:26:55.372Z",
        "questions_updated_at": "2016-12-15T14:26:55.372Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 39",
        "position": 2
      }
    ],
    "topic_id": 66,
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
PUT /v2/courses/45/pin
Content-Type: application/json
Authorization: Bearer d316e2348a0c22b0a2cfecf32b9c871394c81301fb7ce321cc49ca4daa6a7134
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/45/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d316e2348a0c22b0a2cfecf32b9c871394c81301fb7ce321cc49ca4daa6a7134"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/46/pin
Content-Type: application/json
Authorization: Bearer ba3a70b039aacc5333ad022abb07c08c906855e6f4ef930e58d6c732f191591e
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/46/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba3a70b039aacc5333ad022abb07c08c906855e6f4ef930e58d6c732f191591e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4a96ee618d09246c08e6b1135d869a768881b9a7dcac5a2ad091d8cbad11ad91
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
    "creator_id": 201,
    "id": 61,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 62,
    "additional_university_ids": [

    ],
    "discipline_id": 69,
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
    "updated_at": "2016-12-15T14:26:57.164Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 68,
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
	-H "Authorization: Bearer 4a96ee618d09246c08e6b1135d869a768881b9a7dcac5a2ad091d8cbad11ad91"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 81649075ad5e68e9d5462a4c4528dee5ba7a020a0e8fcfcd1dd176b1f521fe0e
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
    "id": 118,
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
    "created_at": "2016-12-15T14:26:44.979Z",
    "updated_at": "2016-12-15T14:26:44.979Z",
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
	-H "Authorization: Bearer 81649075ad5e68e9d5462a4c4528dee5ba7a020a0e8fcfcd1dd176b1f521fe0e"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer fa5e1e5009693292198c9f72a792fd3eabad15e0c91b3bd7937eaf81e4c9eaf4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[37]}
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
    "id": 114,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      37
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T14:26:44.670Z",
    "updated_at": "2016-12-15T14:26:44.713Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[37]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa5e1e5009693292198c9f72a792fd3eabad15e0c91b3bd7937eaf81e4c9eaf4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ee4f5b8b3511890ba2f2e22c22301f76773e0e0c7612dd0d47ca7dcd710399ce
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
    "id": 115,
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
    "created_at": "2016-12-15T14:26:44.739Z",
    "updated_at": "2016-12-15T14:26:44.739Z",
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
	-H "Authorization: Bearer ee4f5b8b3511890ba2f2e22c22301f76773e0e0c7612dd0d47ca7dcd710399ce"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 890fdad409bd410a776310218ab8dec9efd678aeea84c8d062e7d1cfaf18e789
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[40]}
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
    "id": 117,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      40
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T14:26:44.914Z",
    "updated_at": "2016-12-15T14:26:44.914Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[40]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 890fdad409bd410a776310218ab8dec9efd678aeea84c8d062e7d1cfaf18e789"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 7ab66f325bb6882a567879af1c0b3de13dae339407bb84217e31a7fbc9e9d1bb
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

36
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
    "id": 113,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/4a2c08815e6253903bf71198accae686ef1a0ec8.jpg",
    "university_id": null,
    "fields_of_study": [
      36
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T14:26:44.336Z",
    "updated_at": "2016-12-15T14:26:44.606Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/0174fbd18884f064ee792a4ca23fbd19402b3f0e.jpg",
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

36
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 7ab66f325bb6882a567879af1c0b3de13dae339407bb84217e31a7fbc9e9d1bb"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 7b3f12feaf7da9693bff528ae2cd982dd8ff76297cc27873a4a48b12f5f55c79
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
      "bookmarkable_id": 61,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b3f12feaf7da9693bff528ae2cd982dd8ff76297cc27873a4a48b12f5f55c79"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1139edbb017002e572ab444cdec254f7e251d0a464daabeea75422017c94d734
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
	-H "Authorization: Bearer 1139edbb017002e572ab444cdec254f7e251d0a464daabeea75422017c94d734"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 630bb7695a1a3e2f2ea7f5de1b9386005dd126ea1691152200f26a4273f3b6c0
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
      "creator_id": 813,
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-185",
      "html_url": "https://goskive.com/course/mit-course-185",
      "slug": "mit-course-185",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "discipline_id": 262,
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
      "updated_at": "2016-12-15T14:27:56.636Z",
      "shortname": "mit-course-185",
      "topic_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 814,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-186",
      "html_url": "https://goskive.com/course/mit-course-186",
      "slug": "mit-course-186",
      "university_id": 236,
      "additional_university_ids": [

      ],
      "discipline_id": 263,
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
      "updated_at": "2016-12-15T14:27:56.768Z",
      "shortname": "mit-course-186",
      "topic_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 186",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 630bb7695a1a3e2f2ea7f5de1b9386005dd126ea1691152200f26a4273f3b6c0"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer fae7584c08e107ab93eef0fec39bbef83339739e0e1c1b6383a4427333e37b64
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
        "created_at": "2016-12-15T14:26:36.915Z",
        "updated_at": "2016-12-15T14:26:36.915Z",
        "file_url": "memory://63616ae55277bb64058557c8ba6e54f7.pdf",
        "course_id": 5,
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
        "created_at": "2016-12-15T14:26:37.058Z",
        "updated_at": "2016-12-15T14:26:37.058Z",
        "file_url": "memory://c2fea29564d933a00e2108a8eaea138d.pdf",
        "course_id": 6,
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
        "created_at": "2016-12-15T14:26:37.200Z",
        "updated_at": "2016-12-15T14:26:37.200Z",
        "file_url": "memory://f6026e7baa1222e2ab5290ee2d9aea77.pdf",
        "course_id": 7,
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
	-H "Authorization: Bearer fae7584c08e107ab93eef0fec39bbef83339739e0e1c1b6383a4427333e37b64"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 03662416514d9a65150afb1b43ff1be63ea151cd479ff56fb572be6ec7f1fcd6
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
      "created_at": "2016-12-15T14:27:42.412Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 13,
      "updated_at": "2016-12-15T14:27:42.576Z",
      "author_id": "640",
      "thread_subject_id": "209",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 18,
      "created_at": "2016-12-15T14:27:42.565Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 14,
      "updated_at": "2016-12-15T14:27:42.580Z",
      "author_id": "643",
      "thread_subject_id": "210",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-12-15T14:27:42.992Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-12-15T14:27:42.992Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-12-15T14:27:43.430Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-12-15T14:27:43.430Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 21,
      "created_at": "2016-12-15T14:27:43.871Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-12-15T14:27:43.871Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 22,
      "created_at": "2016-12-15T14:27:44.199Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 96,
      "updated_at": "2016-12-15T14:27:44.199Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-12-15T14:27:44.543Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 97,
      "updated_at": "2016-12-15T14:27:44.543Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-12-15T14:27:44.874Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 98,
      "updated_at": "2016-12-15T14:27:44.874Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03662416514d9a65150afb1b43ff1be63ea151cd479ff56fb572be6ec7f1fcd6"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/16
Content-Type: application/json
Authorization: Bearer b98f998dfa043de4a2203045f44121bf6cbd364ae42292af6b002fcf3b05aea0
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T14:17:42.000Z"}}
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
    "id": 16,
    "created_at": "2016-12-15T14:27:42.157Z",
    "read_at": "2016-12-15T14:17:42.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 12,
    "updated_at": "2016-12-15T14:27:42.210Z",
    "author_id": "635",
    "thread_subject_id": "208",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/16" -d '{"notification":{"read_at":"2016-12-15T14:17:42.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b98f998dfa043de4a2203045f44121bf6cbd364ae42292af6b002fcf3b05aea0"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer eb30c95ba7f2432f25e2aebe3a0df0907245ab2fc1c37fcfa8b4b48a11ebc89f
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
      "course_id": 71,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T14:26:59.810Z",
      "course_published": true,
      "updated_at": "2016-12-15T14:26:59.805Z"
    },
    {
      "id": 3,
      "course_id": 72,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T14:26:59.940Z",
      "course_published": true,
      "updated_at": "2016-12-15T14:26:59.935Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb30c95ba7f2432f25e2aebe3a0df0907245ab2fc1c37fcfa8b4b48a11ebc89f"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer a21a6891f3e1837fe8dbf5d01583f86c25e4b217c9b37ce749eb084f1d85b1c2
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
    "id": 5,
    "course_id": 75,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T14:27:00.503Z",
    "course_published": true,
    "updated_at": "2016-12-15T14:27:00.498Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a21a6891f3e1837fe8dbf5d01583f86c25e4b217c9b37ce749eb084f1d85b1c2"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 561efc074ea797ac5be2ce91982dab0e2272c2028a1935f19cef529d2e6c652a
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
    "id": 6,
    "course_id": 76,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T14:27:00.731Z",
    "course_published": true,
    "updated_at": "2016-12-15T14:27:00.722Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 561efc074ea797ac5be2ce91982dab0e2272c2028a1935f19cef529d2e6c652a"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer e94a93c1f48905b32ff606735ff922d6313f81ec1443238740dfbd9776b175c0
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
      "user_id": 878
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 878
    },
    {
      "id": 22,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 129,
      "user_id": 878
    },
    {
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 878
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e94a93c1f48905b32ff606735ff922d6313f81ec1443238740dfbd9776b175c0"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/41
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
    "id": 41,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 41,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 41
      },
      {
        "id": 42,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 41
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/41" -X GET \
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
      "id": 42,
      "name": "Public-key multimedia moderator",
      "name_translations": {
        "en": "Public-key multimedia moderator"
      }
    },
    {
      "id": 43,
      "name": "Optimized leading edge product",
      "name_translations": {
        "en": "Optimized leading edge product"
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
Authorization: Bearer 8df7348801987e128421021c6f2411b7de57fd636092c2d78d808403da8b2f30
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
    "user_id": 679,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T14:27:45.853Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8df7348801987e128421021c6f2411b7de57fd636092c2d78d808403da8b2f30"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/45/fix
Content-Type: application/json
Authorization: Bearer dff0e44ad3fd75224e2a44ccc747093a150a57f5ce012371b9a6a18e9e7253f1
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
    "user_id": 792,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T14:27:54.099Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/45/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dff0e44ad3fd75224e2a44ccc747093a150a57f5ce012371b9a6a18e9e7253f1"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/40
Content-Type: application/json
Authorization: Bearer 9d8ba538c4f1148f48d3729227b15713945e1077214c534153432a481f660ef9
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
    "id": 40,
    "user_id": 765,
    "feedbackable_id": 86,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T14:27:52.510Z",
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
curl "api.goskive.com/v2/feedbacks/40" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d8ba538c4f1148f48d3729227b15713945e1077214c534153432a481f660ef9"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/18/close
Content-Type: application/json
Authorization: Bearer 018594801d211f0ec2e1f314851fe905d161e8a9c87daeb171437f935ab045e1
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
curl "api.goskive.com/v2/feedbacks/18/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 018594801d211f0ec2e1f314851fe905d161e8a9c87daeb171437f935ab045e1"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/fix
Content-Type: application/json
Authorization: Bearer 4945c3ae26c68bee53e7dd4f1b9867609d4dcbc756eda7a164d1612b281191d4
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
curl "api.goskive.com/v2/feedbacks/42/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4945c3ae26c68bee53e7dd4f1b9867609d4dcbc756eda7a164d1612b281191d4"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer ce44074fe23a5fda6ff0a54844306ab9da6a573d46d39a293b51aa8562169155
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
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce44074fe23a5fda6ff0a54844306ab9da6a573d46d39a293b51aa8562169155"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/41
Content-Type: application/json
Authorization: Bearer fcaa39fc3558a63f0d2aab1433786069a81fd13dc9ae265c9580b6b6a237fc90
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
    "user_id": 770,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T14:27:52.888Z",
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
curl "api.goskive.com/v2/feedbacks/41" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcaa39fc3558a63f0d2aab1433786069a81fd13dc9ae265c9580b6b6a237fc90"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer 0aeb1fc63f24ab0bf758a3b5f5f48e654e86126ce8796db2813cf4c52c859a96
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
	-H "Authorization: Bearer 0aeb1fc63f24ab0bf758a3b5f5f48e654e86126ce8796db2813cf4c52c859a96"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/17/bookmark
Content-Type: application/json
Authorization: Bearer 3d4f98d2827c4c8878afab0a89bb2e0adcd0cea891b85422ce65ba0424ebe068
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d4f98d2827c4c8878afab0a89bb2e0adcd0cea891b85422ce65ba0424ebe068"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer cf98624febe0a5a10fa86bcb13eef9b7d4aee7d18e22fb332e38f8cff9b30ee1
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf98624febe0a5a10fa86bcb13eef9b7d4aee7d18e22fb332e38f8cff9b30ee1"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/9
Content-Type: application/json
Authorization: Bearer 7e2a3b379d17c03bad40ffe0bcaf1eb03744432c8f468b9496f3b342140a2aa0
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/f92b3a5e8b58c2a6674c134428063b0f.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T142757Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=85b8873c66ba79aa417c99fa5ba2ea4caeb45aac5d4d86740f40554558024d06",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e2a3b379d17c03bad40ffe0bcaf1eb03744432c8f468b9496f3b342140a2aa0"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/8/preview
Content-Type: application/json
Authorization: Bearer 45c40efe075a1688bb81f39be28c4fb8bc9f1281abb99625191a327b52bc71f2
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/7735ea7a1abe5bee37e946e5627a6e28.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T142757Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=c8645049b6fc0eb4a4d6073d16e439d9416fab951214a4ac2cf1b6a6ea42adc2",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45c40efe075a1688bb81f39be28c4fb8bc9f1281abb99625191a327b52bc71f2"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 9ea11e479d86debaf00c3ed06fa43afe9460e86f49880b4ea5240c16a4346ee2
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
    "id": 11,
    "uploader": {
      "id": 823,
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
      "created_at": "2016-12-15T14:27:57.376Z",
      "updated_at": "2016-12-15T14:27:57.376Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T14:27:57.501Z",
    "updated_at": "2016-12-15T14:27:57.501Z",
    "course_id": 256,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ea11e479d86debaf00c3ed06fa43afe9460e86f49880b4ea5240c16a4346ee2"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/22/matched_courses?required_cu_count=2
Authorization: Bearer 63ddae3cd0b15d4cad1b43be84c0d129faa458f95f6e93ce8be632db00d04c94
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
      "creator_id": 865,
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 280,
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
      "chapters_updated_at": "2016-12-15T14:27:59.818Z",
      "updated_at": "2016-12-15T14:28:01.071Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 279,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 870,
      "id": 270,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-b2da8c4f-be4e-488a-a9e3-073e9a15cf17",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-b2da8c4f-be4e-488a-a9e3-073e9a15cf17",
      "slug": "mit-the-great-british-bake-off-b2da8c4f-be4e-488a-a9e3-073e9a15cf17",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "discipline_id": 281,
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
      "chapters_updated_at": "2016-12-15T14:27:59.818Z",
      "updated_at": "2016-12-15T14:28:01.481Z",
      "shortname": "mit-the-great-british-bake-off-b2da8c4f-be4e-488a-a9e3-073e9a15cf17",
      "topic_id": 280,
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
curl "api.goskive.com/v2/files/22/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 63ddae3cd0b15d4cad1b43be84c0d129faa458f95f6e93ce8be632db00d04c94"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/18/download
Content-Type: application/json
Authorization: Bearer 4dea9652554186451e675e372b054bc246ada293c1c24d17736387157f3ea217
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4dea9652554186451e675e372b054bc246ada293c1c24d17736387157f3ea217"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/19/report
Content-Type: application/json
Authorization: Bearer 1ca432253718e006c41bcce2518f6aab74d098e0683888538330d66b2ab92ae7
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ca432253718e006c41bcce2518f6aab74d098e0683888538330d66b2ab92ae7"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/13/bookmark
Content-Type: application/json
Authorization: Bearer 1694bcfc93acb543df6ea39fce6c4a95094fb16ff9dc18c6d4d492b6be1550f0
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1694bcfc93acb543df6ea39fce6c4a95094fb16ff9dc18c6d4d492b6be1550f0"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/20/upvote
Content-Type: application/json
Authorization: Bearer d5d31541ae3e72993011365454055afd43ce3dac5b8adaa39ad851fb3e9c5703
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5d31541ae3e72993011365454055afd43ce3dac5b8adaa39ad851fb3e9c5703"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/78/comments
Content-Type: application/json
Authorization: Bearer 297effbb5b08415ce797dc30ab0a5ac342e9bea72f1b3054b98689ffd387e1ef
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
    "id": 6,
    "author_id": 576,
    "reply_to_id": null,
    "created_at": "2016-12-15T14:27:36.911Z",
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
curl "api.goskive.com/v2/flashcards/78/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 297effbb5b08415ce797dc30ab0a5ac342e9bea72f1b3054b98689ffd387e1ef"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/80/comments
Content-Type: application/json
Authorization: Bearer 23e3f2655e3f9f49fd368102295d2ef2895c1c5ae9ca13e8913baa283e5b4ba1
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
    "author_id": 582,
    "reply_to_id": null,
    "created_at": "2016-12-15T14:27:37.554Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 582,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:37.551Z",
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
curl "api.goskive.com/v2/flashcards/80/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23e3f2655e3f9f49fd368102295d2ef2895c1c5ae9ca13e8913baa283e5b4ba1"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/81/comments
Content-Type: application/json
Authorization: Bearer 56b399d1b236f27760710cc875dc29b0ce74d3f4e34a412558c734de4790366b
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
      "id": 8,
      "author_id": 588,
      "reply_to_id": null,
      "created_at": "2016-12-15T14:27:37.947Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 589,
      "reply_to_id": null,
      "created_at": "2016-12-15T14:27:37.964Z",
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
curl "api.goskive.com/v2/flashcards/81/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56b399d1b236f27760710cc875dc29b0ce74d3f4e34a412558c734de4790366b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/79/comments
Content-Type: application/json
Authorization: Bearer 282467c0fcf106cdf3c6f1078c681bc9a46dc454e0928ab1e9a9b35d7fd829de
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
curl "api.goskive.com/v2/flashcards/79/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 282467c0fcf106cdf3c6f1078c681bc9a46dc454e0928ab1e9a9b35d7fd829de"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer e0754cb2197fc9b5b1fc1d264b44f5a7ee8246a36f81902943d0dc7d15b2c4ef
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
    "id": 8,
    "user_id": 395,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T14:27:18.178Z",
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
	-H "Authorization: Bearer e0754cb2197fc9b5b1fc1d264b44f5a7ee8246a36f81902943d0dc7d15b2c4ef"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/64/feedbacks
Content-Type: application/json
Authorization: Bearer c0c81e36e0ec25fa70b7bb42cf49c6b9e94473947ff44ad0721d2172fa537ff6
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
      "user_id": 391,
      "feedbackable_id": 64,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:17.390Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 390,
      "feedbackable_id": 64,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:17.378Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/64/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0c81e36e0ec25fa70b7bb42cf49c6b9e94473947ff44ad0721d2172fa537ff6"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/52/votes
Content-Type: application/json
Authorization: Bearer 1d37406d4397f7a7ab189b030d3be8c38108276d95a520b2e68fbdd60eae7db2
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
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 52,
      "user_id": 214
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 52,
      "user_id": 213
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 52,
      "user_id": 212
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/52/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d37406d4397f7a7ab189b030d3be8c38108276d95a520b2e68fbdd60eae7db2"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/1/republish
Content-Type: application/json
Authorization: Bearer a7ba9db157c86196b0c0f8aa22994496b04167998d341574fd3ee73eee7b067d
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
curl "api.goskive.com/v2/flashcards/1/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7ba9db157c86196b0c0f8aa22994496b04167998d341574fd3ee73eee7b067d"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/4/bookmark
Content-Type: application/json
Authorization: Bearer a32a0c9e0b48154698f0f8a78681dbc97a875f461c7ef4381c55a96b2db5b579
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/4/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a32a0c9e0b48154698f0f8a78681dbc97a875f461c7ef4381c55a96b2db5b579"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/5
Content-Type: application/json
Authorization: Bearer a33565b0d78e54f3017b91b8829044d3b5abd0e9a66ddef47105fe2140e0dfb2
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
	-H "Authorization: Bearer a33565b0d78e54f3017b91b8829044d3b5abd0e9a66ddef47105fe2140e0dfb2"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/7/downvote
Content-Type: application/json
Authorization: Bearer 7bc5096b7610c54bef73dafb528933bfcd632691c412288a9a33148974a19334
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/7/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7bc5096b7610c54bef73dafb528933bfcd632691c412288a9a33148974a19334"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/8
Content-Type: application/json
Authorization: Bearer 88b483afe54740c49093829baf07df8f56499a9eb0f673b5059a2f6642ec9f1d
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 54,
    "chapter_id": 8,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:26:40.527Z",
    "created_at": "2016-12-15T14:26:40.527Z",
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
curl "api.goskive.com/v2/flashcards/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88b483afe54740c49093829baf07df8f56499a9eb0f673b5059a2f6642ec9f1d"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/9/report
Content-Type: application/json
Authorization: Bearer dfad4bf3491892ae734f790f43851a07ee4754444ded242a696e1cbeeb62fa0a
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfad4bf3491892ae734f790f43851a07ee4754444ded242a696e1cbeeb62fa0a"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/6/bookmark
Content-Type: application/json
Authorization: Bearer 7ae08e49e873bfc57126b6c5d609798e4553af8a0c14e896e9d66b61d35a8bb6
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/6/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ae08e49e873bfc57126b6c5d609798e4553af8a0c14e896e9d66b61d35a8bb6"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/3/upvote
Content-Type: application/json
Authorization: Bearer 034338acffcaecd8b0744ca481e919fe578e0dc656ac1e8e54177de43f938f95
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/3/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 034338acffcaecd8b0744ca481e919fe578e0dc656ac1e8e54177de43f938f95"
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
    "key": "cache/f880980c74d75e24f7f3e27fe45a81d9.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNToyNzozM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Y4ODA5ODBjNzRkNzVlMjRmN2YzZTI3ZmU0NWE4MWQ5LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTQyNzMzWiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T142733Z",
    "x-amz-signature": "55c7b546d7b4c14284dae6e72c3150569bcdfee04fa7ae7e266d041297dbc623"
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
Authorization: Bearer 80777689b8cb607186aaefebcad2bd84771111221f5a6768f6deee3f63496a46
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
	-H "Authorization: Bearer 80777689b8cb607186aaefebcad2bd84771111221f5a6768f6deee3f63496a46"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 2a0f9cf15d1cf4f25091d46f9994f6ea57539a8a0d17323d74cf5c974cdb401b
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
	-H "Authorization: Bearer 2a0f9cf15d1cf4f25091d46f9994f6ea57539a8a0d17323d74cf5c974cdb401b"
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
{"password":{"reset_password_token":"9pXzJ7EZwhpZuGpi1HFQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 353,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T14:27:14.708Z",
  "updated_at": "2016-12-15T14:27:14.871Z",
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
  "audit_id": 7776
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"9pXzJ7EZwhpZuGpi1HFQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/119/comments
Content-Type: application/json
Authorization: Bearer 903cf9855cb43b81f57072ea4a0a5cccfb95ab5d71ff6c56c1103bc53e76becf
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
    "id": 17,
    "author_id": 797,
    "reply_to_id": null,
    "created_at": "2016-12-15T14:27:55.211Z",
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
curl "api.goskive.com/v2/questions/119/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 903cf9855cb43b81f57072ea4a0a5cccfb95ab5d71ff6c56c1103bc53e76becf"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/118/comments
Content-Type: application/json
Authorization: Bearer 0d35f1c3defee5e9ff243468628e09d4825f51685c573565c0a65378d3eaf586
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
    "id": 16,
    "author_id": 794,
    "reply_to_id": null,
    "created_at": "2016-12-15T14:27:54.702Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 794,
      "feedbackable_id": 118,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:54.699Z",
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
curl "api.goskive.com/v2/questions/118/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d35f1c3defee5e9ff243468628e09d4825f51685c573565c0a65378d3eaf586"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/122/comments
Content-Type: application/json
Authorization: Bearer 78169da195b5c106d10f499efd33e995deae6e8a7fafb195f9a9d7bd96f4d1ae
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
      "id": 19,
      "author_id": 810,
      "reply_to_id": null,
      "created_at": "2016-12-15T14:27:56.379Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 809,
      "reply_to_id": null,
      "created_at": "2016-12-15T14:27:56.362Z",
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
curl "api.goskive.com/v2/questions/122/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78169da195b5c106d10f499efd33e995deae6e8a7fafb195f9a9d7bd96f4d1ae"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/120/comments
Content-Type: application/json
Authorization: Bearer bbc438bce5e69a88c63e10d6e8f7f0487cdbfaa5c452b3671b6d7466ab20c1df
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
curl "api.goskive.com/v2/questions/120/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbc438bce5e69a88c63e10d6e8f7f0487cdbfaa5c452b3671b6d7466ab20c1df"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/85/feedbacks
Content-Type: application/json
Authorization: Bearer 6bd6cedce82d350e46809fae1503da67a5202a347f377e91487659409b0d9ac4
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
    "user_id": 596,
    "feedbackable_id": 85,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T14:27:39.153Z",
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
curl "api.goskive.com/v2/questions/85/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bd6cedce82d350e46809fae1503da67a5202a347f377e91487659409b0d9ac4"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/88/feedbacks
Content-Type: application/json
Authorization: Bearer 6fc20e0d3b8032b321bf47777e96cba70803b88fae565b439123c3ec19a77f94
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
      "id": 15,
      "user_id": 617,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:40.479Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 616,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T14:27:40.467Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/88/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fc20e0d3b8032b321bf47777e96cba70803b88fae565b439123c3ec19a77f94"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/56/votes
Content-Type: application/json
Authorization: Bearer 502a7e00b393323120e0f6f118bf6d367cb1b2fc887f244c6da9f471278d7fbe
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 56,
      "user_id": 341
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 56,
      "user_id": 340
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 56,
      "user_id": 339
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/56/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 502a7e00b393323120e0f6f118bf6d367cb1b2fc887f244c6da9f471278d7fbe"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/46/republish
Content-Type: application/json
Authorization: Bearer f214c5e452ec4e69b7cffc71b5cbe7725a70a4ea61e283c493ea2481b96cf5c4
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
curl "api.goskive.com/v2/questions/46/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f214c5e452ec4e69b7cffc71b5cbe7725a70a4ea61e283c493ea2481b96cf5c4"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/48/bookmark
Content-Type: application/json
Authorization: Bearer 029ffe216f7e8f7f06fdcfaf24c56d573522f2cadc6d32980f79ef0233f0e52f
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 029ffe216f7e8f7f06fdcfaf24c56d573522f2cadc6d32980f79ef0233f0e52f"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/49
Content-Type: application/json
Authorization: Bearer b5d0783594ed631080de2dd9716d9d4bdf916fca1817794992493dc85efba353
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5d0783594ed631080de2dd9716d9d4bdf916fca1817794992493dc85efba353"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/54/downvote
Content-Type: application/json
Authorization: Bearer 27f4157e91964be0d7e81879616afa030b94ef1a9c4786a1dbac58c473df4b98
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/54/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27f4157e91964be0d7e81879616afa030b94ef1a9c4786a1dbac58c473df4b98"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/45
Content-Type: application/json
Authorization: Bearer d2e50557650a7d4af780e10d1bb884ed505b7e9f87ed299f1c97234047879271
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
    "id": 45,
    "obfuscated_id": "IVleRnyZemc",
    "author_id": 303,
    "chapter_id": 62,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:07.424Z",
    "created_at": "2016-12-15T14:27:07.334Z",
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
        "id": 89,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 90,
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
curl "api.goskive.com/v2/questions/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2e50557650a7d4af780e10d1bb884ed505b7e9f87ed299f1c97234047879271"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/52/report
Content-Type: application/json
Authorization: Bearer 74b2f5b9160596aeed4e81b9bbafbb32a30370317b304d7809ecab7a60f8004e
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74b2f5b9160596aeed4e81b9bbafbb32a30370317b304d7809ecab7a60f8004e"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/50/bookmark
Content-Type: application/json
Authorization: Bearer d6b158bb10aa62446f7e5925d38a5c853cb61e9fcd5258dc2b99227e970ae23f
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6b158bb10aa62446f7e5925d38a5c853cb61e9fcd5258dc2b99227e970ae23f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/53
Content-Type: application/json
Authorization: Bearer bec11f3caeb865826c1022e6c2760991dda2b21118281f954dcd8c1941091445
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":53,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T14:27:10.462Z","updated_at":"2016-12-15T14:27:10.556Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":70,"author_id":327,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 53,
    "obfuscated_id": "XffxqHkTsbc",
    "author_id": 327,
    "chapter_id": 70,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T14:27:10.652Z",
    "created_at": "2016-12-15T14:27:10.462Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x00000003408ca8>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 105,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 106,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 107,
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
curl "api.goskive.com/v2/questions/53" -d '{"question":{"question":{"id":53,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T14:27:10.462Z","updated_at":"2016-12-15T14:27:10.556Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":70,"author_id":327,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bec11f3caeb865826c1022e6c2760991dda2b21118281f954dcd8c1941091445"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/51/upvote
Content-Type: application/json
Authorization: Bearer 06980e3d9db3ddf0781632445df76a91307121cfdd5c370424d5fbdeca74ae46
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/51/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06980e3d9db3ddf0781632445df76a91307121cfdd5c370424d5fbdeca74ae46"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 867f345db7d64770002ac967db02504b1141887900973443d038388600511fb4
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
      "creator_id": 6,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "discipline_id": 2,
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
      "updated_at": "2016-12-15T14:26:36.408Z",
      "shortname": "mit-pizza-201",
      "topic_id": 2,
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
	-H "Authorization: Bearer 867f345db7d64770002ac967db02504b1141887900973443d038388600511fb4"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 25de7427dd0555c790fa95be87cdd82eeb37fc6d1edeff2bf1ba84348424dca8
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
      "image_url": "memory://universities/29f58bd989a487d0c83c3bdd5dfb1145.jpg",
      "image_url_small": "memory://universities/6bd00fd85278b012cbc871b3d6f15b22.jpg",
      "image_thumb_url": "memory://universities/a2a1b883ce7a38fc0361564a483fae07.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T14:26:35.916Z",
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
      "image_url": "memory://universities/600fbef02101ef710868e3d133a426e5.jpg",
      "image_url_small": "memory://universities/26d816fca9ff158770dd452ccd73ea76.jpg",
      "image_thumb_url": "memory://universities/e219709141f80f02dbe7fc7945169d05.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T14:26:35.844Z",
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
	-H "Authorization: Bearer 25de7427dd0555c790fa95be87cdd82eeb37fc6d1edeff2bf1ba84348424dca8"
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
      "id": 132,
      "name": "Persistent grid-enabled encryption",
      "name_translations": {
        "en": "Persistent grid-enabled encryption"
      },
      "discipline_id": 133
    },
    {
      "id": 133,
      "name": "Virtual client-server migration",
      "name_translations": {
        "en": "Virtual client-server migration"
      },
      "discipline_id": 134
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
GET /v2/topics/131
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
    "id": 131,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 132
  }
}
```



```shell
curl "api.goskive.com/v2/topics/131" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 96564a5a0952ed64a489f0d72d0387b02aaf3b06782cd060d574ea66a424068d
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
      "id": 113,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-111",
      "html_url": "https://goskive.com/university/uni-111",
      "slug": "uni-111",
      "name": "University 78",
      "short_name": "Uni 111",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/9723e7c23f87bd6ce335d3e5e1364e34.jpg",
      "image_url_small": "memory://universities/74c094373863e63396d554435287eb63.jpg",
      "image_thumb_url": "memory://universities/97f7b6211e03faf6daba034166e3db50.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T14:27:15.239Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-112",
      "html_url": "https://goskive.com/university/uni-112",
      "slug": "uni-112",
      "name": "University 79",
      "short_name": "Uni 112",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/5a6afddadcd770d6ee7f523f327c1e26.jpg",
      "image_url_small": "memory://universities/d17ffc78068b52381de617449a93db8a.jpg",
      "image_thumb_url": "memory://universities/8b0798f588b824757772b9ad4af1a39c.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T14:27:15.309Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-113",
      "html_url": "https://goskive.com/university/uni-113",
      "slug": "uni-113",
      "name": "University 80",
      "short_name": "Uni 113",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/85024af0c0a3dfa94ea1436678392e9b.jpg",
      "image_url_small": "memory://universities/27c8a8f2110c1815d6c889cf7650b29f.jpg",
      "image_thumb_url": "memory://universities/9288ddc80df3cc49cd628330f013d0bd.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T14:27:15.408Z",
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
	-H "Authorization: Bearer 96564a5a0952ed64a489f0d72d0387b02aaf3b06782cd060d574ea66a424068d"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 8f2f1c51196ab49a2103fa16f9261396f173ef644627f34314855e6f0ddd9c9e
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
    "id": 112,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/69443c8201ee06da6057047d2c7c2730.jpg",
    "image_url_small": "memory://universities/b378c08b3090215a6b20c560efa4b3b4.jpg",
    "image_thumb_url": "memory://universities/5d6893984dff8e10c23c259ce86d8e2e.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T14:27:15.086Z",
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
	-H "Authorization: Bearer 8f2f1c51196ab49a2103fa16f9261396f173ef644627f34314855e6f0ddd9c9e"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0053518c5c99e881346356513811521947a2775b818de025d217015dbf5cfd07
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":142,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 442,
    "id": 132,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 138,
    "additional_university_ids": [

    ],
    "discipline_id": 143,
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
    "chapters_updated_at": "2016-12-15T14:27:24.243Z",
    "updated_at": "2016-12-15T14:27:24.408Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 95,
        "updated_at": "2016-12-15T14:27:24.397Z",
        "course_id": 132,
        "author_id": 442,
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
        "id": 96,
        "updated_at": "2016-12-15T14:27:24.411Z",
        "course_id": 132,
        "author_id": 442,
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
        "id": 97,
        "updated_at": "2016-12-15T14:27:24.425Z",
        "course_id": 132,
        "author_id": 442,
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
    "topic_id": 142,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":142,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0053518c5c99e881346356513811521947a2775b818de025d217015dbf5cfd07"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ffc678daccd1c25d449e680592160d71f862c3ad7a5591e7058c0fae8a0f25ab
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":143,"published":false}}
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
    "creator_id": 443,
    "id": 133,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 139,
    "additional_university_ids": [

    ],
    "discipline_id": 144,
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
    "updated_at": "2016-12-15T14:27:24.693Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 143,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":143,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffc678daccd1c25d449e680592160d71f862c3ad7a5591e7058c0fae8a0f25ab"
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
      "creator_id": 445,
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-94",
      "html_url": "https://goskive.com/course/fu-course-94",
      "slug": "fu-course-94",
      "university_id": 140,
      "additional_university_ids": [

      ],
      "discipline_id": 147,
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
      "updated_at": "2016-12-15T14:27:24.926Z",
      "shortname": "fu-course-94",
      "topic_id": 146,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 94",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 445,
      "id": 137,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-95",
      "html_url": "https://goskive.com/course/fu-course-95",
      "slug": "fu-course-95",
      "university_id": 140,
      "additional_university_ids": [

      ],
      "discipline_id": 148,
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
      "chapters_updated_at": "2016-12-15T14:27:24.740Z",
      "updated_at": "2016-12-15T14:27:25.211Z",
      "shortname": "fu-course-95",
      "topic_id": 147,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 95",
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
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e82e9adefab60017d0923873da2298b662c440a9ef128b2fd01d269c8e1a2f63
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
      "creator_id": 452,
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "discipline_id": 155,
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
      "updated_at": "2016-12-15T14:27:25.786Z",
      "shortname": "fu-course-102",
      "topic_id": 154,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 452,
      "id": 145,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 143,
      "additional_university_ids": [

      ],
      "discipline_id": 156,
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
      "chapters_updated_at": "2016-12-15T14:27:25.602Z",
      "updated_at": "2016-12-15T14:27:26.067Z",
      "shortname": "fu-course-103",
      "topic_id": 155,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e82e9adefab60017d0923873da2298b662c440a9ef128b2fd01d269c8e1a2f63"
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
      "creator_id": 450,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "discipline_id": 151,
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
      "updated_at": "2016-12-15T14:27:25.438Z",
      "shortname": "fu-course-98",
      "topic_id": 150,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 450,
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-99",
      "html_url": "https://goskive.com/course/fu-course-99",
      "slug": "fu-course-99",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "discipline_id": 152,
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
      "updated_at": "2016-12-15T14:27:25.475Z",
      "shortname": "fu-course-99",
      "topic_id": 151,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 99",
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
Authorization: Bearer 7598d0f47d17b0321b052f0f3cdd628a123a7dcc4b393b6615974105c4616265
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
      "creator_id": 458,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 144,
      "additional_university_ids": [

      ],
      "discipline_id": 159,
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
      "updated_at": "2016-12-15T14:27:26.346Z",
      "shortname": "fu-course-106",
      "topic_id": 158,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 458,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 144,
      "additional_university_ids": [

      ],
      "discipline_id": 160,
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
      "updated_at": "2016-12-15T14:27:26.383Z",
      "shortname": "fu-course-107",
      "topic_id": 159,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7598d0f47d17b0321b052f0f3cdd628a123a7dcc4b393b6615974105c4616265"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 48f2f4b4bc86f5f904f388314a8262069be3c169e3cdc81cf0a0e1897e82d36f
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
  "id": 119,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T14:26:45.194Z",
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
	-H "Authorization: Bearer 48f2f4b4bc86f5f904f388314a8262069be3c169e3cdc81cf0a0e1897e82d36f"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/894
Content-Type: application/json
Authorization: Bearer a81b8a7bc61a059b2f9fe7c0757d677f31940aa4489cb8f21d169a1a2b0e04ad
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
    "id": 894,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 260,
    "fields_of_study": [
      286,
      287
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T14:28:03.558Z",
    "updated_at": "2016-12-15T14:28:03.558Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/894" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a81b8a7bc61a059b2f9fe7c0757d677f31940aa4489cb8f21d169a1a2b0e04ad"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/892
Content-Type: application/json
Authorization: Bearer 3df4a336ade14fb6584afaf5db9bcef7df57191b853637839c7eb6552f3e031c
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
    "id": 892,
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
    "created_at": "2016-12-15T14:28:03.340Z",
    "updated_at": "2016-12-15T14:28:03.340Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/892" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3df4a336ade14fb6584afaf5db9bcef7df57191b853637839c7eb6552f3e031c"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/3
Content-Type: application/json
Authorization: Bearer 54769f5b820960daf0f5f4f61311d967e24815a7a99b3130e54cd52083a7767f
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54769f5b820960daf0f5f4f61311d967e24815a7a99b3130e54cd52083a7767f"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/4
Content-Type: application/json
Authorization: Bearer 4a2523f828871df6e5fd409a2297f792e583f5dc250be9ba5e849a237aeeeb06
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
    "id": 4,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 2,
    "user_id": 128
  }
}
```



```shell
curl "api.goskive.com/v2/votes/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a2523f828871df6e5fd409a2297f792e583f5dc250be9ba5e849a237aeeeb06"
```
