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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"cdae92422894967781062b8617c53b2bb5b8cd81f8aeaf26ec0fc18a60fa55e2","client_secret":"350bb7c22c09e58977480a38faa46f63f852dfc6630dbfd64a61b181b98edceb"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"cdae92422894967781062b8617c53b2bb5b8cd81f8aeaf26ec0fc18a60fa55e2","client_secret":"350bb7c22c09e58977480a38faa46f63f852dfc6630dbfd64a61b181b98edceb"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDBjNmI5MGFlNGZlM2RkOWYxODIwOWVhYzNkNjAwOWI1MzBmNWRiZTZjMmNj
YWYzYzBkZjdlZWY5YTNhYjUzZTozYWIwYjcwZjY4NjVmZDdkNTFlZTM5NWNk
NTZkZGUwMWE0NGJmNjBiNDJlZjI0ZTE1NmI5MDljNGZhNmY5NDE3

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
	-u d0c6b90ae4fe3dd9f18209eac3d6009b530f5dbe6c2ccaf3c0df7eef9a3ab53e:3ab0b70f6865fd7d51ee395cd56dde01a44bf60b42ef24e156b909c4fa6f9417
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
{"grant_type":"client_credentials","client_id":"27e261aee7668af29552fba7a06dfd377218d9b51cd6ecbceb620423243433e8","client_secret":"e1a56b32f9ab23e6dfa298c65aaf3773fb97250be4ecdcfd0261f277c040ca3f"}
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
  "access_token": "16c60113fa4a1ea03010941147aec57e5f4e1ca128460ae8db948c2767680153",
  "token_type": "bearer",
  "created_at": 1477511119
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"27e261aee7668af29552fba7a06dfd377218d9b51cd6ecbceb620423243433e8","client_secret":"e1a56b32f9ab23e6dfa298c65aaf3773fb97250be4ecdcfd0261f277c040ca3f"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cffe7ee321d1fde12d0b4dd58891add4a2a45ad14bd3088ac258c9e085ec48c0","client_secret":"ed2637474e69a21acdce78512c3ef1a015d73045ad743383984e1242efab2af2"}
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
  "access_token": "2fb07b35beb4d9af8905bc0a877ae2770158648aa707c96951dd2c9576918b4b",
  "token_type": "bearer",
  "created_at": 1477511119
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"cffe7ee321d1fde12d0b4dd58891add4a2a45ad14bd3088ac258c9e085ec48c0","client_secret":"ed2637474e69a21acdce78512c3ef1a015d73045ad743383984e1242efab2af2"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NzdkOWM4M2ZmODMwMGQwMGQwNTA4ZjE0NTkzNzA2MjAxOWExZDhmMGU0YWIy
MzNmYjViMmIxNWQwYTRmZWJjZToyNjk0N2U4YTUzNWM5Y2FlYzM4ZDYwNzgz
ZjllYWFkMDNlNGYzMWQzZmM1NmNhYmZkOGViMjgxMTE3YjQ0MTJk

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
  "access_token": "1af79399b26079f4fc9d677964c7b7aa6f15e62c914693939b408ba00bd63bed",
  "token_type": "bearer",
  "created_at": 1477511119
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 77d9c83ff8300d00d0508f145937062019a1d8f0e4ab233fb5b2b15d0a4febce:26947e8a535c9caec38d60783f9eaad03e4f31d3fc56cabfd8eb281117b4412d
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
Authorization: Bearer ad9caf733fe0b8f180277a2e3bb532ee6a76726ce783709f82954c1e3d3f3a3d
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
	-H "Authorization: Bearer ad9caf733fe0b8f180277a2e3bb532ee6a76726ce783709f82954c1e3d3f3a3d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/148/flashcards
Content-Type: application/json
Authorization: Bearer 65d69bfb2937bd0c8e6f99a6d4ccaa1533394a2de23ed62fb559e0e9644d00e8
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":148,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 58,
    "obfuscated_id": "_S2mxc1kfck",
    "author_id": 762,
    "chapter_id": 148,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:48.531Z",
    "created_at": "2016-10-26T19:45:48.531Z",
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
curl "api.goskive.com/v2/chapters/148/flashcards" -d '{"flashcard":{"chapter_id":148,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65d69bfb2937bd0c8e6f99a6d4ccaa1533394a2de23ed62fb559e0e9644d00e8"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/149/flashcards
Content-Type: application/json
Authorization: Bearer b70a18d68ddcccc937776f24e32f71a39c378df1b34464f180d7c7413187afda
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 763,
      "chapter_id": 149,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:48.669Z",
      "created_at": "2016-10-26T19:45:48.669Z",
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
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 763,
      "chapter_id": 149,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:48.703Z",
      "created_at": "2016-10-26T19:45:48.703Z",
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 763,
      "chapter_id": 149,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:48.737Z",
      "created_at": "2016-10-26T19:45:48.737Z",
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
	-H "Authorization: Bearer b70a18d68ddcccc937776f24e32f71a39c378df1b34464f180d7c7413187afda"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/120/questions
Content-Type: application/json
Authorization: Bearer 895f5f6274234c402547096f75289c01e51fcf070df53d854d1953f9368c54b6
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":120,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 70,
    "obfuscated_id": "EDEz1xzotLc",
    "author_id": 554,
    "chapter_id": 120,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:37.467Z",
    "created_at": "2016-10-26T19:45:37.467Z",
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
        "id": 141,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 142,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 143,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 144,
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
curl "api.goskive.com/v2/chapters/120/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":120,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 895f5f6274234c402547096f75289c01e51fcf070df53d854d1953f9368c54b6"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/118/questions
Content-Type: application/json
Authorization: Bearer fa2aefc1733f5325af56138715327f87055fc2cda91cad821566e866fbdce2dd
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 548,
    "chapter_id": 118,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:36.820Z",
    "created_at": "2016-10-26T19:45:36.820Z",
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
curl "api.goskive.com/v2/chapters/118/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa2aefc1733f5325af56138715327f87055fc2cda91cad821566e866fbdce2dd"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/119/questions
Content-Type: application/json
Authorization: Bearer 6475b008588ef6effbf830bf1e060a9dd928575a9d0216073478e4739165de63
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":119,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 69,
    "obfuscated_id": "1EDi_PBgOnI",
    "author_id": 551,
    "chapter_id": 119,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:37.143Z",
    "created_at": "2016-10-26T19:45:37.143Z",
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
        "id": 139,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 140,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/119/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":119,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6475b008588ef6effbf830bf1e060a9dd928575a9d0216073478e4739165de63"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/117/questions
Content-Type: application/json
Authorization: Bearer 5fe7d7fba1d235c6ec808e37c2d573d242a2bc5ce64a4d7c84837da2341f4c24
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":117,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 545,
    "chapter_id": 117,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:36.419Z",
    "created_at": "2016-10-26T19:45:36.419Z",
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
curl "api.goskive.com/v2/chapters/117/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":117,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fe7d7fba1d235c6ec808e37c2d573d242a2bc5ce64a4d7c84837da2341f4c24"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/122/questions
Content-Type: application/json
Authorization: Bearer 7dfafd7be1b8cd7343eef00577bdc3010236aef606dc498a1cf181c632f59db4
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
      "author_id": 560,
      "chapter_id": 122,
      "position": 58,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:38.169Z",
      "created_at": "2016-10-26T19:45:38.054Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 561,
      "chapter_id": 122,
      "position": 59,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:38.354Z",
      "created_at": "2016-10-26T19:45:38.239Z",
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
        }
      ]
    },
    {
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 562,
      "chapter_id": 122,
      "position": 60,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:38.542Z",
      "created_at": "2016-10-26T19:45:38.424Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/122/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dfafd7be1b8cd7343eef00577bdc3010236aef606dc498a1cf181c632f59db4"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/194
Content-Type: application/json
Authorization: Bearer 8106d2aecd95a02173a899ff8e06289e67fce80e260dff3ff417e51b5fda928f
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
curl "api.goskive.com/v2/chapters/194" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8106d2aecd95a02173a899ff8e06289e67fce80e260dff3ff417e51b5fda928f"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/195
Content-Type: application/json
Authorization: Bearer 66199b3017458374e71a6f60396922017a3027087b956250e559d271e22ff11c
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
	-H "Authorization: Bearer 66199b3017458374e71a6f60396922017a3027087b956250e559d271e22ff11c"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/187
Content-Type: application/json
Authorization: Bearer e5f3e11143335b6dc8d5249c9fa7bdef8fe1491f9ca634845558dc341ae44e15
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
curl "api.goskive.com/v2/chapters/187" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5f3e11143335b6dc8d5249c9fa7bdef8fe1491f9ca634845558dc341ae44e15"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/193
Content-Type: application/json
Authorization: Bearer 044f6c01a86765881edb1a21a1962e0c7cdda30c5b36a5c2f875fe9b55d10b59
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/193" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 044f6c01a86765881edb1a21a1962e0c7cdda30c5b36a5c2f875fe9b55d10b59"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 6edb5f51a28fd430fe49cb8f7cbca077aa1fa704ebc7576e43ec5c96bee9d543
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
    "id": 191,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T19:46:10.628Z",
    "course_id": 308,
    "author_id": 961,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-26T19:46:10.104Z",
    "questions_updated_at": "2016-10-26T19:46:10.104Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 965,
        "chapter_id": 191,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:10.612Z",
        "created_at": "2016-10-26T19:46:10.612Z",
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
        "id": 132,
        "obfuscated_id": "RECRPLqMrqE",
        "author_id": 963,
        "chapter_id": 191,
        "position": 119,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:10.508Z",
        "created_at": "2016-10-26T19:46:10.386Z",
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
            "id": 267,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 268,
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
curl "api.goskive.com/v2/chapters/191" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6edb5f51a28fd430fe49cb8f7cbca077aa1fa704ebc7576e43ec5c96bee9d543"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/188
Content-Type: application/json
Authorization: Bearer 4cd48f6d4e8b7db2fe66e0e6f767cc0e6ac9dfc9d4468fb8dd847cfd774b328f
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
    "updated_at": "2016-10-26T19:46:09.268Z",
    "course_id": 305,
    "author_id": 949,
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
	-H "Authorization: Bearer 4cd48f6d4e8b7db2fe66e0e6f767cc0e6ac9dfc9d4468fb8dd847cfd774b328f"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/54/replies
Content-Type: application/json
Authorization: Bearer 8376645751f1a290ce3e62274392ab9da6851ce1f98f7ae4fb1ec5eda0ab2789
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
    "id": 55,
    "author_id": 843,
    "reply_to_id": 54,
    "created_at": "2016-10-26T19:45:55.600Z",
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
curl "api.goskive.com/v2/comments/54/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8376645751f1a290ce3e62274392ab9da6851ce1f98f7ae4fb1ec5eda0ab2789"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer 871d0d0c2ecece7b1410eec8975c7692367adb84b7a4d59744015133081ca62a
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
	-H "Authorization: Bearer 871d0d0c2ecece7b1410eec8975c7692367adb84b7a4d59744015133081ca62a"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/14
Content-Type: application/json
Authorization: Bearer 358bafa41236f6f44ee49941fdf600e8d27f2e4a27a22fd68f7f88f4c39598cc
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
curl "api.goskive.com/v2/comments/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 358bafa41236f6f44ee49941fdf600e8d27f2e4a27a22fd68f7f88f4c39598cc"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/13/republish
Content-Type: application/json
Authorization: Bearer da16cfe1715c3ad8f07fbcaf55249603f2f62a11e1533bc0036ac43604628ec0
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
curl "api.goskive.com/v2/comments/13/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da16cfe1715c3ad8f07fbcaf55249603f2f62a11e1533bc0036ac43604628ec0"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/16
Content-Type: application/json
Authorization: Bearer bfc3d83ed7082dd4385b2f8d6f57d954a9c4778580fd2a71deec2674a210e342
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfc3d83ed7082dd4385b2f8d6f57d954a9c4778580fd2a71deec2674a210e342"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/11/report
Content-Type: application/json
Authorization: Bearer c0fa801bd5f9ccfd81abc9e6e1726aef265af55ac12f5a8d3cd6308d54313980
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0fa801bd5f9ccfd81abc9e6e1726aef265af55ac12f5a8d3cd6308d54313980"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer 127cc699bbb05f339a12c2c4cd4660ac5fd5442220bcd2b6c2674e9604fdf596
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
    "id": 4,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-26T19:45:07.721Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 127cc699bbb05f339a12c2c4cd4660ac5fd5442220bcd2b6c2674e9604fdf596"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 4b41efc11a986846880fffc0c2789f66ab20455c9a0a03ec5810e0525c7986aa
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
      "id": 1,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:45:07.604Z"
    },
    {
      "id": 2,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:45:07.608Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:45:07.611Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b41efc11a986846880fffc0c2789f66ab20455c9a0a03ec5810e0525c7986aa"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer d81f65be4f96d16d421ef699a03d2032101071fc2f5364edc04f93def7e73fb2
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
	-H "Authorization: Bearer d81f65be4f96d16d421ef699a03d2032101071fc2f5364edc04f93def7e73fb2"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer ac126adbe7f5227b000998dac23f444d3f47cfabb4f014676e94513d65708d15
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
	-H "Authorization: Bearer ac126adbe7f5227b000998dac23f444d3f47cfabb4f014676e94513d65708d15"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 354b214a75778a6e6e48a8bd37a0d08f6be673258c1c7ac9db5808ecd1d70da2
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
      "company_id": 11,
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
      "company_id": 14,
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
	-H "Authorization: Bearer 354b214a75778a6e6e48a8bd37a0d08f6be673258c1c7ac9db5808ecd1d70da2"
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
Authorization: Bearer 61c13e875d34fb133c0e79c42e01293be19e04d4da54efdbf52582ef236d9168
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
	-H "Authorization: Bearer 61c13e875d34fb133c0e79c42e01293be19e04d4da54efdbf52582ef236d9168"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 399dc66991e32757a0f1554c9f84c9317af190629b2c25a2d5c26d8433242ea6
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
    "id": 93,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:45:33.316Z",
    "course_id": 158,
    "author_id": 487,
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
	-H "Authorization: Bearer 399dc66991e32757a0f1554c9f84c9317af190629b2c25a2d5c26d8433242ea6"
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
      "id": 95,
      "title": "Clever Chapter Title 89",
      "position": 1,
      "updated_at": "2016-10-26T19:45:33.564Z",
      "course_id": 160,
      "author_id": 491,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 96,
      "title": "Clever Chapter Title 90",
      "position": 2,
      "updated_at": "2016-10-26T19:45:33.588Z",
      "course_id": 160,
      "author_id": 492,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 97,
      "title": "Clever Chapter Title 91",
      "position": 3,
      "updated_at": "2016-10-26T19:45:33.839Z",
      "course_id": 160,
      "author_id": 493,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T19:45:33.484Z",
      "questions_updated_at": "2016-10-26T19:45:33.484Z",
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
Authorization: Bearer 9f6641f277a40ded5dfdcf64bf6197adc82aa0fad6c21b2fe6405c05872c4b36
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
      "title": "Clever Chapter Title 101",
      "position": 1,
      "updated_at": "2016-10-26T19:45:34.966Z",
      "course_id": 166,
      "author_id": 516,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 108,
      "title": "Clever Chapter Title 102",
      "position": 2,
      "updated_at": "2016-10-26T19:45:34.989Z",
      "course_id": 166,
      "author_id": 517,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 109,
      "title": "Clever Chapter Title 103",
      "position": 3,
      "updated_at": "2016-10-26T19:45:35.240Z",
      "course_id": 166,
      "author_id": 518,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T19:45:34.894Z",
      "questions_updated_at": "2016-10-26T19:45:34.894Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f6641f277a40ded5dfdcf64bf6197adc82aa0fad6c21b2fe6405c05872c4b36"
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
      "id": 98,
      "title": "Clever Chapter Title 92",
      "position": 1,
      "updated_at": "2016-10-26T19:45:34.044Z",
      "course_id": 162,
      "author_id": 498,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 99,
      "title": "Clever Chapter Title 93",
      "position": 2,
      "updated_at": "2016-10-26T19:45:34.069Z",
      "course_id": 162,
      "author_id": 499,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 100,
      "title": "Clever Chapter Title 94",
      "position": 3,
      "updated_at": "2016-10-26T19:45:34.093Z",
      "course_id": 162,
      "author_id": 500,
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
Authorization: Bearer 09b5035ce939b4f17cb2f7a8a9135aef053da5aa816ec32a71480b670b75a899
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
      "title": "Clever Chapter Title 104",
      "position": 1,
      "updated_at": "2016-10-26T19:45:35.391Z",
      "course_id": 167,
      "author_id": 523,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 111,
      "title": "Clever Chapter Title 105",
      "position": 2,
      "updated_at": "2016-10-26T19:45:35.415Z",
      "course_id": 167,
      "author_id": 524,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 112,
      "title": "Clever Chapter Title 106",
      "position": 3,
      "updated_at": "2016-10-26T19:45:35.439Z",
      "course_id": 167,
      "author_id": 525,
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
	-H "Authorization: Bearer 09b5035ce939b4f17cb2f7a8a9135aef053da5aa816ec32a71480b670b75a899"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7c86bae90d02dc86b213569fabd559ee8e8d3e240053983fb7477f0af902b3a6
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
    "course_id": 183,
    "user_id": 579,
    "updated_at": "2016-10-26T19:45:39.566Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c86bae90d02dc86b213569fabd559ee8e8d3e240053983fb7477f0af902b3a6"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer ebadef210c02160044878dceeefdcbaede72217d242d29ad36e207550988beb1
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
      "course_id": 179,
      "user_id": 567,
      "updated_at": "2016-10-26T19:45:39.002Z"
    },
    {
      "id": 3,
      "course_id": 179,
      "user_id": 568,
      "updated_at": "2016-10-26T19:45:39.016Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebadef210c02160044878dceeefdcbaede72217d242d29ad36e207550988beb1"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/127/files
Content-Type: application/json
Authorization: Bearer 52da8750d11be4c04bb3e096ae19f90cc0ec6fa4e0dbed6734eb58525f31e47d
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
        "id": 383,
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
        "created_at": "2016-10-26T19:45:25.559Z",
        "updated_at": "2016-10-26T19:45:25.559Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:45:25.574Z",
      "updated_at": "2016-10-26T19:45:25.574Z",
      "course_id": 127,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 384,
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
        "created_at": "2016-10-26T19:45:25.582Z",
        "updated_at": "2016-10-26T19:45:25.582Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:45:25.593Z",
      "updated_at": "2016-10-26T19:45:25.593Z",
      "course_id": 127,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
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
        "created_at": "2016-10-26T19:45:25.601Z",
        "updated_at": "2016-10-26T19:45:25.601Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:45:25.611Z",
      "updated_at": "2016-10-26T19:45:25.611Z",
      "course_id": 127,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/127/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52da8750d11be4c04bb3e096ae19f90cc0ec6fa4e0dbed6734eb58525f31e47d"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/125/files
Content-Type: application/json
Authorization: Bearer 2042683d4b9158db2d30940e871f9aaa6c746d47d3c55413905c252769c2eba7
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
      "id": 379,
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
      "created_at": "2016-10-26T19:45:25.201Z",
      "updated_at": "2016-10-26T19:45:25.201Z"
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
    "created_at": "2016-10-26T19:45:25.255Z",
    "updated_at": "2016-10-26T19:45:25.255Z",
    "course_id": 125,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/125/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2042683d4b9158db2d30940e871f9aaa6c746d47d3c55413905c252769c2eba7"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/126/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer e471af6088457c516c6bb1800089d3f3b3ff8f49d6db7bc1d9de128d6edc8e8d
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
    "key": "cache/f04197745f0aeb6b7398f3e871e0ae75.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQyMDo0NToyNVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2YwNDE5Nzc0NWYwYWViNmI3Mzk4ZjNlODcxZTBhZTc1LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI2VDE5NDUyNVoifV19",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T194525Z",
    "x-amz-signature": "5a43ea931e800b3e89b9cd1dcc268efc838dfce66f990055df2c1407d135580b"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/126/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e471af6088457c516c6bb1800089d3f3b3ff8f49d6db7bc1d9de128d6edc8e8d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 248d8c27eb35b8bf0e9a85c4f154dabfb22859563304d4992ff6d2c976eed089
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
	-H "Authorization: Bearer 248d8c27eb35b8bf0e9a85c4f154dabfb22859563304d4992ff6d2c976eed089"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8db01927bf34a011c1587ddba8757d98422b5f7555247de9da554f4451ebe6bb
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
	-H "Authorization: Bearer 8db01927bf34a011c1587ddba8757d98422b5f7555247de9da554f4451ebe6bb"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 836b2c5c733eb412b84c517dad5981e5b6869cf36eaea17c624c65871b897707
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
	-H "Authorization: Bearer 836b2c5c733eb412b84c517dad5981e5b6869cf36eaea17c624c65871b897707"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer dfc77c2a8ba6640055b343a3ea877ba9c3d2de483661e15f28f4d06dc5f92f1e
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
	-H "Authorization: Bearer dfc77c2a8ba6640055b343a3ea877ba9c3d2de483661e15f28f4d06dc5f92f1e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 672215b27be9a90f0c6dd9f0738a6602c108a7b172e2a174e6673221b080f8da
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
	-H "Authorization: Bearer 672215b27be9a90f0c6dd9f0738a6602c108a7b172e2a174e6673221b080f8da"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 230d440d68405cdb7efc077f396fee8761ee1474b2316b6c8bc2bb0a7386242a
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
    "creator_id": 891,
    "id": 291,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 276,
    "additional_university_ids": [

    ],
    "topic_id": 303,
    "discipline_id": 304,
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
    "chapters_updated_at": "2016-10-26T19:45:59.478Z",
    "updated_at": "2016-10-26T19:46:00.968Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 170,
        "title": "Clever Chapter Title 155",
        "position": 1,
        "updated_at": "2016-10-26T19:46:00.922Z",
        "course_id": 291,
        "author_id": 891,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:45:59.478Z",
        "questions_updated_at": "2016-10-26T19:45:59.478Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 171,
        "title": "Clever Chapter Title 156",
        "position": 2,
        "updated_at": "2016-10-26T19:46:00.960Z",
        "course_id": 291,
        "author_id": 891,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:45:59.478Z",
        "questions_updated_at": "2016-10-26T19:45:59.478Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 892,
        "chapter_id": 170,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.741Z",
        "created_at": "2016-10-26T19:46:00.741Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 892,
        "chapter_id": 171,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.825Z",
        "created_at": "2016-10-26T19:46:00.825Z",
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
        "author_id": 892,
        "chapter_id": 170,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.788Z",
        "created_at": "2016-10-26T19:46:00.788Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 892,
        "chapter_id": 171,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.872Z",
        "created_at": "2016-10-26T19:46:00.872Z",
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
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 892,
        "chapter_id": 170,
        "position": 83,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:45:59.695Z",
        "created_at": "2016-10-26T19:45:59.578Z",
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
            "id": 195,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 196,
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
        "author_id": 892,
        "chapter_id": 170,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:45:59.868Z",
        "created_at": "2016-10-26T19:45:59.758Z",
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
            "id": 197,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 198,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 98,
        "obfuscated_id": "icApzX10lRE",
        "author_id": 892,
        "chapter_id": 171,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.077Z",
        "created_at": "2016-10-26T19:45:59.956Z",
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
            "id": 199,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 200,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 892,
        "chapter_id": 171,
        "position": 86,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:00.261Z",
        "created_at": "2016-10-26T19:46:00.146Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 230d440d68405cdb7efc077f396fee8761ee1474b2316b6c8bc2bb0a7386242a"
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
    "creator_id": 897,
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
    "chapters_updated_at": "2016-10-26T19:46:01.100Z",
    "updated_at": "2016-10-26T19:46:02.588Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 172,
        "title": "Clever Chapter Title 157",
        "position": 1,
        "updated_at": "2016-10-26T19:46:02.540Z",
        "course_id": 292,
        "author_id": 897,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:46:01.100Z",
        "questions_updated_at": "2016-10-26T19:46:01.100Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 173,
        "title": "Clever Chapter Title 158",
        "position": 2,
        "updated_at": "2016-10-26T19:46:02.581Z",
        "course_id": 292,
        "author_id": 897,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:46:01.100Z",
        "questions_updated_at": "2016-10-26T19:46:01.100Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 102,
        "obfuscated_id": "jFy90P7ldB4",
        "author_id": 897,
        "chapter_id": 172,
        "position": 89,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:01.310Z",
        "created_at": "2016-10-26T19:46:01.196Z",
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
      },
      {
        "id": 104,
        "obfuscated_id": "nIg2bhYRjos",
        "author_id": 897,
        "chapter_id": 173,
        "position": 91,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:01.700Z",
        "created_at": "2016-10-26T19:46:01.574Z",
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
            "id": 211,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 212,
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
PUT /v2/courses/290/pin
Content-Type: application/json
Authorization: Bearer 9ded22068ad15ae5be67e1189d6bbf91a4591eb6ffe8066816ab567029b069a7
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/290/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ded22068ad15ae5be67e1189d6bbf91a4591eb6ffe8066816ab567029b069a7"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/276/pin
Content-Type: application/json
Authorization: Bearer 0fdca5ae64f7145f9ddb1f0f617e09fe003f4466057aad125ab496fe8e1d8fb5
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/276/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fdca5ae64f7145f9ddb1f0f617e09fe003f4466057aad125ab496fe8e1d8fb5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7d6f9b1bf1721cfa23a596e22337aaa61133668c73880da03f2a2c948905eec0
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
    "creator_id": 886,
    "id": 288,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 273,
    "additional_university_ids": [

    ],
    "topic_id": 300,
    "discipline_id": 301,
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
    "updated_at": "2016-10-26T19:45:59.193Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d6f9b1bf1721cfa23a596e22337aaa61133668c73880da03f2a2c948905eec0"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 710bbfd66f95bf220d1374222705c23b82e6c5b1670695ad52ffc1ae45e74c9f
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
    "id": 580,
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
    "created_at": "2016-10-26T19:45:39.583Z",
    "updated_at": "2016-10-26T19:45:39.583Z",
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
	-H "Authorization: Bearer 710bbfd66f95bf220d1374222705c23b82e6c5b1670695ad52ffc1ae45e74c9f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7206660da853b83c40a3d77d2a5d291014d25fb60f06a1f8011ef3ea2788137a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[191]}
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
    "id": 581,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      191
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:45:39.667Z",
    "updated_at": "2016-10-26T19:45:39.701Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[191]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7206660da853b83c40a3d77d2a5d291014d25fb60f06a1f8011ef3ea2788137a"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b9dc6caff68f7c64ed7dd557d8dd91fad1238609f147ad1fd8b0e60b9b395629
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
    "id": 584,
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
    "created_at": "2016-10-26T19:45:39.864Z",
    "updated_at": "2016-10-26T19:45:39.864Z",
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
	-H "Authorization: Bearer b9dc6caff68f7c64ed7dd557d8dd91fad1238609f147ad1fd8b0e60b9b395629"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8c412302c920676c517452b88677f545f6146c0ea5f30c39a3a10346b2cc8279
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[193]}
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
    "id": 583,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      193
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:45:39.816Z",
    "updated_at": "2016-10-26T19:45:39.816Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[193]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c412302c920676c517452b88677f545f6146c0ea5f30c39a3a10346b2cc8279"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 0190359efbaa369332e7ffcb069eaccd07d9de78a3919a14997fa48ac8b177b1
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

195
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
    "id": 585,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/fbf9bec27f23434cac578d642402507dd5d3f73f.jpg",
    "university_id": null,
    "fields_of_study": [
      195
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:45:39.956Z",
    "updated_at": "2016-10-26T19:45:40.250Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/4463d3751afedc44d3b355e28c29036bc8ee41e8.jpg",
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

195
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 0190359efbaa369332e7ffcb069eaccd07d9de78a3919a14997fa48ac8b177b1"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 6af6d8a60793c081c07b841579aaa5f8a5c42d563b9292964739b1389d48a111
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
      "id": 2,
      "bookmarkable_id": 52,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 53,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 54,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6af6d8a60793c081c07b841579aaa5f8a5c42d563b9292964739b1389d48a111"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 5200baf69f8ccf5c727276ad370130d5db1d8536b1b55b56a4cd0e45ba88d5cd
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
	-H "Authorization: Bearer 5200baf69f8ccf5c727276ad370130d5db1d8536b1b55b56a4cd0e45ba88d5cd"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 84258d79995615ba8d3d77603d17e97aab5414bc156bdc5ee88f126c25730f12
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
	-H "Authorization: Bearer 84258d79995615ba8d3d77603d17e97aab5414bc156bdc5ee88f126c25730f12"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer f3c2338a5692a778d66758321bf8971e5a6aff511c619f68155a6ae9c47b03c2
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
      "creator_id": 852,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-225",
      "html_url": "https://goskive.com/course/mit-course-225",
      "slug": "mit-course-225",
      "university_id": 258,
      "additional_university_ids": [

      ],
      "topic_id": 285,
      "discipline_id": 286,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 225",
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
      "updated_at": "2016-10-26T19:45:56.461Z",
      "shortname": "mit-course-225"
    },
    {
      "creator_id": 853,
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-226",
      "html_url": "https://goskive.com/course/mit-course-226",
      "slug": "mit-course-226",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "topic_id": 286,
      "discipline_id": 287,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 226",
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
      "updated_at": "2016-10-26T19:45:56.538Z",
      "shortname": "mit-course-226"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3c2338a5692a778d66758321bf8971e5a6aff511c619f68155a6ae9c47b03c2"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 453426f31909ac093d6e88039fdc2d2a084979a38e482b3af19b35649e45610d
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
        "updated_at": "2016-10-26T19:45:56.819Z"
      },
      "created_at": "2016-10-26T19:45:56.822Z",
      "updated_at": "2016-10-26T19:45:56.822Z",
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
        "updated_at": "2016-10-26T19:45:56.830Z"
      },
      "created_at": "2016-10-26T19:45:56.833Z",
      "updated_at": "2016-10-26T19:45:56.833Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 453426f31909ac093d6e88039fdc2d2a084979a38e482b3af19b35649e45610d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cbd022da1bb9cea0228a252373276828b9eafc1628b4284d585e751b6fd9f279
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
        "updated_at": "2016-10-26T19:45:56.599Z"
      },
      "created_at": "2016-10-26T19:45:56.603Z",
      "updated_at": "2016-10-26T19:45:56.603Z",
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
        "updated_at": "2016-10-26T19:45:56.616Z"
      },
      "created_at": "2016-10-26T19:45:56.619Z",
      "updated_at": "2016-10-26T19:45:56.619Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbd022da1bb9cea0228a252373276828b9eafc1628b4284d585e751b6fd9f279"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer ee92c8f0c5e203e3813543391bdde0e268032065d3ec21844c44ae95542505e2
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
      "id": 11,
      "created_at": "2016-10-26T19:45:26.749Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 9,
      "updated_at": "2016-10-26T19:45:26.857Z",
      "author_id": "401",
      "thread_subject_id": "130",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 12,
      "created_at": "2016-10-26T19:45:26.846Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 10,
      "updated_at": "2016-10-26T19:45:26.860Z",
      "author_id": "404",
      "thread_subject_id": "131",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-10-26T19:45:27.220Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-26T19:45:27.220Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-10-26T19:45:27.585Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-10-26T19:45:27.585Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 15,
      "created_at": "2016-10-26T19:45:27.956Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-26T19:45:27.956Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 16,
      "created_at": "2016-10-26T19:45:28.272Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 61,
      "updated_at": "2016-10-26T19:45:28.272Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-10-26T19:45:28.559Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 62,
      "updated_at": "2016-10-26T19:45:28.559Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-10-26T19:45:28.843Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 63,
      "updated_at": "2016-10-26T19:45:28.843Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee92c8f0c5e203e3813543391bdde0e268032065d3ec21844c44ae95542505e2"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/10
Content-Type: application/json
Authorization: Bearer 8122333dbf000c6620e3ad8e54b045fc29b137c27256eefd86cf9b48ed358c68
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-26T19:35:26.000Z"}}
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
    "id": 10,
    "created_at": "2016-10-26T19:45:26.574Z",
    "read_at": "2016-10-26T19:35:26.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 8,
    "updated_at": "2016-10-26T19:45:26.637Z",
    "author_id": "397",
    "thread_subject_id": "129",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/10" -d '{"notification":{"read_at":"2016-10-26T19:35:26.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8122333dbf000c6620e3ad8e54b045fc29b137c27256eefd86cf9b48ed358c68"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 7dff1de2b76886a02b8904915a76f3cdaee5c23a3495e858b8c5c02b007efd3a
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
      "course_id": 154,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T19:45:31.319Z",
      "course_published": true,
      "updated_at": "2016-10-26T19:45:31.311Z"
    },
    {
      "id": 5,
      "course_id": 155,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T19:45:31.400Z",
      "course_published": true,
      "updated_at": "2016-10-26T19:45:31.393Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dff1de2b76886a02b8904915a76f3cdaee5c23a3495e858b8c5c02b007efd3a"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 3aff183acfd26943a562aed5b9ea8f0a101266a805636d6aec3da35fc9134552
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
    "id": 2,
    "course_id": 152,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T19:45:31.012Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:45:31.005Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aff183acfd26943a562aed5b9ea8f0a101266a805636d6aec3da35fc9134552"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 9b5a95395eb981efd78227ba5d72644546f211c37258d1eac19e09bd5d616e0e
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
    "id": 3,
    "course_id": 153,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-26T19:45:31.179Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:45:31.168Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b5a95395eb981efd78227ba5d72644546f211c37258d1eac19e09bd5d616e0e"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3f68d09233f93d4f9fa3515a2ed2830fd155f54a0403bf3cdade25adb0670b66
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
      "votable_id": 120,
      "user_id": 914
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 914
    },
    {
      "id": 22,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 914
    },
    {
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 914
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f68d09233f93d4f9fa3515a2ed2830fd155f54a0403bf3cdade25adb0670b66"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/183
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
    "id": 183,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 183,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 183
      },
      {
        "id": 184,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 183
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/183" -X GET \
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
      "id": 184,
      "name": "Up-sized uniform time-frame",
      "name_translations": {
        "en": "Up-sized uniform time-frame"
      }
    },
    {
      "id": 185,
      "name": "Configurable interactive productivity",
      "name_translations": {
        "en": "Configurable interactive productivity"
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
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer f17973d58be35f232333e6795e59b1134ee4df2760f1a2abe03741606ac4257f
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
    "id": 27,
    "user_id": 266,
    "feedbackable_id": 12,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-26T19:45:17.327Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f17973d58be35f232333e6795e59b1134ee4df2760f1a2abe03741606ac4257f"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer b80e597870a42b7bbb8e03b436645b0eff9bc14d1b3142c3324d770f2b317db0
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
    "id": 22,
    "user_id": 241,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-26T19:45:16.062Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/22/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b80e597870a42b7bbb8e03b436645b0eff9bc14d1b3142c3324d770f2b317db0"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 3ae62c68df5241783691da46ee049e8bc7ee3d4cf08e2b863b9dc94402c2ad11
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
    "id": 20,
    "user_id": 229,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:45:15.541Z",
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
curl "api.goskive.com/v2/feedbacks/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ae62c68df5241783691da46ee049e8bc7ee3d4cf08e2b863b9dc94402c2ad11"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer c9c36e97c2c1314b54d0f33fa8834d67adbb37fb7b7f8141a675289f8f6676a8
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
	-H "Authorization: Bearer c9c36e97c2c1314b54d0f33fa8834d67adbb37fb7b7f8141a675289f8f6676a8"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 980115a095ea9c6a918823e6201445a771da662f019793af996f2625ade0929e
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
	-H "Authorization: Bearer 980115a095ea9c6a918823e6201445a771da662f019793af996f2625ade0929e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/close
Content-Type: application/json
Authorization: Bearer 60435a5e9bd9f3923a3f97db771e5596ee8f31644468711dd0c30cd36d87ecfb
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
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60435a5e9bd9f3923a3f97db771e5596ee8f31644468711dd0c30cd36d87ecfb"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/21
Content-Type: application/json
Authorization: Bearer 1eca3fdb68fc53a43deab4239d1983687dddb452d484c2de25af227ee187e2a7
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
    "user_id": 234,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:45:15.874Z",
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
curl "api.goskive.com/v2/feedbacks/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1eca3fdb68fc53a43deab4239d1983687dddb452d484c2de25af227ee187e2a7"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer da86a5895372a49070b7820c94116f94ddb0fa6b27b1826a2cf859542ca17617
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
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da86a5895372a49070b7820c94116f94ddb0fa6b27b1826a2cf859542ca17617"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/5/bookmark
Content-Type: application/json
Authorization: Bearer 787a8822ac8c4748175a5a0fdfe4552be1fa7eede3a49a47325821ff9aeaaf58
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 787a8822ac8c4748175a5a0fdfe4552be1fa7eede3a49a47325821ff9aeaaf58"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer a21390391283971a98a1b0075368ab999469bdcef253dd045eefc96c58a224fd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a21390391283971a98a1b0075368ab999469bdcef253dd045eefc96c58a224fd"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/6
Content-Type: application/json
Authorization: Bearer 398bc0810ca2dc3ea79b563220e3fcea3bc404821974e4a774c75950009dfbb3
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/dea931693a005593df9573579a6e833e.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T194529Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=05ed26e67e3d3de154e6dd9c33f6074913f89aaa5604506481697d5e2fd97f34",
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
	-H "Authorization: Bearer 398bc0810ca2dc3ea79b563220e3fcea3bc404821974e4a774c75950009dfbb3"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer a44862be7e46ac153d0fc202a206d48bff07c965d900b9915ea7c132d09fbe4f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/81bc8d18ad1fa45f6610d9059b53144f.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T194529Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=45f2da7f04acc62782db43a3d3f30782454d5998fb511aedd588c567d029033a",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a44862be7e46ac153d0fc202a206d48bff07c965d900b9915ea7c132d09fbe4f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 0bafa102f6f1a2d815ae571663431af3ecc91ac906592d91de778e1298824db7
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
      "id": 437,
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
      "created_at": "2016-10-26T19:45:29.311Z",
      "updated_at": "2016-10-26T19:45:29.311Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-26T19:45:29.382Z",
    "updated_at": "2016-10-26T19:45:29.382Z",
    "course_id": 141,
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bafa102f6f1a2d815ae571663431af3ecc91ac906592d91de778e1298824db7"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/17/matched_courses?required_cu_count=2
Authorization: Bearer 7757670adf9d2638074f986f4bc353b93b20625eae66ea44b8d68ca47cf2a751
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
      "creator_id": 823,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 279,
      "discipline_id": 280,
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
      "chapters_updated_at": "2016-10-26T19:45:52.744Z",
      "updated_at": "2016-10-26T19:45:54.339Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 828,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-675edcfb-8345-466a-bf11-866a129b1918",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-675edcfb-8345-466a-bf11-866a129b1918",
      "slug": "mit-the-great-british-bake-off-675edcfb-8345-466a-bf11-866a129b1918",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 280,
      "discipline_id": 281,
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
      "chapters_updated_at": "2016-10-26T19:45:52.744Z",
      "updated_at": "2016-10-26T19:45:54.926Z",
      "shortname": "mit-the-great-british-bake-off-675edcfb-8345-466a-bf11-866a129b1918"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/17/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 7757670adf9d2638074f986f4bc353b93b20625eae66ea44b8d68ca47cf2a751"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/16/report
Content-Type: application/json
Authorization: Bearer 5efee388f33920ff6c06a0283479c692db005ea4ede1ff5517816aabc9dded68
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5efee388f33920ff6c06a0283479c692db005ea4ede1ff5517816aabc9dded68"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/15/bookmark
Content-Type: application/json
Authorization: Bearer 46beece500668da4edf7006814e7581909b4f5628269f042d65b98c959a7c749
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46beece500668da4edf7006814e7581909b4f5628269f042d65b98c959a7c749"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/11/upvote
Content-Type: application/json
Authorization: Bearer b923b2e5f9e1206d756e1974528f419ff5a1fe3f851de841deecdcbc281e575d
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b923b2e5f9e1206d756e1974528f419ff5a1fe3f851de841deecdcbc281e575d"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/26/comments
Content-Type: application/json
Authorization: Bearer 21bd2981646c586b8e886471cb849c090627e7f806d1695fdded5acfe4fea914
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
    "id": 4,
    "author_id": 340,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:45:21.921Z",
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
curl "api.goskive.com/v2/flashcards/26/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21bd2981646c586b8e886471cb849c090627e7f806d1695fdded5acfe4fea914"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/27/comments
Content-Type: application/json
Authorization: Bearer a098cd4b7b1d970b4b5c548b22b8992fe7f6b0c5a55e76e360c7644b667512b9
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
    "id": 5,
    "author_id": 343,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:45:22.262Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 343,
      "feedbackable_id": 27,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:22.259Z",
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
curl "api.goskive.com/v2/flashcards/27/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a098cd4b7b1d970b4b5c548b22b8992fe7f6b0c5a55e76e360c7644b667512b9"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/29/comments
Content-Type: application/json
Authorization: Bearer f5c7fdf9414ff2dcf1996490f8d8e73afd09fb216651e624a0b73504e690282d
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
      "author_id": 352,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:22.718Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 353,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:22.733Z",
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
curl "api.goskive.com/v2/flashcards/29/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5c7fdf9414ff2dcf1996490f8d8e73afd09fb216651e624a0b73504e690282d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/25/comments
Content-Type: application/json
Authorization: Bearer 51d7217156ea91bd280147dca56b56545e013c0ee96cfa8d25d1fc1fd0daba89
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
curl "api.goskive.com/v2/flashcards/25/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51d7217156ea91bd280147dca56b56545e013c0ee96cfa8d25d1fc1fd0daba89"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/23/feedbacks
Content-Type: application/json
Authorization: Bearer 971aae844ad9bdd0f45072895f19caad5de05245ec980292a54ef203494ba29f
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
    "id": 35,
    "user_id": 331,
    "feedbackable_id": 23,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:45:21.037Z",
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
curl "api.goskive.com/v2/flashcards/23/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 971aae844ad9bdd0f45072895f19caad5de05245ec980292a54ef203494ba29f"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/18/feedbacks
Content-Type: application/json
Authorization: Bearer a69c7a6c4144f12d5cbeda63926dc0a4cd9429d67fbccd226dd6e1ff3a440e20
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
      "id": 30,
      "user_id": 308,
      "feedbackable_id": 18,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:20.076Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 307,
      "feedbackable_id": 18,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:20.065Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/18/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a69c7a6c4144f12d5cbeda63926dc0a4cd9429d67fbccd226dd6e1ff3a440e20"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/15/votes
Content-Type: application/json
Authorization: Bearer a5505b06a374e03bb4600ec8c632a49effecba457ba3478947705fb6e475737f
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
      "votable_id": 15,
      "user_id": 289
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 15,
      "user_id": 288
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 15,
      "user_id": 287
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/15/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5505b06a374e03bb4600ec8c632a49effecba457ba3478947705fb6e475737f"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/53/republish
Content-Type: application/json
Authorization: Bearer 7f25866ddb7c500a797f88340de30a5fb61540d1fd86043fdbc9d7f2a33a4082
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
curl "api.goskive.com/v2/flashcards/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f25866ddb7c500a797f88340de30a5fb61540d1fd86043fdbc9d7f2a33a4082"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/50/bookmark
Content-Type: application/json
Authorization: Bearer 38a0cefad04f41c4d861834f08d805d3e497973c91fce8d24fa7b1f434b54b9c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38a0cefad04f41c4d861834f08d805d3e497973c91fce8d24fa7b1f434b54b9c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/56
Content-Type: application/json
Authorization: Bearer 6a883239cd2ebe2844e93019fd2bee64781490cd3516fdc269806d9349d3b925
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a883239cd2ebe2844e93019fd2bee64781490cd3516fdc269806d9349d3b925"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/57/downvote
Content-Type: application/json
Authorization: Bearer c8b6d6d627914d6dd80248c0f3fa46e676fce1a7c270483f58d98c263eee8d49
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
	-H "Authorization: Bearer c8b6d6d627914d6dd80248c0f3fa46e676fce1a7c270483f58d98c263eee8d49"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/55
Content-Type: application/json
Authorization: Bearer e6d249fcc5fc9b3b2f84240c4ca31244c31ffb4ac93b1f949b228b206dc79845
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
    "id": 55,
    "obfuscated_id": "VX19tR4fHZ8",
    "author_id": 654,
    "chapter_id": 144,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:43.714Z",
    "created_at": "2016-10-26T19:45:43.714Z",
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
curl "api.goskive.com/v2/flashcards/55" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6d249fcc5fc9b3b2f84240c4ca31244c31ffb4ac93b1f949b228b206dc79845"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/51/report
Content-Type: application/json
Authorization: Bearer 9d2df99e0ba393c1660277aa93154b300d7fc67418f4516ba56aff8409b310ba
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
	-H "Authorization: Bearer 9d2df99e0ba393c1660277aa93154b300d7fc67418f4516ba56aff8409b310ba"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/54/bookmark
Content-Type: application/json
Authorization: Bearer 3a655014ef9639a68ef5d90fd5227824f3755e10a466fb248d2ca775f59db5a5
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
	-H "Authorization: Bearer 3a655014ef9639a68ef5d90fd5227824f3755e10a466fb248d2ca775f59db5a5"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/34/upvote
Content-Type: application/json
Authorization: Bearer bf7cc998f0e79e389b398b291fab7d6331cc2132ab199de809505ee00d2d1b62
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf7cc998f0e79e389b398b291fab7d6331cc2132ab199de809505ee00d2d1b62"
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
    "key": "cache/9292063fe94d5b2dd16b3258453b40cb.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQyMDo0NToxOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzkyOTIwNjNmZTk0ZDViMmRkMTZiMzI1ODQ1M2I0MGNiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjZUMTk0NTE5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T194519Z",
    "x-amz-signature": "3908757f89f40bcc7da8cbcabd17bf9a1602cfece4c023810b7f68b7e90a48d5"
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
Authorization: Bearer 850044f802c1630ce50fd12f739bb73d5d1baf08b2e8c7f2f0f4a839b40b2c9a
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
	-H "Authorization: Bearer 850044f802c1630ce50fd12f739bb73d5d1baf08b2e8c7f2f0f4a839b40b2c9a"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 5bbb8e9914526df019ec92e062e9635b7312b868c9348db9ca5e2eefc30bc911
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
	-H "Authorization: Bearer 5bbb8e9914526df019ec92e062e9635b7312b868c9348db9ca5e2eefc30bc911"
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
{"password":{"reset_password_token":"hFLQW5BLBRwe9GoVHxH-","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 474,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-26T19:45:31.444Z",
  "updated_at": "2016-10-26T19:45:32.058Z",
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
  "audit_id": 3823
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"hFLQW5BLBRwe9GoVHxH-","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/126/comments
Content-Type: application/json
Authorization: Bearer 7f3e1df20b3a0724238841ec282ea6c419d5fa952b46e06efac21d04d5ed5685
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
    "id": 58,
    "author_id": 934,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:46:08.261Z",
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
curl "api.goskive.com/v2/questions/126/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f3e1df20b3a0724238841ec282ea6c419d5fa952b46e06efac21d04d5ed5685"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/124/comments
Content-Type: application/json
Authorization: Bearer ba9f89f122fb11894b6217ec6dabc5fd108ea64f960e07808785bc2c7bf9b791
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
    "id": 57,
    "author_id": 928,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:46:07.482Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 928,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:46:07.479Z",
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
curl "api.goskive.com/v2/questions/124/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba9f89f122fb11894b6217ec6dabc5fd108ea64f960e07808785bc2c7bf9b791"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/127/comments
Content-Type: application/json
Authorization: Bearer cbce87fb450cfed32096bdeedd01a1e0c03aa57d9059dfd7da0bd7968112f6e3
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
      "id": 60,
      "author_id": 941,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:46:08.694Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 940,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:46:08.680Z",
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
curl "api.goskive.com/v2/questions/127/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbce87fb450cfed32096bdeedd01a1e0c03aa57d9059dfd7da0bd7968112f6e3"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/125/comments
Content-Type: application/json
Authorization: Bearer 84ddb47a217dfbaa8a4b678f26090e54cb9192570d54438213b2bde8bbd3fbe0
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
curl "api.goskive.com/v2/questions/125/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84ddb47a217dfbaa8a4b678f26090e54cb9192570d54438213b2bde8bbd3fbe0"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/76/feedbacks
Content-Type: application/json
Authorization: Bearer a962a115d656c5744c6d9f86a274c93b5349beec7094bfed5eec63a266bc84bc
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
    "user_id": 772,
    "feedbackable_id": 76,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:45:49.686Z",
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
curl "api.goskive.com/v2/questions/76/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a962a115d656c5744c6d9f86a274c93b5349beec7094bfed5eec63a266bc84bc"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/82/feedbacks
Content-Type: application/json
Authorization: Bearer 2b87eeb4fa54a80a33d45f5111ef64b38c534d49ff8417541c3affe610934901
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
      "id": 45,
      "user_id": 804,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:51.783Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 803,
      "feedbackable_id": 82,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:51.772Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/82/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b87eeb4fa54a80a33d45f5111ef64b38c534d49ff8417541c3affe610934901"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/31/votes
Content-Type: application/json
Authorization: Bearer 873e71d4f2145a4c6db348ff306b42b43f764543046bc3d3ed0f2c12e96dace7
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
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 31,
      "user_id": 137
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 31,
      "user_id": 136
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 31,
      "user_id": 135
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/31/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 873e71d4f2145a4c6db348ff306b42b43f764543046bc3d3ed0f2c12e96dace7"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/11/republish
Content-Type: application/json
Authorization: Bearer 9115a4996e36220de10700b83bb9946637ece2f6cb1b6dbb884690e98774433d
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
curl "api.goskive.com/v2/questions/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9115a4996e36220de10700b83bb9946637ece2f6cb1b6dbb884690e98774433d"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/12/bookmark
Content-Type: application/json
Authorization: Bearer 3c783accfa2fed9ed7c44b6f46261cdca42670eef9bf2ba9701527da231a3d48
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/12/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c783accfa2fed9ed7c44b6f46261cdca42670eef9bf2ba9701527da231a3d48"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/5
Content-Type: application/json
Authorization: Bearer b384666a4db624ac9e9bf3b1d6be66f2d6326c32398054e1f3468c1372c0641a
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b384666a4db624ac9e9bf3b1d6be66f2d6326c32398054e1f3468c1372c0641a"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/6/downvote
Content-Type: application/json
Authorization: Bearer 115db523080bfe8090d833d0133f0cf2f4db44f5865a35e6311a147f7c5d6c87
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/6/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 115db523080bfe8090d833d0133f0cf2f4db44f5865a35e6311a147f7c5d6c87"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/13
Content-Type: application/json
Authorization: Bearer a458d5db23a352895a3d432ed2e385e7d137bbe00e198a06a2f7e5679948edf8
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 70,
    "chapter_id": 16,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:02.484Z",
    "created_at": "2016-10-26T19:45:02.349Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 26,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 27,
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
curl "api.goskive.com/v2/questions/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a458d5db23a352895a3d432ed2e385e7d137bbe00e198a06a2f7e5679948edf8"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/7/report
Content-Type: application/json
Authorization: Bearer e24b8be72f617b5d76f57c0e70d82dcad096f94b022837d440026fe568023d4e
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/7/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e24b8be72f617b5d76f57c0e70d82dcad096f94b022837d440026fe568023d4e"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/9/bookmark
Content-Type: application/json
Authorization: Bearer 10e854c3e286be396d5fdfae950cf49fe5def1ad86e80b64f59a650fbb4b70c9
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/9/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10e854c3e286be396d5fdfae950cf49fe5def1ad86e80b64f59a650fbb4b70c9"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/8
Content-Type: application/json
Authorization: Bearer bb5377f7facf7ba800011ca4bda8977ec85c1b69dcd500361e101f95df4264c5
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":8,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T19:45:00.444Z","updated_at":"2016-10-26T19:45:00.567Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":11,"author_id":55,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 55,
    "chapter_id": 11,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:45:00.718Z",
    "created_at": "2016-10-26T19:45:00.444Z",
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
    "question": "{\"id\"=>8, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-26T19:45:00.444Z\", \"updated_at\"=>\"2016-10-26T19:45:00.567Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>11, \"author_id\"=>55, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 15,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 16,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 17,
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
curl "api.goskive.com/v2/questions/8" -d '{"question":{"question":{"id":8,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T19:45:00.444Z","updated_at":"2016-10-26T19:45:00.567Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":11,"author_id":55,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb5377f7facf7ba800011ca4bda8977ec85c1b69dcd500361e101f95df4264c5"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/14/upvote
Content-Type: application/json
Authorization: Bearer df29682425a4806efb5a0498bf9b9294df5623903624ca517804b0b328b64af3
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/14/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df29682425a4806efb5a0498bf9b9294df5623903624ca517804b0b328b64af3"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 56b674296f06c09c920d0befddd71620bd629cab9e6d1b788ead43d6a3be8ff5
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
      "creator_id": 805,
      "id": 262,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 274,
      "discipline_id": 275,
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
      "updated_at": "2016-10-26T19:45:51.908Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56b674296f06c09c920d0befddd71620bd629cab9e6d1b788ead43d6a3be8ff5"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 63ad2c7c923d3540feeecba360247de6d063d248d9173d80713a71602ce942d5
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
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-228",
      "html_url": "https://goskive.com/university/uni-228",
      "slug": "uni-228",
      "name": "National School of Pizza",
      "short_name": "Uni 228",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8f99815830754135fe1ea966e2f887289702258e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e6e710b2390afd0aec35954566fe8bda19e67b29.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:45:52.150Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-227",
      "html_url": "https://goskive.com/university/uni-227",
      "slug": "uni-227",
      "name": "National School of Pastry",
      "short_name": "Uni 227",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/055789a9b4b1de6e8028fe137a3e74c648231c90.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/25ef9b1512206ad576da811dfe492b1c06bcca53.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:45:52.133Z",
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
	-H "Authorization: Bearer 63ad2c7c923d3540feeecba360247de6d063d248d9173d80713a71602ce942d5"
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
      "id": 70,
      "name": "Horizontal incremental circuit",
      "name_translations": {
        "en": "Horizontal incremental circuit"
      },
      "discipline_id": 70
    },
    {
      "id": 69,
      "name": "Optimized disintermediate core",
      "name_translations": {
        "en": "Optimized disintermediate core"
      },
      "discipline_id": 69
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
GET /v2/topics/71
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
    "id": 71,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 71
  }
}
```



```shell
curl "api.goskive.com/v2/topics/71" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 9c213616eb35f18a2b9192e48deb24376e6a297060bfd4397eb4aac1ab6d259d
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
      "id": 49,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-29",
      "html_url": "https://goskive.com/university/uni-29",
      "slug": "uni-29",
      "name": "University 29",
      "short_name": "Uni 29",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/532ca42a4d33413a1fad58a1c925ea12fd1aaaac.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e5230a1a2c4652e95c9df03f9572f3a47127d484.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:45:09.265Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 50,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-30",
      "html_url": "https://goskive.com/university/uni-30",
      "slug": "uni-30",
      "name": "University 30",
      "short_name": "Uni 30",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/72304e4af02e465701fdc93c3df8755264f8576f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9aef7bfea98b10a79b202a51e3b1f2bd4bc41b01.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:45:09.282Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-31",
      "html_url": "https://goskive.com/university/uni-31",
      "slug": "uni-31",
      "name": "University 31",
      "short_name": "Uni 31",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/47530aee07f05a760298ecc7a31c5ea764cbfe95.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ebf723f2b962013a9c9a48122a0add1b8548d13c.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:45:09.302Z",
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
	-H "Authorization: Bearer 9c213616eb35f18a2b9192e48deb24376e6a297060bfd4397eb4aac1ab6d259d"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer e848d206822c535851515df2c3ff3d93a4e3c4c40f8097d3a598add46d24a085
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
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e6aa0b3ce8cf756564f47adecea4f19e1098f7b3.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8f68223331916973ced2c3074aff9ade550dcdb0.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-26T19:45:09.183Z",
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
	-H "Authorization: Bearer e848d206822c535851515df2c3ff3d93a4e3c4c40f8097d3a598add46d24a085"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 84516d8b60529565e5903c27541cc2c4405630b3ee34c6b4f19f7aa36cb18dd8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":2,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 2,
    "id": 2,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 2,
    "additional_university_ids": [

    ],
    "topic_id": 2,
    "discipline_id": 2,
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
    "chapters_updated_at": "2016-10-26T19:44:54.465Z",
    "updated_at": "2016-10-26T19:44:54.637Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 1,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-26T19:44:54.588Z",
        "course_id": 2,
        "author_id": 2,
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
        "id": 2,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-26T19:44:54.611Z",
        "course_id": 2,
        "author_id": 2,
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
        "id": 3,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-26T19:44:54.627Z",
        "course_id": 2,
        "author_id": 2,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":2,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84516d8b60529565e5903c27541cc2c4405630b3ee34c6b4f19f7aa36cb18dd8"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f267482df3bf5345972af441f2d40659508f65e1506b48c24859ed00a6e1da5a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":3,"published":false}}
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
    "creator_id": 3,
    "id": 3,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 3,
    "additional_university_ids": [

    ],
    "topic_id": 3,
    "discipline_id": 3,
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
    "updated_at": "2016-10-26T19:44:54.794Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":3,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f267482df3bf5345972af441f2d40659508f65e1506b48c24859ed00a6e1da5a"
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
      "creator_id": 10,
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "topic_id": 11,
      "discipline_id": 11,
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
      "updated_at": "2016-10-26T19:44:55.387Z",
      "shortname": "fu-course-7"
    },
    {
      "creator_id": 10,
      "id": 12,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "topic_id": 12,
      "discipline_id": 12,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 8",
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
      "chapters_updated_at": "2016-10-26T19:44:55.732Z",
      "updated_at": "2016-10-26T19:44:55.737Z",
      "shortname": "fu-course-8"
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
Authorization: Bearer 291cf198e4deac7252ee269cffde48383f43944bb2605ac57f6f976b6598ce8b
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
      "creator_id": 37,
      "id": 35,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 35,
      "discipline_id": 35,
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
      "updated_at": "2016-10-26T19:44:57.754Z",
      "shortname": "fu-course-31"
    },
    {
      "creator_id": 37,
      "id": 36,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 36,
      "discipline_id": 36,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
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
      "chapters_updated_at": "2016-10-26T19:44:58.032Z",
      "updated_at": "2016-10-26T19:44:58.038Z",
      "shortname": "fu-course-32"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 291cf198e4deac7252ee269cffde48383f43944bb2605ac57f6f976b6598ce8b"
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
      "creator_id": 15,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 9,
      "additional_university_ids": [

      ],
      "topic_id": 15,
      "discipline_id": 15,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
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
      "updated_at": "2016-10-26T19:44:55.928Z",
      "shortname": "fu-course-11"
    },
    {
      "creator_id": 15,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 9,
      "additional_university_ids": [

      ],
      "topic_id": 16,
      "discipline_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
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
      "updated_at": "2016-10-26T19:44:55.965Z",
      "shortname": "fu-course-12"
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
Authorization: Bearer ee7d7a2f983ce318d0dcb02dcfeca0c9b49e4d097422eb5c013bfb9f06514af2
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
      "creator_id": 43,
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-35",
      "html_url": "https://goskive.com/course/fu-course-35",
      "slug": "fu-course-35",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 39,
      "discipline_id": 39,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 35",
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
      "updated_at": "2016-10-26T19:44:58.256Z",
      "shortname": "fu-course-35"
    },
    {
      "creator_id": 43,
      "id": 40,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-36",
      "html_url": "https://goskive.com/course/fu-course-36",
      "slug": "fu-course-36",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 40,
      "discipline_id": 40,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 36",
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
      "updated_at": "2016-10-26T19:44:58.296Z",
      "shortname": "fu-course-36"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee7d7a2f983ce318d0dcb02dcfeca0c9b49e4d097422eb5c013bfb9f06514af2"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 322c5ee4f632ff82de72e002ed35336a25ec26d38bfb53672cc976fb6de335f2
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
  "id": 849,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-26T19:45:56.144Z",
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
	-H "Authorization: Bearer 322c5ee4f632ff82de72e002ed35336a25ec26d38bfb53672cc976fb6de335f2"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/539
Content-Type: application/json
Authorization: Bearer fe641a9e24cf428e71caa59c5f1820fa6a8829ba5af9ab19e8ee03b13795ac61
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
    "id": 539,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 155,
    "fields_of_study": [
      175,
      176
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-26T19:45:36.157Z",
    "updated_at": "2016-10-26T19:45:36.157Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/539" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe641a9e24cf428e71caa59c5f1820fa6a8829ba5af9ab19e8ee03b13795ac61"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/541
Content-Type: application/json
Authorization: Bearer 941ddcdc0388980d5f689f4ca3a2aa718ed31c4f8c2df147fbf682b6f59ca2e9
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
    "id": 541,
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
    "created_at": "2016-10-26T19:45:36.241Z",
    "updated_at": "2016-10-26T19:45:36.241Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/541" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 941ddcdc0388980d5f689f4ca3a2aa718ed31c4f8c2df147fbf682b6f59ca2e9"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/11
Content-Type: application/json
Authorization: Bearer c3279cebaccf5e0ef37898e0ef45aac4e1548ef0f196437c8b5a35c59e191e9d
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
	-H "Authorization: Bearer c3279cebaccf5e0ef37898e0ef45aac4e1548ef0f196437c8b5a35c59e191e9d"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer ce94fb9816dc42ffb9c2422d8e8e067517fc8f272d8b5c34bf03ab17d9185dbf
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
    "votable_id": 57,
    "user_id": 374
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce94fb9816dc42ffb9c2422d8e8e067517fc8f272d8b5c34bf03ab17d9185dbf"
```
