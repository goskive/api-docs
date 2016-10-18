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
Authorization: Basic MTBjMDUwNTE0YTEyOGJmYjAyNDA1YWI4ODI2MmZiNWNmYjcxMmVjNWRjN2Rj
YzViZTQ1ODRjM2EzOTNmYjNkMjo1MmY4YzU1NGU1M2EzNjdlNDFkOGJmYzhm
Nzc1NzNlOTlmM2RlZGYzMjQxMjVkZjA1MDkwYTYxNjMzNDJjMzAy

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
	-u 10c050514a128bfb02405ab88262fb5cfb712ec5dc7dcc5be4584c3a393fb3d2:52f8c554e53a367e41d8bfc8f77573e99f3dedf324125df05090a6163342c302
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"8248922917713fa3ae2bad970d604a350c245f8fd6ec273a267796457dd492ee","client_secret":"9b8c45d58cffa067f09e448ace4d34610306fee6458b8e5907ac28dae8d6e853"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"8248922917713fa3ae2bad970d604a350c245f8fd6ec273a267796457dd492ee","client_secret":"9b8c45d58cffa067f09e448ace4d34610306fee6458b8e5907ac28dae8d6e853"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"cd29450a52ffdd117964735e5c5bfe91d7991088f9972ba6c759a146adcc63fd","client_secret":"905264a03c1132bbdad1a50c9bfb890f62b43012299dab17af5a5ea28f9b04ab"}
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
  "access_token": "2ce5613c1f479546af6ffda728f4aa441726c4036fd58de6b28859580b2afc02",
  "token_type": "bearer",
  "created_at": 1476782354
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"cd29450a52ffdd117964735e5c5bfe91d7991088f9972ba6c759a146adcc63fd","client_secret":"905264a03c1132bbdad1a50c9bfb890f62b43012299dab17af5a5ea28f9b04ab"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MmE2ZDAzNmY1NDY2ODZkZWVmZGI3NmMwMjdjZmQyODRjOGMwYWNmNmQ0OTIz
OWVmOWVhMWM0NDQ2ZDIxYjE5YTpiNTUxOTM4YzM2YzgzYjFlM2JiOWNlNThj
NDE3Njg0MTI4YjNlMGI4ODUwNGI4YjRiNGVhYWM5ODllMTcyYjdi

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
  "access_token": "61de56facd5439d122ed60c612d0d6b2ba55487931470319db662d3ca748aa94",
  "token_type": "bearer",
  "created_at": 1476782354
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 2a6d036f546686deefdb76c027cfd284c8c0acf6d49239ef9ea1c4446d21b19a:b551938c36c83b1e3bb9ce58c417684128b3e0b88504b8b4b4eaac989e172b7b
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"744b8e3a3bcf62a68f33840b7bc62cdec55f733a08aaff059b4030c9060c21df","client_secret":"1e0d6977029fa5f5da9365e6d7a039c627ad9ab161b5294d8da3cf21b3b32c42"}
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
  "access_token": "afb251f5267b43c6cfdce1002642f14d3401792f257c1c6b1febb280fe9c94c0",
  "token_type": "bearer",
  "created_at": 1476782354
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"744b8e3a3bcf62a68f33840b7bc62cdec55f733a08aaff059b4030c9060c21df","client_secret":"1e0d6977029fa5f5da9365e6d7a039c627ad9ab161b5294d8da3cf21b3b32c42"}' -X POST \
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
GET /v2/campaigns/1
Content-Type: application/json
Authorization: Bearer b1a28d780970b553c4905e2cc0b81862fdf00d5768a3054e693be1385d06d46c
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
    "company_id": 16,
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
	-H "Authorization: Bearer b1a28d780970b553c4905e2cc0b81862fdf00d5768a3054e693be1385d06d46c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/21/flashcards
Content-Type: application/json
Authorization: Bearer 548641c602dd12bc868061f6ea1abab18092cfd4285567505c780fffca3d09bf
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":21,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 86,
    "chapter_id": 21,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:18:54.585Z",
    "created_at": "2016-10-18T09:18:54.585Z",
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
curl "api.goskive.com/v2/chapters/21/flashcards" -d '{"flashcard":{"chapter_id":21,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 548641c602dd12bc868061f6ea1abab18092cfd4285567505c780fffca3d09bf"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/22/flashcards
Content-Type: application/json
Authorization: Bearer 046a8a24767ee82e940ef457829555d42b1846b2388ded3b6cb29416b0a9de21
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 87,
      "chapter_id": 22,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:18:54.737Z",
      "created_at": "2016-10-18T09:18:54.737Z",
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 87,
      "chapter_id": 22,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:18:54.775Z",
      "created_at": "2016-10-18T09:18:54.775Z",
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 87,
      "chapter_id": 22,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:18:54.813Z",
      "created_at": "2016-10-18T09:18:54.813Z",
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
curl "api.goskive.com/v2/chapters/22/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 046a8a24767ee82e940ef457829555d42b1846b2388ded3b6cb29416b0a9de21"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/56/questions
Content-Type: application/json
Authorization: Bearer 2418ddddd259e730eb903e8155d0e4d0a7aec4dd0b6e7a82848ac43b0e4ef6c2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":56,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 65,
    "obfuscated_id": "Pu1fo5_Q1vk",
    "author_id": 243,
    "chapter_id": 56,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:09.338Z",
    "created_at": "2016-10-18T09:19:09.338Z",
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
        "id": 130,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 131,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 132,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 133,
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
curl "api.goskive.com/v2/chapters/56/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":56,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2418ddddd259e730eb903e8155d0e4d0a7aec4dd0b6e7a82848ac43b0e4ef6c2"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/53/questions
Content-Type: application/json
Authorization: Bearer b430525d94f9d6f31939d7aad1938a049ac5a8b964658ecb6d109720cf51aa37
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":53,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 234,
    "chapter_id": 53,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:08.305Z",
    "created_at": "2016-10-18T09:19:08.305Z",
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
        "id": 123,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 124,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/53/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":53,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b430525d94f9d6f31939d7aad1938a049ac5a8b964658ecb6d109720cf51aa37"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/54/questions
Content-Type: application/json
Authorization: Bearer 57caefe9dc6aa9c2d32ab90c94c7dcce9165311c12475dae4170a9894da4eb7a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":54,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 237,
    "chapter_id": 54,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:08.631Z",
    "created_at": "2016-10-18T09:19:08.631Z",
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
        "id": 125,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 126,
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
curl "api.goskive.com/v2/chapters/54/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":54,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57caefe9dc6aa9c2d32ab90c94c7dcce9165311c12475dae4170a9894da4eb7a"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/55/questions
Content-Type: application/json
Authorization: Bearer 3982ad0abc2407d486c075c9f101e9730e8567c6eacdb833d03960f6272e1fa3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":55,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 240,
    "chapter_id": 55,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:08.957Z",
    "created_at": "2016-10-18T09:19:08.957Z",
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
        "id": 127,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 128,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 129,
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
curl "api.goskive.com/v2/chapters/55/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":55,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3982ad0abc2407d486c075c9f101e9730e8567c6eacdb833d03960f6272e1fa3"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/58/questions
Content-Type: application/json
Authorization: Bearer cb02e8df30a08182313b5db3b4414398045f6a671067d8901e1ffbbe3d632d83
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 249,
      "chapter_id": 58,
      "position": 62,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:10.017Z",
      "created_at": "2016-10-18T09:19:09.908Z",
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
          "id": 134,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 135,
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
      "author_id": 250,
      "chapter_id": 58,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:10.197Z",
      "created_at": "2016-10-18T09:19:10.085Z",
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
          "id": 136,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 137,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 251,
      "chapter_id": 58,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:19:10.380Z",
      "created_at": "2016-10-18T09:19:10.266Z",
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
          "id": 138,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 139,
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
curl "api.goskive.com/v2/chapters/58/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb02e8df30a08182313b5db3b4414398045f6a671067d8901e1ffbbe3d632d83"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/47
Content-Type: application/json
Authorization: Bearer 8aeb2fa1317861515b681351fe35a4652e25edc1f48553579a7333ed5d4f8ef6
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
curl "api.goskive.com/v2/chapters/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8aeb2fa1317861515b681351fe35a4652e25edc1f48553579a7333ed5d4f8ef6"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/49
Content-Type: application/json
Authorization: Bearer 63a5f959e6b82a357b95e07b5be2d2ea57642ae2289111c7a2d72e8fd4599b5f
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
curl "api.goskive.com/v2/chapters/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63a5f959e6b82a357b95e07b5be2d2ea57642ae2289111c7a2d72e8fd4599b5f"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/52
Content-Type: application/json
Authorization: Bearer d985327793a7b19a81907067879a9645ba59443f976f644216482e8bd05bdb11
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
curl "api.goskive.com/v2/chapters/52" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d985327793a7b19a81907067879a9645ba59443f976f644216482e8bd05bdb11"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/46
Content-Type: application/json
Authorization: Bearer 5c172316ceec210733190f148e404b86888c2763a228ab4e17a032702de3a913
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c172316ceec210733190f148e404b86888c2763a228ab4e17a032702de3a913"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/45
Content-Type: application/json
Authorization: Bearer 08c01e0edd8695e14cec550b88ca4262c58f3a5702c111887a61a50d49ce5a41
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
    "id": 45,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T09:19:06.817Z",
    "course_id": 57,
    "author_id": 206,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-18T09:19:06.314Z",
    "questions_updated_at": "2016-10-18T09:19:06.314Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 210,
        "chapter_id": 45,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:06.801Z",
        "created_at": "2016-10-18T09:19:06.801Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 208,
        "chapter_id": 45,
        "position": 59,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:19:06.700Z",
        "created_at": "2016-10-18T09:19:06.589Z",
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
}
```



```shell
curl "api.goskive.com/v2/chapters/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08c01e0edd8695e14cec550b88ca4262c58f3a5702c111887a61a50d49ce5a41"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/50
Content-Type: application/json
Authorization: Bearer bf751e605a47ad089fb05a4b6460af04a52ba1b48b036a448e59da3b8642fc78
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
    "id": 50,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T09:19:07.862Z",
    "course_id": 62,
    "author_id": 225,
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
curl "api.goskive.com/v2/chapters/50" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf751e605a47ad089fb05a4b6460af04a52ba1b48b036a448e59da3b8642fc78"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/11/replies
Content-Type: application/json
Authorization: Bearer 6f7b6b8f6ddf388af8ed9c6868438a8a53a69014ddf593a736899f97ffa5e08f
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
    "id": 12,
    "author_id": 353,
    "reply_to_id": 11,
    "created_at": "2016-10-18T09:19:17.267Z",
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
curl "api.goskive.com/v2/comments/11/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f7b6b8f6ddf388af8ed9c6868438a8a53a69014ddf593a736899f97ffa5e08f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/10/replies
Content-Type: application/json
Authorization: Bearer d6a756b0e7733f09be3e9dbb978d98ba41127164fff142b64db6683b0645e3e7
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
curl "api.goskive.com/v2/comments/10/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6a756b0e7733f09be3e9dbb978d98ba41127164fff142b64db6683b0645e3e7"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/20
Content-Type: application/json
Authorization: Bearer 03b8038460d005208c2dafd30aa0af1afc78ec49ac6472e997c9d0a5bca8837c
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
curl "api.goskive.com/v2/comments/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03b8038460d005208c2dafd30aa0af1afc78ec49ac6472e997c9d0a5bca8837c"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/23/republish
Content-Type: application/json
Authorization: Bearer f9d6b61da94f2e373d6198517200d045db85a2bd30d271e75a05406df4fbbce2
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
curl "api.goskive.com/v2/comments/23/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9d6b61da94f2e373d6198517200d045db85a2bd30d271e75a05406df4fbbce2"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/19
Content-Type: application/json
Authorization: Bearer 8aec23087af8af7dd9c738192e522617b0850f2c1ce9ef5622fad236d3d3212f
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8aec23087af8af7dd9c738192e522617b0850f2c1ce9ef5622fad236d3d3212f"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/22/report
Content-Type: application/json
Authorization: Bearer 291d2ac3d5f581e8ae27051a7f6bd123160fdbd99ac39f83347c32a89564c35e
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 291d2ac3d5f581e8ae27051a7f6bd123160fdbd99ac39f83347c32a89564c35e"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/9
Content-Type: application/json
Authorization: Bearer 1cec52dfd0ef5c0ed51f69cb765c788ffac00566a75b1f6320b6fc12722bed8f
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
    "id": 9,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-18T09:19:11.592Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cec52dfd0ef5c0ed51f69cb765c788ffac00566a75b1f6320b6fc12722bed8f"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 0113b71c168880161595787c3a1a989649524423f66174f2b5af04e105a11358
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
      "id": 10,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:19:11.700Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:19:11.704Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:19:11.707Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0113b71c168880161595787c3a1a989649524423f66174f2b5af04e105a11358"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer 551fd46b95cba87423517d4de31cd3bf635ccc198780ac58994d2a37ced7a677
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 551fd46b95cba87423517d4de31cd3bf635ccc198780ac58994d2a37ced7a677"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer d9acef0c1ded6be325dae4ea71cee631ed9a6b44ece88759d368f8a9341137e7
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9acef0c1ded6be325dae4ea71cee631ed9a6b44ece88759d368f8a9341137e7"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer ccacf26ffef49b5e1e8a851b88ddfbaccf28ce806b1b0ac4c814812d016e199f
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
      "id": 2,
      "title": "Campaign 1",
      "company_id": 17,
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
      "id": 5,
      "title": "Campaign 4",
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
	-H "Authorization: Bearer ccacf26ffef49b5e1e8a851b88ddfbaccf28ce806b1b0ac4c814812d016e199f"
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
Authorization: Bearer 2830e2dc52f60000b5accf9f8b5aeda7e4a7c8176d76eb961d84af26cddc0c98
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
	-H "Authorization: Bearer 2830e2dc52f60000b5accf9f8b5aeda7e4a7c8176d76eb961d84af26cddc0c98"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b0e3d41c6c72c2c6b3c3b9941f82dca14aa4e6a19aa6a052248a3244d896568c
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
    "id": 75,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:19:18.645Z",
    "course_id": 104,
    "author_id": 374,
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
	-H "Authorization: Bearer b0e3d41c6c72c2c6b3c3b9941f82dca14aa4e6a19aa6a052248a3244d896568c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 080f8a4819d6b76fb504220dad1c6d611edf8ec29845c0ae1cbbeb152bbe29c8
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
      "id": 80,
      "title": "Clever Chapter Title 59",
      "position": 1,
      "updated_at": "2016-10-18T09:19:19.285Z",
      "course_id": 109,
      "author_id": 387,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 81,
      "title": "Clever Chapter Title 60",
      "position": 2,
      "updated_at": "2016-10-18T09:19:19.309Z",
      "course_id": 109,
      "author_id": 388,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 82,
      "title": "Clever Chapter Title 61",
      "position": 3,
      "updated_at": "2016-10-18T09:19:19.549Z",
      "course_id": 109,
      "author_id": 389,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T09:19:19.210Z",
      "questions_updated_at": "2016-10-18T09:19:19.210Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 080f8a4819d6b76fb504220dad1c6d611edf8ec29845c0ae1cbbeb152bbe29c8"
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
      "id": 92,
      "title": "Clever Chapter Title 71",
      "position": 1,
      "updated_at": "2016-10-18T09:19:20.731Z",
      "course_id": 115,
      "author_id": 415,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 93,
      "title": "Clever Chapter Title 72",
      "position": 2,
      "updated_at": "2016-10-18T09:19:20.756Z",
      "course_id": 115,
      "author_id": 416,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 94,
      "title": "Clever Chapter Title 73",
      "position": 3,
      "updated_at": "2016-10-18T09:19:20.996Z",
      "course_id": 115,
      "author_id": 417,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T09:19:20.656Z",
      "questions_updated_at": "2016-10-18T09:19:20.656Z",
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
Authorization: Bearer ac9ac6e7d7920142ed7fe9ea6ad955e618e593ad788f293ccc550a7874616b14
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
      "id": 83,
      "title": "Clever Chapter Title 62",
      "position": 1,
      "updated_at": "2016-10-18T09:19:19.696Z",
      "course_id": 110,
      "author_id": 394,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 84,
      "title": "Clever Chapter Title 63",
      "position": 2,
      "updated_at": "2016-10-18T09:19:19.721Z",
      "course_id": 110,
      "author_id": 395,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 85,
      "title": "Clever Chapter Title 64",
      "position": 3,
      "updated_at": "2016-10-18T09:19:19.747Z",
      "course_id": 110,
      "author_id": 396,
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
	-H "Authorization: Bearer ac9ac6e7d7920142ed7fe9ea6ad955e618e593ad788f293ccc550a7874616b14"
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
      "id": 95,
      "title": "Clever Chapter Title 74",
      "position": 1,
      "updated_at": "2016-10-18T09:19:21.186Z",
      "course_id": 117,
      "author_id": 422,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 96,
      "title": "Clever Chapter Title 75",
      "position": 2,
      "updated_at": "2016-10-18T09:19:21.211Z",
      "course_id": 117,
      "author_id": 423,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 97,
      "title": "Clever Chapter Title 76",
      "position": 3,
      "updated_at": "2016-10-18T09:19:21.236Z",
      "course_id": 117,
      "author_id": 424,
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
Authorization: Bearer a297054d7bcec0e3af4e8465c74bf1634a8709a34eaa328501cdd951685b3178
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
    "course_id": 302,
    "user_id": 950,
    "updated_at": "2016-10-18T09:19:57.165Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a297054d7bcec0e3af4e8465c74bf1634a8709a34eaa328501cdd951685b3178"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0346dec193b64b555bb4780b7ef5629791b4b9dbfaf79b68d9c90e27688fc9d0
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
      "course_id": 307,
      "user_id": 962,
      "updated_at": "2016-10-18T09:19:57.745Z"
    },
    {
      "id": 7,
      "course_id": 307,
      "user_id": 963,
      "updated_at": "2016-10-18T09:19:57.758Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0346dec193b64b555bb4780b7ef5629791b4b9dbfaf79b68d9c90e27688fc9d0"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/99/files
Content-Type: application/json
Authorization: Bearer 1161f603e7dd50b989cbfeca3dd52faf7bb1056648204a947ed8b9a84dbec1e8
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
      "id": 4,
      "uploader": {
        "id": 359,
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
        "created_at": "2016-10-18T09:19:17.757Z",
        "updated_at": "2016-10-18T09:19:17.757Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:19:17.764Z",
      "updated_at": "2016-10-18T09:19:17.764Z",
      "course_id": 99,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 360,
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
        "created_at": "2016-10-18T09:19:17.772Z",
        "updated_at": "2016-10-18T09:19:17.772Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:19:17.779Z",
      "updated_at": "2016-10-18T09:19:17.779Z",
      "course_id": 99,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 361,
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
        "created_at": "2016-10-18T09:19:17.786Z",
        "updated_at": "2016-10-18T09:19:17.786Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:19:17.794Z",
      "updated_at": "2016-10-18T09:19:17.794Z",
      "course_id": 99,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/99/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1161f603e7dd50b989cbfeca3dd52faf7bb1056648204a947ed8b9a84dbec1e8"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/97/files
Content-Type: application/json
Authorization: Bearer c1d663fe63196745169d0ba521009aba40d0659b981471059cf083c4fc10faf7
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
    "id": 3,
    "uploader": {
      "id": 355,
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
      "created_at": "2016-10-18T09:19:17.487Z",
      "updated_at": "2016-10-18T09:19:17.487Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-18T09:19:17.529Z",
    "updated_at": "2016-10-18T09:19:17.529Z",
    "course_id": 97,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/97/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1d663fe63196745169d0ba521009aba40d0659b981471059cf083c4fc10faf7"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/100/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer d18dc1b3f89d166542127974cdaa23575af49fcf4cb46542f16b546fceb20131
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
    "key": "cache/d9ba3b927489a31cc8bb752d1997a62f.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMDoxOToxN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9kOWJhM2I5Mjc0ODlhMzFjYzhiYjc1MmQxOTk3YTYyZi5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMThUMDkxOTE3WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T091917Z",
    "x-amz-signature": "b59ea7ffb86d8c18598e0055eb0d143c71e7b4c21b9409ee646e4c42a3feee77"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/100/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d18dc1b3f89d166542127974cdaa23575af49fcf4cb46542f16b546fceb20131"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 54a257f2a12a4abe3a767c222087b251d4f9bcd65051c6cfbef8236f74738d79
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
	-H "Authorization: Bearer 54a257f2a12a4abe3a767c222087b251d4f9bcd65051c6cfbef8236f74738d79"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d3f62c5696d60fcedcfd27be43996449601f4d9e092e5a2989625ea73c9a0d3e
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
	-H "Authorization: Bearer d3f62c5696d60fcedcfd27be43996449601f4d9e092e5a2989625ea73c9a0d3e"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8a45a26db2a386648039054a2085d98f0cdc1c7e4666e338d9df74c5a2fc5d2c
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
	-H "Authorization: Bearer 8a45a26db2a386648039054a2085d98f0cdc1c7e4666e338d9df74c5a2fc5d2c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c232171a1e70cc1b8645db67ee455e48c8eaf27534b65e7c7f3abb8708f71936
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
	-H "Authorization: Bearer c232171a1e70cc1b8645db67ee455e48c8eaf27534b65e7c7f3abb8708f71936"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e9daac85f2f841d71b7ef7a70eb055a36cd7d20263c7b770831c648bdf51481e
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
	-H "Authorization: Bearer e9daac85f2f841d71b7ef7a70eb055a36cd7d20263c7b770831c648bdf51481e"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 3fc787fa48f3aeb6cc7156d4808b3b11b629304053044c120f3a8b695f3d5128
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
    "creator_id": 23,
    "id": 11,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 11,
    "additional_university_ids": [

    ],
    "topic_id": 11,
    "discipline_id": 11,
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
    "chapters_updated_at": "2016-10-18T09:18:44.661Z",
    "updated_at": "2016-10-18T09:18:46.046Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 5,
        "title": "Clever Chapter Title 5",
        "position": 1,
        "updated_at": "2016-10-18T09:18:46.001Z",
        "course_id": 11,
        "author_id": 23,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:18:44.661Z",
        "questions_updated_at": "2016-10-18T09:18:44.661Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 6,
        "title": "Clever Chapter Title 6",
        "position": 2,
        "updated_at": "2016-10-18T09:18:46.039Z",
        "course_id": 11,
        "author_id": 23,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:18:44.661Z",
        "questions_updated_at": "2016-10-18T09:18:44.661Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 24,
        "chapter_id": 5,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.846Z",
        "created_at": "2016-10-18T09:18:45.846Z",
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
        "author_id": 24,
        "chapter_id": 6,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.916Z",
        "created_at": "2016-10-18T09:18:45.916Z",
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
        "author_id": 24,
        "chapter_id": 5,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.886Z",
        "created_at": "2016-10-18T09:18:45.886Z",
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
        "author_id": 24,
        "chapter_id": 6,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.954Z",
        "created_at": "2016-10-18T09:18:45.954Z",
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
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 24,
        "chapter_id": 5,
        "position": 3,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:44.867Z",
        "created_at": "2016-10-18T09:18:44.756Z",
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
            "id": 5,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 6,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 24,
        "chapter_id": 5,
        "position": 4,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.034Z",
        "created_at": "2016-10-18T09:18:44.927Z",
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
      },
      {
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 24,
        "chapter_id": 6,
        "position": 5,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.231Z",
        "created_at": "2016-10-18T09:18:45.114Z",
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
            "id": 9,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 10,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 24,
        "chapter_id": 6,
        "position": 6,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:45.402Z",
        "created_at": "2016-10-18T09:18:45.293Z",
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
            "id": 11,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 12,
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
	-H "Authorization: Bearer 3fc787fa48f3aeb6cc7156d4808b3b11b629304053044c120f3a8b695f3d5128"
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
    "creator_id": 35,
    "id": 13,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 13,
    "additional_university_ids": [

    ],
    "topic_id": 13,
    "discipline_id": 13,
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
    "chapters_updated_at": "2016-10-18T09:18:47.693Z",
    "updated_at": "2016-10-18T09:18:49.125Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 9,
        "title": "Clever Chapter Title 9",
        "position": 1,
        "updated_at": "2016-10-18T09:18:49.077Z",
        "course_id": 13,
        "author_id": 35,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:18:47.693Z",
        "questions_updated_at": "2016-10-18T09:18:47.693Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 10,
        "title": "Clever Chapter Title 10",
        "position": 2,
        "updated_at": "2016-10-18T09:18:49.117Z",
        "course_id": 13,
        "author_id": 35,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:18:47.693Z",
        "questions_updated_at": "2016-10-18T09:18:47.693Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 35,
        "chapter_id": 9,
        "position": 15,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:47.905Z",
        "created_at": "2016-10-18T09:18:47.787Z",
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
        "author_id": 35,
        "chapter_id": 10,
        "position": 17,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:18:48.277Z",
        "created_at": "2016-10-18T09:18:48.157Z",
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
PUT /v2/courses/15/pin
Content-Type: application/json
Authorization: Bearer 1ab457a7c3d6d669be585b789e3d1a5283256a8ea31b52d2e5997d555b989a59
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/15/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ab457a7c3d6d669be585b789e3d1a5283256a8ea31b52d2e5997d555b989a59"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/1/pin
Content-Type: application/json
Authorization: Bearer d228e117a9e2a348583afb38181d884e91aa4bfb14cffda859784118cd7c5ecd
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/1/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d228e117a9e2a348583afb38181d884e91aa4bfb14cffda859784118cd7c5ecd"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0b4e82513bbfe9c3ff3f7527b8a8b310eb26da58dea66ea354aecaf5dd758cdf
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
    "creator_id": 50,
    "id": 17,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 17,
    "additional_university_ids": [

    ],
    "topic_id": 17,
    "discipline_id": 17,
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
    "updated_at": "2016-10-18T09:18:51.057Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b4e82513bbfe9c3ff3f7527b8a8b310eb26da58dea66ea354aecaf5dd758cdf"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer fa64f7398ef388306c330f8142bf87f218dad74d42392cc2457c713788ed9684
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
    "id": 258,
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
    "created_at": "2016-10-18T09:19:11.150Z",
    "updated_at": "2016-10-18T09:19:11.150Z",
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
	-H "Authorization: Bearer fa64f7398ef388306c330f8142bf87f218dad74d42392cc2457c713788ed9684"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f6d88058f74c1a76d2ba831b5f623fccda2d0f4aa07dc25b85963c8e28632dca
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[72]}
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
    "id": 254,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      72
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:19:10.884Z",
    "updated_at": "2016-10-18T09:19:10.920Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[72]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6d88058f74c1a76d2ba831b5f623fccda2d0f4aa07dc25b85963c8e28632dca"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 10566f2925f2683c585d8b034ec1fb88269023247e9f80ef2e7db2dce5d6ac23
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
    "id": 257,
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
    "created_at": "2016-10-18T09:19:11.077Z",
    "updated_at": "2016-10-18T09:19:11.077Z",
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
	-H "Authorization: Bearer 10566f2925f2683c585d8b034ec1fb88269023247e9f80ef2e7db2dce5d6ac23"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7654a279949af7d679411be5ede2cc23a604ba080b573f3c24316a4ffbdc0e89
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[73]}
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
    "id": 255,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      73
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:19:10.959Z",
    "updated_at": "2016-10-18T09:19:10.959Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[73]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7654a279949af7d679411be5ede2cc23a604ba080b573f3c24316a4ffbdc0e89"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 50f48f99b4678d0004caaabb5fc015de493d0d3804e13762f5c778e6a962f151
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

71
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
    "id": 253,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/e05ba27ef49ae100cc6ae725b7d96457a5ca50bf.jpg",
    "university_id": null,
    "fields_of_study": [
      71
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:19:10.519Z",
    "updated_at": "2016-10-18T09:19:10.826Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/9b5c08c34fc8fd1fc34a0ebe445605bb29952553.jpg",
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

71
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 50f48f99b4678d0004caaabb5fc015de493d0d3804e13762f5c778e6a962f151"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2d434d8d7f155f201d81dbb4b9c0f822975194ff9d57e801894b5dd565360f32
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
      "bookmarkable_id": 69,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 70,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 71,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d434d8d7f155f201d81dbb4b9c0f822975194ff9d57e801894b5dd565360f32"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 2430d4677d264ff33ddfb48498260eaabaf43890f6d1ba4d281d95c7a4fd36f0
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
	-H "Authorization: Bearer 2430d4677d264ff33ddfb48498260eaabaf43890f6d1ba4d281d95c7a4fd36f0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 772a23cf74078663ad1cd2bf750b194bdd6a718430b6bf0a8e94c87a1ecd2805
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
	-H "Authorization: Bearer 772a23cf74078663ad1cd2bf750b194bdd6a718430b6bf0a8e94c87a1ecd2805"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 383e6c8211922efe9f69ecb2d85df352d10378ee475f80045383b5a8e826513e
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
      "creator_id": 315,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-46",
      "html_url": "https://goskive.com/course/mit-course-46",
      "slug": "mit-course-46",
      "university_id": 85,
      "additional_university_ids": [

      ],
      "topic_id": 90,
      "discipline_id": 90,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 46",
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
      "updated_at": "2016-10-18T09:19:14.315Z",
      "shortname": "mit-course-46"
    },
    {
      "creator_id": 316,
      "id": 86,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-47",
      "html_url": "https://goskive.com/course/mit-course-47",
      "slug": "mit-course-47",
      "university_id": 86,
      "additional_university_ids": [

      ],
      "topic_id": 91,
      "discipline_id": 91,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
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
      "updated_at": "2016-10-18T09:19:14.391Z",
      "shortname": "mit-course-47"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 383e6c8211922efe9f69ecb2d85df352d10378ee475f80045383b5a8e826513e"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e02bbeda9714cb50fec657326cb5be5fb5a964aec907cf8683ff76d17fbbd516
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
        "updated_at": "2016-10-18T09:19:11.492Z"
      },
      "created_at": "2016-10-18T09:19:11.495Z",
      "updated_at": "2016-10-18T09:19:11.495Z",
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
        "updated_at": "2016-10-18T09:19:11.503Z"
      },
      "created_at": "2016-10-18T09:19:11.507Z",
      "updated_at": "2016-10-18T09:19:11.507Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e02bbeda9714cb50fec657326cb5be5fb5a964aec907cf8683ff76d17fbbd516"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 24c3d0de2e7eda96172855f4ca8bc2534e7fac4893c98b16707311530e85b7c5
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
        "updated_at": "2016-10-18T09:19:11.258Z"
      },
      "created_at": "2016-10-18T09:19:11.262Z",
      "updated_at": "2016-10-18T09:19:11.262Z",
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
        "updated_at": "2016-10-18T09:19:11.276Z"
      },
      "created_at": "2016-10-18T09:19:11.279Z",
      "updated_at": "2016-10-18T09:19:11.279Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24c3d0de2e7eda96172855f4ca8bc2534e7fac4893c98b16707311530e85b7c5"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 0998670d474fe4ede0c53077771c8c72978610a5718bebdc8aac8a36181ac49c
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
      "id": 4,
      "created_at": "2016-10-18T09:18:59.732Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 5,
      "updated_at": "2016-10-18T09:18:59.846Z",
      "author_id": "130",
      "thread_subject_id": "38",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 5,
      "created_at": "2016-10-18T09:18:59.834Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-10-18T09:18:59.849Z",
      "author_id": "133",
      "thread_subject_id": "39",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-18T09:19:00.280Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-18T09:19:00.280Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-18T09:19:00.638Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-10-18T09:19:00.638Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 8,
      "created_at": "2016-10-18T09:19:00.983Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-18T09:19:00.983Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 9,
      "created_at": "2016-10-18T09:19:01.265Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 42,
      "updated_at": "2016-10-18T09:19:01.265Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-18T09:19:01.556Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 43,
      "updated_at": "2016-10-18T09:19:01.556Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-18T09:19:01.855Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 44,
      "updated_at": "2016-10-18T09:19:01.855Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0998670d474fe4ede0c53077771c8c72978610a5718bebdc8aac8a36181ac49c"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/12
Content-Type: application/json
Authorization: Bearer 0049143bbe7776e6e5c443bf6870a48be2130e9393812da55b43eff74e6ed8a5
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-18T09:09:01.000Z"}}
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
    "id": 12,
    "created_at": "2016-10-18T09:19:02.004Z",
    "read_at": "2016-10-18T09:09:01.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 7,
    "updated_at": "2016-10-18T09:19:02.047Z",
    "author_id": "158",
    "thread_subject_id": "46",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/12" -d '{"notification":{"read_at":"2016-10-18T09:09:01.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0049143bbe7776e6e5c443bf6870a48be2130e9393812da55b43eff74e6ed8a5"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 15210aa2949ce9c70dacafb3bf055a7693708113b3085520e51cac2b2454847e
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
      "course_id": 72,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T09:19:11.969Z",
      "course_published": true,
      "updated_at": "2016-10-18T09:19:11.962Z"
    },
    {
      "id": 4,
      "course_id": 73,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T09:19:12.049Z",
      "course_published": true,
      "updated_at": "2016-10-18T09:19:12.042Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15210aa2949ce9c70dacafb3bf055a7693708113b3085520e51cac2b2454847e"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 91e5e92e32e6c7446c58da0688e0952639e8bf57d15708501eb2bd7074337a2f
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
    "course_id": 71,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T09:19:11.829Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:19:11.821Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91e5e92e32e6c7446c58da0688e0952639e8bf57d15708501eb2bd7074337a2f"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer a664cc632ae47babd3ae09fd93fd341b2e33bb7bcc97a6a997c0cbf4a64a9ca4
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
    "course_id": 76,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-18T09:19:12.476Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:19:12.465Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a664cc632ae47babd3ae09fd93fd341b2e33bb7bcc97a6a997c0cbf4a64a9ca4"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 2808445d436c6d81e8b94b20142a181781a5e70015aee322eb2cf3dabe885cee
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
      "votable_id": 32,
      "user_id": 93
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 33,
      "user_id": 93
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 34,
      "user_id": 93
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 35,
      "user_id": 93
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2808445d436c6d81e8b94b20142a181781a5e70015aee322eb2cf3dabe885cee"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/94
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
    "id": 94,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 92,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 94
      },
      {
        "id": 93,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 94
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/94" -X GET \
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
      "id": 92,
      "name": "Versatile intangible internet solution",
      "name_translations": {
        "en": "Versatile intangible internet solution"
      }
    },
    {
      "id": 93,
      "name": "Secured asymmetric projection",
      "name_translations": {
        "en": "Secured asymmetric projection"
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
PATCH /v2/feedbacks/44/close
Content-Type: application/json
Authorization: Bearer f40fc86eb47122a741d05ec54898fc7cd38a90dcc0cd00d48dbef8f505afe174
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
    "id": 44,
    "user_id": 854,
    "feedbackable_id": 93,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-18T09:19:48.005Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/44/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f40fc86eb47122a741d05ec54898fc7cd38a90dcc0cd00d48dbef8f505afe174"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/fix
Content-Type: application/json
Authorization: Bearer 4c9d7f51937f56a2e62d72a779982449ccaf5213a1f9b80bbd8902120ed8820f
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
    "id": 42,
    "user_id": 844,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-18T09:19:47.502Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/42/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c9d7f51937f56a2e62d72a779982449ccaf5213a1f9b80bbd8902120ed8820f"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/38
Content-Type: application/json
Authorization: Bearer 4529b4ee81e25b4268340900921f4515eb091c3e9459ccee7134c5e2036fbc6f
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
    "id": 38,
    "user_id": 822,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:19:46.487Z",
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
curl "api.goskive.com/v2/feedbacks/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4529b4ee81e25b4268340900921f4515eb091c3e9459ccee7134c5e2036fbc6f"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/40/fix
Content-Type: application/json
Authorization: Bearer e28064d67f217e64ddcb08cf30791b3baad5a17c2bfc4ff2f63d752847dade94
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
curl "api.goskive.com/v2/feedbacks/40/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e28064d67f217e64ddcb08cf30791b3baad5a17c2bfc4ff2f63d752847dade94"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 46b9c23884600001651aaca989d9710edeb33d71ecee44dbf5142bb21bc4889e
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
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46b9c23884600001651aaca989d9710edeb33d71ecee44dbf5142bb21bc4889e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/close
Content-Type: application/json
Authorization: Bearer b67947e6da256b1a0bc15f209e7301991dbcbcdb3581f65a75797ca16f5a53d5
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
curl "api.goskive.com/v2/feedbacks/46/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b67947e6da256b1a0bc15f209e7301991dbcbcdb3581f65a75797ca16f5a53d5"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/39
Content-Type: application/json
Authorization: Bearer 2a95aa7682a739756f77f49ab150af5c671a9851ec372daa37ab3425a451f3e0
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
    "id": 39,
    "user_id": 827,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:19:46.751Z",
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
curl "api.goskive.com/v2/feedbacks/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a95aa7682a739756f77f49ab150af5c671a9851ec372daa37ab3425a451f3e0"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Authorization: Bearer 9fe92a2c45601537fee164353f5b16f1f6d614e0dfb9ecb05ef6b3a873f53173
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
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Authorization: Bearer 9fe92a2c45601537fee164353f5b16f1f6d614e0dfb9ecb05ef6b3a873f53173" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Authorization: Bearer 465395a80a2f43fc43ba5fc934f8fff60927adf79caf6884a15c3cbad7a59f89
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
	-H "Authorization: Bearer 465395a80a2f43fc43ba5fc934f8fff60927adf79caf6884a15c3cbad7a59f89" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/7
Authorization: Bearer 23cfc0d006d258491c583f70fa129cdc1fce6751d60364a50523a8d689f06f73
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/1844faeafd0d202b54d22dc0b35f052a.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T091927Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=542a5faf11f9d912ca8e1199d3a7d20c5bb416a43cdc966f6789a298c1e819a1"
  }
}
```



```shell
curl "api.goskive.com/v2/files/7" -X GET \
	-H "Authorization: Bearer 23cfc0d006d258491c583f70fa129cdc1fce6751d60364a50523a8d689f06f73"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Authorization: Bearer f7da64276c60ff563cb00f9e79c329849e7c81317fd26ace3dce9a618c41656f
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
    "id": 13,
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
      "created_at": "2016-10-18T09:19:27.601Z",
      "updated_at": "2016-10-18T09:19:27.601Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-18T09:19:27.669Z",
    "updated_at": "2016-10-18T09:19:27.669Z",
    "course_id": 153,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Authorization: Bearer f7da64276c60ff563cb00f9e79c329849e7c81317fd26ace3dce9a618c41656f" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer 15c43be1f33fb077036b115f0729939d06748e5e2fb777a945300723b8ef1322
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
      "creator_id": 173,
      "id": 50,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 50,
      "additional_university_ids": [

      ],
      "topic_id": 50,
      "discipline_id": 50,
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
      "chapters_updated_at": "2016-10-18T09:19:02.244Z",
      "updated_at": "2016-10-18T09:19:03.790Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 178,
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-650b1b56-6d5d-4d6f-bedc-9de2bed12486",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-650b1b56-6d5d-4d6f-bedc-9de2bed12486",
      "slug": "mit-the-great-british-bake-off-650b1b56-6d5d-4d6f-bedc-9de2bed12486",
      "university_id": 51,
      "additional_university_ids": [

      ],
      "topic_id": 51,
      "discipline_id": 51,
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
      "chapters_updated_at": "2016-10-18T09:19:02.244Z",
      "updated_at": "2016-10-18T09:19:04.311Z",
      "shortname": "mit-the-great-british-bake-off-650b1b56-6d5d-4d6f-bedc-9de2bed12486"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 15c43be1f33fb077036b115f0729939d06748e5e2fb777a945300723b8ef1322"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/11/preview
Authorization: Bearer 1a02c4586b798df09272c2ab34a67f8ec6f25876c13dd1bff2d849bc92c3e6e5
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/68ca827d135dfbc0b48b3730b01ea224.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T091927Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=c88f9f107e8999d3189c7286b8d29b80907267b81c09b25fdabd562b63b78ad0"
  }
}
```



```shell
curl "api.goskive.com/v2/files/11/preview" -X GET \
	-H "Authorization: Bearer 1a02c4586b798df09272c2ab34a67f8ec6f25876c13dd1bff2d849bc92c3e6e5"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/12/report
Authorization: Bearer 6a82b4faba65e4bfd21df72b70392074113b7e485272b0f9ab800ab488572cdf
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
	-H "Authorization: Bearer 6a82b4faba65e4bfd21df72b70392074113b7e485272b0f9ab800ab488572cdf" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/57/comments
Content-Type: application/json
Authorization: Bearer 2c2aa45ec57ddebfd03566484bc53ec34860641a52bde0bddc032cb1dd07900b
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
    "id": 15,
    "author_id": 437,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:19:22.064Z",
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
curl "api.goskive.com/v2/flashcards/57/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c2aa45ec57ddebfd03566484bc53ec34860641a52bde0bddc032cb1dd07900b"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/58/comments
Content-Type: application/json
Authorization: Bearer 9c4809bfb1c0364f18412995d638787a17b4b3f054dee4dcb1a040addd18f006
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
    "id": 16,
    "author_id": 440,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:19:22.369Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 440,
      "feedbackable_id": 58,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:22.366Z",
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
	-H "Authorization: Bearer 9c4809bfb1c0364f18412995d638787a17b4b3f054dee4dcb1a040addd18f006"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer fd22f70cec0a995a182ac646ab853091bd75a91f390cc1b4b5f5f3dbdf053f1e
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
      "id": 13,
      "author_id": 432,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:21.664Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 433,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:19:21.680Z",
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
	-H "Authorization: Bearer fd22f70cec0a995a182ac646ab853091bd75a91f390cc1b4b5f5f3dbdf053f1e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/56/comments
Content-Type: application/json
Authorization: Bearer 3de51dcfdcc03273693cb030cf30d9ed616c6d8a258042b6a7335811eff27a93
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
curl "api.goskive.com/v2/flashcards/56/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3de51dcfdcc03273693cb030cf30d9ed616c6d8a258042b6a7335811eff27a93"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/48/feedbacks
Content-Type: application/json
Authorization: Bearer b9472f0e55fa4da965f31933f338c3cc824a9391edf0c9cb41cd8c6ef4799bea
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
    "id": 8,
    "user_id": 307,
    "feedbackable_id": 48,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:19:13.747Z",
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
curl "api.goskive.com/v2/flashcards/48/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9472f0e55fa4da965f31933f338c3cc824a9391edf0c9cb41cd8c6ef4799bea"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/43/feedbacks
Content-Type: application/json
Authorization: Bearer 23a48fbebace1fa75184143ba45d88ab61c47bb643b06b280040cb3a8b6b3ba6
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
      "id": 3,
      "user_id": 284,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:12.809Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 283,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:12.797Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23a48fbebace1fa75184143ba45d88ab61c47bb643b06b280040cb3a8b6b3ba6"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/28/votes
Content-Type: application/json
Authorization: Bearer 460e0e8e9484e1a49d3837556052d4faf76ae6a051ed4661522dbf5163db0132
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
      "id": 4,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 80
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 79
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 28,
      "user_id": 78
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/28/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 460e0e8e9484e1a49d3837556052d4faf76ae6a051ed4661522dbf5163db0132"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/80/republish
Content-Type: application/json
Authorization: Bearer 4d4c66357acb70da5d86311c386f47b7b2f78e50f3c129d98c9f4ddb25c79eda
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
curl "api.goskive.com/v2/flashcards/80/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d4c66357acb70da5d86311c386f47b7b2f78e50f3c129d98c9f4ddb25c79eda"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/78/bookmark
Content-Type: application/json
Authorization: Bearer 06761ff1a06230b5444b84191020467868ec2eb7e9a8ad7a85896e2b30d9426a
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/78/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06761ff1a06230b5444b84191020467868ec2eb7e9a8ad7a85896e2b30d9426a"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/82
Content-Type: application/json
Authorization: Bearer 866da1abd1600a77b271761b921978d96e5e204b23fab96523dfa25e403df6a2
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/82" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 866da1abd1600a77b271761b921978d96e5e204b23fab96523dfa25e403df6a2"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/59/downvote
Content-Type: application/json
Authorization: Bearer b62c99b0ef6e4887727eeaebe7773e87a605ba39a63b750d3e0eddc446f3dcb2
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/59/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b62c99b0ef6e4887727eeaebe7773e87a605ba39a63b750d3e0eddc446f3dcb2"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/79
Content-Type: application/json
Authorization: Bearer 18bc5d4d0a8c500ccca46d51adaec026f5c9b1c9f2b41421ac6b363943cf9421
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 508,
    "chapter_id": 123,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:25.876Z",
    "created_at": "2016-10-18T09:19:25.876Z",
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
curl "api.goskive.com/v2/flashcards/79" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18bc5d4d0a8c500ccca46d51adaec026f5c9b1c9f2b41421ac6b363943cf9421"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/76/report
Content-Type: application/json
Authorization: Bearer 826b48e8d35151828072f3169f32b83eab21bf54d50b7e9dccf5feb52bb4ccc7
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 826b48e8d35151828072f3169f32b83eab21bf54d50b7e9dccf5feb52bb4ccc7"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/77/bookmark
Content-Type: application/json
Authorization: Bearer 9c623122a3bdeeaec48ad84232f265c984723bb15756b3251c4595d798cc813c
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/77/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c623122a3bdeeaec48ad84232f265c984723bb15756b3251c4595d798cc813c"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/75/upvote
Content-Type: application/json
Authorization: Bearer bf4f1e357cf924a171d9fc9a63f38efcc004f14f23ad4cd135e827d1015d7506
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf4f1e357cf924a171d9fc9a63f38efcc004f14f23ad4cd135e827d1015d7506"
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
    "key": "cache/69192c84646cbb62ac6d9f410baf3e14.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMDoxOToxNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS82OTE5MmM4NDY0NmNiYjYyYWM2ZDlmNDEwYmFmM2UxNC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOFQwOTE5MTRaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T091914Z",
    "x-amz-signature": "e410b71bb51e7098d98e57f868ec85dc773552a888c79e602af65cf8e74d5d53"
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
Authorization: Bearer 89f2d6695a88f235715a295ed09a05e8db9012bd708ea502113e06c5446dd431
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
	-H "Authorization: Bearer 89f2d6695a88f235715a295ed09a05e8db9012bd708ea502113e06c5446dd431"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer a649eb0ab69e5dead21a7e04df5d47bd5f8690eb847153e51101a9b42519599e
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
	-H "Authorization: Bearer a649eb0ab69e5dead21a7e04df5d47bd5f8690eb847153e51101a9b42519599e"
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
{"password":{"reset_password_token":"CFivxmp2D5usLSC7XQmv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 107,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-18T09:18:56.596Z",
  "updated_at": "2016-10-18T09:18:57.184Z",
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
  "audit_id": 3313
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"CFivxmp2D5usLSC7XQmv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/31/comments
Content-Type: application/json
Authorization: Bearer dc1aa535dc22a57983827d440015bf9669d7d39588aeab887e33c934ef605f25
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
    "id": 4,
    "author_id": 69,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:18:53.416Z",
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
curl "api.goskive.com/v2/questions/31/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc1aa535dc22a57983827d440015bf9669d7d39588aeab887e33c934ef605f25"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/30/comments
Content-Type: application/json
Authorization: Bearer c3ac62e861c43e581b21474538f65d070b3f35df515e8dad722e3faf3091afb6
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
    "id": 3,
    "author_id": 66,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:18:52.705Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 66,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:18:52.700Z",
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
curl "api.goskive.com/v2/questions/30/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3ac62e861c43e581b21474538f65d070b3f35df515e8dad722e3faf3091afb6"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer fab4cf99107fd08008114af671a3da51f92c8686f61942ce6f74a739de7396d1
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
      "author_id": 58,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:18:51.632Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 59,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:18:51.664Z",
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
curl "api.goskive.com/v2/questions/27/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fab4cf99107fd08008114af671a3da51f92c8686f61942ce6f74a739de7396d1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/29/comments
Content-Type: application/json
Authorization: Bearer 3a21d77c751d55915e44befc5e432db30a0ef02e7bb48a66b06855c57fba512a
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
curl "api.goskive.com/v2/questions/29/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a21d77c751d55915e44befc5e432db30a0ef02e7bb48a66b06855c57fba512a"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/90/feedbacks
Content-Type: application/json
Authorization: Bearer 92f1adf3503e77280576830e7586f75fb94008aafa4d6d9160ec7e41cf375cf1
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
    "id": 18,
    "user_id": 639,
    "feedbackable_id": 90,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:19:35.973Z",
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
curl "api.goskive.com/v2/questions/90/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92f1adf3503e77280576830e7586f75fb94008aafa4d6d9160ec7e41cf375cf1"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/85/feedbacks
Content-Type: application/json
Authorization: Bearer 804935eee81fb7e875a7a09f5d32b491b19b9fec61165e084318b4bb9ffd3be2
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
      "id": 14,
      "user_id": 618,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:34.245Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 617,
      "feedbackable_id": 85,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:19:34.234Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/85/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 804935eee81fb7e875a7a09f5d32b491b19b9fec61165e084318b4bb9ffd3be2"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/55/votes
Content-Type: application/json
Authorization: Bearer ff86e3084d1b5c5419bcb10055971653850cd6fd1545e30193b95b2e9f39ce24
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
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 55,
      "user_id": 197
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 55,
      "user_id": 196
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 55,
      "user_id": 195
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/55/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff86e3084d1b5c5419bcb10055971653850cd6fd1545e30193b95b2e9f39ce24"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/113/republish
Content-Type: application/json
Authorization: Bearer 30555f02b9913166429f8daafb01152108b41025cb0a0e320a49c32e1d9259ed
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
curl "api.goskive.com/v2/questions/113/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30555f02b9913166429f8daafb01152108b41025cb0a0e320a49c32e1d9259ed"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/131/bookmark
Content-Type: application/json
Authorization: Bearer 178f81033af52d496bee4c664280ecbd289ee82dd4c28726aa47b883029e906d
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/131/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 178f81033af52d496bee4c664280ecbd289ee82dd4c28726aa47b883029e906d"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/132
Content-Type: application/json
Authorization: Bearer 4e8c66f0c16cc0da9d7b34dd7478470513b013a12fe1bb934c8feb2e6e59e3bb
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/132" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e8c66f0c16cc0da9d7b34dd7478470513b013a12fe1bb934c8feb2e6e59e3bb"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/115/downvote
Content-Type: application/json
Authorization: Bearer 1dc6cef4fe5d7ba4ef2bbc69d825deadd3120319613fb1cbd068669aaa910fe9
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1dc6cef4fe5d7ba4ef2bbc69d825deadd3120319613fb1cbd068669aaa910fe9"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/112
Content-Type: application/json
Authorization: Bearer 0c5feb3e7d593af6f98d2b82c0a18de8206696e8f6ca70f8dfaecfb5e04e88ac
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
    "id": 112,
    "obfuscated_id": "7Qwj1ZvbWUI",
    "author_id": 872,
    "chapter_id": 173,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:49.854Z",
    "created_at": "2016-10-18T09:19:49.742Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/112" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c5feb3e7d593af6f98d2b82c0a18de8206696e8f6ca70f8dfaecfb5e04e88ac"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/110/report
Content-Type: application/json
Authorization: Bearer 47c10ea657f7fae30b4dcb249f2154788d7ca22fd6a06096cb22dd8eeb186240
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47c10ea657f7fae30b4dcb249f2154788d7ca22fd6a06096cb22dd8eeb186240"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/134/bookmark
Content-Type: application/json
Authorization: Bearer a611841d5f7e93691bdcad955a69dd1ea74f6bd49aef31b0ad7809fcc9b848df
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/134/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a611841d5f7e93691bdcad955a69dd1ea74f6bd49aef31b0ad7809fcc9b848df"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/111
Content-Type: application/json
Authorization: Bearer 00723a37e8e68e8ddeeaae4fbb66bfb051de88680b07672cd6f3c8e335951faf
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":111,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T09:19:49.271Z","updated_at":"2016-10-18T09:19:49.381Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":172,"author_id":869,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 111,
    "obfuscated_id": "G-D-sgMUtTw",
    "author_id": 869,
    "chapter_id": 172,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:19:49.486Z",
    "created_at": "2016-10-18T09:19:49.271Z",
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
    "question": "{\"id\"=>111, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-18T09:19:49.271Z\", \"updated_at\"=>\"2016-10-18T09:19:49.381Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>172, \"author_id\"=>869, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 224,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 225,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 226,
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
curl "api.goskive.com/v2/questions/111" -d '{"question":{"question":{"id":111,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T09:19:49.271Z","updated_at":"2016-10-18T09:19:49.381Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":172,"author_id":869,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00723a37e8e68e8ddeeaae4fbb66bfb051de88680b07672cd6f3c8e335951faf"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/133/upvote
Content-Type: application/json
Authorization: Bearer a097030a323172b6a90344317e52ec3011b90ced52d5c5e5094b7d1ef050328c
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/133/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a097030a323172b6a90344317e52ec3011b90ced52d5c5e5094b7d1ef050328c"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7a6c61e6d16de714dfde08c24be87f6fef8c4560471804d94021ee1e83145c53
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
      "creator_id": 328,
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 88,
      "additional_university_ids": [

      ],
      "topic_id": 96,
      "discipline_id": 97,
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
      "updated_at": "2016-10-18T09:19:15.344Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a6c61e6d16de714dfde08c24be87f6fef8c4560471804d94021ee1e83145c53"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 85916f0386df7ac011adb1dd028430fe9212931d48147b6406ba688e657b8d8a
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
      "id": 91,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-91",
      "html_url": "https://goskive.com/university/uni-91",
      "slug": "uni-91",
      "name": "National School of Pizza",
      "short_name": "Uni 91",
      "acronym": "NSPI",
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
      "updated_at": "2016-10-18T09:19:15.636Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-90",
      "html_url": "https://goskive.com/university/uni-90",
      "slug": "uni-90",
      "name": "National School of Pastry",
      "short_name": "Uni 90",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/43b5fbbd11770049c4e0f41985099c3831c7f96f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/57b3014ced834e5e114cfe048366ffac65aacc51.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:19:15.620Z",
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
	-H "Authorization: Bearer 85916f0386df7ac011adb1dd028430fe9212931d48147b6406ba688e657b8d8a"
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
      "id": 217,
      "name": "Organized didactic process improvement",
      "name_translations": {
        "en": "Organized didactic process improvement"
      },
      "discipline_id": 218
    },
    {
      "id": 218,
      "name": "Assimilated asymmetric software",
      "name_translations": {
        "en": "Assimilated asymmetric software"
      },
      "discipline_id": 219
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
GET /v2/topics/216
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
    "id": 216,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 217
  }
}
```



```shell
curl "api.goskive.com/v2/topics/216" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer b7bf3cb0ce345fd829466ec6b3dee0e90ad3e212a47f8da448d59f9c32037826
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
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-156",
      "html_url": "https://goskive.com/university/uni-156",
      "slug": "uni-156",
      "name": "University 103",
      "short_name": "Uni 156",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/83b2d5989ee779569c8ad2eee200d3abfb22ca72.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/75c438f84409d4f1ed5af72427787e410156bd1d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:19:27.728Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-157",
      "html_url": "https://goskive.com/university/uni-157",
      "slug": "uni-157",
      "name": "University 104",
      "short_name": "Uni 157",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2b05dbbce89b6e59a75693648a70f24a9591d2e6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f6516c2b5088c7afd095d4c9bcb38a6ddd23e79b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:19:27.746Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-158",
      "html_url": "https://goskive.com/university/uni-158",
      "slug": "uni-158",
      "name": "University 105",
      "short_name": "Uni 158",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/76123b5ff16b651ceaf66a45df5580956c368dcb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/58b7fa766f2c4e6ecaefc44c9a5055487cff0ad6.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:19:27.762Z",
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
	-H "Authorization: Bearer b7bf3cb0ce345fd829466ec6b3dee0e90ad3e212a47f8da448d59f9c32037826"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 902fa1a8ec461cf5eef3f959e157a0b02beea639be00b9dfaecc60afe45d51a6
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
    "id": 159,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e9082b09fb2d7c9043a060e32b9865d46ebff2cd.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/89c3600fb51d5466565dd1883a3ef2cbaceb4ae5.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-18T09:19:27.875Z",
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
	-H "Authorization: Bearer 902fa1a8ec461cf5eef3f959e157a0b02beea639be00b9dfaecc60afe45d51a6"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e3cb73b0e912d5fd8c112cde946c8a35f089b8722b79e9ffd10266ae829de676
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":202,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 593,
    "id": 193,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 178,
    "additional_university_ids": [

    ],
    "topic_id": 202,
    "discipline_id": 203,
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
    "chapters_updated_at": "2016-10-18T09:19:32.101Z",
    "updated_at": "2016-10-18T09:19:32.231Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 131,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-18T09:19:32.190Z",
        "course_id": 193,
        "author_id": 593,
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
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-18T09:19:32.206Z",
        "course_id": 193,
        "author_id": 593,
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
        "id": 133,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-18T09:19:32.222Z",
        "course_id": 193,
        "author_id": 593,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":202,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3cb73b0e912d5fd8c112cde946c8a35f089b8722b79e9ffd10266ae829de676"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 37b746018e76dbb93bc9f1bec80975aaf4d43b4969e39e46815cc2184e559724
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":201,"published":false}}
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
    "creator_id": 592,
    "id": 192,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 177,
    "additional_university_ids": [

    ],
    "topic_id": 201,
    "discipline_id": 202,
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
    "updated_at": "2016-10-18T09:19:32.069Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":201,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37b746018e76dbb93bc9f1bec80975aaf4d43b4969e39e46815cc2184e559724"
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
      "creator_id": 560,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 173,
      "discipline_id": 174,
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
      "updated_at": "2016-10-18T09:19:29.028Z",
      "shortname": "fu-course-106"
    },
    {
      "creator_id": 560,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 174,
      "discipline_id": 175,
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
      "chapters_updated_at": "2016-10-18T09:19:29.311Z",
      "updated_at": "2016-10-18T09:19:29.317Z",
      "shortname": "fu-course-107"
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
Authorization: Bearer 8949bc14307d55de3bba8e24686aedea49ac2cd7a50d528f10f782f1796c0958
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
      "creator_id": 577,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 122",
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
      "updated_at": "2016-10-18T09:19:30.739Z",
      "shortname": "fu-course-122"
    },
    {
      "creator_id": 577,
      "id": 181,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 170,
      "additional_university_ids": [

      ],
      "topic_id": 190,
      "discipline_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "chapters_updated_at": "2016-10-18T09:19:31.081Z",
      "updated_at": "2016-10-18T09:19:31.088Z",
      "shortname": "fu-course-123"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8949bc14307d55de3bba8e24686aedea49ac2cd7a50d528f10f782f1796c0958"
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
      "creator_id": 565,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 178,
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
      "updated_at": "2016-10-18T09:19:29.520Z",
      "shortname": "fu-course-110"
    },
    {
      "creator_id": 565,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 179,
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
      "updated_at": "2016-10-18T09:19:29.565Z",
      "shortname": "fu-course-111"
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
Authorization: Bearer 7b001601098239f4b047859a433a112e45856c239f77f533331cf80a592ece8e
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
      "creator_id": 584,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 193,
      "discipline_id": 194,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "updated_at": "2016-10-18T09:19:31.354Z",
      "shortname": "fu-course-126"
    },
    {
      "creator_id": 584,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 194,
      "discipline_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-10-18T09:19:31.392Z",
      "shortname": "fu-course-127"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b001601098239f4b047859a433a112e45856c239f77f533331cf80a592ece8e"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer a1da01fc554ec9e5631ecde713661ca7aa3e79352b426f09224f88e2575893ab
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
  "id": 520,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-18T09:19:26.500Z",
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
	-H "Authorization: Bearer a1da01fc554ec9e5631ecde713661ca7aa3e79352b426f09224f88e2575893ab"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/523
Content-Type: application/json
Authorization: Bearer 64aec17d4b306557bea297f95217faa444b634401332d9acb102fdc214692262
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
    "id": 523,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 148,
    "fields_of_study": [
      154,
      155
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-18T09:19:26.817Z",
    "updated_at": "2016-10-18T09:19:26.817Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/523" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64aec17d4b306557bea297f95217faa444b634401332d9acb102fdc214692262"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/521
Content-Type: application/json
Authorization: Bearer 8ca2cf57f91010e6c7c2e1db7caada64b6ad2e7f689ff50ed6bf62c991b2c01a
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
    "id": 521,
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
    "created_at": "2016-10-18T09:19:26.679Z",
    "updated_at": "2016-10-18T09:19:26.679Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/521" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ca2cf57f91010e6c7c2e1db7caada64b6ad2e7f689ff50ed6bf62c991b2c01a"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/10
Content-Type: application/json
Authorization: Bearer b915832cbdf9a8f756a0c53daedb43b75157617f9b19585a9e09f994f6d8a229
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b915832cbdf9a8f756a0c53daedb43b75157617f9b19585a9e09f994f6d8a229"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/9
Content-Type: application/json
Authorization: Bearer 27d3bbeeab096a313d1fe8f37027e59d69790fe01b7f63afc008d4936439dc50
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
    "id": 9,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 36,
    "user_id": 115
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27d3bbeeab096a313d1fe8f37027e59d69790fe01b7f63afc008d4936439dc50"
```
