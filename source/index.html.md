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
Authorization: Basic ZTYwMGRkMDM5ZWE5MWNmMTAyOTJkN2Y5MzE2NjkwNTYxYzU1ZTllOWFhN2Ew
OTUxYjhjMGEyYjdiOWNjNGYyYTowZjEwMzQ0NWU2MzE4MjVhOGVhMjc5ZmU2
YmYzZjRkZmU5NTRkMTRiNDMwZjU2OTQyNjdiZDgyZDEyMGRkZTRi

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
	-u e600dd039ea91cf10292d7f9316690561c55e9e9aa7a0951b8c0a2b7b9cc4f2a:0f103445e631825a8ea279fe6bf3f4dfe954d14b430f5694267bd82d120dde4b
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"65afee76296e4e7bbbaf0e5b90badacdbb25817139e8977ba1c3293b03e684a6","client_secret":"ab88bffcbb899af2ccb784057844a5fcb068a74a9516a0d013c4de13489aba94"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"65afee76296e4e7bbbaf0e5b90badacdbb25817139e8977ba1c3293b03e684a6","client_secret":"ab88bffcbb899af2ccb784057844a5fcb068a74a9516a0d013c4de13489aba94"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NGY5YTdmZDlkZTI1NmJkNzYwODkwNmUyN2UxNjgzYjBjMTVjMmEzNWMzNTc4
ZWJlODAzYTZkNzdhZjg5MzZmMzpkMTJkNmFjMjAxNWI3MmE5NGFmMTFlMjNi
NTFlODkxNGU0YjMxNGI0YzdkZmE1Y2YxMmQ3Mzc0N2VmZmQ4NmYw

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
  "access_token": "bfe2786d384c792934d63b2ee9c8f1fbfc7d624ccbfee0ba3f49fedc45e197c6",
  "token_type": "bearer",
  "created_at": 1481831399
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 4f9a7fd9de256bd7608906e27e1683b0c15c2a35c3578ebe803a6d77af8936f3:d12d6ac2015b72a94af11e23b51e8914e4b314b4c7dfa5cf12d73747effd86f0
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7debad29cd84b410f28a3f7a14234204adc00a5f38caf3983983cee4200668cb","client_secret":"c6e76ec352f94154d142d009cbf86e846d785c72111372cda24107277384a995"}
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
  "access_token": "0f38799b69730c6811a2d4e3622dfc8adf50d08bbb95572ba4b2420301050374",
  "token_type": "bearer",
  "created_at": 1481831399
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7debad29cd84b410f28a3f7a14234204adc00a5f38caf3983983cee4200668cb","client_secret":"c6e76ec352f94154d142d009cbf86e846d785c72111372cda24107277384a995"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"f1e93529dabacaabbd8b2dff27c8c9dd7e4f2392543a1bf9de0c2595c1e665ae","client_secret":"4828687c0c50bd5ea62e9d3e4c6b5136cc5b4992bbbeb5305053ba6abda40581"}
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
  "access_token": "4e6de516a7fcdbce8b7c0686d221d2db5023c65ceefd1e5f0737d1162c6a1801",
  "token_type": "bearer",
  "created_at": 1481831399
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"f1e93529dabacaabbd8b2dff27c8c9dd7e4f2392543a1bf9de0c2595c1e665ae","client_secret":"4828687c0c50bd5ea62e9d3e4c6b5136cc5b4992bbbeb5305053ba6abda40581"}' -X POST \
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
GET /v2/campaigns/4
Content-Type: application/json
Authorization: Bearer eef610bc6d39c3781e7507ac76e7fb6e730bf4bfe917e970af61ca13d6295f26
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
    "id": 4,
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
curl "api.goskive.com/v2/campaigns/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eef610bc6d39c3781e7507ac76e7fb6e730bf4bfe917e970af61ca13d6295f26"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/159/flashcards
Content-Type: application/json
Authorization: Bearer 0c0708d6510d861bdbb414a5aa48d1770c9a4c60b82ef4b715d7d2c3821ef832
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":159,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 85,
    "obfuscated_id": "xR5KgQjIo2Y",
    "author_id": 794,
    "chapter_id": 159,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:50:22.290Z",
    "created_at": "2016-12-15T19:50:22.290Z",
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
curl "api.goskive.com/v2/chapters/159/flashcards" -d '{"flashcard":{"chapter_id":159,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c0708d6510d861bdbb414a5aa48d1770c9a4c60b82ef4b715d7d2c3821ef832"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/158/flashcards
Content-Type: application/json
Authorization: Bearer 5f8e56c0d7b9bd7a2cbd4293970b0a8fc8151dd1ba8421fc8bed13e4c9303334
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
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 789,
      "chapter_id": 158,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:50:21.946Z",
      "created_at": "2016-12-15T19:50:21.946Z",
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
      "author_id": 789,
      "chapter_id": 158,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:50:21.988Z",
      "created_at": "2016-12-15T19:50:21.988Z",
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
      "id": 84,
      "obfuscated_id": "Hu6DTUHzhWo",
      "author_id": 789,
      "chapter_id": 158,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:50:22.029Z",
      "created_at": "2016-12-15T19:50:22.029Z",
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
curl "api.goskive.com/v2/chapters/158/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f8e56c0d7b9bd7a2cbd4293970b0a8fc8151dd1ba8421fc8bed13e4c9303334"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/76/questions
Content-Type: application/json
Authorization: Bearer 651bca8e45e2bd3f89641e513931406f46ff350da5bd5b962e39e1e3d0c8377c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":76,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 52,
    "obfuscated_id": "_rmh4zxMC_8",
    "author_id": 280,
    "chapter_id": 76,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:35.337Z",
    "created_at": "2016-12-15T19:49:35.337Z",
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
        "id": 104,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 105,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 106,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 107,
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
curl "api.goskive.com/v2/chapters/76/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":76,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 651bca8e45e2bd3f89641e513931406f46ff350da5bd5b962e39e1e3d0c8377c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/75/questions
Content-Type: application/json
Authorization: Bearer ef54b504a607298434cf4854009a3e51d8313513823f0278b7c6f89d1e9633bd
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":75,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 51,
    "obfuscated_id": "fXx2Zpse_KI",
    "author_id": 277,
    "chapter_id": 75,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:34.730Z",
    "created_at": "2016-12-15T19:49:34.730Z",
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
        "id": 102,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 103,
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
curl "api.goskive.com/v2/chapters/75/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":75,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef54b504a607298434cf4854009a3e51d8313513823f0278b7c6f89d1e9633bd"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/77/questions
Content-Type: application/json
Authorization: Bearer 158463b0b70e67c71c4319d1622b9e59769b8113343e6f1c9fb68e10036b8993
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":77,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 53,
    "obfuscated_id": "XffxqHkTsbc",
    "author_id": 283,
    "chapter_id": 77,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:36.047Z",
    "created_at": "2016-12-15T19:49:36.047Z",
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
        "id": 108,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 109,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/77/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":77,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 158463b0b70e67c71c4319d1622b9e59769b8113343e6f1c9fb68e10036b8993"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/78/questions
Content-Type: application/json
Authorization: Bearer 0beb58cc5e537f998263c27f2c92c733d79fb2afaee94daa0f34117a046908d9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":78,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 54,
    "obfuscated_id": "cKxlQSpHm5w",
    "author_id": 286,
    "chapter_id": 78,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:36.649Z",
    "created_at": "2016-12-15T19:49:36.649Z",
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
        "id": 110,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 111,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 112,
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
curl "api.goskive.com/v2/chapters/78/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":78,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0beb58cc5e537f998263c27f2c92c733d79fb2afaee94daa0f34117a046908d9"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/79/questions
Content-Type: application/json
Authorization: Bearer 105d3c582faaddd693ba8fca04c13a9724f6acea236182df4a08d80c1c3c0d01
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
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 289,
      "chapter_id": 79,
      "position": 42,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:49:37.234Z",
      "created_at": "2016-12-15T19:49:37.131Z",
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
          "id": 113,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 114,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 290,
      "chapter_id": 79,
      "position": 43,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:49:37.414Z",
      "created_at": "2016-12-15T19:49:37.310Z",
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
          "id": 115,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 116,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 291,
      "chapter_id": 79,
      "position": 44,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T19:49:37.593Z",
      "created_at": "2016-12-15T19:49:37.488Z",
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
          "id": 117,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 118,
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
curl "api.goskive.com/v2/chapters/79/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 105d3c582faaddd693ba8fca04c13a9724f6acea236182df4a08d80c1c3c0d01"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/117
Content-Type: application/json
Authorization: Bearer c51adbe89313b28857f5cc7d849868756855db301a0bb6f942b311468e90ec4a
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
curl "api.goskive.com/v2/chapters/117" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c51adbe89313b28857f5cc7d849868756855db301a0bb6f942b311468e90ec4a"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/119
Content-Type: application/json
Authorization: Bearer 43c3dd16a7bdfaa3b61865fb5b9d358803233d11eece757e8612cf85b38c590e
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
curl "api.goskive.com/v2/chapters/119" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43c3dd16a7bdfaa3b61865fb5b9d358803233d11eece757e8612cf85b38c590e"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/114
Content-Type: application/json
Authorization: Bearer 02d0cc72542c467d211e20224c3d7eaa6bf03c7586851aa36e6099239c8a2cf6
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
curl "api.goskive.com/v2/chapters/114" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02d0cc72542c467d211e20224c3d7eaa6bf03c7586851aa36e6099239c8a2cf6"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/120
Content-Type: application/json
Authorization: Bearer d0acb0639d0d6b3abc107a0636e3758c30f0dd8ce79d0d15c572a48f9ae84565
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/120" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0acb0639d0d6b3abc107a0636e3758c30f0dd8ce79d0d15c572a48f9ae84565"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/122
Content-Type: application/json
Authorization: Bearer da35ce5d62a21917522b545e9e5e8aa98e18d80927a21486d6be339669e7cc4f
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
    "id": 122,
    "updated_at": "2016-12-15T19:49:59.623Z",
    "course_id": 145,
    "author_id": 512,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T19:49:59.136Z",
    "questions_updated_at": "2016-12-15T19:49:59.136Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 516,
        "chapter_id": 122,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:59.606Z",
        "created_at": "2016-12-15T19:49:59.606Z",
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
        "id": 101,
        "obfuscated_id": "PprZyBVq_gc",
        "author_id": 514,
        "chapter_id": 122,
        "position": 88,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:59.506Z",
        "created_at": "2016-12-15T19:49:59.423Z",
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
            "id": 205,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 206,
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
curl "api.goskive.com/v2/chapters/122" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da35ce5d62a21917522b545e9e5e8aa98e18d80927a21486d6be339669e7cc4f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/116
Content-Type: application/json
Authorization: Bearer e8f591499ad4ac9f1419a15b085eed6fa112ff6b22be33364cd2e51d6babe11f
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
    "id": 116,
    "updated_at": "2016-12-15T19:49:57.485Z",
    "course_id": 139,
    "author_id": 491,
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
curl "api.goskive.com/v2/chapters/116" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8f591499ad4ac9f1419a15b085eed6fa112ff6b22be33364cd2e51d6babe11f"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/8/replies
Content-Type: application/json
Authorization: Bearer fc6f6668bf8d045ad15a922b28c8c3240f1bec622344349759a38ad822d1fbe7
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
    "id": 9,
    "author_id": 254,
    "reply_to_id": 8,
    "created_at": "2016-12-15T19:49:32.027Z",
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
curl "api.goskive.com/v2/comments/8/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc6f6668bf8d045ad15a922b28c8c3240f1bec622344349759a38ad822d1fbe7"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/7/replies
Content-Type: application/json
Authorization: Bearer 3f23f87f677cbb02a804b9b67830ba6eb3b3a7f13593cb218cbc9a237449ee95
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
curl "api.goskive.com/v2/comments/7/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f23f87f677cbb02a804b9b67830ba6eb3b3a7f13593cb218cbc9a237449ee95"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/52
Content-Type: application/json
Authorization: Bearer 5b8ef28d80ff89f498dd397ea52577ac32b74b576d43622f70c4e537c949ccda
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
curl "api.goskive.com/v2/comments/52" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b8ef28d80ff89f498dd397ea52577ac32b74b576d43622f70c4e537c949ccda"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/54/republish
Content-Type: application/json
Authorization: Bearer 520c7906db563f6a645f5376de575a53a11c9b7f5ef5093fc482ba9482755d85
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
	-H "Authorization: Bearer 520c7906db563f6a645f5376de575a53a11c9b7f5ef5093fc482ba9482755d85"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer d8ae64d850bd1f9eb15da653a46f89401bfb70fd4f1484f9601c4caf5af9a4da
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8ae64d850bd1f9eb15da653a46f89401bfb70fd4f1484f9601c4caf5af9a4da"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/15/report
Content-Type: application/json
Authorization: Bearer 66d512363025e60a0351e74a518ccf5d42df7729ef1711cf105eb9a3f82719e5
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/15/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66d512363025e60a0351e74a518ccf5d42df7729ef1711cf105eb9a3f82719e5"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/1
Content-Type: application/json
Authorization: Bearer 6f6a85c1993088a8d82ebe239800e875b6c705e9c57d719ab0a7a7c8762d3efb
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
    "id": 1,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T19:49:33.903Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f6a85c1993088a8d82ebe239800e875b6c705e9c57d719ab0a7a7c8762d3efb"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 99b394b96acba269f9d7c99d500d51e790fa059a0cf7cb575a6adc7105b3e7e5
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
      "id": 2,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T19:49:34.022Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T19:49:34.026Z"
    },
    {
      "id": 4,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T19:49:34.030Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99b394b96acba269f9d7c99d500d51e790fa059a0cf7cb575a6adc7105b3e7e5"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer b65db051e5013596ab66c9f5d8574d7e7a662b4c28442a61958172f6a0c4c07c
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
	-H "Authorization: Bearer b65db051e5013596ab66c9f5d8574d7e7a662b4c28442a61958172f6a0c4c07c"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 1baa609b7551d192517fa7d48eb8a2a00cd5e26698b1eda154bc8fcb9e995e06
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
	-H "Authorization: Bearer 1baa609b7551d192517fa7d48eb8a2a00cd5e26698b1eda154bc8fcb9e995e06"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer cfabaf054d372cec0a2e6e5dbd3dff08702148d857c772ec88ef80e3c0a116ee
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
      "company_id": 20,
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
	-H "Authorization: Bearer cfabaf054d372cec0a2e6e5dbd3dff08702148d857c772ec88ef80e3c0a116ee"
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
Authorization: Bearer 77f4085ee494935ce51850d0e6945f4fe72511ad9958d79415a8be3219c6b782
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
	-H "Authorization: Bearer 77f4085ee494935ce51850d0e6945f4fe72511ad9958d79415a8be3219c6b782"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d9502f5eb1b91ad7573ad06646c66d4431f1192011ec694c4f08b9b135fc5bf2
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
    "updated_at": "2016-12-15T19:50:19.841Z",
    "course_id": 256,
    "author_id": 771,
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
	-H "Authorization: Bearer d9502f5eb1b91ad7573ad06646c66d4431f1192011ec694c4f08b9b135fc5bf2"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6869b095f1bdda438543d4990c9ccae725329bd0d81455ed3a658a99c1424c7c
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
      "id": 133,
      "updated_at": "2016-12-15T19:50:16.489Z",
      "course_id": 243,
      "author_id": 721,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 115",
      "position": 1
    },
    {
      "id": 134,
      "updated_at": "2016-12-15T19:50:16.514Z",
      "course_id": 243,
      "author_id": 722,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 116",
      "position": 2
    },
    {
      "id": 135,
      "updated_at": "2016-12-15T19:50:16.735Z",
      "course_id": 243,
      "author_id": 723,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T19:50:16.364Z",
      "questions_updated_at": "2016-12-15T19:50:16.364Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 117",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6869b095f1bdda438543d4990c9ccae725329bd0d81455ed3a658a99c1424c7c"
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
      "id": 139,
      "updated_at": "2016-12-15T19:50:17.414Z",
      "course_id": 246,
      "author_id": 735,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 121",
      "position": 1
    },
    {
      "id": 140,
      "updated_at": "2016-12-15T19:50:17.439Z",
      "course_id": 246,
      "author_id": 736,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 122",
      "position": 2
    },
    {
      "id": 141,
      "updated_at": "2016-12-15T19:50:17.657Z",
      "course_id": 246,
      "author_id": 737,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T19:50:17.293Z",
      "questions_updated_at": "2016-12-15T19:50:17.293Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 123",
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
Authorization: Bearer 72eefd2872258fcb020fd6defd6ddd020806777fba030da49baab042b34db84a
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
      "id": 136,
      "updated_at": "2016-12-15T19:50:17.115Z",
      "course_id": 245,
      "author_id": 730,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 118",
      "position": 1
    },
    {
      "id": 137,
      "updated_at": "2016-12-15T19:50:17.141Z",
      "course_id": 245,
      "author_id": 731,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 119",
      "position": 2
    },
    {
      "id": 138,
      "updated_at": "2016-12-15T19:50:17.167Z",
      "course_id": 245,
      "author_id": 732,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 120",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72eefd2872258fcb020fd6defd6ddd020806777fba030da49baab042b34db84a"
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
      "id": 142,
      "updated_at": "2016-12-15T19:50:17.828Z",
      "course_id": 247,
      "author_id": 741,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 124",
      "position": 1
    },
    {
      "id": 143,
      "updated_at": "2016-12-15T19:50:17.854Z",
      "course_id": 247,
      "author_id": 742,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 125",
      "position": 2
    },
    {
      "id": 144,
      "updated_at": "2016-12-15T19:50:17.878Z",
      "course_id": 247,
      "author_id": 743,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 126",
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
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer ad812f3ad169173841c4164a6a6e09912a146a6f58f82e4d768f0c11ff0fa480
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
    "course_id": 310,
    "user_id": 976,
    "updated_at": "2016-12-15T19:50:36.210Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad812f3ad169173841c4164a6a6e09912a146a6f58f82e4d768f0c11ff0fa480"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer e5444b2ed8ec549f89bd0163750b34df401c8de6917332ee8a3565804a86433e
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
      "course_id": 306,
      "user_id": 964,
      "updated_at": "2016-12-15T19:50:35.413Z"
    },
    {
      "id": 3,
      "course_id": 306,
      "user_id": 965,
      "updated_at": "2016-12-15T19:50:35.427Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5444b2ed8ec549f89bd0163750b34df401c8de6917332ee8a3565804a86433e"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/87/files
Content-Type: application/json
Authorization: Bearer bd45819e8b344de6ba1bbebb05249f6ab963e8c48c5d12d0f64a535c1128d2a5
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
        "id": 312,
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
        "created_at": "2016-12-15T19:49:39.562Z",
        "updated_at": "2016-12-15T19:49:39.562Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T19:49:39.575Z",
      "updated_at": "2016-12-15T19:49:39.575Z",
      "course_id": 87,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 313,
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
        "created_at": "2016-12-15T19:49:39.586Z",
        "updated_at": "2016-12-15T19:49:39.586Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T19:49:39.596Z",
      "updated_at": "2016-12-15T19:49:39.596Z",
      "course_id": 87,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 7,
      "uploader": {
        "id": 314,
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
        "created_at": "2016-12-15T19:49:39.607Z",
        "updated_at": "2016-12-15T19:49:39.607Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T19:49:39.617Z",
      "updated_at": "2016-12-15T19:49:39.617Z",
      "course_id": 87,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/87/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd45819e8b344de6ba1bbebb05249f6ab963e8c48c5d12d0f64a535c1128d2a5"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/86/files
Content-Type: application/json
Authorization: Bearer be038ff0d958e0cadeecd75bb5873a921b3eb368eea56ed68a4fdba88c6c0027
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
      "id": 310,
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
      "created_at": "2016-12-15T19:49:39.247Z",
      "updated_at": "2016-12-15T19:49:39.247Z"
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
    "created_at": "2016-12-15T19:49:39.297Z",
    "updated_at": "2016-12-15T19:49:39.297Z",
    "course_id": 86,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/86/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be038ff0d958e0cadeecd75bb5873a921b3eb368eea56ed68a4fdba88c6c0027"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/85/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer c33f480d3d6d44c8813695cf341e27c5330f92e9524885d3d91b6848e7660640
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
    "key": "cache/8d9681a1e75d2d82edcbaa6588fa38b5.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQyMDo0OTozOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzhkOTY4MWExZTc1ZDJkODJlZGNiYWE2NTg4ZmEzOGI1LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDE5NDkzOVoifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T194939Z",
    "x-amz-signature": "ade272e18fd3547288cce5f90a5a7c26563ede3e9e7fc0c3d390b0ff78b1e5b9"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/85/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c33f480d3d6d44c8813695cf341e27c5330f92e9524885d3d91b6848e7660640"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 70cfcba877e4e12759c8bc34343812f09a385e9784ca4a4f9dac61733c48f8e7
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
	-H "Authorization: Bearer 70cfcba877e4e12759c8bc34343812f09a385e9784ca4a4f9dac61733c48f8e7"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4bca1ae05c183bb96c941fe1d35457cb2a0d4ce763dd10e4a8267da451c287cb
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
	-H "Authorization: Bearer 4bca1ae05c183bb96c941fe1d35457cb2a0d4ce763dd10e4a8267da451c287cb"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4ef24d960c51baedf627f385c3478c557afd1e63ce520a06d89c43eb0d0421ae
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
	-H "Authorization: Bearer 4ef24d960c51baedf627f385c3478c557afd1e63ce520a06d89c43eb0d0421ae"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 17950c93c9b406806586b7bff941431be0dbf8ab73a1817b8c5272f9a2b88953
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
	-H "Authorization: Bearer 17950c93c9b406806586b7bff941431be0dbf8ab73a1817b8c5272f9a2b88953"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 62c748d7a814d45d798d2240846b418ccfffecd5bb26a8e5244599d9f4f2b749
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
	-H "Authorization: Bearer 62c748d7a814d45d798d2240846b418ccfffecd5bb26a8e5244599d9f4f2b749"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer a3e34c4e9d91338b52a1f28e2c2fb879152b876199b544a29a0f8d5b55de2282
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
    "creator_id": 437,
    "id": 122,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 127,
    "additional_university_ids": [

    ],
    "discipline_id": 130,
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
    "chapters_updated_at": "2016-12-15T19:49:49.329Z",
    "updated_at": "2016-12-15T19:49:50.553Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 438,
        "chapter_id": 102,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:50.341Z",
        "created_at": "2016-12-15T19:49:50.341Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 438,
        "chapter_id": 103,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:50.416Z",
        "created_at": "2016-12-15T19:49:50.416Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 438,
        "chapter_id": 102,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:50.382Z",
        "created_at": "2016-12-15T19:49:50.382Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 438,
        "chapter_id": 103,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:50.456Z",
        "created_at": "2016-12-15T19:49:50.456Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 438,
        "chapter_id": 102,
        "position": 57,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:49.564Z",
        "created_at": "2016-12-15T19:49:49.475Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 438,
        "chapter_id": 102,
        "position": 58,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:49.697Z",
        "created_at": "2016-12-15T19:49:49.622Z",
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
        "author_id": 438,
        "chapter_id": 103,
        "position": 59,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:49.861Z",
        "created_at": "2016-12-15T19:49:49.777Z",
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
        "author_id": 438,
        "chapter_id": 103,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:49.998Z",
        "created_at": "2016-12-15T19:49:49.919Z",
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
        "id": 102,
        "updated_at": "2016-12-15T19:49:50.505Z",
        "course_id": 122,
        "author_id": 437,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T19:49:49.329Z",
        "questions_updated_at": "2016-12-15T19:49:49.329Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 96",
        "position": 1
      },
      {
        "id": 103,
        "updated_at": "2016-12-15T19:49:50.544Z",
        "course_id": 122,
        "author_id": 437,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T19:49:49.329Z",
        "questions_updated_at": "2016-12-15T19:49:49.329Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 97",
        "position": 2
      }
    ],
    "topic_id": 129,
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
	-H "Authorization: Bearer a3e34c4e9d91338b52a1f28e2c2fb879152b876199b544a29a0f8d5b55de2282"
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
    "creator_id": 443,
    "id": 123,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 128,
    "additional_university_ids": [

    ],
    "discipline_id": 131,
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
    "chapters_updated_at": "2016-12-15T19:49:50.707Z",
    "updated_at": "2016-12-15T19:49:51.936Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 443,
        "chapter_id": 104,
        "position": 63,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:50.928Z",
        "created_at": "2016-12-15T19:49:50.845Z",
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
            "id": 155,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 156,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 443,
        "chapter_id": 105,
        "position": 65,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T19:49:51.251Z",
        "created_at": "2016-12-15T19:49:51.164Z",
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
      }
    ],
    "chapters": [
      {
        "id": 104,
        "updated_at": "2016-12-15T19:49:51.888Z",
        "course_id": 123,
        "author_id": 443,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T19:49:50.707Z",
        "questions_updated_at": "2016-12-15T19:49:50.707Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 98",
        "position": 1
      },
      {
        "id": 105,
        "updated_at": "2016-12-15T19:49:51.927Z",
        "course_id": 123,
        "author_id": 443,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T19:49:50.707Z",
        "questions_updated_at": "2016-12-15T19:49:50.707Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 99",
        "position": 2
      }
    ],
    "topic_id": 130,
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
PUT /v2/courses/136/pin
Content-Type: application/json
Authorization: Bearer b2929841a061efe876e8c2b6c2404f38ff8c2a1f23373a07d94f721d9ddbb529
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/136/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2929841a061efe876e8c2b6c2404f38ff8c2a1f23373a07d94f721d9ddbb529"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/126/pin
Content-Type: application/json
Authorization: Bearer 6062880d67957a6d8454acc7e57294500e660e8eef2d78c61dd07d76824097f6
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/126/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6062880d67957a6d8454acc7e57294500e660e8eef2d78c61dd07d76824097f6"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0328ee61a8da9dce61609014a8a7058901d8480a2ba17eb8de22b26f2d32a5a0
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
    "creator_id": 430,
    "id": 118,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 123,
    "additional_university_ids": [

    ],
    "discipline_id": 126,
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
    "updated_at": "2016-12-15T19:49:48.751Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 125,
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
	-H "Authorization: Bearer 0328ee61a8da9dce61609014a8a7058901d8480a2ba17eb8de22b26f2d32a5a0"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 73bbfc15a1ad9e948900b67d9ac04a4d6ac1ee5e0c227b34d89b810a7a8fdcb3
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
    "id": 301,
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
    "created_at": "2016-12-15T19:49:38.489Z",
    "updated_at": "2016-12-15T19:49:38.489Z",
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
	-H "Authorization: Bearer 73bbfc15a1ad9e948900b67d9ac04a4d6ac1ee5e0c227b34d89b810a7a8fdcb3"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b56365e1969922ccc2c37f3ed9d221c143da9b88584c61d6866cbc48a4aeeb2e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[85]}
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
    "id": 297,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      85
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T19:49:38.209Z",
    "updated_at": "2016-12-15T19:49:38.249Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[85]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b56365e1969922ccc2c37f3ed9d221c143da9b88584c61d6866cbc48a4aeeb2e"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 157f2f7c3b35e59cf3803c30d8c80390aa6a8c123ec4bbec35a213179d60ff2d
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
    "id": 300,
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
    "created_at": "2016-12-15T19:49:38.417Z",
    "updated_at": "2016-12-15T19:49:38.417Z",
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
	-H "Authorization: Bearer 157f2f7c3b35e59cf3803c30d8c80390aa6a8c123ec4bbec35a213179d60ff2d"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 28eff75cd2d8257f7d8bc031ea55c21d5d009e3443f865ef3dea08e3bedc808b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[87]}
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
    "id": 299,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      87
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T19:49:38.361Z",
    "updated_at": "2016-12-15T19:49:38.361Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[87]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28eff75cd2d8257f7d8bc031ea55c21d5d009e3443f865ef3dea08e3bedc808b"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 5f276448a7a94bc72ef957abb3f2290ae94e51c5bea4a184e390eff5688ec4f9
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

84
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
    "id": 296,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0944fc9213b72fb25b286e7a8ed006dbd0cbac90.jpg",
    "university_id": null,
    "fields_of_study": [
      84
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T19:49:37.910Z",
    "updated_at": "2016-12-15T19:49:38.156Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/44537a1263152095ab50045ccbb4a9a5ad8202bb.jpg",
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

84
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 5f276448a7a94bc72ef957abb3f2290ae94e51c5bea4a184e390eff5688ec4f9"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2bcee311362b3fcad1a1bf6d6cc14b6c33094b738935ec753a1e7a14bef83632
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
      "bookmarkable_id": 42,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 43,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 44,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bcee311362b3fcad1a1bf6d6cc14b6c33094b738935ec753a1e7a14bef83632"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 462188f7946656a99624d734d0777edb3234730a1bcba12f03e0c9fc116eca2b
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
      "creator_id": 811,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-202",
      "html_url": "https://goskive.com/course/mit-course-202",
      "slug": "mit-course-202",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 281,
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
      "updated_at": "2016-12-15T19:50:24.394Z",
      "shortname": "mit-course-202",
      "topic_id": 280,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 202",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 812,
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-203",
      "html_url": "https://goskive.com/course/mit-course-203",
      "slug": "mit-course-203",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "discipline_id": 282,
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
      "updated_at": "2016-12-15T19:50:24.523Z",
      "shortname": "mit-course-203",
      "topic_id": 281,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 462188f7946656a99624d734d0777edb3234730a1bcba12f03e0c9fc116eca2b"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer e09296082b1977848bacdaa42761f99262a60153a497f19e61e96e13a40b569d
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
        "created_at": "2016-12-15T19:49:10.485Z",
        "updated_at": "2016-12-15T19:49:10.485Z",
        "file_url": "memory://abcb9334d58a3812ee3be0254cdd61c4.pdf",
        "course_id": 6,
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
        "created_at": "2016-12-15T19:49:10.607Z",
        "updated_at": "2016-12-15T19:49:10.607Z",
        "file_url": "memory://38e74e0f2e820037bf03743a7bc33479.pdf",
        "course_id": 7,
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
        "created_at": "2016-12-15T19:49:10.729Z",
        "updated_at": "2016-12-15T19:49:10.729Z",
        "file_url": "memory://dae0a934b21cb6319ff843b9ad6a9963.pdf",
        "course_id": 8,
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
	-H "Authorization: Bearer e09296082b1977848bacdaa42761f99262a60153a497f19e61e96e13a40b569d"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 6df546cbc397268ca4f9fa0b65eac2e79b45fbb67539e63d5fea6376bcde8a90
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
        "updated_at": "2016-12-15T19:50:22.713Z"
      },
      "created_at": "2016-12-15T19:50:22.717Z",
      "updated_at": "2016-12-15T19:50:22.717Z",
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
        "updated_at": "2016-12-15T19:50:22.726Z"
      },
      "created_at": "2016-12-15T19:50:22.729Z",
      "updated_at": "2016-12-15T19:50:22.729Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6df546cbc397268ca4f9fa0b65eac2e79b45fbb67539e63d5fea6376bcde8a90"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer faea4fe30dbbd620a8501a6804612646018d90a5402472127bdf46dffcbeb048
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
      "created_at": "2016-12-15T19:49:44.217Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 12,
      "updated_at": "2016-12-15T19:49:44.367Z",
      "author_id": "374",
      "thread_subject_id": "103",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 15,
      "created_at": "2016-12-15T19:49:44.356Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 13,
      "updated_at": "2016-12-15T19:49:44.371Z",
      "author_id": "377",
      "thread_subject_id": "104",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-12-15T19:49:44.744Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-12-15T19:49:44.744Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-12-15T19:49:45.117Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-12-15T19:49:45.117Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 18,
      "created_at": "2016-12-15T19:49:45.487Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-12-15T19:49:45.487Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 19,
      "created_at": "2016-12-15T19:49:45.769Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 63,
      "updated_at": "2016-12-15T19:49:45.769Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-12-15T19:49:46.060Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 64,
      "updated_at": "2016-12-15T19:49:46.060Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-12-15T19:49:46.341Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 65,
      "updated_at": "2016-12-15T19:49:46.341Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faea4fe30dbbd620a8501a6804612646018d90a5402472127bdf46dffcbeb048"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/22
Content-Type: application/json
Authorization: Bearer 5442a72b70ef0a7c28829b3e0e8c8e19a33f6fa72137a38517d29961043e3713
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T19:39:46.000Z"}}
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
    "id": 22,
    "created_at": "2016-12-15T19:49:46.515Z",
    "read_at": "2016-12-15T19:39:46.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 14,
    "updated_at": "2016-12-15T19:49:46.581Z",
    "author_id": "402",
    "thread_subject_id": "111",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/22" -d '{"notification":{"read_at":"2016-12-15T19:39:46.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5442a72b70ef0a7c28829b3e0e8c8e19a33f6fa72137a38517d29961043e3713"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b9aa9c0f94b66c4ed83c3ca87c3d04d3676ead499595a1c8091404d9f0da0151
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
      "course_id": 311,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T19:50:36.347Z",
      "course_published": true,
      "updated_at": "2016-12-15T19:50:36.342Z"
    },
    {
      "id": 5,
      "course_id": 312,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T19:50:36.469Z",
      "course_published": true,
      "updated_at": "2016-12-15T19:50:36.464Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9aa9c0f94b66c4ed83c3ca87c3d04d3676ead499595a1c8091404d9f0da0151"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer f26e494fdd49fe252042683ef94c2f385ad6ea60e641b00ea9c79e13fbd18315
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
    "course_id": 314,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T19:50:36.879Z",
    "course_published": true,
    "updated_at": "2016-12-15T19:50:36.875Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f26e494fdd49fe252042683ef94c2f385ad6ea60e641b00ea9c79e13fbd18315"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 1b6a4f2a29a0a509b99900ccedd2409961a0fd9dc0770f31478686a8aee5360b
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
    "course_id": 313,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T19:50:36.736Z",
    "course_published": true,
    "updated_at": "2016-12-15T19:50:36.728Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b6a4f2a29a0a509b99900ccedd2409961a0fd9dc0770f31478686a8aee5360b"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 7145c8c1d82d2bf0b121daba39343446fcf388f1981fe72f9c112b08f532f35d
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
      "votable_id": 47,
      "user_id": 256
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 48,
      "user_id": 256
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 256
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 256
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7145c8c1d82d2bf0b121daba39343446fcf388f1981fe72f9c112b08f532f35d"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/119
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
    "id": 119,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 117,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 119
      },
      {
        "id": 118,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 119
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/119" -X GET \
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
      "id": 117,
      "name": "De-engineered foreground strategy",
      "name_translations": {
        "en": "De-engineered foreground strategy"
      }
    },
    {
      "id": 118,
      "name": "Team-oriented maximized moratorium",
      "name_translations": {
        "en": "Team-oriented maximized moratorium"
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
Authorization: Bearer 6028eb98394bd1a932820a6a7cf83a37a971566c98563e5858bc90e3fc001c0d
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
    "user_id": 856,
    "feedbackable_id": 93,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T19:50:27.238Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6028eb98394bd1a932820a6a7cf83a37a971566c98563e5858bc90e3fc001c0d"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer cbf2916f8482d0e72f23c9a6cf58e1398af3661e389c3fdda482967ac16c09f0
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
    "id": 23,
    "user_id": 846,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T19:50:26.555Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbf2916f8482d0e72f23c9a6cf58e1398af3661e389c3fdda482967ac16c09f0"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/18
Content-Type: application/json
Authorization: Bearer 480f45301c7c421c4312a6b24febd90ae7e0ae8bf2438de7ed2dea0186dd9acd
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
    "id": 18,
    "user_id": 819,
    "feedbackable_id": 86,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T19:50:25.043Z",
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
curl "api.goskive.com/v2/feedbacks/18" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 480f45301c7c421c4312a6b24febd90ae7e0ae8bf2438de7ed2dea0186dd9acd"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/fix
Content-Type: application/json
Authorization: Bearer 57680b3bfec5ece00dca85ce4aa73a40619b800a5a4c08f5fcbeee47ffc2f84c
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
curl "api.goskive.com/v2/feedbacks/20/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57680b3bfec5ece00dca85ce4aa73a40619b800a5a4c08f5fcbeee47ffc2f84c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer b0242a3e2d9c20fb25ed5d771c63a6c47ab19c2ea0602082eca16468c82ebab5
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
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0242a3e2d9c20fb25ed5d771c63a6c47ab19c2ea0602082eca16468c82ebab5"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/close
Content-Type: application/json
Authorization: Bearer 1ea515051b3ed65178c193a9c7b8bfde7019e6484d6e6ff138a321b96b0afd64
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
	-H "Authorization: Bearer 1ea515051b3ed65178c193a9c7b8bfde7019e6484d6e6ff138a321b96b0afd64"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer a907bdd2e1bdec3d60b71fe817d62668e13fbc9164dc499003445ccad7ff3fb2
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
    "id": 19,
    "user_id": 824,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T19:50:25.406Z",
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
curl "api.goskive.com/v2/feedbacks/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a907bdd2e1bdec3d60b71fe817d62668e13fbc9164dc499003445ccad7ff3fb2"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer 757ab686f950f33765203961b29b469ffe31dea404cac8bf72688226eb807c50
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
curl "api.goskive.com/v2/files/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 757ab686f950f33765203961b29b469ffe31dea404cac8bf72688226eb807c50"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/21/bookmark
Content-Type: application/json
Authorization: Bearer fe62a5d6019deaa84ac9b7949ada0325e35b1353fe1265dec2ace4f19342142a
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe62a5d6019deaa84ac9b7949ada0325e35b1353fe1265dec2ace4f19342142a"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer 2a39b5969be3d740823b7fa2b5227e567894b497f57043d4bbcab43489599ab1
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a39b5969be3d740823b7fa2b5227e567894b497f57043d4bbcab43489599ab1"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/22
Content-Type: application/json
Authorization: Bearer aa881697220f4c8340dbda004d7babe849770d732e78f03f692e1904664e8e38
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b2c0667a13f1433573a1fe64a8844e33.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T195008Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=3ebe9ac43635285392209aa1823524debe38c845e5c24701911ed6b69f6ae837",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa881697220f4c8340dbda004d7babe849770d732e78f03f692e1904664e8e38"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer 62459f19a79479def545752221ba8748e6050df5cb41da38db0cfd977e785d79
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/ef32babf5a31fa17373b2165f1f35571.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T195005Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=cdb90410b00ee20b8a3b1b2fa9e88317ced5eb1f0a9a2ef0ca876a6631ae2389",
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
	-H "Authorization: Bearer 62459f19a79479def545752221ba8748e6050df5cb41da38db0cfd977e785d79"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/15/metadata
Content-Type: application/json
Authorization: Bearer b3cc20437be4516f8ae6fb33ab94efd09b31c8934931878570e5b2f45974569a
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
    "id": 15,
    "uploader": {
      "id": 631,
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
      "created_at": "2016-12-15T19:50:06.738Z",
      "updated_at": "2016-12-15T19:50:06.738Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T19:50:06.859Z",
    "updated_at": "2016-12-15T19:50:06.859Z",
    "course_id": 192,
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
curl "api.goskive.com/v2/files/15/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3cc20437be4516f8ae6fb33ab94efd09b31c8934931878570e5b2f45974569a"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/9/matched_courses?required_cu_count=2
Authorization: Bearer 7eb2bd2a2dd4069d8d467cc048c6002a875b78e02df0b7f7f53548178959cb83
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
      "creator_id": 417,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 120,
      "additional_university_ids": [

      ],
      "discipline_id": 123,
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
      "chapters_updated_at": "2016-12-15T19:49:46.894Z",
      "updated_at": "2016-12-15T19:49:48.023Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 122,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 422,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-70c57155-7922-4b03-a596-5b9efb36ec47",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-70c57155-7922-4b03-a596-5b9efb36ec47",
      "slug": "mit-the-great-british-bake-off-70c57155-7922-4b03-a596-5b9efb36ec47",
      "university_id": 121,
      "additional_university_ids": [

      ],
      "discipline_id": 124,
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
      "chapters_updated_at": "2016-12-15T19:49:46.894Z",
      "updated_at": "2016-12-15T19:49:48.398Z",
      "shortname": "mit-the-great-british-bake-off-70c57155-7922-4b03-a596-5b9efb36ec47",
      "topic_id": 123,
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
curl "api.goskive.com/v2/files/9/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 7eb2bd2a2dd4069d8d467cc048c6002a875b78e02df0b7f7f53548178959cb83"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/11/download
Content-Type: application/json
Authorization: Bearer c6573969b78355705d20a3c9dffabcafe527c061cace011c35bee82390a4a33d
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6573969b78355705d20a3c9dffabcafe527c061cace011c35bee82390a4a33d"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/16/report
Content-Type: application/json
Authorization: Bearer 7cfe8a00767634e22926b20fef9a9687ff1a9df0d6d0c707da3535d387dc32a7
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
	-H "Authorization: Bearer 7cfe8a00767634e22926b20fef9a9687ff1a9df0d6d0c707da3535d387dc32a7"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/20/bookmark
Content-Type: application/json
Authorization: Bearer 398050b260828cce9561d0bc1838ee916381c9105259b9c2419a2dd9d0377d6b
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 398050b260828cce9561d0bc1838ee916381c9105259b9c2419a2dd9d0377d6b"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/12/upvote
Content-Type: application/json
Authorization: Bearer 302c8120232d004df6fc3b5485a9ecfbbda51505a8440dba0c3ff3ffb8937e2e
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 302c8120232d004df6fc3b5485a9ecfbbda51505a8440dba0c3ff3ffb8937e2e"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/99/comments
Content-Type: application/json
Authorization: Bearer ee582b3dd598163b9c98e6f02cde07113724c0a3ea783c683f1aac84d2b6d9be
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
    "id": 60,
    "author_id": 958,
    "reply_to_id": null,
    "created_at": "2016-12-15T19:50:34.954Z",
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
curl "api.goskive.com/v2/flashcards/99/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee582b3dd598163b9c98e6f02cde07113724c0a3ea783c683f1aac84d2b6d9be"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/97/comments
Content-Type: application/json
Authorization: Bearer bfcf92afb33c16a0df10424957b41aca00aad505f3c215fe3f40da507c4446bb
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
    "id": 59,
    "author_id": 952,
    "reply_to_id": null,
    "created_at": "2016-12-15T19:50:34.326Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 952,
      "feedbackable_id": 97,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:50:34.323Z",
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
curl "api.goskive.com/v2/flashcards/97/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfcf92afb33c16a0df10424957b41aca00aad505f3c215fe3f40da507c4446bb"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/95/comments
Content-Type: application/json
Authorization: Bearer 90e5039753ee9ae2cd5493a6467a0770ec82a53cc79581056a48aa452f4eb88b
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
      "id": 58,
      "author_id": 948,
      "reply_to_id": null,
      "created_at": "2016-12-15T19:50:33.843Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 947,
      "reply_to_id": null,
      "created_at": "2016-12-15T19:50:33.827Z",
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
curl "api.goskive.com/v2/flashcards/95/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90e5039753ee9ae2cd5493a6467a0770ec82a53cc79581056a48aa452f4eb88b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/98/comments
Content-Type: application/json
Authorization: Bearer 5f6bf817aa11eeefb211c130bb071ff9c5d226b8551e4c838ea9259f51f354ff
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
curl "api.goskive.com/v2/flashcards/98/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f6bf817aa11eeefb211c130bb071ff9c5d226b8551e4c838ea9259f51f354ff"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/31/feedbacks
Content-Type: application/json
Authorization: Bearer 21653c5b6faf7a02e844d62f4cf9065e92d4869d962b70349cfdbb65331935c2
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
    "id": 16,
    "user_id": 359,
    "feedbackable_id": 31,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T19:49:42.939Z",
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
curl "api.goskive.com/v2/flashcards/31/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21653c5b6faf7a02e844d62f4cf9065e92d4869d962b70349cfdbb65331935c2"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/28/feedbacks
Content-Type: application/json
Authorization: Bearer 2a1ddcbc25d0301e8ae1801af6c27c41e07f6881202751f80e17962faaf6bf64
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
      "id": 13,
      "user_id": 344,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:49:42.101Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 343,
      "feedbackable_id": 28,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:49:42.090Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/28/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a1ddcbc25d0301e8ae1801af6c27c41e07f6881202751f80e17962faaf6bf64"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/74/votes
Content-Type: application/json
Authorization: Bearer 0997ea73bceda6d812203753b5531b73397b4fb5492115eb5d8f5a0a7ce98787
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 74,
      "user_id": 673
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 74,
      "user_id": 672
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 74,
      "user_id": 671
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/74/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0997ea73bceda6d812203753b5531b73397b4fb5492115eb5d8f5a0a7ce98787"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/1/republish
Content-Type: application/json
Authorization: Bearer db963edc1ecbb9bd6a80831573d89bb6b1f82c277a1efdf70bcfa0642a69b5b8
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
	-H "Authorization: Bearer db963edc1ecbb9bd6a80831573d89bb6b1f82c277a1efdf70bcfa0642a69b5b8"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/4/bookmark
Content-Type: application/json
Authorization: Bearer 5fe3a56cfcaf2f45daf1bd780d7a465ad48cb050dee83f90acaac51f417b5729
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
	-H "Authorization: Bearer 5fe3a56cfcaf2f45daf1bd780d7a465ad48cb050dee83f90acaac51f417b5729"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/24
Content-Type: application/json
Authorization: Bearer 11ec91462984425d38e63fd55932ee83ad42d84089825add9e314bbb55b3d8fb
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11ec91462984425d38e63fd55932ee83ad42d84089825add9e314bbb55b3d8fb"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/8/downvote
Content-Type: application/json
Authorization: Bearer 5076a42b5f943491b0942af0b4257533758089bcb1b812e6971e8517e0e72e6b
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/8/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5076a42b5f943491b0942af0b4257533758089bcb1b812e6971e8517e0e72e6b"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/6
Content-Type: application/json
Authorization: Bearer dcb8a6ff578fc63aade80da954854de0b53be3b35ffadedcf1df7532b7738848
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
    "id": 6,
    "obfuscated_id": "eyxYPTvoIb8",
    "author_id": 183,
    "chapter_id": 50,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:27.109Z",
    "created_at": "2016-12-15T19:49:27.109Z",
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
curl "api.goskive.com/v2/flashcards/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcb8a6ff578fc63aade80da954854de0b53be3b35ffadedcf1df7532b7738848"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/5/report
Content-Type: application/json
Authorization: Bearer 662f857eca36641afb1e0ece3dc922dc52475baad522d7b502b9f98dd7ab3524
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/5/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 662f857eca36641afb1e0ece3dc922dc52475baad522d7b502b9f98dd7ab3524"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/7/bookmark
Content-Type: application/json
Authorization: Bearer e23f07795c71408bc0a9baa2243ff386f280672db3ba9a3c28ca168360085b88
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/7/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e23f07795c71408bc0a9baa2243ff386f280672db3ba9a3c28ca168360085b88"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/3/upvote
Content-Type: application/json
Authorization: Bearer 643264471533b1e9f2a547e5bc700affdabd0a825392dde5848c7346df8a8ac0
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
	-H "Authorization: Bearer 643264471533b1e9f2a547e5bc700affdabd0a825392dde5848c7346df8a8ac0"
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
    "key": "cache/63c09f20999a018067d6391df9af5977.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQyMDo0OTo0M1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzYzYzA5ZjIwOTk5YTAxODA2N2Q2MzkxZGY5YWY1OTc3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTk0OTQzWiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T194943Z",
    "x-amz-signature": "f4789a03e780a2a189f666fd1242260299fb732a3248e2a70dff658021b2e184"
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
Authorization: Bearer c087d27e2d0fee493e2a341840cd36b7ca5db2d5de0a9e2326369ef3d93d4582
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
	-H "Authorization: Bearer c087d27e2d0fee493e2a341840cd36b7ca5db2d5de0a9e2326369ef3d93d4582"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer f0551752da55585a78697a349d5e8193a76839f87b3a0a23aa4daf08a30d1045
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
	-H "Authorization: Bearer f0551752da55585a78697a349d5e8193a76839f87b3a0a23aa4daf08a30d1045"
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
{"password":{"reset_password_token":"kW9E7-4NrFCmsusSAeJU","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 656,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T19:50:08.968Z",
  "updated_at": "2016-12-15T19:50:09.147Z",
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
  "audit_id": 8379
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"kW9E7-4NrFCmsusSAeJU","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/2/comments
Content-Type: application/json
Authorization: Bearer 4d8ec44a01552479dcabfb9466f292e31fbecf32aa56b6b575cd00a2f25ac139
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
    "id": 1,
    "author_id": 8,
    "reply_to_id": null,
    "created_at": "2016-12-15T19:49:08.654Z",
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
curl "api.goskive.com/v2/questions/2/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d8ec44a01552479dcabfb9466f292e31fbecf32aa56b6b575cd00a2f25ac139"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/3/comments
Content-Type: application/json
Authorization: Bearer ed075972a1bb435af17340339949c43a0bf5c06d6351d6fa82b8ea7d0885ba7e
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
    "id": 2,
    "author_id": 11,
    "reply_to_id": null,
    "created_at": "2016-12-15T19:49:09.444Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 11,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:49:09.441Z",
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
curl "api.goskive.com/v2/questions/3/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed075972a1bb435af17340339949c43a0bf5c06d6351d6fa82b8ea7d0885ba7e"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/4/comments
Content-Type: application/json
Authorization: Bearer c495bde6b16d79aefe5e57fc91143ff1b72c9fac68aaff8da3a8f2b23ba5146e
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
      "id": 4,
      "author_id": 18,
      "reply_to_id": null,
      "created_at": "2016-12-15T19:49:09.909Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 17,
      "reply_to_id": null,
      "created_at": "2016-12-15T19:49:09.893Z",
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
curl "api.goskive.com/v2/questions/4/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c495bde6b16d79aefe5e57fc91143ff1b72c9fac68aaff8da3a8f2b23ba5146e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/1/comments
Content-Type: application/json
Authorization: Bearer b63fe243c5f86a0b34f44dcec539740b501ec83f75ad1aabbc659af7ec00469e
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
curl "api.goskive.com/v2/questions/1/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b63fe243c5f86a0b34f44dcec539740b501ec83f75ad1aabbc659af7ec00469e"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/15/feedbacks
Content-Type: application/json
Authorization: Bearer b8ad292a75f57cb282450321a5e50cd5ae91e36080785137c2e47ba9b532a7ad
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
    "id": 8,
    "user_id": 71,
    "feedbackable_id": 15,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T19:49:14.841Z",
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
curl "api.goskive.com/v2/questions/15/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8ad292a75f57cb282450321a5e50cd5ae91e36080785137c2e47ba9b532a7ad"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/11/feedbacks
Content-Type: application/json
Authorization: Bearer 56dc64f0d2b55c7038d2fb1d66338bd2b7571675e99894d1afaa2c03a8e3b9d1
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
      "id": 5,
      "user_id": 59,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:49:13.477Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 58,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T19:49:13.467Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/11/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56dc64f0d2b55c7038d2fb1d66338bd2b7571675e99894d1afaa2c03a8e3b9d1"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/109/votes
Content-Type: application/json
Authorization: Bearer b85acfa6f2f983ff47701df916a9497d8e0a39e31884d7b55142ae40b810d7ef
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
      "votable_id": 109,
      "user_id": 803
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 109,
      "user_id": 802
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 109,
      "user_id": 801
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/109/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b85acfa6f2f983ff47701df916a9497d8e0a39e31884d7b55142ae40b810d7ef"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/17/republish
Content-Type: application/json
Authorization: Bearer 0a7bef63a5b28c58b43aead3be3a2c1c5a64f07352e9ecc7ed2fe404c303270c
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
curl "api.goskive.com/v2/questions/17/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a7bef63a5b28c58b43aead3be3a2c1c5a64f07352e9ecc7ed2fe404c303270c"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/22/bookmark
Content-Type: application/json
Authorization: Bearer e15cccae75f20f75275702a39209fc7feac1c64f00d8b5ec3a9e66a758027e3b
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e15cccae75f20f75275702a39209fc7feac1c64f00d8b5ec3a9e66a758027e3b"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/24
Content-Type: application/json
Authorization: Bearer 142f4c7c5c3c40aa4f8bf098a520e5894f2429c1164ab0f80385b0e7e56a3020
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 142f4c7c5c3c40aa4f8bf098a520e5894f2429c1164ab0f80385b0e7e56a3020"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/21/downvote
Content-Type: application/json
Authorization: Bearer 4a646cd3b91193c48b91be532eb8224cb76fa3d55ce7c7f4383ecff57ddd43cc
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/21/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a646cd3b91193c48b91be532eb8224cb76fa3d55ce7c7f4383ecff57ddd43cc"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/19
Content-Type: application/json
Authorization: Bearer 0b74510afd1b597e2ee8d07703b6434ac0c6920f4e1b4982a10aaacd35defb36
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
    "id": 19,
    "obfuscated_id": "xt199h-LGto",
    "author_id": 83,
    "chapter_id": 19,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:16.450Z",
    "created_at": "2016-12-15T19:49:16.360Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b74510afd1b597e2ee8d07703b6434ac0c6920f4e1b4982a10aaacd35defb36"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/41/report
Content-Type: application/json
Authorization: Bearer 39368c81061c70f1ed224e3fb7e8f0ed20212078b82bdab38b454411c654b535
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/41/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39368c81061c70f1ed224e3fb7e8f0ed20212078b82bdab38b454411c654b535"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/20/bookmark
Content-Type: application/json
Authorization: Bearer e2c32cb0bff610dd6257deb0978145039b1fe62180ac08681e61d5f2622cb5ec
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/20/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2c32cb0bff610dd6257deb0978145039b1fe62180ac08681e61d5f2622cb5ec"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/23
Content-Type: application/json
Authorization: Bearer 97c0d48c41c4dadc600c5d02a6fcffc4a1a44f1bbbe1c99335c44ddbdf465008
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":23,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T19:49:17.777Z","updated_at":"2016-12-15T19:49:17.868Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":23,"author_id":95,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 95,
    "chapter_id": 23,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T19:49:17.962Z",
    "created_at": "2016-12-15T19:49:17.777Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x0000000da651f0>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 47,
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
curl "api.goskive.com/v2/questions/23" -d '{"question":{"question":{"id":23,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T19:49:17.777Z","updated_at":"2016-12-15T19:49:17.868Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":23,"author_id":95,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97c0d48c41c4dadc600c5d02a6fcffc4a1a44f1bbbe1c99335c44ddbdf465008"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/25/upvote
Content-Type: application/json
Authorization: Bearer 6af4f26fe86d1379ff972b021f9959569d74cc27067357202b41210a9a8e7dc6
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/25/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6af4f26fe86d1379ff972b021f9959569d74cc27067357202b41210a9a8e7dc6"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6b517f580456372745254746a62d1e69ca47f5305a5db4640e63d6c350ae4cb9
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
      "creator_id": 776,
      "id": 259,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 244,
      "additional_university_ids": [

      ],
      "discipline_id": 267,
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
      "updated_at": "2016-12-15T19:50:20.515Z",
      "shortname": "mit-pizza-201",
      "topic_id": 266,
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
	-H "Authorization: Bearer 6b517f580456372745254746a62d1e69ca47f5305a5db4640e63d6c350ae4cb9"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 0be2a34b69ce588383ef6cae250e568531e2fb3bb970b157ac02d533ba30369a
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
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-222",
      "html_url": "https://goskive.com/university/uni-222",
      "slug": "uni-222",
      "name": "National School of Pizza",
      "short_name": "Uni 222",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/549ae647dd29b5c0a395a4c9ebe51f04.jpg",
      "image_url_small": "memory://universities/2b7e1788a287921264564dca63fe838e.jpg",
      "image_thumb_url": "memory://universities/7b818a7f496e42fdc565ae4a716433d1.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T19:50:20.253Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-221",
      "html_url": "https://goskive.com/university/uni-221",
      "slug": "uni-221",
      "name": "National School of Pastry",
      "short_name": "Uni 221",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/3607ae4db73310414759b93d7d2a888c.jpg",
      "image_url_small": "memory://universities/384d13dc4afff56ce94e3c64d0cc12c6.jpg",
      "image_thumb_url": "memory://universities/80f1b63842a79f2803095d9c3d0d6757.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T19:50:20.187Z",
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
	-H "Authorization: Bearer 0be2a34b69ce588383ef6cae250e568531e2fb3bb970b157ac02d533ba30369a"
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
      "id": 275,
      "name": "Organized dedicated groupware",
      "name_translations": {
        "en": "Organized dedicated groupware"
      },
      "discipline_id": 276
    },
    {
      "id": 276,
      "name": "Team-oriented tangible encryption",
      "name_translations": {
        "en": "Team-oriented tangible encryption"
      },
      "discipline_id": 277
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
GET /v2/topics/274
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
    "id": 274,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 275
  }
}
```



```shell
curl "api.goskive.com/v2/topics/274" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 805dbe76723ec8fa73e26643db6aab12468e11af26b6a714b6a84c24c82057fe
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
      "id": 1,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-1",
      "html_url": "https://goskive.com/university/uni-1",
      "slug": "uni-1",
      "name": "University 1",
      "short_name": "Uni 1",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/346a2248c94a566b3a7a04bc0361a490.jpg",
      "image_url_small": "memory://universities/d0d5c83dd74679ca743d2edac17f2615.jpg",
      "image_thumb_url": "memory://universities/96991575d655e9c6b97798c9981aefcc.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T19:49:07.307Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "University 2",
      "short_name": "Uni 2",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/c208236104ac656d7e2c8beaad8eb703.jpg",
      "image_url_small": "memory://universities/1c5388c6d625c886c97838f0ead45e05.jpg",
      "image_thumb_url": "memory://universities/ae513c37af95d134547fdecc6206d6fa.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T19:49:07.373Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-3",
      "html_url": "https://goskive.com/university/uni-3",
      "slug": "uni-3",
      "name": "University 3",
      "short_name": "Uni 3",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/095c668b538aa2f1eb7a98f0df96ab6f.jpg",
      "image_url_small": "memory://universities/ac432e5128375cc9045fd491dc21e218.jpg",
      "image_thumb_url": "memory://universities/a880dd1cdc8d0af3b35574d5ee8f3e4a.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T19:49:07.437Z",
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
	-H "Authorization: Bearer 805dbe76723ec8fa73e26643db6aab12468e11af26b6a714b6a84c24c82057fe"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 90518f6f0da33776033d78c4a6ed41cc31c7a41cadf54a7a39a7e025ba4012d4
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
    "id": 5,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/299ee9d265c550627a616009eb63e88c.jpg",
    "image_url_small": "memory://universities/2a73a5e751b58eff464dcc8663c31af1.jpg",
    "image_thumb_url": "memory://universities/9659312d7eadcb504ff40f6de76375be.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T19:49:07.655Z",
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
	-H "Authorization: Bearer 90518f6f0da33776033d78c4a6ed41cc31c7a41cadf54a7a39a7e025ba4012d4"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 65f61cef51169f5763b867447b8c5321c1be94447c2f988bbdeaac1e7bdeb2c6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":211,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 675,
    "id": 204,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 209,
    "additional_university_ids": [

    ],
    "discipline_id": 212,
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
    "chapters_updated_at": "2016-12-15T19:50:11.330Z",
    "updated_at": "2016-12-15T19:50:11.488Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 126,
        "updated_at": "2016-12-15T19:50:11.478Z",
        "course_id": 204,
        "author_id": 675,
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
        "id": 127,
        "updated_at": "2016-12-15T19:50:11.491Z",
        "course_id": 204,
        "author_id": 675,
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
        "id": 128,
        "updated_at": "2016-12-15T19:50:11.504Z",
        "course_id": 204,
        "author_id": 675,
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
    "topic_id": 211,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":211,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65f61cef51169f5763b867447b8c5321c1be94447c2f988bbdeaac1e7bdeb2c6"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2a80552fe850a7d45b2fe12de818ad175898c97ef04cf7bc7a77b15e427387b3
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":212,"published":false}}
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
    "creator_id": 676,
    "id": 205,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 210,
    "additional_university_ids": [

    ],
    "discipline_id": 213,
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
    "updated_at": "2016-12-15T19:50:11.738Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 212,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":212,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a80552fe850a7d45b2fe12de818ad175898c97ef04cf7bc7a77b15e427387b3"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bf074f49f8ec4ea1aacbc411a14ae42a5ffd99da6be12c73aa4040bfe78e56bd
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
      "creator_id": 679,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 212,
      "additional_university_ids": [

      ],
      "discipline_id": 217,
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
      "updated_at": "2016-12-15T19:50:12.145Z",
      "shortname": "fu-course-165",
      "topic_id": 216,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 679,
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 212,
      "additional_university_ids": [

      ],
      "discipline_id": 218,
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
      "chapters_updated_at": "2016-12-15T19:50:11.963Z",
      "updated_at": "2016-12-15T19:50:12.402Z",
      "shortname": "fu-course-166",
      "topic_id": 217,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf074f49f8ec4ea1aacbc411a14ae42a5ffd99da6be12c73aa4040bfe78e56bd"
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
      "creator_id": 699,
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "discipline_id": 233,
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
      "updated_at": "2016-12-15T19:50:14.085Z",
      "shortname": "fu-course-181",
      "topic_id": 232,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 181",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 699,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "discipline_id": 234,
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
      "chapters_updated_at": "2016-12-15T19:50:13.904Z",
      "updated_at": "2016-12-15T19:50:14.371Z",
      "shortname": "fu-course-182",
      "topic_id": 233,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 182",
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
Authorization: Bearer 4228a9e9ebf68252bb4f5fee9d9d7e5e922b6e712de870e7839a44e8aac42099
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
      "creator_id": 686,
      "id": 213,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 214,
      "additional_university_ids": [

      ],
      "discipline_id": 221,
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
      "updated_at": "2016-12-15T19:50:12.786Z",
      "shortname": "fu-course-169",
      "topic_id": 220,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 686,
      "id": 214,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-170",
      "html_url": "https://goskive.com/course/fu-course-170",
      "slug": "fu-course-170",
      "university_id": 214,
      "additional_university_ids": [

      ],
      "discipline_id": 222,
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
      "updated_at": "2016-12-15T19:50:12.822Z",
      "shortname": "fu-course-170",
      "topic_id": 221,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 170",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4228a9e9ebf68252bb4f5fee9d9d7e5e922b6e712de870e7839a44e8aac42099"
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
      "creator_id": 704,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-185",
      "html_url": "https://goskive.com/course/fu-course-185",
      "slug": "fu-course-185",
      "university_id": 220,
      "additional_university_ids": [

      ],
      "discipline_id": 237,
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
      "updated_at": "2016-12-15T19:50:14.671Z",
      "shortname": "fu-course-185",
      "topic_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 704,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-186",
      "html_url": "https://goskive.com/course/fu-course-186",
      "slug": "fu-course-186",
      "university_id": 220,
      "additional_university_ids": [

      ],
      "discipline_id": 238,
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
      "updated_at": "2016-12-15T19:50:14.706Z",
      "shortname": "fu-course-186",
      "topic_id": 237,
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
Authorization: Bearer 8a97ae62a242696c1240264507a672249c37dc0a390e043b7bb8abbcf80ad4bf
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
  "id": 719,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T19:50:16.192Z",
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
	-H "Authorization: Bearer 8a97ae62a242696c1240264507a672249c37dc0a390e043b7bb8abbcf80ad4bf"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/781
Content-Type: application/json
Authorization: Bearer e983aabc37fe467c771f0ada22a1f5863c83e66bfafe4d8d83fc96e9628fe0d2
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
    "id": 781,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 246,
    "fields_of_study": [
      269,
      270
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T19:50:21.027Z",
    "updated_at": "2016-12-15T19:50:21.027Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/781" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e983aabc37fe467c771f0ada22a1f5863c83e66bfafe4d8d83fc96e9628fe0d2"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/779
Content-Type: application/json
Authorization: Bearer d3ebbb636f5d698ca4ddddcd309b8d6795424ce38d9629999bf016e9e0d57c33
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
    "id": 779,
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
    "created_at": "2016-12-15T19:50:20.801Z",
    "updated_at": "2016-12-15T19:50:20.801Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/779" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3ebbb636f5d698ca4ddddcd309b8d6795424ce38d9629999bf016e9e0d57c33"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/2
Content-Type: application/json
Authorization: Bearer c1079ad2b2fc27f9dc96d8a36077b8e4b3c6ca81fdc09c6b63c2c17eea268ec5
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
	-H "Authorization: Bearer c1079ad2b2fc27f9dc96d8a36077b8e4b3c6ca81fdc09c6b63c2c17eea268ec5"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/3
Content-Type: application/json
Authorization: Bearer d06ed5855bfa94cd318f6a96f1fbaff567eb258e99499a29ec0eda51a3319ed6
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
    "id": 3,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 8,
    "user_id": 37
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d06ed5855bfa94cd318f6a96f1fbaff567eb258e99499a29ec0eda51a3319ed6"
```
