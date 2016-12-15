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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1efd758353e39260e19e29e06bb6fb8199de1ee6b1599365e8cbed3fa57e2b80","client_secret":"0c7e147103ce56659b72743dd3b126319817929a8bbb8a573cc85f9f73a3ef05"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1efd758353e39260e19e29e06bb6fb8199de1ee6b1599365e8cbed3fa57e2b80","client_secret":"0c7e147103ce56659b72743dd3b126319817929a8bbb8a573cc85f9f73a3ef05"}' -X POST \
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
Authorization: Basic YjVjYTdhMjdjMWVjM2ZiZTc1ZTA3OTc2OTk5NjA2NmMwZDc2OGRjYmJhOTdm
YTY4ZTVmODQyM2QwYjI5NWI2YzowNDhhNDBkZjUyNTQ1MzJjOWViNjAxZTVj
N2I0YzhlMTY1NjcyMjBmZmY5MTMyNDk2ZTFkOWJlYTRkYjY0ODAx

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
	-u b5ca7a27c1ec3fbe75e079769996066c0d768dcbba97fa68e5f8423d0b295b6c:048a40df5254532c9eb601e5c7b4c8e16567220fff9132496e1d9bea4db64801
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
{"grant_type":"client_credentials","client_id":"7b0b03e1124853a93989b9a4f40070b71b19d097be51af127a15b394e515cdec","client_secret":"7611dec39692d013c81f34e56a4e2b0e33cb7a8f910cce4ea34a902d9f473694"}
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
  "access_token": "824f756d5cb06482a499d819fc88c56b969ed99401eee25235d44a4289bfbd9f",
  "token_type": "bearer",
  "created_at": 1481808759
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"7b0b03e1124853a93989b9a4f40070b71b19d097be51af127a15b394e515cdec","client_secret":"7611dec39692d013c81f34e56a4e2b0e33cb7a8f910cce4ea34a902d9f473694"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8167be4608cb773859245adae52692acc986cbac1d465215847d50302f2b52b0","client_secret":"5fb7d2eb89972dc9b121fa2285367a24d97fae25aa1d8ec4f050de878d57d34b"}
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
  "access_token": "83ad117e3dbc7bab27150736a5c4f6171561a81abcb683924a5f4f6aee8790fd",
  "token_type": "bearer",
  "created_at": 1481808759
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8167be4608cb773859245adae52692acc986cbac1d465215847d50302f2b52b0","client_secret":"5fb7d2eb89972dc9b121fa2285367a24d97fae25aa1d8ec4f050de878d57d34b"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NGRhY2I0YWMyNTEyM2FmNmRlYzE5MzNhYTljZTA0M2JiY2FiMjExOTlmMWU3
OGI2YjE0MjkzZDhkYzVmNDMxNTozYWVlZGVjNTgyMTIzNDg0ZTgyNTBlNGJk
MjQ3MjgwNjVmMmI1YTJiMTMwZDgzZWQ0OGRkNjczNDE5MGQ3MjQz

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
  "access_token": "11ed0c74431f880ea8586cbbfcd9f6801c9e7d4b4e60e5c5d618cdfcc67d37c1",
  "token_type": "bearer",
  "created_at": 1481808760
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 4dacb4ac25123af6dec1933aa9ce043bbcab21199f1e78b6b14293d8dc5f4315:3aeedec582123484e8250e4bd24728065f2b5a2b130d83ed48dd6734190d7243
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
Authorization: Bearer 27264aa8f93037b948465f79b49b6f4852461e4aaf92b885864542023b399d75
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
curl "api.goskive.com/v2/campaigns/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27264aa8f93037b948465f79b49b6f4852461e4aaf92b885864542023b399d75"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/115/flashcards
Content-Type: application/json
Authorization: Bearer 35089b7515efe63cb234ce82d33b75ef6904d5a86a276e31f26d852c67487782
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":115,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 88,
    "obfuscated_id": "CDc29JqT-RA",
    "author_id": 693,
    "chapter_id": 115,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:06.249Z",
    "created_at": "2016-12-15T13:33:06.249Z",
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
curl "api.goskive.com/v2/chapters/115/flashcards" -d '{"flashcard":{"chapter_id":115,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35089b7515efe63cb234ce82d33b75ef6904d5a86a276e31f26d852c67487782"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/116/flashcards
Content-Type: application/json
Authorization: Bearer c8581e1c7826933fcb58c4ae7d34b2836717e06887060b4e98d69521e607d5eb
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 694,
      "chapter_id": 116,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:06.586Z",
      "created_at": "2016-12-15T13:33:06.586Z",
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
      "author_id": 694,
      "chapter_id": 116,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:06.629Z",
      "created_at": "2016-12-15T13:33:06.629Z",
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
      "author_id": 694,
      "chapter_id": 116,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:06.671Z",
      "created_at": "2016-12-15T13:33:06.671Z",
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
	-H "Authorization: Bearer c8581e1c7826933fcb58c4ae7d34b2836717e06887060b4e98d69521e607d5eb"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/170/questions
Content-Type: application/json
Authorization: Bearer e1337df23e62b555936c73ab33dae169cb0af689cc4bdcbe1cfeddbd8245e32c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":170,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 848,
    "chapter_id": 170,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:21.539Z",
    "created_at": "2016-12-15T13:33:21.539Z",
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
        "id": 219,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 220,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 221,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 222,
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
curl "api.goskive.com/v2/chapters/170/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":170,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1337df23e62b555936c73ab33dae169cb0af689cc4bdcbe1cfeddbd8245e32c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/171/questions
Content-Type: application/json
Authorization: Bearer 5363bfb284493a12f42a13d3410b580a4cb8cfe3f2456591737ef4ec7872fbce
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":171,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 110,
    "obfuscated_id": "55JK4PuG2Hk",
    "author_id": 851,
    "chapter_id": 171,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:22.254Z",
    "created_at": "2016-12-15T13:33:22.254Z",
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
        "id": 223,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 224,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/171/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":171,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5363bfb284493a12f42a13d3410b580a4cb8cfe3f2456591737ef4ec7872fbce"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/172/questions
Content-Type: application/json
Authorization: Bearer fc4ad956873193b541a835b23c5f7221848908c0d082b6a244bb94a51c77a0e4
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 111,
    "obfuscated_id": "G-D-sgMUtTw",
    "author_id": 854,
    "chapter_id": 172,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:22.844Z",
    "created_at": "2016-12-15T13:33:22.844Z",
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
        "id": 225,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 226,
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
curl "api.goskive.com/v2/chapters/172/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc4ad956873193b541a835b23c5f7221848908c0d082b6a244bb94a51c77a0e4"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/169/questions
Content-Type: application/json
Authorization: Bearer 427e33f8de3d95aa52a352ee5bb061ca7d4cabbb5d3906ccb1088a0a04cb4ff2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":169,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 845,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:21.022Z",
    "created_at": "2016-12-15T13:33:21.022Z",
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
        "id": 216,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 217,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 218,
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
curl "api.goskive.com/v2/chapters/169/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":169,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 427e33f8de3d95aa52a352ee5bb061ca7d4cabbb5d3906ccb1088a0a04cb4ff2"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/168/questions
Content-Type: application/json
Authorization: Bearer a156602706fd6f8ed1b3cffaab0ec18fbcabaf09390f9efccf17d30156dca240
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
      "id": 105,
      "obfuscated_id": "3yX9LpVrF_M",
      "author_id": 839,
      "chapter_id": 168,
      "position": 96,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:20.376Z",
      "created_at": "2016-12-15T13:33:20.287Z",
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
          "id": 210,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 211,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 106,
      "obfuscated_id": "GEL902caNek",
      "author_id": 840,
      "chapter_id": 168,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:20.538Z",
      "created_at": "2016-12-15T13:33:20.445Z",
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
          "id": 212,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 213,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 107,
      "obfuscated_id": "_2rgp7tgq8o",
      "author_id": 841,
      "chapter_id": 168,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T13:33:20.703Z",
      "created_at": "2016-12-15T13:33:20.610Z",
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
          "id": 214,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 215,
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
curl "api.goskive.com/v2/chapters/168/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a156602706fd6f8ed1b3cffaab0ec18fbcabaf09390f9efccf17d30156dca240"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/30
Content-Type: application/json
Authorization: Bearer d39b88fa02941816370ec0dfec284776963613a2bda9ee1deeca31705d6bf607
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
curl "api.goskive.com/v2/chapters/30" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d39b88fa02941816370ec0dfec284776963613a2bda9ee1deeca31705d6bf607"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/32
Content-Type: application/json
Authorization: Bearer ff7f1530de90e9b7bc2f21275fb7a078c9416a33f7273f5a89e47b5da0287448
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
curl "api.goskive.com/v2/chapters/32" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff7f1530de90e9b7bc2f21275fb7a078c9416a33f7273f5a89e47b5da0287448"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/33
Content-Type: application/json
Authorization: Bearer e1c98043ea390a884e718e115856d9ad2afb44e83c890455e938a153405659fa
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
curl "api.goskive.com/v2/chapters/33" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1c98043ea390a884e718e115856d9ad2afb44e83c890455e938a153405659fa"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/31
Content-Type: application/json
Authorization: Bearer f38104d95d88c79883d6c8faa76fafe4443d4548fd994d655263595c69cc8cb3
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/31" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f38104d95d88c79883d6c8faa76fafe4443d4548fd994d655263595c69cc8cb3"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/37
Content-Type: application/json
Authorization: Bearer abe2189117f56d98a280044e86e5a6af358e0f236d7fb5edf037db9eb546c2d4
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
    "id": 37,
    "updated_at": "2016-12-15T13:32:21.515Z",
    "course_id": 59,
    "author_id": 218,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T13:32:20.951Z",
    "questions_updated_at": "2016-12-15T13:32:20.951Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 222,
        "chapter_id": 37,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:21.494Z",
        "created_at": "2016-12-15T13:32:21.494Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 220,
        "chapter_id": 37,
        "position": 23,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:21.374Z",
        "created_at": "2016-12-15T13:32:21.276Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abe2189117f56d98a280044e86e5a6af358e0f236d7fb5edf037db9eb546c2d4"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/35
Content-Type: application/json
Authorization: Bearer f1cbaee3199c659cab099299efbc76055da10967ae808341d94a1ff34ae8ce31
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
    "id": 35,
    "updated_at": "2016-12-15T13:32:20.225Z",
    "course_id": 57,
    "author_id": 209,
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
curl "api.goskive.com/v2/chapters/35" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1cbaee3199c659cab099299efbc76055da10967ae808341d94a1ff34ae8ce31"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/59/replies
Content-Type: application/json
Authorization: Bearer 019c02f433b58cf7ef8e90a2c4e23802131c0a7fdacd882854e9f30a0cc6fb33
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
    "id": 60,
    "author_id": 937,
    "reply_to_id": 59,
    "created_at": "2016-12-15T13:33:31.377Z",
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
curl "api.goskive.com/v2/comments/59/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 019c02f433b58cf7ef8e90a2c4e23802131c0a7fdacd882854e9f30a0cc6fb33"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 5296952b573986f5a6458c8cf877bca44a807f6901f9a7480769190676240001
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
curl "api.goskive.com/v2/comments/58/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5296952b573986f5a6458c8cf877bca44a807f6901f9a7480769190676240001"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/16
Content-Type: application/json
Authorization: Bearer 16f9afab138635b8a8531b3047b49a2265a3b31b3357223167cb316a71893b36
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
curl "api.goskive.com/v2/comments/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16f9afab138635b8a8531b3047b49a2265a3b31b3357223167cb316a71893b36"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/18/republish
Content-Type: application/json
Authorization: Bearer 854047755c7455315d1098d32819d0271d3dfd7d4e2c8978de2312f752a0f365
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
curl "api.goskive.com/v2/comments/18/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 854047755c7455315d1098d32819d0271d3dfd7d4e2c8978de2312f752a0f365"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/15
Content-Type: application/json
Authorization: Bearer a421c59f6876d6f4315cf2cf08e052396c086037f628f144f4baa91e3425228b
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a421c59f6876d6f4315cf2cf08e052396c086037f628f144f4baa91e3425228b"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/20/report
Content-Type: application/json
Authorization: Bearer ba99efb33375130f4314e3dd6972a13cadfe0fb744ebb1c353f8f7302b3579ba
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/20/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba99efb33375130f4314e3dd6972a13cadfe0fb744ebb1c353f8f7302b3579ba"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/20
Content-Type: application/json
Authorization: Bearer 94517396081741b6f46e8439fb32a2a2d5cabd18b1dab65979d7654b8b57c014
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
    "id": 20,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T13:32:39.801Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94517396081741b6f46e8439fb32a2a2d5cabd18b1dab65979d7654b8b57c014"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer ea4984f1811e3b5782974f8da5ee32e1a175d39a28973ba180e15a494ce6c989
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
      "id": 17,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T13:32:39.733Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T13:32:39.738Z"
    },
    {
      "id": 19,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T13:32:39.742Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea4984f1811e3b5782974f8da5ee32e1a175d39a28973ba180e15a494ce6c989"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer 0912df251959ce11f77d5e84ab7947824095a727edbaf8fb0f9d929bd3670256
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0912df251959ce11f77d5e84ab7947824095a727edbaf8fb0f9d929bd3670256"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer a4492fd76fb38eadbe75b3809928a6717e65482994ccaaf41450d1e0a3f59ed9
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4492fd76fb38eadbe75b3809928a6717e65482994ccaaf41450d1e0a3f59ed9"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 51506004e006a69c7ad4d23ef715dc2387041e723984cd15df514d545eac036b
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
	-H "Authorization: Bearer 51506004e006a69c7ad4d23ef715dc2387041e723984cd15df514d545eac036b"
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
Authorization: Bearer dfc61b9bd0c50ddd190447d33c3eba6de305a5065d22c714ce37b400e70d0885
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
	-H "Authorization: Bearer dfc61b9bd0c50ddd190447d33c3eba6de305a5065d22c714ce37b400e70d0885"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 594d4bfe983d476b8be4f716380cbd4b84ab3575afbd34de9410ee6174b5159d
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
    "id": 145,
    "updated_at": "2016-12-15T13:33:16.745Z",
    "course_id": 233,
    "author_id": 787,
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
	-H "Authorization: Bearer 594d4bfe983d476b8be4f716380cbd4b84ab3575afbd34de9410ee6174b5159d"
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
      "id": 149,
      "updated_at": "2016-12-15T13:33:17.381Z",
      "course_id": 236,
      "author_id": 796,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 134",
      "position": 1
    },
    {
      "id": 150,
      "updated_at": "2016-12-15T13:33:17.409Z",
      "course_id": 236,
      "author_id": 797,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 135",
      "position": 2
    },
    {
      "id": 151,
      "updated_at": "2016-12-15T13:33:17.640Z",
      "course_id": 236,
      "author_id": 798,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T13:33:17.249Z",
      "questions_updated_at": "2016-12-15T13:33:17.249Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 136",
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
Authorization: Bearer c087e5731ef555ad8727fcb532193c3553a9f16088b98760d8f38c41f0e95e66
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
      "id": 155,
      "updated_at": "2016-12-15T13:33:18.238Z",
      "course_id": 239,
      "author_id": 807,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 140",
      "position": 1
    },
    {
      "id": 156,
      "updated_at": "2016-12-15T13:33:18.264Z",
      "course_id": 239,
      "author_id": 808,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 141",
      "position": 2
    },
    {
      "id": 157,
      "updated_at": "2016-12-15T13:33:18.498Z",
      "course_id": 239,
      "author_id": 809,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T13:33:18.107Z",
      "questions_updated_at": "2016-12-15T13:33:18.107Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 142",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c087e5731ef555ad8727fcb532193c3553a9f16088b98760d8f38c41f0e95e66"
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
      "id": 152,
      "updated_at": "2016-12-15T13:33:17.996Z",
      "course_id": 238,
      "author_id": 803,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 137",
      "position": 1
    },
    {
      "id": 153,
      "updated_at": "2016-12-15T13:33:18.024Z",
      "course_id": 238,
      "author_id": 804,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 138",
      "position": 2
    },
    {
      "id": 154,
      "updated_at": "2016-12-15T13:33:18.051Z",
      "course_id": 238,
      "author_id": 805,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 139",
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
Authorization: Bearer 351953dec327ea5f9d3ecb132c03dbd2dbc14119df90d5a5493d65573f7c6610
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
      "id": 158,
      "updated_at": "2016-12-15T13:33:18.894Z",
      "course_id": 241,
      "author_id": 816,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 143",
      "position": 1
    },
    {
      "id": 159,
      "updated_at": "2016-12-15T13:33:18.922Z",
      "course_id": 241,
      "author_id": 817,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 144",
      "position": 2
    },
    {
      "id": 160,
      "updated_at": "2016-12-15T13:33:18.949Z",
      "course_id": 241,
      "author_id": 818,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 145",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 351953dec327ea5f9d3ecb132c03dbd2dbc14119df90d5a5493d65573f7c6610"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c890e75f151881b80ecd203945b3e4bc67e9403c7dad04105c3ad525f1e53fae
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
    "course_id": 11,
    "user_id": 32,
    "updated_at": "2016-12-15T13:32:04.454Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c890e75f151881b80ecd203945b3e4bc67e9403c7dad04105c3ad525f1e53fae"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f85d25adb3bb6c1002e42e0160ccf7f080668c1486cb8f9d813b77bba6a981c9
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
      "id": 1,
      "course_id": 7,
      "user_id": 20,
      "updated_at": "2016-12-15T13:32:03.647Z"
    },
    {
      "id": 2,
      "course_id": 7,
      "user_id": 21,
      "updated_at": "2016-12-15T13:32:03.663Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f85d25adb3bb6c1002e42e0160ccf7f080668c1486cb8f9d813b77bba6a981c9"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/24/files
Content-Type: application/json
Authorization: Bearer a56b53c75526332a086f9a217fd8cba03da352759aed860fed371c8305d6d499
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
        "id": 76,
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
        "created_at": "2016-12-15T13:32:08.555Z",
        "updated_at": "2016-12-15T13:32:08.555Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T13:32:08.571Z",
      "updated_at": "2016-12-15T13:32:08.571Z",
      "course_id": 24,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 77,
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
        "created_at": "2016-12-15T13:32:08.582Z",
        "updated_at": "2016-12-15T13:32:08.582Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T13:32:08.593Z",
      "updated_at": "2016-12-15T13:32:08.593Z",
      "course_id": 24,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 78,
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
        "created_at": "2016-12-15T13:32:08.604Z",
        "updated_at": "2016-12-15T13:32:08.604Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T13:32:08.614Z",
      "updated_at": "2016-12-15T13:32:08.614Z",
      "course_id": 24,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/24/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a56b53c75526332a086f9a217fd8cba03da352759aed860fed371c8305d6d499"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/21/files
Content-Type: application/json
Authorization: Bearer 806f0e0ea824bd0b08e417920ac94922e40e8c0f8aed2411482d7ad27f2a5497
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
    "id": 1,
    "uploader": {
      "id": 70,
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
      "created_at": "2016-12-15T13:32:07.834Z",
      "updated_at": "2016-12-15T13:32:07.834Z"
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
    "created_at": "2016-12-15T13:32:07.903Z",
    "updated_at": "2016-12-15T13:32:07.903Z",
    "course_id": 21,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/21/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 806f0e0ea824bd0b08e417920ac94922e40e8c0f8aed2411482d7ad27f2a5497"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/22/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 3eeb44dcbb0c23a08dfa079e767c3ea87e3e8908c9e8240e54801c361e267a5d
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
    "key": "cache/1ee2001bf896d1a7abdf6b213cee459c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNDozMjowOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzFlZTIwMDFiZjg5NmQxYTdhYmRmNmIyMTNjZWU0NTljLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDEzMzIwOFoifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T133208Z",
    "x-amz-signature": "9824e8b7f2bbcf637523f564b34cbafdfeeb4a6b606400e6da72ca4899b840d9"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/22/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eeb44dcbb0c23a08dfa079e767c3ea87e3e8908c9e8240e54801c361e267a5d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 06dc77e9795f0ed9283a2b0250afc0de966e4fdb2ecdda36b46ac449b9ae5e74
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
	-H "Authorization: Bearer 06dc77e9795f0ed9283a2b0250afc0de966e4fdb2ecdda36b46ac449b9ae5e74"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7428dd7a60566531aecf54937e653b1a67e70f11a0c1dd86c9c581e2c4ab8e9d
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
	-H "Authorization: Bearer 7428dd7a60566531aecf54937e653b1a67e70f11a0c1dd86c9c581e2c4ab8e9d"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cc21c891762ca6d36efe2183a09f6b35babf4d83239253ec0fa37f5491964b11
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
	-H "Authorization: Bearer cc21c891762ca6d36efe2183a09f6b35babf4d83239253ec0fa37f5491964b11"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3f1028be7eb58c8e6fc4c8f2635f961e1f3088e38efe7326316fed8011d3aa6d
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
	-H "Authorization: Bearer 3f1028be7eb58c8e6fc4c8f2635f961e1f3088e38efe7326316fed8011d3aa6d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c727842600f2551e8f7e54744698523610058a82875537a1143ac9bd6417d98f
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
	-H "Authorization: Bearer c727842600f2551e8f7e54744698523610058a82875537a1143ac9bd6417d98f"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 67cf11f5c039c1598373cf6a4de8ed65d2cf6d228e7b691f8374425dcf6e8461
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
    "creator_id": 529,
    "id": 140,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 146,
    "additional_university_ids": [

    ],
    "discipline_id": 150,
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
    "chapters_updated_at": "2016-12-15T13:32:46.907Z",
    "updated_at": "2016-12-15T13:32:48.454Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 530,
        "chapter_id": 103,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:48.180Z",
        "created_at": "2016-12-15T13:32:48.180Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 530,
        "chapter_id": 104,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:48.274Z",
        "created_at": "2016-12-15T13:32:48.274Z",
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
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 530,
        "chapter_id": 103,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:48.232Z",
        "created_at": "2016-12-15T13:32:48.232Z",
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
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 530,
        "chapter_id": 104,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:48.326Z",
        "created_at": "2016-12-15T13:32:48.326Z",
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
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 530,
        "chapter_id": 103,
        "position": 51,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:47.173Z",
        "created_at": "2016-12-15T13:32:47.067Z",
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
            "id": 101,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 102,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 530,
        "chapter_id": 103,
        "position": 52,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:47.343Z",
        "created_at": "2016-12-15T13:32:47.243Z",
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
            "id": 103,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 104,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 530,
        "chapter_id": 104,
        "position": 53,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:47.550Z",
        "created_at": "2016-12-15T13:32:47.437Z",
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
            "id": 105,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 106,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 530,
        "chapter_id": 104,
        "position": 54,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:47.728Z",
        "created_at": "2016-12-15T13:32:47.623Z",
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
            "id": 107,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 108,
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
        "id": 103,
        "updated_at": "2016-12-15T13:32:48.390Z",
        "course_id": 140,
        "author_id": 529,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T13:32:46.907Z",
        "questions_updated_at": "2016-12-15T13:32:46.907Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 94",
        "position": 1
      },
      {
        "id": 104,
        "updated_at": "2016-12-15T13:32:48.441Z",
        "course_id": 140,
        "author_id": 529,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T13:32:46.907Z",
        "questions_updated_at": "2016-12-15T13:32:46.907Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 95",
        "position": 2
      }
    ],
    "topic_id": 149,
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
	-H "Authorization: Bearer 67cf11f5c039c1598373cf6a4de8ed65d2cf6d228e7b691f8374425dcf6e8461"
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
    "creator_id": 541,
    "id": 142,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 148,
    "additional_university_ids": [

    ],
    "discipline_id": 152,
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
    "chapters_updated_at": "2016-12-15T13:32:50.336Z",
    "updated_at": "2016-12-15T13:32:51.945Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 541,
        "chapter_id": 107,
        "position": 63,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:50.609Z",
        "created_at": "2016-12-15T13:32:50.493Z",
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
            "id": 125,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 126,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 541,
        "chapter_id": 108,
        "position": 65,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T13:32:51.011Z",
        "created_at": "2016-12-15T13:32:50.891Z",
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
            "id": 129,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 130,
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
        "id": 107,
        "updated_at": "2016-12-15T13:32:51.883Z",
        "course_id": 142,
        "author_id": 541,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T13:32:50.336Z",
        "questions_updated_at": "2016-12-15T13:32:50.336Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 98",
        "position": 1
      },
      {
        "id": 108,
        "updated_at": "2016-12-15T13:32:51.933Z",
        "course_id": 142,
        "author_id": 541,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T13:32:50.336Z",
        "questions_updated_at": "2016-12-15T13:32:50.336Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 99",
        "position": 2
      }
    ],
    "topic_id": 151,
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
PUT /v2/courses/144/pin
Content-Type: application/json
Authorization: Bearer 2ebb6fdc903a9320b14e065af57104715ce9eee91e75183d04bcda32d3766b78
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/144/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ebb6fdc903a9320b14e065af57104715ce9eee91e75183d04bcda32d3766b78"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/145/pin
Content-Type: application/json
Authorization: Bearer 5f3812e22314495adc38ecec7586b73eb573ae4a5e7bfbaabf14c593a8162122
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/145/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f3812e22314495adc38ecec7586b73eb573ae4a5e7bfbaabf14c593a8162122"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 69b100a7e0bd8f3927c1857ec6faa524bf8a49ab40ececd9347cf83015b8cb9a
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
    "creator_id": 556,
    "id": 146,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 152,
    "additional_university_ids": [

    ],
    "discipline_id": 156,
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
    "updated_at": "2016-12-15T13:32:54.294Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 155,
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
	-H "Authorization: Bearer 69b100a7e0bd8f3927c1857ec6faa524bf8a49ab40ececd9347cf83015b8cb9a"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 94a80bb22fe073ab2a1c79c7ff61a36382eefca37dfe3b53c1c66087c9020fdf
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
    "id": 352,
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
    "created_at": "2016-12-15T13:32:31.482Z",
    "updated_at": "2016-12-15T13:32:31.482Z",
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
	-H "Authorization: Bearer 94a80bb22fe073ab2a1c79c7ff61a36382eefca37dfe3b53c1c66087c9020fdf"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 3984b5a65fac3365a70120f789cf707a7b8a1cd8fb9731e53cb6f2e22ad356c9
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[91]}
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
    "id": 353,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      91
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T13:32:31.563Z",
    "updated_at": "2016-12-15T13:32:31.607Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[91]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3984b5a65fac3365a70120f789cf707a7b8a1cd8fb9731e53cb6f2e22ad356c9"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 3ac826551302d673c413881c21c13d3edf5c1c00d48f27a6aaa1d689c4973860
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
    "id": 356,
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
    "created_at": "2016-12-15T13:32:31.808Z",
    "updated_at": "2016-12-15T13:32:31.808Z",
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
	-H "Authorization: Bearer 3ac826551302d673c413881c21c13d3edf5c1c00d48f27a6aaa1d689c4973860"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 34e8a965f63b09371978eacdf699e0f241c498a3b1f23ced53d712cdec111011
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[92]}
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
    "id": 354,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      92
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T13:32:31.652Z",
    "updated_at": "2016-12-15T13:32:31.652Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[92]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34e8a965f63b09371978eacdf699e0f241c498a3b1f23ced53d712cdec111011"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 17b3ba863eb0706b4f878ddd6938b7cb912910734d8712791c05327293aaf0a5
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

95
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
    "id": 357,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/6f740e46344c54c6ac6801758a691bcd3cf7fc70.jpg",
    "university_id": null,
    "fields_of_study": [
      95
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T13:32:31.912Z",
    "updated_at": "2016-12-15T13:32:32.174Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/78bb5f066085b42e577e9136dbef22b3a5fdb122.jpg",
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

95
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 17b3ba863eb0706b4f878ddd6938b7cb912910734d8712791c05327293aaf0a5"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 5be09d081963b70db503c93a23c3c5ae302571cfc847446950df438e9315eb58
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
      "bookmarkable_id": 15,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 16,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 17,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5be09d081963b70db503c93a23c3c5ae302571cfc847446950df438e9315eb58"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 854257450d4e039f23a337924a36752e09e856d5ed5f7ca85e9135e107945483
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
      "creator_id": 595,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-119",
      "html_url": "https://goskive.com/course/mit-course-119",
      "slug": "mit-course-119",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "discipline_id": 169,
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
      "updated_at": "2016-12-15T13:32:59.452Z",
      "shortname": "mit-course-119",
      "topic_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 596,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-120",
      "html_url": "https://goskive.com/course/mit-course-120",
      "slug": "mit-course-120",
      "university_id": 166,
      "additional_university_ids": [

      ],
      "discipline_id": 170,
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
      "updated_at": "2016-12-15T13:32:59.588Z",
      "shortname": "mit-course-120",
      "topic_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 120",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 854257450d4e039f23a337924a36752e09e856d5ed5f7ca85e9135e107945483"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer dc33a9e297c926e9282aeebeb011c07b9dbbd20d3e6d4ffc6d92009a6d41c553
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
        "id": 5,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T13:32:08.891Z",
        "updated_at": "2016-12-15T13:32:08.891Z",
        "file_url": "memory://42274f2eb308406049d9dd54612b15a1.pdf",
        "course_id": 25,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 6,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T13:32:09.035Z",
        "updated_at": "2016-12-15T13:32:09.035Z",
        "file_url": "memory://3dd532259c909fcaa2e392bcfcd05261.pdf",
        "course_id": 26,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 7,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-15T13:32:09.173Z",
        "updated_at": "2016-12-15T13:32:09.173Z",
        "file_url": "memory://ec0845ce1b21c8aa5af3e3d83fcea634.pdf",
        "course_id": 27,
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
	-H "Authorization: Bearer dc33a9e297c926e9282aeebeb011c07b9dbbd20d3e6d4ffc6d92009a6d41c553"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 9d2b9e2c8c0928a644f017696c04072ff1c43eefea84b05b4996914fb7feddbb
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
      "company_id": 34,
      "company": {
        "id": 34,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-15T13:33:28.827Z"
      },
      "created_at": "2016-12-15T13:33:28.831Z",
      "updated_at": "2016-12-15T13:33:28.831Z",
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
      "company_id": 35,
      "company": {
        "id": 35,
        "name": "Fake Company Name 30",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-15T13:33:28.841Z"
      },
      "created_at": "2016-12-15T13:33:28.845Z",
      "updated_at": "2016-12-15T13:33:28.845Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d2b9e2c8c0928a644f017696c04072ff1c43eefea84b05b4996914fb7feddbb"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 6ab99f41a124a2843b8ce681b0d04a8819aa38fa131970d31b9d8032ea1c378e
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
      "created_at": "2016-12-15T13:32:04.939Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-12-15T13:32:05.091Z",
      "author_id": "40",
      "thread_subject_id": "13",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 3,
      "created_at": "2016-12-15T13:32:05.080Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-12-15T13:32:05.094Z",
      "author_id": "43",
      "thread_subject_id": "14",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-12-15T13:32:05.513Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-12-15T13:32:05.513Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-12-15T13:32:05.926Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-12-15T13:32:05.926Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 6,
      "created_at": "2016-12-15T13:32:06.361Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-12-15T13:32:06.361Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 7,
      "created_at": "2016-12-15T13:32:06.681Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 5,
      "updated_at": "2016-12-15T13:32:06.681Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-12-15T13:32:07.012Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 6,
      "updated_at": "2016-12-15T13:32:07.012Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-12-15T13:32:07.330Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 7,
      "updated_at": "2016-12-15T13:32:07.330Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ab99f41a124a2843b8ce681b0d04a8819aa38fa131970d31b9d8032ea1c378e"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/1
Content-Type: application/json
Authorization: Bearer b57f1b1c485195866b6937bff60474fb80703e3bcbe7016678b1311111a0998e
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T13:22:04.000Z"}}
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
    "created_at": "2016-12-15T13:32:04.679Z",
    "read_at": "2016-12-15T13:22:04.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-12-15T13:32:04.741Z",
    "author_id": "35",
    "thread_subject_id": "12",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/1" -d '{"notification":{"read_at":"2016-12-15T13:22:04.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b57f1b1c485195866b6937bff60474fb80703e3bcbe7016678b1311111a0998e"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 5200cbd0514dd1e884ec422668c324377fa2985001bcb78096d676b980337b7c
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
      "course_id": 256,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T13:33:24.380Z",
      "course_published": true,
      "updated_at": "2016-12-15T13:33:24.375Z"
    },
    {
      "id": 8,
      "course_id": 257,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T13:33:24.513Z",
      "course_published": true,
      "updated_at": "2016-12-15T13:33:24.508Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5200cbd0514dd1e884ec422668c324377fa2985001bcb78096d676b980337b7c"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 06a29793aeefd31f68ce740ef6c2356df22ad94a650acd635e9729912f1854fb
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
    "course_id": 254,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T13:33:23.956Z",
    "course_published": true,
    "updated_at": "2016-12-15T13:33:23.951Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06a29793aeefd31f68ce740ef6c2356df22ad94a650acd635e9729912f1854fb"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 2e9437b055926f0b105edfa9c4db4f35f2a6d61c3d8d7537899105efb00b114f
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
    "course_id": 255,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T13:33:24.178Z",
    "course_published": true,
    "updated_at": "2016-12-15T13:33:24.170Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e9437b055926f0b105edfa9c4db4f35f2a6d61c3d8d7537899105efb00b114f"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 0b39afc446996c3f017b8ddb5b594473012233743c7a70c4e0d5724e9d4f4f53
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
	-H "Authorization: Bearer 0b39afc446996c3f017b8ddb5b594473012233743c7a70c4e0d5724e9d4f4f53"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/122
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
    "id": 122,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 120,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 122
      },
      {
        "id": 121,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 122
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/122" -X GET \
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
      "id": 120,
      "name": "Enhanced fresh-thinking methodology",
      "name_translations": {
        "en": "Enhanced fresh-thinking methodology"
      }
    },
    {
      "id": 121,
      "name": "Cross-platform object-oriented adapter",
      "name_translations": {
        "en": "Cross-platform object-oriented adapter"
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
PATCH /v2/feedbacks/31/close
Content-Type: application/json
Authorization: Bearer 65e5817911ec912775005821ab9de48c9f1c793a7f4929c95e55c4fec9a18408
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
    "id": 31,
    "user_id": 325,
    "feedbackable_id": 27,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T13:32:29.402Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/31/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65e5817911ec912775005821ab9de48c9f1c793a7f4929c95e55c4fec9a18408"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/33/fix
Content-Type: application/json
Authorization: Bearer bd6e6c77e1407da8abc8cd3c044d2faf6c2d80c9dd9d2a329fcf7a0e1395f5b6
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
    "id": 33,
    "user_id": 335,
    "feedbackable_id": 29,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T13:32:30.220Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/33/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd6e6c77e1407da8abc8cd3c044d2faf6c2d80c9dd9d2a329fcf7a0e1395f5b6"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/9
Content-Type: application/json
Authorization: Bearer 214734ffea72242523dc8ecd16ed55b28b2d6a0613650335ca040582879edb6a
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
    "id": 9,
    "user_id": 227,
    "feedbackable_id": 24,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T13:32:21.845Z",
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
curl "api.goskive.com/v2/feedbacks/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 214734ffea72242523dc8ecd16ed55b28b2d6a0613650335ca040582879edb6a"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/30/close
Content-Type: application/json
Authorization: Bearer 67ce617911cea76e1c9392b6263eddf162cf7ea43644ca948a98c3489e01d467
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
curl "api.goskive.com/v2/feedbacks/30/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67ce617911cea76e1c9392b6263eddf162cf7ea43644ca948a98c3489e01d467"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/fix
Content-Type: application/json
Authorization: Bearer bfc52c7612e5fd4406648812b8b21d0e6e6937eeb9e44b8368813de373a3c637
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
curl "api.goskive.com/v2/feedbacks/35/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfc52c7612e5fd4406648812b8b21d0e6e6937eeb9e44b8368813de373a3c637"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/36/fix
Content-Type: application/json
Authorization: Bearer 4997e83dfbd056b526f3a11f050b01474441a7c3ef3171380bca0f4a822727c3
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
curl "api.goskive.com/v2/feedbacks/36/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4997e83dfbd056b526f3a11f050b01474441a7c3ef3171380bca0f4a822727c3"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/10
Content-Type: application/json
Authorization: Bearer c3e79250b227aca7cdf2333a671282f79c596c842748eb3b38651b5f4a099fae
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
    "id": 10,
    "user_id": 232,
    "feedbackable_id": 25,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T13:32:22.266Z",
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
curl "api.goskive.com/v2/feedbacks/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3e79250b227aca7cdf2333a671282f79c596c842748eb3b38651b5f4a099fae"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer fb821bce104a89cf7344bfb7063bb8e9ce8b82ec8a83176e0b46051182470375
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
	-H "Authorization: Bearer fb821bce104a89cf7344bfb7063bb8e9ce8b82ec8a83176e0b46051182470375"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/10/bookmark
Content-Type: application/json
Authorization: Bearer e210fbb0eb04c85e60d294f0247074b7c3251cd3e064975f137752455a066a80
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
	-H "Authorization: Bearer e210fbb0eb04c85e60d294f0247074b7c3251cd3e064975f137752455a066a80"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer b9ddd1aee2217810ca09d301016b6a10417e27d3e0ac272e99e9bfac49f9b9bd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9ddd1aee2217810ca09d301016b6a10417e27d3e0ac272e99e9bfac49f9b9bd"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/16
Content-Type: application/json
Authorization: Bearer 655ff8b5d615eaa8c97e515672e2748f9a3e1b8db13b47b877c445cc803e8a10
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/c4d116c2452d15003d9efc513e28bafe.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T133241Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=02ebc79d5c78680e814d1f37311c463302f783d199190a836921ed55b3e29985",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 655ff8b5d615eaa8c97e515672e2748f9a3e1b8db13b47b877c445cc803e8a10"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/19/preview
Content-Type: application/json
Authorization: Bearer d60b063b20595969914dab8cf97fc8512829bd7e731850e8a0e6502cefa4bca9
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/1a7129e7372bc6791ad59a5b2ff421e8.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T133242Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=94259c9871ca199018a0950a1cb1a57ee0c36744c2eb06bf91ad748a8d4ce5a0",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/19/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d60b063b20595969914dab8cf97fc8512829bd7e731850e8a0e6502cefa4bca9"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/21/metadata
Content-Type: application/json
Authorization: Bearer fc9a6b325b58571cd0b1518e8fbe743d418323e7339df3195dc24a17735a50be
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
    "id": 21,
    "uploader": {
      "id": 492,
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
      "created_at": "2016-12-15T13:32:42.474Z",
      "updated_at": "2016-12-15T13:32:42.474Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T13:32:42.599Z",
    "updated_at": "2016-12-15T13:32:42.599Z",
    "course_id": 129,
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
curl "api.goskive.com/v2/files/21/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc9a6b325b58571cd0b1518e8fbe743d418323e7339df3195dc24a17735a50be"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer 03bab2e80cfec0ca889b43a9a7c45e18e534e8abf17f724c431d23d2c8b8b6e5
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
      "creator_id": 101,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 36,
      "additional_university_ids": [

      ],
      "discipline_id": 32,
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
      "chapters_updated_at": "2016-12-15T13:32:09.565Z",
      "updated_at": "2016-12-15T13:32:11.013Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 106,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-3c487993-328a-4fb5-8a8d-a6871771d9c8",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-3c487993-328a-4fb5-8a8d-a6871771d9c8",
      "slug": "mit-the-great-british-bake-off-3c487993-328a-4fb5-8a8d-a6871771d9c8",
      "university_id": 37,
      "additional_university_ids": [

      ],
      "discipline_id": 33,
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
      "chapters_updated_at": "2016-12-15T13:32:09.565Z",
      "updated_at": "2016-12-15T13:32:11.428Z",
      "shortname": "mit-the-great-british-bake-off-3c487993-328a-4fb5-8a8d-a6871771d9c8",
      "topic_id": 33,
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
curl "api.goskive.com/v2/files/8/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 03bab2e80cfec0ca889b43a9a7c45e18e534e8abf17f724c431d23d2c8b8b6e5"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/18/download
Content-Type: application/json
Authorization: Bearer fdb266c93fa5d0fc46eb3009a3b50c12f5f0f693bb9d7b67b71749cc1bb4025a
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdb266c93fa5d0fc46eb3009a3b50c12f5f0f693bb9d7b67b71749cc1bb4025a"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/15/report
Content-Type: application/json
Authorization: Bearer f0079c5324447f9a8790ef9f38e84faba1412f9274752eddb38f6d89ab57eeca
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0079c5324447f9a8790ef9f38e84faba1412f9274752eddb38f6d89ab57eeca"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/17/bookmark
Content-Type: application/json
Authorization: Bearer 27163fda4d7fc5f506672aebbdcfd08cb7e6618cfc1f89e1d1ffdb5dd65eb78a
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27163fda4d7fc5f506672aebbdcfd08cb7e6618cfc1f89e1d1ffdb5dd65eb78a"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/14/upvote
Content-Type: application/json
Authorization: Bearer a3cd5bcc64e69fd0ea371b11b7d7fd464d7979c06fe517ee3323b78862116ae5
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3cd5bcc64e69fd0ea371b11b7d7fd464d7979c06fe517ee3323b78862116ae5"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/61/comments
Content-Type: application/json
Authorization: Bearer faed2f81f099b7f219e3bfc518f5d2f88952695923cf470775d2f686ea8fe9d0
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
    "id": 10,
    "author_id": 449,
    "reply_to_id": null,
    "created_at": "2016-12-15T13:32:39.454Z",
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
curl "api.goskive.com/v2/flashcards/61/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faed2f81f099b7f219e3bfc518f5d2f88952695923cf470775d2f686ea8fe9d0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/60/comments
Content-Type: application/json
Authorization: Bearer b92d684a43fcc7746b0c32bb27697efe108424ac70b3a16f1ec9c19a409015a3
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
    "id": 9,
    "author_id": 446,
    "reply_to_id": null,
    "created_at": "2016-12-15T13:32:39.041Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 446,
      "feedbackable_id": 60,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:39.038Z",
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
curl "api.goskive.com/v2/flashcards/60/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b92d684a43fcc7746b0c32bb27697efe108424ac70b3a16f1ec9c19a409015a3"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/58/comments
Content-Type: application/json
Authorization: Bearer 1bc93017077473802ad6505fa17020260fbd88012a7c9557a611a804fae3d4b6
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
      "id": 8,
      "author_id": 442,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:32:38.505Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 441,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:32:38.487Z",
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
curl "api.goskive.com/v2/flashcards/58/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bc93017077473802ad6505fa17020260fbd88012a7c9557a611a804fae3d4b6"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/59/comments
Content-Type: application/json
Authorization: Bearer f28e1cac3b49e7b25f1b0a80949230913a7ea6b48d88e1d912c3029e8cf6efca
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
curl "api.goskive.com/v2/flashcards/59/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f28e1cac3b49e7b25f1b0a80949230913a7ea6b48d88e1d912c3029e8cf6efca"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/16/feedbacks
Content-Type: application/json
Authorization: Bearer 89ab29e0530bd8bb23fe2b0c9d6f4b181b72ebb8df9e427dfd8681c466e5e6cf
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
    "user_id": 150,
    "feedbackable_id": 16,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T13:32:14.350Z",
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
curl "api.goskive.com/v2/flashcards/16/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89ab29e0530bd8bb23fe2b0c9d6f4b181b72ebb8df9e427dfd8681c466e5e6cf"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/10/feedbacks
Content-Type: application/json
Authorization: Bearer 4b19f6525e31ba6087df413970f57bae89ecebbe750ee9803d0a7872c9ef027f
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
      "id": 2,
      "user_id": 124,
      "feedbackable_id": 10,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:12.295Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 1,
      "user_id": 123,
      "feedbackable_id": 10,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:12.282Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/10/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b19f6525e31ba6087df413970f57bae89ecebbe750ee9803d0a7872c9ef027f"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/17/votes
Content-Type: application/json
Authorization: Bearer c81a5a9ec5b85afef41ec6a625cc592d4ecea39dc7ae94eac87bf87929d9daf4
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
      "votable_id": 17,
      "user_id": 182
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 17,
      "user_id": 181
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 17,
      "user_id": 180
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/17/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c81a5a9ec5b85afef41ec6a625cc592d4ecea39dc7ae94eac87bf87929d9daf4"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/33/republish
Content-Type: application/json
Authorization: Bearer 8c832f1b5de5fa5917c55e645c23822fc74d33550f1afa892885c17919bfc812
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
curl "api.goskive.com/v2/flashcards/33/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c832f1b5de5fa5917c55e645c23822fc74d33550f1afa892885c17919bfc812"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/39/bookmark
Content-Type: application/json
Authorization: Bearer 73fab797598b2325e95e1ce25802b8f9415ad98d1562687cc795e8b1ede42991
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73fab797598b2325e95e1ce25802b8f9415ad98d1562687cc795e8b1ede42991"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/35
Content-Type: application/json
Authorization: Bearer ce180b22a10b8d09e34312abf4d2f3a0a77ec893c7f8ca68712feb9c0bdeab91
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce180b22a10b8d09e34312abf4d2f3a0a77ec893c7f8ca68712feb9c0bdeab91"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/downvote
Content-Type: application/json
Authorization: Bearer 486032932d92c6e121ab716b628862834f6d9aa6852239636e1a3ffcc5592492
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 486032932d92c6e121ab716b628862834f6d9aa6852239636e1a3ffcc5592492"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/40
Content-Type: application/json
Authorization: Bearer 2f20db85b379f8baafcfff57d85f6a9c1574e9c0c6488a94b16b8bf9f31e1189
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
    "id": 40,
    "obfuscated_id": "lir5nwklJts",
    "author_id": 379,
    "chapter_id": 73,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:32:34.338Z",
    "created_at": "2016-12-15T13:32:34.338Z",
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
curl "api.goskive.com/v2/flashcards/40" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f20db85b379f8baafcfff57d85f6a9c1574e9c0c6488a94b16b8bf9f31e1189"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/36/report
Content-Type: application/json
Authorization: Bearer 04a888c2182c6e78ee27858a7ba6088b26ee82a683e356d280403e201b423bcb
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/36/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04a888c2182c6e78ee27858a7ba6088b26ee82a683e356d280403e201b423bcb"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/38/bookmark
Content-Type: application/json
Authorization: Bearer 05d2a2e9e0804cbe43443a8d8aec571c60dfa2f2f377661aac8e1ec5da02b04e
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05d2a2e9e0804cbe43443a8d8aec571c60dfa2f2f377661aac8e1ec5da02b04e"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/upvote
Content-Type: application/json
Authorization: Bearer b9d13f2a62cdda4ce7061e5f47f698ec96775880671ac7771b238f07fd182501
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9d13f2a62cdda4ce7061e5f47f698ec96775880671ac7771b238f07fd182501"
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
    "key": "cache/d0bb4eddcfc083882d58beedb3c9abae.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNDozMjowOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2QwYmI0ZWRkY2ZjMDgzODgyZDU4YmVlZGIzYzlhYmFlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTMzMjA5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T133209Z",
    "x-amz-signature": "257185802f0908ba7f0446d8214e10cbb6b8dfcf21d340c1440a45d0ef9e202e"
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
Authorization: Bearer 96c5ad5fe1ceeb8a12eaf98225d51a45c94df265e9c4d3c7f2cf3694cc82282a
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
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96c5ad5fe1ceeb8a12eaf98225d51a45c94df265e9c4d3c7f2cf3694cc82282a"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer d53b626ac758780a17a4828fbe0e09f0502ff20214420096d6b8522b9aad82c3
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
	-H "Authorization: Bearer d53b626ac758780a17a4828fbe0e09f0502ff20214420096d6b8522b9aad82c3"
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
{"password":{"reset_password_token":"z6ZVkzUY3U56a_ASzQs4","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 585,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T13:32:57.650Z",
  "updated_at": "2016-12-15T13:32:57.874Z",
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
  "audit_id": 8216
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"z6ZVkzUY3U56a_ASzQs4","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/48/comments
Content-Type: application/json
Authorization: Bearer 3eb214d07d00396685e4d6400e351969545af021dfc0ded697ab7f51d9db524b
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
    "id": 13,
    "author_id": 520,
    "reply_to_id": null,
    "created_at": "2016-12-15T13:32:45.746Z",
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
curl "api.goskive.com/v2/questions/48/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eb214d07d00396685e4d6400e351969545af021dfc0ded697ab7f51d9db524b"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/50/comments
Content-Type: application/json
Authorization: Bearer 66527aa535644e9e306eccd7bb2a7f8aefbfb8429b1da67754f4a1e065408e6a
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
    "id": 14,
    "author_id": 526,
    "reply_to_id": null,
    "created_at": "2016-12-15T13:32:46.698Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 526,
      "feedbackable_id": 50,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:32:46.695Z",
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
curl "api.goskive.com/v2/questions/50/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66527aa535644e9e306eccd7bb2a7f8aefbfb8429b1da67754f4a1e065408e6a"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/47/comments
Content-Type: application/json
Authorization: Bearer 4a9c852005f09dc45d14a4524eca147db40549aa6925994ffc4df7514c74ee4c
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
      "id": 11,
      "author_id": 518,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:32:45.296Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 519,
      "reply_to_id": null,
      "created_at": "2016-12-15T13:32:45.314Z",
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
curl "api.goskive.com/v2/questions/47/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a9c852005f09dc45d14a4524eca147db40549aa6925994ffc4df7514c74ee4c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/49/comments
Content-Type: application/json
Authorization: Bearer c4bcdeb3bb41026cad923e4d2a1eaea50593eccf9d0ba51a85f055525abd7cee
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
curl "api.goskive.com/v2/questions/49/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4bcdeb3bb41026cad923e4d2a1eaea50593eccf9d0ba51a85f055525abd7cee"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/119/feedbacks
Content-Type: application/json
Authorization: Bearer 74432eee86de36dcb20309a9a67cbc451a528172e1cd8bf0afa2a00df6e67642
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
    "user_id": 903,
    "feedbackable_id": 119,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T13:33:27.647Z",
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
curl "api.goskive.com/v2/questions/119/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74432eee86de36dcb20309a9a67cbc451a528172e1cd8bf0afa2a00df6e67642"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/114/feedbacks
Content-Type: application/json
Authorization: Bearer 6f1d12698d362c607ff1a3612df9f359a623900395b049298ff460479cd6be4a
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
      "user_id": 888,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:33:25.666Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 887,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T13:33:25.654Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/114/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f1d12698d362c607ff1a3612df9f359a623900395b049298ff460479cd6be4a"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/44/votes
Content-Type: application/json
Authorization: Bearer 6b386a5815ff2e169748886da37462a92a4093a39aff6762a5032392dac61e80
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
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 506
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 505
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 504
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/44/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b386a5815ff2e169748886da37462a92a4093a39aff6762a5032392dac61e80"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/98/republish
Content-Type: application/json
Authorization: Bearer 3e320a00872574bcb9d27afbcfe69fbbbdf0d876c31afe5b3ecee0f442bb414a
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
curl "api.goskive.com/v2/questions/98/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e320a00872574bcb9d27afbcfe69fbbbdf0d876c31afe5b3ecee0f442bb414a"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/79/bookmark
Content-Type: application/json
Authorization: Bearer ac4840ad120584b29c6ffcf77fa2e477170f6dd542a728add8ced32138aa6676
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/79/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac4840ad120584b29c6ffcf77fa2e477170f6dd542a728add8ced32138aa6676"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/101
Content-Type: application/json
Authorization: Bearer 81ecf3c12c2f0239c9cf21cf30082613394c125ce1a3ef9ad98d3715fd36f19a
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81ecf3c12c2f0239c9cf21cf30082613394c125ce1a3ef9ad98d3715fd36f19a"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/96/downvote
Content-Type: application/json
Authorization: Bearer 5c5cb59b335e6d4093ceb01bc81591a4acb0b2a0c12830c8d48b5ff818a95143
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/96/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c5cb59b335e6d4093ceb01bc81591a4acb0b2a0c12830c8d48b5ff818a95143"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/80
Content-Type: application/json
Authorization: Bearer a2ae0fedbc73649060d34fe268ba9365e407b497cda9eda517883648bd64f130
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
    "id": 80,
    "obfuscated_id": "94gVa2GR5x8",
    "author_id": 709,
    "chapter_id": 121,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:08.488Z",
    "created_at": "2016-12-15T13:33:08.401Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/80" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2ae0fedbc73649060d34fe268ba9365e407b497cda9eda517883648bd64f130"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/78/report
Content-Type: application/json
Authorization: Bearer c60acdd88fefdbf95ab32af8b36cab8dfdd366f4ac0057ec174a83433bb7ca00
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/78/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c60acdd88fefdbf95ab32af8b36cab8dfdd366f4ac0057ec174a83433bb7ca00"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/97/bookmark
Content-Type: application/json
Authorization: Bearer 4188f2a5b5d30de284890831a0b632e4c249d57b6f643b1c2a5425d0362defe9
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/97/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4188f2a5b5d30de284890831a0b632e4c249d57b6f643b1c2a5425d0362defe9"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/100
Content-Type: application/json
Authorization: Bearer 89f48601e6dc7d26bef9db3485d7c611504c896c411a3f073d7903edfe8cc560
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T13:33:15.081Z","updated_at":"2016-12-15T13:33:15.169Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":141,"author_id":774,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 100,
    "obfuscated_id": "erXmBhoMZFI",
    "author_id": 774,
    "chapter_id": 141,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T13:33:15.264Z",
    "created_at": "2016-12-15T13:33:15.081Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x00000011da8c28>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 201,
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
curl "api.goskive.com/v2/questions/100" -d '{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T13:33:15.081Z","updated_at":"2016-12-15T13:33:15.169Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":141,"author_id":774,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89f48601e6dc7d26bef9db3485d7c611504c896c411a3f073d7903edfe8cc560"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/77/upvote
Content-Type: application/json
Authorization: Bearer e5728d48cfa9cf9c683c032268f3d067e416705c3dc6a8a3aef301bb1736f28d
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/77/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5728d48cfa9cf9c683c032268f3d067e416705c3dc6a8a3aef301bb1736f28d"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer adefdfa2977b35e667fab8e8bfd2b509f971f28ae58717d33708553bd094d733
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
      "creator_id": 907,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 272,
      "additional_university_ids": [

      ],
      "discipline_id": 277,
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
      "updated_at": "2016-12-15T13:33:28.034Z",
      "shortname": "mit-pizza-201",
      "topic_id": 276,
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
	-H "Authorization: Bearer adefdfa2977b35e667fab8e8bfd2b509f971f28ae58717d33708553bd094d733"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 76e977bd45885e400e95c1080d093b9aaaa215da5505e670e121c7ff8c31bdbd
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
      "id": 275,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-273",
      "html_url": "https://goskive.com/university/uni-273",
      "slug": "uni-273",
      "name": "National School of Pizza",
      "short_name": "Uni 273",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/3402ec7af1346462cf2034343f067273.jpg",
      "image_url_small": "memory://universities/98ab398d4ffd4d410d642b835b1a5847.jpg",
      "image_thumb_url": "memory://universities/fd30d1746b3f916278c3c3854475b612.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T13:33:28.384Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-272",
      "html_url": "https://goskive.com/university/uni-272",
      "slug": "uni-272",
      "name": "National School of Pastry",
      "short_name": "Uni 272",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/00a52c7288f871818c8beff9b3e69b8d.jpg",
      "image_url_small": "memory://universities/3b01b7870b812228c5c85e56b188b02a.jpg",
      "image_thumb_url": "memory://universities/1d658d1af02f4ff3698841449405b9d1.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T13:33:28.314Z",
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
	-H "Authorization: Bearer 76e977bd45885e400e95c1080d093b9aaaa215da5505e670e121c7ff8c31bdbd"
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
      "id": 287,
      "name": "Persevering 4th generation circuit",
      "name_translations": {
        "en": "Persevering 4th generation circuit"
      },
      "discipline_id": 288
    },
    {
      "id": 288,
      "name": "Secured multi-state benchmark",
      "name_translations": {
        "en": "Secured multi-state benchmark"
      },
      "discipline_id": 289
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
GET /v2/topics/286
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
    "id": 286,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 287
  }
}
```



```shell
curl "api.goskive.com/v2/topics/286" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer c3ed6f301c3f456b2bc560889dd6bcd58662e7150f11e9ec9654e7626a7acc89
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
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-4",
      "html_url": "https://goskive.com/university/uni-4",
      "slug": "uni-4",
      "name": "University 4",
      "short_name": "Uni 4",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/a739d6bec4410535991080c491f209c4.jpg",
      "image_url_small": "memory://universities/1e3f75405946d64ff74356cdec7885a2.jpg",
      "image_thumb_url": "memory://universities/73dccd1b533d23c96573349464ad78ee.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T13:32:01.750Z",
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
      "image_url": "memory://universities/c0ba92d7a6ccfca8282e854de694f87c.jpg",
      "image_url_small": "memory://universities/caf05846b5b1d86e227779161496e995.jpg",
      "image_thumb_url": "memory://universities/505dbec910fbcd01afa4cf0b19b85030.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T13:32:01.618Z",
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
      "image_url": "memory://universities/da9907baa8b3176b288b5e686bb7b014.jpg",
      "image_url_small": "memory://universities/3b25911b94fc56cb798ada18da39e5c8.jpg",
      "image_thumb_url": "memory://universities/8978f98dae0402767fee03c496169735.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T13:32:01.682Z",
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
	-H "Authorization: Bearer c3ed6f301c3f456b2bc560889dd6bcd58662e7150f11e9ec9654e7626a7acc89"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 6a277555219b8a4fe7f55575798a6701997e6ed13f948175033b2951c831a49b
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
    "id": 6,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/1c701cd93453cb42a45fbd5f90ac2561.jpg",
    "image_url_small": "memory://universities/079efe827f85fbdf7db43d8be1c01b41.jpg",
    "image_thumb_url": "memory://universities/ac0fb25e321f66385e05dc0ee1c2b770.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T13:32:02.049Z",
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
	-H "Authorization: Bearer 6a277555219b8a4fe7f55575798a6701997e6ed13f948175033b2951c831a49b"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 47a7812147b19583bfe2d355b80b3001ae2112563bfc47410197f8616d275773
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":291,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 946,
    "id": 279,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 286,
    "additional_university_ids": [

    ],
    "discipline_id": 292,
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
    "chapters_updated_at": "2016-12-15T13:33:32.900Z",
    "updated_at": "2016-12-15T13:33:33.069Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 189,
        "updated_at": "2016-12-15T13:33:33.057Z",
        "course_id": 279,
        "author_id": 946,
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
        "id": 190,
        "updated_at": "2016-12-15T13:33:33.071Z",
        "course_id": 279,
        "author_id": 946,
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
        "id": 191,
        "updated_at": "2016-12-15T13:33:33.085Z",
        "course_id": 279,
        "author_id": 946,
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
    "topic_id": 291,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":291,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47a7812147b19583bfe2d355b80b3001ae2112563bfc47410197f8616d275773"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 937e3f47c8e27dc2671a96988171ffcfb800f73b02f5eb3fb04f10553cfb34b3
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":290,"published":false}}
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
    "creator_id": 945,
    "id": 278,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 285,
    "additional_university_ids": [

    ],
    "discipline_id": 291,
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
    "updated_at": "2016-12-15T13:33:32.852Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 290,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":290,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 937e3f47c8e27dc2671a96988171ffcfb800f73b02f5eb3fb04f10553cfb34b3"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3792c9bae2f0abb33dd717045bbc2d33d2b1c5c7a23018ba909f539f12e01aa9
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
      "creator_id": 953,
      "id": 287,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "discipline_id": 300,
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
      "updated_at": "2016-12-15T13:33:33.994Z",
      "shortname": "fu-course-215",
      "topic_id": 299,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 953,
      "id": 288,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-216",
      "html_url": "https://goskive.com/course/fu-course-216",
      "slug": "fu-course-216",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "discipline_id": 301,
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
      "chapters_updated_at": "2016-12-15T13:33:33.808Z",
      "updated_at": "2016-12-15T13:33:34.266Z",
      "shortname": "fu-course-216",
      "topic_id": 300,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 216",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3792c9bae2f0abb33dd717045bbc2d33d2b1c5c7a23018ba909f539f12e01aa9"
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
      "creator_id": 983,
      "id": 311,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-239",
      "html_url": "https://goskive.com/course/fu-course-239",
      "slug": "fu-course-239",
      "university_id": 299,
      "additional_university_ids": [

      ],
      "discipline_id": 324,
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
      "updated_at": "2016-12-15T13:33:37.058Z",
      "shortname": "fu-course-239",
      "topic_id": 323,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 239",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 983,
      "id": 312,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-240",
      "html_url": "https://goskive.com/course/fu-course-240",
      "slug": "fu-course-240",
      "university_id": 299,
      "additional_university_ids": [

      ],
      "discipline_id": 325,
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
      "chapters_updated_at": "2016-12-15T13:33:36.869Z",
      "updated_at": "2016-12-15T13:33:37.331Z",
      "shortname": "fu-course-240",
      "topic_id": 324,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 240",
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
Authorization: Bearer d2cfb74cd04dbf286cfbce1641f6568af1bc8731c7a3b75847003141afe93bfe
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
      "creator_id": 959,
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-219",
      "html_url": "https://goskive.com/course/fu-course-219",
      "slug": "fu-course-219",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "discipline_id": 304,
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
      "updated_at": "2016-12-15T13:33:34.549Z",
      "shortname": "fu-course-219",
      "topic_id": 303,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 219",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 959,
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-220",
      "html_url": "https://goskive.com/course/fu-course-220",
      "slug": "fu-course-220",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "discipline_id": 305,
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
      "updated_at": "2016-12-15T13:33:34.585Z",
      "shortname": "fu-course-220",
      "topic_id": 304,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 220",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2cfb74cd04dbf286cfbce1641f6568af1bc8731c7a3b75847003141afe93bfe"
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
      "creator_id": 988,
      "id": 315,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-243",
      "html_url": "https://goskive.com/course/fu-course-243",
      "slug": "fu-course-243",
      "university_id": 300,
      "additional_university_ids": [

      ],
      "discipline_id": 328,
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
      "updated_at": "2016-12-15T13:33:37.558Z",
      "shortname": "fu-course-243",
      "topic_id": 327,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 243",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 988,
      "id": 316,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-244",
      "html_url": "https://goskive.com/course/fu-course-244",
      "slug": "fu-course-244",
      "university_id": 300,
      "additional_university_ids": [

      ],
      "discipline_id": 329,
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
      "updated_at": "2016-12-15T13:33:37.595Z",
      "shortname": "fu-course-244",
      "topic_id": 328,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 244",
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
Authorization: Bearer 613202f1255d15bcd56c470653870d2c467a3f01d6c995990956006f7259618d
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
  "id": 189,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T13:32:18.257Z",
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
	-H "Authorization: Bearer 613202f1255d15bcd56c470653870d2c467a3f01d6c995990956006f7259618d"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/87
Content-Type: application/json
Authorization: Bearer 9dc28e2bac69403083e3543d83fee02b7017e3311b508c8296db3e8c6f8264b8
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
    "id": 87,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 33,
    "fields_of_study": [
      28,
      29
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T13:32:09.402Z",
    "updated_at": "2016-12-15T13:32:09.402Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/87" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9dc28e2bac69403083e3543d83fee02b7017e3311b508c8296db3e8c6f8264b8"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/89
Content-Type: application/json
Authorization: Bearer 8e27611b1f7119c7538ef8745d691283560a1ef7ac9f71f6f7d3b55fc071cedc
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
    "id": 89,
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
    "created_at": "2016-12-15T13:32:09.499Z",
    "updated_at": "2016-12-15T13:32:09.499Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/89" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e27611b1f7119c7538ef8745d691283560a1ef7ac9f71f6f7d3b55fc071cedc"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/5
Content-Type: application/json
Authorization: Bearer 394c39b9362030b83e863627e0fa37e2bbdb1cd276f8e7a84663d9fbdb67e40e
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 394c39b9362030b83e863627e0fa37e2bbdb1cd276f8e7a84663d9fbdb67e40e"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/4
Content-Type: application/json
Authorization: Bearer 799722c3fa32b732a1bae563aced4237ccf04a596afa62d38fdfe25592704567
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
    "id": 4,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 12,
    "user_id": 154
  }
}
```



```shell
curl "api.goskive.com/v2/votes/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 799722c3fa32b732a1bae563aced4237ccf04a596afa62d38fdfe25592704567"
```
