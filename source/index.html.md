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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e660d3a4aca446b6fcd00bd841b4e557a7df843c952d77f14d8d020f43198a3d","client_secret":"92f63dc993cf05732dd6c8bd6540c2d4f656b0ab1c0524126d99d142705b5de2"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e660d3a4aca446b6fcd00bd841b4e557a7df843c952d77f14d8d020f43198a3d","client_secret":"92f63dc993cf05732dd6c8bd6540c2d4f656b0ab1c0524126d99d142705b5de2"}' -X POST \
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
Authorization: Basic NjI5MWMyMjIxMTYxNmQ1ODE0MTg2NDcyZWJlYzRmMTEzOTg3ZTBkY2E5ODRh
Y2M3ZDQ2MmQxNjJlMmM0Mzc1ODphNDA1ZDg2NDM2N2JlNWEyNWM0NzBlYjdl
MDY5YmI5MWY5OTIwNjExMTZiYmY2ZjBkYmIyMDk3Mzc3OGI2NDM0

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
	-u 6291c22211616d5814186472ebec4f113987e0dca984acc7d462d162e2c43758:a405d864367be5a25c470eb7e069bb91f992061116bbf6f0dbb20973778b6434
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
{"grant_type":"client_credentials","client_id":"c856edc20267876222feac82a8cf6e09ff75fe06bf58f20807fc73ccc130a722","client_secret":"e7ea8f137f23c4fa9201d9353c51519b53bdb0a298601088219213049ee027d7"}
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
  "access_token": "0269b56036403d8275c70288efe3d4ee3d846225547683d0a907a2d6a9157f9f",
  "token_type": "bearer",
  "created_at": 1476382897
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"c856edc20267876222feac82a8cf6e09ff75fe06bf58f20807fc73ccc130a722","client_secret":"e7ea8f137f23c4fa9201d9353c51519b53bdb0a298601088219213049ee027d7"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9ebbc557cb3bd60a65ee26d1df8af7d3cd206437a1753aeb538230ebaf2031ea","client_secret":"16dcb2b6dd62f05b58b7877023f15a9a5af7177ac02ffdee160e6181b1dee7b4"}
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
  "access_token": "0c416ec0ed8aeb5b130bcb8c71bb29ffedd04b2c3d614cf2651c2a51ddb7dd8d",
  "token_type": "bearer",
  "created_at": 1476382897
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9ebbc557cb3bd60a65ee26d1df8af7d3cd206437a1753aeb538230ebaf2031ea","client_secret":"16dcb2b6dd62f05b58b7877023f15a9a5af7177ac02ffdee160e6181b1dee7b4"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MmM5N2Y4NjBhM2VjMzdjZmY0ZDc3NTgyZDYwMjhlZTg4MzNjOWM3OWQyMGI1
NGQ2ZGE5NzFmZThlNjA4ZGM1Njo0NzllMDA1ODdmNGE1M2I2YjI1NDRjMDJj
ZWI0Njk5YWYzNzhiMDBiY2IzNjMwZjQ2OGU5ZmZhNThjN2FhNWNm

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
  "access_token": "04c5e2930a115ef746c12aad948350db8bbbff5f91a544d66a52a6d151dc2b72",
  "token_type": "bearer",
  "created_at": 1476382897
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 2c97f860a3ec37cff4d77582d6028ee8833c9c79d20b54d6da971fe8e608dc56:479e00587f4a53b6b2544c02ceb4699af378b00bcb3630f468e9ffa58c7aa5cf
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
Authorization: Bearer f9956fedbba27de385b9dff2bf8213023eeb53ffc48b60888be612601caf8fd7
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
    "company_id": 39,
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
	-H "Authorization: Bearer f9956fedbba27de385b9dff2bf8213023eeb53ffc48b60888be612601caf8fd7"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/57/flashcards
Content-Type: application/json
Authorization: Bearer 03bcd63de408f1429240b76f339eadad8fa29e688b709808d4fbbbb0ef20aab6
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":57,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 449,
    "chapter_id": 57,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:38.460Z",
    "created_at": "2016-10-13T18:21:38.460Z",
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
curl "api.goskive.com/v2/chapters/57/flashcards" -d '{"flashcard":{"chapter_id":57,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03bcd63de408f1429240b76f339eadad8fa29e688b709808d4fbbbb0ef20aab6"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/59/flashcards
Content-Type: application/json
Authorization: Bearer 1f3282df6c6f13ac856078744de3fb6fb37eeeb5b1dff19a06f6133fb10cea6c
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 453,
      "chapter_id": 59,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:38.776Z",
      "created_at": "2016-10-13T18:21:38.776Z",
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
      "author_id": 453,
      "chapter_id": 59,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:38.816Z",
      "created_at": "2016-10-13T18:21:38.816Z",
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 453,
      "chapter_id": 59,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:38.856Z",
      "created_at": "2016-10-13T18:21:38.856Z",
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
curl "api.goskive.com/v2/chapters/59/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f3282df6c6f13ac856078744de3fb6fb37eeeb5b1dff19a06f6133fb10cea6c"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/105/questions
Content-Type: application/json
Authorization: Bearer 27315a415ae35c4a2a5a2d4a87d046174aaba52cb4b109de5e1f9265fc3bd2b7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 78,
    "obfuscated_id": "-wsYNe2w7uo",
    "author_id": 623,
    "chapter_id": 105,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:55.313Z",
    "created_at": "2016-10-13T18:21:55.313Z",
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
        "id": 157,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 158,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 159,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 160,
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
curl "api.goskive.com/v2/chapters/105/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27315a415ae35c4a2a5a2d4a87d046174aaba52cb4b109de5e1f9265fc3bd2b7"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/103/questions
Content-Type: application/json
Authorization: Bearer bd53e02d4eeaba033e781a2e8b555c8b100cc73eaabd904a66425a13e59156e7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 76,
    "obfuscated_id": "oK0h_-4yfUk",
    "author_id": 617,
    "chapter_id": 103,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:54.502Z",
    "created_at": "2016-10-13T18:21:54.502Z",
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
        "id": 152,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 153,
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
curl "api.goskive.com/v2/chapters/103/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd53e02d4eeaba033e781a2e8b555c8b100cc73eaabd904a66425a13e59156e7"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/106/questions
Content-Type: application/json
Authorization: Bearer 2e0b557497d9fb692615307f429fad9666f70b71e56d8caa88f19ea023f82b81
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":106,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 626,
    "chapter_id": 106,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:55.842Z",
    "created_at": "2016-10-13T18:21:55.842Z",
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
        "id": 161,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 162,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/106/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":106,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e0b557497d9fb692615307f429fad9666f70b71e56d8caa88f19ea023f82b81"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/104/questions
Content-Type: application/json
Authorization: Bearer f1d1dcdf5bda9851f6f3ee66dea23d9d42c0d055a3231bfeb6b7ad75c6b30e38
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":104,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 620,
    "chapter_id": 104,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:54.866Z",
    "created_at": "2016-10-13T18:21:54.866Z",
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
        "id": 154,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 155,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 156,
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
curl "api.goskive.com/v2/chapters/104/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":104,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1d1dcdf5bda9851f6f3ee66dea23d9d42c0d055a3231bfeb6b7ad75c6b30e38"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/102/questions
Content-Type: application/json
Authorization: Bearer 97cc15d01e9734658f9bf97d46acef17f7b3f881421fd68a97216fd50d5cde86
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 611,
      "chapter_id": 102,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:53.808Z",
      "created_at": "2016-10-13T18:21:53.682Z",
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
          "id": 146,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 147,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 612,
      "chapter_id": 102,
      "position": 65,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:54.015Z",
      "created_at": "2016-10-13T18:21:53.887Z",
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
          "id": 148,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 149,
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
      "author_id": 613,
      "chapter_id": 102,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T18:21:54.219Z",
      "created_at": "2016-10-13T18:21:54.093Z",
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
          "id": 150,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 151,
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
curl "api.goskive.com/v2/chapters/102/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97cc15d01e9734658f9bf97d46acef17f7b3f881421fd68a97216fd50d5cde86"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/192
Content-Type: application/json
Authorization: Bearer aa04a33bd578bf83e72bb0547c5e11e73c2c803698e3efcd851c725227da4135
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
curl "api.goskive.com/v2/chapters/192" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa04a33bd578bf83e72bb0547c5e11e73c2c803698e3efcd851c725227da4135"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/195
Content-Type: application/json
Authorization: Bearer b622feadcaf722d879b40f922a82e9715123dad88eebb6f5a8c1355003e9b4fd
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
curl "api.goskive.com/v2/chapters/195" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b622feadcaf722d879b40f922a82e9715123dad88eebb6f5a8c1355003e9b4fd"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 8db9989eec220aab2f1e530159161cbf9cd8d47e13740d5d0c0d305a91187d97
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
curl "api.goskive.com/v2/chapters/189" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8db9989eec220aab2f1e530159161cbf9cd8d47e13740d5d0c0d305a91187d97"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/194
Content-Type: application/json
Authorization: Bearer d9f2430e9a8a0037a3531dea494516936d0049a97ded702089ef03b91b073a15
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/194" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9f2430e9a8a0037a3531dea494516936d0049a97ded702089ef03b91b073a15"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 95a8060b3a217aea756c4a89e71e93113c150bf67202a8e2b98e528e6648bc40
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
    "id": 190,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T18:22:25.308Z",
    "course_id": 296,
    "author_id": 928,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-13T18:22:24.689Z",
    "questions_updated_at": "2016-10-13T18:22:24.689Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 932,
        "chapter_id": 190,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.290Z",
        "created_at": "2016-10-13T18:22:25.290Z",
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
        "id": 130,
        "obfuscated_id": "N-qIf0IsvWM",
        "author_id": 930,
        "chapter_id": 190,
        "position": 117,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:25.168Z",
        "created_at": "2016-10-13T18:22:25.011Z",
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
            "id": 263,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 264,
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
curl "api.goskive.com/v2/chapters/190" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95a8060b3a217aea756c4a89e71e93113c150bf67202a8e2b98e528e6648bc40"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/188
Content-Type: application/json
Authorization: Bearer c87d68bec0f825a72f1f2d0237388439d3c02fa042c0362fcc7fb6aaf76a92e6
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
    "id": 188,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T18:22:24.505Z",
    "course_id": 294,
    "author_id": 923,
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
curl "api.goskive.com/v2/chapters/188" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c87d68bec0f825a72f1f2d0237388439d3c02fa042c0362fcc7fb6aaf76a92e6"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/52/replies
Content-Type: application/json
Authorization: Bearer e6e13cefe83cb70b7b3976a1c100f83c1b6f1ead9d64427cd8704576ca15d082
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
    "id": 53,
    "author_id": 372,
    "reply_to_id": 52,
    "created_at": "2016-10-13T18:21:31.665Z",
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
curl "api.goskive.com/v2/comments/52/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6e13cefe83cb70b7b3976a1c100f83c1b6f1ead9d64427cd8704576ca15d082"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer 2f010d1cf4ede6b80136855c972eeb9e43e668a3d8d66b60d9eda86f65493de4
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
curl "api.goskive.com/v2/comments/51/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f010d1cf4ede6b80136855c972eeb9e43e668a3d8d66b60d9eda86f65493de4"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer c563af86be2c2c7b54b389f0b0086134dfb33112072c7c5ca789f57e4f5d6c69
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
curl "api.goskive.com/v2/comments/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c563af86be2c2c7b54b389f0b0086134dfb33112072c7c5ca789f57e4f5d6c69"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/10/republish
Content-Type: application/json
Authorization: Bearer 7f6f303339a7344e3e76a09761cc18cd8f9f466c6500cef3936551e3df901142
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
curl "api.goskive.com/v2/comments/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f6f303339a7344e3e76a09761cc18cd8f9f466c6500cef3936551e3df901142"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer b88335aa7a498b6307a77924f2a9bfa6b61ff7057a10cb159f51bfc416a8a53e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b88335aa7a498b6307a77924f2a9bfa6b61ff7057a10cb159f51bfc416a8a53e"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/9/report
Content-Type: application/json
Authorization: Bearer 71675bb14fe6bada52e2c2674badc018749445d6c9cabebf493abc5b227b10ce
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71675bb14fe6bada52e2c2674badc018749445d6c9cabebf493abc5b227b10ce"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/38
Content-Type: application/json
Authorization: Bearer 2d98779618b6b19d918b6a1ec5f54f4dc13c5e1561c78c82d60357c63a742975
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
    "id": 38,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-13T18:21:50.142Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d98779618b6b19d918b6a1ec5f54f4dc13c5e1561c78c82d60357c63a742975"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer ef926b4c8fa30ad61cebef40d3b66cc370719f815a03b8f796824e50a35b8fb2
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
      "id": 35,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T18:21:50.074Z"
    },
    {
      "id": 36,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T18:21:50.080Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T18:21:50.084Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef926b4c8fa30ad61cebef40d3b66cc370719f815a03b8f796824e50a35b8fb2"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 605e1f53349da0f61dd36e9f8d13938fb88d63ee85d86368a93ec579ba7b90e6
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
curl "api.goskive.com/v2/companies/26/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 605e1f53349da0f61dd36e9f8d13938fb88d63ee85d86368a93ec579ba7b90e6"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/24/company_profiles
Content-Type: application/json
Authorization: Bearer 9bbd6b6cbd61624dce216388c5a3c8800038f94413309c00158442786f51590b
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
curl "api.goskive.com/v2/companies/24/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bbd6b6cbd61624dce216388c5a3c8800038f94413309c00158442786f51590b"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 2cd4fd774502b6295146269d2f996e4252f76013d022b55d4f68b5f3fe4760cc
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
      "company_id": 15,
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
	-H "Authorization: Bearer 2cd4fd774502b6295146269d2f996e4252f76013d022b55d4f68b5f3fe4760cc"
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
Authorization: Bearer 3c8fdb8f7965cedabc641b7e15099db9ad4d5f33ef042e8e794f4b7907064bb1
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
	-H "Authorization: Bearer 3c8fdb8f7965cedabc641b7e15099db9ad4d5f33ef042e8e794f4b7907064bb1"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d89dd88e30838568bca5d8410a919c43accf285a4d0772dc26aaa44d0ce8cc4c
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
    "id": 131,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T18:22:00.390Z",
    "course_id": 227,
    "author_id": 688,
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
	-H "Authorization: Bearer d89dd88e30838568bca5d8410a919c43accf285a4d0772dc26aaa44d0ce8cc4c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4bfef6bba15829fa9a9c5e92ed14dc8c73d836c44dc2397388b2798269d83257
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
      "id": 119,
      "title": "Clever Chapter Title 107",
      "position": 1,
      "updated_at": "2016-10-13T18:21:58.709Z",
      "course_id": 220,
      "author_id": 661,
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
      "position": 2,
      "updated_at": "2016-10-13T18:21:58.736Z",
      "course_id": 220,
      "author_id": 662,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 121,
      "title": "Clever Chapter Title 109",
      "position": 3,
      "updated_at": "2016-10-13T18:21:59.014Z",
      "course_id": 220,
      "author_id": 663,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T18:21:58.626Z",
      "questions_updated_at": "2016-10-13T18:21:58.626Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4bfef6bba15829fa9a9c5e92ed14dc8c73d836c44dc2397388b2798269d83257"
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
      "id": 125,
      "title": "Clever Chapter Title 113",
      "position": 1,
      "updated_at": "2016-10-13T18:21:59.534Z",
      "course_id": 223,
      "author_id": 675,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 126,
      "title": "Clever Chapter Title 114",
      "position": 2,
      "updated_at": "2016-10-13T18:21:59.561Z",
      "course_id": 223,
      "author_id": 676,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 127,
      "title": "Clever Chapter Title 115",
      "position": 3,
      "updated_at": "2016-10-13T18:21:59.842Z",
      "course_id": 223,
      "author_id": 677,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T18:21:59.450Z",
      "questions_updated_at": "2016-10-13T18:21:59.450Z",
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
Authorization: Bearer 1b673eccc9a2c4e3f31a2f77dd0a4500d96121fb0b7cfe8ec386b718ce99fe22
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
      "id": 122,
      "title": "Clever Chapter Title 110",
      "position": 1,
      "updated_at": "2016-10-13T18:21:59.189Z",
      "course_id": 221,
      "author_id": 668,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 123,
      "title": "Clever Chapter Title 111",
      "position": 2,
      "updated_at": "2016-10-13T18:21:59.217Z",
      "course_id": 221,
      "author_id": 669,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 124,
      "title": "Clever Chapter Title 112",
      "position": 3,
      "updated_at": "2016-10-13T18:21:59.246Z",
      "course_id": 221,
      "author_id": 670,
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
	-H "Authorization: Bearer 1b673eccc9a2c4e3f31a2f77dd0a4500d96121fb0b7cfe8ec386b718ce99fe22"
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
      "id": 128,
      "title": "Clever Chapter Title 116",
      "position": 1,
      "updated_at": "2016-10-13T18:21:59.975Z",
      "course_id": 224,
      "author_id": 681,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 129,
      "title": "Clever Chapter Title 117",
      "position": 2,
      "updated_at": "2016-10-13T18:22:00.003Z",
      "course_id": 224,
      "author_id": 682,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 130,
      "title": "Clever Chapter Title 118",
      "position": 3,
      "updated_at": "2016-10-13T18:22:00.032Z",
      "course_id": 224,
      "author_id": 683,
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
Authorization: Bearer c2e711d7f7c73c14f4c28814a70256d353cf3ee9bd6f24ef81f4c4c237dcb021
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
    "course_id": 106,
    "user_id": 339,
    "updated_at": "2016-10-13T18:21:28.060Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2e711d7f7c73c14f4c28814a70256d353cf3ee9bd6f24ef81f4c4c237dcb021"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0edb6c3e4d2950deca1577542376f73de3dc391c92b0d5513b97d21d3e224ca3
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
      "course_id": 103,
      "user_id": 329,
      "updated_at": "2016-10-13T18:21:27.529Z"
    },
    {
      "id": 3,
      "course_id": 103,
      "user_id": 330,
      "updated_at": "2016-10-13T18:21:27.546Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0edb6c3e4d2950deca1577542376f73de3dc391c92b0d5513b97d21d3e224ca3"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/161/files
Content-Type: application/json
Authorization: Bearer 2fa150a15edba19d85a7e249f971464dbb132529f18e28e2bfa2657c08906e03
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
      "id": 11,
      "uploader": {
        "id": 443,
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
        "created_at": "2016-10-13T18:21:38.176Z",
        "updated_at": "2016-10-13T18:21:38.176Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T18:21:38.184Z",
      "updated_at": "2016-10-13T18:21:38.184Z",
      "course_id": 161,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 12,
      "uploader": {
        "id": 444,
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
        "created_at": "2016-10-13T18:21:38.192Z",
        "updated_at": "2016-10-13T18:21:38.192Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T18:21:38.200Z",
      "updated_at": "2016-10-13T18:21:38.200Z",
      "course_id": 161,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 445,
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
        "created_at": "2016-10-13T18:21:38.208Z",
        "updated_at": "2016-10-13T18:21:38.208Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T18:21:38.215Z",
      "updated_at": "2016-10-13T18:21:38.215Z",
      "course_id": 161,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/161/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2fa150a15edba19d85a7e249f971464dbb132529f18e28e2bfa2657c08906e03"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/159/files
Content-Type: application/json
Authorization: Bearer 9c208d0387da2c3936ebee3644a00feb133d7cc4a7beea9a3f31422fb15e685e
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
    "id": 10,
    "uploader": {
      "id": 439,
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
      "created_at": "2016-10-13T18:21:37.918Z",
      "updated_at": "2016-10-13T18:21:37.918Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-13T18:21:37.951Z",
    "updated_at": "2016-10-13T18:21:37.951Z",
    "course_id": 159,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/159/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c208d0387da2c3936ebee3644a00feb133d7cc4a7beea9a3f31422fb15e685e"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/158/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer eb3be1fe441375cdc2ab2e9aa1aeb2f085145543a8c12fcbb4dfaa7d32e3f798
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
    "key": "cache/b3f675e9f3c5fe7414e90ad8d3de986a.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxOToyMTozN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9iM2Y2NzVlOWYzYzVmZTc0MTRlOTBhZDhkM2RlOTg2YS5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTgyMTM3WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T182137Z",
    "x-amz-signature": "4bb4bc37eda781696516b40343d199dd1c23b0c316af45b1f6561efcfcf2ae8e"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/158/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb3be1fe441375cdc2ab2e9aa1aeb2f085145543a8c12fcbb4dfaa7d32e3f798"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 27727e1d8cad43d64b5778eefcf525ddb5c2ab8cc320514058a2ba2e8fc53c90
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
	-H "Authorization: Bearer 27727e1d8cad43d64b5778eefcf525ddb5c2ab8cc320514058a2ba2e8fc53c90"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 75793ef86e7582d74d95010778c63a7cc7dbd5a10f9e2cb357eaa4c7091dece7
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
	-H "Authorization: Bearer 75793ef86e7582d74d95010778c63a7cc7dbd5a10f9e2cb357eaa4c7091dece7"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5081bb616327264a1602dc810c7877daf017f1b8b6b38c74123734b54f8c694d
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
	-H "Authorization: Bearer 5081bb616327264a1602dc810c7877daf017f1b8b6b38c74123734b54f8c694d"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 294f106fa1f7937fef039476fe8ea085b88141b1d96bbdbeb131d8e445c00668
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
	-H "Authorization: Bearer 294f106fa1f7937fef039476fe8ea085b88141b1d96bbdbeb131d8e445c00668"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer befdc2c5b4b83f8d31024458eec6775697b258c91fafafe105a3c0c538986952
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
	-H "Authorization: Bearer befdc2c5b4b83f8d31024458eec6775697b258c91fafafe105a3c0c538986952"
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
    "creator_id": 902,
    "id": 290,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 275,
    "additional_university_ids": [

    ],
    "topic_id": 302,
    "discipline_id": 303,
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
    "chapters_updated_at": "2016-10-13T18:22:19.258Z",
    "updated_at": "2016-10-13T18:22:20.781Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 181,
        "title": "Clever Chapter Title 166",
        "position": 1,
        "updated_at": "2016-10-13T18:22:20.731Z",
        "course_id": 290,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T18:22:19.258Z",
        "questions_updated_at": "2016-10-13T18:22:19.258Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 182,
        "title": "Clever Chapter Title 167",
        "position": 2,
        "updated_at": "2016-10-13T18:22:20.773Z",
        "course_id": 290,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T18:22:19.258Z",
        "questions_updated_at": "2016-10-13T18:22:19.258Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 111,
        "obfuscated_id": "G-D-sgMUtTw",
        "author_id": 902,
        "chapter_id": 181,
        "position": 98,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:19.483Z",
        "created_at": "2016-10-13T18:22:19.359Z",
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
            "id": 225,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 226,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 902,
        "chapter_id": 182,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:19.882Z",
        "created_at": "2016-10-13T18:22:19.757Z",
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
Authorization: Bearer d6bb5e77f1ef48a8c551e76e818d1fb84f5adbbfa8a7bef978313519ca468775
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
    "creator_id": 913,
    "id": 292,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 277,
    "additional_university_ids": [

    ],
    "topic_id": 304,
    "discipline_id": 305,
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
    "chapters_updated_at": "2016-10-13T18:22:22.482Z",
    "updated_at": "2016-10-13T18:22:24.051Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 185,
        "title": "Clever Chapter Title 170",
        "position": 1,
        "updated_at": "2016-10-13T18:22:23.999Z",
        "course_id": 292,
        "author_id": 913,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T18:22:22.482Z",
        "questions_updated_at": "2016-10-13T18:22:22.482Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 186,
        "title": "Clever Chapter Title 171",
        "position": 2,
        "updated_at": "2016-10-13T18:22:24.043Z",
        "course_id": 292,
        "author_id": 913,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T18:22:22.482Z",
        "questions_updated_at": "2016-10-13T18:22:22.482Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 914,
        "chapter_id": 185,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.817Z",
        "created_at": "2016-10-13T18:22:23.817Z",
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
        "author_id": 914,
        "chapter_id": 186,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.900Z",
        "created_at": "2016-10-13T18:22:23.900Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 914,
        "chapter_id": 185,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.861Z",
        "created_at": "2016-10-13T18:22:23.861Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 914,
        "chapter_id": 186,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.943Z",
        "created_at": "2016-10-13T18:22:23.943Z",
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
        "id": 123,
        "obfuscated_id": "N9-wuAhut60",
        "author_id": 914,
        "chapter_id": 185,
        "position": 110,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.720Z",
        "created_at": "2016-10-13T18:22:22.595Z",
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
      },
      {
        "id": 124,
        "obfuscated_id": "TD9SVjPLZ0Q",
        "author_id": 914,
        "chapter_id": 185,
        "position": 111,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:22.909Z",
        "created_at": "2016-10-13T18:22:22.791Z",
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
            "id": 251,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 252,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 125,
        "obfuscated_id": "K6zw0Yc6Me8",
        "author_id": 914,
        "chapter_id": 186,
        "position": 112,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.129Z",
        "created_at": "2016-10-13T18:22:22.999Z",
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
            "id": 253,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 254,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 126,
        "obfuscated_id": "fKTMLttUR-w",
        "author_id": 914,
        "chapter_id": 186,
        "position": 113,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T18:22:23.331Z",
        "created_at": "2016-10-13T18:22:23.201Z",
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
            "id": 255,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 256,
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
	-H "Authorization: Bearer d6bb5e77f1ef48a8c551e76e818d1fb84f5adbbfa8a7bef978313519ca468775"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/288/pin
Content-Type: application/json
Authorization: Bearer 120e0482fbbfe652690ddcd6f2f4623cbe91c0131c82c2e4b3e518a82695a27b
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/288/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 120e0482fbbfe652690ddcd6f2f4623cbe91c0131c82c2e4b3e518a82695a27b"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/278/pin
Content-Type: application/json
Authorization: Bearer 74cdb7df66fe677b5cee3d609e4a1a16effad5f4c026615be471c7e3db0a68dd
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/278/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74cdb7df66fe677b5cee3d609e4a1a16effad5f4c026615be471c7e3db0a68dd"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9f6f20d5f1a2d0f19246db18c8e2c46c7e65ddace0aaa0d870ece0ea84d645bc
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
    "creator_id": 871,
    "id": 277,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 262,
    "additional_university_ids": [

    ],
    "topic_id": 289,
    "discipline_id": 290,
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
    "updated_at": "2016-10-13T18:22:15.622Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f6f20d5f1a2d0f19246db18c8e2c46c7e65ddace0aaa0d870ece0ea84d645bc"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 985c8abefc07d9f995cc05e01106dd651b6266c6d3bf67a9cc65ce92218b621c
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
    "id": 823,
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
    "created_at": "2016-10-13T18:22:11.155Z",
    "updated_at": "2016-10-13T18:22:11.155Z",
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
	-H "Authorization: Bearer 985c8abefc07d9f995cc05e01106dd651b6266c6d3bf67a9cc65ce92218b621c"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c704e3bbed5c492b7565d26dced799861a739e950f51c729be91a96a6f4bbe49
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[274]}
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
    "id": 825,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      274
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T18:22:11.630Z",
    "updated_at": "2016-10-13T18:22:11.669Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[274]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c704e3bbed5c492b7565d26dced799861a739e950f51c729be91a96a6f4bbe49"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 52446fa9c2c2c635edd7f2f99cd257f32ae03eb77f4715ce748d3dcb8517e2aa
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
    "id": 827,
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
    "created_at": "2016-10-13T18:22:11.776Z",
    "updated_at": "2016-10-13T18:22:11.776Z",
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
	-H "Authorization: Bearer 52446fa9c2c2c635edd7f2f99cd257f32ae03eb77f4715ce748d3dcb8517e2aa"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a089f1523004842c2d4ea2ad502877dbb38165d20c6afb0dbb2af571371771b3
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[277]}
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
    "id": 828,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      277
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T18:22:11.881Z",
    "updated_at": "2016-10-13T18:22:11.881Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[277]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a089f1523004842c2d4ea2ad502877dbb38165d20c6afb0dbb2af571371771b3"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a7083c25ea469a5908a0adea70575794dbac33dfa6ba33ba72ce01b4c647635a
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

273
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
    "id": 824,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0c07e8b323d5103a0e38299b5bf079e700f7ba85.jpg",
    "university_id": null,
    "fields_of_study": [
      273
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T18:22:11.260Z",
    "updated_at": "2016-10-13T18:22:11.568Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/622ea09bf603bef9e8291936756814623ae0f96a.jpg",
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

273
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a7083c25ea469a5908a0adea70575794dbac33dfa6ba33ba72ce01b4c647635a"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 8cb9eea5eebaeafbcd3960dac8cdcdb5ba5853516d2267035f0845d06e56e8fd
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
      "bookmarkable_id": 28,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 29,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 30,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cb9eea5eebaeafbcd3960dac8cdcdb5ba5853516d2267035f0845d06e56e8fd"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b3bb9eb442aed0603e7964e739d4b26aeb0bb67dedfe7c6a3948b26a783de661
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
      "title": "Campaign 10",
      "company_id": 31,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 32,
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
	-H "Authorization: Bearer b3bb9eb442aed0603e7964e739d4b26aeb0bb67dedfe7c6a3948b26a783de661"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer cce83ed8ee8a2d7ffe574abbe0161cd3851e167852af836a2328196cb5407105
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
      "id": 9,
      "title": "Campaign 9",
      "company_id": 27,
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
	-H "Authorization: Bearer cce83ed8ee8a2d7ffe574abbe0161cd3851e167852af836a2328196cb5407105"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer aa8fac24d5debec31b3ed779b73d20794390c047bd40388a997cd30864a64cdb
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
      "creator_id": 427,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-132",
      "html_url": "https://goskive.com/course/mit-course-132",
      "slug": "mit-course-132",
      "university_id": 141,
      "additional_university_ids": [

      ],
      "topic_id": 163,
      "discipline_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "updated_at": "2016-10-13T18:21:37.346Z",
      "shortname": "mit-course-132"
    },
    {
      "creator_id": 428,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-133",
      "html_url": "https://goskive.com/course/mit-course-133",
      "slug": "mit-course-133",
      "university_id": 142,
      "additional_university_ids": [

      ],
      "topic_id": 164,
      "discipline_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 133",
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
      "updated_at": "2016-10-13T18:21:37.434Z",
      "shortname": "mit-course-133"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa8fac24d5debec31b3ed779b73d20794390c047bd40388a997cd30864a64cdb"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 3ef77bc801f13f872763e45a423dcbb04f390077f011490854d04383268ed8f7
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T18:21:02.945Z"
      },
      "created_at": "2016-10-13T18:21:02.949Z",
      "updated_at": "2016-10-13T18:21:02.949Z",
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 7",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T18:21:02.958Z"
      },
      "created_at": "2016-10-13T18:21:02.962Z",
      "updated_at": "2016-10-13T18:21:02.962Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ef77bc801f13f872763e45a423dcbb04f390077f011490854d04383268ed8f7"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 12e62bf8d6637180deed542b0dd9e8105e956ac9c2b1528ad9aba996dcd8e2a2
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
      "company_id": 2,
      "company": {
        "id": 2,
        "name": "Fake Company Name 2",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T18:21:02.401Z"
      },
      "created_at": "2016-10-13T18:21:02.406Z",
      "updated_at": "2016-10-13T18:21:02.406Z",
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
      "company_id": 3,
      "company": {
        "id": 3,
        "name": "Fake Company Name 3",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T18:21:02.427Z"
      },
      "created_at": "2016-10-13T18:21:02.431Z",
      "updated_at": "2016-10-13T18:21:02.431Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12e62bf8d6637180deed542b0dd9e8105e956ac9c2b1528ad9aba996dcd8e2a2"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 2adbbd50b0e64742610ab3477b09ddaedc371e1510f8f05b3e974a71622f1fd1
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
      "id": 14,
      "created_at": "2016-10-13T18:22:02.568Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-10-13T18:22:02.692Z",
      "author_id": "711",
      "thread_subject_id": "234",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 15,
      "created_at": "2016-10-13T18:22:02.679Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-10-13T18:22:02.696Z",
      "author_id": "714",
      "thread_subject_id": "235",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-10-13T18:22:03.110Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-13T18:22:03.110Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-13T18:22:03.518Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-10-13T18:22:03.518Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 18,
      "created_at": "2016-10-13T18:22:03.924Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 20,
      "updated_at": "2016-10-13T18:22:03.924Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 19,
      "created_at": "2016-10-13T18:22:04.234Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 92,
      "updated_at": "2016-10-13T18:22:04.234Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-10-13T18:22:04.556Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 93,
      "updated_at": "2016-10-13T18:22:04.556Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-13T18:22:04.866Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 94,
      "updated_at": "2016-10-13T18:22:04.866Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2adbbd50b0e64742610ab3477b09ddaedc371e1510f8f05b3e974a71622f1fd1"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/13
Content-Type: application/json
Authorization: Bearer 626295de50c6dde186917a2b95dc4365aa383100315531b46a895511597d4795
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-13T18:12:02.000Z"}}
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
    "id": 13,
    "created_at": "2016-10-13T18:22:02.374Z",
    "read_at": "2016-10-13T18:12:02.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 56,
    "updated_at": "2016-10-13T18:22:02.440Z",
    "author_id": "707",
    "thread_subject_id": "233",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/13" -d '{"notification":{"read_at":"2016-10-13T18:12:02.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 626295de50c6dde186917a2b95dc4365aa383100315531b46a895511597d4795"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3c891466f85b51c3d3056e543f73e50982a200febcd146a332155fa1c56e1c4e
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
      "id": 7,
      "course_id": 306,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T18:22:27.786Z",
      "course_published": true,
      "updated_at": "2016-10-13T18:22:27.778Z"
    },
    {
      "id": 8,
      "course_id": 307,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T18:22:27.878Z",
      "course_published": true,
      "updated_at": "2016-10-13T18:22:27.869Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c891466f85b51c3d3056e543f73e50982a200febcd146a332155fa1c56e1c4e"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer ad14843c0e81a35cf2891bd71f976c1619e6530fd9266cecbb23c50512def2fd
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
    "course_id": 303,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T18:22:27.402Z",
    "course_published": true,
    "updated_at": "2016-10-13T18:22:27.392Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad14843c0e81a35cf2891bd71f976c1619e6530fd9266cecbb23c50512def2fd"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer a7a25cfb47cebfaf3fa240ec5cb1dc2f655782c3e027b4829336845099fabcae
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
    "course_id": 302,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-13T18:22:27.286Z",
    "course_published": true,
    "updated_at": "2016-10-13T18:22:27.274Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7a25cfb47cebfaf3fa240ec5cb1dc2f655782c3e027b4829336845099fabcae"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer d58e3d028f67ebafd4b9a091e94f2a30720b3e37d80218bdde50a90d0b2097bf
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
      "votable_id": 69,
      "user_id": 540
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 70,
      "user_id": 540
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 71,
      "user_id": 540
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 72,
      "user_id": 540
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d58e3d028f67ebafd4b9a091e94f2a30720b3e37d80218bdde50a90d0b2097bf"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/163
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
    "id": 163,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 161,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 163
      },
      {
        "id": 162,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 163
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/163" -X GET \
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
      "id": 161,
      "name": "Intuitive 4th generation help-desk",
      "name_translations": {
        "en": "Intuitive 4th generation help-desk"
      }
    },
    {
      "id": 162,
      "name": "Upgradable global monitoring",
      "name_translations": {
        "en": "Upgradable global monitoring"
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
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer d6fa5094a795380b60529213293eb352ab4218d7df22f684aad68e4103aa8a9e
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
    "id": 21,
    "user_id": 155,
    "feedbackable_id": 10,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-13T18:21:17.894Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/21/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6fa5094a795380b60529213293eb352ab4218d7df22f684aad68e4103aa8a9e"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 2d0f142c32361f8045b74707c94f627798d5a3dd7868095a1c93c635646f36c0
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
    "id": 25,
    "user_id": 175,
    "feedbackable_id": 14,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-13T18:21:19.070Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d0f142c32361f8045b74707c94f627798d5a3dd7868095a1c93c635646f36c0"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer 9031079ac9ce02247df5e2c8106cada33b070bbb35500ae8211708d454c4cf55
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
    "user_id": 190,
    "feedbackable_id": 17,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T18:21:20.102Z",
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
	-H "Authorization: Bearer 9031079ac9ce02247df5e2c8106cada33b070bbb35500ae8211708d454c4cf55"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer 1e5220d388f21b4ed655f1f54014ddec945c43631d2df2f62fc15efaa61cd830
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
curl "api.goskive.com/v2/feedbacks/23/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e5220d388f21b4ed655f1f54014ddec945c43631d2df2f62fc15efaa61cd830"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer a937287fdfb58d04a137c3e98021236c0ee84aae9708a748f50a70c1f8b86b98
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
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a937287fdfb58d04a137c3e98021236c0ee84aae9708a748f50a70c1f8b86b98"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 2db5d66c1d1afe35590eb3e4f918f21c20b5907ea8d21b8833aba662754f957e
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
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2db5d66c1d1afe35590eb3e4f918f21c20b5907ea8d21b8833aba662754f957e"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/29
Content-Type: application/json
Authorization: Bearer a77083704803062c574f04427e010af45b64eb5e159e7807e1dd0736f8eec254
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
    "user_id": 195,
    "feedbackable_id": 18,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T18:21:20.397Z",
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
	-H "Authorization: Bearer a77083704803062c574f04427e010af45b64eb5e159e7807e1dd0736f8eec254"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 7bd39d80d93326f0f7756fa49f7f7f52f1540fa23574e31cd9de34c98d9ac6e3
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
	-H "Authorization: Bearer 7bd39d80d93326f0f7756fa49f7f7f52f1540fa23574e31cd9de34c98d9ac6e3" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer bc92739ca12b237042c2411b6defd440b16b515d37bce58ce16d7931ae4e3d84
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
	-H "Authorization: Bearer bc92739ca12b237042c2411b6defd440b16b515d37bce58ce16d7931ae4e3d84" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/6
Authorization: Bearer b635a9548a61eeb3ca1e81054a20cd7e591631573750b573fdd2832970144f44
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/748373c13f2a890fc1020903510baaf4.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T182126Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=82ed4293727bd8e4648a11279a759288e778a7655adaed0d0efa22a3aae1600c"
  }
}
```



```shell
curl "api.goskive.com/v2/files/6" -X GET \
	-H "Authorization: Bearer b635a9548a61eeb3ca1e81054a20cd7e591631573750b573fdd2832970144f44"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Authorization: Bearer 071cb0af5666716aa7ace4b89296e90b74dce4f7a0fc03b53b78b3153c0ca477
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
    "id": 8,
    "uploader": {
      "id": 317,
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
      "created_at": "2016-10-13T18:21:26.626Z",
      "updated_at": "2016-10-13T18:21:26.626Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-13T18:21:26.704Z",
    "updated_at": "2016-10-13T18:21:26.704Z",
    "course_id": 99,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Authorization: Bearer 071cb0af5666716aa7ace4b89296e90b74dce4f7a0fc03b53b78b3153c0ca477" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer d5b5bfca73a7fe3199a31da0ebebc38a0ce04c499a30228f794f1a53ac864317
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
      "creator_id": 33,
      "id": 9,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 9,
      "additional_university_ids": [

      ],
      "topic_id": 9,
      "discipline_id": 9,
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
      "chapters_updated_at": "2016-10-13T18:21:05.615Z",
      "updated_at": "2016-10-13T18:21:07.428Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 38,
      "id": 10,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-222f9649-60ff-46a9-8885-643290a6f805",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-222f9649-60ff-46a9-8885-643290a6f805",
      "slug": "mit-the-great-british-bake-off-222f9649-60ff-46a9-8885-643290a6f805",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "topic_id": 10,
      "discipline_id": 10,
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
      "chapters_updated_at": "2016-10-13T18:21:05.615Z",
      "updated_at": "2016-10-13T18:21:08.021Z",
      "shortname": "mit-the-great-british-bake-off-222f9649-60ff-46a9-8885-643290a6f805"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer d5b5bfca73a7fe3199a31da0ebebc38a0ce04c499a30228f794f1a53ac864317"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/7/preview
Authorization: Bearer 142ef3f444d781926b4fd48f448d94afb45c0ffe5bc36336a5379f7095382bb2
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/8e8732d924781aed17eaa79234b03fdf.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T182126Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=c499c2e3831b6b8abdea2a6251dae5f8065d26439033177daf7e4820e095fbf1"
  }
}
```



```shell
curl "api.goskive.com/v2/files/7/preview" -X GET \
	-H "Authorization: Bearer 142ef3f444d781926b4fd48f448d94afb45c0ffe5bc36336a5379f7095382bb2"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/9/report
Authorization: Bearer ea577bc883b391eae824d8727e892177d06828505e0137d7e4ab8e74eae8e99d
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
curl "api.goskive.com/v2/files/9/report" -d '' -X PUT \
	-H "Authorization: Bearer ea577bc883b391eae824d8727e892177d06828505e0137d7e4ab8e74eae8e99d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/3/comments
Content-Type: application/json
Authorization: Bearer 03dbab883cc80f955f0ecfaec0d391d557512bb62969d29dc84003da49afae88
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
    "id": 3,
    "author_id": 12,
    "reply_to_id": null,
    "created_at": "2016-10-13T18:21:04.488Z",
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
curl "api.goskive.com/v2/flashcards/3/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03dbab883cc80f955f0ecfaec0d391d557512bb62969d29dc84003da49afae88"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/5/comments
Content-Type: application/json
Authorization: Bearer ef5712a45a1f036159b50ea69d82ba5f89125618da0133aa606b6b0b66d5e56b
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
    "author_id": 18,
    "reply_to_id": null,
    "created_at": "2016-10-13T18:21:05.251Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 18,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:05.246Z",
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
curl "api.goskive.com/v2/flashcards/5/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef5712a45a1f036159b50ea69d82ba5f89125618da0133aa606b6b0b66d5e56b"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/2/comments
Content-Type: application/json
Authorization: Bearer 8afd9c34b8ce54b8810d6c01c443c564c578f1e37f2a9658506e5e95323591c1
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
      "id": 1,
      "author_id": 10,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:04.207Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 11,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:04.247Z",
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
curl "api.goskive.com/v2/flashcards/2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8afd9c34b8ce54b8810d6c01c443c564c578f1e37f2a9658506e5e95323591c1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/4/comments
Content-Type: application/json
Authorization: Bearer 4264dbc02bd82d6736d307ac2a64cb0508d64cf0c9dfa682c7f9bae3c54391b4
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
curl "api.goskive.com/v2/flashcards/4/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4264dbc02bd82d6736d307ac2a64cb0508d64cf0c9dfa682c7f9bae3c54391b4"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/34/feedbacks
Content-Type: application/json
Authorization: Bearer 6add28f9747b503adebfd786522ec1bcf4df4ae54d40bbbca1b150bd0c39bb10
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
    "user_id": 587,
    "feedbackable_id": 34,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T18:21:51.887Z",
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
curl "api.goskive.com/v2/flashcards/34/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6add28f9747b503adebfd786522ec1bcf4df4ae54d40bbbca1b150bd0c39bb10"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/32/feedbacks
Content-Type: application/json
Authorization: Bearer a671ae1e325756ee889be056169b62dbf6bd1475064db19e0b7037ab1814d1fc
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
      "user_id": 583,
      "feedbackable_id": 32,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:51.487Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 582,
      "feedbackable_id": 32,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:51.474Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/32/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a671ae1e325756ee889be056169b62dbf6bd1475064db19e0b7037ab1814d1fc"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/38/votes
Content-Type: application/json
Authorization: Bearer a47f2d1391ad0fe48aa4a8e1a9b146cc3ea40d0ed76cc99f2f4c16662acb456f
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
      "user_id": 605
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 38,
      "user_id": 604
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 38,
      "user_id": 603
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/38/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a47f2d1391ad0fe48aa4a8e1a9b146cc3ea40d0ed76cc99f2f4c16662acb456f"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/61/republish
Content-Type: application/json
Authorization: Bearer 598a8a0546bc43edf0a8a0619f909ab19915b2c647195543cc62fbb51bc8357b
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
curl "api.goskive.com/v2/flashcards/61/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 598a8a0546bc43edf0a8a0619f909ab19915b2c647195543cc62fbb51bc8357b"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/bookmark
Content-Type: application/json
Authorization: Bearer a8a5c0a8afb1847860ece0ba5c494cbd26bcf25d4db373d9156699e785d930f6
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8a5c0a8afb1847860ece0ba5c494cbd26bcf25d4db373d9156699e785d930f6"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/60
Content-Type: application/json
Authorization: Bearer ed223f614577bf0b11ac465537f881d4ff10c250ea825207a7ec679870086b06
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
	-H "Authorization: Bearer ed223f614577bf0b11ac465537f881d4ff10c250ea825207a7ec679870086b06"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/downvote
Content-Type: application/json
Authorization: Bearer 7dd5f25e75181d73e962fade63ccb8ce35d032cb52805e3b8f859f8b591858fe
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dd5f25e75181d73e962fade63ccb8ce35d032cb52805e3b8f859f8b591858fe"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/64
Content-Type: application/json
Authorization: Bearer 619e024473aad174c484e68148bd8382689c880b0ef01023fb5cda0a9fea8f4f
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
    "id": 64,
    "obfuscated_id": "H-V851w7HZg",
    "author_id": 809,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:22:09.155Z",
    "created_at": "2016-10-13T18:22:09.155Z",
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
curl "api.goskive.com/v2/flashcards/64" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 619e024473aad174c484e68148bd8382689c880b0ef01023fb5cda0a9fea8f4f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/59/report
Content-Type: application/json
Authorization: Bearer d5241101adb15c91340b96f5cca6391a81ded807ef2ab44a1b5ff325ce5d97fa
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/59/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5241101adb15c91340b96f5cca6391a81ded807ef2ab44a1b5ff325ce5d97fa"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/42/bookmark
Content-Type: application/json
Authorization: Bearer 0971948d1f0390e655b92a2889f7aabd2a9838d62ec7c2f3b42ba4fa2c0c774c
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0971948d1f0390e655b92a2889f7aabd2a9838d62ec7c2f3b42ba4fa2c0c774c"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/58/upvote
Content-Type: application/json
Authorization: Bearer 68b29e2f60c2b50444d7bbf25ade5751c20ae85339d26e8095facdeaa7922748
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68b29e2f60c2b50444d7bbf25ade5751c20ae85339d26e8095facdeaa7922748"
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
    "key": "cache/940c743aa28c0bcef287ebafcd3ea5e9.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxOToyMTo1M1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS85NDBjNzQzYWEyOGMwYmNlZjI4N2ViYWZjZDNlYTVlOS5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTgyMTUzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T182153Z",
    "x-amz-signature": "a81680948f264eaaf21a80b38e657c03bebd99364e400e7319d0cbb1cc30d43a"
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
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 7be713bf99cc1ca714c9e2f1e19646f8fabfd532d7c455926e2fc9a2fea5cbb8
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
curl "api.goskive.com/v2/me/jobs/9/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7be713bf99cc1ca714c9e2f1e19646f8fabfd532d7c455926e2fc9a2fea5cbb8"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer f255868a6cc9f871a1179258ea5856b5c1e722cd5979f826eb7b428a4b9e2db0
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
	-H "Authorization: Bearer f255868a6cc9f871a1179258ea5856b5c1e722cd5979f826eb7b428a4b9e2db0"
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
{"password":{"reset_password_token":"7dS1B_RFVv8BsfAoTGZz","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 815,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-13T18:22:09.436Z",
  "updated_at": "2016-10-13T18:22:10.104Z",
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
  "audit_id": 4628
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"7dS1B_RFVv8BsfAoTGZz","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/35/comments
Content-Type: application/json
Authorization: Bearer 73cb44adc223676cfb75a0ec91b85f60d491859cf4d54f93aeb39e16b99e2484
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
    "id": 49,
    "author_id": 354,
    "reply_to_id": null,
    "created_at": "2016-10-13T18:21:29.751Z",
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
curl "api.goskive.com/v2/questions/35/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73cb44adc223676cfb75a0ec91b85f60d491859cf4d54f93aeb39e16b99e2484"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/36/comments
Content-Type: application/json
Authorization: Bearer 52b09b896a5b977f25580c43766a48e7c5b6c1269df1c9d4f2fff55137b816a4
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
    "id": 50,
    "author_id": 357,
    "reply_to_id": null,
    "created_at": "2016-10-13T18:21:30.288Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 30,
      "user_id": 357,
      "feedbackable_id": 36,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:21:30.285Z",
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
curl "api.goskive.com/v2/questions/36/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52b09b896a5b977f25580c43766a48e7c5b6c1269df1c9d4f2fff55137b816a4"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/34/comments
Content-Type: application/json
Authorization: Bearer 8b06f5c4e6f2652fe9331ad4e93adf7f32b0b03845caff64a271b0007440ffb3
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
      "id": 47,
      "author_id": 352,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:29.306Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 353,
      "reply_to_id": null,
      "created_at": "2016-10-13T18:21:29.326Z",
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
curl "api.goskive.com/v2/questions/34/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b06f5c4e6f2652fe9331ad4e93adf7f32b0b03845caff64a271b0007440ffb3"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/37/comments
Content-Type: application/json
Authorization: Bearer a95828331f78fd61e8d00e4541085699164cbe33b146f6c93bbbe7d0b67dd8b7
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
curl "api.goskive.com/v2/questions/37/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a95828331f78fd61e8d00e4541085699164cbe33b146f6c93bbbe7d0b67dd8b7"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/102/feedbacks
Content-Type: application/json
Authorization: Bearer c9c234ad162d3dcd0547a6128b801aa6921c643a2f5f90dd5924be1b53ba6f3a
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
    "id": 46,
    "user_id": 862,
    "feedbackable_id": 102,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-13T18:22:14.928Z",
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
curl "api.goskive.com/v2/questions/102/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9c234ad162d3dcd0547a6128b801aa6921c643a2f5f90dd5924be1b53ba6f3a"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer c53c192d87bef908c312ce73977b6ba0f26692322d9a1d494b84df18700a9b79
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
      "user_id": 833,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:22:12.263Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 832,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T18:22:12.251Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/95/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c53c192d87bef908c312ce73977b6ba0f26692322d9a1d494b84df18700a9b79"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/81/votes
Content-Type: application/json
Authorization: Bearer c725247648b2190d6c285cd2b3c6a7055e0852638a7d9cf1ec30ae8dd34db703
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
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 635
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 634
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 633
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/81/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c725247648b2190d6c285cd2b3c6a7055e0852638a7d9cf1ec30ae8dd34db703"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/64/republish
Content-Type: application/json
Authorization: Bearer a9f2990008373532ee2bb05576070c4e58290af75836ff625c9d228d5070d041
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
curl "api.goskive.com/v2/questions/64/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9f2990008373532ee2bb05576070c4e58290af75836ff625c9d228d5070d041"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/47/bookmark
Content-Type: application/json
Authorization: Bearer e9436cf3e263b3983a8d6ff75c55244e9de0b7f535cdf1b4327233efa1b3bb31
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/47/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9436cf3e263b3983a8d6ff75c55244e9de0b7f535cdf1b4327233efa1b3bb31"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/44
Content-Type: application/json
Authorization: Bearer 7b0248d2a9305aa724719886debdd5605e5b6497a637b359228731fea2620089
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b0248d2a9305aa724719886debdd5605e5b6497a637b359228731fea2620089"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/68/downvote
Content-Type: application/json
Authorization: Bearer 5011bd880f4be47899bbf07d61cec95336b99056096d5cb4c03e4a358007a2d4
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/68/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5011bd880f4be47899bbf07d61cec95336b99056096d5cb4c03e4a358007a2d4"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/46
Content-Type: application/json
Authorization: Bearer b56fa0dfa5c23bc8fa3395ba79714c53c08ed9ce99da7a712cb9ca22cb5ca8d9
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
    "id": 46,
    "obfuscated_id": "urkHiAaH08E",
    "author_id": 465,
    "chapter_id": 63,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:40.572Z",
    "created_at": "2016-10-13T18:21:40.449Z",
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
        "id": 91,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 92,
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
curl "api.goskive.com/v2/questions/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b56fa0dfa5c23bc8fa3395ba79714c53c08ed9ce99da7a712cb9ca22cb5ca8d9"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/45/report
Content-Type: application/json
Authorization: Bearer 2b0e624aacbfffa717201a809119deefd8ef8d5f6e3bd3a9bc5ae4d7c5decd30
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b0e624aacbfffa717201a809119deefd8ef8d5f6e3bd3a9bc5ae4d7c5decd30"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/48/bookmark
Content-Type: application/json
Authorization: Bearer 07fbed9435ac7e8f52b351fee3d38307e74abf8e42e3d934e49e94b0a9d2b356
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07fbed9435ac7e8f52b351fee3d38307e74abf8e42e3d934e49e94b0a9d2b356"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/66
Content-Type: application/json
Authorization: Bearer 7c1791bd6edad726d420ffb45880381830cb6d82b97fb4e6d7ae5405933a4255
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":66,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T18:21:47.092Z","updated_at":"2016-10-13T18:21:47.219Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":83,"author_id":530,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 530,
    "chapter_id": 83,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T18:21:47.337Z",
    "created_at": "2016-10-13T18:21:47.092Z",
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
    "question": "{\"id\"=>66, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-13T18:21:47.092Z\", \"updated_at\"=>\"2016-10-13T18:21:47.219Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>83, \"author_id\"=>530, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 131,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 132,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 133,
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
curl "api.goskive.com/v2/questions/66" -d '{"question":{"question":{"id":66,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T18:21:47.092Z","updated_at":"2016-10-13T18:21:47.219Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":83,"author_id":530,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c1791bd6edad726d420ffb45880381830cb6d82b97fb4e6d7ae5405933a4255"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/67/upvote
Content-Type: application/json
Authorization: Bearer 427a6274d0a08b010d6c8d5ae9194ea872bde72496c76e02f6cd66bcf66cf7dd
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
	-H "Authorization: Bearer 427a6274d0a08b010d6c8d5ae9194ea872bde72496c76e02f6cd66bcf66cf7dd"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 2aecae5276326d804207f6b1c138373d74bf109d2468cc5c19082f215ca0adf2
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
      "creator_id": 49,
      "id": 14,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 14,
      "discipline_id": 14,
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
      "updated_at": "2016-10-13T18:21:08.536Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2aecae5276326d804207f6b1c138373d74bf109d2468cc5c19082f215ca0adf2"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 98bf96a4c4e3be34ba76567bb60a3d12fcc8c62e6d2c3b58660df1fe627369f4
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
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-16",
      "html_url": "https://goskive.com/university/uni-16",
      "slug": "uni-16",
      "name": "National School of Pizza",
      "short_name": "Uni 16",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/1ef510945d5d3f43a0a9347f14a495ed8fd64871.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ee933d930ceb53158e4e123f0a5a77fa831367dc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T18:21:08.894Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-15",
      "html_url": "https://goskive.com/university/uni-15",
      "slug": "uni-15",
      "name": "National School of Pastry",
      "short_name": "Uni 15",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/49b13ba9ae73a6b6a418ca371168b83d85364553.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/379dabebbcd9aa1d7a88440cb1930bc2d4f35cb0.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T18:21:08.872Z",
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
	-H "Authorization: Bearer 98bf96a4c4e3be34ba76567bb60a3d12fcc8c62e6d2c3b58660df1fe627369f4"
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
      "id": 21,
      "name": "Open-architected scalable throughput",
      "name_translations": {
        "en": "Open-architected scalable throughput"
      },
      "discipline_id": 21
    },
    {
      "id": 22,
      "name": "Re-engineered clear-thinking application",
      "name_translations": {
        "en": "Re-engineered clear-thinking application"
      },
      "discipline_id": 22
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
GET /v2/topics/23
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
    "id": 23,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 23
  }
}
```



```shell
curl "api.goskive.com/v2/topics/23" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer fac450083459ab92a06d2d5ded71741909b3a774b9451b9e74abbf046d76cdd9
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
      "id": 120,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-118",
      "html_url": "https://goskive.com/university/uni-118",
      "slug": "uni-118",
      "name": "University 103",
      "short_name": "Uni 118",
      "acronym": "MIT",
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
      "updated_at": "2016-10-13T18:21:32.278Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 121,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-119",
      "html_url": "https://goskive.com/university/uni-119",
      "slug": "uni-119",
      "name": "University 104",
      "short_name": "Uni 119",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/470820012be01096d3034d1bbb55fdf7899a179d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6bd6b1122de529932d5408d414466ab16fbcd503.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T18:21:32.298Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 122,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-120",
      "html_url": "https://goskive.com/university/uni-120",
      "slug": "uni-120",
      "name": "University 105",
      "short_name": "Uni 120",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b909b44c83b957d381586d156e48cf99a3b89d07.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1b64eb8a1e9da35f8b37f41ebff0eceafe105546.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T18:21:32.318Z",
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
	-H "Authorization: Bearer fac450083459ab92a06d2d5ded71741909b3a774b9451b9e74abbf046d76cdd9"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 7230e976a47dec1adb3f4dab38a8587d30aeb7bcdb8b1f22784445ecb181d1d8
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
    "id": 118,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/10c45072caa721987b05dfcb635cef9f53e6bb5b.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/abe07e3df800339993de4e0db7bdc7e30ac9c4ff.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-13T18:21:32.120Z",
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
	-H "Authorization: Bearer 7230e976a47dec1adb3f4dab38a8587d30aeb7bcdb8b1f22784445ecb181d1d8"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 106a8232ea930c7e60cb0f665521a215f740d15294e523c4a7c37717a4261181
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":122,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 382,
    "id": 117,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 124,
    "additional_university_ids": [

    ],
    "topic_id": 122,
    "discipline_id": 122,
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
    "chapters_updated_at": "2016-10-13T18:21:32.590Z",
    "updated_at": "2016-10-13T18:21:32.753Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 50,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-13T18:21:32.697Z",
        "course_id": 117,
        "author_id": 382,
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
        "id": 51,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-13T18:21:32.719Z",
        "course_id": 117,
        "author_id": 382,
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
        "id": 52,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-13T18:21:32.740Z",
        "course_id": 117,
        "author_id": 382,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":122,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 106a8232ea930c7e60cb0f665521a215f740d15294e523c4a7c37717a4261181"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b758310fc5a7e7346408ba8b0f6f9659763dc5863e3861e5e0b956cd433b3266
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":123,"published":false}}
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
    "creator_id": 383,
    "id": 118,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 125,
    "additional_university_ids": [

    ],
    "topic_id": 123,
    "discipline_id": 123,
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
    "updated_at": "2016-10-13T18:21:32.925Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":123,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b758310fc5a7e7346408ba8b0f6f9659763dc5863e3861e5e0b956cd433b3266"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 35c88f831dbc702ab5c004c8d38b299c492157295f665d329a4242c3d5af2082
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
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 135,
      "discipline_id": 135,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
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
      "updated_at": "2016-10-13T18:21:34.248Z",
      "shortname": "fu-course-106"
    },
    {
      "creator_id": 396,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 136,
      "discipline_id": 136,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
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
      "chapters_updated_at": "2016-10-13T18:21:34.560Z",
      "updated_at": "2016-10-13T18:21:34.567Z",
      "shortname": "fu-course-107"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35c88f831dbc702ab5c004c8d38b299c492157295f665d329a4242c3d5af2082"
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
      "creator_id": 406,
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-114",
      "html_url": "https://goskive.com/course/fu-course-114",
      "slug": "fu-course-114",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 143,
      "discipline_id": 143,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 114",
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
      "updated_at": "2016-10-13T18:21:35.193Z",
      "shortname": "fu-course-114"
    },
    {
      "creator_id": 406,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 144,
      "discipline_id": 144,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 115",
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
      "chapters_updated_at": "2016-10-13T18:21:35.501Z",
      "updated_at": "2016-10-13T18:21:35.508Z",
      "shortname": "fu-course-115"
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
Authorization: Bearer dad2aef63e528253660b6a94c9dafcc0a5a9959c21e001fa79e92e85a23e0b6e
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
      "creator_id": 403,
      "id": 134,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 139,
      "discipline_id": 139,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
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
      "updated_at": "2016-10-13T18:21:34.880Z",
      "shortname": "fu-course-110"
    },
    {
      "creator_id": 403,
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 140,
      "discipline_id": 140,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
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
      "updated_at": "2016-10-13T18:21:34.926Z",
      "shortname": "fu-course-111"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dad2aef63e528253660b6a94c9dafcc0a5a9959c21e001fa79e92e85a23e0b6e"
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
      "creator_id": 411,
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-118",
      "html_url": "https://goskive.com/course/fu-course-118",
      "slug": "fu-course-118",
      "university_id": 134,
      "additional_university_ids": [

      ],
      "topic_id": 147,
      "discipline_id": 147,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 118",
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
      "updated_at": "2016-10-13T18:21:35.704Z",
      "shortname": "fu-course-118"
    },
    {
      "creator_id": 411,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 134,
      "additional_university_ids": [

      ],
      "topic_id": 148,
      "discipline_id": 148,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
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
      "updated_at": "2016-10-13T18:21:35.748Z",
      "shortname": "fu-course-119"
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
Authorization: Bearer 013df4a964132f5cbdc8443e4afc7b66fb1022e9ac034610278da0fefc3a88c3
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
  "id": 556,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-13T18:21:50.239Z",
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
	-H "Authorization: Bearer 013df4a964132f5cbdc8443e4afc7b66fb1022e9ac034610278da0fefc3a88c3"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/375
Content-Type: application/json
Authorization: Bearer 729800451fbb9a248a19b8c40686f171d95b0612a78a3cc351888fa7bd8dd5e4
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
    "id": 375,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 117,
    "fields_of_study": [
      119,
      120
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-13T18:21:32.036Z",
    "updated_at": "2016-10-13T18:21:32.036Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/375" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 729800451fbb9a248a19b8c40686f171d95b0612a78a3cc351888fa7bd8dd5e4"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/373
Content-Type: application/json
Authorization: Bearer 40ff27ad4e38112f341794cbd49bd21a74edbc0d0f08ebf1c89092d7fe5a847d
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
    "id": 373,
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
    "created_at": "2016-10-13T18:21:31.865Z",
    "updated_at": "2016-10-13T18:21:31.865Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/373" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40ff27ad4e38112f341794cbd49bd21a74edbc0d0f08ebf1c89092d7fe5a847d"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/17
Content-Type: application/json
Authorization: Bearer 434ece689454fe290847539e60eae5f663dde4d6ac89af28e9166b67a5731daa
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
	-H "Authorization: Bearer 434ece689454fe290847539e60eae5f663dde4d6ac89af28e9166b67a5731daa"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/15
Content-Type: application/json
Authorization: Bearer fe96b9d46ab6033f217779615b25daa0d570620047e431b708f2440eb3110068
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
    "id": 15,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 86,
    "user_id": 693
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe96b9d46ab6033f217779615b25daa0d570620047e431b708f2440eb3110068"
```
