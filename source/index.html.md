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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"6753fb6ac21ef43cf5548c04d10b3d0e5c1f398228e8019fe86c8c58ffa1f033","client_secret":"0c34e7d55e78a1bd49f2f4bf8ceb5e6d94af8e0218cb3fe5e11f34e99b3e2147"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"6753fb6ac21ef43cf5548c04d10b3d0e5c1f398228e8019fe86c8c58ffa1f033","client_secret":"0c34e7d55e78a1bd49f2f4bf8ceb5e6d94af8e0218cb3fe5e11f34e99b3e2147"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MjE2YmFlYWYyMTVhZTllMDE4MTQ2NWI1ODQ0NGNkZTliNjIwMDg1NzZlZjE5
ZDA5MmMxZDllZDBhNDlmODI3ZTo1ODkwYmIzZjdjNWM1NzM3OGE3OTRkYjkx
OTlmYTRiY2Q5ODViMDMyMzM5OGRkZDY1Y2ExZDk2OGQ3NmEzN2U1

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
	-u 216baeaf215ae9e0181465b58444cde9b62008576ef19d092c1d9ed0a49f827e:5890bb3f7c5c57378a794db9199fa4bcd985b0323398ddd65ca1d968d76a37e5
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"38731e774272bbc18bdfda1ca9c6a3fb49e8f937e5425016cf641d9dad432053","client_secret":"16de39ae7c55e2beebe602542161ba90a36dac79ccb16fee8b0f7d7b0147a38b"}
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
  "access_token": "1d5f8ff5cbc39f9a05a602c8f6b504eeb02575c45cb509f380960da0fd8b0ea3",
  "token_type": "bearer",
  "created_at": 1476882951
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"38731e774272bbc18bdfda1ca9c6a3fb49e8f937e5425016cf641d9dad432053","client_secret":"16de39ae7c55e2beebe602542161ba90a36dac79ccb16fee8b0f7d7b0147a38b"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic Nzk4NjA2MDgwNTQ3OTlkMjM1MTVkNDQxNzhiNzZjMTM4ODc0YjJjMTU2Mzlj
OTBmZTcxMmE4YTVhZjk2NmVjYTpkNDU1YzZjMWIxODZkMWUzZWMwNGZiZTcw
MGYwZDBjYmJlNDVjMmYzOGQ5MmY4MTExMmE5YTE5NWNmOTEzNGZj

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
  "access_token": "e0b586ddafc5c82ce0d80982c0e16742392e5d9ecb6cb8e19c9e257ccc2761b1",
  "token_type": "bearer",
  "created_at": 1476882951
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 79860608054799d23515d44178b76c138874b2c15639c90fe712a8a5af966eca:d455c6c1b186d1e3ec04fbe700f0d0cbbe45c2f38d92f81112a9a195cf9134fc
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
{"grant_type":"client_credentials","client_id":"28cf16c7db80928655847cefe427ae8af43f5b3d8048de6a6eee9afa26b13f90","client_secret":"4bb0c5505302208281f504b87e2c9dd5b163f47b6c73d891cbd222741c5b57a2"}
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
  "access_token": "9b6edb8d19da2b82fb4acd394ae81aad7dd0404f7ed81940befd39ca45433725",
  "token_type": "bearer",
  "created_at": 1476882951
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"28cf16c7db80928655847cefe427ae8af43f5b3d8048de6a6eee9afa26b13f90","client_secret":"4bb0c5505302208281f504b87e2c9dd5b163f47b6c73d891cbd222741c5b57a2"}' -X POST \
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
Authorization: Bearer f1a07ba5da0584d027d231f9e12c326af6c641b3567f0dfd926cac8280187f69
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
    "company_id": 35,
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
	-H "Authorization: Bearer f1a07ba5da0584d027d231f9e12c326af6c641b3567f0dfd926cac8280187f69"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/133/flashcards
Content-Type: application/json
Authorization: Bearer 5b25c0a7a0c52e4f3cfd3949a1f3aea43f0c18cd54ee6729605e520781bc4825
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":133,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 80,
    "obfuscated_id": "94gVa2GR5x8",
    "author_id": 666,
    "chapter_id": 133,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:24.565Z",
    "created_at": "2016-10-19T13:15:24.565Z",
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
curl "api.goskive.com/v2/chapters/133/flashcards" -d '{"flashcard":{"chapter_id":133,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b25c0a7a0c52e4f3cfd3949a1f3aea43f0c18cd54ee6729605e520781bc4825"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/135/flashcards
Content-Type: application/json
Authorization: Bearer a6b2c11e0b59180c9bff9d795ee894b7c1e91ad83487ad52e59352fc8c0ac3e1
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
      "id": 81,
      "obfuscated_id": "jHF1owx40fU",
      "author_id": 670,
      "chapter_id": 135,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:24.889Z",
      "created_at": "2016-10-19T13:15:24.889Z",
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
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 670,
      "chapter_id": 135,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:24.930Z",
      "created_at": "2016-10-19T13:15:24.930Z",
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
      "id": 83,
      "obfuscated_id": "FCSR-nKROLo",
      "author_id": 670,
      "chapter_id": 135,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:24.970Z",
      "created_at": "2016-10-19T13:15:24.970Z",
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
curl "api.goskive.com/v2/chapters/135/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6b2c11e0b59180c9bff9d795ee894b7c1e91ad83487ad52e59352fc8c0ac3e1"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/95/questions
Content-Type: application/json
Authorization: Bearer 873b0a4e5e3910033694389aa88b61954a1010b9f44b37332759c4c7b581b10c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":95,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 492,
    "chapter_id": 95,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:09.264Z",
    "created_at": "2016-10-19T13:15:09.264Z",
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
        "id": 152,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 153,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 154,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 155,
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
curl "api.goskive.com/v2/chapters/95/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":95,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 873b0a4e5e3910033694389aa88b61954a1010b9f44b37332759c4c7b581b10c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/94/questions
Content-Type: application/json
Authorization: Bearer bb5facfa7e2fcaa6afa36d7590f1de6204185be450311757fb989dccd3f03f38
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":94,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 75,
    "obfuscated_id": "rRYuZazyhgg",
    "author_id": 489,
    "chapter_id": 94,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:08.902Z",
    "created_at": "2016-10-19T13:15:08.902Z",
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
        "id": 150,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 151,
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
curl "api.goskive.com/v2/chapters/94/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":94,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb5facfa7e2fcaa6afa36d7590f1de6204185be450311757fb989dccd3f03f38"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/96/questions
Content-Type: application/json
Authorization: Bearer 6d17b9ff9894f591fb7d85a92a680b588bb0187f51361177bbf4d4e4a6ce0ae8
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 495,
    "chapter_id": 96,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:09.822Z",
    "created_at": "2016-10-19T13:15:09.822Z",
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
        "id": 156,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 157,
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
	-H "Authorization: Bearer 6d17b9ff9894f591fb7d85a92a680b588bb0187f51361177bbf4d4e4a6ce0ae8"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/93/questions
Content-Type: application/json
Authorization: Bearer a323c44a087abcd97e86da24231a349174c073c8130dd0facc78e581c4e1a4a8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":93,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 486,
    "chapter_id": 93,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:08.441Z",
    "created_at": "2016-10-19T13:15:08.441Z",
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
        "id": 147,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 148,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 149,
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
curl "api.goskive.com/v2/chapters/93/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":93,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a323c44a087abcd97e86da24231a349174c073c8130dd0facc78e581c4e1a4a8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/92/questions
Content-Type: application/json
Authorization: Bearer 86dedaddecc159ddf2f4ff351f91727693565f964cf8026e0816d4a8b5f8afb4
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 480,
      "chapter_id": 92,
      "position": 71,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:07.715Z",
      "created_at": "2016-10-19T13:15:07.588Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 481,
      "chapter_id": 92,
      "position": 72,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:07.922Z",
      "created_at": "2016-10-19T13:15:07.792Z",
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
    },
    {
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 482,
      "chapter_id": 92,
      "position": 73,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T13:15:08.154Z",
      "created_at": "2016-10-19T13:15:08.002Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/92/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86dedaddecc159ddf2f4ff351f91727693565f964cf8026e0816d4a8b5f8afb4"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/74
Content-Type: application/json
Authorization: Bearer 2a1b3fd0f311d6a565917ef4950a1d85d3008e7340fc0ef468dbd85438a67407
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
curl "api.goskive.com/v2/chapters/74" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a1b3fd0f311d6a565917ef4950a1d85d3008e7340fc0ef468dbd85438a67407"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/77
Content-Type: application/json
Authorization: Bearer 51a0667af5827b0fa229eb0db9bab3f881cf7c0dcadb522ea9971a71ac13eaab
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
curl "api.goskive.com/v2/chapters/77" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51a0667af5827b0fa229eb0db9bab3f881cf7c0dcadb522ea9971a71ac13eaab"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/81
Content-Type: application/json
Authorization: Bearer b717bca773f89c8125f6e393c27587fed1253adcb03e04ea8c919071eb4881d6
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
curl "api.goskive.com/v2/chapters/81" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b717bca773f89c8125f6e393c27587fed1253adcb03e04ea8c919071eb4881d6"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/75
Content-Type: application/json
Authorization: Bearer ca85475fa1dc0f40a4cc83eca5d1f9003152667ee343ae01815ed8205d1427d4
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/75" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca85475fa1dc0f40a4cc83eca5d1f9003152667ee343ae01815ed8205d1427d4"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/78
Content-Type: application/json
Authorization: Bearer ccd48e8fd9f7014e7a51e0a1d700f4fc57acc5f17aa977ffdfdef65b60b88d42
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
    "id": 78,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T13:15:03.610Z",
    "course_id": 133,
    "author_id": 415,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-19T13:15:02.978Z",
    "questions_updated_at": "2016-10-19T13:15:02.978Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 419,
        "chapter_id": 78,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:03.589Z",
        "created_at": "2016-10-19T13:15:03.589Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 417,
        "chapter_id": 78,
        "position": 68,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:15:03.461Z",
        "created_at": "2016-10-19T13:15:03.317Z",
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
            "id": 135,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 136,
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
curl "api.goskive.com/v2/chapters/78" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccd48e8fd9f7014e7a51e0a1d700f4fc57acc5f17aa977ffdfdef65b60b88d42"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/82
Content-Type: application/json
Authorization: Bearer 1ee2c8ea5493dfbb3da6d1c4dbff7b27e34b6e51341bdece51cb41e65b595275
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
    "id": 82,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T13:15:04.905Z",
    "course_id": 137,
    "author_id": 435,
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
curl "api.goskive.com/v2/chapters/82" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee2c8ea5493dfbb3da6d1c4dbff7b27e34b6e51341bdece51cb41e65b595275"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/50/replies
Content-Type: application/json
Authorization: Bearer f6d965376c8087a22388cdeb26fc53e556529c8fd5a6202bfa8e002d365452b3
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
    "id": 51,
    "author_id": 282,
    "reply_to_id": 50,
    "created_at": "2016-10-19T13:14:50.896Z",
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
curl "api.goskive.com/v2/comments/50/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6d965376c8087a22388cdeb26fc53e556529c8fd5a6202bfa8e002d365452b3"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/49/replies
Content-Type: application/json
Authorization: Bearer 86d06523eedfbad805d9c2c7e812abd45a718cb21e0e288b0cf08301a02eddc4
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
curl "api.goskive.com/v2/comments/49/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86d06523eedfbad805d9c2c7e812abd45a718cb21e0e288b0cf08301a02eddc4"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer 89f60579124b69f36ca7e2f8fc62f10db929c8828589a7742ed974b53dd891a7
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
curl "api.goskive.com/v2/comments/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89f60579124b69f36ca7e2f8fc62f10db929c8828589a7742ed974b53dd891a7"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/42/republish
Content-Type: application/json
Authorization: Bearer bf330425358f38785aca3f39aa2b6d27af0a20aad1840588b04ef39b7b1274ed
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
	-H "Authorization: Bearer bf330425358f38785aca3f39aa2b6d27af0a20aad1840588b04ef39b7b1274ed"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 7268002545128b7b27a7ebb2ec3b6e2aee96dd69cdafcfed4d7614bdc91decde
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7268002545128b7b27a7ebb2ec3b6e2aee96dd69cdafcfed4d7614bdc91decde"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/44/report
Content-Type: application/json
Authorization: Bearer 36109a1504d716590558032fd4d126b110b8ae207adf7df08d6f2a419134a62d
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36109a1504d716590558032fd4d126b110b8ae207adf7df08d6f2a419134a62d"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/39
Content-Type: application/json
Authorization: Bearer 8ebfd8a027f4ad1a081c7d369f6f25e4da06151b16096a7c70607b66439b28ff
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
    "updated_at": "2016-10-19T13:15:40.809Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ebfd8a027f4ad1a081c7d369f6f25e4da06151b16096a7c70607b66439b28ff"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 62de81d5a23a007d593eb2cf11e003baeda1f27a2f38df610b5a3ce6125c093e
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
      "updated_at": "2016-10-19T13:15:40.747Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T13:15:40.752Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T13:15:40.756Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62de81d5a23a007d593eb2cf11e003baeda1f27a2f38df610b5a3ce6125c093e"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/3/company_profiles
Content-Type: application/json
Authorization: Bearer c4d1acc2734665a348c9d4c01a952fe373fc0ab1ed97ca8f43382d93f5c23b53
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
curl "api.goskive.com/v2/companies/3/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4d1acc2734665a348c9d4c01a952fe373fc0ab1ed97ca8f43382d93f5c23b53"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/1/company_profiles
Content-Type: application/json
Authorization: Bearer 52e1dbaf49cb4e2a49f4694962875920ef439a29933d0262378536a39dac2a88
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
curl "api.goskive.com/v2/companies/1/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52e1dbaf49cb4e2a49f4694962875920ef439a29933d0262378536a39dac2a88"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 2297304ccbde8d57884f56684855ab1e53e09af30e74c2d1475afcf0fd6013ac
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
      "id": 7,
      "title": "Campaign 7",
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
	-H "Authorization: Bearer 2297304ccbde8d57884f56684855ab1e53e09af30e74c2d1475afcf0fd6013ac"
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
Authorization: Bearer 2932f612965ff4faa53b22d7ef492542a6fa8e8d81d2b2dca714f4acc2d28d2d
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
	-H "Authorization: Bearer 2932f612965ff4faa53b22d7ef492542a6fa8e8d81d2b2dca714f4acc2d28d2d"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2845f5e085c467835790ea0d1f5cdf896ede55a0881ea897827c72d5f3d0893d
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
    "id": 73,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T13:15:01.808Z",
    "course_id": 128,
    "author_id": 401,
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
	-H "Authorization: Bearer 2845f5e085c467835790ea0d1f5cdf896ede55a0881ea897827c72d5f3d0893d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f93b703509f97ee6c70cdf45d0b49faead6fb573b336eecc9e5f54888bf5d979
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
      "id": 53,
      "title": "Clever Chapter Title 53",
      "position": 1,
      "updated_at": "2016-10-19T13:14:58.805Z",
      "course_id": 116,
      "author_id": 356,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 54,
      "title": "Clever Chapter Title 54",
      "position": 2,
      "updated_at": "2016-10-19T13:14:58.833Z",
      "course_id": 116,
      "author_id": 357,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 55,
      "title": "Clever Chapter Title 55",
      "position": 3,
      "updated_at": "2016-10-19T13:14:59.144Z",
      "course_id": 116,
      "author_id": 358,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T13:14:58.713Z",
      "questions_updated_at": "2016-10-19T13:14:58.713Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f93b703509f97ee6c70cdf45d0b49faead6fb573b336eecc9e5f54888bf5d979"
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
      "id": 65,
      "title": "Clever Chapter Title 65",
      "position": 1,
      "updated_at": "2016-10-19T13:15:00.571Z",
      "course_id": 122,
      "author_id": 384,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 66,
      "title": "Clever Chapter Title 66",
      "position": 2,
      "updated_at": "2016-10-19T13:15:00.602Z",
      "course_id": 122,
      "author_id": 385,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 67,
      "title": "Clever Chapter Title 67",
      "position": 3,
      "updated_at": "2016-10-19T13:15:00.923Z",
      "course_id": 122,
      "author_id": 386,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T13:15:00.479Z",
      "questions_updated_at": "2016-10-19T13:15:00.479Z",
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
Authorization: Bearer 3c6cc959b48d816f48e83a90f99fa6b96eb09a361b13c07cc22c3c44c55c95fa
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
      "id": 56,
      "title": "Clever Chapter Title 56",
      "position": 1,
      "updated_at": "2016-10-19T13:14:59.327Z",
      "course_id": 117,
      "author_id": 363,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 57,
      "title": "Clever Chapter Title 57",
      "position": 2,
      "updated_at": "2016-10-19T13:14:59.384Z",
      "course_id": 117,
      "author_id": 364,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 58,
      "title": "Clever Chapter Title 58",
      "position": 3,
      "updated_at": "2016-10-19T13:14:59.413Z",
      "course_id": 117,
      "author_id": 365,
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
	-H "Authorization: Bearer 3c6cc959b48d816f48e83a90f99fa6b96eb09a361b13c07cc22c3c44c55c95fa"
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
      "id": 68,
      "title": "Clever Chapter Title 68",
      "position": 1,
      "updated_at": "2016-10-19T13:15:01.142Z",
      "course_id": 124,
      "author_id": 391,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 69,
      "title": "Clever Chapter Title 69",
      "position": 2,
      "updated_at": "2016-10-19T13:15:01.170Z",
      "course_id": 124,
      "author_id": 392,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 70,
      "title": "Clever Chapter Title 70",
      "position": 3,
      "updated_at": "2016-10-19T13:15:01.198Z",
      "course_id": 124,
      "author_id": 393,
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
Authorization: Bearer 0bc225fa5c0b8a16eb97067dea94424ab3c32237822f65318c6a8a4ef7ba285e
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
    "course_id": 225,
    "user_id": 657,
    "updated_at": "2016-10-19T13:15:23.988Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bc225fa5c0b8a16eb97067dea94424ab3c32237822f65318c6a8a4ef7ba285e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 20c53aa248dded9612ab581aea061658ba3d868425ceebbd6701087be1812eb2
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
      "course_id": 224,
      "user_id": 653,
      "updated_at": "2016-10-19T13:15:23.783Z"
    },
    {
      "id": 4,
      "course_id": 224,
      "user_id": 654,
      "updated_at": "2016-10-19T13:15:23.800Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20c53aa248dded9612ab581aea061658ba3d868425ceebbd6701087be1812eb2"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/278/files
Content-Type: application/json
Authorization: Bearer f2c31d021f074584cd528b79f5242872103745d10ecbc8278eea8eae1ce8cf53
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
        "id": 862,
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
        "created_at": "2016-10-19T13:15:40.928Z",
        "updated_at": "2016-10-19T13:15:40.928Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T13:15:40.935Z",
      "updated_at": "2016-10-19T13:15:40.935Z",
      "course_id": 278,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 863,
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
        "created_at": "2016-10-19T13:15:40.943Z",
        "updated_at": "2016-10-19T13:15:40.943Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T13:15:40.950Z",
      "updated_at": "2016-10-19T13:15:40.950Z",
      "course_id": 278,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 864,
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
        "created_at": "2016-10-19T13:15:40.957Z",
        "updated_at": "2016-10-19T13:15:40.957Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T13:15:40.964Z",
      "updated_at": "2016-10-19T13:15:40.964Z",
      "course_id": 278,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/278/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2c31d021f074584cd528b79f5242872103745d10ecbc8278eea8eae1ce8cf53"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/280/files
Content-Type: application/json
Authorization: Bearer 24ac09bbba4489d8795abee4d501069ec4ce7b17bc5a4dfbb8f6d0b16f4b05fe
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
      "id": 869,
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
      "created_at": "2016-10-19T13:15:41.228Z",
      "updated_at": "2016-10-19T13:15:41.228Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [

    ],
    "created_at": "2016-10-19T13:15:41.257Z",
    "updated_at": "2016-10-19T13:15:41.257Z",
    "course_id": 280,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/280/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24ac09bbba4489d8795abee4d501069ec4ce7b17bc5a4dfbb8f6d0b16f4b05fe"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/281/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 54a27e9035e6150886b1a49b0b18e80906c564a16375c79ce1a5c229cf159f25
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
    "key": "cache/d7ff42274c1a46f80e3889df4ea237cf.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxNDoxNTo0MVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9kN2ZmNDIyNzRjMWE0NmY4MGUzODg5ZGY0ZWEyMzdjZi5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTlUMTMxNTQxWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T131541Z",
    "x-amz-signature": "36db8e9ecfb4bf8c5f2b27bedb4fba9bded80c235f7074175f93863df13f9477"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/281/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54a27e9035e6150886b1a49b0b18e80906c564a16375c79ce1a5c229cf159f25"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 5231586129be9cba7bae733b6dc3dfec640184d1f03feff927ef8d12f302cc79
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
	-H "Authorization: Bearer 5231586129be9cba7bae733b6dc3dfec640184d1f03feff927ef8d12f302cc79"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0e8a58c3a1f692f737f6c1dd5618c16f72d3cd238037e97c1200cdc62cc5d959
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
	-H "Authorization: Bearer 0e8a58c3a1f692f737f6c1dd5618c16f72d3cd238037e97c1200cdc62cc5d959"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 457e79063c5d71f229de622816decc5977fc6ba04241c92593cf62dc06b74411
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
	-H "Authorization: Bearer 457e79063c5d71f229de622816decc5977fc6ba04241c92593cf62dc06b74411"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e756fcc19e495d1c128c587cf9ffc100e548c456311848f01fb41920128d8751
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
	-H "Authorization: Bearer e756fcc19e495d1c128c587cf9ffc100e548c456311848f01fb41920128d8751"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a43c9eac357f4f8a25a655046bedf3eb01193af3be52cd249a4e5e65749b3005
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
	-H "Authorization: Bearer a43c9eac357f4f8a25a655046bedf3eb01193af3be52cd249a4e5e65749b3005"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 87196750e969c6026dae0043d2460a55e7baf44b4d8a4220954419d68a20db0f
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
    "creator_id": 189,
    "id": 75,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 75,
    "additional_university_ids": [

    ],
    "topic_id": 80,
    "discipline_id": 80,
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
    "chapters_updated_at": "2016-10-19T13:14:38.406Z",
    "updated_at": "2016-10-19T13:14:39.913Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 11,
        "title": "Clever Chapter Title 11",
        "position": 1,
        "updated_at": "2016-10-19T13:14:39.865Z",
        "course_id": 75,
        "author_id": 189,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T13:14:38.406Z",
        "questions_updated_at": "2016-10-19T13:14:38.406Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 12,
        "title": "Clever Chapter Title 12",
        "position": 2,
        "updated_at": "2016-10-19T13:14:39.906Z",
        "course_id": 75,
        "author_id": 189,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T13:14:38.406Z",
        "questions_updated_at": "2016-10-19T13:14:38.406Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 190,
        "chapter_id": 11,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.692Z",
        "created_at": "2016-10-19T13:14:39.692Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 190,
        "chapter_id": 12,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.771Z",
        "created_at": "2016-10-19T13:14:39.771Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 190,
        "chapter_id": 11,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.738Z",
        "created_at": "2016-10-19T13:14:39.738Z",
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
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 190,
        "chapter_id": 12,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.813Z",
        "created_at": "2016-10-19T13:14:39.813Z",
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
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 190,
        "chapter_id": 11,
        "position": 9,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:38.634Z",
        "created_at": "2016-10-19T13:14:38.512Z",
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
            "id": 17,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 18,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 190,
        "chapter_id": 11,
        "position": 10,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:38.819Z",
        "created_at": "2016-10-19T13:14:38.702Z",
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
      },
      {
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 190,
        "chapter_id": 12,
        "position": 11,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.032Z",
        "created_at": "2016-10-19T13:14:38.903Z",
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
            "id": 21,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 22,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 190,
        "chapter_id": 12,
        "position": 12,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:39.222Z",
        "created_at": "2016-10-19T13:14:39.102Z",
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
            "id": 23,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 24,
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
	-H "Authorization: Bearer 87196750e969c6026dae0043d2460a55e7baf44b4d8a4220954419d68a20db0f"
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
    "creator_id": 201,
    "id": 77,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 77,
    "additional_university_ids": [

    ],
    "topic_id": 82,
    "discipline_id": 82,
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
    "chapters_updated_at": "2016-10-19T13:14:41.693Z",
    "updated_at": "2016-10-19T13:14:43.223Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 15,
        "title": "Clever Chapter Title 15",
        "position": 1,
        "updated_at": "2016-10-19T13:14:43.172Z",
        "course_id": 77,
        "author_id": 201,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T13:14:41.693Z",
        "questions_updated_at": "2016-10-19T13:14:41.693Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 16,
        "title": "Clever Chapter Title 16",
        "position": 2,
        "updated_at": "2016-10-19T13:14:43.215Z",
        "course_id": 77,
        "author_id": 201,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T13:14:41.693Z",
        "questions_updated_at": "2016-10-19T13:14:41.693Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 201,
        "chapter_id": 15,
        "position": 21,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:41.919Z",
        "created_at": "2016-10-19T13:14:41.797Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 201,
        "chapter_id": 16,
        "position": 23,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T13:14:42.333Z",
        "created_at": "2016-10-19T13:14:42.203Z",
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
PUT /v2/courses/60/pin
Content-Type: application/json
Authorization: Bearer dd0d9ce6b59b5eacf77eb63434210a9591f89e9cbf4a06d65b268bba2e672955
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/60/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd0d9ce6b59b5eacf77eb63434210a9591f89e9cbf4a06d65b268bba2e672955"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/61/pin
Content-Type: application/json
Authorization: Bearer 13ed65f70f80acd4f572abea4f42ea620b8edcafda4fd5858993bdad4cee8c3b
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/61/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13ed65f70f80acd4f572abea4f42ea620b8edcafda4fd5858993bdad4cee8c3b"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2b8f10b50ff102b49cfd2223f16c1f2d9a8eb5941dba96b2f906404ad0386450
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
    "creator_id": 184,
    "id": 72,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 72,
    "additional_university_ids": [

    ],
    "topic_id": 77,
    "discipline_id": 77,
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
    "updated_at": "2016-10-19T13:14:38.113Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b8f10b50ff102b49cfd2223f16c1f2d9a8eb5941dba96b2f906404ad0386450"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 2f3eb9dc662fa64d15d9ff2a5f1c3097b8cf5978b5d87cc195c4ec1504f02d6b
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
    "id": 64,
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
    "created_at": "2016-10-19T13:14:31.521Z",
    "updated_at": "2016-10-19T13:14:31.521Z",
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
	-H "Authorization: Bearer 2f3eb9dc662fa64d15d9ff2a5f1c3097b8cf5978b5d87cc195c4ec1504f02d6b"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 22c9210aba4a77a97469c2759e04bd8652adbfb42bbc3e1205ad3f80cd8a53df
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[19]}
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
    "id": 59,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      19
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T13:14:30.907Z",
    "updated_at": "2016-10-19T13:14:30.962Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[19]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22c9210aba4a77a97469c2759e04bd8652adbfb42bbc3e1205ad3f80cd8a53df"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer e3d923caa02ee86dd635a575a1b4615f74d9eea5c22458acad1c31a8d8916c6c
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
    "id": 61,
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
    "created_at": "2016-10-19T13:14:31.068Z",
    "updated_at": "2016-10-19T13:14:31.068Z",
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
	-H "Authorization: Bearer e3d923caa02ee86dd635a575a1b4615f74d9eea5c22458acad1c31a8d8916c6c"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 5763b61ac5bdb2f82692139210caef3525d3885b06a25849dd1bb8ba10fd52ca
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[20]}
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
    "id": 60,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      20
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T13:14:31.015Z",
    "updated_at": "2016-10-19T13:14:31.015Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[20]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5763b61ac5bdb2f82692139210caef3525d3885b06a25849dd1bb8ba10fd52ca"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a89ccf82f1763806107f0870263cca2ae39e89812a0280449aefe7d44e8f311b
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

23
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
    "id": 63,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/e489f8d15d6370ad0f683018a0d54ccb5761defa.jpg",
    "university_id": null,
    "fields_of_study": [
      23
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T13:14:31.242Z",
    "updated_at": "2016-10-19T13:14:31.490Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/a680882b7288df4caed17fd71553c0aff6ebb761.jpg",
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

23
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a89ccf82f1763806107f0870263cca2ae39e89812a0280449aefe7d44e8f311b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 08b7cdc5f4bc99b31eee833ab3628e90ba93c45c8aaef6f5e49ce346a83cdf5a
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
      "bookmarkable_id": 33,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 34,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 35,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08b7cdc5f4bc99b31eee833ab3628e90ba93c45c8aaef6f5e49ce346a83cdf5a"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8fed49b167ca35309acdb82ca321167e50519723812cd7b14d61e0b1dd0ce9ca
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
      "company_id": 8,
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
      "id": 3,
      "title": "Campaign 3",
      "company_id": 9,
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
	-H "Authorization: Bearer 8fed49b167ca35309acdb82ca321167e50519723812cd7b14d61e0b1dd0ce9ca"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer c182eb02a0e07a4966bd5cc783f86b54c0f13b55fbcf6545c5b566db9c10acda
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
      "company_id": 4,
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
	-H "Authorization: Bearer c182eb02a0e07a4966bd5cc783f86b54c0f13b55fbcf6545c5b566db9c10acda"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer af449d3dbc00d5c74c13d9e4fd2ba97370a0dde4f71a00fbfd2fe949e9569ee8
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
      "creator_id": 241,
      "id": 87,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-72",
      "html_url": "https://goskive.com/course/mit-course-72",
      "slug": "mit-course-72",
      "university_id": 87,
      "additional_university_ids": [

      ],
      "topic_id": 92,
      "discipline_id": 92,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 72",
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
      "updated_at": "2016-10-19T13:14:47.302Z",
      "shortname": "mit-course-72"
    },
    {
      "creator_id": 242,
      "id": 88,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-73",
      "html_url": "https://goskive.com/course/mit-course-73",
      "slug": "mit-course-73",
      "university_id": 88,
      "additional_university_ids": [

      ],
      "topic_id": 93,
      "discipline_id": 93,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 73",
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
      "updated_at": "2016-10-19T13:14:47.390Z",
      "shortname": "mit-course-73"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af449d3dbc00d5c74c13d9e4fd2ba97370a0dde4f71a00fbfd2fe949e9569ee8"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer d5c8dab15fcf04876ed52be2c74dfa758969466f08c162cf8f251fef60f9641d
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
      "company_id": 17,
      "company": {
        "id": 17,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T13:15:26.788Z"
      },
      "created_at": "2016-10-19T13:15:26.792Z",
      "updated_at": "2016-10-19T13:15:26.792Z",
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T13:15:26.801Z"
      },
      "created_at": "2016-10-19T13:15:26.804Z",
      "updated_at": "2016-10-19T13:15:26.804Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5c8dab15fcf04876ed52be2c74dfa758969466f08c162cf8f251fef60f9641d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 2ac4d4c234fed3cdbb530c90483bc4f3c6c0ec19e3ff4e4a0b81236a7bad028f
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
      "company_id": 13,
      "company": {
        "id": 13,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T13:15:26.563Z"
      },
      "created_at": "2016-10-19T13:15:26.568Z",
      "updated_at": "2016-10-19T13:15:26.568Z",
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 11",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T13:15:26.584Z"
      },
      "created_at": "2016-10-19T13:15:26.588Z",
      "updated_at": "2016-10-19T13:15:26.588Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ac4d4c234fed3cdbb530c90483bc4f3c6c0ec19e3ff4e4a0b81236a7bad028f"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 3096d0f50990868bc8e0925ce9712c54a2170e31f7f7731ca2b1572577b8e5e4
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
      "id": 2,
      "created_at": "2016-10-19T13:14:26.766Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-19T13:14:26.890Z",
      "author_id": "7",
      "thread_subject_id": "2",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 3,
      "created_at": "2016-10-19T13:14:26.878Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-10-19T13:14:26.893Z",
      "author_id": "10",
      "thread_subject_id": "3",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-10-19T13:14:27.417Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-19T13:14:27.417Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-10-19T13:14:27.805Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-19T13:14:27.805Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 6,
      "created_at": "2016-10-19T13:14:28.182Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-19T13:14:28.182Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 7,
      "created_at": "2016-10-19T13:14:28.475Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 4,
      "updated_at": "2016-10-19T13:14:28.475Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-10-19T13:14:28.769Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 5,
      "updated_at": "2016-10-19T13:14:28.769Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-10-19T13:14:29.058Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 6,
      "updated_at": "2016-10-19T13:14:29.058Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3096d0f50990868bc8e0925ce9712c54a2170e31f7f7731ca2b1572577b8e5e4"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/1
Content-Type: application/json
Authorization: Bearer 58598c76bd9eba3dcb45e591cfc86e9eef9e58f5d8d4b81e7c6a61605c3233b0
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-19T13:04:25.000Z"}}
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
    "id": 1,
    "created_at": "2016-10-19T13:14:26.418Z",
    "read_at": "2016-10-19T13:04:25.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-10-19T13:14:26.626Z",
    "author_id": "3",
    "thread_subject_id": "1",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/1" -d '{"notification":{"read_at":"2016-10-19T13:04:25.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58598c76bd9eba3dcb45e591cfc86e9eef9e58f5d8d4b81e7c6a61605c3233b0"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 16b8cf1276faeacba8475df860ce2e1ad64fb423b327b92ea4f7ce9936c705e6
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
      "course_id": 230,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T13:15:25.666Z",
      "course_published": true,
      "updated_at": "2016-10-19T13:15:25.657Z"
    },
    {
      "id": 5,
      "course_id": 231,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T13:15:25.756Z",
      "course_published": true,
      "updated_at": "2016-10-19T13:15:25.746Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16b8cf1276faeacba8475df860ce2e1ad64fb423b327b92ea4f7ce9936c705e6"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 014f11882ed11bd21f696fcba7fd21152dc3edc6feef84782b84b05fdaaaa0a6
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
    "course_id": 234,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T13:15:26.183Z",
    "course_published": true,
    "updated_at": "2016-10-19T13:15:26.174Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 014f11882ed11bd21f696fcba7fd21152dc3edc6feef84782b84b05fdaaaa0a6"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 644efabecf2d05f5aaf8441c69d231cc8498a6f12e21e11d6fca05bb7f8d1d5d
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
    "course_id": 235,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-19T13:15:26.361Z",
    "course_published": true,
    "updated_at": "2016-10-19T13:15:26.348Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 644efabecf2d05f5aaf8441c69d231cc8498a6f12e21e11d6fca05bb7f8d1d5d"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3a5c20be467c1b98187cf85c22885be1ad311384d293cce858148acd00aff048
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
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 578
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 80,
      "user_id": 578
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 578
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 82,
      "user_id": 578
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a5c20be467c1b98187cf85c22885be1ad311384d293cce858148acd00aff048"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/241
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
    "id": 241,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 241,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 241
      },
      {
        "id": 242,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 241
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/241" -X GET \
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
      "id": 242,
      "name": "Exclusive didactic extranet",
      "name_translations": {
        "en": "Exclusive didactic extranet"
      }
    },
    {
      "id": 243,
      "name": "User-friendly optimal artificial intelligence",
      "name_translations": {
        "en": "User-friendly optimal artificial intelligence"
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
PATCH /v2/feedbacks/19/close
Content-Type: application/json
Authorization: Bearer d8d707f0d256e42cc4a3feb380ffbda0c8cd9b6e2c3930be7973e8e58f9c1a0c
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
    "id": 19,
    "user_id": 728,
    "feedbackable_id": 84,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-19T13:15:31.446Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/19/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8d707f0d256e42cc4a3feb380ffbda0c8cd9b6e2c3930be7973e8e58f9c1a0c"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/fix
Content-Type: application/json
Authorization: Bearer 577b749ab2165f7e071d1d686201bc7bb36c9dc1e2f0e02fd55e08f8b77c4eb7
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
    "id": 44,
    "user_id": 839,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-19T13:15:39.694Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/44/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 577b749ab2165f7e071d1d686201bc7bb36c9dc1e2f0e02fd55e08f8b77c4eb7"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/45
Content-Type: application/json
Authorization: Bearer ba20435af2f4bc21cf9a1497afb96f4b2d88d0a5ad8cb4a0124892f7e7cb5414
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
    "user_id": 844,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T13:15:40.053Z",
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
	-H "Authorization: Bearer ba20435af2f4bc21cf9a1497afb96f4b2d88d0a5ad8cb4a0124892f7e7cb5414"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer a8ae3b077bb797c97442a110a9a50f57d22703841204d8ca354b5f6e45569963
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
curl "api.goskive.com/v2/feedbacks/21/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8ae3b077bb797c97442a110a9a50f57d22703841204d8ca354b5f6e45569963"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/41/fix
Content-Type: application/json
Authorization: Bearer ada6d2ba48843ecf030d07dee70d6b09f53d8544c5f8142df5de98cd2c029100
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
curl "api.goskive.com/v2/feedbacks/41/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ada6d2ba48843ecf030d07dee70d6b09f53d8544c5f8142df5de98cd2c029100"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/fix
Content-Type: application/json
Authorization: Bearer c65473f8d7332ab0c1817178d6afdb1c0a8d05fa9024d7a57e2f1d34fb1cf1af
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
curl "api.goskive.com/v2/feedbacks/42/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c65473f8d7332ab0c1817178d6afdb1c0a8d05fa9024d7a57e2f1d34fb1cf1af"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/46
Content-Type: application/json
Authorization: Bearer bd9b84eee09f87578a475e755244a56eef10a347a6bbfd17edda252f2a94f9ec
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
    "user_id": 849,
    "feedbackable_id": 92,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T13:15:40.350Z",
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
	-H "Authorization: Bearer bd9b84eee09f87578a475e755244a56eef10a347a6bbfd17edda252f2a94f9ec"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/5
Content-Type: application/json
Authorization: Bearer 4545e26c5db035a19200f87da5f7be444ee275f84f8684cf5ab82fc4755a8c47
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4545e26c5db035a19200f87da5f7be444ee275f84f8684cf5ab82fc4755a8c47"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer aca5ac904b1b32eca2797ba2c481930b141ad5c3d401d3cee82205aecacaba7a
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aca5ac904b1b32eca2797ba2c481930b141ad5c3d401d3cee82205aecacaba7a"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/1
Content-Type: application/json
Authorization: Bearer 7ff2fbaa07faca75c5d1e7287fcc1e562e948807719368b27be0ea6f8b5e32b1
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/8b4bd4e7765b660fb8fec6663feccc27.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T131429Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=b762d9ee721d68d887671d4d986486d5f515468d38e145b2d7d411a0674bcc70"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ff2fbaa07faca75c5d1e7287fcc1e562e948807719368b27be0ea6f8b5e32b1"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/2/preview
Content-Type: application/json
Authorization: Bearer f61069f62397d639e770978a9cbf962a129610b854d181187948458848e0efba
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/68991a1da03da81645533464d7c4040f.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T131429Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=04b81bf2a98d1deaab16205dca174007daa1225d503023abf4764ead3277ead9"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/2/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f61069f62397d639e770978a9cbf962a129610b854d181187948458848e0efba"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Content-Type: application/json
Authorization: Bearer 7937d17958dbb8b44e5957bad6025b6ef69457f58a988d192d74d15df83efe6d
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
      "id": 56,
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
      "created_at": "2016-10-19T13:14:30.760Z",
      "updated_at": "2016-10-19T13:14:30.760Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-19T13:14:30.834Z",
    "updated_at": "2016-10-19T13:14:30.834Z",
    "course_id": 18,
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7937d17958dbb8b44e5957bad6025b6ef69457f58a988d192d74d15df83efe6d"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/11/matched_courses?required_cu_count=2
Authorization: Bearer e29208e5c5b6c76ac88d73709476cada0b4d6dfbd5015027c023745aeb3b2bfb
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
      "creator_id": 257,
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 92,
      "additional_university_ids": [

      ],
      "topic_id": 97,
      "discipline_id": 97,
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
      "chapters_updated_at": "2016-10-19T13:14:47.664Z",
      "updated_at": "2016-10-19T13:14:49.292Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 262,
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-0315b43b-85a1-4e52-910a-44f4dd3f56ac",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-0315b43b-85a1-4e52-910a-44f4dd3f56ac",
      "slug": "mit-the-great-british-bake-off-0315b43b-85a1-4e52-910a-44f4dd3f56ac",
      "university_id": 93,
      "additional_university_ids": [

      ],
      "topic_id": 98,
      "discipline_id": 98,
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
      "chapters_updated_at": "2016-10-19T13:14:47.664Z",
      "updated_at": "2016-10-19T13:14:49.855Z",
      "shortname": "mit-the-great-british-bake-off-0315b43b-85a1-4e52-910a-44f4dd3f56ac"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/11/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer e29208e5c5b6c76ac88d73709476cada0b4d6dfbd5015027c023745aeb3b2bfb"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/3/report
Content-Type: application/json
Authorization: Bearer 3bb64559e8d05e0fd7b2ab2332595fb9b52c6f7cec070c0ad5111796c8422888
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bb64559e8d05e0fd7b2ab2332595fb9b52c6f7cec070c0ad5111796c8422888"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/30/comments
Content-Type: application/json
Authorization: Bearer a3f8fbc36c6df7a51bf662cff3cdc0bbe9a74365379e558a091f47b8e819fa8b
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
    "id": 47,
    "author_id": 223,
    "reply_to_id": null,
    "created_at": "2016-10-19T13:14:45.717Z",
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
curl "api.goskive.com/v2/flashcards/30/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3f8fbc36c6df7a51bf662cff3cdc0bbe9a74365379e558a091f47b8e819fa8b"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/31/comments
Content-Type: application/json
Authorization: Bearer e3170bca21150ef04e31e0350853aec359ccc8ed4ccc640dc0ba2ec5f705ec48
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
    "id": 48,
    "author_id": 226,
    "reply_to_id": null,
    "created_at": "2016-10-19T13:14:46.072Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 226,
      "feedbackable_id": 31,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:46.068Z",
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
curl "api.goskive.com/v2/flashcards/31/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3170bca21150ef04e31e0350853aec359ccc8ed4ccc640dc0ba2ec5f705ec48"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/28/comments
Content-Type: application/json
Authorization: Bearer 673a7900e7b325cb2ea8439fb72ea38fb4190bafa4718ebf8aba36ec60a3ef20
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
      "id": 46,
      "author_id": 219,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:45.326Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 218,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:45.309Z",
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
curl "api.goskive.com/v2/flashcards/28/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 673a7900e7b325cb2ea8439fb72ea38fb4190bafa4718ebf8aba36ec60a3ef20"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/29/comments
Content-Type: application/json
Authorization: Bearer ea7404aeab8305a10f372188a61c2d1cdb9083ebd30a07496906536a6dec88f7
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
curl "api.goskive.com/v2/flashcards/29/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea7404aeab8305a10f372188a61c2d1cdb9083ebd30a07496906536a6dec88f7"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/45/feedbacks
Content-Type: application/json
Authorization: Bearer c4ab1f6f6b2b1409bbd1b58b0ae029cb654e058d66ae6c47b9889e4bbe36277e
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
    "id": 12,
    "user_id": 442,
    "feedbackable_id": 45,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T13:15:05.907Z",
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
curl "api.goskive.com/v2/flashcards/45/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4ab1f6f6b2b1409bbd1b58b0ae029cb654e058d66ae6c47b9889e4bbe36277e"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/47/feedbacks
Content-Type: application/json
Authorization: Bearer b4273fba13c315dac39aa66c7215744c88d0e3ea7039e860e40015d18c2ca2f7
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
      "id": 14,
      "user_id": 452,
      "feedbackable_id": 47,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:06.473Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 451,
      "feedbackable_id": 47,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:15:06.461Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/47/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4273fba13c315dac39aa66c7215744c88d0e3ea7039e860e40015d18c2ca2f7"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/94/votes
Content-Type: application/json
Authorization: Bearer 5e56abf9522c5269e67a08a4e7eb10109b1475e1ed9af7f66ad44070db19f1c7
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
      "votable_id": 94,
      "user_id": 966
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 965
    },
    {
      "id": 19,
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
	-H "Authorization: Bearer 5e56abf9522c5269e67a08a4e7eb10109b1475e1ed9af7f66ad44070db19f1c7"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/75/republish
Content-Type: application/json
Authorization: Bearer b4940a425789c719d1ac42b11522c612f967408a713504e447c3595b378e97e6
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
curl "api.goskive.com/v2/flashcards/75/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4940a425789c719d1ac42b11522c612f967408a713504e447c3595b378e97e6"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/52/bookmark
Content-Type: application/json
Authorization: Bearer 8f015b1a55ee43cf4424feafe4bb1c9377b4802bf18815f0bc7a5809dee768a5
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/52/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f015b1a55ee43cf4424feafe4bb1c9377b4802bf18815f0bc7a5809dee768a5"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/73
Content-Type: application/json
Authorization: Bearer 659dd01073beb04bb0e9cae163a86f02e0e009e0c80f5762c26d02908a8e4699
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 659dd01073beb04bb0e9cae163a86f02e0e009e0c80f5762c26d02908a8e4699"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/53/downvote
Content-Type: application/json
Authorization: Bearer d4f5972932bba45dc6f57bcc163fe31c476e013d1fcad2efb178a3b0a7979fb7
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/53/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4f5972932bba45dc6f57bcc163fe31c476e013d1fcad2efb178a3b0a7979fb7"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/56
Content-Type: application/json
Authorization: Bearer 481503ec4d72553528975069d5b67b0d39059c98bd51a51a3acabc9f0e3d0d62
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
    "id": 56,
    "obfuscated_id": "PgrpyPCfpqo",
    "author_id": 512,
    "chapter_id": 102,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:11.286Z",
    "created_at": "2016-10-19T13:15:11.286Z",
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
curl "api.goskive.com/v2/flashcards/56" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 481503ec4d72553528975069d5b67b0d39059c98bd51a51a3acabc9f0e3d0d62"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/72/report
Content-Type: application/json
Authorization: Bearer 66f7f9f5d728351fb2ca1685c19ad62a49d97d238e4fe245ee93c9989d01a14f
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66f7f9f5d728351fb2ca1685c19ad62a49d97d238e4fe245ee93c9989d01a14f"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/54/bookmark
Content-Type: application/json
Authorization: Bearer fd95289c9bdd71a2f484683f5fcffd9e5b693a5386e1df5fdf5d9285803b6cd0
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/54/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd95289c9bdd71a2f484683f5fcffd9e5b693a5386e1df5fdf5d9285803b6cd0"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/55/upvote
Content-Type: application/json
Authorization: Bearer bf650e4ccd50e77609a255a9c6320ab7173b2cb07c9bd987e54e747c9cf64bd5
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/55/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf650e4ccd50e77609a255a9c6320ab7173b2cb07c9bd987e54e747c9cf64bd5"
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
    "key": "cache/41a865acbcbcc0245e7de8e512ecd093.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxNDoxNTozMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS80MWE4NjVhY2JjYmNjMDI0NWU3ZGU4ZTUxMmVjZDA5My5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE5L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOVQxMzE1MzFaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T131531Z",
    "x-amz-signature": "c2c26da5f4f1fc2bcef65416529946561444f818a71c3ced80321866b50ace4c"
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
Authorization: Bearer 3e32b41cf95556d95a96b3607c71a3b4c7590c34be2771c7bb24e7613bab173b
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
	-H "Authorization: Bearer 3e32b41cf95556d95a96b3607c71a3b4c7590c34be2771c7bb24e7613bab173b"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 989bd293a1eff24b746a218b3c063f6a0b99afedbd189ca90ce93f10bbe0917e
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
	-H "Authorization: Bearer 989bd293a1eff24b746a218b3c063f6a0b99afedbd189ca90ce93f10bbe0917e"
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
{"password":{"reset_password_token":"iWygKS-aH5xK6ix-emoy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 597,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-19T13:15:18.520Z",
  "updated_at": "2016-10-19T13:15:18.660Z",
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
  "audit_id": 4395
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"iWygKS-aH5xK6ix-emoy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/46/comments
Content-Type: application/json
Authorization: Bearer 4f623c027a4a120a33da129677bec13cfd097b4a9be46d7fe0d090febbd2699e
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
    "id": 52,
    "author_id": 283,
    "reply_to_id": null,
    "created_at": "2016-10-19T13:14:51.406Z",
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
curl "api.goskive.com/v2/questions/46/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f623c027a4a120a33da129677bec13cfd097b4a9be46d7fe0d090febbd2699e"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/47/comments
Content-Type: application/json
Authorization: Bearer 84d7d65a792a91deadd2ed3dee384ff2b279c5d83c8c832aac09033b51c729c1
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
    "id": 53,
    "author_id": 286,
    "reply_to_id": null,
    "created_at": "2016-10-19T13:14:51.914Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 2,
      "user_id": 286,
      "feedbackable_id": 47,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:51.911Z",
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
curl "api.goskive.com/v2/questions/47/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84d7d65a792a91deadd2ed3dee384ff2b279c5d83c8c832aac09033b51c729c1"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/49/comments
Content-Type: application/json
Authorization: Bearer b8b72b310e8204c273069bfceeca4f02cc83c319b354f21dc205c0b23fce3f5a
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
      "author_id": 295,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:52.693Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 296,
      "reply_to_id": null,
      "created_at": "2016-10-19T13:14:52.709Z",
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
curl "api.goskive.com/v2/questions/49/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8b72b310e8204c273069bfceeca4f02cc83c319b354f21dc205c0b23fce3f5a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/48/comments
Content-Type: application/json
Authorization: Bearer 1d9e8873b0bc8cd6f0609468f9f684d912de7a09e30888c9b1c77594406aaaf0
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
curl "api.goskive.com/v2/questions/48/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d9e8873b0bc8cd6f0609468f9f684d912de7a09e30888c9b1c77594406aaaf0"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/58/feedbacks
Content-Type: application/json
Authorization: Bearer faa2309c246c6e66cc96a39eb2623e196a86f19148adf42fbe270a8bb0f40725
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
    "user_id": 333,
    "feedbackable_id": 58,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-19T13:14:56.657Z",
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
curl "api.goskive.com/v2/questions/58/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faa2309c246c6e66cc96a39eb2623e196a86f19148adf42fbe270a8bb0f40725"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/55/feedbacks
Content-Type: application/json
Authorization: Bearer d26fabe82836af190dc0e4fd05cb6d668548d5faff6d6415d45d7eda0c380a39
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
      "id": 8,
      "user_id": 326,
      "feedbackable_id": 55,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:55.241Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 325,
      "feedbackable_id": 55,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T13:14:55.225Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/55/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d26fabe82836af190dc0e4fd05cb6d668548d5faff6d6415d45d7eda0c380a39"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/59/votes
Content-Type: application/json
Authorization: Bearer f1f5013485711f296bd90dc2ac416d8e7d1d41e57124fd90491e23136beb04f8
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
      "votable_id": 59,
      "user_id": 341
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 340
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 339
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/59/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1f5013485711f296bd90dc2ac416d8e7d1d41e57124fd90491e23136beb04f8"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/112/republish
Content-Type: application/json
Authorization: Bearer b56de5dc27487734d6a296c05e353b7f18f5794bdfdee18d44a7349767cc3c1b
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
curl "api.goskive.com/v2/questions/112/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b56de5dc27487734d6a296c05e353b7f18f5794bdfdee18d44a7349767cc3c1b"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/134/bookmark
Content-Type: application/json
Authorization: Bearer 5a46a08300b965aa2d14801db4b5181bbc8227b925fc6630148af7c64b3080aa
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/134/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a46a08300b965aa2d14801db4b5181bbc8227b925fc6630148af7c64b3080aa"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/113
Content-Type: application/json
Authorization: Bearer e8fd889f2c291b666347c7aa08af26c6558b6bd355c781fa631c9edcc9f687a0
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
	-H "Authorization: Bearer e8fd889f2c291b666347c7aa08af26c6558b6bd355c781fa631c9edcc9f687a0"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/130/downvote
Content-Type: application/json
Authorization: Bearer c1213c7ca0411e75c386ed22e67be9af94f32767494c0de9c77cac86cf7c3ae9
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/130/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1213c7ca0411e75c386ed22e67be9af94f32767494c0de9c77cac86cf7c3ae9"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/110
Content-Type: application/json
Authorization: Bearer 3a53188641a36259ca56c3f0fbb3240fa100d1cd227b4b963f031a2ed29dc16b
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
    "id": 110,
    "obfuscated_id": "55JK4PuG2Hk",
    "author_id": 872,
    "chapter_id": 168,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:41.607Z",
    "created_at": "2016-10-19T13:15:41.495Z",
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
        "id": 222,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 223,
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
curl "api.goskive.com/v2/questions/110" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a53188641a36259ca56c3f0fbb3240fa100d1cd227b4b963f031a2ed29dc16b"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/129/report
Content-Type: application/json
Authorization: Bearer 1fbc90b512bfa5981fd06602f719c3a03c7d340a67240f9b7e83f42314719907
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/129/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fbc90b512bfa5981fd06602f719c3a03c7d340a67240f9b7e83f42314719907"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/133/bookmark
Content-Type: application/json
Authorization: Bearer 15e6ce2c8713744914df86dd3045cc2cb4bce2b722a4052ced9656576d5d55be
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/133/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15e6ce2c8713744914df86dd3045cc2cb4bce2b722a4052ced9656576d5d55be"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/132
Content-Type: application/json
Authorization: Bearer 292ea754cef7638651551044ac35e406bf02ee8f8bece2084d0d0c641dcf1869
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":132,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T13:15:49.847Z","updated_at":"2016-10-19T13:15:49.994Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":190,"author_id":943,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 132,
    "obfuscated_id": "RECRPLqMrqE",
    "author_id": 943,
    "chapter_id": 190,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T13:15:50.132Z",
    "created_at": "2016-10-19T13:15:49.847Z",
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
    "question": "{\"id\"=>132, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-19T13:15:49.847Z\", \"updated_at\"=>\"2016-10-19T13:15:49.994Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>190, \"author_id\"=>943, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 266,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 267,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 268,
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
curl "api.goskive.com/v2/questions/132" -d '{"question":{"question":{"id":132,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T13:15:49.847Z","updated_at":"2016-10-19T13:15:49.994Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":190,"author_id":943,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 292ea754cef7638651551044ac35e406bf02ee8f8bece2084d0d0c641dcf1869"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/131/upvote
Content-Type: application/json
Authorization: Bearer 4a8ea973bc67fc901cf489fbf64b028368faf08bbec1954795fc770042f78a41
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
	-H "Authorization: Bearer 4a8ea973bc67fc901cf489fbf64b028368faf08bbec1954795fc770042f78a41"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 3f6060609c229604cd0dae7934e9be29ea2cedb3075077ce8993c312f1bdbc91
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
      "creator_id": 705,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "topic_id": 251,
      "discipline_id": 252,
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
      "updated_at": "2016-10-19T13:15:28.745Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f6060609c229604cd0dae7934e9be29ea2cedb3075077ce8993c312f1bdbc91"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 9767e98e269f5655d6e4aeaad2810a160f325565d5fd567dce87e7aa2b463c63
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
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-204",
      "html_url": "https://goskive.com/university/uni-204",
      "slug": "uni-204",
      "name": "National School of Pizza",
      "short_name": "Uni 204",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a84bf632b347637bac652448b90e5f6222b618e0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/abfbb312a94690ff6ff345279fab061786255995.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T13:15:28.424Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-203",
      "html_url": "https://goskive.com/university/uni-203",
      "slug": "uni-203",
      "name": "National School of Pastry",
      "short_name": "Uni 203",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/509cfb4345634e438ae043d2afe3ad13be7a04cf.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9413f9633b8ed5dc93a2bb997bd39d06ed3dc5b4.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T13:15:28.406Z",
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
	-H "Authorization: Bearer 9767e98e269f5655d6e4aeaad2810a160f325565d5fd567dce87e7aa2b463c63"
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
      "id": 244,
      "name": "Inverse web-enabled emulation",
      "name_translations": {
        "en": "Inverse web-enabled emulation"
      },
      "discipline_id": 245
    },
    {
      "id": 245,
      "name": "Networked homogeneous internet solution",
      "name_translations": {
        "en": "Networked homogeneous internet solution"
      },
      "discipline_id": 246
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
GET /v2/topics/243
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
    "id": 243,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 244
  }
}
```



```shell
curl "api.goskive.com/v2/topics/243" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 73d82f580bc1a4c623b14243abaec1490e157e10142239c54540dc2d992c2e28
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
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-187",
      "html_url": "https://goskive.com/university/uni-187",
      "slug": "uni-187",
      "name": "University 136",
      "short_name": "Uni 187",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d49d24f5d0070561e7d4979d39ae424d6987e402.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/5e31fbf583340c7e443c78afcb4da7e62af53ad7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T13:15:24.342Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-188",
      "html_url": "https://goskive.com/university/uni-188",
      "slug": "uni-188",
      "name": "University 137",
      "short_name": "Uni 188",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c1bcbe98f5e30a1d2c062d00e265207a3c76c1d6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3db8b7a7fd23a5908ee95827523b8d2a965fac10.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T13:15:24.359Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-189",
      "html_url": "https://goskive.com/university/uni-189",
      "slug": "uni-189",
      "name": "University 138",
      "short_name": "Uni 189",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/94a8023f21254ce163a5b5ede98bdc819440a3a0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6d49f3aa5d676dcd5fa043f4ff8e782f8f1ac73f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T13:15:24.376Z",
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
	-H "Authorization: Bearer 73d82f580bc1a4c623b14243abaec1490e157e10142239c54540dc2d992c2e28"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer bacde0d5647d7f4e556984801d779c37320c52c63ea4c8bc79895de668667572
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
    "id": 205,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/251a3379388b624d381a43405118f30764fe4f9f.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7ed7b255515aee55da5cb2e74b72737d8381795f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-19T13:15:24.161Z",
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
	-H "Authorization: Bearer bacde0d5647d7f4e556984801d779c37320c52c63ea4c8bc79895de668667572"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 28ac68ea67ea945bab0f06a7bee5fb3445cef0850106237321c6330e634bb2d1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":224,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 642,
    "id": 219,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 197,
    "additional_university_ids": [

    ],
    "topic_id": 224,
    "discipline_id": 224,
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
    "chapters_updated_at": "2016-10-19T13:15:22.890Z",
    "updated_at": "2016-10-19T13:15:23.049Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 130,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-19T13:15:22.992Z",
        "course_id": 219,
        "author_id": 642,
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
        "id": 131,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-19T13:15:23.013Z",
        "course_id": 219,
        "author_id": 642,
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
        "id": 132,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-19T13:15:23.034Z",
        "course_id": 219,
        "author_id": 642,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":224,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28ac68ea67ea945bab0f06a7bee5fb3445cef0850106237321c6330e634bb2d1"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b43d0cb4888524cc5c5a910e99380997cd58dd2e07db4db3fa6f99869cc426a9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":225,"published":false}}
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
    "creator_id": 643,
    "id": 220,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 198,
    "additional_university_ids": [

    ],
    "topic_id": 225,
    "discipline_id": 225,
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
    "updated_at": "2016-10-19T13:15:23.202Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":225,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b43d0cb4888524cc5c5a910e99380997cd58dd2e07db4db3fa6f99869cc426a9"
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
      "creator_id": 614,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-144",
      "html_url": "https://goskive.com/course/fu-course-144",
      "slug": "fu-course-144",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 200,
      "discipline_id": 200,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 144",
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
      "updated_at": "2016-10-19T13:15:20.152Z",
      "shortname": "fu-course-144"
    },
    {
      "creator_id": 614,
      "id": 196,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "topic_id": 201,
      "discipline_id": 201,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
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
      "chapters_updated_at": "2016-10-19T13:15:20.469Z",
      "updated_at": "2016-10-19T13:15:20.476Z",
      "shortname": "fu-course-145"
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
Authorization: Bearer 5da5ac63cc40106436575ec335045bd520a3331c9564b602f8e7092211b88edf
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
      "creator_id": 621,
      "id": 203,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "topic_id": 208,
      "discipline_id": 208,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
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
      "updated_at": "2016-10-19T13:15:20.920Z",
      "shortname": "fu-course-152"
    },
    {
      "creator_id": 621,
      "id": 204,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "topic_id": 209,
      "discipline_id": 209,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 153",
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
      "chapters_updated_at": "2016-10-19T13:15:21.243Z",
      "updated_at": "2016-10-19T13:15:21.251Z",
      "shortname": "fu-course-153"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5da5ac63cc40106436575ec335045bd520a3331c9564b602f8e7092211b88edf"
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
      "creator_id": 619,
      "id": 199,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 187,
      "additional_university_ids": [

      ],
      "topic_id": 204,
      "discipline_id": 204,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
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
      "updated_at": "2016-10-19T13:15:20.662Z",
      "shortname": "fu-course-148"
    },
    {
      "creator_id": 619,
      "id": 200,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 187,
      "additional_university_ids": [

      ],
      "topic_id": 205,
      "discipline_id": 205,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
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
      "updated_at": "2016-10-19T13:15:20.702Z",
      "shortname": "fu-course-149"
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
Authorization: Bearer d11d54b582c706d77500b3c918bad4ebc86f0cf482ae129bff50139927a80140
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
      "creator_id": 628,
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "topic_id": 212,
      "discipline_id": 212,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 156",
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
      "updated_at": "2016-10-19T13:15:21.536Z",
      "shortname": "fu-course-156"
    },
    {
      "creator_id": 628,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-157",
      "html_url": "https://goskive.com/course/fu-course-157",
      "slug": "fu-course-157",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "topic_id": 213,
      "discipline_id": 213,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 157",
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
      "updated_at": "2016-10-19T13:15:21.576Z",
      "shortname": "fu-course-157"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d11d54b582c706d77500b3c918bad4ebc86f0cf482ae129bff50139927a80140"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 8b5aeca86d59d5c61ebfa12c96ce25f2273cd3af4d50bd9c18f3d472055728c9
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
  "id": 712,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-19T13:15:29.451Z",
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
	-H "Authorization: Bearer 8b5aeca86d59d5c61ebfa12c96ce25f2273cd3af4d50bd9c18f3d472055728c9"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/854
Content-Type: application/json
Authorization: Bearer c3a90f21c4efa00161f861f3806214d104c086c8b97fc39709c7e7b32196e533
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
    "id": 854,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 262,
    "fields_of_study": [
      288,
      289
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-19T13:15:40.537Z",
    "updated_at": "2016-10-19T13:15:40.537Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/854" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3a90f21c4efa00161f861f3806214d104c086c8b97fc39709c7e7b32196e533"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/856
Content-Type: application/json
Authorization: Bearer 6c0516e168b6ae70dc4bf2735e3cb98416fb762ba923b35d68f2e04fd9c440f2
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
    "id": 856,
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
    "created_at": "2016-10-19T13:15:40.626Z",
    "updated_at": "2016-10-19T13:15:40.626Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/856" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c0516e168b6ae70dc4bf2735e3cb98416fb762ba923b35d68f2e04fd9c440f2"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/14
Content-Type: application/json
Authorization: Bearer c204268e9e609d04da1e89deda8735863c164ce87d799a9a75dccb74453d29b7
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c204268e9e609d04da1e89deda8735863c164ce87d799a9a75dccb74453d29b7"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/16
Content-Type: application/json
Authorization: Bearer 320ec96e2e618317849441f80395e351273a568de2c708909a655a1c0599a251
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
    "id": 16,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 90,
    "user_id": 721
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 320ec96e2e618317849441f80395e351273a568de2c708909a655a1c0599a251"
```
