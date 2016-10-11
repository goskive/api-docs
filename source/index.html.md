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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"778ff50e812b5deee0b063778afe6e518b981f418c48d53069cb8d045563938c","client_secret":"dc71db94136c537034dec87cb957f3f1d0b7a998f06f03632d1d58a53700500d"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"778ff50e812b5deee0b063778afe6e518b981f418c48d53069cb8d045563938c","client_secret":"dc71db94136c537034dec87cb957f3f1d0b7a998f06f03632d1d58a53700500d"}' -X POST \
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
Authorization: Basic YjlkYTk0MzRkYzcwNDI3ODFiOGU4NTU0OGY4MGE3MGEzY2QyMzUzZmEwMjFi
NWJhOTU5OTExZDZjOGQ0MWRiNDowZDZhYWNiZmE5YWMxY2I3M2VhNjE4MjY1
ZGViNDQ5N2I4ZTYzODJlOGE2OTllNDhlZWJhNWRlN2Q2Mjc5YmRi

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
	-u b9da9434dc7042781b8e85548f80a70a3cd2353fa021b5ba959911d6c8d41db4:0d6aacbfa9ac1cb73ea618265deb4497b8e6382e8a699e48eeba5de7d6279bdb
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
{"grant_type":"client_credentials","client_id":"978dedb02b99dcb6cb802b5cb9f0a2bbd29372511a481c811475ac2f007a93e9","client_secret":"dcb5c95f89090b44ba062797d8e14b82c4ac4b33c96156a21c744d5d426f652c"}
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
  "access_token": "b6447a8801cffb0cbdcb81110c877fa9aadb32f1ab9500f47fb615e02cec38d7",
  "token_type": "bearer",
  "created_at": 1476205212
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"978dedb02b99dcb6cb802b5cb9f0a2bbd29372511a481c811475ac2f007a93e9","client_secret":"dcb5c95f89090b44ba062797d8e14b82c4ac4b33c96156a21c744d5d426f652c"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"62c37e118cb377d2647530b7fcecb07bf88702f05ae4b4129d1a93653f5b05ac","client_secret":"67ea8a2ab2f237fc58f00a8be08fbcbd1e1a06c5042b77a8ed76cd31e70e3146"}
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
  "access_token": "248610300b1b3807dd8a8c1e758cb602273db1440a60cc646cea4d1c9c5e55e4",
  "token_type": "bearer",
  "created_at": 1476205212
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"62c37e118cb377d2647530b7fcecb07bf88702f05ae4b4129d1a93653f5b05ac","client_secret":"67ea8a2ab2f237fc58f00a8be08fbcbd1e1a06c5042b77a8ed76cd31e70e3146"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic N2YzY2YxZWQ5Y2MwZDFlOGM0MzliMzg5Zjk5NjBiYWZhYzExZWY1ZWY3ZjU0
M2IyZWFkMmIyNTNhOTE0ODE2NjpiOWU2OGY3NjJlYTYxNTNlOTQ2MzM0Y2Qz
MTcwODY2OGU3NmEzOWY5NWUwNmY0OGJkNDdlN2FlMjJmY2M0OTZh

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
  "access_token": "330da26b6df88887f8f1603a7b46d57caaf73e04e1f3c0460d8a23b7bba6b9ce",
  "token_type": "bearer",
  "created_at": 1476205212
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 7f3cf1ed9cc0d1e8c439b389f9960bafac11ef5ef7f543b2ead2b253a9148166:b9e68f762ea6153e946334cd31708668e76a39f95e06f48bd47e7ae22fcc496a
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
Authorization: Bearer 575519aa2289e74f30a49d0742bf45bd0e73140695a6060fec76069ba8415b9c
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
	-H "Authorization: Bearer 575519aa2289e74f30a49d0742bf45bd0e73140695a6060fec76069ba8415b9c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/186/flashcards
Content-Type: application/json
Authorization: Bearer 6be4261dc0a45acdd549e99114aa3835bb0179c76adec98906d48e7c9c1ea061
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":186,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 91,
    "obfuscated_id": "EqPpyB0JN58",
    "author_id": 921,
    "chapter_id": 186,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T17:00:33.262Z",
    "created_at": "2016-10-11T17:00:33.262Z",
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
curl "api.goskive.com/v2/chapters/186/flashcards" -d '{"flashcard":{"chapter_id":186,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6be4261dc0a45acdd549e99114aa3835bb0179c76adec98906d48e7c9c1ea061"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/184/flashcards
Content-Type: application/json
Authorization: Bearer eb6366af4f486a0c6dc6982719407725c9f2f026873156b387105c91312dcfd3
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 913,
      "chapter_id": 184,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:32.824Z",
      "created_at": "2016-10-11T17:00:32.824Z",
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 913,
      "chapter_id": 184,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:32.863Z",
      "created_at": "2016-10-11T17:00:32.863Z",
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
      "author_id": 913,
      "chapter_id": 184,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:32.901Z",
      "created_at": "2016-10-11T17:00:32.901Z",
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
curl "api.goskive.com/v2/chapters/184/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb6366af4f486a0c6dc6982719407725c9f2f026873156b387105c91312dcfd3"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/143/questions
Content-Type: application/json
Authorization: Bearer e7a60d76205029ab16de960d1c3dfdf69c12ecd59affc24dc70311a338a930fd
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":143,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 768,
    "chapter_id": 143,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T17:00:21.125Z",
    "created_at": "2016-10-11T17:00:21.125Z",
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
curl "api.goskive.com/v2/chapters/143/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":143,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7a60d76205029ab16de960d1c3dfdf69c12ecd59affc24dc70311a338a930fd"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/142/questions
Content-Type: application/json
Authorization: Bearer b58547e011a9e6b7a82fc0a68c69e0440ea8f1123b9f5476cb07d4f64029ee35
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":142,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 105,
    "obfuscated_id": "3yX9LpVrF_M",
    "author_id": 765,
    "chapter_id": 142,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T17:00:20.760Z",
    "created_at": "2016-10-11T17:00:20.760Z",
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
        "id": 210,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 211,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/142/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":142,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b58547e011a9e6b7a82fc0a68c69e0440ea8f1123b9f5476cb07d4f64029ee35"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/145/questions
Content-Type: application/json
Authorization: Bearer 7441c9eddfaca663d8fbbc86b96d1b7fb3e66db7544978d93e907b37c5aadebc
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 774,
    "chapter_id": 145,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T17:00:22.085Z",
    "created_at": "2016-10-11T17:00:22.085Z",
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
        "id": 219,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 220,
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
curl "api.goskive.com/v2/chapters/145/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7441c9eddfaca663d8fbbc86b96d1b7fb3e66db7544978d93e907b37c5aadebc"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/144/questions
Content-Type: application/json
Authorization: Bearer ee0022ed6d84ccd6fdbf6118bfd4b291a736dac612cec57661578f9a5127fda0
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":144,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 771,
    "chapter_id": 144,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T17:00:21.653Z",
    "created_at": "2016-10-11T17:00:21.653Z",
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
curl "api.goskive.com/v2/chapters/144/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":144,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee0022ed6d84ccd6fdbf6118bfd4b291a736dac612cec57661578f9a5127fda0"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/141/questions
Content-Type: application/json
Authorization: Bearer 7eac93ffd89d2bd1e202b1919e30e0d7d7a7e53ad8e8ac4444d3d7c2bf7b0a02
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
      "id": 102,
      "obfuscated_id": "jFy90P7ldB4",
      "author_id": 759,
      "chapter_id": 141,
      "position": 93,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:20.088Z",
      "created_at": "2016-10-11T17:00:19.971Z",
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
          "id": 204,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 205,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 103,
      "obfuscated_id": "AVhVflMAvL0",
      "author_id": 760,
      "chapter_id": 141,
      "position": 94,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:20.283Z",
      "created_at": "2016-10-11T17:00:20.164Z",
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
          "id": 206,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 207,
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
      "author_id": 761,
      "chapter_id": 141,
      "position": 95,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-11T17:00:20.481Z",
      "created_at": "2016-10-11T17:00:20.359Z",
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
          "id": 208,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 209,
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
curl "api.goskive.com/v2/chapters/141/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7eac93ffd89d2bd1e202b1919e30e0d7d7a7e53ad8e8ac4444d3d7c2bf7b0a02"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/150
Content-Type: application/json
Authorization: Bearer 1b82191abcc2ba21cc3e80ecb146209333540533ad29ed800a7037ecf43191ea
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
curl "api.goskive.com/v2/chapters/150" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b82191abcc2ba21cc3e80ecb146209333540533ad29ed800a7037ecf43191ea"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/152
Content-Type: application/json
Authorization: Bearer 43a2b48c9a25fc7c22eafb5bf241c7a3a2e1a19ce9dbc2116fe73512de6a0492
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
curl "api.goskive.com/v2/chapters/152" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43a2b48c9a25fc7c22eafb5bf241c7a3a2e1a19ce9dbc2116fe73512de6a0492"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/158
Content-Type: application/json
Authorization: Bearer 13822ec4923e587fe064c78ef0bf33f67dceb7e613a55a1c8443e1df78d79120
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
curl "api.goskive.com/v2/chapters/158" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13822ec4923e587fe064c78ef0bf33f67dceb7e613a55a1c8443e1df78d79120"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/153
Content-Type: application/json
Authorization: Bearer 35d6effbc2761ced0106762f72a7446c50e757fa15db121b9caf93614bd0c71c
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/153" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35d6effbc2761ced0106762f72a7446c50e757fa15db121b9caf93614bd0c71c"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/155
Content-Type: application/json
Authorization: Bearer ede29e216321e5c6da40aee5dce7b9809a3c2405a36089d000e493737293362f
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
    "id": 155,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-11T17:00:28.019Z",
    "course_id": 270,
    "author_id": 828,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-11T17:00:27.428Z",
    "questions_updated_at": "2016-10-11T17:00:27.428Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 832,
        "chapter_id": 155,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:28.001Z",
        "created_at": "2016-10-11T17:00:28.001Z",
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
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 830,
        "chapter_id": 155,
        "position": 105,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T17:00:27.880Z",
        "created_at": "2016-10-11T17:00:27.756Z",
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
            "id": 239,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 240,
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
curl "api.goskive.com/v2/chapters/155" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ede29e216321e5c6da40aee5dce7b9809a3c2405a36089d000e493737293362f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/156
Content-Type: application/json
Authorization: Bearer 64c21b8cdf42fc816249502c77f49756a621a25012d7a77eb9ba4605749c3883
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
    "id": 156,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-11T17:00:28.269Z",
    "course_id": 271,
    "author_id": 835,
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
curl "api.goskive.com/v2/chapters/156" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64c21b8cdf42fc816249502c77f49756a621a25012d7a77eb9ba4605749c3883"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/12/replies
Content-Type: application/json
Authorization: Bearer 75f42efa2246c1aa3dd34ed51e7091fa8effa07c287d838b1e3825ec6e9f2fda
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
    "id": 13,
    "author_id": 408,
    "reply_to_id": 12,
    "created_at": "2016-10-11T16:59:55.084Z",
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
curl "api.goskive.com/v2/comments/12/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75f42efa2246c1aa3dd34ed51e7091fa8effa07c287d838b1e3825ec6e9f2fda"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/14/replies
Content-Type: application/json
Authorization: Bearer 73ab85944fb5c63a767dfc35140f25c7acd2d68c8a3832b0f454f190a6401917
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
curl "api.goskive.com/v2/comments/14/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73ab85944fb5c63a767dfc35140f25c7acd2d68c8a3832b0f454f190a6401917"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer 52bded342bc62ccbeb91fea71c21a609ff52056216275224dacf070f4f843fa2
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
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52bded342bc62ccbeb91fea71c21a609ff52056216275224dacf070f4f843fa2"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/15/republish
Content-Type: application/json
Authorization: Bearer 4b984fa08b5c4d11aa2debcee2ef8128b90d27ab7fd098d30b702a6613be7402
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
curl "api.goskive.com/v2/comments/15/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b984fa08b5c4d11aa2debcee2ef8128b90d27ab7fd098d30b702a6613be7402"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer cb508bcc9bfc48f41b6c1783f9f4614454d7925fbefaa85e25cabc414bef736a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb508bcc9bfc48f41b6c1783f9f4614454d7925fbefaa85e25cabc414bef736a"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/17/report
Content-Type: application/json
Authorization: Bearer fb3b09ca950c3a1e905ee45ae0e599eb5606be90241fa3985d827d564462b31e
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb3b09ca950c3a1e905ee45ae0e599eb5606be90241fa3985d827d564462b31e"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 91e3e85dfa4a2073c3b575d39c9147c962bf587c7f1655bade59772968a3b087
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
    "id": 36,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-11T17:00:28.802Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91e3e85dfa4a2073c3b575d39c9147c962bf587c7f1655bade59772968a3b087"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f4ac32ff15a6d18b6ba384312eec1aa398c50ed3816ea818382907c53c4ef34b
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
      "id": 37,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-11T17:00:28.953Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-11T17:00:28.958Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-11T17:00:28.964Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4ac32ff15a6d18b6ba384312eec1aa398c50ed3816ea818382907c53c4ef34b"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/35/company_profiles
Content-Type: application/json
Authorization: Bearer 6e3f1ae864454d1714fe254e0f06895b15335bfc55e6d5bc00ab751636eed29f
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
	-H "Authorization: Bearer 6e3f1ae864454d1714fe254e0f06895b15335bfc55e6d5bc00ab751636eed29f"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/33/company_profiles
Content-Type: application/json
Authorization: Bearer f62ce012fbbceeea2d46c2a80abe5c3898cfd2edfd3191918c01cf0dd46746cf
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
curl "api.goskive.com/v2/companies/33/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f62ce012fbbceeea2d46c2a80abe5c3898cfd2edfd3191918c01cf0dd46746cf"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 196943395d5c25964e3c73966f116b869fb5e3cfa1bec4a253d7a0f69386d14c
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 1,
      "precluded_campaign_ids": [

      ],
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
      "id": 4,
      "title": "Campaign 4",
      "company_id": 4,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 2,
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
	-H "Authorization: Bearer 196943395d5c25964e3c73966f116b869fb5e3cfa1bec4a253d7a0f69386d14c"
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
Authorization: Bearer b1c7a2207865ff44bcc77e2752b93a3ca78843f52459280e2388717735cf7ff8
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
	-H "Authorization: Bearer b1c7a2207865ff44bcc77e2752b93a3ca78843f52459280e2388717735cf7ff8"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7cd6824f70c4d789ffe5379b915808a0dc676afc2ee22f5fd68bdf46721f9506
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
    "id": 181,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-11T17:00:32.279Z",
    "course_id": 290,
    "author_id": 906,
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
	-H "Authorization: Bearer 7cd6824f70c4d789ffe5379b915808a0dc676afc2ee22f5fd68bdf46721f9506"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 47d9a8ea481567e8a757d3a8b2743d21787489a0e385f5bdd9dd9e88b9717d60
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
      "id": 169,
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-11T17:00:30.724Z",
      "course_id": 284,
      "author_id": 881,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 170,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-11T17:00:30.751Z",
      "course_id": 284,
      "author_id": 882,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 171,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-11T17:00:31.023Z",
      "course_id": 284,
      "author_id": 883,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-11T17:00:30.640Z",
      "questions_updated_at": "2016-10-11T17:00:30.640Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47d9a8ea481567e8a757d3a8b2743d21787489a0e385f5bdd9dd9e88b9717d60"
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
      "id": 175,
      "title": "Clever Chapter Title 157",
      "position": 1,
      "updated_at": "2016-10-11T17:00:31.574Z",
      "course_id": 287,
      "author_id": 895,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 176,
      "title": "Clever Chapter Title 158",
      "position": 2,
      "updated_at": "2016-10-11T17:00:31.600Z",
      "course_id": 287,
      "author_id": 896,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 177,
      "title": "Clever Chapter Title 159",
      "position": 3,
      "updated_at": "2016-10-11T17:00:31.866Z",
      "course_id": 287,
      "author_id": 897,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-11T17:00:31.459Z",
      "questions_updated_at": "2016-10-11T17:00:31.459Z",
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
Authorization: Bearer d5ffa83720f1762b137379b189a074802315f0b35275c121b8da0dbda4601bcb
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
      "id": 172,
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-11T17:00:31.314Z",
      "course_id": 286,
      "author_id": 890,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 173,
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-11T17:00:31.343Z",
      "course_id": 286,
      "author_id": 891,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 174,
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-11T17:00:31.371Z",
      "course_id": 286,
      "author_id": 892,
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
	-H "Authorization: Bearer d5ffa83720f1762b137379b189a074802315f0b35275c121b8da0dbda4601bcb"
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
      "id": 178,
      "title": "Clever Chapter Title 160",
      "position": 1,
      "updated_at": "2016-10-11T17:00:31.992Z",
      "course_id": 288,
      "author_id": 901,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 179,
      "title": "Clever Chapter Title 161",
      "position": 2,
      "updated_at": "2016-10-11T17:00:32.019Z",
      "course_id": 288,
      "author_id": 902,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 180,
      "title": "Clever Chapter Title 162",
      "position": 3,
      "updated_at": "2016-10-11T17:00:32.046Z",
      "course_id": 288,
      "author_id": 903,
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
Authorization: Bearer f362fbf2f0dfd93c81385efe7b913349b99f58a08259e63c4849f7f56056e9c3
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
    "course_id": 119,
    "user_id": 415,
    "updated_at": "2016-10-11T16:59:55.718Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f362fbf2f0dfd93c81385efe7b913349b99f58a08259e63c4849f7f56056e9c3"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 63408a1bc335b697ddb67358ae411a7cbf8ba29ebe4424963b11daa10f79b03c
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
      "course_id": 123,
      "user_id": 425,
      "updated_at": "2016-10-11T16:59:56.243Z"
    },
    {
      "id": 7,
      "course_id": 123,
      "user_id": 426,
      "updated_at": "2016-10-11T16:59:56.259Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63408a1bc335b697ddb67358ae411a7cbf8ba29ebe4424963b11daa10f79b03c"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/276/files
Content-Type: application/json
Authorization: Bearer 649040cf3ea300fdc4a070fe304eac2f40fe1642f549a23ea55ccb38a6e092a2
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
      "id": 8,
      "uploader": {
        "id": 851,
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
        "created_at": "2016-10-11T17:00:29.214Z",
        "updated_at": "2016-10-11T17:00:29.214Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-11T17:00:29.221Z",
      "updated_at": "2016-10-11T17:00:29.221Z",
      "course_id": 276,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 852,
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
        "created_at": "2016-10-11T17:00:29.230Z",
        "updated_at": "2016-10-11T17:00:29.230Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-11T17:00:29.238Z",
      "updated_at": "2016-10-11T17:00:29.238Z",
      "course_id": 276,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 10,
      "uploader": {
        "id": 853,
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
        "created_at": "2016-10-11T17:00:29.245Z",
        "updated_at": "2016-10-11T17:00:29.245Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-11T17:00:29.252Z",
      "updated_at": "2016-10-11T17:00:29.252Z",
      "course_id": 276,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/276/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 649040cf3ea300fdc4a070fe304eac2f40fe1642f549a23ea55ccb38a6e092a2"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/278/files
Content-Type: application/json
Authorization: Bearer 4b9a864c8bdec0c6d02211c5a6ddca2f6fbda958a31760cb83d87f179c1637f5
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
    "id": 11,
    "uploader": {
      "id": 858,
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
      "created_at": "2016-10-11T17:00:29.486Z",
      "updated_at": "2016-10-11T17:00:29.486Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-11T17:00:29.516Z",
    "updated_at": "2016-10-11T17:00:29.516Z",
    "course_id": 278,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/278/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b9a864c8bdec0c6d02211c5a6ddca2f6fbda958a31760cb83d87f179c1637f5"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/277/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 7f7af92b2230eef58d582be8e9b1f90e88d449232cd0b2faac00432e1202f89f
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
    "key": "cache/ade6fd5ea55c99e793d1cf3b4094ed6d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xMVQxODowMDoyOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9hZGU2ZmQ1ZWE1NWM5OWU3OTNkMWNmM2I0MDk0ZWQ2ZC5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTFUMTcwMDI5WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161011/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161011T170029Z",
    "x-amz-signature": "afe65373a35603c770f1b075bc880f80d2b53779da7deca1dbbd19fe85b85017"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/277/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f7af92b2230eef58d582be8e9b1f90e88d449232cd0b2faac00432e1202f89f"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 912883958af2c3d5e663543d580f97c791acaf7b10f65b8c90cb0becc0067edd
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
	-H "Authorization: Bearer 912883958af2c3d5e663543d580f97c791acaf7b10f65b8c90cb0becc0067edd"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f5d3e3814bce004126a0e7161398cac7fb46c3ef438d364f97ef7a7774ee3582
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
	-H "Authorization: Bearer f5d3e3814bce004126a0e7161398cac7fb46c3ef438d364f97ef7a7774ee3582"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f2ae820e0956adbdc21772ea7873fc95504dc2b6b04e251bd7e56964ee3bb21a
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
	-H "Authorization: Bearer f2ae820e0956adbdc21772ea7873fc95504dc2b6b04e251bd7e56964ee3bb21a"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0ec26cc400fbd5b5ddc1f4511a8bedd31040f129e2bb7e3b411b001eb136d4dd
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
	-H "Authorization: Bearer 0ec26cc400fbd5b5ddc1f4511a8bedd31040f129e2bb7e3b411b001eb136d4dd"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5eb69b8903d142c8f20d8a06a1ef5be27cd5a10dac8960470285cc30038c61a4
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
	-H "Authorization: Bearer 5eb69b8903d142c8f20d8a06a1ef5be27cd5a10dac8960470285cc30038c61a4"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 0a18cff4c48745e7aec4e8b195442597d3510797997d133c924213d4379530aa
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
    "creator_id": 9,
    "id": 3,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 3,
    "additional_university_ids": [

    ],
    "topic_id": 5,
    "discipline_id": 6,
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
    "chapters_updated_at": "2016-10-11T16:59:15.932Z",
    "updated_at": "2016-10-11T16:59:17.417Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 3,
        "title": "Clever Chapter Title 3",
        "position": 1,
        "updated_at": "2016-10-11T16:59:17.368Z",
        "course_id": 3,
        "author_id": 9,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-11T16:59:15.932Z",
        "questions_updated_at": "2016-10-11T16:59:15.932Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 4,
        "title": "Clever Chapter Title 4",
        "position": 2,
        "updated_at": "2016-10-11T16:59:17.409Z",
        "course_id": 3,
        "author_id": 9,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-11T16:59:15.932Z",
        "questions_updated_at": "2016-10-11T16:59:15.932Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 10,
        "chapter_id": 3,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:17.200Z",
        "created_at": "2016-10-11T16:59:17.200Z",
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
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 10,
        "chapter_id": 4,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:17.277Z",
        "created_at": "2016-10-11T16:59:17.277Z",
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
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 10,
        "chapter_id": 3,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:17.243Z",
        "created_at": "2016-10-11T16:59:17.243Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 10,
        "chapter_id": 4,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:17.318Z",
        "created_at": "2016-10-11T16:59:17.318Z",
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
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 10,
        "chapter_id": 3,
        "position": 7,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:16.161Z",
        "created_at": "2016-10-11T16:59:16.038Z",
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
          }
        ]
      },
      {
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 10,
        "chapter_id": 3,
        "position": 8,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:16.338Z",
        "created_at": "2016-10-11T16:59:16.226Z",
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
          }
        ]
      },
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 10,
        "chapter_id": 4,
        "position": 9,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:16.545Z",
        "created_at": "2016-10-11T16:59:16.423Z",
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
        "author_id": 10,
        "chapter_id": 4,
        "position": 10,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:16.730Z",
        "created_at": "2016-10-11T16:59:16.613Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a18cff4c48745e7aec4e8b195442597d3510797997d133c924213d4379530aa"
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
    "creator_id": 15,
    "id": 4,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 4,
    "additional_university_ids": [

    ],
    "topic_id": 6,
    "discipline_id": 7,
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
    "chapters_updated_at": "2016-10-11T16:59:17.553Z",
    "updated_at": "2016-10-11T16:59:19.076Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 5,
        "title": "Clever Chapter Title 5",
        "position": 1,
        "updated_at": "2016-10-11T16:59:19.024Z",
        "course_id": 4,
        "author_id": 15,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-11T16:59:17.553Z",
        "questions_updated_at": "2016-10-11T16:59:17.553Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 6,
        "title": "Clever Chapter Title 6",
        "position": 2,
        "updated_at": "2016-10-11T16:59:19.069Z",
        "course_id": 4,
        "author_id": 15,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-11T16:59:17.553Z",
        "questions_updated_at": "2016-10-11T16:59:17.553Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 15,
        "chapter_id": 5,
        "position": 13,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:17.773Z",
        "created_at": "2016-10-11T16:59:17.648Z",
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
      },
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 15,
        "chapter_id": 6,
        "position": 15,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-11T16:59:18.176Z",
        "created_at": "2016-10-11T16:59:18.044Z",
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
PUT /v2/courses/6/pin
Content-Type: application/json
Authorization: Bearer bcfebbb127e3182445a52a6b8dc603d175bb6784abdd6f1a66d36db1b4fbcab1
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/6/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcfebbb127e3182445a52a6b8dc603d175bb6784abdd6f1a66d36db1b4fbcab1"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/1/pin
Content-Type: application/json
Authorization: Bearer 15b8afebffa875f60f4db3a73ee030452557ce78499142742f80879da024ef0a
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
	-H "Authorization: Bearer 15b8afebffa875f60f4db3a73ee030452557ce78499142742f80879da024ef0a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b1bcf33b48c40b051cfc749402971f68953a93fe4bf98029cf44b3f896dbcfd9
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
    "creator_id": 28,
    "id": 7,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 7,
    "additional_university_ids": [

    ],
    "topic_id": 9,
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
    "updated_at": "2016-10-11T16:59:21.014Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1bcf33b48c40b051cfc749402971f68953a93fe4bf98029cf44b3f896dbcfd9"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1216955827eccab7c945eca0cb265135bbb0d05556e2bbf35caf45b94b6bb63f
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
    "id": 708,
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
    "created_at": "2016-10-11T17:00:15.144Z",
    "updated_at": "2016-10-11T17:00:15.144Z",
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
	-H "Authorization: Bearer 1216955827eccab7c945eca0cb265135bbb0d05556e2bbf35caf45b94b6bb63f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 672c1179eb40606b05caa4f578f777ad358b451c759b30858b366d91d4b45704
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[216]}
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
    "id": 703,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      216
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-11T17:00:14.484Z",
    "updated_at": "2016-10-11T17:00:14.536Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[216]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 672c1179eb40606b05caa4f578f777ad358b451c759b30858b366d91d4b45704"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 57f0f2354e7f95a9a381aea521072d93eae64e1fd98bb6d4a194a73029d92d04
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
    "id": 705,
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
    "created_at": "2016-10-11T17:00:14.648Z",
    "updated_at": "2016-10-11T17:00:14.648Z",
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
	-H "Authorization: Bearer 57f0f2354e7f95a9a381aea521072d93eae64e1fd98bb6d4a194a73029d92d04"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 794400a9f37a890ec76b5958de623c1147ef0a07b98adc072a3766555b7faa92
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[219]}
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
    "id": 706,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      219
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-11T17:00:14.751Z",
    "updated_at": "2016-10-11T17:00:14.751Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[219]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 794400a9f37a890ec76b5958de623c1147ef0a07b98adc072a3766555b7faa92"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 084c756160dc9607a932b1dc2852acc81fd9de370ed1ad81f608cdd4a369cce1
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

220
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
    "id": 707,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/fe9872866e007f7f543e50884e01f0a47b960f1c.jpg",
    "university_id": null,
    "fields_of_study": [
      220
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-11T17:00:14.827Z",
    "updated_at": "2016-10-11T17:00:15.113Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/92f456f1f1a56f6575207cf315c3515bbb29c63a.jpg",
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

220
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 084c756160dc9607a932b1dc2852acc81fd9de370ed1ad81f608cdd4a369cce1"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer a30cf8412cadcf8b53b0dc51cf5899a39e5e85893c1a0b90492cd1defb781809
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
      "bookmarkable_id": 95,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 96,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 97,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a30cf8412cadcf8b53b0dc51cf5899a39e5e85893c1a0b90492cd1defb781809"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8c15e00022ed9c54bccc37d4b77ccb33d1a91a8b2352bcc4e3121e9128a4b9bf
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
      "company_id": 29,
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
      "company_id": 30,
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
	-H "Authorization: Bearer 8c15e00022ed9c54bccc37d4b77ccb33d1a91a8b2352bcc4e3121e9128a4b9bf"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 7bbfef850c1eda0dc723f60792cb267611c4f2af42f601159ae1e90ea95e1a29
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
      "company_id": 25,
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
	-H "Authorization: Bearer 7bbfef850c1eda0dc723f60792cb267611c4f2af42f601159ae1e90ea95e1a29"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 6f3d4622f12dab8f89957b46480967d3fcd40c66187f3702be7c44d2ad487489
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
      "creator_id": 443,
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-103",
      "html_url": "https://goskive.com/course/mit-course-103",
      "slug": "mit-course-103",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 130,
      "discipline_id": 131,
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
      "updated_at": "2016-10-11T16:59:57.423Z",
      "shortname": "mit-course-103"
    },
    {
      "creator_id": 444,
      "id": 129,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-104",
      "html_url": "https://goskive.com/course/mit-course-104",
      "slug": "mit-course-104",
      "university_id": 134,
      "additional_university_ids": [

      ],
      "topic_id": 131,
      "discipline_id": 132,
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
      "updated_at": "2016-10-11T16:59:57.540Z",
      "shortname": "mit-course-104"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f3d4622f12dab8f89957b46480967d3fcd40c66187f3702be7c44d2ad487489"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer b10dcf6358172607706748ae1f45e97c9470bff722dc56224bf7341af259e087
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
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-11T17:00:03.161Z"
      },
      "created_at": "2016-10-11T17:00:03.164Z",
      "updated_at": "2016-10-11T17:00:03.164Z",
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
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-11T17:00:03.173Z"
      },
      "created_at": "2016-10-11T17:00:03.176Z",
      "updated_at": "2016-10-11T17:00:03.176Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b10dcf6358172607706748ae1f45e97c9470bff722dc56224bf7341af259e087"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8069df51669ef5de9952205dd6bc816511e4512e8dcc12768633ffa13992bd7c
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
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-11T17:00:02.932Z"
      },
      "created_at": "2016-10-11T17:00:02.935Z",
      "updated_at": "2016-10-11T17:00:02.935Z",
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
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-11T17:00:02.951Z"
      },
      "created_at": "2016-10-11T17:00:02.954Z",
      "updated_at": "2016-10-11T17:00:02.954Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8069df51669ef5de9952205dd6bc816511e4512e8dcc12768633ffa13992bd7c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer b6091416fd64c2f53603202f6c4b1f4eb28fbcaf20f4b5aefb11a1a6f66a8f0a
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
      "id": 5,
      "created_at": "2016-10-11T16:59:35.587Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 1,
      "updated_at": "2016-10-11T16:59:35.709Z",
      "author_id": "196",
      "thread_subject_id": "62",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 6,
      "created_at": "2016-10-11T16:59:35.695Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-11T16:59:35.713Z",
      "author_id": "199",
      "thread_subject_id": "63",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-11T16:59:36.153Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 10,
      "updated_at": "2016-10-11T16:59:36.153Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-10-11T16:59:36.590Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-10-11T16:59:36.590Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 9,
      "created_at": "2016-10-11T16:59:37.038Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-11T16:59:37.038Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 10,
      "created_at": "2016-10-11T16:59:37.404Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 36,
      "updated_at": "2016-10-11T16:59:37.404Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-11T16:59:37.751Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 37,
      "updated_at": "2016-10-11T16:59:37.751Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-10-11T16:59:38.092Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 38,
      "updated_at": "2016-10-11T16:59:38.092Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6091416fd64c2f53603202f6c4b1f4eb28fbcaf20f4b5aefb11a1a6f66a8f0a"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/13
Content-Type: application/json
Authorization: Bearer 1bf53e1a2d91b748e2dda291e2b3e68b0ea4cd3cf9135e137efe084ef59764cb
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-11T16:49:38.000Z"}}
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
    "id": 13,
    "created_at": "2016-10-11T16:59:38.310Z",
    "read_at": "2016-10-11T16:49:38.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 3,
    "updated_at": "2016-10-11T16:59:38.353Z",
    "author_id": "225",
    "thread_subject_id": "70",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/13" -d '{"notification":{"read_at":"2016-10-11T16:49:38.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bf53e1a2d91b748e2dda291e2b3e68b0ea4cd3cf9135e137efe084ef59764cb"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9da687cac08d14ce61b1ed0b71ecc4b4b188590fb728eb3dca0dbe29ffc0178b
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
      "course_id": 259,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-11T17:00:24.564Z",
      "course_published": true,
      "updated_at": "2016-10-11T17:00:24.555Z"
    },
    {
      "id": 5,
      "course_id": 260,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-11T17:00:24.660Z",
      "course_published": true,
      "updated_at": "2016-10-11T17:00:24.652Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9da687cac08d14ce61b1ed0b71ecc4b4b188590fb728eb3dca0dbe29ffc0178b"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 059239d70bfde628f33828383e88a25a570ee1f158e7f36d4f23d9df4717e8ec
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
    "id": 6,
    "course_id": 261,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-11T17:00:24.791Z",
    "course_published": true,
    "updated_at": "2016-10-11T17:00:24.783Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 059239d70bfde628f33828383e88a25a570ee1f158e7f36d4f23d9df4717e8ec"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 49608df306eb3e3f99adc10cf40279b691c3d08c10b7fb6913baeae6716ed025
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
    "course_id": 262,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-11T17:00:24.981Z",
    "course_published": true,
    "updated_at": "2016-10-11T17:00:24.969Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49608df306eb3e3f99adc10cf40279b691c3d08c10b7fb6913baeae6716ed025"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer b9123982defd4d343caeaac01d1d202927c2b5f90773d3c0fe84a8284d6c9889
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
      "votable_id": 109,
      "user_id": 779
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 110,
      "user_id": 779
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 111,
      "user_id": 779
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 112,
      "user_id": 779
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9123982defd4d343caeaac01d1d202927c2b5f90773d3c0fe84a8284d6c9889"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/1
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
    "id": 1,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 1,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 1
      },
      {
        "id": 2,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 1
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/1" -X GET \
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
      "id": 2,
      "name": "Face to face executive extranet",
      "name_translations": {
        "en": "Face to face executive extranet"
      }
    },
    {
      "id": 3,
      "name": "Seamless attitude-oriented infrastructure",
      "name_translations": {
        "en": "Seamless attitude-oriented infrastructure"
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
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer 616829bcd8f83b1d304c16f8fe809a811932cab14438f0b80a718f49bd3efa2a
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
    "id": 20,
    "user_id": 562,
    "feedbackable_id": 69,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-11T17:00:04.049Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 616829bcd8f83b1d304c16f8fe809a811932cab14438f0b80a718f49bd3efa2a"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer 36b5b9a4b54b6834bbaed36e2787beb50894a5bb1d27a44786f2deab797a269c
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
    "user_id": 577,
    "feedbackable_id": 72,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-11T17:00:04.850Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36b5b9a4b54b6834bbaed36e2787beb50894a5bb1d27a44786f2deab797a269c"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/25
Content-Type: application/json
Authorization: Bearer fd1d86b6816eba82e27d2e684a763dac88363b1b4728b7c8c0e7eb1ef514941f
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
    "id": 25,
    "user_id": 587,
    "feedbackable_id": 74,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-11T17:00:05.786Z",
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
curl "api.goskive.com/v2/feedbacks/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd1d86b6816eba82e27d2e684a763dac88363b1b4728b7c8c0e7eb1ef514941f"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/18/close
Content-Type: application/json
Authorization: Bearer 0ac97faa1289916be1e2b912b63de1dac9f42844a531d78c8270390a8b0cc2fe
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
curl "api.goskive.com/v2/feedbacks/18/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ac97faa1289916be1e2b912b63de1dac9f42844a531d78c8270390a8b0cc2fe"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer c1867d8cfd4d0a3962bcb1d62e6771cf7c41727ae3825bf8f343abd150318421
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
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1867d8cfd4d0a3962bcb1d62e6771cf7c41727ae3825bf8f343abd150318421"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer f7907cd419f86ccab0c801cffffe04284ae8a79ee28992298d1b377912b094b2
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
curl "api.goskive.com/v2/feedbacks/22/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7907cd419f86ccab0c801cffffe04284ae8a79ee28992298d1b377912b094b2"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/26
Content-Type: application/json
Authorization: Bearer 491e3c3e44bf4cd7c17a1ee1a0339fbdbb0339dca41a87309c62d42572ba79af
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
    "id": 26,
    "user_id": 592,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-11T17:00:06.092Z",
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
curl "api.goskive.com/v2/feedbacks/26" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 491e3c3e44bf4cd7c17a1ee1a0339fbdbb0339dca41a87309c62d42572ba79af"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/2
Authorization: Bearer 98f29fb829e0eb097f76702ac967f765bcb4a681ecdc5406ed125bdf84a3b84c
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
curl "api.goskive.com/v2/files/2" -d '' -X DELETE \
	-H "Authorization: Bearer 98f29fb829e0eb097f76702ac967f765bcb4a681ecdc5406ed125bdf84a3b84c" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/3
Authorization: Bearer 4f51c621e6aad73d124fd79a8e515305c5f4321453df5a605bf1c8147332ebbe
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
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Authorization: Bearer 4f51c621e6aad73d124fd79a8e515305c5f4321453df5a605bf1c8147332ebbe" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/5
Authorization: Bearer 27e83bd9b3c601673f464a96c992b74385449199c3fbe297c0310742c7277ce6
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/9e6783610e3ab05c0f5434faf9f9c87e.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161011%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161011T165935Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=d85d748bdc2f73f4ac3770b1fddde9e97285437548e0fa5893b9c77db87276f3"
  }
}
```



```shell
curl "api.goskive.com/v2/files/5" -X GET \
	-H "Authorization: Bearer 27e83bd9b3c601673f464a96c992b74385449199c3fbe297c0310742c7277ce6"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer 8f32468b8d71af234a320f28e3544c6e79e58bf8133107400bff0e29ea32b4e6
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
      "id": 191,
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
      "created_at": "2016-10-11T16:59:35.293Z",
      "updated_at": "2016-10-11T16:59:35.293Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-11T16:59:35.375Z",
    "updated_at": "2016-10-11T16:59:35.375Z",
    "course_id": 61,
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
	-H "Authorization: Bearer 8f32468b8d71af234a320f28e3544c6e79e58bf8133107400bff0e29ea32b4e6" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/13/matched_courses
Authorization: Bearer 149a78235193947f22bd2b723490237bc04abbeaea1775d3de7fb6f533cc1de6
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
      "creator_id": 935,
      "id": 300,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 285,
      "additional_university_ids": [

      ],
      "topic_id": 312,
      "discipline_id": 313,
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
      "chapters_updated_at": "2016-10-11T17:00:33.457Z",
      "updated_at": "2016-10-11T17:00:35.153Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 940,
      "id": 301,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-7f7af7fd-a3ba-479a-9c38-67b820a039c2",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-7f7af7fd-a3ba-479a-9c38-67b820a039c2",
      "slug": "mit-the-great-british-bake-off-7f7af7fd-a3ba-479a-9c38-67b820a039c2",
      "university_id": 286,
      "additional_university_ids": [

      ],
      "topic_id": 313,
      "discipline_id": 314,
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
      "chapters_updated_at": "2016-10-11T17:00:33.457Z",
      "updated_at": "2016-10-11T17:00:35.740Z",
      "shortname": "mit-the-great-british-bake-off-7f7af7fd-a3ba-479a-9c38-67b820a039c2"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/13/matched_courses" -X GET \
	-H "Authorization: Bearer 149a78235193947f22bd2b723490237bc04abbeaea1775d3de7fb6f533cc1de6"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/6/preview
Authorization: Bearer fdbb3aa46018fdcdb7879854034430c96fb8e461d782118c3b3782fdc05f51ce
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/db83bb29b9237c7c0496b80e6e7d9810.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161011%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161011T165935Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=155d2eb3a574a4be5a50d00fc21fe4dee0cdcd157bd7cbebbfef619946365e21"
  }
}
```



```shell
curl "api.goskive.com/v2/files/6/preview" -X GET \
	-H "Authorization: Bearer fdbb3aa46018fdcdb7879854034430c96fb8e461d782118c3b3782fdc05f51ce"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/1/report
Authorization: Bearer 0e8d6ed1968e6a27967a648e9f52ec834a17a405968def2a852134a5b3ff60d9
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
curl "api.goskive.com/v2/files/1/report" -d '' -X PUT \
	-H "Authorization: Bearer 0e8d6ed1968e6a27967a648e9f52ec834a17a405968def2a852134a5b3ff60d9" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/54/comments
Content-Type: application/json
Authorization: Bearer 8f7794dcbbad4a5dd584c3ca788cb5d7ae70af1a952263bedff3854b56aa2baf
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
    "id": 7,
    "author_id": 242,
    "reply_to_id": null,
    "created_at": "2016-10-11T16:59:39.905Z",
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
curl "api.goskive.com/v2/flashcards/54/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f7794dcbbad4a5dd584c3ca788cb5d7ae70af1a952263bedff3854b56aa2baf"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/53/comments
Content-Type: application/json
Authorization: Bearer a8d8c8aeb92f1238eff62b182ad73084d866d63a0d51ade3548944be90bf93b3
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
    "id": 6,
    "author_id": 239,
    "reply_to_id": null,
    "created_at": "2016-10-11T16:59:39.536Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 239,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:39.531Z",
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
curl "api.goskive.com/v2/flashcards/53/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8d8c8aeb92f1238eff62b182ad73084d866d63a0d51ade3548944be90bf93b3"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/52/comments
Content-Type: application/json
Authorization: Bearer 87bdaed5c4c3bb44a06b6254d233d615c9a80aa963f766d2f5664aaf731e395f
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
      "id": 4,
      "author_id": 237,
      "reply_to_id": null,
      "created_at": "2016-10-11T16:59:39.274Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 238,
      "reply_to_id": null,
      "created_at": "2016-10-11T16:59:39.291Z",
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
curl "api.goskive.com/v2/flashcards/52/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87bdaed5c4c3bb44a06b6254d233d615c9a80aa963f766d2f5664aaf731e395f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer 26419fd2ba1f35c11a5ebc18cc5548ac990acce2afbbee5c04f9e69fc7477040
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
curl "api.goskive.com/v2/flashcards/55/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26419fd2ba1f35c11a5ebc18cc5548ac990acce2afbbee5c04f9e69fc7477040"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/56/feedbacks
Content-Type: application/json
Authorization: Bearer 86989a71e6068005eb9ac3885755931c4de9617039b3d433d8e050468dbc7267
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
    "id": 10,
    "user_id": 284,
    "feedbackable_id": 56,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-11T16:59:43.824Z",
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
curl "api.goskive.com/v2/flashcards/56/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86989a71e6068005eb9ac3885755931c4de9617039b3d433d8e050468dbc7267"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/60/feedbacks
Content-Type: application/json
Authorization: Bearer 997a8efb031e5b5e7125bddc372b9a267d7a395e8c9af1a5148f5fb25708b69d
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
      "id": 15,
      "user_id": 308,
      "feedbackable_id": 60,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:44.942Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 307,
      "feedbackable_id": 60,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:44.930Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/60/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 997a8efb031e5b5e7125bddc372b9a267d7a395e8c9af1a5148f5fb25708b69d"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/66/votes
Content-Type: application/json
Authorization: Bearer a3366cbe768b71c43de25d392a9619423e91b23780abbc1d1de883cf6ea8a5ce
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
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 66,
      "user_id": 441
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 66,
      "user_id": 440
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 66,
      "user_id": 439
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/66/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3366cbe768b71c43de25d392a9619423e91b23780abbc1d1de883cf6ea8a5ce"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/27/republish
Content-Type: application/json
Authorization: Bearer 561075407bd63b53bcf21ba1c96fcf4a44367931b59ca911c2003a3f71d0a127
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
curl "api.goskive.com/v2/flashcards/27/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 561075407bd63b53bcf21ba1c96fcf4a44367931b59ca911c2003a3f71d0a127"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/47/bookmark
Content-Type: application/json
Authorization: Bearer aec584c3524a2f1851dff10834b421a33047a4fbb02081e2ffd1ad2a9be10dcf
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/47/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aec584c3524a2f1851dff10834b421a33047a4fbb02081e2ffd1ad2a9be10dcf"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/44
Content-Type: application/json
Authorization: Bearer 2d3e722f63824e2534187d6e2bfd680be8b3b4a0a9a2ecb97a60e222474ad4db
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d3e722f63824e2534187d6e2bfd680be8b3b4a0a9a2ecb97a60e222474ad4db"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/48/downvote
Content-Type: application/json
Authorization: Bearer de8afb59b7bd6902e3d829ce9d39867fe83dd7af1a086082e71d87bf5c3472bb
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/48/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de8afb59b7bd6902e3d829ce9d39867fe83dd7af1a086082e71d87bf5c3472bb"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/46
Content-Type: application/json
Authorization: Bearer 9856f5eb8f81755a5bfe924101384d38f67bbccbab3dd8bc08c6dbc63b1fdb28
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
    "id": 46,
    "obfuscated_id": "urkHiAaH08E",
    "author_id": 137,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T16:59:30.654Z",
    "created_at": "2016-10-11T16:59:30.654Z",
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
curl "api.goskive.com/v2/flashcards/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9856f5eb8f81755a5bfe924101384d38f67bbccbab3dd8bc08c6dbc63b1fdb28"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/49/report
Content-Type: application/json
Authorization: Bearer 6401d5818e7e8bffa73166420744a3608c35e80c330e6b6681b346892ed97db3
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6401d5818e7e8bffa73166420744a3608c35e80c330e6b6681b346892ed97db3"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50/bookmark
Content-Type: application/json
Authorization: Bearer 88b5973c30def45209dcad351b0e66459bf2abe2b9f73d07a7e509b1f8057a34
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
	-H "Authorization: Bearer 88b5973c30def45209dcad351b0e66459bf2abe2b9f73d07a7e509b1f8057a34"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/45/upvote
Content-Type: application/json
Authorization: Bearer ae061c78ec3d9c4b07b18950687230bd7e7213deb87ae6f2a3a01940f5aeb466
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/45/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae061c78ec3d9c4b07b18950687230bd7e7213deb87ae6f2a3a01940f5aeb466"
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
    "key": "cache/78598bae82a8c20cb19766661bc64412.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xMVQxNzo1OToyN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS83ODU5OGJhZTgyYThjMjBjYjE5NzY2NjYxYmM2NDQxMi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTFUMTY1OTI3WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161011/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161011T165927Z",
    "x-amz-signature": "97ecca622f0961d9774313b0c95feea1a8d0de58220ebe0babe6810e91f21145"
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
Authorization: Bearer b5ceb2ce7c503412ab6ec8026f93fda9f419829320f0b1095a87355161458f4c
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
	-H "Authorization: Bearer b5ceb2ce7c503412ab6ec8026f93fda9f419829320f0b1095a87355161458f4c"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 833e237f81173500e7408a89caa640e95e3c681a4f9f806f6af3cff49c2edba7
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
	-H "Authorization: Bearer 833e237f81173500e7408a89caa640e95e3c681a4f9f806f6af3cff49c2edba7"
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
{"password":{"reset_password_token":"_4gnxEiXxGAidXrLgTbK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 73,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-11T16:59:26.994Z",
  "updated_at": "2016-10-11T16:59:27.136Z",
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
  "audit_id": 3042
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"_4gnxEiXxGAidXrLgTbK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/132/comments
Content-Type: application/json
Authorization: Bearer 95c9c2997cc61052de61a924da6825cb0be13f42ae7d1b3885b027fd238508be
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
    "author_id": 954,
    "reply_to_id": null,
    "created_at": "2016-10-11T17:00:37.079Z",
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
curl "api.goskive.com/v2/questions/132/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95c9c2997cc61052de61a924da6825cb0be13f42ae7d1b3885b027fd238508be"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/131/comments
Content-Type: application/json
Authorization: Bearer 2024acbef463e743eccd7fb7cf4ac9d83e7d5116139e339453b813afdf154cd3
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
    "author_id": 951,
    "reply_to_id": null,
    "created_at": "2016-10-11T17:00:36.596Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 951,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T17:00:36.593Z",
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
curl "api.goskive.com/v2/questions/131/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2024acbef463e743eccd7fb7cf4ac9d83e7d5116139e339453b813afdf154cd3"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/133/comments
Content-Type: application/json
Authorization: Bearer 69c2eaff80b98e7196b51464b110b116a759ec3826d5e5f7fb3b9e24e4f8d902
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
      "author_id": 961,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:37.552Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 960,
      "reply_to_id": null,
      "created_at": "2016-10-11T17:00:37.534Z",
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
curl "api.goskive.com/v2/questions/133/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69c2eaff80b98e7196b51464b110b116a759ec3826d5e5f7fb3b9e24e4f8d902"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/130/comments
Content-Type: application/json
Authorization: Bearer 8ffd41a198d120a57a837bf8886fc3dbe01cbf072918a385676ec186d0b485aa
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
curl "api.goskive.com/v2/questions/130/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ffd41a198d120a57a837bf8886fc3dbe01cbf072918a385676ec186d0b485aa"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/39/feedbacks
Content-Type: application/json
Authorization: Bearer 570341402d4ff9dbcf9459e556aca86f4bb9b836d06b044edaabdbdde4b5fa15
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
    "id": 2,
    "user_id": 248,
    "feedbackable_id": 39,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-11T16:59:40.671Z",
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
curl "api.goskive.com/v2/questions/39/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 570341402d4ff9dbcf9459e556aca86f4bb9b836d06b044edaabdbdde4b5fa15"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/43/feedbacks
Content-Type: application/json
Authorization: Bearer 274253cf93e4ef5b7255e1bba7f22674c1196edb87fb81c12bb29e6b48f90edc
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
      "id": 7,
      "user_id": 272,
      "feedbackable_id": 43,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:42.610Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 271,
      "feedbackable_id": 43,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-11T16:59:42.597Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/43/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 274253cf93e4ef5b7255e1bba7f22674c1196edb87fb81c12bb29e6b48f90edc"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/28/votes
Content-Type: application/json
Authorization: Bearer 49a41759af4e0ec61500eff54f52eefdfd9a31f878d4830a7dea7e69261022f7
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
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 63
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 62
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 61
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/28/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49a41759af4e0ec61500eff54f52eefdfd9a31f878d4830a7dea7e69261022f7"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/69/republish
Content-Type: application/json
Authorization: Bearer fa2bf17f7225e16aca44955b8113f5097893e93b9af162a911219782cf1ced8b
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
curl "api.goskive.com/v2/questions/69/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa2bf17f7225e16aca44955b8113f5097893e93b9af162a911219782cf1ced8b"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/66/bookmark
Content-Type: application/json
Authorization: Bearer 16814d9a255e193b13199501d173a90fc5fd8b16f35e19a1e91e832db8633028
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/66/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16814d9a255e193b13199501d173a90fc5fd8b16f35e19a1e91e832db8633028"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/65
Content-Type: application/json
Authorization: Bearer 7cbf581ce535d7ccf25c02b3d5cc59f44eef626a4702be76e94f3cb69422225c
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cbf581ce535d7ccf25c02b3d5cc59f44eef626a4702be76e94f3cb69422225c"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/67/downvote
Content-Type: application/json
Authorization: Bearer cbfb2e979f86b29ef64ef9e490bf6e15e909f809227e0e65cef52838d9f543b0
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/67/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbfb2e979f86b29ef64ef9e490bf6e15e909f809227e0e65cef52838d9f543b0"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/71
Content-Type: application/json
Authorization: Bearer 53b367c2b7482a0ced93f4c29e70fee8de3dff4931d7876cafd29c9d2178779d
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
    "id": 71,
    "obfuscated_id": "--JhLc6KEBw",
    "author_id": 397,
    "chapter_id": 94,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T16:59:54.324Z",
    "created_at": "2016-10-11T16:59:54.205Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 142,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 143,
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
curl "api.goskive.com/v2/questions/71" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53b367c2b7482a0ced93f4c29e70fee8de3dff4931d7876cafd29c9d2178779d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/47/report
Content-Type: application/json
Authorization: Bearer 4d082257d939fe8553e5d46ef11b703bfe9f6582ce85d8ec149f16157cb0a14a
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/47/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d082257d939fe8553e5d46ef11b703bfe9f6582ce85d8ec149f16157cb0a14a"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/49/bookmark
Content-Type: application/json
Authorization: Bearer 12ccdea76d638da9bc99745f6f503ca38195e8bb73c9ae73a0a069697af9c65f
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
	-H "Authorization: Bearer 12ccdea76d638da9bc99745f6f503ca38195e8bb73c9ae73a0a069697af9c65f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/68
Content-Type: application/json
Authorization: Bearer be52a29c6281a6b9cb51af4ea41c93ea3f4a80d801fbf9960892004a504e26a9
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":68,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-11T16:59:52.956Z","updated_at":"2016-10-11T16:59:53.073Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":91,"author_id":388,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 388,
    "chapter_id": 91,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-11T16:59:53.186Z",
    "created_at": "2016-10-11T16:59:52.956Z",
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
    "question": "{\"id\"=>68, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-11T16:59:52.956Z\", \"updated_at\"=>\"2016-10-11T16:59:53.073Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>91, \"author_id\"=>388, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 137,
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
curl "api.goskive.com/v2/questions/68" -d '{"question":{"question":{"id":68,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-11T16:59:52.956Z","updated_at":"2016-10-11T16:59:53.073Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":91,"author_id":388,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be52a29c6281a6b9cb51af4ea41c93ea3f4a80d801fbf9960892004a504e26a9"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/48/upvote
Content-Type: application/json
Authorization: Bearer 209a04cfb282b0a0001fb723d6264f0891ddde95b3c5045bf0b29a37b8bea3f6
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 209a04cfb282b0a0001fb723d6264f0891ddde95b3c5045bf0b29a37b8bea3f6"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer dc271b7a39e9a58aeea11765a44c7217223aadf68bb0c104cefd5d99e9cccd20
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
      "creator_id": 701,
      "id": 206,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 214,
      "additional_university_ids": [

      ],
      "topic_id": 213,
      "discipline_id": 214,
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
      "updated_at": "2016-10-11T17:00:14.291Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc271b7a39e9a58aeea11765a44c7217223aadf68bb0c104cefd5d99e9cccd20"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 6c2c0129c1b6030fa252ccd30383946454bbe5610a636799805797b1b3db5cbc
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
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-210",
      "html_url": "https://goskive.com/university/uni-210",
      "slug": "uni-210",
      "name": "National School of Pizza",
      "short_name": "Uni 210",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/00a31358daafcf5bb69c7f7fe9a4f7834d0b34e1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2cad3d6b785347184fb4aaf7589f7acdba85adc7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-11T17:00:14.062Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-209",
      "html_url": "https://goskive.com/university/uni-209",
      "slug": "uni-209",
      "name": "National School of Pastry",
      "short_name": "Uni 209",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d1110a973573c8974a39e5f6375fbdb606ee1c84.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ff09bc3bf3d009bff704e63ea3ef6b24839d4267.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-11T17:00:14.046Z",
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
	-H "Authorization: Bearer 6c2c0129c1b6030fa252ccd30383946454bbe5610a636799805797b1b3db5cbc"
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
      "id": 176,
      "name": "Digitized transitional initiative",
      "name_translations": {
        "en": "Digitized transitional initiative"
      },
      "discipline_id": 177
    },
    {
      "id": 177,
      "name": "Streamlined analyzing info-mediaries",
      "name_translations": {
        "en": "Streamlined analyzing info-mediaries"
      },
      "discipline_id": 178
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
GET /v2/topics/178
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
    "id": 178,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 179
  }
}
```



```shell
curl "api.goskive.com/v2/topics/178" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 21385e65173462f131afdd4b7065f604391db9e6263ad7530fb7f24c2b8d9845
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
      "id": 117,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-117",
      "html_url": "https://goskive.com/university/uni-117",
      "slug": "uni-117",
      "name": "University 98",
      "short_name": "Uni 117",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2b6739d4bdec870260d7525d9d3791a7fbf79818.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f83d0662811dd3779b84a2d425f643ab027f38a0.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-11T16:59:54.515Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-118",
      "html_url": "https://goskive.com/university/uni-118",
      "slug": "uni-118",
      "name": "University 99",
      "short_name": "Uni 118",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/10c45072caa721987b05dfcb635cef9f53e6bb5b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/abe07e3df800339993de4e0db7bdc7e30ac9c4ff.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-11T16:59:54.532Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-119",
      "html_url": "https://goskive.com/university/uni-119",
      "slug": "uni-119",
      "name": "University 100",
      "short_name": "Uni 119",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/18b3243e0496f81e57c0841ffc50d1ffea7771fc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8235339619085a5aaf31c8771d17b1288f8e8a68.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-11T16:59:54.548Z",
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
	-H "Authorization: Bearer 21385e65173462f131afdd4b7065f604391db9e6263ad7530fb7f24c2b8d9845"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 79f42c8da000a6ec9fe56293b21582a3b5e1f23dfb67079585e0f120c18135b3
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
    "id": 120,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b5c059d79ca15ef51a64141885c41356b7eb6d7f.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2ad2f4c4aa6e2cd2c784d7880241d6c1b55f4863.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-11T16:59:54.611Z",
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
	-H "Authorization: Bearer 79f42c8da000a6ec9fe56293b21582a3b5e1f23dfb67079585e0f120c18135b3"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 407ec8a3997637e7a86bdc8f55707d65e68777ac4a34af9d8e11dc478b387047
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":258,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 751,
    "id": 246,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 231,
    "additional_university_ids": [

    ],
    "topic_id": 258,
    "discipline_id": 259,
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
    "chapters_updated_at": "2016-10-11T17:00:19.223Z",
    "updated_at": "2016-10-11T17:00:19.368Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 137,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-11T17:00:19.319Z",
        "course_id": 246,
        "author_id": 751,
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
        "id": 138,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-11T17:00:19.338Z",
        "course_id": 246,
        "author_id": 751,
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
        "id": 139,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-11T17:00:19.357Z",
        "course_id": 246,
        "author_id": 751,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":258,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 407ec8a3997637e7a86bdc8f55707d65e68777ac4a34af9d8e11dc478b387047"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b9df63105b66e9908cff7b714d839a8ef5b42a8cd05bb649b2a1ae9318f1e119
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":259,"published":false}}
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
    "creator_id": 752,
    "id": 247,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 232,
    "additional_university_ids": [

    ],
    "topic_id": 259,
    "discipline_id": 260,
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
    "updated_at": "2016-10-11T17:00:19.558Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":259,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9df63105b66e9908cff7b714d839a8ef5b42a8cd05bb649b2a1ae9318f1e119"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 26b1783524e088480b637eca10218ea1fddd2eafb2938ba8aadf9fe8c8a76f09
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
      "creator_id": 714,
      "id": 215,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-186",
      "html_url": "https://goskive.com/course/fu-course-186",
      "slug": "fu-course-186",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "topic_id": 227,
      "discipline_id": 228,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 186",
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
      "updated_at": "2016-10-11T17:00:15.689Z",
      "shortname": "fu-course-186"
    },
    {
      "creator_id": 714,
      "id": 216,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-187",
      "html_url": "https://goskive.com/course/fu-course-187",
      "slug": "fu-course-187",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "topic_id": 228,
      "discipline_id": 229,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 187",
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
      "chapters_updated_at": "2016-10-11T17:00:15.987Z",
      "updated_at": "2016-10-11T17:00:15.994Z",
      "shortname": "fu-course-187"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26b1783524e088480b637eca10218ea1fddd2eafb2938ba8aadf9fe8c8a76f09"
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
      "creator_id": 744,
      "id": 239,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-210",
      "html_url": "https://goskive.com/course/fu-course-210",
      "slug": "fu-course-210",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "topic_id": 251,
      "discipline_id": 252,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 210",
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
      "updated_at": "2016-10-11T17:00:18.477Z",
      "shortname": "fu-course-210"
    },
    {
      "creator_id": 744,
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-211",
      "html_url": "https://goskive.com/course/fu-course-211",
      "slug": "fu-course-211",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "topic_id": 252,
      "discipline_id": 253,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 211",
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
      "chapters_updated_at": "2016-10-11T17:00:18.776Z",
      "updated_at": "2016-10-11T17:00:18.783Z",
      "shortname": "fu-course-211"
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
Authorization: Bearer 080ebfbb7aecb96461333d013a56cc9af5c2ec392d308e8d3e6495850f8dfeae
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
      "creator_id": 720,
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-190",
      "html_url": "https://goskive.com/course/fu-course-190",
      "slug": "fu-course-190",
      "university_id": 219,
      "additional_university_ids": [

      ],
      "topic_id": 231,
      "discipline_id": 232,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 190",
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
      "updated_at": "2016-10-11T17:00:16.223Z",
      "shortname": "fu-course-190"
    },
    {
      "creator_id": 720,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 219,
      "additional_university_ids": [

      ],
      "topic_id": 232,
      "discipline_id": 233,
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
      "updated_at": "2016-10-11T17:00:16.264Z",
      "shortname": "fu-course-191"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 080ebfbb7aecb96461333d013a56cc9af5c2ec392d308e8d3e6495850f8dfeae"
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
      "creator_id": 749,
      "id": 243,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 255,
      "discipline_id": 256,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
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
      "updated_at": "2016-10-11T17:00:18.983Z",
      "shortname": "fu-course-214"
    },
    {
      "creator_id": 749,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
      "updated_at": "2016-10-11T17:00:19.029Z",
      "shortname": "fu-course-215"
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
Authorization: Bearer e64be9bdfb45d2b1073783b79f654af1f48cb79e4e5e8122d954ae50c6f1812a
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
  "id": 807,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-11T17:00:25.577Z",
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
	-H "Authorization: Bearer e64be9bdfb45d2b1073783b79f654af1f48cb79e4e5e8122d954ae50c6f1812a"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/448
Content-Type: application/json
Authorization: Bearer 052e7705ac66b04021ff460800d20b602cc111967f654fa7bd24fa721174cff0
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
    "id": 448,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 135,
    "fields_of_study": [
      132,
      133
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-11T16:59:57.826Z",
    "updated_at": "2016-10-11T16:59:57.826Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/448" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 052e7705ac66b04021ff460800d20b602cc111967f654fa7bd24fa721174cff0"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/446
Content-Type: application/json
Authorization: Bearer 88085afaaac3d14dccd308ab6c1024cf1c822174c58b4bcb487299ecfca71a3f
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
    "id": 446,
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
    "created_at": "2016-10-11T16:59:57.658Z",
    "updated_at": "2016-10-11T16:59:57.658Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/446" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88085afaaac3d14dccd308ab6c1024cf1c822174c58b4bcb487299ecfca71a3f"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/8
Content-Type: application/json
Authorization: Bearer a643dba2c74fcd627313197c2221e15c9acf348d5225330d445e5fbe8aac880e
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a643dba2c74fcd627313197c2221e15c9acf348d5225330d445e5fbe8aac880e"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/9
Content-Type: application/json
Authorization: Bearer f343cafedc441bed2fba375bb04184bf746a320cd14d5016d03f3532dfb2b322
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
    "votable_id": 32,
    "user_id": 160
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f343cafedc441bed2fba375bb04184bf746a320cd14d5016d03f3532dfb2b322"
```
