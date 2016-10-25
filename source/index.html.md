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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a8e31f936a35055bf9b3b8f2503f03a5cfc0e08fc7091c36804c152ac31d1afd","client_secret":"7388ecba2a074f8c15d5543da461e73c139ad929f08c9debeb4b15e1c58ba42d"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a8e31f936a35055bf9b3b8f2503f03a5cfc0e08fc7091c36804c152ac31d1afd","client_secret":"7388ecba2a074f8c15d5543da461e73c139ad929f08c9debeb4b15e1c58ba42d"}' -X POST \
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
Authorization: Basic MGFiYTkzYzdiZmJkOWQwYjBhOWVlMTUzYjEwMmFjZGM1ZTlmYzA2MDYzNTcw
Yjg2MjMzMGYxYTVlOGVmODQyZDpjNWY0YjE2YTdiODEwMzUzNmQ2Mjg0NTEz
ZDBiOGE1MTg2NGJhMjg0MWVmZjEyYjM0YTU1MDM2MTE1N2QwYmU5

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
	-u 0aba93c7bfbd9d0b0a9ee153b102acdc5e9fc06063570b862330f1a5e8ef842d:c5f4b16a7b8103536d6284513d0b8a51864ba2841eff12b34a550361157d0be9
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
{"grant_type":"client_credentials","client_id":"334956fc961c8546f5a4d422b46cf4e4d3d34c0b3423fe6a1c5a9c348d2669f1","client_secret":"94fa6162d789fdf54a329346d1796a7eafab8152819c83b1f5449e9de14b61f6"}
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
  "access_token": "85398d14e6f54673f5c0cde5b24a518779b6ccba3b2964c8ec514cb5a0e61370",
  "token_type": "bearer",
  "created_at": 1477415565
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"334956fc961c8546f5a4d422b46cf4e4d3d34c0b3423fe6a1c5a9c348d2669f1","client_secret":"94fa6162d789fdf54a329346d1796a7eafab8152819c83b1f5449e9de14b61f6"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"c2926d2d8c5d03d4b9fe1f221c3e7361883f6bdcd303c0350c17d7d74d8890e2","client_secret":"e31a75da85bb21cdef1091dec9115ebc6d297dfdb79676069f44581d633805a9"}
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
  "access_token": "b527f5421ab8060baa1602f73631987e03228e2e7d60da92d86779b99e6144ac",
  "token_type": "bearer",
  "created_at": 1477415565
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"c2926d2d8c5d03d4b9fe1f221c3e7361883f6bdcd303c0350c17d7d74d8890e2","client_secret":"e31a75da85bb21cdef1091dec9115ebc6d297dfdb79676069f44581d633805a9"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NGViZWFhYzhjY2Y5NTg0OWU2NmI4Mjc1ZmY4ZDYzZmYzZDFlM2Y3Y2VlMWRj
OTczZWU1OTgyYWQ0NDc1ZGMyMTo1NWY3Y2E3MDMzMGE4NTc4ZDMzMTBjZDEy
YzI3NTVlYTkyM2ZhNjQ2NjkxMzM5MjIxY2I4NDNlMTdlM2VmNWE5

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
  "access_token": "59b95fcef8f31ae6866de0c9204659b34d2d6a94ff030bf76575ea367b8ba9ef",
  "token_type": "bearer",
  "created_at": 1477415565
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 4ebeaac8ccf95849e66b8275ff8d63ff3d1e3f7cee1dc973ee5982ad4475dc21:55f7ca70330a8578d3310cd12c2755ea923fa646691339221cb843e17e3ef5a9
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
Authorization: Bearer 741e4bf7e648862e1c8a9489707729f0fa8fdb091e9bed08697e5f58ef52fa07
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
    "company_id": 36,
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
	-H "Authorization: Bearer 741e4bf7e648862e1c8a9489707729f0fa8fdb091e9bed08697e5f58ef52fa07"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/48/flashcards
Content-Type: application/json
Authorization: Bearer cbef0d51d84f795838612182429a27c98b2c157c86e7bfd657cffa6668bbcccf
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":48,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 14,
    "obfuscated_id": "gbKzjBR_8tw",
    "author_id": 234,
    "chapter_id": 48,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:12:40.486Z",
    "created_at": "2016-10-25T17:12:40.486Z",
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
curl "api.goskive.com/v2/chapters/48/flashcards" -d '{"flashcard":{"chapter_id":48,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbef0d51d84f795838612182429a27c98b2c157c86e7bfd657cffa6668bbcccf"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/49/flashcards
Content-Type: application/json
Authorization: Bearer c14c50347c2cb7c118038424bcfbfe3788ea4ecc5a63dadfa9e151e807b54b87
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 235,
      "chapter_id": 49,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:40.635Z",
      "created_at": "2016-10-25T17:12:40.635Z",
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 235,
      "chapter_id": 49,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:40.675Z",
      "created_at": "2016-10-25T17:12:40.675Z",
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 235,
      "chapter_id": 49,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:12:40.714Z",
      "created_at": "2016-10-25T17:12:40.714Z",
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
curl "api.goskive.com/v2/chapters/49/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c14c50347c2cb7c118038424bcfbfe3788ea4ecc5a63dadfa9e151e807b54b87"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/184/questions
Content-Type: application/json
Authorization: Bearer 991dab45ef309b4762ffaa5da363823fbe8a2c371f44e0b5f283ac331d87513e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 122,
    "obfuscated_id": "cMWZX2w28hY",
    "author_id": 921,
    "chapter_id": 184,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:13:29.974Z",
    "created_at": "2016-10-25T17:13:29.974Z",
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
        "id": 245,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 246,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 247,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 248,
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
curl "api.goskive.com/v2/chapters/184/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 991dab45ef309b4762ffaa5da363823fbe8a2c371f44e0b5f283ac331d87513e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/183/questions
Content-Type: application/json
Authorization: Bearer 65a70bac200825af688dba1be3303ba106f81ac54d3e9d00f325bb6dcdf1f48b
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 121,
    "obfuscated_id": "LQhaXfRg6ZA",
    "author_id": 918,
    "chapter_id": 183,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:13:29.629Z",
    "created_at": "2016-10-25T17:13:29.629Z",
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
        "id": 243,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 244,
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
curl "api.goskive.com/v2/chapters/183/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65a70bac200825af688dba1be3303ba106f81ac54d3e9d00f325bb6dcdf1f48b"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/185/questions
Content-Type: application/json
Authorization: Bearer f2ddb34e5862aada7274642211559f489fe47f3b8dc3f46c793627e4e6446631
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":185,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 123,
    "obfuscated_id": "N9-wuAhut60",
    "author_id": 924,
    "chapter_id": 185,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:13:30.440Z",
    "created_at": "2016-10-25T17:13:30.440Z",
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
        "id": 249,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 250,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/185/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":185,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2ddb34e5862aada7274642211559f489fe47f3b8dc3f46c793627e4e6446631"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/182/questions
Content-Type: application/json
Authorization: Bearer 62df37349403d5a5c7cf1112c1b277808f9cb466efb5e3f6433aa7b1a786ea53
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":182,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 120,
    "obfuscated_id": "vEr9LtFjURM",
    "author_id": 915,
    "chapter_id": 182,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:13:29.239Z",
    "created_at": "2016-10-25T17:13:29.239Z",
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
        "id": 240,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 241,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 242,
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
curl "api.goskive.com/v2/chapters/182/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":182,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62df37349403d5a5c7cf1112c1b277808f9cb466efb5e3f6433aa7b1a786ea53"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/186/questions
Content-Type: application/json
Authorization: Bearer d1d2030fdee5cfe28e8cd308ccc3260e370ba864942d4a4525a64760b2655359
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
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 927,
      "chapter_id": 186,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:13:30.832Z",
      "created_at": "2016-10-25T17:13:30.724Z",
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
      "author_id": 928,
      "chapter_id": 186,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:13:31.011Z",
      "created_at": "2016-10-25T17:13:30.899Z",
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
      "author_id": 929,
      "chapter_id": 186,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T17:13:31.194Z",
      "created_at": "2016-10-25T17:13:31.080Z",
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
```



```shell
curl "api.goskive.com/v2/chapters/186/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1d2030fdee5cfe28e8cd308ccc3260e370ba864942d4a4525a64760b2655359"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/179
Content-Type: application/json
Authorization: Bearer 9e73f19306ed155089a3db6e46f1b0df70ffb93c911001eef6c9e07c5aa87304
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
curl "api.goskive.com/v2/chapters/179" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e73f19306ed155089a3db6e46f1b0df70ffb93c911001eef6c9e07c5aa87304"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/180
Content-Type: application/json
Authorization: Bearer 35d81249abc5f9ee949bea5d117b1b34059dc732100dcb3f109dc445a55530bf
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
curl "api.goskive.com/v2/chapters/180" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35d81249abc5f9ee949bea5d117b1b34059dc732100dcb3f109dc445a55530bf"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/175
Content-Type: application/json
Authorization: Bearer d1eb6d653ebd5b1bac812e2cd87011f8e8a7fb573c345fd228cab6d4e50937f1
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
curl "api.goskive.com/v2/chapters/175" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1eb6d653ebd5b1bac812e2cd87011f8e8a7fb573c345fd228cab6d4e50937f1"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/178
Content-Type: application/json
Authorization: Bearer 0143140fc55a71ca06c33906335852cac4521439d96f86896f1ffe3f662be97e
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/178" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0143140fc55a71ca06c33906335852cac4521439d96f86896f1ffe3f662be97e"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/177
Content-Type: application/json
Authorization: Bearer 487080b130865e4906ed857653c62b064b3f74ec2093eb29325bec3d5066338a
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
    "id": 177,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T17:13:28.179Z",
    "course_id": 291,
    "author_id": 895,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-25T17:13:27.682Z",
    "questions_updated_at": "2016-10-25T17:13:27.682Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 899,
        "chapter_id": 177,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:28.163Z",
        "created_at": "2016-10-25T17:13:28.163Z",
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
        "id": 117,
        "obfuscated_id": "BsA8mEPn8aM",
        "author_id": 897,
        "chapter_id": 177,
        "position": 108,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:28.064Z",
        "created_at": "2016-10-25T17:13:27.952Z",
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
            "id": 234,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 235,
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
curl "api.goskive.com/v2/chapters/177" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 487080b130865e4906ed857653c62b064b3f74ec2093eb29325bec3d5066338a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/174
Content-Type: application/json
Authorization: Bearer 039e1c4729312bc51fc333715dcaa8af544b033ae3e2e5f5b15591b3a13d4de1
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
    "id": 174,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T17:13:26.957Z",
    "course_id": 288,
    "author_id": 883,
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
curl "api.goskive.com/v2/chapters/174" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 039e1c4729312bc51fc333715dcaa8af544b033ae3e2e5f5b15591b3a13d4de1"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/4/replies
Content-Type: application/json
Authorization: Bearer 8d272c308faba9cd3fb6b9bfe23c584195c0d4b743bfe5a6c95effa53052aab1
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
    "author_id": 110,
    "reply_to_id": 4,
    "created_at": "2016-10-25T17:12:27.905Z",
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
	-H "Authorization: Bearer 8d272c308faba9cd3fb6b9bfe23c584195c0d4b743bfe5a6c95effa53052aab1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 520411accecd82cbb86e56c4a98d1c1085b280eed0ad74d851772023b9daf544
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
	-H "Authorization: Bearer 520411accecd82cbb86e56c4a98d1c1085b280eed0ad74d851772023b9daf544"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/50
Content-Type: application/json
Authorization: Bearer 1789fe761aeb20bc56ea3305276964867e08b4b9daa24e8728c40bbbc6a80d33
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
curl "api.goskive.com/v2/comments/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1789fe761aeb20bc56ea3305276964867e08b4b9daa24e8728c40bbbc6a80d33"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/53/republish
Content-Type: application/json
Authorization: Bearer 19eee591685071b7deeb1c714f89f2986922768d40e95ea4605e77c09cf10c72
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
curl "api.goskive.com/v2/comments/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19eee591685071b7deeb1c714f89f2986922768d40e95ea4605e77c09cf10c72"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 3f9520bd86631fb8824176aa19a73613a9618458502bdcbaa415e4f373122035
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f9520bd86631fb8824176aa19a73613a9618458502bdcbaa415e4f373122035"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/54/report
Content-Type: application/json
Authorization: Bearer 5eda765b45bc38f94188e5d6f2dc59f3569f148ac709a2a9c4b621a9cc669534
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5eda765b45bc38f94188e5d6f2dc59f3569f148ac709a2a9c4b621a9cc669534"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/32
Content-Type: application/json
Authorization: Bearer 566177ba6c57aa48b2c8340825c3df3d9668ffcd03abc20f32ff0f90a3d03086
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
    "id": 32,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/4827d71e510ab6acd29eb9520c31ac72b53161f6.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-25T17:13:23.156Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/32" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 566177ba6c57aa48b2c8340825c3df3d9668ffcd03abc20f32ff0f90a3d03086"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 1cd9a6d96c684a888de95c8e7cf171f2f635e94a9f2af12a1a50346b42c32c4a
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
      "id": 33,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T17:13:23.264Z"
    },
    {
      "id": 34,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T17:13:23.268Z"
    },
    {
      "id": 35,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T17:13:23.272Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cd9a6d96c684a888de95c8e7cf171f2f635e94a9f2af12a1a50346b42c32c4a"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/39/company_profiles
Content-Type: application/json
Authorization: Bearer cc9c7d751122fc533bc31a861efb746e148c32a940f96eab109bc830be77d15c
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
	-H "Authorization: Bearer cc9c7d751122fc533bc31a861efb746e148c32a940f96eab109bc830be77d15c"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer bac2f8829cffe172c95aa66361fcd4949c6f147fd25d92e6abfb58e80e70f7a2
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
	-H "Authorization: Bearer bac2f8829cffe172c95aa66361fcd4949c6f147fd25d92e6abfb58e80e70f7a2"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer b72d10e06660b8e6ba1a2f2a64ae29835e8d871949247d61c80d53fd6c0de9d8
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
	-H "Authorization: Bearer b72d10e06660b8e6ba1a2f2a64ae29835e8d871949247d61c80d53fd6c0de9d8"
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
Authorization: Bearer 609563e4fb12f21fd41da33f8c087dacea37900d09ce89fc671cffed8fca3e91
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
	-H "Authorization: Bearer 609563e4fb12f21fd41da33f8c087dacea37900d09ce89fc671cffed8fca3e91"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6963d8001b2e8b3cb49e580057d22bfe5fd40ecfa6a447db23b91ee3c0903241
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
    "id": 140,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T17:13:02.143Z",
    "course_id": 158,
    "author_id": 593,
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
	-H "Authorization: Bearer 6963d8001b2e8b3cb49e580057d22bfe5fd40ecfa6a447db23b91ee3c0903241"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f2530592db416d642a645f7f9597ddfc034a03434443338edd6aa714029d4f83
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
      "id": 121,
      "title": "Clever Chapter Title 118",
      "position": 1,
      "updated_at": "2016-10-25T17:12:59.882Z",
      "course_id": 147,
      "author_id": 550,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 122,
      "title": "Clever Chapter Title 119",
      "position": 2,
      "updated_at": "2016-10-25T17:12:59.905Z",
      "course_id": 147,
      "author_id": 551,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 123,
      "title": "Clever Chapter Title 120",
      "position": 3,
      "updated_at": "2016-10-25T17:13:00.144Z",
      "course_id": 147,
      "author_id": 552,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T17:12:59.807Z",
      "questions_updated_at": "2016-10-25T17:12:59.807Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2530592db416d642a645f7f9597ddfc034a03434443338edd6aa714029d4f83"
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
      "id": 127,
      "title": "Clever Chapter Title 124",
      "position": 1,
      "updated_at": "2016-10-25T17:13:00.582Z",
      "course_id": 150,
      "author_id": 564,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 128,
      "title": "Clever Chapter Title 125",
      "position": 2,
      "updated_at": "2016-10-25T17:13:00.606Z",
      "course_id": 150,
      "author_id": 565,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 129,
      "title": "Clever Chapter Title 126",
      "position": 3,
      "updated_at": "2016-10-25T17:13:00.843Z",
      "course_id": 150,
      "author_id": 566,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T17:13:00.509Z",
      "questions_updated_at": "2016-10-25T17:13:00.509Z",
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
Authorization: Bearer 45cda07dacdae02a33515ebf24c0243e9b0925d407508a1602d4ebef0f16cc64
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
      "id": 124,
      "title": "Clever Chapter Title 121",
      "position": 1,
      "updated_at": "2016-10-25T17:13:00.390Z",
      "course_id": 149,
      "author_id": 559,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 125,
      "title": "Clever Chapter Title 122",
      "position": 2,
      "updated_at": "2016-10-25T17:13:00.413Z",
      "course_id": 149,
      "author_id": 560,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 126,
      "title": "Clever Chapter Title 123",
      "position": 3,
      "updated_at": "2016-10-25T17:13:00.435Z",
      "course_id": 149,
      "author_id": 561,
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
	-H "Authorization: Bearer 45cda07dacdae02a33515ebf24c0243e9b0925d407508a1602d4ebef0f16cc64"
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
      "id": 130,
      "title": "Clever Chapter Title 127",
      "position": 1,
      "updated_at": "2016-10-25T17:13:00.954Z",
      "course_id": 151,
      "author_id": 570,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 131,
      "title": "Clever Chapter Title 128",
      "position": 2,
      "updated_at": "2016-10-25T17:13:00.976Z",
      "course_id": 151,
      "author_id": 571,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 129",
      "position": 3,
      "updated_at": "2016-10-25T17:13:00.999Z",
      "course_id": 151,
      "author_id": 572,
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
Authorization: Bearer 840aa6a3f899f0c99dd26e64056543e3dde76f96d15c85b0b092fe1884274917
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
    "course_id": 2,
    "user_id": 4,
    "updated_at": "2016-10-25T17:12:19.931Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 840aa6a3f899f0c99dd26e64056543e3dde76f96d15c85b0b092fe1884274917"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 57fed4dd73ed742f5f495dff5b9718ca401ffc653ce81e28702aa510e2642094
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
      "course_id": 5,
      "user_id": 12,
      "updated_at": "2016-10-25T17:12:20.267Z"
    },
    {
      "id": 6,
      "course_id": 5,
      "user_id": 13,
      "updated_at": "2016-10-25T17:12:20.281Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57fed4dd73ed742f5f495dff5b9718ca401ffc653ce81e28702aa510e2642094"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/191/files
Content-Type: application/json
Authorization: Bearer 0478e83984dd4bd92477b48825c6e5c80c622d237755c0e419cd4cffd104d191
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
        "id": 673,
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
        "created_at": "2016-10-25T17:13:12.031Z",
        "updated_at": "2016-10-25T17:13:12.031Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T17:13:12.041Z",
      "updated_at": "2016-10-25T17:13:12.041Z",
      "course_id": 191,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 674,
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
        "created_at": "2016-10-25T17:13:12.047Z",
        "updated_at": "2016-10-25T17:13:12.047Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T17:13:12.056Z",
      "updated_at": "2016-10-25T17:13:12.056Z",
      "course_id": 191,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 675,
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
        "created_at": "2016-10-25T17:13:12.062Z",
        "updated_at": "2016-10-25T17:13:12.062Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T17:13:12.070Z",
      "updated_at": "2016-10-25T17:13:12.070Z",
      "course_id": 191,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/191/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0478e83984dd4bd92477b48825c6e5c80c622d237755c0e419cd4cffd104d191"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/192/files
Content-Type: application/json
Authorization: Bearer a37ea3bff938132c97fbeb5bee71e6d91a3dadfeae37ade75715d62eb79f0d37
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
      "id": 678,
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
      "created_at": "2016-10-25T17:13:12.186Z",
      "updated_at": "2016-10-25T17:13:12.186Z"
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
    "created_at": "2016-10-25T17:13:12.213Z",
    "updated_at": "2016-10-25T17:13:12.213Z",
    "course_id": 192,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/192/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a37ea3bff938132c97fbeb5bee71e6d91a3dadfeae37ade75715d62eb79f0d37"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/189/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer b30b7c27d82e8750a5da53ac9875c14cb3bdae678e31ef887856e61be1299f98
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
    "key": "cache/7dafa7e191e4c3f01833c3b3ca0f7449.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxODoxMzoxMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzdkYWZhN2UxOTFlNGMzZjAxODMzYzNiM2NhMGY3NDQ5LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI1VDE3MTMxMVoifV19",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T171311Z",
    "x-amz-signature": "ad7f298032b73e9d44665c0b3870d4af2611890b0205f13f38af919774dd53f0"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/189/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b30b7c27d82e8750a5da53ac9875c14cb3bdae678e31ef887856e61be1299f98"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer f826da76a5b2f1c7ed11f5a4d2450228539d4a2976c781c8bb1b14aaab48b685
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
	-H "Authorization: Bearer f826da76a5b2f1c7ed11f5a4d2450228539d4a2976c781c8bb1b14aaab48b685"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e9bbb4853014275fc9f045ad8d4e6455ecf5ccd2b084e6d8be83f1cb1d0bc36e
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
	-H "Authorization: Bearer e9bbb4853014275fc9f045ad8d4e6455ecf5ccd2b084e6d8be83f1cb1d0bc36e"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b4bed6cda36b030ad0392db0cde4426b9e39108aee800235b5e5df269ba9800f
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
	-H "Authorization: Bearer b4bed6cda36b030ad0392db0cde4426b9e39108aee800235b5e5df269ba9800f"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 41ea1fa0993a71c856b1c7b59a7dd70eb6633367971bbe940fb7a3af84535dde
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
	-H "Authorization: Bearer 41ea1fa0993a71c856b1c7b59a7dd70eb6633367971bbe940fb7a3af84535dde"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 05fe647b7c2c8714c369e89313418381313e5348601daa9810438e02960edfe7
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
	-H "Authorization: Bearer 05fe647b7c2c8714c369e89313418381313e5348601daa9810438e02960edfe7"
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
    "creator_id": 613,
    "id": 166,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 173,
    "additional_university_ids": [

    ],
    "topic_id": 168,
    "discipline_id": 168,
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
    "chapters_updated_at": "2016-10-25T17:13:05.648Z",
    "updated_at": "2016-10-25T17:13:07.014Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 146,
        "title": "Clever Chapter Title 140",
        "position": 1,
        "updated_at": "2016-10-25T17:13:06.970Z",
        "course_id": 166,
        "author_id": 613,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T17:13:05.648Z",
        "questions_updated_at": "2016-10-25T17:13:05.648Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 147,
        "title": "Clever Chapter Title 141",
        "position": 2,
        "updated_at": "2016-10-25T17:13:07.007Z",
        "course_id": 166,
        "author_id": 613,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T17:13:05.648Z",
        "questions_updated_at": "2016-10-25T17:13:05.648Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 613,
        "chapter_id": 146,
        "position": 75,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:05.848Z",
        "created_at": "2016-10-25T17:13:05.738Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 613,
        "chapter_id": 147,
        "position": 77,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:06.211Z",
        "created_at": "2016-10-25T17:13:06.094Z",
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
Authorization: Bearer 0e35b02c2aa5f33871484e2760f0021b44ddbe94f0525e0246ad4189594866ce
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
    "creator_id": 618,
    "id": 167,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 174,
    "additional_university_ids": [

    ],
    "topic_id": 169,
    "discipline_id": 169,
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
    "chapters_updated_at": "2016-10-25T17:13:07.067Z",
    "updated_at": "2016-10-25T17:13:08.484Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 148,
        "title": "Clever Chapter Title 142",
        "position": 1,
        "updated_at": "2016-10-25T17:13:08.410Z",
        "course_id": 167,
        "author_id": 618,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T17:13:07.067Z",
        "questions_updated_at": "2016-10-25T17:13:07.067Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 149,
        "title": "Clever Chapter Title 143",
        "position": 2,
        "updated_at": "2016-10-25T17:13:08.476Z",
        "course_id": 167,
        "author_id": 618,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T17:13:07.067Z",
        "questions_updated_at": "2016-10-25T17:13:07.067Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 619,
        "chapter_id": 148,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:08.253Z",
        "created_at": "2016-10-25T17:13:08.253Z",
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
        "author_id": 619,
        "chapter_id": 149,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:08.322Z",
        "created_at": "2016-10-25T17:13:08.322Z",
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
        "author_id": 619,
        "chapter_id": 148,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:08.292Z",
        "created_at": "2016-10-25T17:13:08.292Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 619,
        "chapter_id": 149,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:08.360Z",
        "created_at": "2016-10-25T17:13:08.360Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 619,
        "chapter_id": 148,
        "position": 81,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:07.272Z",
        "created_at": "2016-10-25T17:13:07.163Z",
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
            "id": 180,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 181,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 619,
        "chapter_id": 148,
        "position": 82,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:07.437Z",
        "created_at": "2016-10-25T17:13:07.332Z",
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
            "id": 182,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 183,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 619,
        "chapter_id": 149,
        "position": 83,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:07.633Z",
        "created_at": "2016-10-25T17:13:07.517Z",
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
            "id": 184,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 185,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 619,
        "chapter_id": 149,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T17:13:07.808Z",
        "created_at": "2016-10-25T17:13:07.696Z",
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
            "id": 186,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 187,
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
	-H "Authorization: Bearer 0e35b02c2aa5f33871484e2760f0021b44ddbe94f0525e0246ad4189594866ce"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/181/pin
Content-Type: application/json
Authorization: Bearer e35a154e779cdb079b5b29347d4fc0dd242720d6c9c8063f9d4f68d5f3e7efd6
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/181/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e35a154e779cdb079b5b29347d4fc0dd242720d6c9c8063f9d4f68d5f3e7efd6"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/182/pin
Content-Type: application/json
Authorization: Bearer b19618dc450367fbd49a457f4722f270f695757ea64c11dd87ae447ed294a2cc
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/182/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b19618dc450367fbd49a457f4722f270f695757ea64c11dd87ae447ed294a2cc"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c8c46443e5860b85bc14f38ac63c473699b102525127b5721408d2075c5fa32c
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
    "creator_id": 628,
    "id": 170,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 177,
    "additional_university_ids": [

    ],
    "topic_id": 172,
    "discipline_id": 172,
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
    "updated_at": "2016-10-25T17:13:08.984Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8c46443e5860b85bc14f38ac63c473699b102525127b5721408d2075c5fa32c"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 376f910469d4962f17cc5089b03ce09ca3066d92027e20c792719dff07496336
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
    "id": 679,
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
    "created_at": "2016-10-25T17:13:12.267Z",
    "updated_at": "2016-10-25T17:13:12.267Z",
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
	-H "Authorization: Bearer 376f910469d4962f17cc5089b03ce09ca3066d92027e20c792719dff07496336"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 78d5a6513bac45e546e073653e3ca832aa64ad4b8180221f87322c27547465f0
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[195]}
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
    "id": 680,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      195
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T17:13:12.349Z",
    "updated_at": "2016-10-25T17:13:12.384Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[195]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78d5a6513bac45e546e073653e3ca832aa64ad4b8180221f87322c27547465f0"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d897995f2c5bc60919f2b7a21dfc1d7ab721215c997ca8ac57c9a0b8deefd073
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
    "id": 681,
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
    "created_at": "2016-10-25T17:13:12.404Z",
    "updated_at": "2016-10-25T17:13:12.404Z",
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
	-H "Authorization: Bearer d897995f2c5bc60919f2b7a21dfc1d7ab721215c997ca8ac57c9a0b8deefd073"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 311ce72e5bb4d145b857674b8df6240ac209cce47a611d67a671b348d270669e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[198]}
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
    "id": 683,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      198
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T17:13:12.566Z",
    "updated_at": "2016-10-25T17:13:12.566Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[198]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 311ce72e5bb4d145b857674b8df6240ac209cce47a611d67a671b348d270669e"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b6296e52694cbb3a9c310c061f168611ecc2d6d7772b63cd890bc1e2d555ba4f
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

199
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
    "id": 684,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0337e583b7f48832cd7f13ab87cf8456e933190f.jpg",
    "university_id": null,
    "fields_of_study": [
      199
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T17:13:12.633Z",
    "updated_at": "2016-10-25T17:13:12.880Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/e856647869588d3f4d73ec83287940c3598436d9.jpg",
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

199
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b6296e52694cbb3a9c310c061f168611ecc2d6d7772b63cd890bc1e2d555ba4f"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 8515b7e68962d27edc2b8bc8b887f9fe676ece3735e9e6b9bccdc1d30e48fad1
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
      "id": 5,
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8515b7e68962d27edc2b8bc8b887f9fe676ece3735e9e6b9bccdc1d30e48fad1"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 0192aa6ffda9f5b848c68dd7e1385a5566f47923e41748f070a5043c25c6a518
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
      "company_id": 25,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 26,
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
	-H "Authorization: Bearer 0192aa6ffda9f5b848c68dd7e1385a5566f47923e41748f070a5043c25c6a518"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 239d97bda8c6873f84d0331a22cd5b7f2d16820aa7a8fabfb2f0dcc34ae9aba8
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
      "company_id": 21,
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
	-H "Authorization: Bearer 239d97bda8c6873f84d0331a22cd5b7f2d16820aa7a8fabfb2f0dcc34ae9aba8"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 2ede407b5fa52c61b8080ae8422cd9f414b490dab0385d8d229c44c754554749
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
      "creator_id": 472,
      "id": 122,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-103",
      "html_url": "https://goskive.com/course/mit-course-103",
      "slug": "mit-course-103",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "topic_id": 124,
      "discipline_id": 124,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
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
      "updated_at": "2016-10-25T17:12:54.609Z",
      "shortname": "mit-course-103"
    },
    {
      "creator_id": 473,
      "id": 123,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-104",
      "html_url": "https://goskive.com/course/mit-course-104",
      "slug": "mit-course-104",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "topic_id": 125,
      "discipline_id": 125,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
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
      "updated_at": "2016-10-25T17:12:54.684Z",
      "shortname": "mit-course-104"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ede407b5fa52c61b8080ae8422cd9f414b490dab0385d8d229c44c754554749"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer ecc6382e6ddc29d6f1721b7dda9ee59755bba85fc99857bdfaad57fecb62c336
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
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T17:12:26.919Z"
      },
      "created_at": "2016-10-25T17:12:26.923Z",
      "updated_at": "2016-10-25T17:12:26.923Z",
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
        "name": "Fake Company Name 19",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T17:12:26.930Z"
      },
      "created_at": "2016-10-25T17:12:26.933Z",
      "updated_at": "2016-10-25T17:12:26.933Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecc6382e6ddc29d6f1721b7dda9ee59755bba85fc99857bdfaad57fecb62c336"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 651066f403621e6a3dd9c70210adc5609f07531b4946c26662a016aa0da1a8ed
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T17:12:26.665Z"
      },
      "created_at": "2016-10-25T17:12:26.670Z",
      "updated_at": "2016-10-25T17:12:26.670Z",
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T17:12:26.682Z"
      },
      "created_at": "2016-10-25T17:12:26.685Z",
      "updated_at": "2016-10-25T17:12:26.685Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 651066f403621e6a3dd9c70210adc5609f07531b4946c26662a016aa0da1a8ed"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 925f757ddc454d736863aca5240d0d2a42f6125e40edc2374a92da634d69a69e
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
      "id": 8,
      "created_at": "2016-10-25T17:12:38.069Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-10-25T17:12:38.168Z",
      "author_id": "205",
      "thread_subject_id": "55",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 9,
      "created_at": "2016-10-25T17:12:38.157Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 8,
      "updated_at": "2016-10-25T17:12:38.171Z",
      "author_id": "208",
      "thread_subject_id": "56",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-10-25T17:12:38.561Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-25T17:12:38.561Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-10-25T17:12:38.942Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-10-25T17:12:38.942Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 12,
      "created_at": "2016-10-25T17:12:39.342Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-10-25T17:12:39.342Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 13,
      "created_at": "2016-10-25T17:12:39.649Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 40,
      "updated_at": "2016-10-25T17:12:39.649Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-10-25T17:12:39.958Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 41,
      "updated_at": "2016-10-25T17:12:39.958Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-10-25T17:12:40.271Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 42,
      "updated_at": "2016-10-25T17:12:40.271Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 925f757ddc454d736863aca5240d0d2a42f6125e40edc2374a92da634d69a69e"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/7
Content-Type: application/json
Authorization: Bearer 90d21b6adff9fa2aa75fb1a51d427a202178d64c968a06230131a40c44b772ff
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-25T17:02:37.000Z"}}
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
    "id": 7,
    "created_at": "2016-10-25T17:12:37.909Z",
    "read_at": "2016-10-25T17:02:37.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 6,
    "updated_at": "2016-10-25T17:12:37.965Z",
    "author_id": "201",
    "thread_subject_id": "54",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/7" -d '{"notification":{"read_at":"2016-10-25T17:02:37.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90d21b6adff9fa2aa75fb1a51d427a202178d64c968a06230131a40c44b772ff"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b6775b9cbe0b75f4da76ec70aac247d9c851ebc08a61c2100bd90ab37b7f2d5e
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
      "course_id": 183,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T17:13:10.888Z",
      "course_published": true,
      "updated_at": "2016-10-25T17:13:10.882Z"
    },
    {
      "id": 5,
      "course_id": 184,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T17:13:10.964Z",
      "course_published": true,
      "updated_at": "2016-10-25T17:13:10.957Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6775b9cbe0b75f4da76ec70aac247d9c851ebc08a61c2100bd90ab37b7f2d5e"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer eeddb51ca6a728342368d274d03fad46a207e1c12db7e937db605dc66ad072d4
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
    "course_id": 187,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T17:13:11.349Z",
    "course_published": true,
    "updated_at": "2016-10-25T17:13:11.342Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eeddb51ca6a728342368d274d03fad46a207e1c12db7e937db605dc66ad072d4"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 4d27c980abc38b16c9ab645c644fd211d2c94200cc4441baa8ac7ad1467f9343
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
    "course_id": 188,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-25T17:13:11.536Z",
    "course_published": true,
    "updated_at": "2016-10-25T17:13:11.526Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d27c980abc38b16c9ab645c644fd211d2c94200cc4441baa8ac7ad1467f9343"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 5d391c00908f9a7839f67b666de8b732d50eb3aef3a415f64bc835731498aff1
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
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 65,
      "user_id": 499
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 66,
      "user_id": 499
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 67,
      "user_id": 499
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 68,
      "user_id": 499
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d391c00908f9a7839f67b666de8b732d50eb3aef3a415f64bc835731498aff1"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/291
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
    "id": 291,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 289,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 291
      },
      {
        "id": 290,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 291
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/291" -X GET \
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
      "id": 289,
      "name": "Profit-focused secondary methodology",
      "name_translations": {
        "en": "Profit-focused secondary methodology"
      }
    },
    {
      "id": 290,
      "name": "Versatile intangible internet solution",
      "name_translations": {
        "en": "Versatile intangible internet solution"
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
PATCH /v2/feedbacks/35/close
Content-Type: application/json
Authorization: Bearer 0d884b66fefa557f50c455761c2e1a71c700ed80f6f75cd54ccc19e9346b87ac
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
    "id": 35,
    "user_id": 452,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-25T17:12:53.266Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/35/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d884b66fefa557f50c455761c2e1a71c700ed80f6f75cd54ccc19e9346b87ac"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/32/fix
Content-Type: application/json
Authorization: Bearer 719a724aa11f8dbf1c16f0fd8163a6b49e92fc937b2feac9e9266967400f8e6e
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
    "id": 32,
    "user_id": 437,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-25T17:12:52.271Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/32/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 719a724aa11f8dbf1c16f0fd8163a6b49e92fc937b2feac9e9266967400f8e6e"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer 832a69778370382656dcdcf6b842131145fcd61659c7b830f6edcc9eccd05392
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
    "user_id": 415,
    "feedbackable_id": 42,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T17:12:51.461Z",
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
	-H "Authorization: Bearer 832a69778370382656dcdcf6b842131145fcd61659c7b830f6edcc9eccd05392"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/30/fix
Content-Type: application/json
Authorization: Bearer 5af5bd191e9bbfacb7cec8a38f36d7bfd61aae37b4f91b331bb62bfd63b5e99b
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
curl "api.goskive.com/v2/feedbacks/30/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5af5bd191e9bbfacb7cec8a38f36d7bfd61aae37b4f91b331bb62bfd63b5e99b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/31/fix
Content-Type: application/json
Authorization: Bearer a6eae7c993c9348a9cdac27aaf3e154243d29b77b09eba50536304090c03aa7c
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
curl "api.goskive.com/v2/feedbacks/31/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6eae7c993c9348a9cdac27aaf3e154243d29b77b09eba50536304090c03aa7c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/36/close
Content-Type: application/json
Authorization: Bearer 96e46b2d795d53d04e075da62a899d981594cb3601362fdfc7c180674a80468f
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
curl "api.goskive.com/v2/feedbacks/36/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96e46b2d795d53d04e075da62a899d981594cb3601362fdfc7c180674a80468f"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/29
Content-Type: application/json
Authorization: Bearer ad602fe63e6107347a26de64ad41863751faf7cb7c0c3ba7cafb4496d4b5afe7
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
    "user_id": 420,
    "feedbackable_id": 43,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T17:12:51.718Z",
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
	-H "Authorization: Bearer ad602fe63e6107347a26de64ad41863751faf7cb7c0c3ba7cafb4496d4b5afe7"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 842b911171af482a7ba593d921159d4e5b0e23edab1c27ff6af354cdf61b5d0c
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
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 842b911171af482a7ba593d921159d4e5b0e23edab1c27ff6af354cdf61b5d0c"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer c546a5c3fa4bf21d8489a7a46b62c4e1dff60a614ee44d75ece1b418997d1f8c
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
	-H "Authorization: Bearer c546a5c3fa4bf21d8489a7a46b62c4e1dff60a614ee44d75ece1b418997d1f8c"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/3
Content-Type: application/json
Authorization: Bearer 3143961af42d4bea7b9504d6207c13ded81c6cf071adb0e702cbfeaa0c138c89
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/0e249efa5c7f68a4059e6f1a267c6065.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T171254Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=13a36a53a8ac65eb92512cf50a9d01c2b2da2f16124e3b60801be354a5482452",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3143961af42d4bea7b9504d6207c13ded81c6cf071adb0e702cbfeaa0c138c89"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/5/preview
Content-Type: application/json
Authorization: Bearer 1cd889d07efc89f05141398191af6591d7f8d368274a1c6ee267083c494c1a49
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/3f0cb76c324e7fde1ca35dc96a270f10.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T171255Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f93952e76b42ff3a538466e1c7b3bd668c12ea08258c9776e65cc91d87c52bff",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/5/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cd889d07efc89f05141398191af6591d7f8d368274a1c6ee267083c494c1a49"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 3d0a630164bb56e882060caa7210c6634a60cf06e1c3814f0e3d9d5afd396cec
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
    "id": 7,
    "uploader": {
      "id": 485,
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
      "created_at": "2016-10-25T17:12:55.507Z",
      "updated_at": "2016-10-25T17:12:55.507Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T17:12:55.578Z",
    "updated_at": "2016-10-25T17:12:55.578Z",
    "course_id": 128,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d0a630164bb56e882060caa7210c6634a60cf06e1c3814f0e3d9d5afd396cec"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer cd44893069790ee4b0f409ce347dbe4dde53ba68cbd140606267702f7c71a068
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
      "creator_id": 78,
      "id": 23,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 23,
      "additional_university_ids": [

      ],
      "topic_id": 23,
      "discipline_id": 23,
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
      "chapters_updated_at": "2016-10-25T17:12:24.212Z",
      "updated_at": "2016-10-25T17:12:25.773Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 83,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-62b5da81-4003-4452-b379-2d4180a879ab",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-62b5da81-4003-4452-b379-2d4180a879ab",
      "slug": "mit-the-great-british-bake-off-62b5da81-4003-4452-b379-2d4180a879ab",
      "university_id": 24,
      "additional_university_ids": [

      ],
      "topic_id": 24,
      "discipline_id": 24,
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
      "chapters_updated_at": "2016-10-25T17:12:24.212Z",
      "updated_at": "2016-10-25T17:12:26.303Z",
      "shortname": "mit-the-great-british-bake-off-62b5da81-4003-4452-b379-2d4180a879ab"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer cd44893069790ee4b0f409ce347dbe4dde53ba68cbd140606267702f7c71a068"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/4/report
Content-Type: application/json
Authorization: Bearer d6045d85145847aa1cd89e670c2b4019a51c641d0f43747bf7c1cc80ea37f202
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6045d85145847aa1cd89e670c2b4019a51c641d0f43747bf7c1cc80ea37f202"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/56/comments
Content-Type: application/json
Authorization: Bearer 27035e1887162b8d3d0979fc80d1a8f7b3acfde4848258be5f3df33c4d179ccb
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
    "id": 12,
    "author_id": 533,
    "reply_to_id": null,
    "created_at": "2016-10-25T17:12:58.837Z",
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
curl "api.goskive.com/v2/flashcards/56/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27035e1887162b8d3d0979fc80d1a8f7b3acfde4848258be5f3df33c4d179ccb"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/58/comments
Content-Type: application/json
Authorization: Bearer 6ca6bc4995679b3525e012ddf12cd23650ab09345e55d89bb813b29d746877d0
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
    "id": 13,
    "author_id": 539,
    "reply_to_id": null,
    "created_at": "2016-10-25T17:12:59.334Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 539,
      "feedbackable_id": 58,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:59.331Z",
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
curl "api.goskive.com/v2/flashcards/58/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ca6bc4995679b3525e012ddf12cd23650ab09345e55d89bb813b29d746877d0"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer 0828737b60b89826bafd6507909b6ec3e2828283309e3d0009ceb048867f69ca
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
      "id": 11,
      "author_id": 532,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:12:58.637Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 531,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:12:58.622Z",
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
curl "api.goskive.com/v2/flashcards/55/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0828737b60b89826bafd6507909b6ec3e2828283309e3d0009ceb048867f69ca"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/57/comments
Content-Type: application/json
Authorization: Bearer 669d9389467af75e9cbe3d501c17d218a752c55049ea548f068646d0f9d0ac28
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
curl "api.goskive.com/v2/flashcards/57/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 669d9389467af75e9cbe3d501c17d218a752c55049ea548f068646d0f9d0ac28"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/2/feedbacks
Content-Type: application/json
Authorization: Bearer 5db7e8d1a11337bf28b897000e59b44e4392d75e5ec91f837f761b9ac171b1b0
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
    "id": 2,
    "user_id": 32,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T17:12:22.540Z",
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
curl "api.goskive.com/v2/flashcards/2/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5db7e8d1a11337bf28b897000e59b44e4392d75e5ec91f837f761b9ac171b1b0"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/3/feedbacks
Content-Type: application/json
Authorization: Bearer d61dc97fae4d66cea3503519f0ff7bc18871849491b8ec702e04e764e932ffb5
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
      "id": 4,
      "user_id": 39,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:22.887Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 38,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:12:22.874Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d61dc97fae4d66cea3503519f0ff7bc18871849491b8ec702e04e764e932ffb5"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/51/votes
Content-Type: application/json
Authorization: Bearer 2b9952fb6ddfe5d213baa8a8aa2401e13c65cab4c5de36ea00ae3aebe0a6d13e
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
      "id": 14,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 51,
      "user_id": 518
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 51,
      "user_id": 517
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 51,
      "user_id": 516
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/51/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b9952fb6ddfe5d213baa8a8aa2401e13c65cab4c5de36ea00ae3aebe0a6d13e"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/39/republish
Content-Type: application/json
Authorization: Bearer f6df0589c5798af84bbf561411f249bbcd2b5e9ff381328b3d781216df8fc2b4
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
curl "api.goskive.com/v2/flashcards/39/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6df0589c5798af84bbf561411f249bbcd2b5e9ff381328b3d781216df8fc2b4"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/bookmark
Content-Type: application/json
Authorization: Bearer 494881eaa8e37c937ae1b6d0b8e27730d48007fa3c2c7dfd78de0a8077d4d3b7
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
	-H "Authorization: Bearer 494881eaa8e37c937ae1b6d0b8e27730d48007fa3c2c7dfd78de0a8077d4d3b7"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/37
Content-Type: application/json
Authorization: Bearer f3cdd96fd15a943dc196cdeff7c1cfe477ae20e19e277443c6e52ad977a8cfd8
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3cdd96fd15a943dc196cdeff7c1cfe477ae20e19e277443c6e52ad977a8cfd8"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/downvote
Content-Type: application/json
Authorization: Bearer 33b83781ee3ebaba29bbc61d955f1455763a85f64d9ad9cb3da5953bcd2e27e4
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
	-H "Authorization: Bearer 33b83781ee3ebaba29bbc61d955f1455763a85f64d9ad9cb3da5953bcd2e27e4"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/36
Content-Type: application/json
Authorization: Bearer 3aa38f5a9c6a218cf14bf0ef992ca9aae12bcc6415deaf01198e3f0458a79bc8
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
    "id": 36,
    "obfuscated_id": "01Tx8eTrCOA",
    "author_id": 300,
    "chapter_id": 69,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:12:43.968Z",
    "created_at": "2016-10-25T17:12:43.968Z",
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
curl "api.goskive.com/v2/flashcards/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aa38f5a9c6a218cf14bf0ef992ca9aae12bcc6415deaf01198e3f0458a79bc8"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/34/report
Content-Type: application/json
Authorization: Bearer e8f675c52d8eec9a02c0931a1e8dec0acffb7ed85e75000892fe4b843e7aada1
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8f675c52d8eec9a02c0931a1e8dec0acffb7ed85e75000892fe4b843e7aada1"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/18/bookmark
Content-Type: application/json
Authorization: Bearer 1329729c9ad8429bd63a2fbb6b0386a3eaf31743f58da3f61e653a231eb3112a
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/18/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1329729c9ad8429bd63a2fbb6b0386a3eaf31743f58da3f61e653a231eb3112a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/38/upvote
Content-Type: application/json
Authorization: Bearer 4412ee79d8a3860586623700aa9aa7942a133343a976a79f3b55fba4bbe9a15e
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4412ee79d8a3860586623700aa9aa7942a133343a976a79f3b55fba4bbe9a15e"
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
    "key": "cache/92562c7480034d6ba2ae931866a1f491.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxODoxMjo0NVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzkyNTYyYzc0ODAwMzRkNmJhMmFlOTMxODY2YTFmNDkxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjVUMTcxMjQ1WiJ9XX0=",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T171245Z",
    "x-amz-signature": "1b6198df5e215c0b99822d5a4f13b2ae61c1a5934fc603ece1b5eabfaf097a13"
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
Authorization: Bearer a5af688ec3a26e09f8a39ae1f4b714b94cc34f55e2e380f3b3beab77d75b6a6a
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
	-H "Authorization: Bearer a5af688ec3a26e09f8a39ae1f4b714b94cc34f55e2e380f3b3beab77d75b6a6a"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 80fd8e2895913dbb7df9a379f27714bcb1d1544f2e79c78695a9e1aa67d5c19f
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
	-H "Authorization: Bearer 80fd8e2895913dbb7df9a379f27714bcb1d1544f2e79c78695a9e1aa67d5c19f"
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
{"password":{"reset_password_token":"rSPHhsyboahx_sCL1hpA","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 197,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-25T17:12:37.671Z",
  "updated_at": "2016-10-25T17:12:37.803Z",
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
  "audit_id": 3853
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"rSPHhsyboahx_sCL1hpA","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/111/comments
Content-Type: application/json
Authorization: Bearer d118e4d7f15a9ed011475e5eca6c2fa7753627cfb5b48718fc4905cc799c0702
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
    "author_id": 868,
    "reply_to_id": null,
    "created_at": "2016-10-25T17:13:25.927Z",
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
curl "api.goskive.com/v2/questions/111/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d118e4d7f15a9ed011475e5eca6c2fa7753627cfb5b48718fc4905cc799c0702"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/109/comments
Content-Type: application/json
Authorization: Bearer a1707c2bbc7be17ea9a56d40b871031b33fc77227bff82b2baf92463e0743f97
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
    "author_id": 862,
    "reply_to_id": null,
    "created_at": "2016-10-25T17:13:25.199Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 862,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:13:25.196Z",
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
curl "api.goskive.com/v2/questions/109/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1707c2bbc7be17ea9a56d40b871031b33fc77227bff82b2baf92463e0743f97"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/113/comments
Content-Type: application/json
Authorization: Bearer 6ee88a79a7d9ad5f4ce0faaf661557978ba3e2a0d7f7a46d6d94f6a895fcbd5c
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
      "author_id": 878,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:26.666Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 877,
      "reply_to_id": null,
      "created_at": "2016-10-25T17:13:26.651Z",
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
curl "api.goskive.com/v2/questions/113/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ee88a79a7d9ad5f4ce0faaf661557978ba3e2a0d7f7a46d6d94f6a895fcbd5c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/110/comments
Content-Type: application/json
Authorization: Bearer 64ac6b49b095fb1fd24ec8901857e0d57cee0a3c45efe3252f0db835871bae1e
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
curl "api.goskive.com/v2/questions/110/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64ac6b49b095fb1fd24ec8901857e0d57cee0a3c45efe3252f0db835871bae1e"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/134/feedbacks
Content-Type: application/json
Authorization: Bearer e662fa0e2051cfcd6e5fc269b9b44c2da6b22ec618cef12ec966ab3d2d6f211f
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
    "user_id": 967,
    "feedbackable_id": 134,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-25T17:13:33.992Z",
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
curl "api.goskive.com/v2/questions/134/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e662fa0e2051cfcd6e5fc269b9b44c2da6b22ec618cef12ec966ab3d2d6f211f"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/132/feedbacks
Content-Type: application/json
Authorization: Bearer cb110ab951e19f2bfde0c5b7372e3c90d070fd1d5d14851b1a4bd4881b95cefd
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
      "id": 44,
      "user_id": 963,
      "feedbackable_id": 132,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:13:33.238Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 962,
      "feedbackable_id": 132,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T17:13:33.228Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/132/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb110ab951e19f2bfde0c5b7372e3c90d070fd1d5d14851b1a4bd4881b95cefd"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/107/votes
Content-Type: application/json
Authorization: Bearer b399d4f67b4abeea0fb0c799e2edbb3d53a7c5813be5ddbfe15e79ebf7753926
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
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 107,
      "user_id": 858
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 107,
      "user_id": 857
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 107,
      "user_id": 856
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/107/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b399d4f67b4abeea0fb0c799e2edbb3d53a7c5813be5ddbfe15e79ebf7753926"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/14/republish
Content-Type: application/json
Authorization: Bearer 7358c86dd5275210b2020831f723f891960fbb5ac66f593825ff185da76bb0f8
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
curl "api.goskive.com/v2/questions/14/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7358c86dd5275210b2020831f723f891960fbb5ac66f593825ff185da76bb0f8"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/19/bookmark
Content-Type: application/json
Authorization: Bearer 9e5fa191346c92c3f20d7772b96f43187c975e28acc270b8f05133fba2a37f14
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/19/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e5fa191346c92c3f20d7772b96f43187c975e28acc270b8f05133fba2a37f14"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/36
Content-Type: application/json
Authorization: Bearer 355083c93cde1de4426d2a5d4375949dc9830f13f6adea0b52c5fc511b92511b
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/36" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 355083c93cde1de4426d2a5d4375949dc9830f13f6adea0b52c5fc511b92511b"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/17/downvote
Content-Type: application/json
Authorization: Bearer 83333c0663a5916397e6a04bdb50ae4b59bf2bf47d922a2061e5f86b2530f2b9
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/17/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83333c0663a5916397e6a04bdb50ae4b59bf2bf47d922a2061e5f86b2530f2b9"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/35
Content-Type: application/json
Authorization: Bearer 00296a587cdc9932a6a842833b6e8ab552435b648153cd9a8a2f057f4e8aed8d
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
    "id": 35,
    "obfuscated_id": "soCS52BooV0",
    "author_id": 185,
    "chapter_id": 40,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:12:35.901Z",
    "created_at": "2016-10-25T17:12:35.773Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00296a587cdc9932a6a842833b6e8ab552435b648153cd9a8a2f057f4e8aed8d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/13/report
Content-Type: application/json
Authorization: Bearer 3d0767b66f127c97deb0c8255799f5e8c1df4ebeb3217ae36d908e1177f2af6f
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/13/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d0767b66f127c97deb0c8255799f5e8c1df4ebeb3217ae36d908e1177f2af6f"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/18/bookmark
Content-Type: application/json
Authorization: Bearer d886cb1596480d2efd1e5af5be2744491e87f9d20412b523ee83c79097e50dc2
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/18/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d886cb1596480d2efd1e5af5be2744491e87f9d20412b523ee83c79097e50dc2"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/12
Content-Type: application/json
Authorization: Bearer e83af228a8bd9fc21dad4b5ba4825d0645907d26dbddc175f851a3c6b9c288dd
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":12,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T17:12:28.147Z","updated_at":"2016-10-25T17:12:28.263Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":17,"author_id":111,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 12,
    "obfuscated_id": "4vzz6KHlMwo",
    "author_id": 111,
    "chapter_id": 17,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T17:12:28.399Z",
    "created_at": "2016-10-25T17:12:28.147Z",
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
    "question": "{\"id\"=>12, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-25T17:12:28.147Z\", \"updated_at\"=>\"2016-10-25T17:12:28.263Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>17, \"author_id\"=>111, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 25,
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
curl "api.goskive.com/v2/questions/12" -d '{"question":{"question":{"id":12,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T17:12:28.147Z","updated_at":"2016-10-25T17:12:28.263Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":17,"author_id":111,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e83af228a8bd9fc21dad4b5ba4825d0645907d26dbddc175f851a3c6b9c288dd"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/16/upvote
Content-Type: application/json
Authorization: Bearer 3b0264b45db18e1ccadc5ecce501f0480e0e2a0561497662a3f9a1a91feb2297
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/16/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b0264b45db18e1ccadc5ecce501f0480e0e2a0561497662a3f9a1a91feb2297"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7d5b660045584bc3aa0d1331a948448a40b0df685e4947efa5fcb094f58bd99d
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
      "creator_id": 597,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "topic_id": 163,
      "discipline_id": 163,
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
      "updated_at": "2016-10-25T17:13:02.445Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d5b660045584bc3aa0d1331a948448a40b0df685e4947efa5fcb094f58bd99d"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer c29ae9ba46dd9326699ad3c54c11286323f6895f0e049605b10e15a56531b8e0
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
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-167",
      "html_url": "https://goskive.com/university/uni-167",
      "slug": "uni-167",
      "name": "National School of Pizza",
      "short_name": "Uni 167",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/7bc79840e61bacbd55aa93f5552ed498973da7e3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ef722df136740df4f3ec930d2c63e36ea0aab6cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T17:13:02.668Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-166",
      "html_url": "https://goskive.com/university/uni-166",
      "slug": "uni-166",
      "name": "National School of Pastry",
      "short_name": "Uni 166",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/04608c10e52ede3ea37be09b081d69e95b921be1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2de1e8a9f298593a399f64c7eacf215a79baee4a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T17:13:02.653Z",
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
	-H "Authorization: Bearer c29ae9ba46dd9326699ad3c54c11286323f6895f0e049605b10e15a56531b8e0"
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
      "id": 246,
      "name": "Virtual heuristic implementation",
      "name_translations": {
        "en": "Virtual heuristic implementation"
      },
      "discipline_id": 246
    },
    {
      "id": 247,
      "name": "Robust next generation functionalities",
      "name_translations": {
        "en": "Robust next generation functionalities"
      },
      "discipline_id": 247
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
GET /v2/topics/245
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
    "id": 245,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 245
  }
}
```



```shell
curl "api.goskive.com/v2/topics/245" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 48efc681ed72805a72b997555e462f55fb50970033e82d5bb778a8988738217f
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
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-93",
      "html_url": "https://goskive.com/university/uni-93",
      "slug": "uni-93",
      "name": "University 80",
      "short_name": "Uni 93",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b4bec54a7f7cd323d36919c55d64b5b5c335955f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c663f9415e0a293c066cadc042878bf2842ce887.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T17:12:45.468Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-92",
      "html_url": "https://goskive.com/university/uni-92",
      "slug": "uni-92",
      "name": "University 79",
      "short_name": "Uni 92",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b3ea3d00a2d8319ab945fe9e5e810ffa19a4d3bd.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e1569ad6c3d0aedaf265cb53f0e148deb76c43ab.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T17:12:45.453Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 91,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-91",
      "html_url": "https://goskive.com/university/uni-91",
      "slug": "uni-91",
      "name": "University 78",
      "short_name": "Uni 91",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0acbb8c8fa3ee80c22c483f268ba1d99f253aa4e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b2cf275a516a5fe6923a38239128ad7a28df233b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T17:12:45.438Z",
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
	-H "Authorization: Bearer 48efc681ed72805a72b997555e462f55fb50970033e82d5bb778a8988738217f"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 82f2fa041191fd9e3a5f8ee198ca990dbae64031d959d544a9e77c018c9bd995
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
    "id": 95,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dc8f2469ecddd5af6505d9db2042b45f53ad683e.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c9a133dca397548adb89a35bebfdaee19823cf8d.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-25T17:12:45.582Z",
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
	-H "Authorization: Bearer 82f2fa041191fd9e3a5f8ee198ca990dbae64031d959d544a9e77c018c9bd995"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer eb3f1a0b957a87bdc5ebf9e3b40ad36a0e3d2f7f1082c4797a942cd574e9e184
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":250,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 798,
    "id": 240,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 247,
    "additional_university_ids": [

    ],
    "topic_id": 250,
    "discipline_id": 250,
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
    "chapters_updated_at": "2016-10-25T17:13:19.158Z",
    "updated_at": "2016-10-25T17:13:19.290Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 158,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-25T17:13:19.248Z",
        "course_id": 240,
        "author_id": 798,
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
        "id": 159,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-25T17:13:19.264Z",
        "course_id": 240,
        "author_id": 798,
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
        "id": 160,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-25T17:13:19.280Z",
        "course_id": 240,
        "author_id": 798,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":250,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb3f1a0b957a87bdc5ebf9e3b40ad36a0e3d2f7f1082c4797a942cd574e9e184"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5a5d761c2a7c2a1c11d9a7fa8d99e2d5c68f507fb34570b637f2b15f65006130
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":251,"published":false}}
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
    "creator_id": 799,
    "id": 241,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 248,
    "additional_university_ids": [

    ],
    "topic_id": 251,
    "discipline_id": 251,
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
    "updated_at": "2016-10-25T17:13:19.433Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":251,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a5d761c2a7c2a1c11d9a7fa8d99e2d5c68f507fb34570b637f2b15f65006130"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 48e95e77fe0b9544cd4957419a8a4333828e0ee98ea5997f49e35a1bd08e9ea2
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
      "creator_id": 805,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 251,
      "additional_university_ids": [

      ],
      "topic_id": 258,
      "discipline_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 191",
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
      "updated_at": "2016-10-25T17:13:19.961Z",
      "shortname": "fu-course-191"
    },
    {
      "creator_id": 805,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 251,
      "additional_university_ids": [

      ],
      "topic_id": 259,
      "discipline_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
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
      "chapters_updated_at": "2016-10-25T17:13:20.243Z",
      "updated_at": "2016-10-25T17:13:20.249Z",
      "shortname": "fu-course-192"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48e95e77fe0b9544cd4957419a8a4333828e0ee98ea5997f49e35a1bd08e9ea2"
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
      "creator_id": 815,
      "id": 256,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 266,
      "discipline_id": 266,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
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
      "updated_at": "2016-10-25T17:13:20.774Z",
      "shortname": "fu-course-199"
    },
    {
      "creator_id": 815,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-200",
      "html_url": "https://goskive.com/course/fu-course-200",
      "slug": "fu-course-200",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 267,
      "discipline_id": 267,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 200",
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
      "chapters_updated_at": "2016-10-25T17:13:21.060Z",
      "updated_at": "2016-10-25T17:13:21.066Z",
      "shortname": "fu-course-200"
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
Authorization: Bearer 370c436ec3ea1ea0e7a567a692b51a14d40b1a596e3af78649fbb6cd07912757
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
      "creator_id": 811,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 262,
      "discipline_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
      "updated_at": "2016-10-25T17:13:20.461Z",
      "shortname": "fu-course-195"
    },
    {
      "creator_id": 811,
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 263,
      "discipline_id": 263,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
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
      "updated_at": "2016-10-25T17:13:20.501Z",
      "shortname": "fu-course-196"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 370c436ec3ea1ea0e7a567a692b51a14d40b1a596e3af78649fbb6cd07912757"
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
      "creator_id": 820,
      "id": 260,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 256,
      "additional_university_ids": [

      ],
      "topic_id": 270,
      "discipline_id": 270,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
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
      "updated_at": "2016-10-25T17:13:21.272Z",
      "shortname": "fu-course-203"
    },
    {
      "creator_id": 820,
      "id": 261,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-204",
      "html_url": "https://goskive.com/course/fu-course-204",
      "slug": "fu-course-204",
      "university_id": 256,
      "additional_university_ids": [

      ],
      "topic_id": 271,
      "discipline_id": 271,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 204",
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
      "updated_at": "2016-10-25T17:13:21.312Z",
      "shortname": "fu-course-204"
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
Authorization: Bearer 1f35d6c5de1aecdd7ff5c12416d8dc3ea5b355a68a0d741dde68a2ccf734fc52
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
  "id": 667,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-25T17:13:11.588Z",
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
	-H "Authorization: Bearer 1f35d6c5de1aecdd7ff5c12416d8dc3ea5b355a68a0d741dde68a2ccf734fc52"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/97
Content-Type: application/json
Authorization: Bearer f0368f7a0258dd9d2bfea1434b6cb607480cc6fb8b8d96122570993258b78d69
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
    "id": 97,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 27,
    "fields_of_study": [
      27,
      28
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-25T17:12:27.116Z",
    "updated_at": "2016-10-25T17:12:27.116Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/97" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0368f7a0258dd9d2bfea1434b6cb607480cc6fb8b8d96122570993258b78d69"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/99
Content-Type: application/json
Authorization: Bearer d8b675135a4b2593020bc80e576d992c8dd3f91d93ddb7659dee6b627620cd17
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
    "id": 99,
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
    "created_at": "2016-10-25T17:12:27.199Z",
    "updated_at": "2016-10-25T17:12:27.199Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/99" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8b675135a4b2593020bc80e576d992c8dd3f91d93ddb7659dee6b627620cd17"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/18
Content-Type: application/json
Authorization: Bearer 5524b630d95a1453d4e5a15ce33b34fdbcfc1a6a2435c89ff635abd3422bcd84
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5524b630d95a1453d4e5a15ce33b34fdbcfc1a6a2435c89ff635abd3422bcd84"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/16
Content-Type: application/json
Authorization: Bearer 7730f7699a198c4f8dffbb4621823178a83ade779484903e7f215f55a0a64130
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
    "votable_id": 99,
    "user_id": 781
  }
}
```



```shell
curl "api.goskive.com/v2/votes/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7730f7699a198c4f8dffbb4621823178a83ade779484903e7f215f55a0a64130"
```
