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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"08dea4296bbdf2871c227eb9dd54a395217ab440a8a075b66c2a1bd3c920f9c2","client_secret":"f23aa3b41a6dd6e3e6a06fba04ac716d0a2b881716ac275032f79f87936cc211"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"08dea4296bbdf2871c227eb9dd54a395217ab440a8a075b66c2a1bd3c920f9c2","client_secret":"f23aa3b41a6dd6e3e6a06fba04ac716d0a2b881716ac275032f79f87936cc211"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NWM2MjZhMjFhOTc3YTAxODJjYTlkYjAyNjkxZjg3ZGFkZTIwZTFkNzBmNmU2
NzEzNzVlZWVjYzg3YzZmYmIyZDo3ODA1MTZhN2IwYjUzZDVkOWE0ZjMyMTQ0
ZWM3YjdkNTc1ODIxOGY3YzYxNTM5MWIzZGY5ZjQ0YTIyOGFjM2I4

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
	-u 5c626a21a977a0182ca9db02691f87dade20e1d70f6e671375eeecc87c6fbb2d:780516a7b0b53d5d9a4f32144ec7b7d5758218f7c615391b3df9f44a228ac3b8
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
{"grant_type":"client_credentials","client_id":"a652c1ee48fa92be35a4884ad4d20aa8a1ac786e9233a64b28c8ea27146976a6","client_secret":"c0aee69fca7a93c7e2f52fd21b5144f8a5e4c28b02c60d4ba7884c1aaf3e168b"}
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
  "access_token": "ec400a94f7581c3fe30dd21ca23ea6fc04080b49ab5f8bc7fae524f568e5fb25",
  "token_type": "bearer",
  "created_at": 1476877545
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"a652c1ee48fa92be35a4884ad4d20aa8a1ac786e9233a64b28c8ea27146976a6","client_secret":"c0aee69fca7a93c7e2f52fd21b5144f8a5e4c28b02c60d4ba7884c1aaf3e168b"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8848f7a2f631b78b60ba77b41dbb99d71a7176de588df404056688f6288e11fc","client_secret":"6de8fcb351c509595f13b252f7d0c8e8a51bf75d410063535a0c97cc6b9d287c"}
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
  "access_token": "31d11773c78b28f1ccfd6539d898599d919739b84f115e732bb698da78e4f560",
  "token_type": "bearer",
  "created_at": 1476877545
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8848f7a2f631b78b60ba77b41dbb99d71a7176de588df404056688f6288e11fc","client_secret":"6de8fcb351c509595f13b252f7d0c8e8a51bf75d410063535a0c97cc6b9d287c"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YjNlZGY5YThhNDlhOTU1MWYyNTEzMzgxODA2MmNjZTIyMTZjN2JjODY4NDk4
OGNmNDFiMGMwMzU5ODcxOTZlNDpkZDk4OTFjMzMxNWQzYzVhNDhiZGQ3ZjEy
MWIxODFlMzI5NDc0YTUyODkwOTIyNzM2NDEzNzdkZjBhZDRkMjgx

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
  "access_token": "26b862448be8d40a8c0d457698dddb153c214a435c0f91f5d180ea3650dd81cd",
  "token_type": "bearer",
  "created_at": 1476877545
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u b3edf9a8a49a9551f25133818062cce2216c7bc8684988cf41b0c035987196e4:dd9891c3315d3c5a48bdd7f121b181e329474a5289092273641377df0ad4d281
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
Authorization: Bearer 87ed87030396229f144a876abe75ee6aae6abc98ebe7ceeba3bec19dde06f9fd
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
	-H "Authorization: Bearer 87ed87030396229f144a876abe75ee6aae6abc98ebe7ceeba3bec19dde06f9fd"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/162/flashcards
Content-Type: application/json
Authorization: Bearer 348dac193476ff5241c500bbf0cbec96ce2cf21adf9489f9d37f5412ff2e47fb
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":162,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 702,
    "chapter_id": 162,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:38.921Z",
    "created_at": "2016-10-19T11:45:38.921Z",
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
curl "api.goskive.com/v2/chapters/162/flashcards" -d '{"flashcard":{"chapter_id":162,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 348dac193476ff5241c500bbf0cbec96ce2cf21adf9489f9d37f5412ff2e47fb"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/164/flashcards
Content-Type: application/json
Authorization: Bearer ca70d09116f8d449e17c5d27eada902b64d3617468077764a1be12777186ce79
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 706,
      "chapter_id": 164,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:39.214Z",
      "created_at": "2016-10-19T11:45:39.214Z",
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 706,
      "chapter_id": 164,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:39.251Z",
      "created_at": "2016-10-19T11:45:39.251Z",
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
      "author_id": 706,
      "chapter_id": 164,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:39.290Z",
      "created_at": "2016-10-19T11:45:39.290Z",
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
curl "api.goskive.com/v2/chapters/164/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca70d09116f8d449e17c5d27eada902b64d3617468077764a1be12777186ce79"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/102/questions
Content-Type: application/json
Authorization: Bearer c855609742d5e045e585682f3085914ce7d60ab3c27211991bbd6559a305550a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":102,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 61,
    "obfuscated_id": "Acd5zhQoy8g",
    "author_id": 405,
    "chapter_id": 102,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:15.305Z",
    "created_at": "2016-10-19T11:45:15.305Z",
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
        "id": 122,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 123,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 124,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 125,
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
curl "api.goskive.com/v2/chapters/102/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":102,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c855609742d5e045e585682f3085914ce7d60ab3c27211991bbd6559a305550a"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/103/questions
Content-Type: application/json
Authorization: Bearer c182680c31de723691a01405ec2325ab1daa65aac8de7f9efbbb412834cacc5c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 62,
    "obfuscated_id": "fj_KMGohXD4",
    "author_id": 408,
    "chapter_id": 103,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:15.808Z",
    "created_at": "2016-10-19T11:45:15.808Z",
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
        "id": 126,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 127,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/103/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c182680c31de723691a01405ec2325ab1daa65aac8de7f9efbbb412834cacc5c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/105/questions
Content-Type: application/json
Authorization: Bearer 64db44843bb56b54d4234c718c0f2237a28ed40fc7f3d32af664fd763cf1d978
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 414,
    "chapter_id": 105,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:16.580Z",
    "created_at": "2016-10-19T11:45:16.580Z",
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
        "id": 131,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 132,
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
curl "api.goskive.com/v2/chapters/105/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64db44843bb56b54d4234c718c0f2237a28ed40fc7f3d32af664fd763cf1d978"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/104/questions
Content-Type: application/json
Authorization: Bearer af5ee4eb0cff47036b79740c1cc1c30d6046490b7a7d482de80d239116caac09
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
    "id": 63,
    "obfuscated_id": "k3ebr8XrqxE",
    "author_id": 411,
    "chapter_id": 104,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:16.151Z",
    "created_at": "2016-10-19T11:45:16.151Z",
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
        "id": 128,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 129,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 130,
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
	-H "Authorization: Bearer af5ee4eb0cff47036b79740c1cc1c30d6046490b7a7d482de80d239116caac09"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/107/questions
Content-Type: application/json
Authorization: Bearer 3a65f956356aeb5f7767875f9d5796c6f609c06a692570f62a0307a1d638c4c8
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 420,
      "chapter_id": 107,
      "position": 52,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:17.236Z",
      "created_at": "2016-10-19T11:45:17.119Z",
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
          "id": 133,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 134,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 421,
      "chapter_id": 107,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:17.428Z",
      "created_at": "2016-10-19T11:45:17.309Z",
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
    },
    {
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 422,
      "chapter_id": 107,
      "position": 54,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T11:45:17.622Z",
      "created_at": "2016-10-19T11:45:17.502Z",
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
          "id": 137,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 138,
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
curl "api.goskive.com/v2/chapters/107/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a65f956356aeb5f7767875f9d5796c6f609c06a692570f62a0307a1d638c4c8"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/5
Content-Type: application/json
Authorization: Bearer ef77b0f23ffd51146ad62e3a9bb24e418cca9bd0a2887cf8b125bb76b62377c4
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
curl "api.goskive.com/v2/chapters/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef77b0f23ffd51146ad62e3a9bb24e418cca9bd0a2887cf8b125bb76b62377c4"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 27f2f0b69e18a5e9370085aeb89325380173ed41baee7a1d95d169203daaded8
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
curl "api.goskive.com/v2/chapters/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27f2f0b69e18a5e9370085aeb89325380173ed41baee7a1d95d169203daaded8"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/3
Content-Type: application/json
Authorization: Bearer afe9ed54b115c71457591f6083bc76c5725d88e1f4e35b9e4e2e69fd37fbe343
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
curl "api.goskive.com/v2/chapters/3" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afe9ed54b115c71457591f6083bc76c5725d88e1f4e35b9e4e2e69fd37fbe343"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/4
Content-Type: application/json
Authorization: Bearer b7d13a03f4d39bd9d62b5b5681858d9409eafbb974d81eca9c20e794a0a04e46
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7d13a03f4d39bd9d62b5b5681858d9409eafbb974d81eca9c20e794a0a04e46"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/8
Content-Type: application/json
Authorization: Bearer 956e279c40ff4d975e4ebfba5ea59a93e2a2a9476f42ba0095c64d07e3fae385
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
    "id": 8,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-19T11:44:43.446Z",
    "course_id": 8,
    "author_id": 22,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-19T11:44:42.836Z",
    "questions_updated_at": "2016-10-19T11:44:42.836Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 26,
        "chapter_id": 8,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:43.427Z",
        "created_at": "2016-10-19T11:44:43.427Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 24,
        "chapter_id": 8,
        "position": 4,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:44:43.298Z",
        "created_at": "2016-10-19T11:44:43.150Z",
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
            "id": 7,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 8,
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
curl "api.goskive.com/v2/chapters/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 956e279c40ff4d975e4ebfba5ea59a93e2a2a9476f42ba0095c64d07e3fae385"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/1
Content-Type: application/json
Authorization: Bearer f819c1c33448242088cc1a15649198934cdb7717e2b36e991fbcec42349e77ab
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
    "id": 1,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-19T11:44:41.423Z",
    "course_id": 1,
    "author_id": 2,
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
curl "api.goskive.com/v2/chapters/1" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f819c1c33448242088cc1a15649198934cdb7717e2b36e991fbcec42349e77ab"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 4430aaa7900a79ed933e09d3a03f4510d2c4f2d3a0b9599b4cd3b42604928ce0
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
    "id": 59,
    "author_id": 861,
    "reply_to_id": 58,
    "created_at": "2016-10-19T11:45:48.242Z",
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
curl "api.goskive.com/v2/comments/58/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4430aaa7900a79ed933e09d3a03f4510d2c4f2d3a0b9599b4cd3b42604928ce0"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer 17aa85c972f422ee6b8aa9fdfa65ea86d68dfa4cfd9c0a3559172ac7f1718b96
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
curl "api.goskive.com/v2/comments/60/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17aa85c972f422ee6b8aa9fdfa65ea86d68dfa4cfd9c0a3559172ac7f1718b96"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/15
Content-Type: application/json
Authorization: Bearer 13099d7dfe9c2e8efc25300e0d61f6dd176ca0bf55a38b52c64ff69a43aeef07
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
curl "api.goskive.com/v2/comments/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13099d7dfe9c2e8efc25300e0d61f6dd176ca0bf55a38b52c64ff69a43aeef07"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/54/republish
Content-Type: application/json
Authorization: Bearer 0e2ec4a67064a549dc1dbe5702942d9bb10da26d009fdb30a242e1e8797ff870
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
curl "api.goskive.com/v2/comments/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e2ec4a67064a549dc1dbe5702942d9bb10da26d009fdb30a242e1e8797ff870"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/16
Content-Type: application/json
Authorization: Bearer c29871c9b6063c6ce9c5a27d35664f16d6cb55d3508c95e0e45cabcb3d95539e
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
	-H "Authorization: Bearer c29871c9b6063c6ce9c5a27d35664f16d6cb55d3508c95e0e45cabcb3d95539e"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/55/report
Content-Type: application/json
Authorization: Bearer 1275ae2e075b250b8d96e8703759932fcdee5ee11799db80fa1fe6c4de413708
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1275ae2e075b250b8d96e8703759932fcdee5ee11799db80fa1fe6c4de413708"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/8
Content-Type: application/json
Authorization: Bearer 94ebb4e17e5f8e9b98f2b823dd741ef0b9045154ae55580e0c12f88fca38ea5c
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
    "id": 8,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-19T11:45:03.448Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94ebb4e17e5f8e9b98f2b823dd741ef0b9045154ae55580e0c12f88fca38ea5c"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 6f48578e68edc7ddfd4bf88ab7f7e125faf1fa2be49a33f0028db7edcf25fad6
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
      "id": 5,
      "name": "Fake Company Name 4",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T11:45:03.311Z"
    },
    {
      "id": 6,
      "name": "Fake Company Name 5",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T11:45:03.315Z"
    },
    {
      "id": 7,
      "name": "Fake Company Name 6",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T11:45:03.320Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f48578e68edc7ddfd4bf88ab7f7e125faf1fa2be49a33f0028db7edcf25fad6"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/39/company_profiles
Content-Type: application/json
Authorization: Bearer 806034ab94693762d6d6c94bb882850359638e331ee3064c33a3ee20ebed4aef
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
curl "api.goskive.com/v2/companies/39/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 806034ab94693762d6d6c94bb882850359638e331ee3064c33a3ee20ebed4aef"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 5d8d087fd4488d46d1d7565aeb8f027d074599626e6be4bcd896c590eb5b3c99
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
curl "api.goskive.com/v2/companies/37/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d8d087fd4488d46d1d7565aeb8f027d074599626e6be4bcd896c590eb5b3c99"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer fea965bb64371273d8b6f9982378c3594bb08fb9dcf78d98ba85cf9e7ace0c34
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
      "company_id": 31,
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
      "id": 12,
      "title": "Campaign 11",
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
	-H "Authorization: Bearer fea965bb64371273d8b6f9982378c3594bb08fb9dcf78d98ba85cf9e7ace0c34"
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
Authorization: Bearer 7269530172408e53440f4ffe0505c9ef3ca3e4a37b0d7d6a15d0af0e74fa75cf
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
	-H "Authorization: Bearer 7269530172408e53440f4ffe0505c9ef3ca3e4a37b0d7d6a15d0af0e74fa75cf"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6e4958809a69f6785db23b155ecf16a573e8ba1e7a17f8be433e96f16ec642e4
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
    "id": 43,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T11:44:59.649Z",
    "course_id": 81,
    "author_id": 174,
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
	-H "Authorization: Bearer 6e4958809a69f6785db23b155ecf16a573e8ba1e7a17f8be433e96f16ec642e4"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4df7ee6290e3d39d2763c43a9ad432abada3634560ad10b61eaf6150c0b1bb87
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
      "id": 51,
      "title": "Clever Chapter Title 36",
      "position": 1,
      "updated_at": "2016-10-19T11:45:00.642Z",
      "course_id": 86,
      "author_id": 192,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 52,
      "title": "Clever Chapter Title 37",
      "position": 2,
      "updated_at": "2016-10-19T11:45:00.668Z",
      "course_id": 86,
      "author_id": 193,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 53,
      "title": "Clever Chapter Title 38",
      "position": 3,
      "updated_at": "2016-10-19T11:45:00.923Z",
      "course_id": 86,
      "author_id": 194,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T11:45:00.563Z",
      "questions_updated_at": "2016-10-19T11:45:00.563Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4df7ee6290e3d39d2763c43a9ad432abada3634560ad10b61eaf6150c0b1bb87"
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
      "id": 57,
      "title": "Clever Chapter Title 42",
      "position": 1,
      "updated_at": "2016-10-19T11:45:01.444Z",
      "course_id": 89,
      "author_id": 206,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 58,
      "title": "Clever Chapter Title 43",
      "position": 2,
      "updated_at": "2016-10-19T11:45:01.469Z",
      "course_id": 89,
      "author_id": 207,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 59,
      "title": "Clever Chapter Title 44",
      "position": 3,
      "updated_at": "2016-10-19T11:45:01.726Z",
      "course_id": 89,
      "author_id": 208,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T11:45:01.364Z",
      "questions_updated_at": "2016-10-19T11:45:01.364Z",
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
Authorization: Bearer 171680a9424f1e0f76f1ee9d1ad26ba02afd77d1ca1113e33644c4b0a7f620ba
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
      "id": 54,
      "title": "Clever Chapter Title 39",
      "position": 1,
      "updated_at": "2016-10-19T11:45:01.098Z",
      "course_id": 87,
      "author_id": 199,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 55,
      "title": "Clever Chapter Title 40",
      "position": 2,
      "updated_at": "2016-10-19T11:45:01.127Z",
      "course_id": 87,
      "author_id": 200,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 56,
      "title": "Clever Chapter Title 41",
      "position": 3,
      "updated_at": "2016-10-19T11:45:01.152Z",
      "course_id": 87,
      "author_id": 201,
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
	-H "Authorization: Bearer 171680a9424f1e0f76f1ee9d1ad26ba02afd77d1ca1113e33644c4b0a7f620ba"
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
      "id": 60,
      "title": "Clever Chapter Title 45",
      "position": 1,
      "updated_at": "2016-10-19T11:45:01.946Z",
      "course_id": 91,
      "author_id": 213,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 61,
      "title": "Clever Chapter Title 46",
      "position": 2,
      "updated_at": "2016-10-19T11:45:01.975Z",
      "course_id": 91,
      "author_id": 214,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 62,
      "title": "Clever Chapter Title 47",
      "position": 3,
      "updated_at": "2016-10-19T11:45:02.003Z",
      "course_id": 91,
      "author_id": 215,
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
Authorization: Bearer 6cf67efaf4fc6040ca6fcdfff351ef08a166d040370c345d603b73a4b6f35e91
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
    "course_id": 95,
    "user_id": 226,
    "updated_at": "2016-10-19T11:45:02.707Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cf67efaf4fc6040ca6fcdfff351ef08a166d040370c345d603b73a4b6f35e91"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0ce3cae05d971432edbcfd7238994879a834a6487c56e4e64b3715ec6cfcd07a
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
      "course_id": 96,
      "user_id": 228,
      "updated_at": "2016-10-19T11:45:02.801Z"
    },
    {
      "id": 4,
      "course_id": 96,
      "user_id": 229,
      "updated_at": "2016-10-19T11:45:02.818Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ce3cae05d971432edbcfd7238994879a834a6487c56e4e64b3715ec6cfcd07a"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/187/files
Content-Type: application/json
Authorization: Bearer 86b3f553e30c989026a2dc5cc6c6594ffbc8c95ec787ffc45ae0d0a88a8a0f31
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
      "id": 10,
      "uploader": {
        "id": 573,
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
        "created_at": "2016-10-19T11:45:29.786Z",
        "updated_at": "2016-10-19T11:45:29.786Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T11:45:29.794Z",
      "updated_at": "2016-10-19T11:45:29.794Z",
      "course_id": 187,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 11,
      "uploader": {
        "id": 574,
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
        "created_at": "2016-10-19T11:45:29.801Z",
        "updated_at": "2016-10-19T11:45:29.801Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T11:45:29.808Z",
      "updated_at": "2016-10-19T11:45:29.808Z",
      "course_id": 187,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 12,
      "uploader": {
        "id": 575,
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
        "created_at": "2016-10-19T11:45:29.816Z",
        "updated_at": "2016-10-19T11:45:29.816Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T11:45:29.823Z",
      "updated_at": "2016-10-19T11:45:29.823Z",
      "course_id": 187,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/187/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86b3f553e30c989026a2dc5cc6c6594ffbc8c95ec787ffc45ae0d0a88a8a0f31"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/189/files
Content-Type: application/json
Authorization: Bearer e6ea487af278392e6e3bbd879f270874c34633a070d7631156d6f03abf8be0cb
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
    "id": 13,
    "uploader": {
      "id": 580,
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
      "created_at": "2016-10-19T11:45:30.063Z",
      "updated_at": "2016-10-19T11:45:30.063Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [

    ],
    "created_at": "2016-10-19T11:45:30.093Z",
    "updated_at": "2016-10-19T11:45:30.093Z",
    "course_id": 189,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/189/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6ea487af278392e6e3bbd879f270874c34633a070d7631156d6f03abf8be0cb"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/186/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 603e21c9b459ef3ad9893f24cdbc18e17a65324b76203f1ee67fda9c897f37a2
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
    "key": "cache/9f3ab513f58042e0629286440371c850.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxMjo0NToyOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS85ZjNhYjUxM2Y1ODA0MmUwNjI5Mjg2NDQwMzcxYzg1MC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTlUMTE0NTI5WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T114529Z",
    "x-amz-signature": "0506dd04055f2b53cd95cda1f721727c8f3f7cc71139be5a0d01bfdad38540da"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/186/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 603e21c9b459ef3ad9893f24cdbc18e17a65324b76203f1ee67fda9c897f37a2"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 577cc4ff5f6bdafe9caf65ce481a08bf1fa38be8d9994e3d0bf75b9da783cfc7
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
	-H "Authorization: Bearer 577cc4ff5f6bdafe9caf65ce481a08bf1fa38be8d9994e3d0bf75b9da783cfc7"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 28ce66fff2d5c60f4a966d5c4fdca480049d7370e741587b697bcf9b4303404a
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
	-H "Authorization: Bearer 28ce66fff2d5c60f4a966d5c4fdca480049d7370e741587b697bcf9b4303404a"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer dd55641e8db6d94c3c3b4e3b0bbb68de287e7f52e23aa94cb95bd8fcf57a4117
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
	-H "Authorization: Bearer dd55641e8db6d94c3c3b4e3b0bbb68de287e7f52e23aa94cb95bd8fcf57a4117"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fd79d336bf1e2050bab6d83c7f54919901bde1b3ce23a61c87757253aea59057
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
	-H "Authorization: Bearer fd79d336bf1e2050bab6d83c7f54919901bde1b3ce23a61c87757253aea59057"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 593f3eb78dee266942c7831d02c0ea504c05a48d0bd1472bb87557b37d06c07a
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
	-H "Authorization: Bearer 593f3eb78dee266942c7831d02c0ea504c05a48d0bd1472bb87557b37d06c07a"
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
    "id": 293,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 278,
    "additional_university_ids": [

    ],
    "topic_id": 300,
    "discipline_id": 301,
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
    "chapters_updated_at": "2016-10-19T11:45:52.782Z",
    "updated_at": "2016-10-19T11:45:54.259Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 181,
        "title": "Clever Chapter Title 157",
        "position": 1,
        "updated_at": "2016-10-19T11:45:54.207Z",
        "course_id": 293,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T11:45:52.782Z",
        "questions_updated_at": "2016-10-19T11:45:52.782Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 182,
        "title": "Clever Chapter Title 158",
        "position": 2,
        "updated_at": "2016-10-19T11:45:54.251Z",
        "course_id": 293,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T11:45:52.782Z",
        "questions_updated_at": "2016-10-19T11:45:52.782Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 109,
        "obfuscated_id": "VSPyck5c2RY",
        "author_id": 902,
        "chapter_id": 181,
        "position": 96,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:53.003Z",
        "created_at": "2016-10-19T11:45:52.884Z",
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
            "id": 221,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 222,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 111,
        "obfuscated_id": "G-D-sgMUtTw",
        "author_id": 902,
        "chapter_id": 182,
        "position": 98,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:53.394Z",
        "created_at": "2016-10-19T11:45:53.272Z",
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
Authorization: Bearer 275c7b98a7ec9efd58f51606072dffdd7966488bbe0a83e685d648560a397c53
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
    "id": 295,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 280,
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
    "chapters_updated_at": "2016-10-19T11:45:56.051Z",
    "updated_at": "2016-10-19T11:45:57.523Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 185,
        "title": "Clever Chapter Title 161",
        "position": 1,
        "updated_at": "2016-10-19T11:45:57.475Z",
        "course_id": 295,
        "author_id": 913,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T11:45:56.051Z",
        "questions_updated_at": "2016-10-19T11:45:56.051Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 186,
        "title": "Clever Chapter Title 162",
        "position": 2,
        "updated_at": "2016-10-19T11:45:57.516Z",
        "course_id": 295,
        "author_id": 913,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T11:45:56.051Z",
        "questions_updated_at": "2016-10-19T11:45:56.051Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 914,
        "chapter_id": 185,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:57.308Z",
        "created_at": "2016-10-19T11:45:57.308Z",
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
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 914,
        "chapter_id": 186,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:57.381Z",
        "created_at": "2016-10-19T11:45:57.381Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 914,
        "chapter_id": 185,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:57.349Z",
        "created_at": "2016-10-19T11:45:57.349Z",
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
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 914,
        "chapter_id": 186,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:57.424Z",
        "created_at": "2016-10-19T11:45:57.424Z",
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
        "id": 121,
        "obfuscated_id": "LQhaXfRg6ZA",
        "author_id": 914,
        "chapter_id": 185,
        "position": 108,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:56.270Z",
        "created_at": "2016-10-19T11:45:56.156Z",
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
        "author_id": 914,
        "chapter_id": 185,
        "position": 109,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:56.448Z",
        "created_at": "2016-10-19T11:45:56.337Z",
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
      },
      {
        "id": 123,
        "obfuscated_id": "N9-wuAhut60",
        "author_id": 914,
        "chapter_id": 186,
        "position": 110,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:56.653Z",
        "created_at": "2016-10-19T11:45:56.532Z",
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
        "chapter_id": 186,
        "position": 111,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T11:45:56.837Z",
        "created_at": "2016-10-19T11:45:56.722Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 275c7b98a7ec9efd58f51606072dffdd7966488bbe0a83e685d648560a397c53"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/291/pin
Content-Type: application/json
Authorization: Bearer 202fcb639312ad737fa4d8e681814aebedb1a558555c6a220ec1a3c4af5943d0
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/291/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 202fcb639312ad737fa4d8e681814aebedb1a558555c6a220ec1a3c4af5943d0"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/296/pin
Content-Type: application/json
Authorization: Bearer 9247f706551a490348b50d743b16391b35cd4ce8bf786f0010d8809fd94c0304
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/296/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9247f706551a490348b50d743b16391b35cd4ce8bf786f0010d8809fd94c0304"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b5984d8bb02e48b276202e503407d232fb87c2909da1a198e7386aba1b26fe4e
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
    "creator_id": 867,
    "id": 278,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 263,
    "additional_university_ids": [

    ],
    "topic_id": 285,
    "discipline_id": 286,
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
    "updated_at": "2016-10-19T11:45:48.881Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5984d8bb02e48b276202e503407d232fb87c2909da1a198e7386aba1b26fe4e"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 4da71df04fee791c2001a05cddf4074730275b54ca3ac80b5446db955ffa09e8
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
    "id": 944,
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
    "created_at": "2016-10-19T11:46:00.335Z",
    "updated_at": "2016-10-19T11:46:00.335Z",
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
	-H "Authorization: Bearer 4da71df04fee791c2001a05cddf4074730275b54ca3ac80b5446db955ffa09e8"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d56da988ef1e670baee1fd38ca4116c769440b9df807bbaa7bcc338a3a02500b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[312]}
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
    "id": 945,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      312
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T11:46:00.429Z",
    "updated_at": "2016-10-19T11:46:00.469Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[312]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d56da988ef1e670baee1fd38ca4116c769440b9df807bbaa7bcc338a3a02500b"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer e4fceffea47f7afdf2f122869fe0cfa0506a4cc326d7be20d6ff48755d85314c
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
    "id": 948,
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
    "created_at": "2016-10-19T11:46:00.649Z",
    "updated_at": "2016-10-19T11:46:00.649Z",
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
	-H "Authorization: Bearer e4fceffea47f7afdf2f122869fe0cfa0506a4cc326d7be20d6ff48755d85314c"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0ad8f3d71f924fdae6f928f1a573ab8719cdfa43291213fcb3f3ad582c154325
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[314]}
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
    "id": 947,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      314
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T11:46:00.597Z",
    "updated_at": "2016-10-19T11:46:00.597Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[314]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ad8f3d71f924fdae6f928f1a573ab8719cdfa43291213fcb3f3ad582c154325"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 66fe552852abbbf0d6d93174c0de77a7e0ae25be4a1a2dacc3878c360168fd09
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

316
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
    "id": 949,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/ad3e1b10ba8ecbff2a6bce9ab9ad6d0c9da8cbe7.jpg",
    "university_id": null,
    "fields_of_study": [
      316
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T11:46:00.752Z",
    "updated_at": "2016-10-19T11:46:01.026Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/30b951922a7a81d7726f1e4017c9a5aec527ea2c.jpg",
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

316
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 66fe552852abbbf0d6d93174c0de77a7e0ae25be4a1a2dacc3878c360168fd09"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 296e90378ba7acb78aa0a362d5babfe79d9fbdba95f435d01e54825b5b6a0191
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
      "bookmarkable_id": 58,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 59,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 60,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 296e90378ba7acb78aa0a362d5babfe79d9fbdba95f435d01e54825b5b6a0191"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer fe4038c09833012f71143ad5fc8c55a871bc987a6de1994458ab2863b8b248e0
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
      "company_id": 13,
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 14,
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
	-H "Authorization: Bearer fe4038c09833012f71143ad5fc8c55a871bc987a6de1994458ab2863b8b248e0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1ec8351898424cfc5b7b2cb2ee111a14157ffb321a3e2952b37e6098102b89e8
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
      "title": "Campaign 1",
      "company_id": 9,
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
	-H "Authorization: Bearer 1ec8351898424cfc5b7b2cb2ee111a14157ffb321a3e2952b37e6098102b89e8"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 2dee682cfe4cd43789de8c53b9ceda9810ff658f7813fac6443d2a29d5d894a2
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
      "creator_id": 547,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-135",
      "html_url": "https://goskive.com/course/mit-course-135",
      "slug": "mit-course-135",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "updated_at": "2016-10-19T11:45:26.951Z",
      "shortname": "mit-course-135"
    },
    {
      "creator_id": 548,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-136",
      "html_url": "https://goskive.com/course/mit-course-136",
      "slug": "mit-course-136",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
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
      "updated_at": "2016-10-19T11:45:27.045Z",
      "shortname": "mit-course-136"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dee682cfe4cd43789de8c53b9ceda9810ff658f7813fac6443d2a29d5d894a2"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cfa0748b82a6cd97d74bb3c60e7c299e2f8556b5ec508b962c032c38cd86e5e0
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
        "updated_at": "2016-10-19T11:45:29.481Z"
      },
      "created_at": "2016-10-19T11:45:29.485Z",
      "updated_at": "2016-10-19T11:45:29.485Z",
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
        "updated_at": "2016-10-19T11:45:29.494Z"
      },
      "created_at": "2016-10-19T11:45:29.498Z",
      "updated_at": "2016-10-19T11:45:29.498Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfa0748b82a6cd97d74bb3c60e7c299e2f8556b5ec508b962c032c38cd86e5e0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer bcf9772ee60d9b3334e9c0e3ed74bcd593ad92afe13fdb5ce237c914c310f5f1
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 16",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T11:45:29.250Z"
      },
      "created_at": "2016-10-19T11:45:29.254Z",
      "updated_at": "2016-10-19T11:45:29.254Z",
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
      "company_id": 19,
      "company": {
        "id": 19,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-19T11:45:29.270Z"
      },
      "created_at": "2016-10-19T11:45:29.273Z",
      "updated_at": "2016-10-19T11:45:29.273Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcf9772ee60d9b3334e9c0e3ed74bcd593ad92afe13fdb5ce237c914c310f5f1"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 4db8a723dabf44bb9c9309e939ce838b1e1a3f8d1c9600f63a726ff0cb716bc6
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
      "id": 6,
      "created_at": "2016-10-19T11:45:17.905Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-10-19T11:45:18.016Z",
      "author_id": "427",
      "thread_subject_id": "144",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 7,
      "created_at": "2016-10-19T11:45:18.004Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-10-19T11:45:18.021Z",
      "author_id": "430",
      "thread_subject_id": "145",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-10-19T11:45:18.395Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-19T11:45:18.395Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 9,
      "created_at": "2016-10-19T11:45:18.818Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-10-19T11:45:18.818Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 10,
      "created_at": "2016-10-19T11:45:19.227Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-10-19T11:45:19.227Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 11,
      "created_at": "2016-10-19T11:45:19.552Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 71,
      "updated_at": "2016-10-19T11:45:19.552Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-10-19T11:45:19.839Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 72,
      "updated_at": "2016-10-19T11:45:19.839Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 13,
      "created_at": "2016-10-19T11:45:20.120Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 73,
      "updated_at": "2016-10-19T11:45:20.120Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4db8a723dabf44bb9c9309e939ce838b1e1a3f8d1c9600f63a726ff0cb716bc6"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer 2cee718ffefff10e34dbeb6047138f4676bf38e02a798eb1d1b815925540c405
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-19T11:35:20.000Z"}}
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
    "created_at": "2016-10-19T11:45:20.257Z",
    "read_at": "2016-10-19T11:35:20.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 8,
    "updated_at": "2016-10-19T11:45:20.298Z",
    "author_id": "455",
    "thread_subject_id": "152",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-10-19T11:35:20.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cee718ffefff10e34dbeb6047138f4676bf38e02a798eb1d1b815925540c405"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f7e6433275845ccd686d5c023d918535cfe0044089bb7cc9d9dfcaebb5efba28
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
      "course_id": 157,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T11:45:20.959Z",
      "course_published": true,
      "updated_at": "2016-10-19T11:45:20.951Z"
    },
    {
      "id": 5,
      "course_id": 158,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T11:45:21.046Z",
      "course_published": true,
      "updated_at": "2016-10-19T11:45:21.037Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7e6433275845ccd686d5c023d918535cfe0044089bb7cc9d9dfcaebb5efba28"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 5d0bfef08cda5da8963eb4a32cf4751503832b6c7d41ec652c2058a89eed6a08
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
    "course_id": 156,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T11:45:20.790Z",
    "course_published": true,
    "updated_at": "2016-10-19T11:45:20.783Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d0bfef08cda5da8963eb4a32cf4751503832b6c7d41ec652c2058a89eed6a08"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 816528068f34f31fe512bf5ecb6a5d5009aa8fa1a39e304bada2e43cb0ba1fdc
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
    "course_id": 155,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-19T11:45:20.691Z",
    "course_published": true,
    "updated_at": "2016-10-19T11:45:20.681Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 816528068f34f31fe512bf5ecb6a5d5009aa8fa1a39e304bada2e43cb0ba1fdc"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer da818572b14c041f0a145da5f905e2dfc6b2f14a2222ef4eda2f5856582163bb
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
      "votable_id": 131,
      "user_id": 951
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 132,
      "user_id": 951
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 951
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 134,
      "user_id": 951
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da818572b14c041f0a145da5f905e2dfc6b2f14a2222ef4eda2f5856582163bb"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/224
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
    "id": 224,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 224,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 224
      },
      {
        "id": 225,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 224
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/224" -X GET \
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
      "id": 225,
      "name": "Up-sized web-enabled moderator",
      "name_translations": {
        "en": "Up-sized web-enabled moderator"
      }
    },
    {
      "id": 226,
      "name": "Versatile responsive capacity",
      "name_translations": {
        "en": "Versatile responsive capacity"
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
Authorization: Bearer 55f8c350c961658c23e4542fd3844c4e947c88e30acdc31903cdf91ec9562ecc
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
    "user_id": 250,
    "feedbackable_id": 13,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-19T11:45:03.904Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55f8c350c961658c23e4542fd3844c4e947c88e30acdc31903cdf91ec9562ecc"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 95d1936dd246ae463e90ef110a2bcf4ac5f5c77d67acf4095e9b29fa1cbd6cde
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
    "user_id": 353,
    "feedbackable_id": 17,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-19T11:45:11.148Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95d1936dd246ae463e90ef110a2bcf4ac5f5c77d67acf4095e9b29fa1cbd6cde"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/4
Content-Type: application/json
Authorization: Bearer c156c8dd7938f0b5d97687b52f16f72d15e2d498b3e8114b99d561d7772e3a46
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
    "id": 4,
    "user_id": 260,
    "feedbackable_id": 15,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T11:45:04.606Z",
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
curl "api.goskive.com/v2/feedbacks/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c156c8dd7938f0b5d97687b52f16f72d15e2d498b3e8114b99d561d7772e3a46"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer 00417f047ca9b0dc412cf59ac37666d5f61ab5a4f75d56641cdd482182fa641b
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
curl "api.goskive.com/v2/feedbacks/1/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00417f047ca9b0dc412cf59ac37666d5f61ab5a4f75d56641cdd482182fa641b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer a87e07a81aa7cf714b4c666d8c6de506ae3b12425dd01a2f97a23c6aa8528a2a
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
	-H "Authorization: Bearer a87e07a81aa7cf714b4c666d8c6de506ae3b12425dd01a2f97a23c6aa8528a2a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 9ebd789256fb54fba18f9ec748b5a6cc34ec8a2c34f16dc0466a6e891863d6e2
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
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ebd789256fb54fba18f9ec748b5a6cc34ec8a2c34f16dc0466a6e891863d6e2"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer 6f6cd52d02e3e5ecbfcdad968c7c6454dfea2f8fc50d93e4fa2036c69ec3d06b
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
    "id": 5,
    "user_id": 265,
    "feedbackable_id": 16,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T11:45:04.928Z",
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
curl "api.goskive.com/v2/feedbacks/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f6cd52d02e3e5ecbfcdad968c7c6454dfea2f8fc50d93e4fa2036c69ec3d06b"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/4
Content-Type: application/json
Authorization: Bearer 8268b33d69892b19725a3e123700897f9807889341d7f20d59bc45a3e506ad7c
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
	-H "Authorization: Bearer 8268b33d69892b19725a3e123700897f9807889341d7f20d59bc45a3e506ad7c"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/2
Content-Type: application/json
Authorization: Bearer e7d488a6dbc92cd58e2be4c272a128680e923fd8ce3d05dbb0f1e8a6edf9e224
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7d488a6dbc92cd58e2be4c272a128680e923fd8ce3d05dbb0f1e8a6edf9e224"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/5
Content-Type: application/json
Authorization: Bearer bf76fdfaa46984ee41b82e9f1f745236bb1231beeb1199da2f04cfe2cce80745
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/d116a3bbac525f55b8b9c1b5be00a3d0.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T114526Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=a3a9e13e609bace6b931da436e263d285f72069c59dccd1c30c971c38ae9119d"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf76fdfaa46984ee41b82e9f1f745236bb1231beeb1199da2f04cfe2cce80745"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/1/preview
Content-Type: application/json
Authorization: Bearer 6f5ceb0173770bd09bd07a205f92ba6d38fe4b6321334fa81a2027c532620ccc
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/ff56e229d39b35d57b9b278e53126f57.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T114525Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=8a96f310c42691dd8ee965fcb2db9501b02e8e9cac3eee18fbd750191d7a4e6d"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/1/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f5ceb0173770bd09bd07a205f92ba6d38fe4b6321334fa81a2027c532620ccc"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Content-Type: application/json
Authorization: Bearer c32305aebc7e507c75e1449af1138002939a549ba059e017f371a71646f085b6
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
      "id": 543,
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
      "created_at": "2016-10-19T11:45:26.736Z",
      "updated_at": "2016-10-19T11:45:26.736Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-19T11:45:26.814Z",
    "updated_at": "2016-10-19T11:45:26.814Z",
    "course_id": 178,
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
	-H "Authorization: Bearer c32305aebc7e507c75e1449af1138002939a549ba059e017f371a71646f085b6"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/15/matched_courses?required_cu_count=2
Authorization: Bearer 66f82c178281d51ea1f655f3e613400ff23993bd8619262591dbcd591469b661
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
      "creator_id": 594,
      "id": 193,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 177,
      "additional_university_ids": [

      ],
      "topic_id": 193,
      "discipline_id": 193,
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
      "chapters_updated_at": "2016-10-19T11:45:30.273Z",
      "updated_at": "2016-10-19T11:45:31.915Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 599,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-5fe0e255-fbbd-4939-b008-8b200b7f7d11",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-5fe0e255-fbbd-4939-b008-8b200b7f7d11",
      "slug": "mit-the-great-british-bake-off-5fe0e255-fbbd-4939-b008-8b200b7f7d11",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "topic_id": 194,
      "discipline_id": 194,
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
      "chapters_updated_at": "2016-10-19T11:45:30.273Z",
      "updated_at": "2016-10-19T11:45:32.530Z",
      "shortname": "mit-the-great-british-bake-off-5fe0e255-fbbd-4939-b008-8b200b7f7d11"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/15/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 66f82c178281d51ea1f655f3e613400ff23993bd8619262591dbcd591469b661"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/6/report
Content-Type: application/json
Authorization: Bearer de665cb04440d0eda61456d111b4ab3bf9881d8d4f76707c7aa4ec6cae5979fb
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de665cb04440d0eda61456d111b4ab3bf9881d8d4f76707c7aa4ec6cae5979fb"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/24/comments
Content-Type: application/json
Authorization: Bearer 9c605c2c8d13b40e922218b5869c2e8bad4e0b3abe72c37646b4170ca0bf3823
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
    "author_id": 386,
    "reply_to_id": null,
    "created_at": "2016-10-19T11:45:13.594Z",
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
curl "api.goskive.com/v2/flashcards/24/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c605c2c8d13b40e922218b5869c2e8bad4e0b3abe72c37646b4170ca0bf3823"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/25/comments
Content-Type: application/json
Authorization: Bearer baac8f11b9c1552ba2fd2ee8342ea91189ad5ed5237158109c66323807718df8
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
    "author_id": 389,
    "reply_to_id": null,
    "created_at": "2016-10-19T11:45:13.996Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 29,
      "user_id": 389,
      "feedbackable_id": 25,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:13.993Z",
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
	-H "Authorization: Bearer baac8f11b9c1552ba2fd2ee8342ea91189ad5ed5237158109c66323807718df8"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/22/comments
Content-Type: application/json
Authorization: Bearer 0ffae53c7c6ad9392d3e4bab38c3f78b074996ca456c7ffe699ff3d8c996a20f
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
      "id": 3,
      "author_id": 382,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:13.198Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 381,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:13.180Z",
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
	-H "Authorization: Bearer 0ffae53c7c6ad9392d3e4bab38c3f78b074996ca456c7ffe699ff3d8c996a20f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/23/comments
Content-Type: application/json
Authorization: Bearer 4b825164da6b891eb0ce8e6dd4af87cceb08f4125918b60cce393aef269a8e4a
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
curl "api.goskive.com/v2/flashcards/23/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b825164da6b891eb0ce8e6dd4af87cceb08f4125918b60cce393aef269a8e4a"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/62/feedbacks
Content-Type: application/json
Authorization: Bearer c9dc3f1e8a224ba0d9e9ea62cea5c87c2994fa45a3bb35384cf27021b673865b
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
    "id": 40,
    "user_id": 820,
    "feedbackable_id": 62,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T11:45:46.117Z",
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
curl "api.goskive.com/v2/flashcards/62/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9dc3f1e8a224ba0d9e9ea62cea5c87c2994fa45a3bb35384cf27021b673865b"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer fe343d925f2be3c800d0f4c7552f15ed019e111c697962363c8e72bfe9bc8923
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
      "user_id": 844,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:47.045Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 843,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:47.033Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/66/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe343d925f2be3c800d0f4c7552f15ed019e111c697962363c8e72bfe9bc8923"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer 3cf8fe32b3653664ea0621d95f6e252ef22a6562ec7ee98517970117bfdc687c
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
      "votable_id": 27,
      "user_id": 481
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 480
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 479
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3cf8fe32b3653664ea0621d95f6e252ef22a6562ec7ee98517970117bfdc687c"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/34/republish
Content-Type: application/json
Authorization: Bearer 008145fb7750c3defe4f9b0776d38964beea06e9293fa9b8ed9121d770045c39
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
curl "api.goskive.com/v2/flashcards/34/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 008145fb7750c3defe4f9b0776d38964beea06e9293fa9b8ed9121d770045c39"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/36/bookmark
Content-Type: application/json
Authorization: Bearer 272f044482b1331e6f65e8a9bd2535a598a99c3fe60fdd3fee056a41b675eaf3
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
	-H "Authorization: Bearer 272f044482b1331e6f65e8a9bd2535a598a99c3fe60fdd3fee056a41b675eaf3"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/53
Content-Type: application/json
Authorization: Bearer a866f017329c30e0f1ef7c8dc27c50a791572f1a19be8d460a21d01a99a1abb4
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a866f017329c30e0f1ef7c8dc27c50a791572f1a19be8d460a21d01a99a1abb4"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/downvote
Content-Type: application/json
Authorization: Bearer 8ec7f3cf8e85ed9508d75645eaf4de9a8259d69c8ef1d662893d31db32185823
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ec7f3cf8e85ed9508d75645eaf4de9a8259d69c8ef1d662893d31db32185823"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/54
Content-Type: application/json
Authorization: Bearer 86fd12add5c552f4ee5a22ac67b587a736d6a058a0585cd91b28d677021284d7
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
    "id": 54,
    "obfuscated_id": "cKxlQSpHm5w",
    "author_id": 691,
    "chapter_id": 159,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:45:37.996Z",
    "created_at": "2016-10-19T11:45:37.996Z",
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
curl "api.goskive.com/v2/flashcards/54" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86fd12add5c552f4ee5a22ac67b587a736d6a058a0585cd91b28d677021284d7"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/report
Content-Type: application/json
Authorization: Bearer cf2304f0f4b20340a04f1de5b679f10cae2a17c5447427e8282d2174a9b8942e
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/56/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf2304f0f4b20340a04f1de5b679f10cae2a17c5447427e8282d2174a9b8942e"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/55/bookmark
Content-Type: application/json
Authorization: Bearer 4d20ab1bf422309b40fa22dc01df1b13810b9c5e8072d9ae29647a8dcfffa87b
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/55/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d20ab1bf422309b40fa22dc01df1b13810b9c5e8072d9ae29647a8dcfffa87b"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/upvote
Content-Type: application/json
Authorization: Bearer b83a779956106f1f9cd0699966934557ee5363daf9f25d7ab23a01e2a6439aa6
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b83a779956106f1f9cd0699966934557ee5363daf9f25d7ab23a01e2a6439aa6"
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
    "key": "cache/da865fa090bb1bf8667826fed215fbc8.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxMjo0NTo0N1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9kYTg2NWZhMDkwYmIxYmY4NjY3ODI2ZmVkMjE1ZmJjOC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE5L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOVQxMTQ1NDdaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T114547Z",
    "x-amz-signature": "9c5c070f3992c0262479c66d04dc64a5372a2206e4c0d58633fe6dccdbafe277"
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
Authorization: Bearer 967ce1402c831bbad81acb5c0898eed55ed868b5074a98e9e4a125ee82bd156a
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
	-H "Authorization: Bearer 967ce1402c831bbad81acb5c0898eed55ed868b5074a98e9e4a125ee82bd156a"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer a153dafb3f9f92fddb79dd94023eff3eb39c5916158eaa696ba351ed4d68d759
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
	-H "Authorization: Bearer a153dafb3f9f92fddb79dd94023eff3eb39c5916158eaa696ba351ed4d68d759"
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
{"password":{"reset_password_token":"rT6_MU3ueTKmHMzq1y-s","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 802,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-19T11:45:43.749Z",
  "updated_at": "2016-10-19T11:45:44.355Z",
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
  "audit_id": 4892
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"rT6_MU3ueTKmHMzq1y-s","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/83/comments
Content-Type: application/json
Authorization: Bearer eb3a336ecb6c634ae9981c74b1a59cc41bd24a996ed197ffe0619f4039b9c146
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
    "id": 11,
    "author_id": 553,
    "reply_to_id": null,
    "created_at": "2016-10-19T11:45:27.832Z",
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
curl "api.goskive.com/v2/questions/83/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb3a336ecb6c634ae9981c74b1a59cc41bd24a996ed197ffe0619f4039b9c146"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/84/comments
Content-Type: application/json
Authorization: Bearer 56f2d27746604f608b37e9faf02e734397c1f2dd92f7e27faaca0255ebc2f286
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
    "id": 12,
    "author_id": 556,
    "reply_to_id": null,
    "created_at": "2016-10-19T11:45:28.345Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 556,
      "feedbackable_id": 84,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:28.342Z",
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
curl "api.goskive.com/v2/questions/84/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56f2d27746604f608b37e9faf02e734397c1f2dd92f7e27faaca0255ebc2f286"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/86/comments
Content-Type: application/json
Authorization: Bearer 1b32beb4fd337592c7e495f17050090bbaf11fc4c2a691d2e66f00332ccee33d
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
      "author_id": 565,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:29.167Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 566,
      "reply_to_id": null,
      "created_at": "2016-10-19T11:45:29.185Z",
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
curl "api.goskive.com/v2/questions/86/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b32beb4fd337592c7e495f17050090bbaf11fc4c2a691d2e66f00332ccee33d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/82/comments
Content-Type: application/json
Authorization: Bearer ef69d1fe7bfb94b06cb662ac4f522996c525742b471d9bdce672deb965de9262
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
curl "api.goskive.com/v2/questions/82/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef69d1fe7bfb94b06cb662ac4f522996c525742b471d9bdce672deb965de9262"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/80/feedbacks
Content-Type: application/json
Authorization: Bearer 27cb61afad9bcdb927c041e0d0d25289753d03a68a13e26d1653ee507b2bd8f6
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
    "id": 36,
    "user_id": 515,
    "feedbackable_id": 80,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-19T11:45:24.687Z",
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
curl "api.goskive.com/v2/questions/80/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27cb61afad9bcdb927c041e0d0d25289753d03a68a13e26d1653ee507b2bd8f6"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/74/feedbacks
Content-Type: application/json
Authorization: Bearer fb06aeb17856701da2b73cc2df27998fc8e5e3cddeccdaa3f43cdf728250bbf1
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
      "id": 31,
      "user_id": 489,
      "feedbackable_id": 74,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:22.605Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 488,
      "feedbackable_id": 74,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T11:45:22.590Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/74/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb06aeb17856701da2b73cc2df27998fc8e5e3cddeccdaa3f43cdf728250bbf1"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/95/votes
Content-Type: application/json
Authorization: Bearer aca77c452e3b7bd7821213ab3ac9c8975e94055cda08167a60c0d652bbc83514
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
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 95,
      "user_id": 612
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 95,
      "user_id": 611
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 95,
      "user_id": 610
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/95/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aca77c452e3b7bd7821213ab3ac9c8975e94055cda08167a60c0d652bbc83514"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/30/republish
Content-Type: application/json
Authorization: Bearer 790ff86503532a5c333df1399984616f703ac35422254d11f376b9bd0a6391c5
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
curl "api.goskive.com/v2/questions/30/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 790ff86503532a5c333df1399984616f703ac35422254d11f376b9bd0a6391c5"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/26/bookmark
Content-Type: application/json
Authorization: Bearer ed9aacf20b7eb0cfe5c90f964ececd45fe4257366196f90bebd8abe9c6e4d9e2
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/26/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed9aacf20b7eb0cfe5c90f964ececd45fe4257366196f90bebd8abe9c6e4d9e2"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/29
Content-Type: application/json
Authorization: Bearer aa076989fe50c105e0c83b0e59ed9bc6b955bd153a76114bbca16f9b9cb2ae13
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/29" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa076989fe50c105e0c83b0e59ed9bc6b955bd153a76114bbca16f9b9cb2ae13"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/24/downvote
Content-Type: application/json
Authorization: Bearer 217e811dc14467c71f2ea4621bb287bdea80991af458621dbb51a04fb2145543
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 217e811dc14467c71f2ea4621bb287bdea80991af458621dbb51a04fb2145543"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/23
Content-Type: application/json
Authorization: Bearer 26f4ff1fe2dc561fe91e04d32a1525ce4fa38bed6e7dcfb40fb79f3ffff03a32
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 94,
    "chapter_id": 26,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:44:50.507Z",
    "created_at": "2016-10-19T11:44:50.392Z",
    "tags": [
      {
        "id": 4,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 3,
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
        "id": 46,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 47,
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
curl "api.goskive.com/v2/questions/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26f4ff1fe2dc561fe91e04d32a1525ce4fa38bed6e7dcfb40fb79f3ffff03a32"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/25/report
Content-Type: application/json
Authorization: Bearer 04c4fc1d3441ad76a01b4e6fb1876c9f4f7f1e6c264eb15f14686bebf8b553f0
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
	-H "Authorization: Bearer 04c4fc1d3441ad76a01b4e6fb1876c9f4f7f1e6c264eb15f14686bebf8b553f0"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/27/bookmark
Content-Type: application/json
Authorization: Bearer 8833db715edb88aa9dbeb3f135e1339fa7495850b22b8349c851eb8f6a5e22a6
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8833db715edb88aa9dbeb3f135e1339fa7495850b22b8349c851eb8f6a5e22a6"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/7
Content-Type: application/json
Authorization: Bearer 4a4b98a251d0a2741c7980ca0831b6b319a456b3062a55f8a58b62996331e72d
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":7,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T11:44:44.959Z","updated_at":"2016-10-19T11:44:45.080Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":10,"author_id":41,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 7,
    "obfuscated_id": "XFkue8saGAM",
    "author_id": 41,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T11:44:45.224Z",
    "created_at": "2016-10-19T11:44:44.959Z",
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
    "question": "{\"id\"=>7, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-19T11:44:44.959Z\", \"updated_at\"=>\"2016-10-19T11:44:45.080Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>10, \"author_id\"=>41, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 13,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 14,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 15,
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
curl "api.goskive.com/v2/questions/7" -d '{"question":{"question":{"id":7,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T11:44:44.959Z","updated_at":"2016-10-19T11:44:45.080Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":10,"author_id":41,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a4b98a251d0a2741c7980ca0831b6b319a456b3062a55f8a58b62996331e72d"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/28/upvote
Content-Type: application/json
Authorization: Bearer a02a49a48b699cd2d501132e3c259edff4e322e94a3b3dc13058d63b408dad6a
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/28/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a02a49a48b699cd2d501132e3c259edff4e322e94a3b3dc13058d63b408dad6a"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer c15eb897d92e544e8e7dac403b92fde12c06f315aeace070000f857e0443e6c6
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
      "creator_id": 38,
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 11,
      "discipline_id": 11,
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
      "updated_at": "2016-10-19T11:44:44.538Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c15eb897d92e544e8e7dac403b92fde12c06f315aeace070000f857e0443e6c6"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 789372ae37bec2a5c967f8a7040f62dd2f0c5ac0a6e4c1df84fbfb1b3b9d9f76
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
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-11",
      "html_url": "https://goskive.com/university/uni-11",
      "slug": "uni-11",
      "name": "National School of Pizza",
      "short_name": "Uni 11",
      "acronym": "NSPI",
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
      "updated_at": "2016-10-19T11:44:44.211Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 10,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-10",
      "html_url": "https://goskive.com/university/uni-10",
      "slug": "uni-10",
      "name": "National School of Pastry",
      "short_name": "Uni 10",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/907b97acad454546ae110f7cad7c8a133f868482.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/590c7f8b9d9c518ab5b695e676ac1e98a5606cc2.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T11:44:44.194Z",
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
	-H "Authorization: Bearer 789372ae37bec2a5c967f8a7040f62dd2f0c5ac0a6e4c1df84fbfb1b3b9d9f76"
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
      "id": 279,
      "name": "Re-engineered mission-critical initiative",
      "name_translations": {
        "en": "Re-engineered mission-critical initiative"
      },
      "discipline_id": 280
    },
    {
      "id": 280,
      "name": "Down-sized disintermediate Graphic Interface",
      "name_translations": {
        "en": "Down-sized disintermediate Graphic Interface"
      },
      "discipline_id": 281
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
GET /v2/topics/278
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
    "id": 278,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 279
  }
}
```



```shell
curl "api.goskive.com/v2/topics/278" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer a7aa8244fc203d3535754d3bbdf365be98e257a37fed7ae7f04f306fa4ebe168
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
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-120",
      "html_url": "https://goskive.com/university/uni-120",
      "slug": "uni-120",
      "name": "University 79",
      "short_name": "Uni 120",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9c6d4a02aaa10e209b469cca6dfb9e9f70584ae2.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4ffc6a0934a0fcfefc12f93f32ab4f698a70f36e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T11:45:21.287Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-121",
      "html_url": "https://goskive.com/university/uni-121",
      "slug": "uni-121",
      "name": "University 80",
      "short_name": "Uni 121",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/028e2c78fc16120f1cddd69a9aab85c5e925ba88.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/de5e8cc9ffbd1c7e3a93e097bfe367e4eb856f07.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T11:45:21.304Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-122",
      "html_url": "https://goskive.com/university/uni-122",
      "slug": "uni-122",
      "name": "University 81",
      "short_name": "Uni 122",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4e8c460abbec499dd99d478cc172f1e311637150.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cd0031c8786d89a75fa1088367b50eae39532c27.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T11:45:21.321Z",
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
	-H "Authorization: Bearer a7aa8244fc203d3535754d3bbdf365be98e257a37fed7ae7f04f306fa4ebe168"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 491fddebac221c5931a3398ae38841cb98bdbbd4bb2671ed5446a55de53d2a63
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
    "id": 139,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ab579cf0549c0e7eba559c572851343dff25569f.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8f32c6a49762b023840149b8fa2b39f07948f63c.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-19T11:45:21.189Z",
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
	-H "Authorization: Bearer 491fddebac221c5931a3398ae38841cb98bdbbd4bb2671ed5446a55de53d2a63"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 46c5c4b9337e2f23079cc9e6b0e9e2058622e610bd8a746ceb274f9fb629a3ca
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":41,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 126,
    "id": 41,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 42,
    "additional_university_ids": [

    ],
    "topic_id": 41,
    "discipline_id": 41,
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
    "chapters_updated_at": "2016-10-19T11:44:54.969Z",
    "updated_at": "2016-10-19T11:44:55.139Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 35,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-19T11:44:55.092Z",
        "course_id": 41,
        "author_id": 126,
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
        "id": 36,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-19T11:44:55.110Z",
        "course_id": 41,
        "author_id": 126,
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
        "id": 37,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-19T11:44:55.128Z",
        "course_id": 41,
        "author_id": 126,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":41,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46c5c4b9337e2f23079cc9e6b0e9e2058622e610bd8a746ceb274f9fb629a3ca"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1c41cb9a59b75d4f93a728c13c1644ad20a84551371fc5e35e56784f878a010e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}
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
    "creator_id": 125,
    "id": 40,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 41,
    "additional_university_ids": [

    ],
    "topic_id": 40,
    "discipline_id": 40,
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
    "updated_at": "2016-10-19T11:44:54.935Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c41cb9a59b75d4f93a728c13c1644ad20a84551371fc5e35e56784f878a010e"
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
      "creator_id": 133,
      "id": 49,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "topic_id": 49,
      "discipline_id": 49,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
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
      "updated_at": "2016-10-19T11:44:55.868Z",
      "shortname": "fu-course-32"
    },
    {
      "creator_id": 133,
      "id": 50,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-33",
      "html_url": "https://goskive.com/course/fu-course-33",
      "slug": "fu-course-33",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "topic_id": 50,
      "discipline_id": 50,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 33",
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
      "chapters_updated_at": "2016-10-19T11:44:56.155Z",
      "updated_at": "2016-10-19T11:44:56.161Z",
      "shortname": "fu-course-33"
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
Authorization: Bearer be9b1722e03decb0f28ae3a30c080ca0ef2ef47be390e0450a5ce61c712a9a9b
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
      "creator_id": 140,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-40",
      "html_url": "https://goskive.com/course/fu-course-40",
      "slug": "fu-course-40",
      "university_id": 49,
      "additional_university_ids": [

      ],
      "topic_id": 57,
      "discipline_id": 57,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 40",
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
      "updated_at": "2016-10-19T11:44:56.635Z",
      "shortname": "fu-course-40"
    },
    {
      "creator_id": 140,
      "id": 58,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 49,
      "additional_university_ids": [

      ],
      "topic_id": 58,
      "discipline_id": 58,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
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
      "chapters_updated_at": "2016-10-19T11:44:56.939Z",
      "updated_at": "2016-10-19T11:44:56.945Z",
      "shortname": "fu-course-41"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be9b1722e03decb0f28ae3a30c080ca0ef2ef47be390e0450a5ce61c712a9a9b"
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
      "creator_id": 138,
      "id": 53,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-36",
      "html_url": "https://goskive.com/course/fu-course-36",
      "slug": "fu-course-36",
      "university_id": 47,
      "additional_university_ids": [

      ],
      "topic_id": 53,
      "discipline_id": 53,
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
      "updated_at": "2016-10-19T11:44:56.353Z",
      "shortname": "fu-course-36"
    },
    {
      "creator_id": 138,
      "id": 54,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-37",
      "html_url": "https://goskive.com/course/fu-course-37",
      "slug": "fu-course-37",
      "university_id": 47,
      "additional_university_ids": [

      ],
      "topic_id": 54,
      "discipline_id": 54,
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
      "updated_at": "2016-10-19T11:44:56.395Z",
      "shortname": "fu-course-37"
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
Authorization: Bearer 61cde7b7843e6e3519574c81148db698fb41405c6be41d341997c343fab5116c
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
      "creator_id": 146,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 50,
      "additional_university_ids": [

      ],
      "topic_id": 61,
      "discipline_id": 61,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 44",
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
      "updated_at": "2016-10-19T11:44:57.187Z",
      "shortname": "fu-course-44"
    },
    {
      "creator_id": 146,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 50,
      "additional_university_ids": [

      ],
      "topic_id": 62,
      "discipline_id": 62,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 45",
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
      "updated_at": "2016-10-19T11:44:57.228Z",
      "shortname": "fu-course-45"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61cde7b7843e6e3519574c81148db698fb41405c6be41d341997c343fab5116c"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer d6e96db1e6aadc4dc3b54b81d5ebd1b86ce4587c6a16df40d8b39a27eb7fb58c
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
  "id": 810,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-19T11:45:45.161Z",
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
	-H "Authorization: Bearer d6e96db1e6aadc4dc3b54b81d5ebd1b86ce4587c6a16df40d8b39a27eb7fb58c"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/853
Content-Type: application/json
Authorization: Bearer f80a7a879e9e6de50bb2e3585a2594e6cf1df1ca774e44747f37167505972672
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
    "id": 853,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 260,
    "fields_of_study": [
      281,
      282
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-19T11:45:47.729Z",
    "updated_at": "2016-10-19T11:45:47.729Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/853" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f80a7a879e9e6de50bb2e3585a2594e6cf1df1ca774e44747f37167505972672"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/855
Content-Type: application/json
Authorization: Bearer 51a5745547ba2d90eb57a7f711a47243fbd83e967f0ae02ac5327725d2e7e2db
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
    "id": 855,
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
    "created_at": "2016-10-19T11:45:47.825Z",
    "updated_at": "2016-10-19T11:45:47.825Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/855" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51a5745547ba2d90eb57a7f711a47243fbd83e967f0ae02ac5327725d2e7e2db"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/16
Content-Type: application/json
Authorization: Bearer 17265c9594bb9e423116d85f6c9b1b67485b6fc0d52794c2ba95d84410542af3
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17265c9594bb9e423116d85f6c9b1b67485b6fc0d52794c2ba95d84410542af3"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/18
Content-Type: application/json
Authorization: Bearer 71875988ecfd2a24b63d6d2cc63c5fe1e77afe43fff5ff3726c692247739bc93
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
    "id": 18,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 129,
    "user_id": 937
  }
}
```



```shell
curl "api.goskive.com/v2/votes/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71875988ecfd2a24b63d6d2cc63c5fe1e77afe43fff5ff3726c692247739bc93"
```
