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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"9aea8988236ccfcfb864d84b31aa9a90b6568354fe318635e25badb6641bb9bb","client_secret":"a27d5a987e2ecaf139db207c12747c9448a23e39d566025670775f222af1207e"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"9aea8988236ccfcfb864d84b31aa9a90b6568354fe318635e25badb6641bb9bb","client_secret":"a27d5a987e2ecaf139db207c12747c9448a23e39d566025670775f222af1207e"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MzRlZmM1MzYwMjYzNjdlNTQxZjZjMzM5ZjQzZDI0MDg4MDhlNzdlZWM1ZDQw
NTg1MGRjZGM3ZjlmOWU3YmYyNDphMWFjYWFmZGIzZjY3NTg3MTRkN2UxMzcx
Nzg0NmQxMGUzODEyMTRhZjQ3YWMwNWZiMjQ5MTkzMmY2MGNiMGEz

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
	-u 34efc536026367e541f6c339f43d2408808e77eec5d405850dcdc7f9f9e7bf24:a1acaafdb3f6758714d7e13717846d10e381214af47ac05fb2491932f60cb0a3
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
{"grant_type":"client_credentials","client_id":"08cf4845c63cc4d89fe6a6419eb327944877c5aa7070f10a224c4653350a9fc1","client_secret":"5d814f4caa389eb8913bf3e1842508b4018e4a6d3f79cbc9285d5f848467d89c"}
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
  "access_token": "7c5a944f957dc589d69ffa603dcb6a1f8df6a1c84e174e78e677e7283009d11b",
  "token_type": "bearer",
  "created_at": 1477062266
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"08cf4845c63cc4d89fe6a6419eb327944877c5aa7070f10a224c4653350a9fc1","client_secret":"5d814f4caa389eb8913bf3e1842508b4018e4a6d3f79cbc9285d5f848467d89c"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"13c4fac1643b704645c22c78f903f3ef643663dce0e54581bb7d5236662f738b","client_secret":"926e0b54405a8f344650b97105d92dd8cc1e8618d6dfb747858fcd06b1a38f65"}
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
  "access_token": "cca55a7a86d06f75998f295eceddae8a7e12d9cc299d649959b0fc5be6c14a14",
  "token_type": "bearer",
  "created_at": 1477062266
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"13c4fac1643b704645c22c78f903f3ef643663dce0e54581bb7d5236662f738b","client_secret":"926e0b54405a8f344650b97105d92dd8cc1e8618d6dfb747858fcd06b1a38f65"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MWY1YzZjYWY3ZGRmZDc0NGU0Y2FjMzdjYjY2NmZhYThmZDA5ZmE0ZjI5ZWM5
ZWI5ZjZkMmQ1ZTg1YzI5ZTY0YTo1ZDY5ODZiNzczNDY0MTcwNmZlNTI3YmI1
YThiNzQwOTRlMDJmNmJjMGMzMTlmZjVkMWNlYjg5ZmM2MWE3ZTlm

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
  "access_token": "0dfc09ff92310cb22fddf7abd00d8dc0b0c5da2d62cf0324d17f7e17715a74d1",
  "token_type": "bearer",
  "created_at": 1477062266
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 1f5c6caf7ddfd744e4cac37cb666faa8fd09fa4f29ec9eb9f6d2d5e85c29e64a:5d6986b7734641706fe527bb5a8b74094e02f6bc0c319ff5d1ceb89fc61a7e9f
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
Authorization: Bearer 7469d47babc32f662655853e676a91ac75b3290c035537eed3b42b32dcc958df
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
    "company_id": 28,
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
	-H "Authorization: Bearer 7469d47babc32f662655853e676a91ac75b3290c035537eed3b42b32dcc958df"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/158/flashcards
Content-Type: application/json
Authorization: Bearer 488c7b02d8290d54e909a88ecd9013004af0f9d918f0e2533465ca218f287451
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":158,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 75,
    "obfuscated_id": "rRYuZazyhgg",
    "author_id": 662,
    "chapter_id": 158,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:31.807Z",
    "created_at": "2016-10-21T15:04:31.807Z",
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
curl "api.goskive.com/v2/chapters/158/flashcards" -d '{"flashcard":{"chapter_id":158,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 488c7b02d8290d54e909a88ecd9013004af0f9d918f0e2533465ca218f287451"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/159/flashcards
Content-Type: application/json
Authorization: Bearer 953edb430a52c694927bd42cca373a419feffd39fd50ed492ee1613612ec84a1
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 663,
      "chapter_id": 159,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:31.958Z",
      "created_at": "2016-10-21T15:04:31.958Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 663,
      "chapter_id": 159,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:31.996Z",
      "created_at": "2016-10-21T15:04:31.996Z",
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 663,
      "chapter_id": 159,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:32.034Z",
      "created_at": "2016-10-21T15:04:32.034Z",
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
curl "api.goskive.com/v2/chapters/159/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 953edb430a52c694927bd42cca373a419feffd39fd50ed492ee1613612ec84a1"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/165/questions
Content-Type: application/json
Authorization: Bearer 7d862ab4f8c50b938d853ec7405d76d8db0530a7d2b5209eb2bb842abae74c7d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":165,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 802,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:40.843Z",
    "created_at": "2016-10-21T15:04:40.843Z",
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
        "id": 239,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 240,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 241,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 242,
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
curl "api.goskive.com/v2/chapters/165/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":165,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d862ab4f8c50b938d853ec7405d76d8db0530a7d2b5209eb2bb842abae74c7d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/162/questions
Content-Type: application/json
Authorization: Bearer a0cf32c5a854c4031bc39a133c4077cb482133d8716d572cea19653f377de5b4
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
    "id": 116,
    "obfuscated_id": "PhHGVKqnHFA",
    "author_id": 793,
    "chapter_id": 162,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:39.542Z",
    "created_at": "2016-10-21T15:04:39.542Z",
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
        "id": 232,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 233,
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
	-H "Authorization: Bearer a0cf32c5a854c4031bc39a133c4077cb482133d8716d572cea19653f377de5b4"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/164/questions
Content-Type: application/json
Authorization: Bearer 80f1ee0efaad5bc4223b84912f6c882b473b8b77b5ed932e6da15df415557973
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":164,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 799,
    "chapter_id": 164,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:40.488Z",
    "created_at": "2016-10-21T15:04:40.488Z",
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
        "id": 237,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 238,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/164/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":164,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80f1ee0efaad5bc4223b84912f6c882b473b8b77b5ed932e6da15df415557973"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/163/questions
Content-Type: application/json
Authorization: Bearer 6250f259199e90f950e063f03c4ae7e2e3bb58ad994f3d525e31c2f13783d8f7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":163,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 796,
    "chapter_id": 163,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:40.060Z",
    "created_at": "2016-10-21T15:04:40.060Z",
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
curl "api.goskive.com/v2/chapters/163/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":163,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6250f259199e90f950e063f03c4ae7e2e3bb58ad994f3d525e31c2f13783d8f7"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/167/questions
Content-Type: application/json
Authorization: Bearer 875cbff313cc58de829674a3306afd818e837117814dee2166bb713a382f15a8
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
      "id": 120,
      "obfuscated_id": "vEr9LtFjURM",
      "author_id": 808,
      "chapter_id": 167,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:41.596Z",
      "created_at": "2016-10-21T15:04:41.476Z",
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
          "id": 243,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 244,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 809,
      "chapter_id": 167,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:41.794Z",
      "created_at": "2016-10-21T15:04:41.671Z",
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
      "author_id": 810,
      "chapter_id": 167,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-21T15:04:41.993Z",
      "created_at": "2016-10-21T15:04:41.870Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/167/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 875cbff313cc58de829674a3306afd818e837117814dee2166bb713a382f15a8"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/37
Content-Type: application/json
Authorization: Bearer 20be5868187c5110a81fc2b5370a1156df4231a9fa02406390e63ddd520ac541
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
	-H "Authorization: Bearer 20be5868187c5110a81fc2b5370a1156df4231a9fa02406390e63ddd520ac541"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/40
Content-Type: application/json
Authorization: Bearer b4c1a5a0824d93e57cdcd6b18359eed5d777c52463c045c43ca51cd236bc2322
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
curl "api.goskive.com/v2/chapters/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4c1a5a0824d93e57cdcd6b18359eed5d777c52463c045c43ca51cd236bc2322"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/35
Content-Type: application/json
Authorization: Bearer 19e9115abd9cd54adb652405c0e41379298fb3fe1c885d45c993d36d58ef827d
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
curl "api.goskive.com/v2/chapters/35" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19e9115abd9cd54adb652405c0e41379298fb3fe1c885d45c993d36d58ef827d"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/39
Content-Type: application/json
Authorization: Bearer 854004a0175d9608ef78b822b3385d6e33f088f62c9cd5066859789efb757d71
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/39" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 854004a0175d9608ef78b822b3385d6e33f088f62c9cd5066859789efb757d71"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/33
Content-Type: application/json
Authorization: Bearer 22fe6870f852ffea502f342bbaa5c45cbb1cb353d645e12ea79ba6adc4ec6c8a
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
    "id": 33,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-21T15:03:55.117Z",
    "course_id": 81,
    "author_id": 174,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-21T15:03:54.571Z",
    "questions_updated_at": "2016-10-21T15:03:54.571Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 178,
        "chapter_id": 33,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:55.100Z",
        "created_at": "2016-10-21T15:03:55.100Z",
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
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 176,
        "chapter_id": 33,
        "position": 50,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:54.990Z",
        "created_at": "2016-10-21T15:03:54.869Z",
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
            "id": 99,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 100,
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
curl "api.goskive.com/v2/chapters/33" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22fe6870f852ffea502f342bbaa5c45cbb1cb353d645e12ea79ba6adc4ec6c8a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/34
Content-Type: application/json
Authorization: Bearer e108dfa3e1f48a91a001ea38318f25f0daa0074b3e8bf2ff839f70a8550545a5
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
    "id": 34,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-21T15:03:55.319Z",
    "course_id": 82,
    "author_id": 181,
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
curl "api.goskive.com/v2/chapters/34" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e108dfa3e1f48a91a001ea38318f25f0daa0074b3e8bf2ff839f70a8550545a5"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/59/replies
Content-Type: application/json
Authorization: Bearer a6a6596ad3544be49fad220a23aaeb55b97be901398caabc4e0fa656441788dc
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
    "author_id": 950,
    "reply_to_id": 59,
    "created_at": "2016-10-21T15:04:53.886Z",
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
	-H "Authorization: Bearer a6a6596ad3544be49fad220a23aaeb55b97be901398caabc4e0fa656441788dc"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 8d5e8f6819e728616f3c6fd9bb92739c2399c4f435cc4f88051ec476e1e0d665
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
	-H "Authorization: Bearer 8d5e8f6819e728616f3c6fd9bb92739c2399c4f435cc4f88051ec476e1e0d665"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/45
Content-Type: application/json
Authorization: Bearer bb0fb7700b266275c4b6b0fa2f88f2977393d8abb73917d685df96cd274af6bb
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
	-H "Authorization: Bearer bb0fb7700b266275c4b6b0fa2f88f2977393d8abb73917d685df96cd274af6bb"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/47/republish
Content-Type: application/json
Authorization: Bearer 12c77c0f02becbf98dc2b35cecd60782206e6ea875a631bb0b09a61a57f2e815
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
curl "api.goskive.com/v2/comments/47/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12c77c0f02becbf98dc2b35cecd60782206e6ea875a631bb0b09a61a57f2e815"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/44
Content-Type: application/json
Authorization: Bearer 7de8359c20d779625cb71a50d6b6aaa94ebed0a44ea8785b5ba7505c373cfcc3
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7de8359c20d779625cb71a50d6b6aaa94ebed0a44ea8785b5ba7505c373cfcc3"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/46/report
Content-Type: application/json
Authorization: Bearer ff21215e3c3ddb9ac20a6414ac490008eb2846fa8c081b7b1aa848de4ba71815
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff21215e3c3ddb9ac20a6414ac490008eb2846fa8c081b7b1aa848de4ba71815"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/27
Content-Type: application/json
Authorization: Bearer afd22f0e7e6e01fe136b267ac57b952933a0a20491590926ff9567bd32858382
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
    "id": 27,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-21T15:04:26.996Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afd22f0e7e6e01fe136b267ac57b952933a0a20491590926ff9567bd32858382"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f660fdbc52fc9615ba70cf6c20c4d7b7e4100d02a38fc0aeac6b10f8a37b49a1
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
      "id": 24,
      "name": "Fake Company Name 21",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-21T15:04:26.870Z"
    },
    {
      "id": 25,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-21T15:04:26.874Z"
    },
    {
      "id": 26,
      "name": "Fake Company Name 23",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-21T15:04:26.878Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f660fdbc52fc9615ba70cf6c20c4d7b7e4100d02a38fc0aeac6b10f8a37b49a1"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer e658f43afe5e132d020708ec397ecaedd37cb0f4954ec2903ead6068a4a0ed7c
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e658f43afe5e132d020708ec397ecaedd37cb0f4954ec2903ead6068a4a0ed7c"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer a9ed673a6572f5c64eb0902d386353c271d70e5bf84d0ba52e7178bda733897d
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9ed673a6572f5c64eb0902d386353c271d70e5bf84d0ba52e7178bda733897d"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer d1538362140bc8390ca4fee29c59a127bb81fc692dfeb8e997b168f4142aa169
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 1,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 1,
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
          "image_url_absolute": "banners/8dbf7d28f3cbdc6d654d6324af20a11fe3653b85.png",
          "target_url": "http://goskive.com",
          "id": 1,
          "target_url_ios": "http://goskive.com",
          "target_url_android": "http://goskive.com",
          "screens": [

          ]
        }
      ]
    },
    {
      "id": 4,
      "title": "Campaign 4",
      "company_id": 4,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 2,
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
          "image_url_absolute": "banners/889019b341716d48f4f28718872d4f688cd18499.png",
          "target_url": "http://goskive.com",
          "id": 2,
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
	-H "Authorization: Bearer d1538362140bc8390ca4fee29c59a127bb81fc692dfeb8e997b168f4142aa169"
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
Authorization: Bearer d7462caddea409a4ebc4fcd09a7f066e775e1fed441cf48365cc24bb9525ed81
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
	-H "Authorization: Bearer d7462caddea409a4ebc4fcd09a7f066e775e1fed441cf48365cc24bb9525ed81"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a4603a56bd53ccb915df0e90a56ab7192579cf82916dac1804fbd39c9681c2c8
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
    "id": 130,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-21T15:04:26.258Z",
    "course_id": 186,
    "author_id": 562,
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
	-H "Authorization: Bearer a4603a56bd53ccb915df0e90a56ab7192579cf82916dac1804fbd39c9681c2c8"
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
      "id": 109,
      "title": "Clever Chapter Title 97",
      "position": 1,
      "updated_at": "2016-10-21T15:04:23.700Z",
      "course_id": 175,
      "author_id": 516,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 110,
      "title": "Clever Chapter Title 98",
      "position": 2,
      "updated_at": "2016-10-21T15:04:23.726Z",
      "course_id": 175,
      "author_id": 517,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 111,
      "title": "Clever Chapter Title 99",
      "position": 3,
      "updated_at": "2016-10-21T15:04:23.990Z",
      "course_id": 175,
      "author_id": 518,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-21T15:04:23.619Z",
      "questions_updated_at": "2016-10-21T15:04:23.619Z",
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
Authorization: Bearer d640be3b17f935f41256006a4c8c3731cf0c3fdc02951daba61dfc64b3272f60
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
      "id": 115,
      "title": "Clever Chapter Title 103",
      "position": 1,
      "updated_at": "2016-10-21T15:04:24.367Z",
      "course_id": 178,
      "author_id": 527,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 116,
      "title": "Clever Chapter Title 104",
      "position": 2,
      "updated_at": "2016-10-21T15:04:24.392Z",
      "course_id": 178,
      "author_id": 528,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 117,
      "title": "Clever Chapter Title 105",
      "position": 3,
      "updated_at": "2016-10-21T15:04:24.652Z",
      "course_id": 178,
      "author_id": 529,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-21T15:04:24.286Z",
      "questions_updated_at": "2016-10-21T15:04:24.286Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d640be3b17f935f41256006a4c8c3731cf0c3fdc02951daba61dfc64b3272f60"
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
      "id": 112,
      "title": "Clever Chapter Title 100",
      "position": 1,
      "updated_at": "2016-10-21T15:04:24.115Z",
      "course_id": 176,
      "author_id": 522,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 113,
      "title": "Clever Chapter Title 101",
      "position": 2,
      "updated_at": "2016-10-21T15:04:24.140Z",
      "course_id": 176,
      "author_id": 523,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 114,
      "title": "Clever Chapter Title 102",
      "position": 3,
      "updated_at": "2016-10-21T15:04:24.164Z",
      "course_id": 176,
      "author_id": 524,
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
Authorization: Bearer 12c9b2910832b98ffbc3712b047a93ced292e154ada667dae9bf438f4fba7ce2
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
      "title": "Clever Chapter Title 106",
      "position": 1,
      "updated_at": "2016-10-21T15:04:24.924Z",
      "course_id": 180,
      "author_id": 536,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 119,
      "title": "Clever Chapter Title 107",
      "position": 2,
      "updated_at": "2016-10-21T15:04:24.949Z",
      "course_id": 180,
      "author_id": 537,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 120,
      "title": "Clever Chapter Title 108",
      "position": 3,
      "updated_at": "2016-10-21T15:04:24.975Z",
      "course_id": 180,
      "author_id": 538,
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
	-H "Authorization: Bearer 12c9b2910832b98ffbc3712b047a93ced292e154ada667dae9bf438f4fba7ce2"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d576c5fff97b04d854fcb5ba68dd6e3f154adbe6cb8b952cc217a246ae4c8692
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
    "id": 2,
    "course_id": 97,
    "user_id": 220,
    "updated_at": "2016-10-21T15:03:58.708Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d576c5fff97b04d854fcb5ba68dd6e3f154adbe6cb8b952cc217a246ae4c8692"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 19771f5c3d0d1be6970e4404c56a18e33163ccf0e9c7d7a8e5fcd64db94a0434
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
      "course_id": 100,
      "user_id": 228,
      "updated_at": "2016-10-21T15:03:59.104Z"
    },
    {
      "id": 6,
      "course_id": 100,
      "user_id": 229,
      "updated_at": "2016-10-21T15:03:59.119Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19771f5c3d0d1be6970e4404c56a18e33163ccf0e9c7d7a8e5fcd64db94a0434"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/297/files
Content-Type: application/json
Authorization: Bearer f05d582bdd410731f4a773af34aea1b7b97920dda7284e02126a42ac817be5cd
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
      "id": 13,
      "uploader": {
        "id": 904,
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
        "created_at": "2016-10-21T15:04:48.812Z",
        "updated_at": "2016-10-21T15:04:48.812Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-21T15:04:48.822Z",
      "updated_at": "2016-10-21T15:04:48.822Z",
      "course_id": 297,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 905,
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
        "created_at": "2016-10-21T15:04:48.829Z",
        "updated_at": "2016-10-21T15:04:48.829Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-21T15:04:48.838Z",
      "updated_at": "2016-10-21T15:04:48.838Z",
      "course_id": 297,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 15,
      "uploader": {
        "id": 906,
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
        "created_at": "2016-10-21T15:04:48.845Z",
        "updated_at": "2016-10-21T15:04:48.845Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-21T15:04:48.853Z",
      "updated_at": "2016-10-21T15:04:48.853Z",
      "course_id": 297,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/297/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f05d582bdd410731f4a773af34aea1b7b97920dda7284e02126a42ac817be5cd"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/295/files
Content-Type: application/json
Authorization: Bearer 7150c625d81a2f5cf1d77e31cb1becbcc762d4b2f8be80fb7a6a9963ca74e56d
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
    "id": 12,
    "uploader": {
      "id": 900,
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
      "created_at": "2016-10-21T15:04:48.555Z",
      "updated_at": "2016-10-21T15:04:48.555Z"
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
    "created_at": "2016-10-21T15:04:48.586Z",
    "updated_at": "2016-10-21T15:04:48.586Z",
    "course_id": 295,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/295/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7150c625d81a2f5cf1d77e31cb1becbcc762d4b2f8be80fb7a6a9963ca74e56d"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/296/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer e4a2586e4ffd6b36c54d62d44425e346d1e71e8d3756450408f31ca9c366a468
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
  "url": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com",
  "fields": {
    "key": "cache/0f3686048832a704b542ca3c002402de.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMVQxNjowNDo0OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzBmMzY4NjA0ODgzMmE3MDRiNTQyY2EzYzAwMjQwMmRlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjEvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDIxVDE1MDQ0OFoifV19",
    "x-amz-credential": "FAKE/20161021/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161021T150448Z",
    "x-amz-signature": "232c556567b35315aadb04eeccc5dc9e06b32d1d2eeafcf05c0c319cc0910233"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/296/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4a2586e4ffd6b36c54d62d44425e346d1e71e8d3756450408f31ca9c366a468"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 4501cca05c41ad280e2e762c50ce0ca1b26c5cb4c7282007c01486d38e95468a
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
	-H "Authorization: Bearer 4501cca05c41ad280e2e762c50ce0ca1b26c5cb4c7282007c01486d38e95468a"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5f875f4efbcfc001e65a7572db8f87430cece16cb2810408cbe5444fa30ccb2a
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
	-H "Authorization: Bearer 5f875f4efbcfc001e65a7572db8f87430cece16cb2810408cbe5444fa30ccb2a"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2d4320a693fc98b83f603188d7b6de33534b76a54abbacaa4597b47fc054a8d0
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
	-H "Authorization: Bearer 2d4320a693fc98b83f603188d7b6de33534b76a54abbacaa4597b47fc054a8d0"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a9335d85d11615a6ea841101aab3c4600c87a5d06bd88956f85bfd3900ba4917
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
	-H "Authorization: Bearer a9335d85d11615a6ea841101aab3c4600c87a5d06bd88956f85bfd3900ba4917"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 85919779555610a877c0d99e13d5e62afd052dff7bd9ab8a33e17de7cd905a88
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
	-H "Authorization: Bearer 85919779555610a877c0d99e13d5e62afd052dff7bd9ab8a33e17de7cd905a88"
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
    "creator_id": 73,
    "id": 25,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 25,
    "additional_university_ids": [

    ],
    "topic_id": 25,
    "discipline_id": 25,
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
    "chapters_updated_at": "2016-10-21T15:03:42.387Z",
    "updated_at": "2016-10-21T15:03:43.847Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 12,
        "title": "Clever Chapter Title 12",
        "position": 1,
        "updated_at": "2016-10-21T15:03:43.800Z",
        "course_id": 25,
        "author_id": 73,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-21T15:03:42.387Z",
        "questions_updated_at": "2016-10-21T15:03:42.387Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 13,
        "title": "Clever Chapter Title 13",
        "position": 2,
        "updated_at": "2016-10-21T15:03:43.840Z",
        "course_id": 25,
        "author_id": 73,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-21T15:03:42.387Z",
        "questions_updated_at": "2016-10-21T15:03:42.387Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 73,
        "chapter_id": 12,
        "position": 20,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:42.604Z",
        "created_at": "2016-10-21T15:03:42.484Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 73,
        "chapter_id": 13,
        "position": 22,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:42.984Z",
        "created_at": "2016-10-21T15:03:42.863Z",
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
Authorization: Bearer ad6045dc9f72954b3ccd9b4bda77870297cda559dbb9c1ecd00623573b1beac0
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
    "creator_id": 84,
    "id": 27,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 27,
    "additional_university_ids": [

    ],
    "topic_id": 27,
    "discipline_id": 27,
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
    "chapters_updated_at": "2016-10-21T15:03:45.466Z",
    "updated_at": "2016-10-21T15:03:46.942Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 16,
        "title": "Clever Chapter Title 16",
        "position": 1,
        "updated_at": "2016-10-21T15:03:46.895Z",
        "course_id": 27,
        "author_id": 84,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-21T15:03:45.466Z",
        "questions_updated_at": "2016-10-21T15:03:45.466Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 17,
        "title": "Clever Chapter Title 17",
        "position": 2,
        "updated_at": "2016-10-21T15:03:46.935Z",
        "course_id": 27,
        "author_id": 84,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-21T15:03:45.466Z",
        "questions_updated_at": "2016-10-21T15:03:45.466Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 85,
        "chapter_id": 16,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.702Z",
        "created_at": "2016-10-21T15:03:46.702Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 85,
        "chapter_id": 17,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.774Z",
        "created_at": "2016-10-21T15:03:46.774Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 85,
        "chapter_id": 16,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.742Z",
        "created_at": "2016-10-21T15:03:46.742Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 85,
        "chapter_id": 17,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.814Z",
        "created_at": "2016-10-21T15:03:46.814Z",
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
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 85,
        "chapter_id": 16,
        "position": 32,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.680Z",
        "created_at": "2016-10-21T15:03:45.565Z",
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
          }
        ]
      },
      {
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 85,
        "chapter_id": 16,
        "position": 33,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:45.851Z",
        "created_at": "2016-10-21T15:03:45.742Z",
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
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 85,
        "chapter_id": 17,
        "position": 34,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.051Z",
        "created_at": "2016-10-21T15:03:45.931Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 85,
        "chapter_id": 17,
        "position": 35,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-21T15:03:46.233Z",
        "created_at": "2016-10-21T15:03:46.117Z",
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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad6045dc9f72954b3ccd9b4bda77870297cda559dbb9c1ecd00623573b1beac0"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/19/pin
Content-Type: application/json
Authorization: Bearer 173130a0530e216cc68ef06b887e11a765c290dc1e6be1285cb317d9b0733b38
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/19/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 173130a0530e216cc68ef06b887e11a765c290dc1e6be1285cb317d9b0733b38"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/18/pin
Content-Type: application/json
Authorization: Bearer ab004ae6017b4e4b6836946c682abcdc3b9777505728c8affcd55e213c6b2e1c
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/18/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab004ae6017b4e4b6836946c682abcdc3b9777505728c8affcd55e213c6b2e1c"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 88c9bda2c394a7b56789bed62582ffa0f75ede486619e966f221131afa15ae32
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
    "creator_id": 62,
    "id": 21,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 21,
    "additional_university_ids": [

    ],
    "topic_id": 21,
    "discipline_id": 21,
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
    "updated_at": "2016-10-21T15:03:40.546Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88c9bda2c394a7b56789bed62582ffa0f75ede486619e966f221131afa15ae32"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer e5db0a786d46553b649e782dc0966efc5258048cfca894fff276c5ba8042c483
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
    "id": 865,
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
    "created_at": "2016-10-21T15:04:46.012Z",
    "updated_at": "2016-10-21T15:04:46.012Z",
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
	-H "Authorization: Bearer e5db0a786d46553b649e782dc0966efc5258048cfca894fff276c5ba8042c483"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 636dd86767e70c5d6cd3c4fd48c244644d164511a8be2a1603b5929fec6423f6
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[292]}
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
    "id": 861,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      292
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-21T15:04:45.697Z",
    "updated_at": "2016-10-21T15:04:45.735Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[292]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 636dd86767e70c5d6cd3c4fd48c244644d164511a8be2a1603b5929fec6423f6"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 94c356c00ff1b34e3e18be2324be5a990415780f26963c06cdf8b3a968e26d81
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
    "id": 863,
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
    "created_at": "2016-10-21T15:04:45.856Z",
    "updated_at": "2016-10-21T15:04:45.856Z",
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
	-H "Authorization: Bearer 94c356c00ff1b34e3e18be2324be5a990415780f26963c06cdf8b3a968e26d81"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 082840dae0a50ccb937fe925d3743e0f614d89c0f8e1094fb4771684dbf74444
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[293]}
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
    "id": 862,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      293
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-21T15:04:45.804Z",
    "updated_at": "2016-10-21T15:04:45.804Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[293]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 082840dae0a50ccb937fe925d3743e0f614d89c0f8e1094fb4771684dbf74444"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer cc121b23bc91b8ac881686658bbe4ebd298382369028958361bfba616c2b39d8
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

291
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
    "id": 860,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/5e3b5b7694866d5e9cdaad692c7c94634e0101e1.jpg",
    "university_id": null,
    "fields_of_study": [
      291
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-21T15:04:45.357Z",
    "updated_at": "2016-10-21T15:04:45.638Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/a2549d259c8840e1ae01449ee223f56f8ee06ca4.jpg",
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

291
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer cc121b23bc91b8ac881686658bbe4ebd298382369028958361bfba616c2b39d8"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer f4b79f17c4686b6e241b83bab31d759ebea56498758e5c98d39cd8591e3e6b8c
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
      "bookmarkable_id": 44,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 45,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 46,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4b79f17c4686b6e241b83bab31d759ebea56498758e5c98d39cd8591e3e6b8c"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 6a5459f8ed720bcc77c0d7115fe0189034c644577413a8eb8ee3980e1b388d22
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
	-H "Authorization: Bearer 6a5459f8ed720bcc77c0d7115fe0189034c644577413a8eb8ee3980e1b388d22"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 58d9dacbaac2cb5183d9df69da065d2a53535beaf9ecfc6c86a2bd123a7115c0
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
	-H "Authorization: Bearer 58d9dacbaac2cb5183d9df69da065d2a53535beaf9ecfc6c86a2bd123a7115c0"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 4055c2064e464d407737b93922226d0ca06bde92a1282696e46cf36b21856e36
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
      "creator_id": 54,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-6",
      "html_url": "https://goskive.com/course/mit-course-6",
      "slug": "mit-course-6",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 16,
      "discipline_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
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
      "updated_at": "2016-10-21T15:03:39.863Z",
      "shortname": "mit-course-6"
    },
    {
      "creator_id": 55,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-7",
      "html_url": "https://goskive.com/course/mit-course-7",
      "slug": "mit-course-7",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 17,
      "discipline_id": 17,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
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
      "updated_at": "2016-10-21T15:03:39.962Z",
      "shortname": "mit-course-7"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4055c2064e464d407737b93922226d0ca06bde92a1282696e46cf36b21856e36"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 39a59dc22670801313ab97402612b3c1f819b761586ac5b3d65db05b7be5e85b
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-21T15:04:18.692Z"
      },
      "created_at": "2016-10-21T15:04:18.696Z",
      "updated_at": "2016-10-21T15:04:18.696Z",
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 19",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-21T15:04:18.704Z"
      },
      "created_at": "2016-10-21T15:04:18.708Z",
      "updated_at": "2016-10-21T15:04:18.708Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39a59dc22670801313ab97402612b3c1f819b761586ac5b3d65db05b7be5e85b"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 48ca456816831760194fdaa3ee9091f24c8c76ad9f740a9ddff1a4f08f3d0954
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
      "company_id": 17,
      "company": {
        "id": 17,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-21T15:04:18.414Z"
      },
      "created_at": "2016-10-21T15:04:18.419Z",
      "updated_at": "2016-10-21T15:04:18.419Z",
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-21T15:04:18.435Z"
      },
      "created_at": "2016-10-21T15:04:18.439Z",
      "updated_at": "2016-10-21T15:04:18.439Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48ca456816831760194fdaa3ee9091f24c8c76ad9f740a9ddff1a4f08f3d0954"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 4c76dc7a29903244157742323cc7bf11408b6923e57584dc71d9dbea32ffb983
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
      "id": 15,
      "created_at": "2016-10-21T15:04:46.356Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 52,
      "updated_at": "2016-10-21T15:04:46.468Z",
      "author_id": "873",
      "thread_subject_id": "287",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-21T15:04:46.456Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 53,
      "updated_at": "2016-10-21T15:04:46.471Z",
      "author_id": "876",
      "thread_subject_id": "288",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-21T15:04:46.841Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-21T15:04:46.841Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-21T15:04:47.209Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-21T15:04:47.209Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-21T15:04:47.578Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-21T15:04:47.578Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-21T15:04:47.863Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 129,
      "updated_at": "2016-10-21T15:04:47.863Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-21T15:04:48.157Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 130,
      "updated_at": "2016-10-21T15:04:48.157Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-21T15:04:48.439Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 131,
      "updated_at": "2016-10-21T15:04:48.439Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c76dc7a29903244157742323cc7bf11408b6923e57584dc71d9dbea32ffb983"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer 3e4791b624141b42b5b1c9abb692272e0c2123aff3a872701980a39ba5cc2516
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-21T14:54:46.000Z"}}
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
    "id": 14,
    "created_at": "2016-10-21T15:04:46.149Z",
    "read_at": "2016-10-21T14:54:46.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 51,
    "updated_at": "2016-10-21T15:04:46.206Z",
    "author_id": "868",
    "thread_subject_id": "286",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-10-21T14:54:46.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e4791b624141b42b5b1c9abb692272e0c2123aff3a872701980a39ba5cc2516"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1158598722c720d9155d95ce1b22594d9347e5e543d7f45681626cdbd2caea32
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
      "course_id": 159,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-21T15:04:18.082Z",
      "course_published": true,
      "updated_at": "2016-10-21T15:04:18.074Z"
    },
    {
      "id": 7,
      "course_id": 160,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-21T15:04:18.169Z",
      "course_published": true,
      "updated_at": "2016-10-21T15:04:18.160Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1158598722c720d9155d95ce1b22594d9347e5e543d7f45681626cdbd2caea32"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer bc1e73aa3fed553aa03947c4db735116c3be0e421d540e0e53a5ae6b3ef1c67e
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
    "course_id": 156,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-21T15:04:17.654Z",
    "course_published": true,
    "updated_at": "2016-10-21T15:04:17.644Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc1e73aa3fed553aa03947c4db735116c3be0e421d540e0e53a5ae6b3ef1c67e"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 839e3d7206e272417c27b3341e514569adae617aeb8baae111eb84653397d88d
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
    "id": 8,
    "course_id": 161,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-21T15:04:18.339Z",
    "course_published": true,
    "updated_at": "2016-10-21T15:04:18.328Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 839e3d7206e272417c27b3341e514569adae617aeb8baae111eb84653397d88d"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer fd1102ff97c9f87de5928d597ebb6978da077681a646cdff6c4af40614625900
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
      "votable_id": 108,
      "user_id": 500
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 109,
      "user_id": 500
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 110,
      "user_id": 500
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 111,
      "user_id": 500
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd1102ff97c9f87de5928d597ebb6978da077681a646cdff6c4af40614625900"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/158
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
    "id": 158,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 156,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 158
      },
      {
        "id": 157,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 158
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/158" -X GET \
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
      "id": 156,
      "name": "Operative impactful intranet",
      "name_translations": {
        "en": "Operative impactful intranet"
      }
    },
    {
      "id": 157,
      "name": "Function-based heuristic initiative",
      "name_translations": {
        "en": "Function-based heuristic initiative"
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
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer 35d9835a3414c62e80420cc5fb71f31b6cfa7cfe59cebd05c84567c90b122958
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
    "id": 23,
    "user_id": 416,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-21T15:04:15.498Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35d9835a3414c62e80420cc5fb71f31b6cfa7cfe59cebd05c84567c90b122958"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 543d7c7ed1685adc02d74e896d61198a366c86c071373dc1e9e8f574e7ffa38c
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
    "id": 28,
    "user_id": 441,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-21T15:04:16.976Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 543d7c7ed1685adc02d74e896d61198a366c86c071373dc1e9e8f574e7ffa38c"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/21
Content-Type: application/json
Authorization: Bearer 70e940ddd2ff02f32f189aebc86be65ba8c97cd20d4bbf9d691bd81f8dc10857
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
    "id": 21,
    "user_id": 404,
    "feedbackable_id": 39,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-21T15:04:14.963Z",
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
curl "api.goskive.com/v2/feedbacks/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70e940ddd2ff02f32f189aebc86be65ba8c97cd20d4bbf9d691bd81f8dc10857"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/close
Content-Type: application/json
Authorization: Bearer dc9edc88182b8e460c433a962fcad4965de2d93cdfdf4614efca20ca8fdd2849
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
curl "api.goskive.com/v2/feedbacks/25/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc9edc88182b8e460c433a962fcad4965de2d93cdfdf4614efca20ca8fdd2849"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer c1959a302e6dc0f634d2a80fff20e9ff2e24871e688adc5b0e6c44bc1e95037c
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
curl "api.goskive.com/v2/feedbacks/26/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1959a302e6dc0f634d2a80fff20e9ff2e24871e688adc5b0e6c44bc1e95037c"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/29/fix
Content-Type: application/json
Authorization: Bearer 59dd3c017c8c0654c1922a63bc4018d83debddf38b2063e7debbecde516e81e0
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
curl "api.goskive.com/v2/feedbacks/29/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59dd3c017c8c0654c1922a63bc4018d83debddf38b2063e7debbecde516e81e0"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/22
Content-Type: application/json
Authorization: Bearer ec3443f7abb9f70af2899d00ce0b8f47d4937f6249640d8a9a70713248efbb54
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
    "id": 22,
    "user_id": 409,
    "feedbackable_id": 40,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-21T15:04:15.308Z",
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
curl "api.goskive.com/v2/feedbacks/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec3443f7abb9f70af2899d00ce0b8f47d4937f6249640d8a9a70713248efbb54"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/4
Content-Type: application/json
Authorization: Bearer 3d5f8cf6a5a8f2919e3384b5acebeaab4098f07d2944a1cb346a2e407c17be4e
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d5f8cf6a5a8f2919e3384b5acebeaab4098f07d2944a1cb346a2e407c17be4e"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Content-Type: application/json
Authorization: Bearer 0ed43a82d72df9d5f61b7678ced7115d9030fed6aad1cdd199a474b8eb7fedba
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ed43a82d72df9d5f61b7678ced7115d9030fed6aad1cdd199a474b8eb7fedba"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/7
Content-Type: application/json
Authorization: Bearer 615e12147f68fc6540aa9d91ebe85b40ac65647f627f0daf55cb6ccb61287b87
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/dbf5826bd6b36f570f8dee3fbafb7b74.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161021%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161021T150438Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=b63057fc8680b3b863ee1375a9b9b5380a3c96966919b70adc810855dd97da6e"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 615e12147f68fc6540aa9d91ebe85b40ac65647f627f0daf55cb6ccb61287b87"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/6/preview
Content-Type: application/json
Authorization: Bearer a814274fe5e4877f614d9342f3ae437bc4a5c1e1d8efafbdce8508e1da81988b
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/2fa989a2e4cd0d954522023bd748a732.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161021%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161021T150438Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=e2d5070126e17f5329f1620352aa90d9b1156a6c2191fb09fadedd07e7a0b27f"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/6/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a814274fe5e4877f614d9342f3ae437bc4a5c1e1d8efafbdce8508e1da81988b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer a7916377389edd47cecb4b13b3a2c19e63bc32f32d48aa4528a9820c4fd5ba6b
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
      "id": 785,
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
      "created_at": "2016-10-21T15:04:38.841Z",
      "updated_at": "2016-10-21T15:04:38.841Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-21T15:04:38.921Z",
    "updated_at": "2016-10-21T15:04:38.921Z",
    "course_id": 267,
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7916377389edd47cecb4b13b3a2c19e63bc32f32d48aa4528a9820c4fd5ba6b"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer 986e053ba51996fdde02add047db062e755468b7fcb81ae1432a3c8f17a0cb19
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
      "creator_id": 14,
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "topic_id": 4,
      "discipline_id": 4,
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
      "chapters_updated_at": "2016-10-21T15:03:33.741Z",
      "updated_at": "2016-10-21T15:03:35.495Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 19,
      "id": 5,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-75a90798-cfb6-446f-bd3c-270cb633640d",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-75a90798-cfb6-446f-bd3c-270cb633640d",
      "slug": "mit-the-great-british-bake-off-75a90798-cfb6-446f-bd3c-270cb633640d",
      "university_id": 5,
      "additional_university_ids": [

      ],
      "topic_id": 5,
      "discipline_id": 5,
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
      "chapters_updated_at": "2016-10-21T15:03:33.741Z",
      "updated_at": "2016-10-21T15:03:36.059Z",
      "shortname": "mit-the-great-british-bake-off-75a90798-cfb6-446f-bd3c-270cb633640d"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 986e053ba51996fdde02add047db062e755468b7fcb81ae1432a3c8f17a0cb19"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer bf2192de8c6598d09ff6570b744ec06a9561044731c03d9086a52bd31bafe923
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
	-H "Authorization: Bearer bf2192de8c6598d09ff6570b744ec06a9561044731c03d9086a52bd31bafe923"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/91/comments
Content-Type: application/json
Authorization: Bearer 46660b77aa909bddf4499e9a76e191f964109e798cb8dbf3ca135dcd55fb8e3a
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
    "id": 56,
    "author_id": 935,
    "reply_to_id": null,
    "created_at": "2016-10-21T15:04:52.663Z",
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
curl "api.goskive.com/v2/flashcards/91/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46660b77aa909bddf4499e9a76e191f964109e798cb8dbf3ca135dcd55fb8e3a"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/92/comments
Content-Type: application/json
Authorization: Bearer a086feda9e04322b65316058fa3c43902ce16ed3cb017342ebe0ddd9858a349f
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
    "id": 57,
    "author_id": 938,
    "reply_to_id": null,
    "created_at": "2016-10-21T15:04:52.995Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 938,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:52.992Z",
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
curl "api.goskive.com/v2/flashcards/92/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a086feda9e04322b65316058fa3c43902ce16ed3cb017342ebe0ddd9858a349f"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/88/comments
Content-Type: application/json
Authorization: Bearer 2ebcd00a2d8fc1a1e3f5ec742d004f6606af9e9999274d6ebd7788b191c38f35
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
      "id": 54,
      "author_id": 927,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:52.074Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 928,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:04:52.092Z",
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
curl "api.goskive.com/v2/flashcards/88/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ebcd00a2d8fc1a1e3f5ec742d004f6606af9e9999274d6ebd7788b191c38f35"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/90/comments
Content-Type: application/json
Authorization: Bearer 5d0d62b31bfc034b06ee5fe870d77b597a22c8b87bab36db46b33a13f981186e
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
curl "api.goskive.com/v2/flashcards/90/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d0d62b31bfc034b06ee5fe870d77b597a22c8b87bab36db46b33a13f981186e"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/81/feedbacks
Content-Type: application/json
Authorization: Bearer baec249ff620caae6b03eee2fe39baa29e932d4678840e93ffd66a901d697114
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
    "user_id": 815,
    "feedbackable_id": 81,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-21T15:04:42.649Z",
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
curl "api.goskive.com/v2/flashcards/81/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer baec249ff620caae6b03eee2fe39baa29e932d4678840e93ffd66a901d697114"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/83/feedbacks
Content-Type: application/json
Authorization: Bearer 830cdf8e624a7a9c989b75301cca1d1af39dbc67b108f9200003df3ea950a579
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
      "id": 41,
      "user_id": 825,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:43.130Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 824,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:43.118Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 830cdf8e624a7a9c989b75301cca1d1af39dbc67b108f9200003df3ea950a579"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/94/votes
Content-Type: application/json
Authorization: Bearer 2640011e9248e2feb1e26b989deb2e7b07ea117e3ce0009c54094dd97b0eeb73
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 966
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 965
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 964
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/94/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2640011e9248e2feb1e26b989deb2e7b07ea117e3ce0009c54094dd97b0eeb73"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/73/republish
Content-Type: application/json
Authorization: Bearer 129c5d0979a3637d3086241bc921984890d4656e67ebe154764ac5eacc388cca
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
curl "api.goskive.com/v2/flashcards/73/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 129c5d0979a3637d3086241bc921984890d4656e67ebe154764ac5eacc388cca"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/bookmark
Content-Type: application/json
Authorization: Bearer ce9d8a328203025bdb5b26f3833990be29b1f7fe26bdb7953f0b1b0d1716dc21
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce9d8a328203025bdb5b26f3833990be29b1f7fe26bdb7953f0b1b0d1716dc21"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/67
Content-Type: application/json
Authorization: Bearer 431e0d4d364b6b4e41aebf8b620272a24c0df1618a6ade48276ed40a7164c5e6
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/67" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 431e0d4d364b6b4e41aebf8b620272a24c0df1618a6ade48276ed40a7164c5e6"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/downvote
Content-Type: application/json
Authorization: Bearer 7ba5174f8eb1bc2512c8487bd6ed5b2cf0531c8918949dadbab8beced053002d
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ba5174f8eb1bc2512c8487bd6ed5b2cf0531c8918949dadbab8beced053002d"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/68
Content-Type: application/json
Authorization: Bearer be43ab1a25698585459e8098272c4f96dc7d7e844040e48f3d5cf3e876490393
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 635,
    "chapter_id": 150,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:30.166Z",
    "created_at": "2016-10-21T15:04:30.166Z",
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
curl "api.goskive.com/v2/flashcards/68" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be43ab1a25698585459e8098272c4f96dc7d7e844040e48f3d5cf3e876490393"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/51/report
Content-Type: application/json
Authorization: Bearer edcc3ad8bc458d03907219fea04ba09f2ae6c0136af41f232beec4afdc138903
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/51/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edcc3ad8bc458d03907219fea04ba09f2ae6c0136af41f232beec4afdc138903"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/71/bookmark
Content-Type: application/json
Authorization: Bearer a220d70d953d1086defe9c977d18a8e26d828af95a274e04cc88806aa378c264
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
	-H "Authorization: Bearer a220d70d953d1086defe9c977d18a8e26d828af95a274e04cc88806aa378c264"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/70/upvote
Content-Type: application/json
Authorization: Bearer fc32be1373f4d00c9ea715b41c45ab4a766dfe7cd2e7d2fcaec0c029dbb7e1e3
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/70/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc32be1373f4d00c9ea715b41c45ab4a766dfe7cd2e7d2fcaec0c029dbb7e1e3"
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
    "key": "cache/40ffc0390e31c825b630c54bc1454611.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMVQxNjowNDo1NFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzQwZmZjMDM5MGUzMWM4MjViNjMwYzU0YmMxNDU0NjExLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyMS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjFUMTUwNDU0WiJ9XX0=",
    "x-amz-credential": "FAKE/20161021/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161021T150454Z",
    "x-amz-signature": "529a4bdc837e012e669a598c160a593f81d0df15976f4e0c85ad824c5092538f"
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
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 5baacaf4323e135a74153c92fa084a8ff386bb8d7e3ab3d826b6d95dd45f13f6
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
curl "api.goskive.com/v2/me/jobs/7/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5baacaf4323e135a74153c92fa084a8ff386bb8d7e3ab3d826b6d95dd45f13f6"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 3ba0296f955e9293416888758cebb9e01656682196f174f5e1b54dd30bee3e1f
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
	-H "Authorization: Bearer 3ba0296f955e9293416888758cebb9e01656682196f174f5e1b54dd30bee3e1f"
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
{"password":{"reset_password_token":"X1PYygZhPRsyTv3SFFsV","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 918,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-21T15:04:50.299Z",
  "updated_at": "2016-10-21T15:04:50.483Z",
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
  "audit_id": 4864
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"X1PYygZhPRsyTv3SFFsV","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer cf0dd2c1ea10b99bc340e19d78c86a77d28653b3972c5fff80af488055d0314e
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
    "author_id": 43,
    "reply_to_id": null,
    "created_at": "2016-10-21T15:03:38.234Z",
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
curl "api.goskive.com/v2/questions/11/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf0dd2c1ea10b99bc340e19d78c86a77d28653b3972c5fff80af488055d0314e"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/13/comments
Content-Type: application/json
Authorization: Bearer ff7ab9802707614f807047a434a7c1ca9884c5bac6c2524831d6ce691a594a0b
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
    "author_id": 49,
    "reply_to_id": null,
    "created_at": "2016-10-21T15:03:39.469Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 49,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:03:39.465Z",
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
curl "api.goskive.com/v2/questions/13/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff7ab9802707614f807047a434a7c1ca9884c5bac6c2524831d6ce691a594a0b"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/10/comments
Content-Type: application/json
Authorization: Bearer 9a7ee65fa4311f40416cb76e77454871d680a6f952f419cdc126584281835c7a
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
      "author_id": 41,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:03:37.826Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 42,
      "reply_to_id": null,
      "created_at": "2016-10-21T15:03:37.862Z",
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
curl "api.goskive.com/v2/questions/10/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a7ee65fa4311f40416cb76e77454871d680a6f952f419cdc126584281835c7a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer 4983494c0c51a41aea3b60f612e9a487cd1c17f19f705a6ce374f2170d643da4
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
curl "api.goskive.com/v2/questions/12/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4983494c0c51a41aea3b60f612e9a487cd1c17f19f705a6ce374f2170d643da4"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/100/feedbacks
Content-Type: application/json
Authorization: Bearer bbf84f42dfd8eff412152ea5a6d80c8818ba56197d741f75f586c43dd2eafa4b
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
    "user_id": 463,
    "feedbackable_id": 100,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-21T15:04:19.125Z",
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
curl "api.goskive.com/v2/questions/100/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbf84f42dfd8eff412152ea5a6d80c8818ba56197d741f75f586c43dd2eafa4b"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/106/feedbacks
Content-Type: application/json
Authorization: Bearer f1e6f74c6e3365aa5f5443681d53e7e49a8b78112e656892ce1cb7cae97dfbb7
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
      "id": 37,
      "user_id": 495,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:21.539Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 494,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-21T15:04:21.528Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/106/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1e6f74c6e3365aa5f5443681d53e7e49a8b78112e656892ce1cb7cae97dfbb7"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/54/votes
Content-Type: application/json
Authorization: Bearer 295f02fc7b5838c2a786be1cf3211a4299610d507dbb953cdf712e1b63706657
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
      "votable_id": 54,
      "user_id": 213
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 212
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 54,
      "user_id": 211
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/54/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 295f02fc7b5838c2a786be1cf3211a4299610d507dbb953cdf712e1b63706657"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/76/republish
Content-Type: application/json
Authorization: Bearer 3c4b37e0046f236e9aec2be5436d6430a13c6cdb1027155e2fea4cd054802bcb
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
curl "api.goskive.com/v2/questions/76/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c4b37e0046f236e9aec2be5436d6430a13c6cdb1027155e2fea4cd054802bcb"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/71/bookmark
Content-Type: application/json
Authorization: Bearer dc81c897b88b499764d6cefc667220ce20a4f08c1db0d219fac88a2c1d0063fe
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
	-H "Authorization: Bearer dc81c897b88b499764d6cefc667220ce20a4f08c1db0d219fac88a2c1d0063fe"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/78
Content-Type: application/json
Authorization: Bearer 2179a40fce87d9df0674006f1f94318c006b0c35c3645fa7961153ddc8cf96f7
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/78" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2179a40fce87d9df0674006f1f94318c006b0c35c3645fa7961153ddc8cf96f7"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/72/downvote
Content-Type: application/json
Authorization: Bearer 630b175bfd304c21f4ef47bc580595e4c65d01c6b244130c0dbc59be9788107c
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/72/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 630b175bfd304c21f4ef47bc580595e4c65d01c6b244130c0dbc59be9788107c"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/73
Content-Type: application/json
Authorization: Bearer 4ac6b1d3023250f460bce933f167af76923b8c0adae0376f56b0db3f8e3e091a
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
    "id": 73,
    "obfuscated_id": "LJvjpBojvP0",
    "author_id": 289,
    "chapter_id": 61,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:04.942Z",
    "created_at": "2016-10-21T15:04:04.824Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/73" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ac6b1d3023250f460bce933f167af76923b8c0adae0376f56b0db3f8e3e091a"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/77/report
Content-Type: application/json
Authorization: Bearer 87dbe48f8924fdf821f9e74e6b01bc71b47230fcb39b0634347c486d032542ca
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/77/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87dbe48f8924fdf821f9e74e6b01bc71b47230fcb39b0634347c486d032542ca"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/79/bookmark
Content-Type: application/json
Authorization: Bearer 2cadcf1c9bb3caff3140372c540382c34eb0f202708192364f9e1237f78b09e7
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/79/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cadcf1c9bb3caff3140372c540382c34eb0f202708192364f9e1237f78b09e7"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/74
Content-Type: application/json
Authorization: Bearer 07ae0ebd4535946abf7763d4d050cf64ac9c2386d879e04cd295d888b428fba1
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":74,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-21T15:04:05.172Z","updated_at":"2016-10-21T15:04:05.291Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":62,"author_id":292,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 292,
    "chapter_id": 62,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-21T15:04:05.402Z",
    "created_at": "2016-10-21T15:04:05.172Z",
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
    "question": "{\"id\"=>74, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-21T15:04:05.172Z\", \"updated_at\"=>\"2016-10-21T15:04:05.291Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>62, \"author_id\"=>292, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 147,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 148,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 149,
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
curl "api.goskive.com/v2/questions/74" -d '{"question":{"question":{"id":74,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-21T15:04:05.172Z","updated_at":"2016-10-21T15:04:05.291Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":62,"author_id":292,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07ae0ebd4535946abf7763d4d050cf64ac9c2386d879e04cd295d888b428fba1"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/80/upvote
Content-Type: application/json
Authorization: Bearer 2439e3186814287d7c639fcfd627cf896288028b80bad2b71fe8a65ab0a96db8
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/80/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2439e3186814287d7c639fcfd627cf896288028b80bad2b71fe8a65ab0a96db8"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 41e3eca8351037000a97dcee58cb5662fda8df5cdef852fb681a7f0a608d5fbe
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
      "creator_id": 200,
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 67,
      "additional_university_ids": [

      ],
      "topic_id": 90,
      "discipline_id": 90,
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
      "updated_at": "2016-10-21T15:03:56.686Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41e3eca8351037000a97dcee58cb5662fda8df5cdef852fb681a7f0a608d5fbe"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 9bdf32de8f039162974f220e6b4e652e8e4b1c1d2e82e44ab555d34715b81a04
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
      "id": 70,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-52",
      "html_url": "https://goskive.com/university/uni-52",
      "slug": "uni-52",
      "name": "National School of Pizza",
      "short_name": "Uni 52",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe68b2e1c81a7d5c35fd1107da0e373597f006d5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e85940cf8561c3a456df79e408c963432af4ba51.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-21T15:03:57.007Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-51",
      "html_url": "https://goskive.com/university/uni-51",
      "slug": "uni-51",
      "name": "National School of Pastry",
      "short_name": "Uni 51",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/708a005b52f81ade5d5c9481071b7a8cff7c4cd9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/822e4ae5676b385680a75a35bb9799eaca85f11e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-21T15:03:56.989Z",
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
	-H "Authorization: Bearer 9bdf32de8f039162974f220e6b4e652e8e4b1c1d2e82e44ab555d34715b81a04"
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
      "id": 222,
      "name": "Fundamental object-oriented hub",
      "name_translations": {
        "en": "Fundamental object-oriented hub"
      },
      "discipline_id": 223
    },
    {
      "id": 223,
      "name": "Secured logistical policy",
      "name_translations": {
        "en": "Secured logistical policy"
      },
      "discipline_id": 224
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
GET /v2/topics/221
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
    "id": 221,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 222
  }
}
```



```shell
curl "api.goskive.com/v2/topics/221" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 3e3aa7f885d026b44427eba408279b57406c57f7ae507205e5ac1182b0d35f52
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
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-88",
      "html_url": "https://goskive.com/university/uni-88",
      "slug": "uni-88",
      "name": "University 49",
      "short_name": "Uni 88",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6a9fa24a498e1c0325fb6c3481402b3b7b1edc26.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a95ae5e7e91665458aaf1066d893915854be5394.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-21T15:04:08.565Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-89",
      "html_url": "https://goskive.com/university/uni-89",
      "slug": "uni-89",
      "name": "University 50",
      "short_name": "Uni 89",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4bb8ec2c77619620225b3baa5e95c92743b5375d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2d8a95d4c289fcc26bc01926bad682d4733c5159.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-21T15:04:08.583Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-90",
      "html_url": "https://goskive.com/university/uni-90",
      "slug": "uni-90",
      "name": "University 51",
      "short_name": "Uni 90",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/82018de485d26c9bc27540446774b49169a40672.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/185a914e401fa48a03ae327e11f997764d72b2a1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-21T15:04:08.601Z",
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
	-H "Authorization: Bearer 3e3aa7f885d026b44427eba408279b57406c57f7ae507205e5ac1182b0d35f52"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer c2a68cc996c867bcbcf89957bf5ab44c271df85b4065a722750599c246e89b00
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
    "id": 107,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/47501c30005ace1e8cf5ce8d311d35f8e8031d1e.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8701d988977fa68699c888ee61dc7050e74864f5.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-21T15:04:08.467Z",
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
	-H "Authorization: Bearer c2a68cc996c867bcbcf89957bf5ab44c271df85b4065a722750599c246e89b00"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 177a9e1385a4c19096aadad6580e434094373e0b49cbd8fa624a1afff161b95f
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":38,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 111,
    "id": 38,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 38,
    "additional_university_ids": [

    ],
    "topic_id": 38,
    "discipline_id": 38,
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
    "chapters_updated_at": "2016-10-21T15:03:48.761Z",
    "updated_at": "2016-10-21T15:03:48.897Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 22,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-21T15:03:48.855Z",
        "course_id": 38,
        "author_id": 111,
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
        "id": 23,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-21T15:03:48.871Z",
        "course_id": 38,
        "author_id": 111,
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
        "id": 24,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-21T15:03:48.888Z",
        "course_id": 38,
        "author_id": 111,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":38,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 177a9e1385a4c19096aadad6580e434094373e0b49cbd8fa624a1afff161b95f"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a37fa8e39817b451f1b52cd0be327617d24d75f8254fb216bbeca3b74efa47ba
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":39,"published":false}}
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
    "creator_id": 112,
    "id": 39,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 39,
    "additional_university_ids": [

    ],
    "topic_id": 39,
    "discipline_id": 39,
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
    "updated_at": "2016-10-21T15:03:49.046Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":39,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a37fa8e39817b451f1b52cd0be327617d24d75f8254fb216bbeca3b74efa47ba"
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
      "creator_id": 129,
      "id": 55,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-26",
      "html_url": "https://goskive.com/course/fu-course-26",
      "slug": "fu-course-26",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "topic_id": 55,
      "discipline_id": 55,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 26",
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
      "updated_at": "2016-10-21T15:03:50.586Z",
      "shortname": "fu-course-26"
    },
    {
      "creator_id": 129,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "topic_id": 56,
      "discipline_id": 56,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
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
      "chapters_updated_at": "2016-10-21T15:03:50.871Z",
      "updated_at": "2016-10-21T15:03:50.878Z",
      "shortname": "fu-course-27"
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
Authorization: Bearer 52617839c47a0a3bc8d921f055828b5f0cf61dd972b1fe1fb60922c5896bd1b5
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
      "creator_id": 136,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-34",
      "html_url": "https://goskive.com/course/fu-course-34",
      "slug": "fu-course-34",
      "university_id": 49,
      "additional_university_ids": [

      ],
      "topic_id": 63,
      "discipline_id": 63,
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
      "updated_at": "2016-10-21T15:03:51.328Z",
      "shortname": "fu-course-34"
    },
    {
      "creator_id": 136,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-35",
      "html_url": "https://goskive.com/course/fu-course-35",
      "slug": "fu-course-35",
      "university_id": 49,
      "additional_university_ids": [

      ],
      "topic_id": 64,
      "discipline_id": 64,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 35",
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
      "chapters_updated_at": "2016-10-21T15:03:51.626Z",
      "updated_at": "2016-10-21T15:03:51.633Z",
      "shortname": "fu-course-35"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52617839c47a0a3bc8d921f055828b5f0cf61dd972b1fe1fb60922c5896bd1b5"
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
      "creator_id": 134,
      "id": 59,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-30",
      "html_url": "https://goskive.com/course/fu-course-30",
      "slug": "fu-course-30",
      "university_id": 47,
      "additional_university_ids": [

      ],
      "topic_id": 59,
      "discipline_id": 59,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 30",
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
      "updated_at": "2016-10-21T15:03:51.068Z",
      "shortname": "fu-course-30"
    },
    {
      "creator_id": 134,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 47,
      "additional_university_ids": [

      ],
      "topic_id": 60,
      "discipline_id": 60,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 31",
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
      "updated_at": "2016-10-21T15:03:51.110Z",
      "shortname": "fu-course-31"
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
Authorization: Bearer 3c0e0ead49cf06bb561a8e95f373c2855f6ca4807d0f43c9c3ab0a1ffdad105a
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
      "creator_id": 143,
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-38",
      "html_url": "https://goskive.com/course/fu-course-38",
      "slug": "fu-course-38",
      "university_id": 51,
      "additional_university_ids": [

      ],
      "topic_id": 67,
      "discipline_id": 67,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 38",
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
      "updated_at": "2016-10-21T15:03:51.919Z",
      "shortname": "fu-course-38"
    },
    {
      "creator_id": 143,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-39",
      "html_url": "https://goskive.com/course/fu-course-39",
      "slug": "fu-course-39",
      "university_id": 51,
      "additional_university_ids": [

      ],
      "topic_id": 68,
      "discipline_id": 68,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 39",
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
      "updated_at": "2016-10-21T15:03:51.959Z",
      "shortname": "fu-course-39"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c0e0ead49cf06bb561a8e95f373c2855f6ca4807d0f43c9c3ab0a1ffdad105a"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 2388df5f00fa214f9f01cca32281fc6ddfec27cde0e3b092ee9c505a8acf3dc4
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
  "id": 672,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-21T15:04:32.510Z",
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
	-H "Authorization: Bearer 2388df5f00fa214f9f01cca32281fc6ddfec27cde0e3b092ee9c505a8acf3dc4"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/956
Content-Type: application/json
Authorization: Bearer 3a06a21a01242544e8ebd301b6f6f6b1f5bc87444d726a1b3f4a3d70ccfda42d
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
    "id": 956,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 291,
    "fields_of_study": [
      317,
      318
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-21T15:04:54.606Z",
    "updated_at": "2016-10-21T15:04:54.606Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/956" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a06a21a01242544e8ebd301b6f6f6b1f5bc87444d726a1b3f4a3d70ccfda42d"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/954
Content-Type: application/json
Authorization: Bearer ee48a1a18995edeb5c74ab0d9e5154f8d594f6db6ae03c1f292bb4ffd5e2647f
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
    "id": 954,
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
    "created_at": "2016-10-21T15:04:54.454Z",
    "updated_at": "2016-10-21T15:04:54.454Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/954" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee48a1a18995edeb5c74ab0d9e5154f8d594f6db6ae03c1f292bb4ffd5e2647f"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/15
Content-Type: application/json
Authorization: Bearer 713a777b5c7c3e9c49501b86dd525c6c2c7645f7205d559b5b32e3e12f385ff9
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
	-H "Authorization: Bearer 713a777b5c7c3e9c49501b86dd525c6c2c7645f7205d559b5b32e3e12f385ff9"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer 57a63e82083bd617de0fe7d3dbb8857081baee6040e7d78c4f725bca2b881445
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
    "votable_id": 124,
    "user_id": 852
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57a63e82083bd617de0fe7d3dbb8857081baee6040e7d78c4f725bca2b881445"
```
