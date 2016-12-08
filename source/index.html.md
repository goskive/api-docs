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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"bee2797333544136402f950321c210e5c76ac13d1bf2044cb51f24f51c604d3d","client_secret":"86518d2f8f10aadad8b645bb189fee23b1ce0d5cf8b4d290b4d0adf109e07659"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"bee2797333544136402f950321c210e5c76ac13d1bf2044cb51f24f51c604d3d","client_secret":"86518d2f8f10aadad8b645bb189fee23b1ce0d5cf8b4d290b4d0adf109e07659"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTk1NzJkODgyNDBjZjExMDFkOGYxNWQ1MTM5OWFiNGJjODQwNjRhZjVmN2Ji
MTMyNTJlMTg1MzgxM2UyNTMzMjo3NDMzNjgyMzEyYmYzZGI1NzVhMWVmYmU3
NmM4YjQwZjBhODU0Y2UyNmQ5MmQwYzFlM2IxM2IzYzE0ZWM1OTRm

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
	-u a9572d88240cf1101d8f15d51399ab4bc84064af5f7bb13252e1853813e25332:7433682312bf3db575a1efbe76c8b40f0a854ce26d92d0c1e3b13b3c14ec594f
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
{"grant_type":"client_credentials","client_id":"d400110f0a72ab13c2700764770e8731860fac8dd0517188f7ad12eb5b2a2eb4","client_secret":"e7dbc70faf44adbbb822415cdabf7473937ba037c000ea49ab9c1392d42aacda"}
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
  "access_token": "c8798b4a3919587bef8b4dbf568f7d459b44a5b52c7863eb77b98e01ccd7272e",
  "token_type": "bearer",
  "created_at": 1481231087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"d400110f0a72ab13c2700764770e8731860fac8dd0517188f7ad12eb5b2a2eb4","client_secret":"e7dbc70faf44adbbb822415cdabf7473937ba037c000ea49ab9c1392d42aacda"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"15582b1272c594d3b18a1bab6cdd6d2a981c210cdef53d0e621a07844554cd31","client_secret":"3c43d162d0291504044654a0a0ff572dbbc5c9ba60a3a52cbf7ad87ca0bdaeb2"}
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
  "access_token": "591160e3ef2f27f450895a2ddc1aed91d64811d0e4382547a680b77483aeecad",
  "token_type": "bearer",
  "created_at": 1481231087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"15582b1272c594d3b18a1bab6cdd6d2a981c210cdef53d0e621a07844554cd31","client_secret":"3c43d162d0291504044654a0a0ff572dbbc5c9ba60a3a52cbf7ad87ca0bdaeb2"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZWUzNWE2YzBhOGZiYmU1OTUyNDJkY2M0OWM0MGY3NjBhOTVkOGNhYzhlYTNk
M2ZlYjJhMjMzMWQwZGY5ZDBkYTo1Njg3ZmZhMGIxZTA1MmE4ODQ4MzFkYTA3
NDlkNTA5OTA0OGI1NjRmZGFlMmJkZWUyMDFkZmYyNDBjN2RmMGI5

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
  "access_token": "4f531051a12fd65a195efae3addc69ecb89735beda343b0648ec6fc8e4308ccc",
  "token_type": "bearer",
  "created_at": 1481231087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u ee35a6c0a8fbbe595242dcc49c40f760a95d8cac8ea3d3feb2a2331d0df9d0da:5687ffa0b1e052a884831da0749d5099048b564fdae2bdee201dff240c7df0b9
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
Authorization: Bearer c25007fe9f452673c59e0213dba84a390889c4507001e48ad18d8e8b21c2e852
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
	-H "Authorization: Bearer c25007fe9f452673c59e0213dba84a390889c4507001e48ad18d8e8b21c2e852"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/125/flashcards
Content-Type: application/json
Authorization: Bearer 47c8ad464c4f46410dafed2a06a244b698ba0eae7c927f93fefb043eab65ce5c
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":125,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 70,
    "obfuscated_id": "EDEz1xzotLc",
    "author_id": 696,
    "chapter_id": 125,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:54.142Z",
    "created_at": "2016-12-08T21:04:54.142Z",
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
curl "api.goskive.com/v2/chapters/125/flashcards" -d '{"flashcard":{"chapter_id":125,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47c8ad464c4f46410dafed2a06a244b698ba0eae7c927f93fefb043eab65ce5c"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/123/flashcards
Content-Type: application/json
Authorization: Bearer cade8c85505641ee44c4804dc5723138204527391870a648e49f2fc6d390ccf1
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 688,
      "chapter_id": 123,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:53.662Z",
      "created_at": "2016-12-08T21:04:53.662Z",
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 688,
      "chapter_id": 123,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:53.702Z",
      "created_at": "2016-12-08T21:04:53.702Z",
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
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 688,
      "chapter_id": 123,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:53.742Z",
      "created_at": "2016-12-08T21:04:53.742Z",
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
curl "api.goskive.com/v2/chapters/123/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cade8c85505641ee44c4804dc5723138204527391870a648e49f2fc6d390ccf1"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/18/questions
Content-Type: application/json
Authorization: Bearer b8612cb9c567f07766087c35b17672b2af33381393e0d8e709f98eaf7fa13acb
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":18,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 22,
    "obfuscated_id": "V2ZFfduV4jE",
    "author_id": 101,
    "chapter_id": 18,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:02.663Z",
    "created_at": "2016-12-08T21:04:02.663Z",
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
        "id": 43,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 44,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 45,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 46,
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
curl "api.goskive.com/v2/chapters/18/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":18,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8612cb9c567f07766087c35b17672b2af33381393e0d8e709f98eaf7fa13acb"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/20/questions
Content-Type: application/json
Authorization: Bearer 6272685ac09c04c7b0ce0fd8bb6aa95342685d1b5aab1b7082f6f2253c5cbe6d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":20,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 24,
    "obfuscated_id": "KHM5yo_z4Ds",
    "author_id": 107,
    "chapter_id": 20,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:03.842Z",
    "created_at": "2016-12-08T21:04:03.842Z",
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
        "id": 50,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 51,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/20/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":20,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6272685ac09c04c7b0ce0fd8bb6aa95342685d1b5aab1b7082f6f2253c5cbe6d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/21/questions
Content-Type: application/json
Authorization: Bearer 41eed986b4d8fe9eaa8d1827c4d034d27dd72deb403f696af2882a09c7f6b98f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":21,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 25,
    "obfuscated_id": "HsmcIJXdRE4",
    "author_id": 110,
    "chapter_id": 21,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:04.399Z",
    "created_at": "2016-12-08T21:04:04.399Z",
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
        "id": 52,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 53,
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
curl "api.goskive.com/v2/chapters/21/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":21,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41eed986b4d8fe9eaa8d1827c4d034d27dd72deb403f696af2882a09c7f6b98f"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/19/questions
Content-Type: application/json
Authorization: Bearer 480c67f677cac640ef9dc005fda50dd5318420c2c302f8b85c1d224dc2342215
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":19,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 104,
    "chapter_id": 19,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:03.344Z",
    "created_at": "2016-12-08T21:04:03.344Z",
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
        "id": 47,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 48,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 49,
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
curl "api.goskive.com/v2/chapters/19/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":19,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 480c67f677cac640ef9dc005fda50dd5318420c2c302f8b85c1d224dc2342215"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/22/questions
Content-Type: application/json
Authorization: Bearer a3bd1fc00319246042da4e1a183728a5738c370abe3bbb0104bda559a21bf7d4
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 113,
      "chapter_id": 22,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:05.025Z",
      "created_at": "2016-12-08T21:04:04.932Z",
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
          "id": 54,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 55,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 114,
      "chapter_id": 22,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:05.192Z",
      "created_at": "2016-12-08T21:04:05.095Z",
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
          "id": 56,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 57,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 115,
      "chapter_id": 22,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T21:04:05.360Z",
      "created_at": "2016-12-08T21:04:05.264Z",
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
          "id": 58,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 59,
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
curl "api.goskive.com/v2/chapters/22/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3bd1fc00319246042da4e1a183728a5738c370abe3bbb0104bda559a21bf7d4"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/126
Content-Type: application/json
Authorization: Bearer e02a323491509c28d92af08da80bc021050ace110ac91608b0fe01f397c756f1
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
curl "api.goskive.com/v2/chapters/126" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e02a323491509c28d92af08da80bc021050ace110ac91608b0fe01f397c756f1"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/128
Content-Type: application/json
Authorization: Bearer 79a50465fef9abe43c30883bb35dddf25db3214267519e83064137287e78c38f
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
curl "api.goskive.com/v2/chapters/128" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79a50465fef9abe43c30883bb35dddf25db3214267519e83064137287e78c38f"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/133
Content-Type: application/json
Authorization: Bearer b08adee6581f82becc57549ac035daaf10e74c5c4e204211e865aa4425b77ad8
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
curl "api.goskive.com/v2/chapters/133" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b08adee6581f82becc57549ac035daaf10e74c5c4e204211e865aa4425b77ad8"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/127
Content-Type: application/json
Authorization: Bearer 191491a41afbe08f093186a0adac55343d165b571e4ee1103d29228d690d28a2
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/127" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 191491a41afbe08f093186a0adac55343d165b571e4ee1103d29228d690d28a2"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/131
Content-Type: application/json
Authorization: Bearer 7de44a7a4b7116458e147bcf89b08e5ffa79f8001e23bf3a24462346b4395565
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
    "id": 131,
    "updated_at": "2016-12-08T21:04:56.328Z",
    "course_id": 213,
    "author_id": 717,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-08T21:04:55.835Z",
    "questions_updated_at": "2016-12-08T21:04:55.835Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 721,
        "chapter_id": 131,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:56.309Z",
        "created_at": "2016-12-08T21:04:56.309Z",
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
        "id": 111,
        "obfuscated_id": "G-D-sgMUtTw",
        "author_id": 719,
        "chapter_id": 131,
        "position": 98,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:56.203Z",
        "created_at": "2016-12-08T21:04:56.115Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/131" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7de44a7a4b7116458e147bcf89b08e5ffa79f8001e23bf3a24462346b4395565"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/132
Content-Type: application/json
Authorization: Bearer 916c6e1c3e8c49393b49c319c8572f6ef1214c0b0b4e3fccfd546b3c931320bd
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
    "id": 132,
    "updated_at": "2016-12-08T21:04:56.601Z",
    "course_id": 214,
    "author_id": 724,
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
curl "api.goskive.com/v2/chapters/132" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 916c6e1c3e8c49393b49c319c8572f6ef1214c0b0b4e3fccfd546b3c931320bd"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 9c8bf4132adc95596ff7a57ca1c8d2f189beefaf1dd65426b294a62f774f794e
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
    "id": 3,
    "author_id": 58,
    "reply_to_id": 2,
    "created_at": "2016-12-08T21:03:59.167Z",
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
curl "api.goskive.com/v2/comments/2/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c8bf4132adc95596ff7a57ca1c8d2f189beefaf1dd65426b294a62f774f794e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 0ea3a7a1d37cd27ffb6d02a373de3f7d5a33131b3937683222cd6894375f1c25
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
curl "api.goskive.com/v2/comments/1/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ea3a7a1d37cd27ffb6d02a373de3f7d5a33131b3937683222cd6894375f1c25"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 2ec1ea490409756b385d043ee2799f47f4caf5b1ad2ddf5030c9ab659c26fb30
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
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ec1ea490409756b385d043ee2799f47f4caf5b1ad2ddf5030c9ab659c26fb30"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/12/republish
Content-Type: application/json
Authorization: Bearer 7a28457a37309b5c7f2c76cc060f05c3d7dbc930cfa47e6279e5c77940a10ed2
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
curl "api.goskive.com/v2/comments/12/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a28457a37309b5c7f2c76cc060f05c3d7dbc930cfa47e6279e5c77940a10ed2"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/9
Content-Type: application/json
Authorization: Bearer 562961f1ce6623755cd008da0ce39bb70fa8a33c0c7cdb58e59e6d7e7b36abcb
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 562961f1ce6623755cd008da0ce39bb70fa8a33c0c7cdb58e59e6d7e7b36abcb"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/13/report
Content-Type: application/json
Authorization: Bearer e828247a799c11e96713787607ada64d397ea64637d10788704e264c7c0854c4
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/13/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e828247a799c11e96713787607ada64d397ea64637d10788704e264c7c0854c4"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/39
Content-Type: application/json
Authorization: Bearer 6cc3c3b77a4fbf41317e58af0e0b1346a9a15b994a08ca30da47df4a4ca958fe
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
    "id": 39,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-08T21:05:18.307Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cc3c3b77a4fbf41317e58af0e0b1346a9a15b994a08ca30da47df4a4ca958fe"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer de33a22ebd83a544201906d7d9f2292cdc23edde24721f19c6928e2a6b4f73a1
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
      "id": 36,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T21:05:18.241Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T21:05:18.246Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T21:05:18.250Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de33a22ebd83a544201906d7d9f2292cdc23edde24721f19c6928e2a6b4f73a1"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/7/company_profiles
Content-Type: application/json
Authorization: Bearer 6ffc715c7f31e32a2ae978ea2a4278dea9d5d8fbc1408dd1a22e7184aa991411
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

      ]
    },
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
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/7/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ffc715c7f31e32a2ae978ea2a4278dea9d5d8fbc1408dd1a22e7184aa991411"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/5/company_profiles
Content-Type: application/json
Authorization: Bearer 210058cbc1b6d5b60160b475e984e733695befd142d7d8fcb2df0420eca19ddb
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
      "id": 1,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/0adf1955ecfb39ff0d02f85dd384e7aeaf694927.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/39195f7a12fa003c1584dcee68597ed4a180cb4b.png",
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
curl "api.goskive.com/v2/companies/5/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 210058cbc1b6d5b60160b475e984e733695befd142d7d8fcb2df0420eca19ddb"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 1b496ecd8e272d3911efc80d3f1bbd4190a0bc47f8b1fa11dfcab005602eaaac
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
      "company_id": 33,
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
	-H "Authorization: Bearer 1b496ecd8e272d3911efc80d3f1bbd4190a0bc47f8b1fa11dfcab005602eaaac"
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
Authorization: Bearer 435f42e8b98d493adfc9262d26fb311909d99893e321c24e714aebb07439b6b9
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
	-H "Authorization: Bearer 435f42e8b98d493adfc9262d26fb311909d99893e321c24e714aebb07439b6b9"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7d36e5eda2f105ddd0fe6d80487442bafa312b1006970fb757dc031e4feba57d
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
    "id": 155,
    "updated_at": "2016-12-08T21:05:08.124Z",
    "course_id": 280,
    "author_id": 846,
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
	-H "Authorization: Bearer 7d36e5eda2f105ddd0fe6d80487442bafa312b1006970fb757dc031e4feba57d"
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
      "id": 159,
      "updated_at": "2016-12-08T21:05:08.647Z",
      "course_id": 283,
      "author_id": 855,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 135",
      "position": 1
    },
    {
      "id": 160,
      "updated_at": "2016-12-08T21:05:08.671Z",
      "course_id": 283,
      "author_id": 856,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 136",
      "position": 2
    },
    {
      "id": 161,
      "updated_at": "2016-12-08T21:05:08.885Z",
      "course_id": 283,
      "author_id": 857,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T21:05:08.546Z",
      "questions_updated_at": "2016-12-08T21:05:08.546Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 137",
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
Authorization: Bearer ab6eec31e2d2beea54d7793a0b80de5b8a1447b4ace2ae8650e7e4798c28e1fb
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
      "id": 165,
      "updated_at": "2016-12-08T21:05:09.352Z",
      "course_id": 286,
      "author_id": 866,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 141",
      "position": 1
    },
    {
      "id": 166,
      "updated_at": "2016-12-08T21:05:09.377Z",
      "course_id": 286,
      "author_id": 867,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 142",
      "position": 2
    },
    {
      "id": 167,
      "updated_at": "2016-12-08T21:05:09.593Z",
      "course_id": 286,
      "author_id": 868,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T21:05:09.251Z",
      "questions_updated_at": "2016-12-08T21:05:09.251Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 143",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab6eec31e2d2beea54d7793a0b80de5b8a1447b4ace2ae8650e7e4798c28e1fb"
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
      "id": 162,
      "updated_at": "2016-12-08T21:05:09.040Z",
      "course_id": 284,
      "author_id": 861,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 138",
      "position": 1
    },
    {
      "id": 163,
      "updated_at": "2016-12-08T21:05:09.065Z",
      "course_id": 284,
      "author_id": 862,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 139",
      "position": 2
    },
    {
      "id": 164,
      "updated_at": "2016-12-08T21:05:09.089Z",
      "course_id": 284,
      "author_id": 863,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 140",
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
Authorization: Bearer c25439d626ba529c28dec7df030e6a2b331a5dc485ad7cd4a8a93f1e7dca5efe
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
      "id": 168,
      "updated_at": "2016-12-08T21:05:09.921Z",
      "course_id": 288,
      "author_id": 875,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 144",
      "position": 1
    },
    {
      "id": 169,
      "updated_at": "2016-12-08T21:05:09.945Z",
      "course_id": 288,
      "author_id": 876,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 145",
      "position": 2
    },
    {
      "id": 170,
      "updated_at": "2016-12-08T21:05:09.969Z",
      "course_id": 288,
      "author_id": 877,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 146",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c25439d626ba529c28dec7df030e6a2b331a5dc485ad7cd4a8a93f1e7dca5efe"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer bdf2904f4422e63846f7e7ae3a73d23e26f1b8c57ad1ce55bc250d3b364789de
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
    "id": 5,
    "course_id": 179,
    "user_id": 605,
    "updated_at": "2016-12-08T21:04:48.204Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdf2904f4422e63846f7e7ae3a73d23e26f1b8c57ad1ce55bc250d3b364789de"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer a601ed9d4677d0d53619b2d44fe24f2ba060923bc16504d6c3f0a9aa7f40802a
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
      "course_id": 178,
      "user_id": 601,
      "updated_at": "2016-12-08T21:04:47.976Z"
    },
    {
      "id": 4,
      "course_id": 178,
      "user_id": 602,
      "updated_at": "2016-12-08T21:04:47.992Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a601ed9d4677d0d53619b2d44fe24f2ba060923bc16504d6c3f0a9aa7f40802a"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/268/files
Content-Type: application/json
Authorization: Bearer 2995685a0e8d57313dd6e003362cd6f3796368ccd5fd133382c34540b3112c2f
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
        "id": 819,
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
        "created_at": "2016-12-08T21:05:05.907Z",
        "updated_at": "2016-12-08T21:05:05.907Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T21:05:05.917Z",
      "updated_at": "2016-12-08T21:05:05.917Z",
      "course_id": 268,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 20,
      "uploader": {
        "id": 820,
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
        "created_at": "2016-12-08T21:05:05.926Z",
        "updated_at": "2016-12-08T21:05:05.926Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T21:05:05.936Z",
      "updated_at": "2016-12-08T21:05:05.936Z",
      "course_id": 268,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 821,
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
        "created_at": "2016-12-08T21:05:05.947Z",
        "updated_at": "2016-12-08T21:05:05.947Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T21:05:05.956Z",
      "updated_at": "2016-12-08T21:05:05.956Z",
      "course_id": 268,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/268/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2995685a0e8d57313dd6e003362cd6f3796368ccd5fd133382c34540b3112c2f"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/270/files
Content-Type: application/json
Authorization: Bearer ef4cee8f8722c73fa339c5ae4eea2fa52d93c4d5b6eba9e3e20384cebff78e4d
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
      "id": 826,
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
      "created_at": "2016-12-08T21:05:06.252Z",
      "updated_at": "2016-12-08T21:05:06.252Z"
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
    "created_at": "2016-12-08T21:05:06.284Z",
    "updated_at": "2016-12-08T21:05:06.284Z",
    "course_id": 270,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/270/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef4cee8f8722c73fa339c5ae4eea2fa52d93c4d5b6eba9e3e20384cebff78e4d"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/271/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 97a110d16ef99ccfd2587e34bb22963b41a9886046168f1b81377357c48a9c91
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
    "key": "cache/40105a4a82132207adc60aa3c94e2384.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQyMjowNTowNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzQwMTA1YTRhODIxMzIyMDdhZGM2MGFhM2M5NGUyMzg0LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA4VDIxMDUwNloifV19",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T210506Z",
    "x-amz-signature": "672eda6a762e73379d7a2586e63dec7bffab6ab6a1a5f55f462ceed76962fa45"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/271/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97a110d16ef99ccfd2587e34bb22963b41a9886046168f1b81377357c48a9c91"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 07e4779b89a8ee2dc749ff8912cda3af8d7fc95fd7245ba417e39f7af89ea4d2
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
	-H "Authorization: Bearer 07e4779b89a8ee2dc749ff8912cda3af8d7fc95fd7245ba417e39f7af89ea4d2"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 548f8c5a28c8963d75c082a7b8296df0685ba589cf1acd1ce1bf107e36e8949b
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
	-H "Authorization: Bearer 548f8c5a28c8963d75c082a7b8296df0685ba589cf1acd1ce1bf107e36e8949b"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a6b2838d88de356cd8ee338474d20011c7b524fb9c1d3fad58bb8078b5a8c766
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
	-H "Authorization: Bearer a6b2838d88de356cd8ee338474d20011c7b524fb9c1d3fad58bb8078b5a8c766"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f625ba390566c34d43eb43beb20cd8ee93f6a9edbac854618172aa1c0a4ff2ab
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
	-H "Authorization: Bearer f625ba390566c34d43eb43beb20cd8ee93f6a9edbac854618172aa1c0a4ff2ab"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d792a67f0a2e48ea81e1718936816b9084af506110d33f2b56c6402ecbd3f357
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
	-H "Authorization: Bearer d792a67f0a2e48ea81e1718936816b9084af506110d33f2b56c6402ecbd3f357"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 21a98e179a44ae580a5c002f23b493adfe54091a57a4998390ca1131175ae8bc
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
    "creator_id": 126,
    "id": 30,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 31,
    "additional_university_ids": [

    ],
    "discipline_id": 32,
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
    "chapters_updated_at": "2016-12-08T21:04:07.173Z",
    "updated_at": "2016-12-08T21:04:08.549Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 127,
        "chapter_id": 26,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:08.317Z",
        "created_at": "2016-12-08T21:04:08.317Z",
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
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 127,
        "chapter_id": 27,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:08.397Z",
        "created_at": "2016-12-08T21:04:08.397Z",
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
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 127,
        "chapter_id": 26,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:08.362Z",
        "created_at": "2016-12-08T21:04:08.362Z",
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
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 127,
        "chapter_id": 27,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:08.443Z",
        "created_at": "2016-12-08T21:04:08.443Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 127,
        "chapter_id": 26,
        "position": 31,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:07.412Z",
        "created_at": "2016-12-08T21:04:07.315Z",
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
        "author_id": 127,
        "chapter_id": 26,
        "position": 32,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:07.586Z",
        "created_at": "2016-12-08T21:04:07.500Z",
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
      },
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 127,
        "chapter_id": 27,
        "position": 33,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:07.766Z",
        "created_at": "2016-12-08T21:04:07.669Z",
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
            "id": 76,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 77,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 127,
        "chapter_id": 27,
        "position": 34,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:07.919Z",
        "created_at": "2016-12-08T21:04:07.830Z",
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
            "id": 78,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 79,
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
        "id": 26,
        "updated_at": "2016-12-08T21:04:08.496Z",
        "course_id": 30,
        "author_id": 126,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T21:04:07.173Z",
        "questions_updated_at": "2016-12-08T21:04:07.173Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 20",
        "position": 1
      },
      {
        "id": 27,
        "updated_at": "2016-12-08T21:04:08.538Z",
        "course_id": 30,
        "author_id": 126,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T21:04:07.173Z",
        "questions_updated_at": "2016-12-08T21:04:07.173Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 21",
        "position": 2
      }
    ],
    "topic_id": 32,
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
	-H "Authorization: Bearer 21a98e179a44ae580a5c002f23b493adfe54091a57a4998390ca1131175ae8bc"
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
    "creator_id": 132,
    "id": 31,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 32,
    "additional_university_ids": [

    ],
    "discipline_id": 33,
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
    "chapters_updated_at": "2016-12-08T21:04:08.707Z",
    "updated_at": "2016-12-08T21:04:10.066Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 132,
        "chapter_id": 28,
        "position": 37,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:08.925Z",
        "created_at": "2016-12-08T21:04:08.828Z",
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
            "id": 84,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 85,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 132,
        "chapter_id": 29,
        "position": 39,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T21:04:09.272Z",
        "created_at": "2016-12-08T21:04:09.167Z",
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
            "id": 88,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 89,
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
        "id": 28,
        "updated_at": "2016-12-08T21:04:10.009Z",
        "course_id": 31,
        "author_id": 132,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T21:04:08.707Z",
        "questions_updated_at": "2016-12-08T21:04:08.707Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 22",
        "position": 1
      },
      {
        "id": 29,
        "updated_at": "2016-12-08T21:04:10.055Z",
        "course_id": 31,
        "author_id": 132,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T21:04:08.707Z",
        "questions_updated_at": "2016-12-08T21:04:08.707Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 23",
        "position": 2
      }
    ],
    "topic_id": 33,
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
PUT /v2/courses/33/pin
Content-Type: application/json
Authorization: Bearer 303300829aca5bada870984b4fd24242ef88bf6fea76614685f1e2a72a55c295
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/33/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 303300829aca5bada870984b4fd24242ef88bf6fea76614685f1e2a72a55c295"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/47/pin
Content-Type: application/json
Authorization: Bearer 96201f1a6e70df055429acc5f354c51361c78ad212aeeb8a0e53b64b1853a98a
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/47/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96201f1a6e70df055429acc5f354c51361c78ad212aeeb8a0e53b64b1853a98a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 876096befb07cf05e89fdf1b9deff5dc27c8765536ee5cc9f3f7e009b5347bfc
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
    "creator_id": 169,
    "id": 45,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 46,
    "additional_university_ids": [

    ],
    "discipline_id": 47,
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
    "updated_at": "2016-12-08T21:04:14.049Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 47,
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
	-H "Authorization: Bearer 876096befb07cf05e89fdf1b9deff5dc27c8765536ee5cc9f3f7e009b5347bfc"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1490be0805224ff0a9ef561ad0ef47a02ba8a36844ae22ce1397438989d80831
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
    "id": 214,
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
    "created_at": "2016-12-08T21:04:19.701Z",
    "updated_at": "2016-12-08T21:04:19.701Z",
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
	-H "Authorization: Bearer 1490be0805224ff0a9ef561ad0ef47a02ba8a36844ae22ce1397438989d80831"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7d31eeb4d2aee7a367e5d0059249e8cb20d0a946d451dc56d884bf87f6e9f3e4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[57]}
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
    "id": 209,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      57
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T21:04:19.050Z",
    "updated_at": "2016-12-08T21:04:19.104Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[57]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d31eeb4d2aee7a367e5d0059249e8cb20d0a946d451dc56d884bf87f6e9f3e4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 77cd4be15a4d876fb31225c342842132be073cbe959ef76a837683a3c12af5f0
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
    "id": 210,
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
    "created_at": "2016-12-08T21:04:19.134Z",
    "updated_at": "2016-12-08T21:04:19.134Z",
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
	-H "Authorization: Bearer 77cd4be15a4d876fb31225c342842132be073cbe959ef76a837683a3c12af5f0"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 129a3c887152f31f40c45d2111037c8db557854902c4a833274f3b57d8840070
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[59]}
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
    "id": 211,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      59
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T21:04:19.229Z",
    "updated_at": "2016-12-08T21:04:19.229Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[59]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 129a3c887152f31f40c45d2111037c8db557854902c4a833274f3b57d8840070"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer c661a71c80c8e37158a34071652c59eb9f8ce2e869d25b645f1fbf3ad689d0cd
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

61
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
    "id": 213,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0c2820cb02e601a8f0d34ed3bdb0f84d8bb0fc38.jpg",
    "university_id": null,
    "fields_of_study": [
      61
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T21:04:19.381Z",
    "updated_at": "2016-12-08T21:04:19.667Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/61b3cdacacc408bd39e5ff773b2c9606a155080c.jpg",
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

61
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer c661a71c80c8e37158a34071652c59eb9f8ce2e869d25b645f1fbf3ad689d0cd"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 258d7983cd26f56871e832aac795a950516685fd06f20ac62692f470b0b71cad
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
      "bookmarkable_id": 103,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 104,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 105,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 258d7983cd26f56871e832aac795a950516685fd06f20ac62692f470b0b71cad"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer dad27ce4dcdd1f78483c625f272cd9b2dd0996abd364f21f2c2eba722887bf64
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
      "id": 3,
      "title": "Campaign 2",
      "company_id": 20,
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 21,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 8,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/4e8ccb4fdbb03332710724b7199bfb925ebb8588.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/1751c1fcb04de04c20e97d74547e239755abd978.png",
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
	-H "Authorization: Bearer dad27ce4dcdd1f78483c625f272cd9b2dd0996abd364f21f2c2eba722887bf64"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer c6c5fcc163f45be99e5b09ed7be13c6e1a09d997409b3459742110854fe49173
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
      "creator_id": 935,
      "id": 304,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-232",
      "html_url": "https://goskive.com/course/mit-course-232",
      "slug": "mit-course-232",
      "university_id": 289,
      "additional_university_ids": [

      ],
      "discipline_id": 314,
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
      "updated_at": "2016-12-08T21:05:14.509Z",
      "shortname": "mit-course-232",
      "topic_id": 314,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 232",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 936,
      "id": 305,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-233",
      "html_url": "https://goskive.com/course/mit-course-233",
      "slug": "mit-course-233",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "discipline_id": 315,
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
      "updated_at": "2016-12-08T21:05:14.614Z",
      "shortname": "mit-course-233",
      "topic_id": 315,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 233",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6c5fcc163f45be99e5b09ed7be13c6e1a09d997409b3459742110854fe49173"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 9087a6fefb5a94b297873e1a778c973dc2005603bb1571be410ef1fe8607cf8f
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
        "id": 3,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T21:04:19.845Z",
        "updated_at": "2016-12-08T21:04:19.845Z",
        "file_url": "memory://4494278f5a2b3bf1c265d8ef3385f045.pdf",
        "course_id": 55,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 4,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T21:04:19.950Z",
        "updated_at": "2016-12-08T21:04:19.950Z",
        "file_url": "memory://ac2668067193e2d3c8e536fa24798646.pdf",
        "course_id": 56,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 5,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T21:04:20.055Z",
        "updated_at": "2016-12-08T21:04:20.055Z",
        "file_url": "memory://21e133057bc022c868831c8cba842b10.pdf",
        "course_id": 57,
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
	-H "Authorization: Bearer 9087a6fefb5a94b297873e1a778c973dc2005603bb1571be410ef1fe8607cf8f"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 11e6b2ae8619c817139a4d8750428f9b94c913775be125d514d4b0334c8b8dca
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
      "created_at": "2016-12-08T21:04:00.209Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 5,
      "updated_at": "2016-12-08T21:04:00.337Z",
      "author_id": "72",
      "thread_subject_id": "15",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 4,
      "created_at": "2016-12-08T21:04:00.326Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-12-08T21:04:00.340Z",
      "author_id": "75",
      "thread_subject_id": "16",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-12-08T21:04:00.706Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-12-08T21:04:00.706Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-12-08T21:04:01.067Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 6,
      "updated_at": "2016-12-08T21:04:01.067Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 7,
      "created_at": "2016-12-08T21:04:01.437Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-12-08T21:04:01.437Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 8,
      "created_at": "2016-12-08T21:04:01.757Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 19,
      "updated_at": "2016-12-08T21:04:01.757Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-12-08T21:04:02.053Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-12-08T21:04:02.053Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-12-08T21:04:02.349Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 21,
      "updated_at": "2016-12-08T21:04:02.349Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11e6b2ae8619c817139a4d8750428f9b94c913775be125d514d4b0334c8b8dca"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/2
Content-Type: application/json
Authorization: Bearer c5598355a828d49c2989ee3e248c56a2d06cf197a48c21ab5a002fdc06f01456
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-08T20:53:59.000Z"}}
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
    "created_at": "2016-12-08T21:04:00.034Z",
    "read_at": "2016-12-08T20:53:59.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 4,
    "updated_at": "2016-12-08T21:04:00.082Z",
    "author_id": "68",
    "thread_subject_id": "14",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/2" -d '{"notification":{"read_at":"2016-12-08T20:53:59.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5598355a828d49c2989ee3e248c56a2d06cf197a48c21ab5a002fdc06f01456"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1ee4aa2077fb5705e4b53a799ed11a452faf27bcfe496115d07ffb47b33c9d54
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
      "course_id": 102,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T21:04:32.229Z",
      "course_published": true,
      "updated_at": "2016-12-08T21:04:32.223Z"
    },
    {
      "id": 5,
      "course_id": 103,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T21:04:32.340Z",
      "course_published": true,
      "updated_at": "2016-12-08T21:04:32.335Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee4aa2077fb5705e4b53a799ed11a452faf27bcfe496115d07ffb47b33c9d54"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 142ee43ebef5989218ad7991135b04b17f78dd22133494a59d0b295514fff117
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
    "course_id": 101,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T21:04:32.074Z",
    "course_published": true,
    "updated_at": "2016-12-08T21:04:32.069Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 142ee43ebef5989218ad7991135b04b17f78dd22133494a59d0b295514fff117"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 39f2619cad474ed51e0c95965d190a6e09ac3230d4684551bcb531d90d7ba4c7
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
    "course_id": 100,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-08T21:04:31.944Z",
    "course_published": true,
    "updated_at": "2016-12-08T21:04:31.934Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39f2619cad474ed51e0c95965d190a6e09ac3230d4684551bcb531d90d7ba4c7"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 8a2df1ab0e4bda4263c08cb0d6df8032de1d8584a61f313e3f52f8abe2e4aacf
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
      "votable_id": 9,
      "user_id": 28
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 10,
      "user_id": 28
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 11,
      "user_id": 28
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 12,
      "user_id": 28
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a2df1ab0e4bda4263c08cb0d6df8032de1d8584a61f313e3f52f8abe2e4aacf"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/327
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
    "id": 327,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 327,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 327
      },
      {
        "id": 328,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 327
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/327" -X GET \
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
      "id": 328,
      "name": "Multi-tiered demand-driven strategy",
      "name_translations": {
        "en": "Multi-tiered demand-driven strategy"
      }
    },
    {
      "id": 329,
      "name": "Enterprise-wide leading edge firmware",
      "name_translations": {
        "en": "Enterprise-wide leading edge firmware"
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
PATCH /v2/feedbacks/25/close
Content-Type: application/json
Authorization: Bearer 313e6275bd6e33e6bf30a3f646f94b94ba72c16c4de589ee86e97aa7fa1cdeca
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
    "id": 25,
    "user_id": 331,
    "feedbackable_id": 39,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-08T21:04:28.111Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 313e6275bd6e33e6bf30a3f646f94b94ba72c16c4de589ee86e97aa7fa1cdeca"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/2/fix
Content-Type: application/json
Authorization: Bearer c24c3c28d98ce64c4e9f414277b8f9d187d201e1a47e76cde86d748b04d59a29
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
    "id": 2,
    "user_id": 230,
    "feedbackable_id": 35,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-08T21:04:20.791Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c24c3c28d98ce64c4e9f414277b8f9d187d201e1a47e76cde86d748b04d59a29"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/27
Content-Type: application/json
Authorization: Bearer 5abb15123cbfcf722f6ba63cb0f820caea7a03e333933835458e3d23f3b69e48
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
    "user_id": 341,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T21:04:28.886Z",
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
	-H "Authorization: Bearer 5abb15123cbfcf722f6ba63cb0f820caea7a03e333933835458e3d23f3b69e48"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/fix
Content-Type: application/json
Authorization: Bearer 921bda519401efb2cb5bd79cf8a980a8209056a2e250e6ddc4dca9c314007cd1
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
curl "api.goskive.com/v2/feedbacks/3/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 921bda519401efb2cb5bd79cf8a980a8209056a2e250e6ddc4dca9c314007cd1"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer bedb57b155aab99b23b461e468266230a482d8f78793a3db5cdb496f1e0c87f0
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
	-H "Authorization: Bearer bedb57b155aab99b23b461e468266230a482d8f78793a3db5cdb496f1e0c87f0"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/close
Content-Type: application/json
Authorization: Bearer ba11d01ffad7b7517391fe8db1dcbab8a57b12d8ea46e4d03a622f2bbfd24906
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
curl "api.goskive.com/v2/feedbacks/24/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba11d01ffad7b7517391fe8db1dcbab8a57b12d8ea46e4d03a622f2bbfd24906"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer f7c63fe1783404e915885fd1367d724e2dc640330ec0523a807445ff680d37f0
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
    "user_id": 346,
    "feedbackable_id": 42,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T21:04:29.243Z",
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
	-H "Authorization: Bearer f7c63fe1783404e915885fd1367d724e2dc640330ec0523a807445ff680d37f0"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 949baf5c554b838fd49e46f3f6b3bb0ebd782f54ee3aaf4ffa424b44b27fba0b
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
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 949baf5c554b838fd49e46f3f6b3bb0ebd782f54ee3aaf4ffa424b44b27fba0b"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/8/bookmark
Content-Type: application/json
Authorization: Bearer 0fdb044577c82a7f4dae5d0dd335fe99e1d614f18eeec4d2529a16ee0a1a9ed5
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fdb044577c82a7f4dae5d0dd335fe99e1d614f18eeec4d2529a16ee0a1a9ed5"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer fc240634dec4c42ab05e54ef9920bd4b3e3777e3ae6b93a2afffffeaa01d9d8e
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
	-H "Authorization: Bearer fc240634dec4c42ab05e54ef9920bd4b3e3777e3ae6b93a2afffffeaa01d9d8e"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/18
Content-Type: application/json
Authorization: Bearer d253ef34327ffbb67a615d4d462a750f75c3ca51ebfb06111e5b256b15b72ebc
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/9256d0451aa0338c9a24b485e3c71a41.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T210431Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=33e523207f04346acff6a5fedbc2b12b9c1a8765f110e971674a3dd1463b0703",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d253ef34327ffbb67a615d4d462a750f75c3ca51ebfb06111e5b256b15b72ebc"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/9/preview
Content-Type: application/json
Authorization: Bearer 95e735c3a443c3fc466ac055bd34e2f0c574ff4606fb05998f10bb79e048d0eb
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5398d7645aacf8c1b64154aca692c241.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T210429Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b57c41e05cc624edde7b0e4337f8b91913e1207c36d5a8705fda903ef19987b0",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/9/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95e735c3a443c3fc466ac055bd34e2f0c574ff4606fb05998f10bb79e048d0eb"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer 56130d5fa103c2dc907abfed1a93c47f76e6a0289aeaacb665a20b320dcee09b
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
    "id": 13,
    "uploader": {
      "id": 371,
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
      "created_at": "2016-12-08T21:04:30.844Z",
      "updated_at": "2016-12-08T21:04:30.844Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-08T21:04:30.944Z",
    "updated_at": "2016-12-08T21:04:30.944Z",
    "course_id": 94,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56130d5fa103c2dc907abfed1a93c47f76e6a0289aeaacb665a20b320dcee09b"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer dbd1e28590e49ad47d78417f1c2a67d4933942f612e25e9151f10fe4c2a22270
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
      "creator_id": 11,
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 3,
      "additional_university_ids": [

      ],
      "discipline_id": 3,
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
      "chapters_updated_at": "2016-12-08T21:03:51.652Z",
      "updated_at": "2016-12-08T21:03:54.411Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 3,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 16,
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-75b17643-a533-437a-87b6-9d91442be276",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-75b17643-a533-437a-87b6-9d91442be276",
      "slug": "mit-the-great-british-bake-off-75b17643-a533-437a-87b6-9d91442be276",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "discipline_id": 4,
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
      "chapters_updated_at": "2016-12-08T21:03:51.652Z",
      "updated_at": "2016-12-08T21:03:54.887Z",
      "shortname": "mit-the-great-british-bake-off-75b17643-a533-437a-87b6-9d91442be276",
      "topic_id": 4,
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
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer dbd1e28590e49ad47d78417f1c2a67d4933942f612e25e9151f10fe4c2a22270"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/10/download
Content-Type: application/json
Authorization: Bearer fefc63aa7055bb764c2d5cfc84faea97400b74a111eb00bdb9b5bb1d266eff48
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fefc63aa7055bb764c2d5cfc84faea97400b74a111eb00bdb9b5bb1d266eff48"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer a6c7c38e9816d7456dce45f77126ea76414944a97d82a48ee2d5a98d5f843fb9
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
	-H "Authorization: Bearer a6c7c38e9816d7456dce45f77126ea76414944a97d82a48ee2d5a98d5f843fb9"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/7/bookmark
Content-Type: application/json
Authorization: Bearer 07858743555258808653fd4ab4d8874bdaa725feb5f9d13888cdbd9c067f542a
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07858743555258808653fd4ab4d8874bdaa725feb5f9d13888cdbd9c067f542a"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/6/upvote
Content-Type: application/json
Authorization: Bearer b3a77bd2b68c9057703e07bd635f4c6301a689376c5f043b88d100b1a5d0f5fd
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
	-H "Authorization: Bearer b3a77bd2b68c9057703e07bd635f4c6301a689376c5f043b88d100b1a5d0f5fd"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/82/comments
Content-Type: application/json
Authorization: Bearer f9c4caaff6e21abc1966b8e259d179408dfca022397d2ada0c4b1fcc47587ba1
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
    "id": 50,
    "author_id": 789,
    "reply_to_id": null,
    "created_at": "2016-12-08T21:05:03.084Z",
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
curl "api.goskive.com/v2/flashcards/82/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9c4caaff6e21abc1966b8e259d179408dfca022397d2ada0c4b1fcc47587ba1"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/81/comments
Content-Type: application/json
Authorization: Bearer 25268a7c6bc27ec6a9f52a1907bbc02100a20ec75ea273561f5227c4684bc4ff
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
    "id": 49,
    "author_id": 786,
    "reply_to_id": null,
    "created_at": "2016-12-08T21:05:02.690Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 29,
      "user_id": 786,
      "feedbackable_id": 81,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:02.687Z",
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
curl "api.goskive.com/v2/flashcards/81/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25268a7c6bc27ec6a9f52a1907bbc02100a20ec75ea273561f5227c4684bc4ff"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/83/comments
Content-Type: application/json
Authorization: Bearer b692a95eb4a018337fc2ca2f62736ecd66bbc7762dd4da1befdd1a138d75bb54
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
      "id": 51,
      "author_id": 795,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:05:03.425Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 796,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:05:03.441Z",
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
curl "api.goskive.com/v2/flashcards/83/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b692a95eb4a018337fc2ca2f62736ecd66bbc7762dd4da1befdd1a138d75bb54"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/80/comments
Content-Type: application/json
Authorization: Bearer c63a7f69cc117e0087956bdd4f4e152a1123e63ed63c13a6e81c601e36e3b7a0
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
curl "api.goskive.com/v2/flashcards/80/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c63a7f69cc117e0087956bdd4f4e152a1123e63ed63c13a6e81c601e36e3b7a0"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/94/feedbacks
Content-Type: application/json
Authorization: Bearer 0eac5ffa6afbe58c932cadc14fe9c17258976db6b0c3bfada333d074eff21350
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
    "id": 45,
    "user_id": 968,
    "feedbackable_id": 94,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T21:05:16.232Z",
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
curl "api.goskive.com/v2/flashcards/94/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0eac5ffa6afbe58c932cadc14fe9c17258976db6b0c3bfada333d074eff21350"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/93/feedbacks
Content-Type: application/json
Authorization: Bearer 6198ba377fa3c9877439bf6774145dfbb5999925dc684ab7a3f99472346b788f
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
      "user_id": 967,
      "feedbackable_id": 93,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:16.000Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 966,
      "feedbackable_id": 93,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:15.990Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/93/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6198ba377fa3c9877439bf6774145dfbb5999925dc684ab7a3f99472346b788f"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/32/votes
Content-Type: application/json
Authorization: Bearer c15157be99b03d8e3b1b862893d261062c1ab92925b054aab28d930f7fe7611b
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
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 32,
      "user_id": 190
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 32,
      "user_id": 189
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 32,
      "user_id": 188
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/32/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c15157be99b03d8e3b1b862893d261062c1ab92925b054aab28d930f7fe7611b"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/43/republish
Content-Type: application/json
Authorization: Bearer 4e70809b764996d9e95d36a7c0b59255a781d105ff70de3275d67f9b29050305
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
curl "api.goskive.com/v2/flashcards/43/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e70809b764996d9e95d36a7c0b59255a781d105ff70de3275d67f9b29050305"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/bookmark
Content-Type: application/json
Authorization: Bearer 1d361155a78a38be0a281d95c08388acbb36ae6cd54fb2695a9a77a300a895d6
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d361155a78a38be0a281d95c08388acbb36ae6cd54fb2695a9a77a300a895d6"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/65
Content-Type: application/json
Authorization: Bearer 501d0f13f9f815690270b0c15621ad7936bf2b91fe08d3f5ebd92c3ebe4cd8bc
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 501d0f13f9f815690270b0c15621ad7936bf2b91fe08d3f5ebd92c3ebe4cd8bc"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/45/downvote
Content-Type: application/json
Authorization: Bearer 9a4acc23d17bc9383d4da9c129d0e40f64ad34e9525b880df6520c968096f869
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/45/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a4acc23d17bc9383d4da9c129d0e40f64ad34e9525b880df6520c968096f869"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/62
Content-Type: application/json
Authorization: Bearer f6340bd15b546672f1395c28197da9d3c7e2c492e1cb06c31c14994f30cbd040
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
    "author_id": 673,
    "chapter_id": 118,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:52.346Z",
    "created_at": "2016-12-08T21:04:52.346Z",
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
	-H "Authorization: Bearer f6340bd15b546672f1395c28197da9d3c7e2c492e1cb06c31c14994f30cbd040"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/66/report
Content-Type: application/json
Authorization: Bearer 4780bc5898ca1450c8b6cdab51cd4974d7442720b052656270dbcf2279dafe23
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4780bc5898ca1450c8b6cdab51cd4974d7442720b052656270dbcf2279dafe23"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/46/bookmark
Content-Type: application/json
Authorization: Bearer b9087fd7a8b0125cfe489b9ab44b57ab6f5f5b445ec523060fea29bca2f906f0
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/46/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9087fd7a8b0125cfe489b9ab44b57ab6f5f5b445ec523060fea29bca2f906f0"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/upvote
Content-Type: application/json
Authorization: Bearer ea03114fab5e6f1855d2fbec1123a66e3cdf5def9aa1920d9e937e863d5ed679
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea03114fab5e6f1855d2fbec1123a66e3cdf5def9aa1920d9e937e863d5ed679"
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
    "key": "cache/03fc5103225fa8e50a52938539bbb657.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQyMjowNDozMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzAzZmM1MTAzMjI1ZmE4ZTUwYTUyOTM4NTM5YmJiNjU3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDhUMjEwNDMxWiJ9XX0=",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T210431Z",
    "x-amz-signature": "56420fdf92813179293a29aa4ab632046fdbf660b9f8268a089c0a6445d68473"
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
Authorization: Bearer 5e5b8b398b2e958a80a4fc048646d71e476c79fc586b2deb4118481b217c1aff
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
	-H "Authorization: Bearer 5e5b8b398b2e958a80a4fc048646d71e476c79fc586b2deb4118481b217c1aff"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 4288e58c5dd135888768cc132e37f15635ae99d91d851d21c9044001c91c7c92
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
	-H "Authorization: Bearer 4288e58c5dd135888768cc132e37f15635ae99d91d851d21c9044001c91c7c92"
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
{"password":{"reset_password_token":"j5sxHnkgtUYKPsEfDuh6","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 176,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-08T21:04:14.862Z",
  "updated_at": "2016-12-08T21:04:15.032Z",
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
  "audit_id": 7477
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"j5sxHnkgtUYKPsEfDuh6","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/120/comments
Content-Type: application/json
Authorization: Bearer d5801b0c368e1fa2c601a9a2d2d0b191b3660aaf6dda22652b4fdda1366d2017
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
    "id": 56,
    "author_id": 814,
    "reply_to_id": null,
    "created_at": "2016-12-08T21:05:05.391Z",
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
curl "api.goskive.com/v2/questions/120/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5801b0c368e1fa2c601a9a2d2d0b191b3660aaf6dda22652b4fdda1366d2017"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/119/comments
Content-Type: application/json
Authorization: Bearer 272820b5bf831ca80ecdcc4c6b4e05b1820ccb6a9073c9705b1ddbd9a32bf559
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
    "id": 55,
    "author_id": 811,
    "reply_to_id": null,
    "created_at": "2016-12-08T21:05:04.921Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 30,
      "user_id": 811,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:04.919Z",
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
curl "api.goskive.com/v2/questions/119/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 272820b5bf831ca80ecdcc4c6b4e05b1820ccb6a9073c9705b1ddbd9a32bf559"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/117/comments
Content-Type: application/json
Authorization: Bearer fb387b24f56fdd8f17829cb9a59d805e95eb25464d26b2503fd201b24b151518
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
      "id": 54,
      "author_id": 807,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:05:04.275Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 806,
      "reply_to_id": null,
      "created_at": "2016-12-08T21:05:04.259Z",
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
curl "api.goskive.com/v2/questions/117/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb387b24f56fdd8f17829cb9a59d805e95eb25464d26b2503fd201b24b151518"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/118/comments
Content-Type: application/json
Authorization: Bearer a37c2f8f8973e2be474bec531a418a327c8cadbcb6bb6db0e91c9931afcb1243
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
curl "api.goskive.com/v2/questions/118/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a37c2f8f8973e2be474bec531a418a327c8cadbcb6bb6db0e91c9931afcb1243"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/130/feedbacks
Content-Type: application/json
Authorization: Bearer 51c68947b64c427c4019eec32bff0bce3917f96132abb1a57418ed6425b977d9
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
    "user_id": 923,
    "feedbackable_id": 130,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-08T21:05:13.133Z",
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
curl "api.goskive.com/v2/questions/130/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51c68947b64c427c4019eec32bff0bce3917f96132abb1a57418ed6425b977d9"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/127/feedbacks
Content-Type: application/json
Authorization: Bearer 609f15247aba0921a1a7dc572026f7f8e3324313c853c6d249f3a9aa0f27fa8b
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
      "user_id": 914,
      "feedbackable_id": 127,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:12.183Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 913,
      "feedbackable_id": 127,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T21:05:12.172Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/127/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 609f15247aba0921a1a7dc572026f7f8e3324313c853c6d249f3a9aa0f27fa8b"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/57/votes
Content-Type: application/json
Authorization: Bearer 6ee1bbec3024b58f125f3bfcdd332166b40b43a90d0cf0b71cc3922e002aa428
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
      "votable_id": 57,
      "user_id": 205
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 204
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 203
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/57/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ee1bbec3024b58f125f3bfcdd332166b40b43a90d0cf0b71cc3922e002aa428"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/99/republish
Content-Type: application/json
Authorization: Bearer 892d55d1db7b4715c2f55512a7922c755f527d81cbf8daacff9968077e0c532d
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
curl "api.goskive.com/v2/questions/99/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 892d55d1db7b4715c2f55512a7922c755f527d81cbf8daacff9968077e0c532d"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/100/bookmark
Content-Type: application/json
Authorization: Bearer 13200aef6b7ab231b15a5bcbe00ec726c7968748ce1e316bfc40482af1df25dd
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/100/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13200aef6b7ab231b15a5bcbe00ec726c7968748ce1e316bfc40482af1df25dd"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/79
Content-Type: application/json
Authorization: Bearer bbfe12aed0f758e4dbf2e199cee2c5b16b24eca1292d20a278e661ecca39c817
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/79" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbfe12aed0f758e4dbf2e199cee2c5b16b24eca1292d20a278e661ecca39c817"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/97/downvote
Content-Type: application/json
Authorization: Bearer 18a9d8faf1648140e0a54b436dd7607dcd04a9e613bd21b672a4151054c637b4
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/97/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18a9d8faf1648140e0a54b436dd7607dcd04a9e613bd21b672a4151054c637b4"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/102
Content-Type: application/json
Authorization: Bearer 18dafadff31a7b829afefbd25b855b7fd274d2f4b5113bc51aa9ac125ba62820
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
    "id": 102,
    "obfuscated_id": "jFy90P7ldB4",
    "author_id": 476,
    "chapter_id": 95,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:40.785Z",
    "created_at": "2016-12-08T21:04:40.702Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/102" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18dafadff31a7b829afefbd25b855b7fd274d2f4b5113bc51aa9ac125ba62820"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/80/report
Content-Type: application/json
Authorization: Bearer f1ef72086ff3c3aa9540a4d9264c5874dc001845d00156d237052c7b54c556c0
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/80/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1ef72086ff3c3aa9540a4d9264c5874dc001845d00156d237052c7b54c556c0"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/96/bookmark
Content-Type: application/json
Authorization: Bearer 5eb1b5e60a63b747cc420d75e3490164b0eba89fa520dac5e6729835d94bb37a
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/96/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5eb1b5e60a63b747cc420d75e3490164b0eba89fa520dac5e6729835d94bb37a"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/78
Content-Type: application/json
Authorization: Bearer 51b3a091f0add351eac1c202f0c8afaf3ec76830bbeb748347fe8a094737ba9a
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":78,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T21:04:32.854Z","updated_at":"2016-12-08T21:04:32.964Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":71,"author_id":399,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 78,
    "obfuscated_id": "-wsYNe2w7uo",
    "author_id": 399,
    "chapter_id": 71,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T21:04:33.067Z",
    "created_at": "2016-12-08T21:04:32.854Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x000000123f28b8>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 160,
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
curl "api.goskive.com/v2/questions/78" -d '{"question":{"question":{"id":78,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T21:04:32.854Z","updated_at":"2016-12-08T21:04:32.964Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":71,"author_id":399,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51b3a091f0add351eac1c202f0c8afaf3ec76830bbeb748347fe8a094737ba9a"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/101/upvote
Content-Type: application/json
Authorization: Bearer bd938cfda2338b7eb9fdbefdb5e02ef813675f9f5aafe01e1441603b94d00901
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/101/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd938cfda2338b7eb9fdbefdb5e02ef813675f9f5aafe01e1441603b94d00901"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 2856b55ea75b47750a9ea52fff3e9b246f2edd75004792726de06edc2db3100f
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
      "creator_id": 931,
      "id": 301,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 287,
      "additional_university_ids": [

      ],
      "discipline_id": 311,
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
      "updated_at": "2016-12-08T21:05:14.142Z",
      "shortname": "mit-pizza-201",
      "topic_id": 311,
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
	-H "Authorization: Bearer 2856b55ea75b47750a9ea52fff3e9b246f2edd75004792726de06edc2db3100f"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 81c1ed0bcb570f10bb6a19a5b3042902870b2e378fd057539bde97cfa61f9264
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
      "id": 285,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-265",
      "html_url": "https://goskive.com/university/uni-265",
      "slug": "uni-265",
      "name": "National School of Pizza",
      "short_name": "Uni 265",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/3e8f08d757c4033d78611ebc133d32b0.jpg",
      "image_thumb_url": "memory://universities/a7e1bf3df0b465f81b04b3414ce04787.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T21:05:13.927Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 284,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-264",
      "html_url": "https://goskive.com/university/uni-264",
      "slug": "uni-264",
      "name": "National School of Pastry",
      "short_name": "Uni 264",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/bf3893cc7304e931c6125d5820a0b093.jpg",
      "image_thumb_url": "memory://universities/6e97a22a943a6bbc584481fbeaa44e5d.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T21:05:13.880Z",
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
	-H "Authorization: Bearer 81c1ed0bcb570f10bb6a19a5b3042902870b2e378fd057539bde97cfa61f9264"
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
      "id": 265,
      "name": "Horizontal neutral model",
      "name_translations": {
        "en": "Horizontal neutral model"
      },
      "discipline_id": 265
    },
    {
      "id": 266,
      "name": "Progressive zero tolerance architecture",
      "name_translations": {
        "en": "Progressive zero tolerance architecture"
      },
      "discipline_id": 266
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
GET /v2/topics/267
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
    "id": 267,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 267
  }
}
```



```shell
curl "api.goskive.com/v2/topics/267" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 377265f50a3bc6f8e1938201180fc7e33832fd19fc12775d7aa8ea4377333ede
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
      "id": 237,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-219",
      "html_url": "https://goskive.com/university/uni-219",
      "slug": "uni-219",
      "name": "University 180",
      "short_name": "Uni 219",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/1e4f5f9f24f2b4568225ff6f2957f7e8.jpg",
      "image_thumb_url": "memory://universities/d22ede403a7233e287fd1a89d76c97d0.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T21:05:01.899Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 238,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-220",
      "html_url": "https://goskive.com/university/uni-220",
      "slug": "uni-220",
      "name": "University 181",
      "short_name": "Uni 220",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/69d43d5493d4b9d17538fc8036bb21f9.jpg",
      "image_thumb_url": "memory://universities/de46db1ba723fec0d684f71622304784.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T21:05:01.947Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 239,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-221",
      "html_url": "https://goskive.com/university/uni-221",
      "slug": "uni-221",
      "name": "University 182",
      "short_name": "Uni 221",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/a6a894f1b2f4b03f7b62caab0ff7b392.jpg",
      "image_thumb_url": "memory://universities/217724fc31731691c5f6af694af3920d.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T21:05:01.996Z",
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
	-H "Authorization: Bearer 377265f50a3bc6f8e1938201180fc7e33832fd19fc12775d7aa8ea4377333ede"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1fd77034f2619458c71a6c0464e9117819b42f2087583fe1e770e8a4353202cf
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
    "id": 240,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/bdefe32d92f07489cc6a3e5781d0655f.jpg",
    "image_thumb_url": "memory://universities/5d7201cd7079763b530472ab0f6cd176.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-08T21:05:02.143Z",
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
	-H "Authorization: Bearer 1fd77034f2619458c71a6c0464e9117819b42f2087583fe1e770e8a4353202cf"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ee1dde3f6c135f487b1a26f8a729874db3fd8fdd37e2ce2d90f70b5b52e88177
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":263,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 775,
    "id": 256,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 235,
    "additional_university_ids": [

    ],
    "discipline_id": 263,
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
    "chapters_updated_at": "2016-12-08T21:05:01.274Z",
    "updated_at": "2016-12-08T21:05:01.419Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 139,
        "updated_at": "2016-12-08T21:05:01.409Z",
        "course_id": 256,
        "author_id": 775,
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
        "id": 140,
        "updated_at": "2016-12-08T21:05:01.422Z",
        "course_id": 256,
        "author_id": 775,
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
        "id": 141,
        "updated_at": "2016-12-08T21:05:01.434Z",
        "course_id": 256,
        "author_id": 775,
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
    "topic_id": 263,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":263,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee1dde3f6c135f487b1a26f8a729874db3fd8fdd37e2ce2d90f70b5b52e88177"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2c3fb2c495f6f82a480d3eda5546ac20af08006d01de033ecf6107408248c565
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":262,"published":false}}
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
    "creator_id": 774,
    "id": 255,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 234,
    "additional_university_ids": [

    ],
    "discipline_id": 262,
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
    "updated_at": "2016-12-08T21:05:01.230Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 262,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":262,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c3fb2c495f6f82a480d3eda5546ac20af08006d01de033ecf6107408248c565"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer dd83c82e9bcfc3514b5849a9aacda99d58e645a69df04e6b14833d2385ed71bb
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
      "creator_id": 732,
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-174",
      "html_url": "https://goskive.com/course/fu-course-174",
      "slug": "fu-course-174",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "discipline_id": 226,
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
      "updated_at": "2016-12-08T21:04:57.141Z",
      "shortname": "fu-course-174",
      "topic_id": 226,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 174",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 732,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-175",
      "html_url": "https://goskive.com/course/fu-course-175",
      "slug": "fu-course-175",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "discipline_id": 227,
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
      "chapters_updated_at": "2016-12-08T21:04:56.981Z",
      "updated_at": "2016-12-08T21:04:57.393Z",
      "shortname": "fu-course-175",
      "topic_id": 227,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd83c82e9bcfc3514b5849a9aacda99d58e645a69df04e6b14833d2385ed71bb"
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
      "creator_id": 752,
      "id": 235,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-190",
      "html_url": "https://goskive.com/course/fu-course-190",
      "slug": "fu-course-190",
      "university_id": 224,
      "additional_university_ids": [

      ],
      "discipline_id": 242,
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
      "updated_at": "2016-12-08T21:04:58.924Z",
      "shortname": "fu-course-190",
      "topic_id": 242,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 190",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 752,
      "id": 236,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 224,
      "additional_university_ids": [

      ],
      "discipline_id": 243,
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
      "chapters_updated_at": "2016-12-08T21:04:58.766Z",
      "updated_at": "2016-12-08T21:04:59.174Z",
      "shortname": "fu-course-191",
      "topic_id": 243,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 191",
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
Authorization: Bearer a9fc7bd22a2300546ad28155961e2af68464b2154d93f860dc4c62f38e1661c4
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
      "creator_id": 738,
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-178",
      "html_url": "https://goskive.com/course/fu-course-178",
      "slug": "fu-course-178",
      "university_id": 219,
      "additional_university_ids": [

      ],
      "discipline_id": 230,
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
      "updated_at": "2016-12-08T21:04:57.649Z",
      "shortname": "fu-course-178",
      "topic_id": 230,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 178",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 738,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-179",
      "html_url": "https://goskive.com/course/fu-course-179",
      "slug": "fu-course-179",
      "university_id": 219,
      "additional_university_ids": [

      ],
      "discipline_id": 231,
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
      "updated_at": "2016-12-08T21:04:57.683Z",
      "shortname": "fu-course-179",
      "topic_id": 231,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9fc7bd22a2300546ad28155961e2af68464b2154d93f860dc4c62f38e1661c4"
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
      "creator_id": 757,
      "id": 239,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-194",
      "html_url": "https://goskive.com/course/fu-course-194",
      "slug": "fu-course-194",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 246,
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
      "updated_at": "2016-12-08T21:04:59.430Z",
      "shortname": "fu-course-194",
      "topic_id": 246,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 194",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 757,
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 247,
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
      "updated_at": "2016-12-08T21:04:59.466Z",
      "shortname": "fu-course-195",
      "topic_id": 247,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
Authorization: Bearer a5e7d77acd35db83ead14f28a88d2526cde16b39ca4726154fefa7a3897acda9
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
  "id": 817,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-08T21:05:05.626Z",
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
	-H "Authorization: Bearer a5e7d77acd35db83ead14f28a88d2526cde16b39ca4726154fefa7a3897acda9"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/61
Content-Type: application/json
Authorization: Bearer 45f9f89afac2fba1f5cf64426bbd1f679099e9fdca61c7413518d4729635197f
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
    "id": 61,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 14,
    "fields_of_study": [
      14,
      15
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-08T21:03:59.540Z",
    "updated_at": "2016-12-08T21:03:59.540Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/61" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45f9f89afac2fba1f5cf64426bbd1f679099e9fdca61c7413518d4729635197f"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/59
Content-Type: application/json
Authorization: Bearer 488de30bb1d01278d9bec2a505e3eb4ba0e764ddc2b6a51c377248f7ab6e9f20
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
    "id": 59,
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
    "created_at": "2016-12-08T21:03:59.352Z",
    "updated_at": "2016-12-08T21:03:59.352Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/59" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 488de30bb1d01278d9bec2a505e3eb4ba0e764ddc2b6a51c377248f7ab6e9f20"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer 2872373b8938efc39fb65a37edfae9a4523107eb9c0931db2ac21ae0e1023332
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2872373b8938efc39fb65a37edfae9a4523107eb9c0931db2ac21ae0e1023332"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/23
Content-Type: application/json
Authorization: Bearer 09df5f00390737afb848fd20f3470e2de3a6ce574789f8310ca02bf518721f7d
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
    "id": 23,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 134,
    "user_id": 982
  }
}
```



```shell
curl "api.goskive.com/v2/votes/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09df5f00390737afb848fd20f3470e2de3a6ce574789f8310ca02bf518721f7d"
```
