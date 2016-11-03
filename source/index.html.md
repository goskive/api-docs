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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"cf3d3e3359ee5d0f36cdde9183073f680a84d16d1f799a22efe41af36d5baa22","client_secret":"13fb148b6cc95a3b9660e1e9df7c7b64e07b1bd95de8da2d1850c83c36d7d9de"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"cf3d3e3359ee5d0f36cdde9183073f680a84d16d1f799a22efe41af36d5baa22","client_secret":"13fb148b6cc95a3b9660e1e9df7c7b64e07b1bd95de8da2d1850c83c36d7d9de"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic M2RjZjdkMDcxMTQwNjVkNjkzZWE4ZWNkZWRkZDg2ZjgyOGRlZDA2OGI0ZWFh
ZDE2OTA3ZDNhMWRmN2NjMjFmNjo1ZDBkMDU4ZTgwN2Y1YTE0ODA0ZDM3Nzk2
MGU2ZWM5MmYzYTYzNmYwMDk5NTQ3M2E0Yjk3NmZiZDc4NTdkM2Q3

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
	-u 3dcf7d07114065d693ea8ecdeddd86f828ded068b4eaad16907d3a1df7cc21f6:5d0d058e807f5a14804d377960e6ec92f3a636f00995473a4b976fbd7857d3d7
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
{"grant_type":"client_credentials","client_id":"01fbac2b95c5ca0f39936b491b158516af5cf80e7b998c0507567b3b133b7510","client_secret":"a114f0228fb1b34e9754395595910e6ffe01d7a1e3cda63586a27ec828c2f812"}
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
  "access_token": "2290673bcf80552cedcec675888be701a2253352a45912da9f4aa80499a8787d",
  "token_type": "bearer",
  "created_at": 1478195268
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"01fbac2b95c5ca0f39936b491b158516af5cf80e7b998c0507567b3b133b7510","client_secret":"a114f0228fb1b34e9754395595910e6ffe01d7a1e3cda63586a27ec828c2f812"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e1af226dc8070051e9c805fe8f5a4e74e750801959bf185d728d447a13b576a5","client_secret":"abc9dcf7330d5c035e8ad33dcb377a036e36f73c65f24ba587f0afa3e67221b8"}
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
  "access_token": "00e122c482e29dacb74da6ca245257120c57a3f3a986828c5cfced1c09e9afcb",
  "token_type": "bearer",
  "created_at": 1478195268
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e1af226dc8070051e9c805fe8f5a4e74e750801959bf185d728d447a13b576a5","client_secret":"abc9dcf7330d5c035e8ad33dcb377a036e36f73c65f24ba587f0afa3e67221b8"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OWIxN2Q0MTQyMjNmZTEwMDM3MTU4MDc3NWQ5M2ZmNzU1ZjY1N2Y0NmZkNjE1
MWU5NmExZDMwMThkMTA0ZTU0MDowOGQ3NjY0M2U5MGRiYzI2Nzc4ODg1MWQ0
NDNkMTk3ODAxZDk5ZTdjZjE2NTQzNjRjN2UyYTRkOGQ0NTgxZDJj

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
  "access_token": "42b6ab77cb6d64fb982fe054504fa81e2e8d14ff551fd08ce5bb8d3bf2d474a8",
  "token_type": "bearer",
  "created_at": 1478195268
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 9b17d414223fe100371580775d93ff755f657f46fd6151e96a1d3018d104e540:08d76643e90dbc267788851d443d197801d99e7cf1654364c7e2a4d8d4581d2c
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
Authorization: Bearer bc268556a59a0ad74c97fd53b44429537d4dc1681cb79f8874a768503a3dd25d
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
    "company_id": 13,
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
	-H "Authorization: Bearer bc268556a59a0ad74c97fd53b44429537d4dc1681cb79f8874a768503a3dd25d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/114/flashcards
Content-Type: application/json
Authorization: Bearer 0e4b04e7489948f371a73797ad1a0f9c74f9d7f2f4d43d74472af0e5dad1e6a0
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":114,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 50,
    "obfuscated_id": "3_Ybw_gc_HE",
    "author_id": 591,
    "chapter_id": 114,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:27.328Z",
    "created_at": "2016-11-03T17:48:27.328Z",
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
curl "api.goskive.com/v2/chapters/114/flashcards" -d '{"flashcard":{"chapter_id":114,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e4b04e7489948f371a73797ad1a0f9c74f9d7f2f4d43d74472af0e5dad1e6a0"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/116/flashcards
Content-Type: application/json
Authorization: Bearer caba7afafdacde1e0f3c6a2664995aea6043f13d84795c31b61646eff2d36a60
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 595,
      "chapter_id": 116,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:27.722Z",
      "created_at": "2016-11-03T17:48:27.722Z",
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 595,
      "chapter_id": 116,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:27.761Z",
      "created_at": "2016-11-03T17:48:27.761Z",
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 595,
      "chapter_id": 116,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:27.800Z",
      "created_at": "2016-11-03T17:48:27.800Z",
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
curl "api.goskive.com/v2/chapters/116/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer caba7afafdacde1e0f3c6a2664995aea6043f13d84795c31b61646eff2d36a60"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/68/questions
Content-Type: application/json
Authorization: Bearer 51d6d624139099c4a594488f152f5af25050c20a258e377365734f9863c2b032
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":68,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 16,
    "obfuscated_id": "Drq0t9y67cE",
    "author_id": 341,
    "chapter_id": 68,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:01.776Z",
    "created_at": "2016-11-03T17:48:01.776Z",
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
        "id": 32,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 33,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 34,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 35,
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
curl "api.goskive.com/v2/chapters/68/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":68,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51d6d624139099c4a594488f152f5af25050c20a258e377365734f9863c2b032"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/67/questions
Content-Type: application/json
Authorization: Bearer 0267e5d97fc90aa4bfa681042f83189b409d7019f146079aea8d968755c7700c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":67,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 15,
    "obfuscated_id": "j5PwoYQzNCc",
    "author_id": 338,
    "chapter_id": 67,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:01.161Z",
    "created_at": "2016-11-03T17:48:01.161Z",
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
        "id": 30,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 31,
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
curl "api.goskive.com/v2/chapters/67/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":67,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0267e5d97fc90aa4bfa681042f83189b409d7019f146079aea8d968755c7700c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/69/questions
Content-Type: application/json
Authorization: Bearer 32e54cbc301b578f83528042f6c1cc3942e355a564022dbb6143717cee6d33b5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":69,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 17,
    "obfuscated_id": "s3oqsdqLejU",
    "author_id": 344,
    "chapter_id": 69,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:02.607Z",
    "created_at": "2016-11-03T17:48:02.607Z",
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
        "id": 36,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 37,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/69/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":69,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32e54cbc301b578f83528042f6c1cc3942e355a564022dbb6143717cee6d33b5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/66/questions
Content-Type: application/json
Authorization: Bearer 2a2c0a4b99187a98a7d348eebb778df2ed068d86740421074c14693e5b3530ed
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":66,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 14,
    "obfuscated_id": "gbKzjBR_8tw",
    "author_id": 335,
    "chapter_id": 66,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:00.550Z",
    "created_at": "2016-11-03T17:48:00.550Z",
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
        "id": 27,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 28,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 29,
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
curl "api.goskive.com/v2/chapters/66/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":66,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a2c0a4b99187a98a7d348eebb778df2ed068d86740421074c14693e5b3530ed"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/65/questions
Content-Type: application/json
Authorization: Bearer 16cddee5f8ecbec9d846c33a94f376949171b52f778c633aaa0af887d4f67dfa
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 329,
      "chapter_id": 65,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:47:59.810Z",
      "created_at": "2016-11-03T17:47:59.673Z",
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
      "author_id": 330,
      "chapter_id": 65,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:00.031Z",
      "created_at": "2016-11-03T17:47:59.890Z",
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
    },
    {
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 331,
      "chapter_id": 65,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T17:48:00.259Z",
      "created_at": "2016-11-03T17:48:00.116Z",
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
          "id": 25,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 26,
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
curl "api.goskive.com/v2/chapters/65/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16cddee5f8ecbec9d846c33a94f376949171b52f778c633aaa0af887d4f67dfa"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/171
Content-Type: application/json
Authorization: Bearer 68e5d2effad2fbfc7146e7998d9a40ede0736a30ab1e0f5b501352c32fed11e4
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
curl "api.goskive.com/v2/chapters/171" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68e5d2effad2fbfc7146e7998d9a40ede0736a30ab1e0f5b501352c32fed11e4"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/172
Content-Type: application/json
Authorization: Bearer b1972b8f0e2cc664ff19e7dc854b3bc7bfd87d0d49915459b2e168a27a70199c
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
curl "api.goskive.com/v2/chapters/172" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1972b8f0e2cc664ff19e7dc854b3bc7bfd87d0d49915459b2e168a27a70199c"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/167
Content-Type: application/json
Authorization: Bearer 51c00c2ef2e3f843267e2e32fe120d08db8336728c3a931087a786cbedf23505
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
curl "api.goskive.com/v2/chapters/167" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51c00c2ef2e3f843267e2e32fe120d08db8336728c3a931087a786cbedf23505"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/173
Content-Type: application/json
Authorization: Bearer 68e3bcaa8a4bb6f9d2721a23a3a56aa8142178b0ab2bb0fa6b41def7e5e27350
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/173" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68e3bcaa8a4bb6f9d2721a23a3a56aa8142178b0ab2bb0fa6b41def7e5e27350"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/169
Content-Type: application/json
Authorization: Bearer 005ee4ac9ae0267c8c225d7ade0d101adcbc6377cb2fb2da0aead6d3951f6b57
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
    "id": 169,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T17:48:47.694Z",
    "course_id": 267,
    "author_id": 836,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-03T17:48:47.124Z",
    "questions_updated_at": "2016-11-03T17:48:47.124Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 840,
        "chapter_id": 169,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:47.676Z",
        "created_at": "2016-11-03T17:48:47.676Z",
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
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 838,
        "chapter_id": 169,
        "position": 83,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:47.563Z",
        "created_at": "2016-11-03T17:48:47.435Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/169" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 005ee4ac9ae0267c8c225d7ade0d101adcbc6377cb2fb2da0aead6d3951f6b57"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/165
Content-Type: application/json
Authorization: Bearer daac1667112f6ab62f18ab727d5362f391c21003625459eccdae52a93aa856ff
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
    "id": 165,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T17:48:46.132Z",
    "course_id": 263,
    "author_id": 821,
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
curl "api.goskive.com/v2/chapters/165" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daac1667112f6ab62f18ab727d5362f391c21003625459eccdae52a93aa856ff"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/48/replies
Content-Type: application/json
Authorization: Bearer bcb91090c0ef4ec81b946f40b822ccf638ce35ea61f158779beb5beb362a8539
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
    "id": 49,
    "author_id": 583,
    "reply_to_id": 48,
    "created_at": "2016-11-03T17:48:26.655Z",
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
curl "api.goskive.com/v2/comments/48/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcb91090c0ef4ec81b946f40b822ccf638ce35ea61f158779beb5beb362a8539"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/50/replies
Content-Type: application/json
Authorization: Bearer 96b27be8c3c3f37a093e7b1cf8e617394cc3975298a7f07c53ff3f13b4e1da9c
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
curl "api.goskive.com/v2/comments/50/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96b27be8c3c3f37a093e7b1cf8e617394cc3975298a7f07c53ff3f13b4e1da9c"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer f7bc244d2aff103c2e1e7d12a2961232274226f738a3cadc6a0fba0acdcbe946
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
	-H "Authorization: Bearer f7bc244d2aff103c2e1e7d12a2961232274226f738a3cadc6a0fba0acdcbe946"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer 4afd14867e8b8f0bf8ac1151a175934b97b89317192e8e7627086505e2b6f3de
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
curl "api.goskive.com/v2/comments/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4afd14867e8b8f0bf8ac1151a175934b97b89317192e8e7627086505e2b6f3de"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 2665b8b5ca991d4437fee3742dd356b7e65e1cbc5e861aec0863e86062b5a2cd
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
	-H "Authorization: Bearer 2665b8b5ca991d4437fee3742dd356b7e65e1cbc5e861aec0863e86062b5a2cd"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/3/report
Content-Type: application/json
Authorization: Bearer 31d865bd4bb570f3ebf737a0dde6817ed642498d11e575538baf058b43d39ac2
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31d865bd4bb570f3ebf737a0dde6817ed642498d11e575538baf058b43d39ac2"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/31
Content-Type: application/json
Authorization: Bearer 0866117c718a664d26e0c45720736931e7c6b3849f1b8bf3aaf12674868e077d
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
    "id": 31,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/0df235007210ab1331461f6a10296cd43f327e64.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-03T17:48:53.082Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/31" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0866117c718a664d26e0c45720736931e7c6b3849f1b8bf3aaf12674868e077d"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 7a314fb203b937ac4b4ed281c533bc8a4aec5076f2b1bc931bc37d6570399983
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
      "id": 28,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T17:48:53.020Z"
    },
    {
      "id": 29,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/eb30fd9939333e805126ba26a8736769f7ca2ba6.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T17:48:53.025Z"
    },
    {
      "id": 30,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T17:48:53.029Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a314fb203b937ac4b4ed281c533bc8a4aec5076f2b1bc931bc37d6570399983"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 8d1691d8aa401e8a41e84f82d8f5545b599a7c2fdc26f24fb7a8ca26221b3bc9
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
	-H "Authorization: Bearer 8d1691d8aa401e8a41e84f82d8f5545b599a7c2fdc26f24fb7a8ca26221b3bc9"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 231ca071d41cd4de30df99e2e331f5866c44f1896fee11f47fc06471dd23dc92
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
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 231ca071d41cd4de30df99e2e331f5866c44f1896fee11f47fc06471dd23dc92"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 3418356ff42ecbc64b4da71a4a2899e5999c4163b405ae9a104e249e5e8a5e75
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
	-H "Authorization: Bearer 3418356ff42ecbc64b4da71a4a2899e5999c4163b405ae9a104e249e5e8a5e75"
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
Authorization: Bearer 2854541d4bb872f03fd07de9815be86d80716cbda58667ca2126a969e2500d03
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
	-H "Authorization: Bearer 2854541d4bb872f03fd07de9815be86d80716cbda58667ca2126a969e2500d03"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3d336ee00f4dabc0c5900ada447fc9a5b30b18e07e5a08926d1e108930fad1a9
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
    "id": 23,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T17:47:43.727Z",
    "course_id": 21,
    "author_id": 70,
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
	-H "Authorization: Bearer 3d336ee00f4dabc0c5900ada447fc9a5b30b18e07e5a08926d1e108930fad1a9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ac0bb1607a34470b246beb144620f9e2417f660fdca4ae58ee7f06828ac71c5b
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
      "id": 4,
      "title": "Clever Chapter Title 4",
      "position": 1,
      "updated_at": "2016-11-03T17:47:41.156Z",
      "course_id": 10,
      "author_id": 27,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 5,
      "title": "Clever Chapter Title 5",
      "position": 2,
      "updated_at": "2016-11-03T17:47:41.182Z",
      "course_id": 10,
      "author_id": 28,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 6,
      "title": "Clever Chapter Title 6",
      "position": 3,
      "updated_at": "2016-11-03T17:47:41.528Z",
      "course_id": 10,
      "author_id": 29,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T17:47:41.080Z",
      "questions_updated_at": "2016-11-03T17:47:41.080Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac0bb1607a34470b246beb144620f9e2417f660fdca4ae58ee7f06828ac71c5b"
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
      "id": 16,
      "title": "Clever Chapter Title 16",
      "position": 1,
      "updated_at": "2016-11-03T17:47:42.724Z",
      "course_id": 16,
      "author_id": 55,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 17,
      "title": "Clever Chapter Title 17",
      "position": 2,
      "updated_at": "2016-11-03T17:47:42.748Z",
      "course_id": 16,
      "author_id": 56,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 18,
      "title": "Clever Chapter Title 18",
      "position": 3,
      "updated_at": "2016-11-03T17:47:43.012Z",
      "course_id": 16,
      "author_id": 57,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T17:47:42.647Z",
      "questions_updated_at": "2016-11-03T17:47:42.647Z",
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
Authorization: Bearer 7d43c29e5906d49cb79f3c5da9deca7eb0fe161aac799cedea25617072db634b
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
      "title": "Clever Chapter Title 7",
      "position": 1,
      "updated_at": "2016-11-03T17:47:41.789Z",
      "course_id": 12,
      "author_id": 36,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 8,
      "title": "Clever Chapter Title 8",
      "position": 2,
      "updated_at": "2016-11-03T17:47:41.814Z",
      "course_id": 12,
      "author_id": 37,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 9,
      "title": "Clever Chapter Title 9",
      "position": 3,
      "updated_at": "2016-11-03T17:47:41.839Z",
      "course_id": 12,
      "author_id": 38,
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
	-H "Authorization: Bearer 7d43c29e5906d49cb79f3c5da9deca7eb0fe161aac799cedea25617072db634b"
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
      "id": 19,
      "title": "Clever Chapter Title 19",
      "position": 1,
      "updated_at": "2016-11-03T17:47:43.130Z",
      "course_id": 17,
      "author_id": 61,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 20,
      "title": "Clever Chapter Title 20",
      "position": 2,
      "updated_at": "2016-11-03T17:47:43.156Z",
      "course_id": 17,
      "author_id": 62,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 21,
      "title": "Clever Chapter Title 21",
      "position": 3,
      "updated_at": "2016-11-03T17:47:43.181Z",
      "course_id": 17,
      "author_id": 63,
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
Authorization: Bearer 4324779aeb3f75a14b0357aa0094648eb438926e76d71b14de4632576ba51328
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
    "updated_at": "2016-11-03T17:47:39.816Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4324779aeb3f75a14b0357aa0094648eb438926e76d71b14de4632576ba51328"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 8a0e9a9a9e345316ca6f34ed1a1b985a694b74814797a238679dce1feadb8859
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
      "updated_at": "2016-11-03T17:47:40.204Z"
    },
    {
      "id": 4,
      "course_id": 4,
      "user_id": 9,
      "updated_at": "2016-11-03T17:47:40.220Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a0e9a9a9e345316ca6f34ed1a1b985a694b74814797a238679dce1feadb8859"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/159/files
Content-Type: application/json
Authorization: Bearer d342816c1df29f1c9f5d280621af6632512d41e29e1e4e2bd6313c8a0f05919d
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
      "id": 3,
      "uploader": {
        "id": 426,
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
        "created_at": "2016-11-03T17:48:12.500Z",
        "updated_at": "2016-11-03T17:48:12.500Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T17:48:12.513Z",
      "updated_at": "2016-11-03T17:48:12.513Z",
      "course_id": 159,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 427,
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
        "created_at": "2016-11-03T17:48:12.521Z",
        "updated_at": "2016-11-03T17:48:12.521Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T17:48:12.532Z",
      "updated_at": "2016-11-03T17:48:12.532Z",
      "course_id": 159,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 428,
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
        "created_at": "2016-11-03T17:48:12.541Z",
        "updated_at": "2016-11-03T17:48:12.541Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T17:48:12.553Z",
      "updated_at": "2016-11-03T17:48:12.553Z",
      "course_id": 159,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/159/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d342816c1df29f1c9f5d280621af6632512d41e29e1e4e2bd6313c8a0f05919d"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/162/files
Content-Type: application/json
Authorization: Bearer e1ebcfadd7bc3217428e1c98aaddbcf5b7ccc165d1fe7fc6abaf88524cd45740
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
    "id": 6,
    "uploader": {
      "id": 435,
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
      "created_at": "2016-11-03T17:48:12.950Z",
      "updated_at": "2016-11-03T17:48:12.950Z"
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
    "created_at": "2016-11-03T17:48:12.983Z",
    "updated_at": "2016-11-03T17:48:12.983Z",
    "course_id": 162,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/162/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1ebcfadd7bc3217428e1c98aaddbcf5b7ccc165d1fe7fc6abaf88524cd45740"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/161/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 61b0e857d2037f6b2134eacfd29be25ac8af21c265190228341167ab9610988d
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
    "key": "cache/24269f6f9e59fd94f01554837e641d25.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxODo0ODoxMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzI0MjY5ZjZmOWU1OWZkOTRmMDE1NTQ4MzdlNjQxZDI1LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDMvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTAzVDE3NDgxMloifV19",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T174812Z",
    "x-amz-signature": "f3318f6594b2e4281274ea2191984b28764c971b9c0dda475efa32731df99520"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/161/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61b0e857d2037f6b2134eacfd29be25ac8af21c265190228341167ab9610988d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer c8a1f475af3cf6e16f48d5a039104f307813b2b1e91194a18e90db964e43ed1e
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
	-H "Authorization: Bearer c8a1f475af3cf6e16f48d5a039104f307813b2b1e91194a18e90db964e43ed1e"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9986bf703056c6d19fd5af14f5ab70ac5abb83d7fbdb4c98172c5f98f80d35f0
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
	-H "Authorization: Bearer 9986bf703056c6d19fd5af14f5ab70ac5abb83d7fbdb4c98172c5f98f80d35f0"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 451dd5d1f3aec25ba50ecc6118aec7a28f66caf339e632e6937edfaeb9d3dd8c
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
	-H "Authorization: Bearer 451dd5d1f3aec25ba50ecc6118aec7a28f66caf339e632e6937edfaeb9d3dd8c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c144ad61eee23782ef5bb1b11298ee06ee88bc24fc519cfc37f066ed9998c32d
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
	-H "Authorization: Bearer c144ad61eee23782ef5bb1b11298ee06ee88bc24fc519cfc37f066ed9998c32d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 19b9cca34a45f4d81a99856f1d0982ac681bafb2b6c06493e96528350673b3a4
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
	-H "Authorization: Bearer 19b9cca34a45f4d81a99856f1d0982ac681bafb2b6c06493e96528350673b3a4"
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
    "creator_id": 954,
    "id": 310,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 295,
    "additional_university_ids": [

    ],
    "topic_id": 322,
    "discipline_id": 323,
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
    "chapters_updated_at": "2016-11-03T17:48:57.643Z",
    "updated_at": "2016-11-03T17:48:59.168Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 186,
        "title": "Clever Chapter Title 162",
        "position": 1,
        "updated_at": "2016-11-03T17:48:59.118Z",
        "course_id": 310,
        "author_id": 954,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T17:48:57.643Z",
        "questions_updated_at": "2016-11-03T17:48:57.643Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 187,
        "title": "Clever Chapter Title 163",
        "position": 2,
        "updated_at": "2016-11-03T17:48:59.160Z",
        "course_id": 310,
        "author_id": 954,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T17:48:57.643Z",
        "questions_updated_at": "2016-11-03T17:48:57.643Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 954,
        "chapter_id": 186,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:57.865Z",
        "created_at": "2016-11-03T17:48:57.741Z",
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
      },
      {
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 954,
        "chapter_id": 187,
        "position": 102,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:48:58.269Z",
        "created_at": "2016-11-03T17:48:58.139Z",
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
            "id": 233,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 234,
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
Authorization: Bearer 589d3d313203b14d5e2effed4518fb8fc2f0621c556bca82957e29d09594c2d9
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
    "creator_id": 965,
    "id": 312,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 297,
    "additional_university_ids": [

    ],
    "topic_id": 324,
    "discipline_id": 325,
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
    "chapters_updated_at": "2016-11-03T17:49:00.890Z",
    "updated_at": "2016-11-03T17:49:02.439Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 190,
        "title": "Clever Chapter Title 166",
        "position": 1,
        "updated_at": "2016-11-03T17:49:02.389Z",
        "course_id": 312,
        "author_id": 965,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T17:49:00.890Z",
        "questions_updated_at": "2016-11-03T17:49:00.890Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 191,
        "title": "Clever Chapter Title 167",
        "position": 2,
        "updated_at": "2016-11-03T17:49:02.431Z",
        "course_id": 312,
        "author_id": 965,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T17:49:00.890Z",
        "questions_updated_at": "2016-11-03T17:49:00.890Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 966,
        "chapter_id": 190,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:02.219Z",
        "created_at": "2016-11-03T17:49:02.219Z",
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
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 966,
        "chapter_id": 191,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:02.295Z",
        "created_at": "2016-11-03T17:49:02.295Z",
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
        "author_id": 966,
        "chapter_id": 190,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:02.262Z",
        "created_at": "2016-11-03T17:49:02.262Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 966,
        "chapter_id": 191,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:02.338Z",
        "created_at": "2016-11-03T17:49:02.338Z",
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
        "id": 125,
        "obfuscated_id": "K6zw0Yc6Me8",
        "author_id": 966,
        "chapter_id": 190,
        "position": 112,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:01.118Z",
        "created_at": "2016-11-03T17:49:00.995Z",
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
        "author_id": 966,
        "chapter_id": 190,
        "position": 113,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:01.306Z",
        "created_at": "2016-11-03T17:49:01.186Z",
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
      },
      {
        "id": 127,
        "obfuscated_id": "E3yfRgAzssw",
        "author_id": 966,
        "chapter_id": 191,
        "position": 114,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:01.531Z",
        "created_at": "2016-11-03T17:49:01.399Z",
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
            "id": 257,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 258,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 128,
        "obfuscated_id": "Q4ODZIcqv0E",
        "author_id": 966,
        "chapter_id": 191,
        "position": 115,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T17:49:01.726Z",
        "created_at": "2016-11-03T17:49:01.601Z",
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
            "id": 259,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 260,
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
	-H "Authorization: Bearer 589d3d313203b14d5e2effed4518fb8fc2f0621c556bca82957e29d09594c2d9"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/298/pin
Content-Type: application/json
Authorization: Bearer 17227782e956d033c642d60b2b1c0376333557f0b78fbf07659215fbec4642a8
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/298/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17227782e956d033c642d60b2b1c0376333557f0b78fbf07659215fbec4642a8"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/308/pin
Content-Type: application/json
Authorization: Bearer f2e069b7eaf3d507f36f2b9a64cc56b60e278c408fa20e946c71f79006bff941
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/308/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2e069b7eaf3d507f36f2b9a64cc56b60e278c408fa20e946c71f79006bff941"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 24cef3e6bc1af9ebca566bb77cd714520fef37dff56a20b6525531620e3bf9b8
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
    "creator_id": 919,
    "id": 295,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 280,
    "additional_university_ids": [

    ],
    "topic_id": 307,
    "discipline_id": 308,
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
    "updated_at": "2016-11-03T17:48:53.862Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24cef3e6bc1af9ebca566bb77cd714520fef37dff56a20b6525531620e3bf9b8"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer e40c38b5453b2885f028cedd9c2d02de0fb2fc69996d5ee47264e2ac658b8175
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
    "id": 533,
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
    "created_at": "2016-11-03T17:48:23.366Z",
    "updated_at": "2016-11-03T17:48:23.366Z",
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
	-H "Authorization: Bearer e40c38b5453b2885f028cedd9c2d02de0fb2fc69996d5ee47264e2ac658b8175"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 41369f62fa78afb29196b357721e0142458aa057203ecf4d45d5af6dec1d52b6
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
    "id": 534,
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
    "created_at": "2016-11-03T17:48:23.470Z",
    "updated_at": "2016-11-03T17:48:23.513Z",
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
	-H "Authorization: Bearer 41369f62fa78afb29196b357721e0142458aa057203ecf4d45d5af6dec1d52b6"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2f21854784a78766072d0bc074abb2a82d2b6bcebf78efbc583ea74494d6bace
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
    "id": 535,
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
    "created_at": "2016-11-03T17:48:23.537Z",
    "updated_at": "2016-11-03T17:48:23.537Z",
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
	-H "Authorization: Bearer 2f21854784a78766072d0bc074abb2a82d2b6bcebf78efbc583ea74494d6bace"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a84c5bad812cce8c8c84c2474c8c16daef2228790a74c5bc22a03e5f81838c2e
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
    "id": 537,
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
    "created_at": "2016-11-03T17:48:23.711Z",
    "updated_at": "2016-11-03T17:48:23.711Z",
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
	-H "Authorization: Bearer a84c5bad812cce8c8c84c2474c8c16daef2228790a74c5bc22a03e5f81838c2e"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 38cd8d463ba9f3632767e9f1be92a028fc56a28244fa91301edfbddf4e48d2a4
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
    "id": 538,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/64a7c82bb2a0cd054ae618e278ccfd419ba323ef.jpg",
    "university_id": null,
    "fields_of_study": [
      199
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T17:48:23.790Z",
    "updated_at": "2016-11-03T17:48:24.031Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/35dfc096d3685c0a0d5900fafbb914d6aa75380b.jpg",
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
	-H "Authorization: Bearer 38cd8d463ba9f3632767e9f1be92a028fc56a28244fa91301edfbddf4e48d2a4"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 913b04d7cf2add37b73b5ece4eec4ec7e43499d8d4a163531f03dbb20ea246cb
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
      "bookmarkable_id": 8,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 9,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 10,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 913b04d7cf2add37b73b5ece4eec4ec7e43499d8d4a163531f03dbb20ea246cb"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 51f722f576b87c6d5f49a66760ea47a115c5590bd793e985fb5866bbab1efcc2
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
	-H "Authorization: Bearer 51f722f576b87c6d5f49a66760ea47a115c5590bd793e985fb5866bbab1efcc2"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1ec6738457bdb4a144e002a5d78d9cc34bd28c2db3f77d19fce629936faeb518
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
	-H "Authorization: Bearer 1ec6738457bdb4a144e002a5d78d9cc34bd28c2db3f77d19fce629936faeb518"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 7f423792b4bb414fb6de3e836eb215443c0f5880a45e2af9d44c4fe89e6a0ecd
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
      "creator_id": 630,
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-175",
      "html_url": "https://goskive.com/course/mit-course-175",
      "slug": "mit-course-175",
      "university_id": 203,
      "additional_university_ids": [

      ],
      "topic_id": 228,
      "discipline_id": 229,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
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
      "updated_at": "2016-11-03T17:48:30.665Z",
      "shortname": "mit-course-175"
    },
    {
      "creator_id": 631,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-176",
      "html_url": "https://goskive.com/course/mit-course-176",
      "slug": "mit-course-176",
      "university_id": 204,
      "additional_university_ids": [

      ],
      "topic_id": 229,
      "discipline_id": 230,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "updated_at": "2016-11-03T17:48:30.748Z",
      "shortname": "mit-course-176"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f423792b4bb414fb6de3e836eb215443c0f5880a45e2af9d44c4fe89e6a0ecd"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 0085f21ef8ef96e3a35e4ffc28be93146075dd3cab24be7959de072d35410a29
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
        "created_at": "2016-11-03T17:48:53.277Z",
        "updated_at": "2016-11-03T17:48:53.277Z",
        "file_url": "memory://4a7cffd5db24fcd126e62db7d4373e78.pdf",
        "course_id": 291,
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
        "created_at": "2016-11-03T17:48:53.362Z",
        "updated_at": "2016-11-03T17:48:53.362Z",
        "file_url": "memory://5e6dffdf9210faf07570f01ede849aaf.pdf",
        "course_id": 292,
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
        "created_at": "2016-11-03T17:48:53.447Z",
        "updated_at": "2016-11-03T17:48:53.447Z",
        "file_url": "memory://68a3eb29ef659b4c44941c92faf3cfca.pdf",
        "course_id": 293,
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
	-H "Authorization: Bearer 0085f21ef8ef96e3a35e4ffc28be93146075dd3cab24be7959de072d35410a29"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer dbb16629413e21c983e8c68d612c29f178adf01106af284f19b7dbb7938f89c8
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
      "company_id": 19,
      "company": {
        "id": 19,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T17:48:40.275Z"
      },
      "created_at": "2016-11-03T17:48:40.278Z",
      "updated_at": "2016-11-03T17:48:40.278Z",
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
      "company_id": 20,
      "company": {
        "id": 20,
        "name": "Fake Company Name 19",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T17:48:40.287Z"
      },
      "created_at": "2016-11-03T17:48:40.290Z",
      "updated_at": "2016-11-03T17:48:40.290Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbb16629413e21c983e8c68d612c29f178adf01106af284f19b7dbb7938f89c8"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 26abd62cbb6256120db8f2fabaaed30f80a07736afd8f7866bcec6cde3933ebb
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T17:48:40.001Z"
      },
      "created_at": "2016-11-03T17:48:40.007Z",
      "updated_at": "2016-11-03T17:48:40.007Z",
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
      "company_id": 16,
      "company": {
        "id": 16,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T17:48:40.023Z"
      },
      "created_at": "2016-11-03T17:48:40.027Z",
      "updated_at": "2016-11-03T17:48:40.027Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26abd62cbb6256120db8f2fabaaed30f80a07736afd8f7866bcec6cde3933ebb"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 14a3e69e2cb8023c5cd661fa09e31fd920b9ae5c0f6a039d99d7fbcab30dc57a
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
      "id": 19,
      "created_at": "2016-11-03T17:48:50.170Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-11-03T17:48:50.279Z",
      "author_id": "876",
      "thread_subject_id": "279",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 20,
      "created_at": "2016-11-03T17:48:50.268Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 60,
      "updated_at": "2016-11-03T17:48:50.283Z",
      "author_id": "879",
      "thread_subject_id": "280",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 21,
      "created_at": "2016-11-03T17:48:50.667Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-03T17:48:50.667Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 22,
      "created_at": "2016-11-03T17:48:51.061Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-11-03T17:48:51.061Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 23,
      "created_at": "2016-11-03T17:48:51.461Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-11-03T17:48:51.461Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 24,
      "created_at": "2016-11-03T17:48:51.767Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 102,
      "updated_at": "2016-11-03T17:48:51.767Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-11-03T17:48:52.085Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 103,
      "updated_at": "2016-11-03T17:48:52.085Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 26,
      "created_at": "2016-11-03T17:48:52.407Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 104,
      "updated_at": "2016-11-03T17:48:52.407Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14a3e69e2cb8023c5cd661fa09e31fd920b9ae5c0f6a039d99d7fbcab30dc57a"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/18
Content-Type: application/json
Authorization: Bearer bcb650ddbe74eab3984def5271d50679bef3a9d6f9b20ca2fa22e6a073e64e5d
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-03T17:38:49.000Z"}}
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
    "id": 18,
    "created_at": "2016-11-03T17:48:49.957Z",
    "read_at": "2016-11-03T17:38:49.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-11-03T17:48:50.016Z",
    "author_id": "871",
    "thread_subject_id": "278",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/18" -d '{"notification":{"read_at":"2016-11-03T17:38:49.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcb650ddbe74eab3984def5271d50679bef3a9d6f9b20ca2fa22e6a073e64e5d"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4f04607379f291abf1ccf7d64b8ec6c96492298cfd7ad9b2ae6e242cb613e371
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
      "course_id": 272,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T17:48:49.128Z",
      "course_published": true,
      "updated_at": "2016-11-03T17:48:49.120Z"
    },
    {
      "id": 4,
      "course_id": 273,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T17:48:49.210Z",
      "course_published": true,
      "updated_at": "2016-11-03T17:48:49.202Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f04607379f291abf1ccf7d64b8ec6c96492298cfd7ad9b2ae6e242cb613e371"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 7891a332d78d8c66093ecba418ff9fd642871cc5d83b419f2042034d06ea7a5a
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
    "course_id": 277,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T17:48:49.778Z",
    "course_published": true,
    "updated_at": "2016-11-03T17:48:49.770Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7891a332d78d8c66093ecba418ff9fd642871cc5d83b419f2042034d06ea7a5a"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer af8250c28b52aa4c5d8511e625040e6d504191b9191f85d1f74f3c1ff7a50e4b
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
    "course_id": 276,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-03T17:48:49.676Z",
    "course_published": true,
    "updated_at": "2016-11-03T17:48:49.665Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af8250c28b52aa4c5d8511e625040e6d504191b9191f85d1f74f3c1ff7a50e4b"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 959530c6fcc998f7e7feaa86455fb16fd25604cb5d7d7c41d01ca4ca670e675c
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
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 57,
      "user_id": 598
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 58,
      "user_id": 598
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 598
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 60,
      "user_id": 598
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 959530c6fcc998f7e7feaa86455fb16fd25604cb5d7d7c41d01ca4ca670e675c"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/65
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
    "id": 65,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 63,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 65
      },
      {
        "id": 64,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 65
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/65" -X GET \
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
      "id": 63,
      "name": "Automated stable approach",
      "name_translations": {
        "en": "Automated stable approach"
      }
    },
    {
      "id": 64,
      "name": "Advanced tangible standardization",
      "name_translations": {
        "en": "Advanced tangible standardization"
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
PATCH /v2/feedbacks/14/close
Content-Type: application/json
Authorization: Bearer 69f064cf433b1641c3b586170bb98565a8ed051dc0981d4817909b0fa6583707
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
    "id": 14,
    "user_id": 655,
    "feedbackable_id": 61,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-03T17:48:32.132Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/14/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69f064cf433b1641c3b586170bb98565a8ed051dc0981d4817909b0fa6583707"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer c6d05aa40e2d414c3a73919790fb6e3dd8ad272edcfe7a300266f9be78525b0c
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
    "id": 12,
    "user_id": 645,
    "feedbackable_id": 59,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-03T17:48:31.397Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6d05aa40e2d414c3a73919790fb6e3dd8ad272edcfe7a300266f9be78525b0c"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/36
Content-Type: application/json
Authorization: Bearer c9e5d50877181a4738372c969ec5730313324481b0ad07072de927a6e7f25d9b
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
    "user_id": 751,
    "feedbackable_id": 64,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T17:48:39.323Z",
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
curl "api.goskive.com/v2/feedbacks/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9e5d50877181a4738372c969ec5730313324481b0ad07072de927a6e7f25d9b"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/10/fix
Content-Type: application/json
Authorization: Bearer cf1fe9d04c66507ef5d27724dc84a279699686ab871aebe24e15fc4f3f485887
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
curl "api.goskive.com/v2/feedbacks/10/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf1fe9d04c66507ef5d27724dc84a279699686ab871aebe24e15fc4f3f485887"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/11/fix
Content-Type: application/json
Authorization: Bearer cc6663122483c9c9e57fbc36695cadf8c0ccc13563dda90e736f08c95668ab17
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
curl "api.goskive.com/v2/feedbacks/11/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc6663122483c9c9e57fbc36695cadf8c0ccc13563dda90e736f08c95668ab17"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/close
Content-Type: application/json
Authorization: Bearer c503d161fe467869ab88474f825ce106d03dbd1e993bf6accf32a692d7495b7a
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
curl "api.goskive.com/v2/feedbacks/16/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c503d161fe467869ab88474f825ce106d03dbd1e993bf6accf32a692d7495b7a"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/37
Content-Type: application/json
Authorization: Bearer 355dda5561d2170e661eb2989f283d788702d69cdd6fffa57d2a61bf7bea1370
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
    "id": 37,
    "user_id": 756,
    "feedbackable_id": 65,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T17:48:39.629Z",
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
curl "api.goskive.com/v2/feedbacks/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 355dda5561d2170e661eb2989f283d788702d69cdd6fffa57d2a61bf7bea1370"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer c3b62cb2f040900eeb7da9af73356c353ee66bb8da5e34314da5e5afa89c3960
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
	-H "Authorization: Bearer c3b62cb2f040900eeb7da9af73356c353ee66bb8da5e34314da5e5afa89c3960"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/10/bookmark
Content-Type: application/json
Authorization: Bearer 63f99aae3c639c44b918f0fdf5b19f9181647a0642c64199e41f80cdcf278a26
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63f99aae3c639c44b918f0fdf5b19f9181647a0642c64199e41f80cdcf278a26"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer c734821e32b866abc6b548f0cffc655fed61fec543b668a9ec91a5958821154e
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
	-H "Authorization: Bearer c734821e32b866abc6b548f0cffc655fed61fec543b668a9ec91a5958821154e"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/11
Content-Type: application/json
Authorization: Bearer b4bdb272696ceffdc8d15df3a8ae7bd866e2e364d62b830b833600c372742787
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/81716d3d07935322640b233f5b2dbbf1.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T174824Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=5a31843dcf97aff8c870c9f652e99b0fc8d5fd7c7edc054eb72748e567042e1d",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4bdb272696ceffdc8d15df3a8ae7bd866e2e364d62b830b833600c372742787"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/13/preview
Content-Type: application/json
Authorization: Bearer fe493edfb730401a48cb4599f8f6ec0aabc9156ed348ade678e30ab0aa93474c
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/a4792b8f815cceca9e6567e879f29319.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T174825Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=49fc43dce697db1fec5a29873c48179802945739a9674a709d63b35eccc3b3b2",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/13/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe493edfb730401a48cb4599f8f6ec0aabc9156ed348ade678e30ab0aa93474c"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer dc5ec245eab61216c194934b7abc9b2a96b04bdcdde926750faa80a0357948b8
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
      "id": 542,
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
      "created_at": "2016-11-03T17:48:24.277Z",
      "updated_at": "2016-11-03T17:48:24.277Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-03T17:48:24.357Z",
    "updated_at": "2016-11-03T17:48:24.357Z",
    "course_id": 194,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc5ec245eab61216c194934b7abc9b2a96b04bdcdde926750faa80a0357948b8"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer 4437f98ef0c3e4b9193fe96265aaf4b4d2d9c7228aaf232c6283f41d73c82419
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
      "creator_id": 358,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 121,
      "additional_university_ids": [

      ],
      "topic_id": 118,
      "discipline_id": 119,
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
      "chapters_updated_at": "2016-11-03T17:48:03.372Z",
      "updated_at": "2016-11-03T17:48:05.274Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 363,
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-58474650-09d3-4f6c-8ec3-623a5d87c05f",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-58474650-09d3-4f6c-8ec3-623a5d87c05f",
      "slug": "mit-the-great-british-bake-off-58474650-09d3-4f6c-8ec3-623a5d87c05f",
      "university_id": 122,
      "additional_university_ids": [

      ],
      "topic_id": 119,
      "discipline_id": 120,
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
      "chapters_updated_at": "2016-11-03T17:48:03.372Z",
      "updated_at": "2016-11-03T17:48:05.929Z",
      "shortname": "mit-the-great-british-bake-off-58474650-09d3-4f6c-8ec3-623a5d87c05f"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 4437f98ef0c3e4b9193fe96265aaf4b4d2d9c7228aaf232c6283f41d73c82419"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/19/download
Content-Type: application/json
Authorization: Bearer 2532b1156f5e079b3230f7ca206a0fd10de878b1be9e6ac56b0d775e5f763e89
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2532b1156f5e079b3230f7ca206a0fd10de878b1be9e6ac56b0d775e5f763e89"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/17/report
Content-Type: application/json
Authorization: Bearer c92bef82e7630327f3826201917aad4fdbfc36423b12508042b3f05ac01cf086
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c92bef82e7630327f3826201917aad4fdbfc36423b12508042b3f05ac01cf086"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer 8ee50d83076314af178ce047f28fb026aa5f902305416aec30d628a9d5bd4499
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ee50d83076314af178ce047f28fb026aa5f902305416aec30d628a9d5bd4499"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/18/upvote
Content-Type: application/json
Authorization: Bearer 3ac7ffbd0e866b77db235db6eb5e21d245a0e562eafa511031a2d443094fee94
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ac7ffbd0e866b77db235db6eb5e21d245a0e562eafa511031a2d443094fee94"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/46/comments
Content-Type: application/json
Authorization: Bearer 7ccb35e3c0203f805fe881bc027c934f5b84464835dd900a9c24bb41e5d09ec5
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
    "id": 46,
    "author_id": 444,
    "reply_to_id": null,
    "created_at": "2016-11-03T17:48:13.630Z",
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
curl "api.goskive.com/v2/flashcards/46/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ccb35e3c0203f805fe881bc027c934f5b84464835dd900a9c24bb41e5d09ec5"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/47/comments
Content-Type: application/json
Authorization: Bearer 04246a876b6344f8d3e3d92c311a8c478b6e0a5892cae418418610c9d2458b0e
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
    "id": 47,
    "author_id": 447,
    "reply_to_id": null,
    "created_at": "2016-11-03T17:48:14.002Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 447,
      "feedbackable_id": 47,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:13.997Z",
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
curl "api.goskive.com/v2/flashcards/47/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04246a876b6344f8d3e3d92c311a8c478b6e0a5892cae418418610c9d2458b0e"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/45/comments
Content-Type: application/json
Authorization: Bearer 6f48f5755d8e0cca59d151cef75011cd67efd43c155a83a6e601522b3480207d
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
      "id": 44,
      "author_id": 442,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:48:13.392Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 443,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:48:13.411Z",
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
curl "api.goskive.com/v2/flashcards/45/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f48f5755d8e0cca59d151cef75011cd67efd43c155a83a6e601522b3480207d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/48/comments
Content-Type: application/json
Authorization: Bearer 5b856ab498a9e6727e797e682e4424c7ca8e0cf0b2dab3ce215983b7b446d30f
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
curl "api.goskive.com/v2/flashcards/48/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b856ab498a9e6727e797e682e4424c7ca8e0cf0b2dab3ce215983b7b446d30f"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/4/feedbacks
Content-Type: application/json
Authorization: Bearer e7e63e7417d9c60bb116beb9d5a8aa7668ba336e75c892b167ab5f3d79ec8171
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
    "id": 1,
    "user_id": 85,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T17:47:45.651Z",
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
curl "api.goskive.com/v2/flashcards/4/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7e63e7417d9c60bb116beb9d5a8aa7668ba336e75c892b167ab5f3d79ec8171"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/6/feedbacks
Content-Type: application/json
Authorization: Bearer 9b963755980c540db1ea65c379f53ccaedd6a20ccd4765e96df816d1eb6c062c
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
      "user_id": 95,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:47:46.570Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 94,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:47:46.557Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/6/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b963755980c540db1ea65c379f53ccaedd6a20ccd4765e96df816d1eb6c062c"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/55/votes
Content-Type: application/json
Authorization: Bearer c82389a5c37a9b37357c3a9fdaa97560153fe41dd6807244a8a255b5e46e1da9
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 55,
      "user_id": 620
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 55,
      "user_id": 619
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 55,
      "user_id": 618
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/55/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c82389a5c37a9b37357c3a9fdaa97560153fe41dd6807244a8a255b5e46e1da9"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/17/republish
Content-Type: application/json
Authorization: Bearer ebc441ceb2ef310d054743d87c835c3628eb4096a44b8972ac4a88fa4bc54fa4
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
curl "api.goskive.com/v2/flashcards/17/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebc441ceb2ef310d054743d87c835c3628eb4096a44b8972ac4a88fa4bc54fa4"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/14/bookmark
Content-Type: application/json
Authorization: Bearer 77db9dd0c03c98cfdb1d80b2c0b0ea790c316866e43eb73dbdd81be15779ccb7
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/14/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77db9dd0c03c98cfdb1d80b2c0b0ea790c316866e43eb73dbdd81be15779ccb7"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/15
Content-Type: application/json
Authorization: Bearer 954e677f0cd9a50e84947b418ebaa141acbeb98bc1ffe9067fd51067ed02a1fb
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 954e677f0cd9a50e84947b418ebaa141acbeb98bc1ffe9067fd51067ed02a1fb"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/12/downvote
Content-Type: application/json
Authorization: Bearer be13c5c9ebba37c9cc4819ea89394970258d52506af39d4734b6f1d7eafb4b42
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/12/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be13c5c9ebba37c9cc4819ea89394970258d52506af39d4734b6f1d7eafb4b42"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/13
Content-Type: application/json
Authorization: Bearer f1febc4a8ab7351552e718ec93c1a4a7f055b50e15f88707cdcfb74c4664444a
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 138,
    "chapter_id": 37,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:47:49.040Z",
    "created_at": "2016-11-03T17:47:49.040Z",
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
curl "api.goskive.com/v2/flashcards/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1febc4a8ab7351552e718ec93c1a4a7f055b50e15f88707cdcfb74c4664444a"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/19/report
Content-Type: application/json
Authorization: Bearer a15101effe0241ce6244e756c9819ab57ad59863d800ff436cd4e369dc1aa8d3
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a15101effe0241ce6244e756c9819ab57ad59863d800ff436cd4e369dc1aa8d3"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/35/bookmark
Content-Type: application/json
Authorization: Bearer 56df10b9f2f08774b69905bfe18fa6e4b098a03fda6e62dc3554f0c236fef50a
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56df10b9f2f08774b69905bfe18fa6e4b098a03fda6e62dc3554f0c236fef50a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/16/upvote
Content-Type: application/json
Authorization: Bearer 7ea088c039004427282ea23f316a4f4d59f25900ac6faa2bf1b9520a150e2643
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ea088c039004427282ea23f316a4f4d59f25900ac6faa2bf1b9520a150e2643"
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
    "key": "cache/b41cc0b90a46f18676f34403a71b31c9.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxODo0ODozMFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I0MWNjMGI5MGE0NmYxODY3NmYzNDQwM2E3MWIzMWM5LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwMy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDNUMTc0ODMwWiJ9XX0=",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T174830Z",
    "x-amz-signature": "57efdf701b4ebc675dfe7f7b515c71d701ca0887ec4c8cb606e627fe9518a794"
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
Authorization: Bearer 2340df5e35aadfaa5c275d31e5abe0eb2307fd4c80797677df224a5e0005b44f
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
	-H "Authorization: Bearer 2340df5e35aadfaa5c275d31e5abe0eb2307fd4c80797677df224a5e0005b44f"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 0ed51869e08a2ac337ce6c67622d563511bcf415aa09f2af8210b654515cff7c
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
	-H "Authorization: Bearer 0ed51869e08a2ac337ce6c67622d563511bcf415aa09f2af8210b654515cff7c"
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
{"password":{"reset_password_token":"rur6XqGkrhpiTxVqKgvk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 377,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-03T17:48:07.555Z",
  "updated_at": "2016-11-03T17:48:07.698Z",
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
  "audit_id": 4320
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"rur6XqGkrhpiTxVqKgvk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/84/comments
Content-Type: application/json
Authorization: Bearer 1e5459be4cce801a055d53070a254e950cbba4ae5320073d8d9483470d628490
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
    "id": 55,
    "author_id": 781,
    "reply_to_id": null,
    "created_at": "2016-11-03T17:48:42.794Z",
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
curl "api.goskive.com/v2/questions/84/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e5459be4cce801a055d53070a254e950cbba4ae5320073d8d9483470d628490"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/83/comments
Content-Type: application/json
Authorization: Bearer 563356befcdc4c83b893769bda9f68b0354ccf7c8dd7bb002b965fae22a76121
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
    "id": 54,
    "author_id": 778,
    "reply_to_id": null,
    "created_at": "2016-11-03T17:48:42.264Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 778,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:42.261Z",
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
curl "api.goskive.com/v2/questions/83/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 563356befcdc4c83b893769bda9f68b0354ccf7c8dd7bb002b965fae22a76121"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/80/comments
Content-Type: application/json
Authorization: Bearer 6c31ac51e14cabd1a1eb41ef60f31f57cbf51e9557b7be262c9cc590c2cf2e7b
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
      "id": 53,
      "author_id": 771,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:48:41.207Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 770,
      "reply_to_id": null,
      "created_at": "2016-11-03T17:48:41.189Z",
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
curl "api.goskive.com/v2/questions/80/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c31ac51e14cabd1a1eb41ef60f31f57cbf51e9557b7be262c9cc590c2cf2e7b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/82/comments
Content-Type: application/json
Authorization: Bearer ae8f1aa0e8821ae509af43927e1ff6f631a0359f8173f7837e49b9f483065b43
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
	-H "Authorization: Bearer ae8f1aa0e8821ae509af43927e1ff6f631a0359f8173f7837e49b9f483065b43"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/92/feedbacks
Content-Type: application/json
Authorization: Bearer f3d9e23bacfbc1d96ac2492cebbe8cee5229d5b3b6701c6ca82df7160bf9117a
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
    "user_id": 817,
    "feedbackable_id": 92,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-03T17:48:45.824Z",
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
curl "api.goskive.com/v2/questions/92/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3d9e23bacfbc1d96ac2492cebbe8cee5229d5b3b6701c6ca82df7160bf9117a"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/88/feedbacks
Content-Type: application/json
Authorization: Bearer fd7d4d3194c3e2972c5e7b82780409b197119dc3439879fd472ffe8a2d15c742
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
      "id": 42,
      "user_id": 805,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:44.322Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 804,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T17:48:44.311Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/88/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd7d4d3194c3e2972c5e7b82780409b197119dc3439879fd472ffe8a2d15c742"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/133/votes
Content-Type: application/json
Authorization: Bearer 27b50e49940474518be40e7d78f22251c02609a818192e94c5fec488d3273e34
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 985
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 984
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 983
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/133/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27b50e49940474518be40e7d78f22251c02609a818192e94c5fec488d3273e34"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/53/republish
Content-Type: application/json
Authorization: Bearer 7fb002d9583751681ff6c90c8946a73cda2a2bceceda1ea871ca2bda6a043ff2
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
curl "api.goskive.com/v2/questions/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7fb002d9583751681ff6c90c8946a73cda2a2bceceda1ea871ca2bda6a043ff2"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/35/bookmark
Content-Type: application/json
Authorization: Bearer 89acdd661cf7facddd7b020dd777e878509e6a60ebc3d3dd2a9b57af3a576b6e
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/35/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89acdd661cf7facddd7b020dd777e878509e6a60ebc3d3dd2a9b57af3a576b6e"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/33
Content-Type: application/json
Authorization: Bearer 262e57e07a02f97f1a632b7fb687be7de9a0bf3b17bb7bcd54e6f9c08f277d2f
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/33" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 262e57e07a02f97f1a632b7fb687be7de9a0bf3b17bb7bcd54e6f9c08f277d2f"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/31/downvote
Content-Type: application/json
Authorization: Bearer 4761d5f00266bfe6237805bc232eab90b2c8175e835ec8c0933e34f93b66ffcb
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4761d5f00266bfe6237805bc232eab90b2c8175e835ec8c0933e34f93b66ffcb"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/36
Content-Type: application/json
Authorization: Bearer dcc1fe0f8f268290be2d8e31f33f7adc3f94be2ed1af57e6b6dd9a53db25d83c
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
    "id": 36,
    "obfuscated_id": "01Tx8eTrCOA",
    "author_id": 471,
    "chapter_id": 92,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:17.437Z",
    "created_at": "2016-11-03T17:48:17.309Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 75,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 76,
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
curl "api.goskive.com/v2/questions/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcc1fe0f8f268290be2d8e31f33f7adc3f94be2ed1af57e6b6dd9a53db25d83c"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/30/report
Content-Type: application/json
Authorization: Bearer 04f32681dda8b5b710b14e49dddcdc743abff6d2e8f460fc4c1665729b93063d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/30/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04f32681dda8b5b710b14e49dddcdc743abff6d2e8f460fc4c1665729b93063d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/34/bookmark
Content-Type: application/json
Authorization: Bearer cc4d8097032823d6e810933fcdc47854873d19b39e7dcfd016ed07aa6a27a154
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc4d8097032823d6e810933fcdc47854873d19b39e7dcfd016ed07aa6a27a154"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/32
Content-Type: application/json
Authorization: Bearer 0b166e9195751bb9ed8b461c598bde5ff636803fb9e9602275e9b957dc391587
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T17:48:15.365Z","updated_at":"2016-11-03T17:48:15.489Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":88,"author_id":459,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 459,
    "chapter_id": 88,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T17:48:15.604Z",
    "created_at": "2016-11-03T17:48:15.365Z",
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
    "question": "{\"id\"=>32, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-03T17:48:15.365Z\", \"updated_at\"=>\"2016-11-03T17:48:15.489Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>88, \"author_id\"=>459, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 68,
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
curl "api.goskive.com/v2/questions/32" -d '{"question":{"question":{"id":32,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T17:48:15.365Z","updated_at":"2016-11-03T17:48:15.489Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":88,"author_id":459,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b166e9195751bb9ed8b461c598bde5ff636803fb9e9602275e9b957dc391587"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/54/upvote
Content-Type: application/json
Authorization: Bearer de7d68f893456a691f76f5eed1b154e612fa2c99a744e43eb1b820d87548f9ce
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/54/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de7d68f893456a691f76f5eed1b154e612fa2c99a744e43eb1b820d87548f9ce"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7b66841ff6c3d44af2f1e8b7ecdabd63c69bd6e8fda915f064104ec8cb9387a0
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
      "creator_id": 903,
      "id": 288,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 271,
      "additional_university_ids": [

      ],
      "topic_id": 297,
      "discipline_id": 298,
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
      "updated_at": "2016-11-03T17:48:52.620Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b66841ff6c3d44af2f1e8b7ecdabd63c69bd6e8fda915f064104ec8cb9387a0"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 9c823bc36fd3e46791e6ae20131e506148232c0185d1aa717764424919e97fd3
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
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-254",
      "html_url": "https://goskive.com/university/uni-254",
      "slug": "uni-254",
      "name": "National School of Pizza",
      "short_name": "Uni 254",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5aa26f7e4f52a3698c45d9eb3b26ed17d370ea61.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3d90cf539c5651617f18a342d537fae964163306.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T17:48:52.880Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-253",
      "html_url": "https://goskive.com/university/uni-253",
      "slug": "uni-253",
      "name": "National School of Pastry",
      "short_name": "Uni 253",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/95ce47863c09564fb1d903d45e32265f58fad291.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b8ba0e50ec9e8506a381b04b02de55954f460524.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T17:48:52.862Z",
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
	-H "Authorization: Bearer 9c823bc36fd3e46791e6ae20131e506148232c0185d1aa717764424919e97fd3"
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
      "id": 303,
      "name": "Synchronised bi-directional standardization",
      "name_translations": {
        "en": "Synchronised bi-directional standardization"
      },
      "discipline_id": 304
    },
    {
      "id": 304,
      "name": "Open-architected even-keeled secured line",
      "name_translations": {
        "en": "Open-architected even-keeled secured line"
      },
      "discipline_id": 305
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
GET /v2/topics/305
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
    "id": 305,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 306
  }
}
```



```shell
curl "api.goskive.com/v2/topics/305" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 2b2cf05b8d656d8d29c676edbe56964917bae21cccb9a5ca83d3345f71279844
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
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-63",
      "html_url": "https://goskive.com/university/uni-63",
      "slug": "uni-63",
      "name": "University 38",
      "short_name": "Uni 63",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f0455cb406a50dfa205f9dfc8a84dec6ed607634.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ee88380d46739e088ac23d7ad0ef1eb91c7c5fb1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T17:47:53.840Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-64",
      "html_url": "https://goskive.com/university/uni-64",
      "slug": "uni-64",
      "name": "University 39",
      "short_name": "Uni 64",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/34ae0a587d54bcfff28a891b60e4ff558b06fe03.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/82b731c89e2f272b7201803005596c5d91004739.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T17:47:53.856Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 65,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-65",
      "html_url": "https://goskive.com/university/uni-65",
      "slug": "uni-65",
      "name": "University 40",
      "short_name": "Uni 65",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0b554848511eb0c693e5b33d9e9f705745f9f331.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/fabb93546afe8266713ab5e9a36016b55dab1bfd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T17:47:53.874Z",
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
	-H "Authorization: Bearer 2b2cf05b8d656d8d29c676edbe56964917bae21cccb9a5ca83d3345f71279844"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 560009cedd6df22f9281538f1459fc2f66fcb60f80b0353caca5256bc137e459
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
    "id": 67,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9f2d41a18511a2bab0b208f8d4f94d96036b52a5.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/008381d2042e430be1fc7c898823f8fcf7e9cf5f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-03T17:47:54.000Z",
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
	-H "Authorization: Bearer 560009cedd6df22f9281538f1459fc2f66fcb60f80b0353caca5256bc137e459"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 54d571a7d0706686b9e53c8c9d15c0c397094ea3d2ae63717dda5d5b6b739d69
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":158,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 421,
    "id": 156,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 139,
    "additional_university_ids": [

    ],
    "topic_id": 158,
    "discipline_id": 159,
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
    "chapters_updated_at": "2016-11-03T17:48:11.877Z",
    "updated_at": "2016-11-03T17:48:12.023Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 78,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-11-03T17:48:11.971Z",
        "course_id": 156,
        "author_id": 421,
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
        "id": 79,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-11-03T17:48:11.990Z",
        "course_id": 156,
        "author_id": 421,
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
        "id": 80,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-11-03T17:48:12.011Z",
        "course_id": 156,
        "author_id": 421,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":158,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54d571a7d0706686b9e53c8c9d15c0c397094ea3d2ae63717dda5d5b6b739d69"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f969118b126eb9e77536a2fd81bd5668ccb6b0be36a7e1750d01146d5599f5b5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":159,"published":false}}
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
    "creator_id": 422,
    "id": 157,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 140,
    "additional_university_ids": [

    ],
    "topic_id": 159,
    "discipline_id": 160,
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
    "updated_at": "2016-11-03T17:48:12.180Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":159,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f969118b126eb9e77536a2fd81bd5668ccb6b0be36a7e1750d01146d5599f5b5"
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
      "creator_id": 384,
      "id": 125,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-88",
      "html_url": "https://goskive.com/course/fu-course-88",
      "slug": "fu-course-88",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 127,
      "discipline_id": 128,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 88",
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
      "updated_at": "2016-11-03T17:48:08.256Z",
      "shortname": "fu-course-88"
    },
    {
      "creator_id": 384,
      "id": 126,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-89",
      "html_url": "https://goskive.com/course/fu-course-89",
      "slug": "fu-course-89",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 128,
      "discipline_id": 129,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
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
      "chapters_updated_at": "2016-11-03T17:48:08.612Z",
      "updated_at": "2016-11-03T17:48:08.621Z",
      "shortname": "fu-course-89"
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
Authorization: Bearer 1b198473654f615c8fe7cd8fbb075a2bf0c96f86208e1b1763c23069e6c13a51
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
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-112",
      "html_url": "https://goskive.com/course/fu-course-112",
      "slug": "fu-course-112",
      "university_id": 135,
      "additional_university_ids": [

      ],
      "topic_id": 151,
      "discipline_id": 152,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 112",
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
      "updated_at": "2016-11-03T17:48:10.996Z",
      "shortname": "fu-course-112"
    },
    {
      "creator_id": 411,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-113",
      "html_url": "https://goskive.com/course/fu-course-113",
      "slug": "fu-course-113",
      "university_id": 135,
      "additional_university_ids": [

      ],
      "topic_id": 152,
      "discipline_id": 153,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 113",
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
      "chapters_updated_at": "2016-11-03T17:48:11.343Z",
      "updated_at": "2016-11-03T17:48:11.351Z",
      "shortname": "fu-course-113"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b198473654f615c8fe7cd8fbb075a2bf0c96f86208e1b1763c23069e6c13a51"
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
      "creator_id": 389,
      "id": 129,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-92",
      "html_url": "https://goskive.com/course/fu-course-92",
      "slug": "fu-course-92",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "topic_id": 131,
      "discipline_id": 132,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 92",
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
      "updated_at": "2016-11-03T17:48:08.850Z",
      "shortname": "fu-course-92"
    },
    {
      "creator_id": 389,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-93",
      "html_url": "https://goskive.com/course/fu-course-93",
      "slug": "fu-course-93",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "topic_id": 132,
      "discipline_id": 133,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 93",
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
      "updated_at": "2016-11-03T17:48:08.894Z",
      "shortname": "fu-course-93"
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
Authorization: Bearer 7b67ed6c03abce2548364966afb52f4cd30553480aeae93fb7182a2b82447285
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
      "creator_id": 417,
      "id": 153,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-116",
      "html_url": "https://goskive.com/course/fu-course-116",
      "slug": "fu-course-116",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 155,
      "discipline_id": 156,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 116",
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
      "updated_at": "2016-11-03T17:48:11.581Z",
      "shortname": "fu-course-116"
    },
    {
      "creator_id": 417,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-117",
      "html_url": "https://goskive.com/course/fu-course-117",
      "slug": "fu-course-117",
      "university_id": 136,
      "additional_university_ids": [

      ],
      "topic_id": 156,
      "discipline_id": 157,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 117",
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
      "updated_at": "2016-11-03T17:48:11.623Z",
      "shortname": "fu-course-117"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b67ed6c03abce2548364966afb52f4cd30553480aeae93fb7182a2b82447285"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 9648c5cb5ef2ae71ef975441041807eb4dcd9590384baba03a184d42c9e3fc8d
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
  "id": 760,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-03T17:48:39.720Z",
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
	-H "Authorization: Bearer 9648c5cb5ef2ae71ef975441041807eb4dcd9590384baba03a184d42c9e3fc8d"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/624
Content-Type: application/json
Authorization: Bearer f166c3f36d773791c6ee6a4d35eb3b2f09fe17cf81031dd28adb648d2defe2a1
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
    "id": 624,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 202,
    "fields_of_study": [
      226,
      227
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-03T17:48:30.371Z",
    "updated_at": "2016-11-03T17:48:30.371Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/624" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f166c3f36d773791c6ee6a4d35eb3b2f09fe17cf81031dd28adb648d2defe2a1"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/626
Content-Type: application/json
Authorization: Bearer c1d19ecca944b9921459bf082eac42b2bb2b400bad1300f835c821d67430be6a
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
    "id": 626,
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
    "created_at": "2016-11-03T17:48:30.463Z",
    "updated_at": "2016-11-03T17:48:30.463Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/626" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1d19ecca944b9921459bf082eac42b2bb2b400bad1300f835c821d67430be6a"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/2
Content-Type: application/json
Authorization: Bearer 40dfe8dca3f988fc02ff93768e055e3179c61424d32e962e4522bffc0fbdacaa
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40dfe8dca3f988fc02ff93768e055e3179c61424d32e962e4522bffc0fbdacaa"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/1
Content-Type: application/json
Authorization: Bearer 1fb7777cfa5bbddfa6c747fca5c562b67bfe058834d259a4c9335a72dbfc7e0e
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
    "id": 1,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 4,
    "user_id": 73
  }
}
```



```shell
curl "api.goskive.com/v2/votes/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fb7777cfa5bbddfa6c747fca5c562b67bfe058834d259a4c9335a72dbfc7e0e"
```
