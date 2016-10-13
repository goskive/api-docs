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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"586dffd45b47ad43488dce6956b6bcbb2c98c7a37e889098aa0795e62aaafd6c","client_secret":"31d2a440b81b858b99af62515fbf2aa7e1a5f4a6a33d9b7078621602d253d1dc"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"586dffd45b47ad43488dce6956b6bcbb2c98c7a37e889098aa0795e62aaafd6c","client_secret":"31d2a440b81b858b99af62515fbf2aa7e1a5f4a6a33d9b7078621602d253d1dc"}' -X POST \
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
Authorization: Basic MTc4YjkzYzdiODc2NDNhMTdlNWIzYmM2ODJmZmNkMjViZGRiZWY3YTlhMzM4
MGNiZDQzZjNhNThiZjdjMjAwNjozZjQyOWRjNmYzMWZlYzdlMWQzZTJiY2Yz
MDFlODA2MDViNGYzODA4MGRhNjM3NDY5OTI3OTU5OTNhNGJkNjM5

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
	-u 178b93c7b87643a17e5b3bc682ffcd25bddbef7a9a3380cbd43f3a58bf7c2006:3f429dc6f31fec7e1d3e2bcf301e80605b4f38080da63746992795993a4bd639
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e91217e03ea20fd395b0ac4286a46f0429eefa9cecf1b89559cfd1abb6c8354c","client_secret":"7a854ae9cee9de248886ed22e54e5b81047da59d9e81ac5e66a6c6d5243cf106"}
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
  "access_token": "09068b59722afb2b053453bd816f2053cf7c3c4541d183f17603dc5e436c8d7b",
  "token_type": "bearer",
  "created_at": 1476367183
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e91217e03ea20fd395b0ac4286a46f0429eefa9cecf1b89559cfd1abb6c8354c","client_secret":"7a854ae9cee9de248886ed22e54e5b81047da59d9e81ac5e66a6c6d5243cf106"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTg1ZTllOTEwMjNhZjMyNWNlMDAzMWNjZDYyODEzMDA2OGI2NDdhN2UyYzYx
MmIzMThmMTdlYmNhZDBhNjhjMTo3OTllODhkYzEzYWQyYThjYTRlNDFkODg1
MjZiNzkwOTA3MjNkOTMxNzBlNGE2ZGJkZThjNTUxODI0ZWFhYzBi

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
  "access_token": "df91b2c83afc6a60c875bf8d948f3128d4be03fb7afee218f3cadeee2b860a28",
  "token_type": "bearer",
  "created_at": 1476367183
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 985e9e91023af325ce0031ccd628130068b647a7e2c612b318f17ebcad0a68c1:799e88dc13ad2a8ca4e41d88526b79090723d93170e4a6dbde8c551824eaac0b
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
{"grant_type":"client_credentials","client_id":"2e31bfe027f9196488a5c553198d7d5b5ca5db5580b1fe3a378cdfc381a5ef12","client_secret":"92dad65edba4a4c29dab071e9da43b306d302d218463678c7f2acedc8cffe84d"}
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
  "access_token": "0131c27ba045f1407c72af9c98217506e8f485da82fdd2de5677eff790b8f988",
  "token_type": "bearer",
  "created_at": 1476367183
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"2e31bfe027f9196488a5c553198d7d5b5ca5db5580b1fe3a378cdfc381a5ef12","client_secret":"92dad65edba4a4c29dab071e9da43b306d302d218463678c7f2acedc8cffe84d"}' -X POST \
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
GET /v2/campaigns/9
Content-Type: application/json
Authorization: Bearer 58e0ff2e131d381c2d1ca7d5733af01f5ea3316550ca0df8a5599cab49e4b1a8
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
	-H "Authorization: Bearer 58e0ff2e131d381c2d1ca7d5733af01f5ea3316550ca0df8a5599cab49e4b1a8"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/150/flashcards
Content-Type: application/json
Authorization: Bearer 9050013bb839ee9396f791c348b2b61b1c05dfb72fcb0e3e5bf7017532dd2e83
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":150,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 724,
    "chapter_id": 150,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:45.485Z",
    "created_at": "2016-10-13T14:00:45.485Z",
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
curl "api.goskive.com/v2/chapters/150/flashcards" -d '{"flashcard":{"chapter_id":150,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9050013bb839ee9396f791c348b2b61b1c05dfb72fcb0e3e5bf7017532dd2e83"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/149/flashcards
Content-Type: application/json
Authorization: Bearer e14ccde8b8ddaf6fe6b887ebf493d8bdacbe0f5e2729e671eeb73055d1a2d859
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 719,
      "chapter_id": 149,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:45.193Z",
      "created_at": "2016-10-13T14:00:45.193Z",
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
      "author_id": 719,
      "chapter_id": 149,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:45.233Z",
      "created_at": "2016-10-13T14:00:45.233Z",
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
      "id": 79,
      "obfuscated_id": "BFjsqYG0c2I",
      "author_id": 719,
      "chapter_id": 149,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:45.273Z",
      "created_at": "2016-10-13T14:00:45.273Z",
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
	-H "Authorization: Bearer e14ccde8b8ddaf6fe6b887ebf493d8bdacbe0f5e2729e671eeb73055d1a2d859"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/153/questions
Content-Type: application/json
Authorization: Bearer 6ef41d3a8f5a0482077e695554f830df14db459e5e4c4c81a660d67d4a84b6ee
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":153,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 106,
    "obfuscated_id": "GEL902caNek",
    "author_id": 743,
    "chapter_id": 153,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:47.381Z",
    "created_at": "2016-10-13T14:00:47.381Z",
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
        "id": 212,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 213,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 214,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 215,
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
curl "api.goskive.com/v2/chapters/153/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":153,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ef41d3a8f5a0482077e695554f830df14db459e5e4c4c81a660d67d4a84b6ee"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/154/questions
Content-Type: application/json
Authorization: Bearer 9ff50ad6c4550f03097ce6929c9682367d081df8501a5b363c6eab25827c9301
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":154,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 107,
    "obfuscated_id": "_2rgp7tgq8o",
    "author_id": 746,
    "chapter_id": 154,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:47.887Z",
    "created_at": "2016-10-13T14:00:47.887Z",
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
        "id": 216,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 217,
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
curl "api.goskive.com/v2/chapters/154/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":154,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ff50ad6c4550f03097ce6929c9682367d081df8501a5b363c6eab25827c9301"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/155/questions
Content-Type: application/json
Authorization: Bearer faa784753bc495e9998155facec4c57138060a69892ffe7f7959d8417df522d5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":155,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 749,
    "chapter_id": 155,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:48.234Z",
    "created_at": "2016-10-13T14:00:48.234Z",
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
        "id": 218,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 219,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/155/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":155,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faa784753bc495e9998155facec4c57138060a69892ffe7f7959d8417df522d5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/156/questions
Content-Type: application/json
Authorization: Bearer 15b872d8bbb1009186378ecc0dd3d7b4451aeb895c7820ad319263604e51dd2c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":156,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 109,
    "obfuscated_id": "VSPyck5c2RY",
    "author_id": 752,
    "chapter_id": 156,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:48.571Z",
    "created_at": "2016-10-13T14:00:48.571Z",
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
        "id": 220,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 221,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 222,
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
curl "api.goskive.com/v2/chapters/156/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":156,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15b872d8bbb1009186378ecc0dd3d7b4451aeb895c7820ad319263604e51dd2c"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/157/questions
Content-Type: application/json
Authorization: Bearer 09d35bb753461cab509b200d55a216c55444f29974dfacf71e8276f3254ac586
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
      "id": 110,
      "obfuscated_id": "55JK4PuG2Hk",
      "author_id": 755,
      "chapter_id": 157,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:49.085Z",
      "created_at": "2016-10-13T14:00:48.967Z",
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
          "id": 223,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 224,
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
      "author_id": 756,
      "chapter_id": 157,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:49.285Z",
      "created_at": "2016-10-13T14:00:49.159Z",
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
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 757,
      "chapter_id": 157,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T14:00:49.491Z",
      "created_at": "2016-10-13T14:00:49.364Z",
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
          "id": 227,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 228,
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
curl "api.goskive.com/v2/chapters/157/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09d35bb753461cab509b200d55a216c55444f29974dfacf71e8276f3254ac586"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/39
Content-Type: application/json
Authorization: Bearer 8811ffcaef29af63a7c54c6c97757de3036c51bf88adf1d52b20eb9d3c1c030b
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
curl "api.goskive.com/v2/chapters/39" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8811ffcaef29af63a7c54c6c97757de3036c51bf88adf1d52b20eb9d3c1c030b"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/41
Content-Type: application/json
Authorization: Bearer d5cfd7df31fa342b78ebde798b74b056a5ef95f80d7e3edc64729a624b182790
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
curl "api.goskive.com/v2/chapters/41" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5cfd7df31fa342b78ebde798b74b056a5ef95f80d7e3edc64729a624b182790"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/43
Content-Type: application/json
Authorization: Bearer b1aa5ee221048e744d04fe94ae5d5bd96288747907bb8b9d74f9aef3049a7721
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
curl "api.goskive.com/v2/chapters/43" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1aa5ee221048e744d04fe94ae5d5bd96288747907bb8b9d74f9aef3049a7721"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/40
Content-Type: application/json
Authorization: Bearer fe7f6ac42185ae82e83c8ac10bb30f0c6d242d4d8de513b38089cb23f20ffd2b
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe7f6ac42185ae82e83c8ac10bb30f0c6d242d4d8de513b38089cb23f20ffd2b"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/46
Content-Type: application/json
Authorization: Bearer d8f8801af3a5071df681cef2be56a82789c8dbc64a86dfa6c4c6ead4c341ce0b
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
    "id": 46,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T14:00:11.787Z",
    "course_id": 140,
    "author_id": 336,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-13T14:00:11.157Z",
    "questions_updated_at": "2016-10-13T14:00:11.157Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 340,
        "chapter_id": 46,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:11.766Z",
        "created_at": "2016-10-13T14:00:11.766Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 338,
        "chapter_id": 46,
        "position": 42,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T14:00:11.642Z",
        "created_at": "2016-10-13T14:00:11.490Z",
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
            "id": 83,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 84,
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
curl "api.goskive.com/v2/chapters/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8f8801af3a5071df681cef2be56a82789c8dbc64a86dfa6c4c6ead4c341ce0b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/45
Content-Type: application/json
Authorization: Bearer 20e40ae6aff00977d32f7c38ea0fffe0862cfd7d8732f847cd5215340b4cf818
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
    "id": 45,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T14:00:11.120Z",
    "course_id": 139,
    "author_id": 334,
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
curl "api.goskive.com/v2/chapters/45" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20e40ae6aff00977d32f7c38ea0fffe0862cfd7d8732f847cd5215340b4cf818"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/54/replies
Content-Type: application/json
Authorization: Bearer 2a465f189a101974101a41cd3ba0b38d23fe7d5f55624165de6bd67b28545579
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
    "author_id": 734,
    "reply_to_id": 54,
    "created_at": "2016-10-13T14:00:46.225Z",
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
	-H "Authorization: Bearer 2a465f189a101974101a41cd3ba0b38d23fe7d5f55624165de6bd67b28545579"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/53/replies
Content-Type: application/json
Authorization: Bearer a0221f63304bc9a878201ea9ea5ae29775143759c6c0d5adf161e23911ab0a6d
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
curl "api.goskive.com/v2/comments/53/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0221f63304bc9a878201ea9ea5ae29775143759c6c0d5adf161e23911ab0a6d"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer 6f45d3831651122b2debcc7f699afe11ca124ce19b4b740005f0a9b1dc72c42d
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
curl "api.goskive.com/v2/comments/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f45d3831651122b2debcc7f699afe11ca124ce19b4b740005f0a9b1dc72c42d"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/1/republish
Content-Type: application/json
Authorization: Bearer 239079f8d603048ea1294eb5aca05c0a14242d6b3c558ad12463e1401c88ddd3
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
curl "api.goskive.com/v2/comments/1/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 239079f8d603048ea1294eb5aca05c0a14242d6b3c558ad12463e1401c88ddd3"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 05789ef89b439fa701a505e96f8b72fbc7fbc76543955477bda1f3367e3947a3
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05789ef89b439fa701a505e96f8b72fbc7fbc76543955477bda1f3367e3947a3"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/41/report
Content-Type: application/json
Authorization: Bearer 65a47abc8b56c64d36de7b9a370a62d66854d9c983bea195a7dcc91fff866938
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/41/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65a47abc8b56c64d36de7b9a370a62d66854d9c983bea195a7dcc91fff866938"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/17
Content-Type: application/json
Authorization: Bearer 65524542d89d64962fac1d030800c7ec998019f5cbc4b35593d8b1087e9dcde4
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
    "id": 17,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-13T14:00:00.256Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/17" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65524542d89d64962fac1d030800c7ec998019f5cbc4b35593d8b1087e9dcde4"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 90ead380457d39683d3190375ae7bce4c4bcb1a3eed347082de3abd8d9f074be
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
      "id": 14,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T14:00:00.126Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T14:00:00.131Z"
    },
    {
      "id": 16,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T14:00:00.135Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90ead380457d39683d3190375ae7bce4c4bcb1a3eed347082de3abd8d9f074be"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/35/company_profiles
Content-Type: application/json
Authorization: Bearer 4fe99dd1b0a2a22843caa5b68d6ef5afa0dd699b16375c2dfe01bfdb18a3c53e
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
curl "api.goskive.com/v2/companies/35/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fe99dd1b0a2a22843caa5b68d6ef5afa0dd699b16375c2dfe01bfdb18a3c53e"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/34/company_profiles
Content-Type: application/json
Authorization: Bearer 3b6c3dbe192a574009a96fd98cf2ad5a693d76bc90729cbbd545d604c064f7b8
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
curl "api.goskive.com/v2/companies/34/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b6c3dbe192a574009a96fd98cf2ad5a693d76bc90729cbbd545d604c064f7b8"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 46ed0db44014dfbf394bb3e4ffd174cd49f7e55c09afb01674f0f80bb34914d3
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
	-H "Authorization: Bearer 46ed0db44014dfbf394bb3e4ffd174cd49f7e55c09afb01674f0f80bb34914d3"
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
Authorization: Bearer cb5e3d0a4abd6ff6ef1a37ee93faf37f7802f12e929e8ac7b4a04232f4e92248
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
	-H "Authorization: Bearer cb5e3d0a4abd6ff6ef1a37ee93faf37f7802f12e929e8ac7b4a04232f4e92248"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 366ab0dd8f971922154ac87ff5ee8f41cbccfb026a25e6ec57e999e609a458b9
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
    "id": 50,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T14:00:14.424Z",
    "course_id": 150,
    "author_id": 372,
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
	-H "Authorization: Bearer 366ab0dd8f971922154ac87ff5ee8f41cbccfb026a25e6ec57e999e609a458b9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 763d513675804396b3d92d001655ad6bc7b8b83d3ba89e4b52892f6a92ec997b
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
      "updated_at": "2016-10-13T14:00:14.961Z",
      "course_id": 154,
      "author_id": 383,
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
      "updated_at": "2016-10-13T14:00:14.988Z",
      "course_id": 154,
      "author_id": 384,
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
      "updated_at": "2016-10-13T14:00:15.312Z",
      "course_id": 154,
      "author_id": 385,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T14:00:14.884Z",
      "questions_updated_at": "2016-10-13T14:00:14.884Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 763d513675804396b3d92d001655ad6bc7b8b83d3ba89e4b52892f6a92ec997b"
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
      "id": 66,
      "title": "Clever Chapter Title 51",
      "position": 1,
      "updated_at": "2016-10-13T14:00:16.582Z",
      "course_id": 160,
      "author_id": 411,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 67,
      "title": "Clever Chapter Title 52",
      "position": 2,
      "updated_at": "2016-10-13T14:00:16.609Z",
      "course_id": 160,
      "author_id": 412,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 68,
      "title": "Clever Chapter Title 53",
      "position": 3,
      "updated_at": "2016-10-13T14:00:16.917Z",
      "course_id": 160,
      "author_id": 413,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T14:00:16.505Z",
      "questions_updated_at": "2016-10-13T14:00:16.505Z",
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
Authorization: Bearer 423d1eb64137e212107bf3371fc647688bf9667e1ea53542e5332431340559b5
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
      "updated_at": "2016-10-13T14:00:15.574Z",
      "course_id": 156,
      "author_id": 392,
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
      "updated_at": "2016-10-13T14:00:15.603Z",
      "course_id": 156,
      "author_id": 393,
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
      "updated_at": "2016-10-13T14:00:15.631Z",
      "course_id": 156,
      "author_id": 394,
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
	-H "Authorization: Bearer 423d1eb64137e212107bf3371fc647688bf9667e1ea53542e5332431340559b5"
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
      "id": 69,
      "title": "Clever Chapter Title 54",
      "position": 1,
      "updated_at": "2016-10-13T14:00:17.114Z",
      "course_id": 162,
      "author_id": 418,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 70,
      "title": "Clever Chapter Title 55",
      "position": 2,
      "updated_at": "2016-10-13T14:00:17.141Z",
      "course_id": 162,
      "author_id": 419,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 71,
      "title": "Clever Chapter Title 56",
      "position": 3,
      "updated_at": "2016-10-13T14:00:17.167Z",
      "course_id": 162,
      "author_id": 420,
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
Authorization: Bearer 4a192ec555175b8f9c3331e1529eea5876bfcd372e9a838db6e7af4ad6dd8138
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
    "course_id": 72,
    "user_id": 191,
    "updated_at": "2016-10-13T13:59:59.429Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a192ec555175b8f9c3331e1529eea5876bfcd372e9a838db6e7af4ad6dd8138"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f1270e53a57a4bb4517f608d0d89cdcc360ccf8c633227fca6f2dce365499d99
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
      "id": 6,
      "course_id": 76,
      "user_id": 201,
      "updated_at": "2016-10-13T13:59:59.927Z"
    },
    {
      "id": 7,
      "course_id": 76,
      "user_id": 202,
      "updated_at": "2016-10-13T13:59:59.943Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1270e53a57a4bb4517f608d0d89cdcc360ccf8c633227fca6f2dce365499d99"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/235/files
Content-Type: application/json
Authorization: Bearer ae4964ac4ed639931f38ae1d75b38e0029479cc674072006c65a2ff7defa48d2
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
        "id": 672,
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
        "created_at": "2016-10-13T14:00:41.623Z",
        "updated_at": "2016-10-13T14:00:41.623Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T14:00:41.630Z",
      "updated_at": "2016-10-13T14:00:41.630Z",
      "course_id": 235,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
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
        "created_at": "2016-10-13T14:00:41.637Z",
        "updated_at": "2016-10-13T14:00:41.637Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T14:00:41.644Z",
      "updated_at": "2016-10-13T14:00:41.644Z",
      "course_id": 235,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
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
        "created_at": "2016-10-13T14:00:41.651Z",
        "updated_at": "2016-10-13T14:00:41.651Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T14:00:41.657Z",
      "updated_at": "2016-10-13T14:00:41.657Z",
      "course_id": 235,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/235/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae4964ac4ed639931f38ae1d75b38e0029479cc674072006c65a2ff7defa48d2"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/237/files
Content-Type: application/json
Authorization: Bearer d70257936fb7624a96cf94ae0e97402d1156ffeb1a43406046d41fcebe7c73a6
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
    "id": 6,
    "uploader": {
      "id": 679,
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
      "created_at": "2016-10-13T14:00:41.881Z",
      "updated_at": "2016-10-13T14:00:41.881Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-13T14:00:41.913Z",
    "updated_at": "2016-10-13T14:00:41.913Z",
    "course_id": 237,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/237/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d70257936fb7624a96cf94ae0e97402d1156ffeb1a43406046d41fcebe7c73a6"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/236/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 596279c0e02b145353b7da5120386fd4686d38e77de058aaca59e6a08f2a81bd
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
    "key": "cache/753bd8be3777e3de9e2382f07fb86b22.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxNTowMDo0MVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS83NTNiZDhiZTM3NzdlM2RlOWUyMzgyZjA3ZmI4NmIyMi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTQwMDQxWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T140041Z",
    "x-amz-signature": "a9bc09746305b5699bd45c5ed6779e0e1ef12930070a16cbd5a0d21ef4414f10"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/236/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 596279c0e02b145353b7da5120386fd4686d38e77de058aaca59e6a08f2a81bd"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 70c8c62ca5cc4da0f703a511c15ebdac3196781f4504d99d07acfa4813771bb1
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
	-H "Authorization: Bearer 70c8c62ca5cc4da0f703a511c15ebdac3196781f4504d99d07acfa4813771bb1"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 486d2ee9141769c669287539c77c46236abc301e041ecb700c3595a245b1914c
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
	-H "Authorization: Bearer 486d2ee9141769c669287539c77c46236abc301e041ecb700c3595a245b1914c"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6ca49588cfdea4072e46bf916855f21a8ec1ef617d4fdc3343ef1439c88858ae
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
	-H "Authorization: Bearer 6ca49588cfdea4072e46bf916855f21a8ec1ef617d4fdc3343ef1439c88858ae"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 026d12a41d76a8a09eec5fbeee170b3dc0a9d748fa28dd468bb4f857094e8197
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
	-H "Authorization: Bearer 026d12a41d76a8a09eec5fbeee170b3dc0a9d748fa28dd468bb4f857094e8197"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e32efb7d952cea37bc9137dedd720b7e7b47b658e99029ae9c8bfcf527c429dc
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
	-H "Authorization: Bearer e32efb7d952cea37bc9137dedd720b7e7b47b658e99029ae9c8bfcf527c429dc"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer bcb2493ddcef698d59ea3a166137bc5e75ece597f25c208f3bfa72f1af837fc3
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
    "creator_id": 48,
    "id": 19,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 19,
    "additional_university_ids": [

    ],
    "topic_id": 22,
    "discipline_id": 22,
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
    "chapters_updated_at": "2016-10-13T13:59:47.280Z",
    "updated_at": "2016-10-13T13:59:48.778Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 7,
        "title": "Clever Chapter Title 7",
        "position": 1,
        "updated_at": "2016-10-13T13:59:48.731Z",
        "course_id": 19,
        "author_id": 48,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:59:47.280Z",
        "questions_updated_at": "2016-10-13T13:59:47.280Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 8,
        "title": "Clever Chapter Title 8",
        "position": 2,
        "updated_at": "2016-10-13T13:59:48.771Z",
        "course_id": 19,
        "author_id": 48,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:59:47.280Z",
        "questions_updated_at": "2016-10-13T13:59:47.280Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 49,
        "chapter_id": 7,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:48.560Z",
        "created_at": "2016-10-13T13:59:48.560Z",
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
        "id": 11,
        "obfuscated_id": "KS_N8rRWCuE",
        "author_id": 49,
        "chapter_id": 8,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:48.637Z",
        "created_at": "2016-10-13T13:59:48.637Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 49,
        "chapter_id": 7,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:48.604Z",
        "created_at": "2016-10-13T13:59:48.604Z",
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
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 49,
        "chapter_id": 8,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:48.680Z",
        "created_at": "2016-10-13T13:59:48.680Z",
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
        "author_id": 49,
        "chapter_id": 7,
        "position": 9,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:47.506Z",
        "created_at": "2016-10-13T13:59:47.385Z",
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
        "author_id": 49,
        "chapter_id": 7,
        "position": 10,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:47.687Z",
        "created_at": "2016-10-13T13:59:47.571Z",
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
        "author_id": 49,
        "chapter_id": 8,
        "position": 11,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:47.903Z",
        "created_at": "2016-10-13T13:59:47.775Z",
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
        "author_id": 49,
        "chapter_id": 8,
        "position": 12,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:48.091Z",
        "created_at": "2016-10-13T13:59:47.971Z",
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
	-H "Authorization: Bearer bcb2493ddcef698d59ea3a166137bc5e75ece597f25c208f3bfa72f1af837fc3"
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
    "creator_id": 54,
    "id": 20,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 20,
    "additional_university_ids": [

    ],
    "topic_id": 23,
    "discipline_id": 23,
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
    "chapters_updated_at": "2016-10-13T13:59:48.914Z",
    "updated_at": "2016-10-13T13:59:50.449Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 9,
        "title": "Clever Chapter Title 9",
        "position": 1,
        "updated_at": "2016-10-13T13:59:50.372Z",
        "course_id": 20,
        "author_id": 54,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:59:48.914Z",
        "questions_updated_at": "2016-10-13T13:59:48.914Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 10,
        "title": "Clever Chapter Title 10",
        "position": 2,
        "updated_at": "2016-10-13T13:59:50.442Z",
        "course_id": 20,
        "author_id": 54,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:59:48.914Z",
        "questions_updated_at": "2016-10-13T13:59:48.914Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 54,
        "chapter_id": 9,
        "position": 15,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:49.133Z",
        "created_at": "2016-10-13T13:59:49.009Z",
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
            "id": 29,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 30,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 54,
        "chapter_id": 10,
        "position": 17,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:59:49.536Z",
        "created_at": "2016-10-13T13:59:49.408Z",
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
            "id": 33,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 34,
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
PUT /v2/courses/23/pin
Content-Type: application/json
Authorization: Bearer 28849b4ad5490065780516e0fcc6513be9f8d4374ed620b2244e5443ae10cf2d
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/23/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28849b4ad5490065780516e0fcc6513be9f8d4374ed620b2244e5443ae10cf2d"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/22/pin
Content-Type: application/json
Authorization: Bearer cb3f31648ab223250369eebf2ec58c616baead292e7764e4b41fa6c1c67543bc
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/22/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb3f31648ab223250369eebf2ec58c616baead292e7764e4b41fa6c1c67543bc"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 93a3ba0698e46bb199d2d07d0ecbe7983117559c763aa8cf1b38b3508bc36cd8
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
    "creator_id": 19,
    "id": 7,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 7,
    "additional_university_ids": [

    ],
    "topic_id": 10,
    "discipline_id": 10,
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
    "updated_at": "2016-10-13T13:59:43.868Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93a3ba0698e46bb199d2d07d0ecbe7983117559c763aa8cf1b38b3508bc36cd8"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1295d066d879c70ef7411f3884ca4e32c5de53665ca1ed426fe57023064626e6
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
    "id": 361,
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
    "created_at": "2016-10-13T14:00:13.384Z",
    "updated_at": "2016-10-13T14:00:13.384Z",
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
	-H "Authorization: Bearer 1295d066d879c70ef7411f3884ca4e32c5de53665ca1ed426fe57023064626e6"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer cbb07ba6203df0930cab0a4705b68d0a7b998d2a200330b8e5930b45ab6b716d
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[154]}
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
    "id": 363,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      154
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T14:00:13.787Z",
    "updated_at": "2016-10-13T14:00:13.823Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[154]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbb07ba6203df0930cab0a4705b68d0a7b998d2a200330b8e5930b45ab6b716d"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b064a59d707c66a011b6455a33c104b3a2d62f114fcb2c5f5ad517aaea5c9cf0
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
    "id": 364,
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
    "created_at": "2016-10-13T14:00:13.843Z",
    "updated_at": "2016-10-13T14:00:13.843Z",
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
	-H "Authorization: Bearer b064a59d707c66a011b6455a33c104b3a2d62f114fcb2c5f5ad517aaea5c9cf0"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 430d821a2e3d3297437e6a484ef6d3ebdd0978796ed10017dcef418fc0b05a56
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[156]}
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
    "id": 365,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      156
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T14:00:13.937Z",
    "updated_at": "2016-10-13T14:00:13.937Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[156]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 430d821a2e3d3297437e6a484ef6d3ebdd0978796ed10017dcef418fc0b05a56"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 3e07f37e5caafeb83de146494994f5441e5cfd90cca5f2a9cde40c2b611d22b4
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

153
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
    "id": 362,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9e10f25e4569062340f56deb63dafc6b27ada7e8.jpg",
    "university_id": null,
    "fields_of_study": [
      153
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T14:00:13.470Z",
    "updated_at": "2016-10-13T14:00:13.734Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/d1fb90d8bb5af9d181f9ddf40d7ac7693779a0db.jpg",
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

153
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 3e07f37e5caafeb83de146494994f5441e5cfd90cca5f2a9cde40c2b611d22b4"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 852d7a3691e9f1af460b5b40abe6a72c1b5ffdc3ee220dd0f0f72df024c71cf2
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
      "bookmarkable_id": 32,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 33,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 34,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 852d7a3691e9f1af460b5b40abe6a72c1b5ffdc3ee220dd0f0f72df024c71cf2"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1fe105c17c03269b99fe2cc588feea8b185e8d8b18a465f41a1c7b018b972cb3
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
      "company_id": 30,
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
      "company_id": 31,
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
	-H "Authorization: Bearer 1fe105c17c03269b99fe2cc588feea8b185e8d8b18a465f41a1c7b018b972cb3"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a08d964341dc09aab6473cbbca69495ca313931e1ec0a7abe55cabf7123bab7d
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
      "company_id": 26,
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
	-H "Authorization: Bearer a08d964341dc09aab6473cbbca69495ca313931e1ec0a7abe55cabf7123bab7d"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 0dbc52af556545843ca4a19fbacf69626eb0d5f22c328dfc7cc1dc8d428959dc
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
      "creator_id": 188,
      "id": 70,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-51",
      "html_url": "https://goskive.com/course/mit-course-51",
      "slug": "mit-course-51",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 51",
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
      "updated_at": "2016-10-13T13:59:59.175Z",
      "shortname": "mit-course-51"
    },
    {
      "creator_id": 189,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-52",
      "html_url": "https://goskive.com/course/mit-course-52",
      "slug": "mit-course-52",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 76,
      "discipline_id": 76,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 52",
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
      "updated_at": "2016-10-13T13:59:59.258Z",
      "shortname": "mit-course-52"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dbc52af556545843ca4a19fbacf69626eb0d5f22c328dfc7cc1dc8d428959dc"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a2f00584822b37938e1363d1a9ba15bd1d4bc54e29cb4537ff655071ae728e39
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
      "company_id": 23,
      "company": {
        "id": 23,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T14:00:46.652Z"
      },
      "created_at": "2016-10-13T14:00:46.656Z",
      "updated_at": "2016-10-13T14:00:46.656Z",
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
      "company_id": 24,
      "company": {
        "id": 24,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T14:00:46.664Z"
      },
      "created_at": "2016-10-13T14:00:46.667Z",
      "updated_at": "2016-10-13T14:00:46.667Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2f00584822b37938e1363d1a9ba15bd1d4bc54e29cb4537ff655071ae728e39"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 4858b0bd1d5a6349909847791d4677977d71fcaaae0dfa90b621743f969c62b8
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
      "company_id": 19,
      "company": {
        "id": 19,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T14:00:46.437Z"
      },
      "created_at": "2016-10-13T14:00:46.442Z",
      "updated_at": "2016-10-13T14:00:46.442Z",
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
      "company_id": 20,
      "company": {
        "id": 20,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T14:00:46.457Z"
      },
      "created_at": "2016-10-13T14:00:46.460Z",
      "updated_at": "2016-10-13T14:00:46.460Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4858b0bd1d5a6349909847791d4677977d71fcaaae0dfa90b621743f969c62b8"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 191057e00735846134e544ed90aa1b9b3feb34c9ba08b98d010d14513634d131
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
      "created_at": "2016-10-13T14:00:42.378Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 50,
      "updated_at": "2016-10-13T14:00:42.496Z",
      "author_id": "685",
      "thread_subject_id": "239",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-13T14:00:42.483Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 51,
      "updated_at": "2016-10-13T14:00:42.500Z",
      "author_id": "688",
      "thread_subject_id": "240",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-13T14:00:42.870Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-13T14:00:42.870Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-13T14:00:43.250Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-13T14:00:43.250Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-13T14:00:43.628Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-10-13T14:00:43.628Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-13T14:00:43.931Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 101,
      "updated_at": "2016-10-13T14:00:43.931Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-13T14:00:44.263Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 102,
      "updated_at": "2016-10-13T14:00:44.263Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-13T14:00:44.558Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 103,
      "updated_at": "2016-10-13T14:00:44.558Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 191057e00735846134e544ed90aa1b9b3feb34c9ba08b98d010d14513634d131"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/23
Content-Type: application/json
Authorization: Bearer 0af8700eee06cb0958b0446c113b3a54a3b0f525c217dd0784ee3fcd5ce2b245
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-13T13:50:44.000Z"}}
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
    "id": 23,
    "created_at": "2016-10-13T14:00:44.764Z",
    "read_at": "2016-10-13T13:50:44.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 52,
    "updated_at": "2016-10-13T14:00:44.807Z",
    "author_id": "714",
    "thread_subject_id": "247",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/23" -d '{"notification":{"read_at":"2016-10-13T13:50:44.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0af8700eee06cb0958b0446c113b3a54a3b0f525c217dd0784ee3fcd5ce2b245"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer bca99ffd58179eadeeb7400ce6dfab10f69f328494ceb9f5a909abac2fb0a263
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
      "course_id": 142,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T14:00:12.701Z",
      "course_published": true,
      "updated_at": "2016-10-13T14:00:12.692Z"
    },
    {
      "id": 5,
      "course_id": 143,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T14:00:12.783Z",
      "course_published": true,
      "updated_at": "2016-10-13T14:00:12.774Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bca99ffd58179eadeeb7400ce6dfab10f69f328494ceb9f5a909abac2fb0a263"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer f9694e6260a69700fba86dc764f7ea36b15b73dd3517f666c46d46f35cab1067
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
    "id": 8,
    "course_id": 147,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T14:00:13.335Z",
    "course_published": true,
    "updated_at": "2016-10-13T14:00:13.327Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9694e6260a69700fba86dc764f7ea36b15b73dd3517f666c46d46f35cab1067"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer d6b3d05510db38cc35515df833ed106ee675b7d7773b53ef3401e53810433f20
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
    "id": 7,
    "course_id": 146,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-13T14:00:13.237Z",
    "course_published": true,
    "updated_at": "2016-10-13T14:00:13.225Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6b3d05510db38cc35515df833ed106ee675b7d7773b53ef3401e53810433f20"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3ffc7762b0c11153c189e8e2f565d98007987844cbfdf288557ce101c7fc023c
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
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 35,
      "user_id": 302
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 36,
      "user_id": 302
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 37,
      "user_id": 302
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 38,
      "user_id": 302
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ffc7762b0c11153c189e8e2f565d98007987844cbfdf288557ce101c7fc023c"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/258
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
    "id": 258,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 258,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 258
      },
      {
        "id": 259,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 258
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/258" -X GET \
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
      "id": 259,
      "name": "Re-contextualized modular synergy",
      "name_translations": {
        "en": "Re-contextualized modular synergy"
      }
    },
    {
      "id": 260,
      "name": "Total tertiary forecast",
      "name_translations": {
        "en": "Total tertiary forecast"
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
PATCH /v2/feedbacks/22/close
Content-Type: application/json
Authorization: Bearer abb96815ebe0de124e570b42b2a0efac14d9e41d56999430c1d7b567ed8752e4
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
    "id": 22,
    "user_id": 799,
    "feedbackable_id": 86,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-13T14:00:51.944Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/22/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abb96815ebe0de124e570b42b2a0efac14d9e41d56999430c1d7b567ed8752e4"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer 1a3f2e33c8dfc5c65c8f2cd27daa7a2097c2dc7a5c0937b04d25673c77d2a1ef
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
    "id": 26,
    "user_id": 819,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-13T14:00:53.103Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a3f2e33c8dfc5c65c8f2cd27daa7a2097c2dc7a5c0937b04d25673c77d2a1ef"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/18
Content-Type: application/json
Authorization: Bearer dfd774bd5b9fb1ecb721ded68626250f3a2346d199a1c3a195bed148a19578f3
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
    "user_id": 777,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T14:00:50.903Z",
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
	-H "Authorization: Bearer dfd774bd5b9fb1ecb721ded68626250f3a2346d199a1c3a195bed148a19578f3"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer d29fb61cae496fe55a414ab50d94d37ad404601fd824fc4e9202e8cf76c10759
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
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d29fb61cae496fe55a414ab50d94d37ad404601fd824fc4e9202e8cf76c10759"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer e3f17183da8cadf37921802b4db5dd6d486f9bf161eb4330ebbe0e2da8ccde9c
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
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3f17183da8cadf37921802b4db5dd6d486f9bf161eb4330ebbe0e2da8ccde9c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer 91caa085bd828abbd1a38b17410963120d366d0cadde8757ca5f460e0580c299
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
	-H "Authorization: Bearer 91caa085bd828abbd1a38b17410963120d366d0cadde8757ca5f460e0580c299"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer 69778654cce66f60d81a2631aadc93e0a718bc66c346d66a84141827ba5d941c
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
    "user_id": 782,
    "feedbackable_id": 83,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T14:00:51.199Z",
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
	-H "Authorization: Bearer 69778654cce66f60d81a2631aadc93e0a718bc66c346d66a84141827ba5d941c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/10
Authorization: Bearer 7da4db172d2b049446a2869e73620472c49e18fdfbb9730c78c9763b11b62e38
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
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Authorization: Bearer 7da4db172d2b049446a2869e73620472c49e18fdfbb9730c78c9763b11b62e38" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Authorization: Bearer 0e7831766b4d385a517b5019a80615552e0dee5f835de84c988dea2a00551053
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Authorization: Bearer 0e7831766b4d385a517b5019a80615552e0dee5f835de84c988dea2a00551053" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/13
Authorization: Bearer 5897761f3a2f3675b84dc4bb833ef2b22769d3fbb514a408042b60f1da2bdf24
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/0a387b44eaa541a1a8c8f50ac9ce4b62.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T140103Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=42accba3694211b8e2a520ececd33672406ea6bd5d26bfc93dad44c391b1ca38"
  }
}
```



```shell
curl "api.goskive.com/v2/files/13" -X GET \
	-H "Authorization: Bearer 5897761f3a2f3675b84dc4bb833ef2b22769d3fbb514a408042b60f1da2bdf24"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer 0c1507a99021c1e3c23e2dfebdda1694928873d76ebdbc11d59244e808c40dba
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
    "id": 7,
    "uploader": {
      "id": 927,
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
      "created_at": "2016-10-13T14:01:02.772Z",
      "updated_at": "2016-10-13T14:01:02.772Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-13T14:01:02.851Z",
    "updated_at": "2016-10-13T14:01:02.851Z",
    "course_id": 298,
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
	-H "Authorization: Bearer 0c1507a99021c1e3c23e2dfebdda1694928873d76ebdbc11d59244e808c40dba" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses
Authorization: Bearer ab7db182e7ca86b6ad7176d444fdf73ca5a974fb128a7579fee40211ec2f6ba7
```

`GET /v2/files/:file_id/matched_courses`

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
      "creator_id": 656,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 210,
      "additional_university_ids": [

      ],
      "topic_id": 241,
      "discipline_id": 241,
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
      "chapters_updated_at": "2016-10-13T14:00:38.998Z",
      "updated_at": "2016-10-13T14:00:40.701Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 661,
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-4929d00c-7ea1-44ad-af00-ad7b76b5f85e",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-4929d00c-7ea1-44ad-af00-ad7b76b5f85e",
      "slug": "mit-the-great-british-bake-off-4929d00c-7ea1-44ad-af00-ad7b76b5f85e",
      "university_id": 211,
      "additional_university_ids": [

      ],
      "topic_id": 242,
      "discipline_id": 242,
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
      "chapters_updated_at": "2016-10-13T14:00:38.998Z",
      "updated_at": "2016-10-13T14:00:41.271Z",
      "shortname": "mit-the-great-british-bake-off-4929d00c-7ea1-44ad-af00-ad7b76b5f85e"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses" -X GET \
	-H "Authorization: Bearer ab7db182e7ca86b6ad7176d444fdf73ca5a974fb128a7579fee40211ec2f6ba7"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/8/preview
Authorization: Bearer cce126aa959cbba81f84576a91934e5aebc9e7d7021c5303a0c94f27dd31e370
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/e54f3c3e34337d9d17895e4bea55e84b.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T140103Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=95745faf9e408ca72e78132f8d3c34d669677916b605fa9504f42801d61b60e8"
  }
}
```



```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Authorization: Bearer cce126aa959cbba81f84576a91934e5aebc9e7d7021c5303a0c94f27dd31e370"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/12/report
Authorization: Bearer 285471d372da593922965e81dcab8c5b38fca390e6f837b46d446bdf41670d8a
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
curl "api.goskive.com/v2/files/12/report" -d '' -X PUT \
	-H "Authorization: Bearer 285471d372da593922965e81dcab8c5b38fca390e6f837b46d446bdf41670d8a" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/91/comments
Content-Type: application/json
Authorization: Bearer 01d6c657c9491f9445774c4299a0b7d7b5ef3652e0af362ada063bfed399ef66
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
    "id": 57,
    "author_id": 910,
    "reply_to_id": null,
    "created_at": "2016-10-13T14:01:01.728Z",
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
	-H "Authorization: Bearer 01d6c657c9491f9445774c4299a0b7d7b5ef3652e0af362ada063bfed399ef66"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/93/comments
Content-Type: application/json
Authorization: Bearer cd21e720a73fb9dccb7ef929729ac09fa5eba7d3cac67b38ede9f95253a71cbe
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
    "id": 58,
    "author_id": 916,
    "reply_to_id": null,
    "created_at": "2016-10-13T14:01:02.233Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 916,
      "feedbackable_id": 93,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:01:02.230Z",
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
curl "api.goskive.com/v2/flashcards/93/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd21e720a73fb9dccb7ef929729ac09fa5eba7d3cac67b38ede9f95253a71cbe"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/94/comments
Content-Type: application/json
Authorization: Bearer b87e839dbb033924c0ea2e3c92c9a11c7e0cd7f2d92de997a4c1317aa2e38164
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
      "id": 60,
      "author_id": 923,
      "reply_to_id": null,
      "created_at": "2016-10-13T14:01:02.551Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 922,
      "reply_to_id": null,
      "created_at": "2016-10-13T14:01:02.535Z",
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
curl "api.goskive.com/v2/flashcards/94/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b87e839dbb033924c0ea2e3c92c9a11c7e0cd7f2d92de997a4c1317aa2e38164"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/92/comments
Content-Type: application/json
Authorization: Bearer cfb68d38e2603421387a4579860b5aa0600b365344ac0610a460e0ed1ce0f29b
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
curl "api.goskive.com/v2/flashcards/92/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfb68d38e2603421387a4579860b5aa0600b365344ac0610a460e0ed1ce0f29b"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/30/feedbacks
Content-Type: application/json
Authorization: Bearer 5ec316e3fd57594b0a8ffb66657bea3f11e9ffeba534153bc3e163ccbbeeb947
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
    "user_id": 209,
    "feedbackable_id": 30,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T14:00:00.510Z",
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
curl "api.goskive.com/v2/flashcards/30/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ec316e3fd57594b0a8ffb66657bea3f11e9ffeba534153bc3e163ccbbeeb947"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/34/feedbacks
Content-Type: application/json
Authorization: Bearer e3a4cf45a1239d4ef70609d42ecf5c7cdf3517a621b8260416e70402734d1cf7
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
      "user_id": 227,
      "feedbackable_id": 34,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:01.577Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 226,
      "feedbackable_id": 34,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:01.565Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/34/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3a4cf45a1239d4ef70609d42ecf5c7cdf3517a621b8260416e70402734d1cf7"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer f34b7637f5ddfdb72aa4bc5c058c95760ecd19f61385aa47e2ba1d36502835c9
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 79
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 78
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 77
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f34b7637f5ddfdb72aa4bc5c058c95760ecd19f61385aa47e2ba1d36502835c9"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/52/republish
Content-Type: application/json
Authorization: Bearer 706df3dd4a141159478403aaf6b798ae0b44e976554d615cc22dca9194ab4c2f
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
curl "api.goskive.com/v2/flashcards/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 706df3dd4a141159478403aaf6b798ae0b44e976554d615cc22dca9194ab4c2f"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/70/bookmark
Content-Type: application/json
Authorization: Bearer 720061111dda258643c29d1e305d555e04741e6908608f9793dbc2f5ff1251ea
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/70/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 720061111dda258643c29d1e305d555e04741e6908608f9793dbc2f5ff1251ea"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/72
Content-Type: application/json
Authorization: Bearer 1226079644a3734d7afb1e310e3b81a137da887738851cc8ed641615c4948973
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1226079644a3734d7afb1e310e3b81a137da887738851cc8ed641615c4948973"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/71/downvote
Content-Type: application/json
Authorization: Bearer 59e87296c1b5e0902d2f3d331dbf08bff1e54e3b0518b54541d7dd5e8a236f38
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/71/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59e87296c1b5e0902d2f3d331dbf08bff1e54e3b0518b54541d7dd5e8a236f38"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/68
Content-Type: application/json
Authorization: Bearer ed384b55ec591779f183658a7f179914712aa4d94151c41bcbc3257d1e75961d
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
    "author_id": 628,
    "chapter_id": 132,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:37.837Z",
    "created_at": "2016-10-13T14:00:37.837Z",
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
	-H "Authorization: Bearer ed384b55ec591779f183658a7f179914712aa4d94151c41bcbc3257d1e75961d"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/report
Content-Type: application/json
Authorization: Bearer 394ccb25cef6d5bb064fb302d121702ca412edbbaea62c2ba85cb848d706559f
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 394ccb25cef6d5bb064fb302d121702ca412edbbaea62c2ba85cb848d706559f"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50/bookmark
Content-Type: application/json
Authorization: Bearer 7caad477a7d0334cff2279594f6e846eabe350619cf809067d6cc282c6caeecd
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7caad477a7d0334cff2279594f6e846eabe350619cf809067d6cc282c6caeecd"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/49/upvote
Content-Type: application/json
Authorization: Bearer 67656bb57fc082c5ae698d32247004e1fa715ab9a1fd684e73ee4e4fb5a400b1
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67656bb57fc082c5ae698d32247004e1fa715ab9a1fd684e73ee4e4fb5a400b1"
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
    "key": "cache/80fe11d670128c181d61e3c2451a6156.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxNDo1OTo1OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS84MGZlMTFkNjcwMTI4YzE4MWQ2MWUzYzI0NTFhNjE1Ni5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTM1OTU4WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T135958Z",
    "x-amz-signature": "33105008854c9f4ef297721da3eae1b5f13996a7ac4e5edd86a795053bb835f2"
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
Authorization: Bearer 1a590eab68d1b047a093660c7f064f2f7cc244bb727a44a42c863a1d18b40992
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
	-H "Authorization: Bearer 1a590eab68d1b047a093660c7f064f2f7cc244bb727a44a42c863a1d18b40992"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 87da88d214f31c0b385a692382370e698f883fdab919695cba541ab1c44830d0
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
	-H "Authorization: Bearer 87da88d214f31c0b385a692382370e698f883fdab919695cba541ab1c44830d0"
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
{"password":{"reset_password_token":"UtjERurx8hreZ1u2gTR5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 908,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-13T14:01:01.396Z",
  "updated_at": "2016-10-13T14:01:01.537Z",
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
  "audit_id": 4803
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"UtjERurx8hreZ1u2gTR5","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/73/comments
Content-Type: application/json
Authorization: Bearer a64cde6654f4ca766d766bf67a0218fbf54d3fe1e52dcc47972b8c7b1cd79972
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
    "id": 44,
    "author_id": 501,
    "reply_to_id": null,
    "created_at": "2016-10-13T14:00:27.807Z",
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
curl "api.goskive.com/v2/questions/73/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a64cde6654f4ca766d766bf67a0218fbf54d3fe1e52dcc47972b8c7b1cd79972"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/74/comments
Content-Type: application/json
Authorization: Bearer d999c46fb85d9e6d8548d74cbb405c857f2a7c0b721c495c510db036147479f5
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
    "id": 45,
    "author_id": 504,
    "reply_to_id": null,
    "created_at": "2016-10-13T14:00:28.356Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 504,
      "feedbackable_id": 74,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:28.353Z",
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
curl "api.goskive.com/v2/questions/74/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d999c46fb85d9e6d8548d74cbb405c857f2a7c0b721c495c510db036147479f5"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/77/comments
Content-Type: application/json
Authorization: Bearer c0d3aa81c1083dd91d4e0d50c803fe170c2ff4e84a471eb2cfe71422ced6d819
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
      "author_id": 517,
      "reply_to_id": null,
      "created_at": "2016-10-13T14:00:29.722Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 516,
      "reply_to_id": null,
      "created_at": "2016-10-13T14:00:29.705Z",
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
curl "api.goskive.com/v2/questions/77/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0d3aa81c1083dd91d4e0d50c803fe170c2ff4e84a471eb2cfe71422ced6d819"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/75/comments
Content-Type: application/json
Authorization: Bearer c862ab8e2d416fc4502226cf8e8763860970282f5ce08e329b712db65adddd76
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
curl "api.goskive.com/v2/questions/75/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c862ab8e2d416fc4502226cf8e8763860970282f5ce08e329b712db65adddd76"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/82/feedbacks
Content-Type: application/json
Authorization: Bearer a984bcea62d97ecf1bb9abe0187588f9376f0bf4ab72d89024b0e21bf84a44dd
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
    "user_id": 533,
    "feedbackable_id": 82,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-13T14:00:32.398Z",
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
curl "api.goskive.com/v2/questions/82/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a984bcea62d97ecf1bb9abe0187588f9376f0bf4ab72d89024b0e21bf84a44dd"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/83/feedbacks
Content-Type: application/json
Authorization: Bearer 2b6dbec5c710c317fb1d6ff73442a75366703dabbfc34f63ba4c0b90224ee0b5
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
      "id": 13,
      "user_id": 540,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:32.974Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 539,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T14:00:32.960Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b6dbec5c710c317fb1d6ff73442a75366703dabbfc34f63ba4c0b90224ee0b5"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/79/votes
Content-Type: application/json
Authorization: Bearer 75381e8e05ee750f473d715cc004f1d931c207a752bd5fb75aa274c4b744b425
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
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 526
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 525
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 524
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/79/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75381e8e05ee750f473d715cc004f1d931c207a752bd5fb75aa274c4b744b425"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/54/republish
Content-Type: application/json
Authorization: Bearer 5ff62f8f98c65affb1102b3879052544fdb3983fa2f077373449667ab893daf2
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
curl "api.goskive.com/v2/questions/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ff62f8f98c65affb1102b3879052544fdb3983fa2f077373449667ab893daf2"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/51/bookmark
Content-Type: application/json
Authorization: Bearer b4b5c60279ffdd8c9042df8a9cbb0aa610f5af3663578b7571efb1bc5ad09f29
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/51/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4b5c60279ffdd8c9042df8a9cbb0aa610f5af3663578b7571efb1bc5ad09f29"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/71
Content-Type: application/json
Authorization: Bearer fe68f231846ed0616c1d4799604c476d18f605821f4c2154269642055762e2d4
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/71" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe68f231846ed0616c1d4799604c476d18f605821f4c2154269642055762e2d4"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/48/downvote
Content-Type: application/json
Authorization: Bearer 9c9424bdd257e0a46fa8b098ff245adbcde8c06f1ea504e80230d2f0ff5f5213
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c9424bdd257e0a46fa8b098ff245adbcde8c06f1ea504e80230d2f0ff5f5213"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/55
Content-Type: application/json
Authorization: Bearer cf2a933f9a571650be236ffc567227b8e81c78c92ea3d6581325509092f366fa
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
    "id": 55,
    "obfuscated_id": "VX19tR4fHZ8",
    "author_id": 442,
    "chapter_id": 79,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:20.505Z",
    "created_at": "2016-10-13T14:00:20.351Z",
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
        "id": 109,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 110,
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
curl "api.goskive.com/v2/questions/55" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf2a933f9a571650be236ffc567227b8e81c78c92ea3d6581325509092f366fa"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/52/report
Content-Type: application/json
Authorization: Bearer badc45c8d3455dad99b713c415b0491187be6f51aff53fe52251d030a1cad09e
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
	-H "Authorization: Bearer badc45c8d3455dad99b713c415b0491187be6f51aff53fe52251d030a1cad09e"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/49/bookmark
Content-Type: application/json
Authorization: Bearer 3df85ce1b909420f7ee2789fdab7db34476966e5205c9151e7be627bc59d136d
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3df85ce1b909420f7ee2789fdab7db34476966e5205c9151e7be627bc59d136d"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/72
Content-Type: application/json
Authorization: Bearer e5f5d52effa237c71676a6b3aee7eaf1404a0be6ac79cc5781ee76666bb6d4fe
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":72,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T14:00:26.919Z","updated_at":"2016-10-13T14:00:27.087Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":96,"author_id":498,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 72,
    "obfuscated_id": "oqzxOzwzIgw",
    "author_id": 498,
    "chapter_id": 96,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T14:00:27.218Z",
    "created_at": "2016-10-13T14:00:26.919Z",
    "tags": [
      {
        "id": 18,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 17,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>72, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-13T14:00:26.919Z\", \"updated_at\"=>\"2016-10-13T14:00:27.087Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>96, \"author_id\"=>498, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 145,
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
curl "api.goskive.com/v2/questions/72" -d '{"question":{"question":{"id":72,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T14:00:26.919Z","updated_at":"2016-10-13T14:00:27.087Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":96,"author_id":498,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5f5d52effa237c71676a6b3aee7eaf1404a0be6ac79cc5781ee76666bb6d4fe"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/50/upvote
Content-Type: application/json
Authorization: Bearer 31ad25364790eae2fdb432cd833ad5284936a05c147837725bc4af099d1aa30c
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31ad25364790eae2fdb432cd833ad5284936a05c147837725bc4af099d1aa30c"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 9d787aeed85520845d7921af223bd5ac04f7e5ea0274504880fba3d1ded9ac05
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
      "creator_id": 763,
      "id": 260,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 238,
      "additional_university_ids": [

      ],
      "topic_id": 272,
      "discipline_id": 273,
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
      "updated_at": "2016-10-13T14:00:49.911Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d787aeed85520845d7921af223bd5ac04f7e5ea0274504880fba3d1ded9ac05"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 714c58d5f7a0785e2002b7e15c2dee4f1d17b28d23b8f61998dfb48291c6f909
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
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-223",
      "html_url": "https://goskive.com/university/uni-223",
      "slug": "uni-223",
      "name": "National School of Pizza",
      "short_name": "Uni 223",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/48a2378f71bf32b4659c203b40668d09183285f6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6167303c927184e4d13783875ec6336736353ae3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T14:00:50.120Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-222",
      "html_url": "https://goskive.com/university/uni-222",
      "slug": "uni-222",
      "name": "National School of Pastry",
      "short_name": "Uni 222",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cc8c1bd4bd1d61da3756102e429ffda134c94210.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8bcd38c77c90580d88b3e155e39aad65f49060cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T14:00:50.101Z",
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
	-H "Authorization: Bearer 714c58d5f7a0785e2002b7e15c2dee4f1d17b28d23b8f61998dfb48291c6f909"
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
      "id": 6,
      "name": "Persistent bifurcated database",
      "name_translations": {
        "en": "Persistent bifurcated database"
      },
      "discipline_id": 6
    },
    {
      "id": 7,
      "name": "Self-enabling responsive ability",
      "name_translations": {
        "en": "Self-enabling responsive ability"
      },
      "discipline_id": 7
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
GET /v2/topics/5
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
    "id": 5,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 5
  }
}
```



```shell
curl "api.goskive.com/v2/topics/5" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 7facff721c2bc336c81610c69354502205dda7b8e085e99088c84167bfe68cfc
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
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-227",
      "html_url": "https://goskive.com/university/uni-227",
      "slug": "uni-227",
      "name": "University 164",
      "short_name": "Uni 227",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/27aee39e692923fdc4aeb25de35e40b8ec218d04.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7222332e536113456a5e807d4ab0657afc2d9100.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T14:00:50.496Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-228",
      "html_url": "https://goskive.com/university/uni-228",
      "slug": "uni-228",
      "name": "University 165",
      "short_name": "Uni 228",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/19a90aa6da94abb0d69f773db6db944e6c0d6693.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/732c0153b64d420f623bcbdde736f59a6a5fd436.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T14:00:50.513Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-226",
      "html_url": "https://goskive.com/university/uni-226",
      "slug": "uni-226",
      "name": "University 163",
      "short_name": "Uni 226",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/87c3f9f71cf52333b2986fa88abdba11d6d168a8.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/46defa593c16692a9235879b7aedb6fa7da5c984.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T14:00:50.478Z",
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
	-H "Authorization: Bearer 7facff721c2bc336c81610c69354502205dda7b8e085e99088c84167bfe68cfc"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer b05f33efebcebe3f12fdaf9a20e8ef5ae9b0b68f84feb07a03aebd0e05ca6863
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
    "id": 247,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/055789a9b4b1de6e8028fe137a3e74c648231c90.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/25ef9b1512206ad576da811dfe492b1c06bcca53.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-13T14:00:50.635Z",
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
	-H "Authorization: Bearer b05f33efebcebe3f12fdaf9a20e8ef5ae9b0b68f84feb07a03aebd0e05ca6863"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ec5fb689bc4a8b1439cbbd8f38f21d776243237d5af4b387dd2492f754778ecd
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":128,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 287,
    "id": 123,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 102,
    "additional_university_ids": [

    ],
    "topic_id": 128,
    "discipline_id": 128,
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
    "chapters_updated_at": "2016-10-13T14:00:06.320Z",
    "updated_at": "2016-10-13T14:00:06.465Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 29,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-13T14:00:06.416Z",
        "course_id": 123,
        "author_id": 287,
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
        "id": 30,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-13T14:00:06.436Z",
        "course_id": 123,
        "author_id": 287,
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
        "id": 31,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-13T14:00:06.454Z",
        "course_id": 123,
        "author_id": 287,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":128,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec5fb689bc4a8b1439cbbd8f38f21d776243237d5af4b387dd2492f754778ecd"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9992868bb04bcd770be66abb94bf7538e4b7ece9ff233a0bc3f26a38f98ade64
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":127,"published":false}}
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
    "creator_id": 286,
    "id": 122,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 101,
    "additional_university_ids": [

    ],
    "topic_id": 127,
    "discipline_id": 127,
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
    "updated_at": "2016-10-13T14:00:06.281Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":127,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9992868bb04bcd770be66abb94bf7538e4b7ece9ff233a0bc3f26a38f98ade64"
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
      "creator_id": 246,
      "id": 88,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-63",
      "html_url": "https://goskive.com/course/fu-course-63",
      "slug": "fu-course-63",
      "university_id": 87,
      "additional_university_ids": [

      ],
      "topic_id": 93,
      "discipline_id": 93,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 63",
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
      "updated_at": "2016-10-13T14:00:02.407Z",
      "shortname": "fu-course-63"
    },
    {
      "creator_id": 246,
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-64",
      "html_url": "https://goskive.com/course/fu-course-64",
      "slug": "fu-course-64",
      "university_id": 87,
      "additional_university_ids": [

      ],
      "topic_id": 94,
      "discipline_id": 94,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 64",
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
      "chapters_updated_at": "2016-10-13T14:00:02.728Z",
      "updated_at": "2016-10-13T14:00:02.735Z",
      "shortname": "fu-course-64"
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
Authorization: Bearer 6d09b1887c6cfaec4b8688c9fe6866be2ecf44b032063a4aaba570c13f0b005c
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
      "creator_id": 263,
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-79",
      "html_url": "https://goskive.com/course/fu-course-79",
      "slug": "fu-course-79",
      "university_id": 93,
      "additional_university_ids": [

      ],
      "topic_id": 109,
      "discipline_id": 109,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 79",
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
      "updated_at": "2016-10-13T14:00:04.151Z",
      "shortname": "fu-course-79"
    },
    {
      "creator_id": 263,
      "id": 105,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-80",
      "html_url": "https://goskive.com/course/fu-course-80",
      "slug": "fu-course-80",
      "university_id": 93,
      "additional_university_ids": [

      ],
      "topic_id": 110,
      "discipline_id": 110,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 80",
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
      "chapters_updated_at": "2016-10-13T14:00:04.479Z",
      "updated_at": "2016-10-13T14:00:04.487Z",
      "shortname": "fu-course-80"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d09b1887c6cfaec4b8688c9fe6866be2ecf44b032063a4aaba570c13f0b005c"
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
      "creator_id": 251,
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-67",
      "html_url": "https://goskive.com/course/fu-course-67",
      "slug": "fu-course-67",
      "university_id": 88,
      "additional_university_ids": [

      ],
      "topic_id": 97,
      "discipline_id": 97,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
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
      "updated_at": "2016-10-13T14:00:02.939Z",
      "shortname": "fu-course-67"
    },
    {
      "creator_id": 251,
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-68",
      "html_url": "https://goskive.com/course/fu-course-68",
      "slug": "fu-course-68",
      "university_id": 88,
      "additional_university_ids": [

      ],
      "topic_id": 98,
      "discipline_id": 98,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
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
      "updated_at": "2016-10-13T14:00:02.980Z",
      "shortname": "fu-course-68"
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
Authorization: Bearer 0a7637655e98d1493f296c794090b52f542eead39d664651a73dafec8bfe569b
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
      "creator_id": 270,
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-83",
      "html_url": "https://goskive.com/course/fu-course-83",
      "slug": "fu-course-83",
      "university_id": 95,
      "additional_university_ids": [

      ],
      "topic_id": 113,
      "discipline_id": 113,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 83",
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
      "updated_at": "2016-10-13T14:00:04.772Z",
      "shortname": "fu-course-83"
    },
    {
      "creator_id": 270,
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-84",
      "html_url": "https://goskive.com/course/fu-course-84",
      "slug": "fu-course-84",
      "university_id": 95,
      "additional_university_ids": [

      ],
      "topic_id": 114,
      "discipline_id": 114,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 84",
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
      "updated_at": "2016-10-13T14:00:04.812Z",
      "shortname": "fu-course-84"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a7637655e98d1493f296c794090b52f542eead39d664651a73dafec8bfe569b"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 7d144f5008f7c7da740faab29b1622cf62b7728d328c8c5cfabd230af96ae35b
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
  "id": 86,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-13T13:59:53.793Z",
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
	-H "Authorization: Bearer 7d144f5008f7c7da740faab29b1622cf62b7728d328c8c5cfabd230af96ae35b"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/184
Content-Type: application/json
Authorization: Bearer 10f622b9d4d4cefe3d3fe6cb8444f5db78144e171206d10f7b02ab254152e0c8
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
    "id": 184,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 70,
    "fields_of_study": [
      73,
      74
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-13T13:59:58.974Z",
    "updated_at": "2016-10-13T13:59:58.974Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/184" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10f622b9d4d4cefe3d3fe6cb8444f5db78144e171206d10f7b02ab254152e0c8"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/182
Content-Type: application/json
Authorization: Bearer d1be8979ecaa90a20b67c7e2da7059ca8eb9482eed7546dea0820b190f87d369
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
    "id": 182,
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
    "created_at": "2016-10-13T13:59:58.811Z",
    "updated_at": "2016-10-13T13:59:58.811Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/182" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1be8979ecaa90a20b67c7e2da7059ca8eb9482eed7546dea0820b190f87d369"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/22
Content-Type: application/json
Authorization: Bearer 2c9790106221044a7d014e8a11d620b1f1b1c106c7885c5f15b4c04734f1e853
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c9790106221044a7d014e8a11d620b1f1b1c106c7885c5f15b4c04734f1e853"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/21
Content-Type: application/json
Authorization: Bearer e83d861d9cdd0e3047cee903d93bfc2469b2d89b82b907fcacbd82625ff2d481
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
    "id": 21,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 133,
    "user_id": 957
  }
}
```



```shell
curl "api.goskive.com/v2/votes/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e83d861d9cdd0e3047cee903d93bfc2469b2d89b82b907fcacbd82625ff2d481"
```
