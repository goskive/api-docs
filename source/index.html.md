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
Authorization: Basic MzIxMWE3ZDJiNDhhNGFkOGRhNDc3MjY5YzRjYjg4MDJmMjcyMTRjMzdlMjk1
MzEyNmM4YzI2Nzk4YzgyYzBkMzpiMDM1N2ZkOWMxMWVkY2MwMmYyOTZkNWZj
ZTA3Mzc2OTExM2JkZTBkMDRiNmUxMGIxNTBlYTFlYTFiNGJjYmQy

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
	-u 3211a7d2b48a4ad8da477269c4cb8802f27214c37e2953126c8c26798c82c0d3:b0357fd9c11edcc02f296d5fce073769113bde0d04b6e10b150ea1ea1b4bcbd2
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0f5912d01845979559958c62d5115fa298ab665a47c1e21e9e09468e83d2f65f","client_secret":"3e9ab533da98fa15003114a1917a4aec7a59ce7eadeba68fae685afffda966f7"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0f5912d01845979559958c62d5115fa298ab665a47c1e21e9e09468e83d2f65f","client_secret":"3e9ab533da98fa15003114a1917a4aec7a59ce7eadeba68fae685afffda966f7"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"f52bf1c74cf7b63f675678c92acf05aba95c1147104b3eed25968831557838ea","client_secret":"50e4c11454a71a57a6abc21cc463ed062fb8fab3da9ebffa95bab6546e7717ed"}
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
  "access_token": "81fd12a218bad19d5a945baf94733478c90953a22eff0c60f92d770785b6a399",
  "token_type": "bearer",
  "created_at": 1477478111
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"f52bf1c74cf7b63f675678c92acf05aba95c1147104b3eed25968831557838ea","client_secret":"50e4c11454a71a57a6abc21cc463ed062fb8fab3da9ebffa95bab6546e7717ed"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTA5YjhhMTk2ODgxMzgxNTQxYjAyZTViZDI2ZjQ2NGUwMDk2NDM0NTQwOGI0
YjMxNmQzZWQ0ZTIyYzEyNDZjZTpmZGEyNzE5OTkwZmQzNjY1NzQ5NGRmMTVm
MTdmMmVjNTBkOTZhNTQzYTQ1ZmNiNmVhZDRiOTljYzhkNjc4MzQ5

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
  "access_token": "0ce3d561c8948109878ec96f19cb4c1ef5c1f9245e827e749d3aa93453e3409c",
  "token_type": "bearer",
  "created_at": 1477478111
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 909b8a196881381541b02e5bd26f464e00964345408b4b316d3ed4e22c1246ce:fda2719990fd36657494df15f17f2ec50d96a543a45fcb6ead4b99cc8d678349
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1793ba4a195960a10faef8c6d96ab4060e2648c9dd38d5db6e0a4858cae259ef","client_secret":"2966658177838f459107ae06f298534be74ec37ef3e718af7234fc32be88dcc4"}
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
  "access_token": "c54f24ff45266793f6c55b39d5d32826eb8a04bb823eb43cae18e1a0388e27e3",
  "token_type": "bearer",
  "created_at": 1477478111
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1793ba4a195960a10faef8c6d96ab4060e2648c9dd38d5db6e0a4858cae259ef","client_secret":"2966658177838f459107ae06f298534be74ec37ef3e718af7234fc32be88dcc4"}' -X POST \
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
Authorization: Bearer 8556121c72f6a3a19f7f7d3ac6f309a7e0142c65fb2290a76c7c901355cb7bb2
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
    "company_id": 24,
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
	-H "Authorization: Bearer 8556121c72f6a3a19f7f7d3ac6f309a7e0142c65fb2290a76c7c901355cb7bb2"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/1/flashcards
Content-Type: application/json
Authorization: Bearer 5a8a0195bcf814e9e9044a4a15726a3e950ef0b302c2a1fbc8c7d642b488ee60
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":1,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 1,
    "obfuscated_id": "vnOJWgI0jGc",
    "author_id": 11,
    "chapter_id": 1,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:35:05.607Z",
    "created_at": "2016-10-26T10:35:05.607Z",
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
curl "api.goskive.com/v2/chapters/1/flashcards" -d '{"flashcard":{"chapter_id":1,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a8a0195bcf814e9e9044a4a15726a3e950ef0b302c2a1fbc8c7d642b488ee60"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/2/flashcards
Content-Type: application/json
Authorization: Bearer 18ca35f964bcfcdee517a8063b26c19872274fc8ac14feccc4652401ce12701b
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
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 12,
      "chapter_id": 2,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:05.775Z",
      "created_at": "2016-10-26T10:35:05.775Z",
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
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 12,
      "chapter_id": 2,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:05.811Z",
      "created_at": "2016-10-26T10:35:05.811Z",
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
      "author_id": 12,
      "chapter_id": 2,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:35:05.846Z",
      "created_at": "2016-10-26T10:35:05.846Z",
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
curl "api.goskive.com/v2/chapters/2/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18ca35f964bcfcdee517a8063b26c19872274fc8ac14feccc4652401ce12701b"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/173/questions
Content-Type: application/json
Authorization: Bearer 35ae95977dcc188ed068ed2c253a1c3763f2bf461ee424f7d45ac1174529225c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":173,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 840,
    "chapter_id": 173,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:36:07.460Z",
    "created_at": "2016-10-26T10:36:07.460Z",
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
        "id": 214,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 215,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 216,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 217,
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
curl "api.goskive.com/v2/chapters/173/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":173,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35ae95977dcc188ed068ed2c253a1c3763f2bf461ee424f7d45ac1174529225c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/172/questions
Content-Type: application/json
Authorization: Bearer 9b29fb39f81519ccd301bddd3f939df83eb0dbb638b54d3dedac43e157c42c58
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 837,
    "chapter_id": 172,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:36:07.130Z",
    "created_at": "2016-10-26T10:36:07.130Z",
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
        "id": 212,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 213,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/172/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b29fb39f81519ccd301bddd3f939df83eb0dbb638b54d3dedac43e157c42c58"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/175/questions
Content-Type: application/json
Authorization: Bearer a65619e496e52a4e1b5ba86ad0611b3517900027c1a00c947f0ccad19202ce4a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":175,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 846,
    "chapter_id": 175,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:36:08.351Z",
    "created_at": "2016-10-26T10:36:08.351Z",
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
        "id": 221,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 222,
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
curl "api.goskive.com/v2/chapters/175/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":175,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a65619e496e52a4e1b5ba86ad0611b3517900027c1a00c947f0ccad19202ce4a"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/174/questions
Content-Type: application/json
Authorization: Bearer 703e6139416246f55e4f63ca91c7ff792bfe192b5a7331de4af0cc24ab1a8b47
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":174,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 843,
    "chapter_id": 174,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:36:07.950Z",
    "created_at": "2016-10-26T10:36:07.950Z",
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
        "id": 218,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 219,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 220,
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
curl "api.goskive.com/v2/chapters/174/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":174,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 703e6139416246f55e4f63ca91c7ff792bfe192b5a7331de4af0cc24ab1a8b47"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/177/questions
Content-Type: application/json
Authorization: Bearer cd0ba569c7b82c93ef081757b9a9c6b3732c79a09846da5d096c0846d05bf18b
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
      "author_id": 852,
      "chapter_id": 177,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:36:08.887Z",
      "created_at": "2016-10-26T10:36:08.773Z",
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
      "author_id": 853,
      "chapter_id": 177,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:36:09.075Z",
      "created_at": "2016-10-26T10:36:08.958Z",
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
      "author_id": 854,
      "chapter_id": 177,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T10:36:09.269Z",
      "created_at": "2016-10-26T10:36:09.149Z",
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
curl "api.goskive.com/v2/chapters/177/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd0ba569c7b82c93ef081757b9a9c6b3732c79a09846da5d096c0846d05bf18b"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/17
Content-Type: application/json
Authorization: Bearer a4ca048030d32d6d8470e6857847b812bbdc0caa03a0f5078a9bfbac8d05f11d
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
curl "api.goskive.com/v2/chapters/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4ca048030d32d6d8470e6857847b812bbdc0caa03a0f5078a9bfbac8d05f11d"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/19
Content-Type: application/json
Authorization: Bearer 7c9f523cebef451f56ad399db8eb5d9a4b0a1bbb0881bd530e2c6a2a592a2e5e
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
curl "api.goskive.com/v2/chapters/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c9f523cebef451f56ad399db8eb5d9a4b0a1bbb0881bd530e2c6a2a592a2e5e"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/21
Content-Type: application/json
Authorization: Bearer ed2c818faf2632eaea53cd758ce2c244e7232a63aba63ebc00c3895a755667d2
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
curl "api.goskive.com/v2/chapters/21" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed2c818faf2632eaea53cd758ce2c244e7232a63aba63ebc00c3895a755667d2"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/18
Content-Type: application/json
Authorization: Bearer 3a677a5b05479ee3f8a41354a4d71671248b8f533b109b491cd126547a6eca15
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a677a5b05479ee3f8a41354a4d71671248b8f533b109b491cd126547a6eca15"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/14
Content-Type: application/json
Authorization: Bearer f659bb81ad82e68503c22c699835114282f3c8b93868a74df4f7418f7ecd6a01
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
    "id": 14,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T10:35:15.903Z",
    "course_id": 92,
    "author_id": 178,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-26T10:35:15.397Z",
    "questions_updated_at": "2016-10-26T10:35:15.397Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 182,
        "chapter_id": 14,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:15.886Z",
        "created_at": "2016-10-26T10:35:15.886Z",
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
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 180,
        "chapter_id": 14,
        "position": 6,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:15.786Z",
        "created_at": "2016-10-26T10:35:15.670Z",
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
curl "api.goskive.com/v2/chapters/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f659bb81ad82e68503c22c699835114282f3c8b93868a74df4f7418f7ecd6a01"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/22
Content-Type: application/json
Authorization: Bearer d3d57b4e0f56fd56e3473e894d584eb43373df520a7c1a7019594bcdf907a9e9
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
    "id": 22,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T10:35:17.864Z",
    "course_id": 100,
    "author_id": 210,
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
curl "api.goskive.com/v2/chapters/22" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3d57b4e0f56fd56e3473e894d584eb43373df520a7c1a7019594bcdf907a9e9"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/49/replies
Content-Type: application/json
Authorization: Bearer 9ef5bc321cf1581e7911f059d054521572a56a5a0b247bbfdc5ae1f0151785af
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
    "id": 50,
    "author_id": 550,
    "reply_to_id": 49,
    "created_at": "2016-10-26T10:35:49.258Z",
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
curl "api.goskive.com/v2/comments/49/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ef5bc321cf1581e7911f059d054521572a56a5a0b247bbfdc5ae1f0151785af"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer 562406226d6cde91e14f0e526b5cebe5853227a59e1d7fcb6dc6eba7cb4f4bb9
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
curl "api.goskive.com/v2/comments/51/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 562406226d6cde91e14f0e526b5cebe5853227a59e1d7fcb6dc6eba7cb4f4bb9"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer fa6cc2fb548bfc0a0fcd312fbbe14d6894e494a3cbb90ad797fb800c1adebddd
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
	-H "Authorization: Bearer fa6cc2fb548bfc0a0fcd312fbbe14d6894e494a3cbb90ad797fb800c1adebddd"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/6/republish
Content-Type: application/json
Authorization: Bearer 37d31deebb9dd305f62bedefc280641ba7523c0d94920e1e677fdd38d1477983
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
curl "api.goskive.com/v2/comments/6/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37d31deebb9dd305f62bedefc280641ba7523c0d94920e1e677fdd38d1477983"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer 0054895e70213bd8bd11ab8da93b3e7df7b5d65192cdc70c01274183e4a39375
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0054895e70213bd8bd11ab8da93b3e7df7b5d65192cdc70c01274183e4a39375"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/1/report
Content-Type: application/json
Authorization: Bearer 8950f0f9c41067e7fd9fc286b6c62f1b3147801a3b72bd48fd7e1879510cd65a
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/1/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8950f0f9c41067e7fd9fc286b6c62f1b3147801a3b72bd48fd7e1879510cd65a"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/39
Content-Type: application/json
Authorization: Bearer 6f857127fbd8bf279593ffb74c45c576bf3efd77b8e319c2b1fb23c590b56d6b
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
    "updated_at": "2016-10-26T10:36:18.878Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f857127fbd8bf279593ffb74c45c576bf3efd77b8e319c2b1fb23c590b56d6b"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer fb0baea82737554ed3c5e94568e6a0ce81ba5147d6579a62e5786b17d4de7bb9
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
      "updated_at": "2016-10-26T10:36:18.756Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T10:36:18.760Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T10:36:18.764Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb0baea82737554ed3c5e94568e6a0ce81ba5147d6579a62e5786b17d4de7bb9"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer c59e938d3968d14a7d50f3244a9f9ea551513686c2fa296af546afa4c9fc538b
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
	-H "Authorization: Bearer c59e938d3968d14a7d50f3244a9f9ea551513686c2fa296af546afa4c9fc538b"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer b5577fda8f776ef2b99038ec252dc3826a1df5e21856baefc8d34a0c01b2b7af
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
	-H "Authorization: Bearer b5577fda8f776ef2b99038ec252dc3826a1df5e21856baefc8d34a0c01b2b7af"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer e3e40100f8340861c4d5ab8375b032e3afef1dd6e8f0c23966e9951d361bd86f
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
	-H "Authorization: Bearer e3e40100f8340861c4d5ab8375b032e3afef1dd6e8f0c23966e9951d361bd86f"
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
Authorization: Bearer 1ce9408e1a6336beae576b5054ba9a26bef836bbc3e819ac56389fb78aefce49
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
	-H "Authorization: Bearer 1ce9408e1a6336beae576b5054ba9a26bef836bbc3e819ac56389fb78aefce49"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 853842f1dcf7b972e66e0e0796ce0b7f493e078a9a1f8e863aaa29822ad558f7
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
    "id": 170,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T10:36:06.467Z",
    "course_id": 270,
    "author_id": 826,
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
	-H "Authorization: Bearer 853842f1dcf7b972e66e0e0796ce0b7f493e078a9a1f8e863aaa29822ad558f7"
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
      "id": 151,
      "title": "Clever Chapter Title 136",
      "position": 1,
      "updated_at": "2016-10-26T10:36:04.215Z",
      "course_id": 260,
      "author_id": 785,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 152,
      "title": "Clever Chapter Title 137",
      "position": 2,
      "updated_at": "2016-10-26T10:36:04.238Z",
      "course_id": 260,
      "author_id": 786,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 153,
      "title": "Clever Chapter Title 138",
      "position": 3,
      "updated_at": "2016-10-26T10:36:04.489Z",
      "course_id": 260,
      "author_id": 787,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T10:36:04.134Z",
      "questions_updated_at": "2016-10-26T10:36:04.134Z",
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
Authorization: Bearer 6d0e1f659c58b3c0d37e6fe0a7f6fd2dc3aea9b8e53a744ad2bb6e886da2c9a8
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
      "id": 157,
      "title": "Clever Chapter Title 142",
      "position": 1,
      "updated_at": "2016-10-26T10:36:04.851Z",
      "course_id": 263,
      "author_id": 796,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 158,
      "title": "Clever Chapter Title 143",
      "position": 2,
      "updated_at": "2016-10-26T10:36:04.875Z",
      "course_id": 263,
      "author_id": 797,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 159,
      "title": "Clever Chapter Title 144",
      "position": 3,
      "updated_at": "2016-10-26T10:36:05.118Z",
      "course_id": 263,
      "author_id": 798,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T10:36:04.777Z",
      "questions_updated_at": "2016-10-26T10:36:04.777Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d0e1f659c58b3c0d37e6fe0a7f6fd2dc3aea9b8e53a744ad2bb6e886da2c9a8"
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
      "id": 154,
      "title": "Clever Chapter Title 139",
      "position": 1,
      "updated_at": "2016-10-26T10:36:04.689Z",
      "course_id": 262,
      "author_id": 792,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 155,
      "title": "Clever Chapter Title 140",
      "position": 2,
      "updated_at": "2016-10-26T10:36:04.713Z",
      "course_id": 262,
      "author_id": 793,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 156,
      "title": "Clever Chapter Title 141",
      "position": 3,
      "updated_at": "2016-10-26T10:36:04.737Z",
      "course_id": 262,
      "author_id": 794,
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
Authorization: Bearer 0e47e94a7c225fcb26fcc571d9fe337e5e24902ae30466249a4306726d49d775
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
      "id": 160,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-26T10:36:05.285Z",
      "course_id": 264,
      "author_id": 803,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 161,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-26T10:36:05.310Z",
      "course_id": 264,
      "author_id": 804,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 162,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-26T10:36:05.334Z",
      "course_id": 264,
      "author_id": 805,
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
	-H "Authorization: Bearer 0e47e94a7c225fcb26fcc571d9fe337e5e24902ae30466249a4306726d49d775"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer df2a699dcd296986c852159327f5c78a48ec7f64bf8caad83ebd575ab6422ec5
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
    "id": 3,
    "course_id": 140,
    "user_id": 351,
    "updated_at": "2016-10-26T10:35:28.627Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df2a699dcd296986c852159327f5c78a48ec7f64bf8caad83ebd575ab6422ec5"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c5acea676704a1a6858ccd48de3ec9163f6bdca7e6b4eaf840e6fcb0d60fbceb
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
      "course_id": 144,
      "user_id": 361,
      "updated_at": "2016-10-26T10:35:29.089Z"
    },
    {
      "id": 7,
      "course_id": 144,
      "user_id": 362,
      "updated_at": "2016-10-26T10:35:29.103Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5acea676704a1a6858ccd48de3ec9163f6bdca7e6b4eaf840e6fcb0d60fbceb"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/103/files
Content-Type: application/json
Authorization: Bearer 189092da0a3fe7cd444bcf2ec5bcc2778cf83f149fefb4effa9061e954e03f94
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
        "id": 222,
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
        "created_at": "2016-10-26T10:35:18.965Z",
        "updated_at": "2016-10-26T10:35:18.965Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T10:35:18.978Z",
      "updated_at": "2016-10-26T10:35:18.978Z",
      "course_id": 103,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 223,
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
        "created_at": "2016-10-26T10:35:18.985Z",
        "updated_at": "2016-10-26T10:35:18.985Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T10:35:18.995Z",
      "updated_at": "2016-10-26T10:35:18.995Z",
      "course_id": 103,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 224,
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
        "created_at": "2016-10-26T10:35:19.002Z",
        "updated_at": "2016-10-26T10:35:19.002Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T10:35:19.011Z",
      "updated_at": "2016-10-26T10:35:19.011Z",
      "course_id": 103,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/103/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 189092da0a3fe7cd444bcf2ec5bcc2778cf83f149fefb4effa9061e954e03f94"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/101/files
Content-Type: application/json
Authorization: Bearer 752485da3bea5016012ad93fff5066854a631f68046ba9c3a05097db3885c563
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
      "id": 218,
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
      "created_at": "2016-10-26T10:35:18.632Z",
      "updated_at": "2016-10-26T10:35:18.632Z"
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
    "created_at": "2016-10-26T10:35:18.685Z",
    "updated_at": "2016-10-26T10:35:18.685Z",
    "course_id": 101,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/101/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 752485da3bea5016012ad93fff5066854a631f68046ba9c3a05097db3885c563"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/102/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 0d73b1bca5d59639dafee45f0917830b10ec59cd1ba9428c19bff11e58756d2e
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
    "key": "cache/7f041dae21eb44c7b9d0c41799d8436b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxMTozNToxOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzdmMDQxZGFlMjFlYjQ0YzdiOWQwYzQxNzk5ZDg0MzZiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI2VDEwMzUxOFoifV19",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T103518Z",
    "x-amz-signature": "77c932bf1a3d1a649f62ae9746b6d02975937cd3e55b0d78acdb9ed8d7f44b84"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/102/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d73b1bca5d59639dafee45f0917830b10ec59cd1ba9428c19bff11e58756d2e"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 47134288a489985ca056affc8bf74b5590c4512ab0799a22648f4e847c340f24
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
	-H "Authorization: Bearer 47134288a489985ca056affc8bf74b5590c4512ab0799a22648f4e847c340f24"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2b33d9b4c4934a6562f42eb4f5729c5abf9ce00b03ad820329b6578935fc7d13
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
	-H "Authorization: Bearer 2b33d9b4c4934a6562f42eb4f5729c5abf9ce00b03ad820329b6578935fc7d13"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 549d575b6a15f581af3d22329631568f71974e29140eb04dfa4ffe97d75303fa
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
	-H "Authorization: Bearer 549d575b6a15f581af3d22329631568f71974e29140eb04dfa4ffe97d75303fa"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a7cb7b7970654dd7abbe10dc8832dc9d3eaa21c03b72dba2bea6c8c0bdb26018
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
	-H "Authorization: Bearer a7cb7b7970654dd7abbe10dc8832dc9d3eaa21c03b72dba2bea6c8c0bdb26018"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d1b705a63014433c878fc125fb5ca7cb823f4e13f52b51945255cd1a0d07cc73
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
	-H "Authorization: Bearer d1b705a63014433c878fc125fb5ca7cb823f4e13f52b51945255cd1a0d07cc73"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer af52ccb5773c76891e5c13c2209f294d886bbd4eb39b988294b5df74b36070ca
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
    "creator_id": 443,
    "id": 176,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 156,
    "additional_university_ids": [

    ],
    "topic_id": 185,
    "discipline_id": 186,
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
    "chapters_updated_at": "2016-10-26T10:35:34.736Z",
    "updated_at": "2016-10-26T10:35:36.151Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 63,
        "title": "Clever Chapter Title 48",
        "position": 1,
        "updated_at": "2016-10-26T10:35:36.106Z",
        "course_id": 176,
        "author_id": 443,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T10:35:34.736Z",
        "questions_updated_at": "2016-10-26T10:35:34.736Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 64,
        "title": "Clever Chapter Title 49",
        "position": 2,
        "updated_at": "2016-10-26T10:35:36.144Z",
        "course_id": 176,
        "author_id": 443,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T10:35:34.736Z",
        "questions_updated_at": "2016-10-26T10:35:34.736Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 444,
        "chapter_id": 63,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:35.955Z",
        "created_at": "2016-10-26T10:35:35.955Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 444,
        "chapter_id": 64,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:36.021Z",
        "created_at": "2016-10-26T10:35:36.021Z",
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
        "author_id": 444,
        "chapter_id": 63,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:35.992Z",
        "created_at": "2016-10-26T10:35:35.992Z",
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
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 444,
        "chapter_id": 64,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:36.059Z",
        "created_at": "2016-10-26T10:35:36.059Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 444,
        "chapter_id": 63,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:34.937Z",
        "created_at": "2016-10-26T10:35:34.827Z",
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
            "id": 47,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 48,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 444,
        "chapter_id": 63,
        "position": 25,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:35.131Z",
        "created_at": "2016-10-26T10:35:35.025Z",
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
            "id": 49,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 50,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 444,
        "chapter_id": 64,
        "position": 26,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:35.330Z",
        "created_at": "2016-10-26T10:35:35.213Z",
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
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 444,
        "chapter_id": 64,
        "position": 27,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:35.507Z",
        "created_at": "2016-10-26T10:35:35.395Z",
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
            "id": 53,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 54,
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
	-H "Authorization: Bearer af52ccb5773c76891e5c13c2209f294d886bbd4eb39b988294b5df74b36070ca"
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
    "creator_id": 455,
    "id": 178,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 158,
    "additional_university_ids": [

    ],
    "topic_id": 187,
    "discipline_id": 188,
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
    "chapters_updated_at": "2016-10-26T10:35:37.742Z",
    "updated_at": "2016-10-26T10:35:39.128Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 67,
        "title": "Clever Chapter Title 52",
        "position": 1,
        "updated_at": "2016-10-26T10:35:39.081Z",
        "course_id": 178,
        "author_id": 455,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T10:35:37.742Z",
        "questions_updated_at": "2016-10-26T10:35:37.742Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 68,
        "title": "Clever Chapter Title 53",
        "position": 2,
        "updated_at": "2016-10-26T10:35:39.120Z",
        "course_id": 178,
        "author_id": 455,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T10:35:37.742Z",
        "questions_updated_at": "2016-10-26T10:35:37.742Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 455,
        "chapter_id": 67,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:37.941Z",
        "created_at": "2016-10-26T10:35:37.832Z",
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
            "id": 71,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 72,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 455,
        "chapter_id": 68,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T10:35:38.307Z",
        "created_at": "2016-10-26T10:35:38.189Z",
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
PUT /v2/courses/166/pin
Content-Type: application/json
Authorization: Bearer 998b3f483425fb5b90fdfb8adb6d0dc0d7dc588c38c707438f53c392a89244e6
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/166/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 998b3f483425fb5b90fdfb8adb6d0dc0d7dc588c38c707438f53c392a89244e6"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/165/pin
Content-Type: application/json
Authorization: Bearer 7640d72c437cd251b014e17df9ac816ab03374674e4ec4caaed5bd0a61f66793
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/165/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7640d72c437cd251b014e17df9ac816ab03374674e4ec4caaed5bd0a61f66793"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5947efa757964bdea039aa48f30b60225b004054dc302bd7215e7af09241931d
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
    "creator_id": 418,
    "id": 164,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 144,
    "additional_university_ids": [

    ],
    "topic_id": 173,
    "discipline_id": 174,
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
    "updated_at": "2016-10-26T10:35:33.005Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5947efa757964bdea039aa48f30b60225b004054dc302bd7215e7af09241931d"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 4f0189aee33cdbaea9b97f27c84299ff7c753f31ca9551a6ba27730228e87622
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
    "id": 211,
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
    "created_at": "2016-10-26T10:35:17.901Z",
    "updated_at": "2016-10-26T10:35:17.901Z",
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
	-H "Authorization: Bearer 4f0189aee33cdbaea9b97f27c84299ff7c753f31ca9551a6ba27730228e87622"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f07ebb1141739f9c868f2a2c64636af67e220feca3aa556472fa1c173c6ce1da
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[104]}
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
    "id": 213,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      104
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T10:35:18.312Z",
    "updated_at": "2016-10-26T10:35:18.344Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[104]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f07ebb1141739f9c868f2a2c64636af67e220feca3aa556472fa1c173c6ce1da"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1117948ba739077c882379552f94c52c7b6f64bab9d0f1531c62182db8419878
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
    "id": 215,
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
    "created_at": "2016-10-26T10:35:18.431Z",
    "updated_at": "2016-10-26T10:35:18.431Z",
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
	-H "Authorization: Bearer 1117948ba739077c882379552f94c52c7b6f64bab9d0f1531c62182db8419878"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer aa17e61565eb2d82c25ba465aa054603376a35830ddef371b53a5e9dfa980135
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[105]}
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
    "id": 214,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      105
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T10:35:18.384Z",
    "updated_at": "2016-10-26T10:35:18.384Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[105]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa17e61565eb2d82c25ba465aa054603376a35830ddef371b53a5e9dfa980135"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 53bcf5bc3a58eec71edbf02b370b93cfb170ee6295cb92b78af99959cf2c4898
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

103
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
    "id": 212,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/649580b9affb7fc992ecada2597de9d9ca587d90.jpg",
    "university_id": null,
    "fields_of_study": [
      103
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T10:35:18.004Z",
    "updated_at": "2016-10-26T10:35:18.262Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/2499cb1b8d3a8951924f4da16c8d383844513148.jpg",
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

103
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 53bcf5bc3a58eec71edbf02b370b93cfb170ee6295cb92b78af99959cf2c4898"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer e91a1c3a8a519cb50c9f89c267496cb06f6454a154513948d2d6bae355abf025
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
      "id": 7,
      "bookmarkable_id": 132,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 133,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 134,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e91a1c3a8a519cb50c9f89c267496cb06f6454a154513948d2d6bae355abf025"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a2db7f13174ecf3b86ce36c34ffc4736c34735bd523b27a252bbff26588eece4
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
      "company_id": 30,
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
	-H "Authorization: Bearer a2db7f13174ecf3b86ce36c34ffc4736c34735bd523b27a252bbff26588eece4"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer d7f01b827cf0c8d3872182809be20f13e1efe169e030052ff6151ad6cb7cff2d
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
	-H "Authorization: Bearer d7f01b827cf0c8d3872182809be20f13e1efe169e030052ff6151ad6cb7cff2d"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 79877a0e4d0ceae0a6efc6b76a84db5a6ee72198fc948e0aac5f927ce47e5d87
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
      "creator_id": 833,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-213",
      "html_url": "https://goskive.com/course/mit-course-213",
      "slug": "mit-course-213",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 285,
      "discipline_id": 286,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 213",
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
      "updated_at": "2016-10-26T10:36:06.877Z",
      "shortname": "mit-course-213"
    },
    {
      "creator_id": 834,
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-214",
      "html_url": "https://goskive.com/course/mit-course-214",
      "slug": "mit-course-214",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 286,
      "discipline_id": 287,
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
      "updated_at": "2016-10-26T10:36:06.954Z",
      "shortname": "mit-course-214"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79877a0e4d0ceae0a6efc6b76a84db5a6ee72198fc948e0aac5f927ce47e5d87"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 3bcc097a15176ef6039bb6c75247bb8cfa3b824767e9da19a0cc8248fab1f781
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T10:35:19.407Z"
      },
      "created_at": "2016-10-26T10:35:19.410Z",
      "updated_at": "2016-10-26T10:35:19.410Z",
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 19",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T10:35:19.418Z"
      },
      "created_at": "2016-10-26T10:35:19.421Z",
      "updated_at": "2016-10-26T10:35:19.421Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bcc097a15176ef6039bb6c75247bb8cfa3b824767e9da19a0cc8248fab1f781"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 1ba4dc56cba3c0f120a2aea6a7733a69d18a2004caa924ec867f9a7b2323c809
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
      "company_id": 17,
      "company": {
        "id": 17,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T10:35:19.215Z"
      },
      "created_at": "2016-10-26T10:35:19.220Z",
      "updated_at": "2016-10-26T10:35:19.220Z",
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T10:35:19.234Z"
      },
      "created_at": "2016-10-26T10:35:19.237Z",
      "updated_at": "2016-10-26T10:35:19.237Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ba4dc56cba3c0f120a2aea6a7733a69d18a2004caa924ec867f9a7b2323c809"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 158c153b46670d7ac82aab970266551d299e6070d59bd47605809f536090c752
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
      "created_at": "2016-10-26T10:35:29.598Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 47,
      "updated_at": "2016-10-26T10:35:29.707Z",
      "author_id": "373",
      "thread_subject_id": "147",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 9,
      "created_at": "2016-10-26T10:35:29.696Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 48,
      "updated_at": "2016-10-26T10:35:29.710Z",
      "author_id": "376",
      "thread_subject_id": "148",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 10,
      "created_at": "2016-10-26T10:35:30.069Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-10-26T10:35:30.069Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-10-26T10:35:30.434Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 8,
      "updated_at": "2016-10-26T10:35:30.434Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 12,
      "created_at": "2016-10-26T10:35:30.817Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 9,
      "updated_at": "2016-10-26T10:35:30.817Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 13,
      "created_at": "2016-10-26T10:35:31.113Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 19,
      "updated_at": "2016-10-26T10:35:31.113Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 14,
      "created_at": "2016-10-26T10:35:31.415Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-10-26T10:35:31.415Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-10-26T10:35:31.700Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 21,
      "updated_at": "2016-10-26T10:35:31.700Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 158c153b46670d7ac82aab970266551d299e6070d59bd47605809f536090c752"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/7
Content-Type: application/json
Authorization: Bearer fb22c4f2c908c14261bd0c330b1bdd83c233698035f0ce4679b504032806a4e6
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-26T10:25:29.000Z"}}
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
    "created_at": "2016-10-26T10:35:29.433Z",
    "read_at": "2016-10-26T10:25:29.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 46,
    "updated_at": "2016-10-26T10:35:29.488Z",
    "author_id": "369",
    "thread_subject_id": "146",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/7" -d '{"notification":{"read_at":"2016-10-26T10:25:29.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb22c4f2c908c14261bd0c330b1bdd83c233698035f0ce4679b504032806a4e6"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 489938365790eec58abde7ed6050faaf0fcda9c60e75d0b600636121557b7f33
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
      "course_id": 158,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T10:35:32.296Z",
      "course_published": true,
      "updated_at": "2016-10-26T10:35:32.289Z"
    },
    {
      "id": 4,
      "course_id": 159,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T10:35:32.374Z",
      "course_published": true,
      "updated_at": "2016-10-26T10:35:32.367Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 489938365790eec58abde7ed6050faaf0fcda9c60e75d0b600636121557b7f33"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer 26e99153ada4af5ec43306f8be05c8d81b77972f452cba4aa365475a736f6f08
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
    "id": 1,
    "course_id": 155,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T10:35:31.899Z",
    "course_published": true,
    "updated_at": "2016-10-26T10:35:31.891Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26e99153ada4af5ec43306f8be05c8d81b77972f452cba4aa365475a736f6f08"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 6013f25bb5002fb676aad13e8d6060c36f0e0a11165aea96a3bec64806178a24
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
    "id": 5,
    "course_id": 160,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-26T10:35:32.531Z",
    "course_published": true,
    "updated_at": "2016-10-26T10:35:32.521Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6013f25bb5002fb676aad13e8d6060c36f0e0a11165aea96a3bec64806178a24"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f3e5a21e3dcf5d1cb996984dcada9d5dd2705cec8d028fe4414f7d928c7dd663
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
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 113,
      "user_id": 861
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 114,
      "user_id": 861
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 115,
      "user_id": 861
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 116,
      "user_id": 861
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3e5a21e3dcf5d1cb996984dcada9d5dd2705cec8d028fe4414f7d928c7dd663"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/3
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
    "id": 3,
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
        "discipline_id": 3
      },
      {
        "id": 2,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 3
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/3" -X GET \
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
      "id": 1,
      "name": "Total well-modulated parallelism",
      "name_translations": {
        "en": "Total well-modulated parallelism"
      }
    },
    {
      "id": 2,
      "name": "Persistent mission-critical encryption",
      "name_translations": {
        "en": "Persistent mission-critical encryption"
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
PATCH /v2/feedbacks/29/close
Content-Type: application/json
Authorization: Bearer fa22a6cf702dad23c3e0de4c7f75c211563a8fd8f3a0b316464df7ae181f5521
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
    "id": 29,
    "user_id": 682,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-26T10:35:57.591Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/29/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa22a6cf702dad23c3e0de4c7f75c211563a8fd8f3a0b316464df7ae181f5521"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/6/fix
Content-Type: application/json
Authorization: Bearer 101a2ebfb26c6dbcff15ac0cf1eaba8887abe315f0981763e96dacdaa98178c8
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
    "id": 6,
    "user_id": 581,
    "feedbackable_id": 71,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-26T10:35:50.896Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/6/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 101a2ebfb26c6dbcff15ac0cf1eaba8887abe315f0981763e96dacdaa98178c8"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/2
Content-Type: application/json
Authorization: Bearer 6d95b837d8a5f4d178c5ea028278bb3ee52d7dcc679ce0fc4d74937d171ab0fd
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
    "id": 2,
    "user_id": 559,
    "feedbackable_id": 67,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T10:35:49.866Z",
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
curl "api.goskive.com/v2/feedbacks/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d95b837d8a5f4d178c5ea028278bb3ee52d7dcc679ce0fc4d74937d171ab0fd"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer f658b45881fd37c60139c8a1b9ae52c78852d6fd703039a3048c2fc6c16c2f5b
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
curl "api.goskive.com/v2/feedbacks/4/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f658b45881fd37c60139c8a1b9ae52c78852d6fd703039a3048c2fc6c16c2f5b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/7/fix
Content-Type: application/json
Authorization: Bearer 53dcc3ee0306937077e23d580056daa0eb217e20919b16c65011a3e21694b9b1
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
curl "api.goskive.com/v2/feedbacks/7/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53dcc3ee0306937077e23d580056daa0eb217e20919b16c65011a3e21694b9b1"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer 669e46fee5c4d7223a54962cdb155e46a20f2668c4210abbf19cd2e29fe81199
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
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 669e46fee5c4d7223a54962cdb155e46a20f2668c4210abbf19cd2e29fe81199"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/3
Content-Type: application/json
Authorization: Bearer 6cd00528ff99f3cffb4ac1d7931925a8cf3d090cefa17a8292b9a285993fcc67
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
    "id": 3,
    "user_id": 564,
    "feedbackable_id": 68,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T10:35:50.154Z",
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
curl "api.goskive.com/v2/feedbacks/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cd00528ff99f3cffb4ac1d7931925a8cf3d090cefa17a8292b9a285993fcc67"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 026526a633972806f15812536ac286060a9154c0fc75cdb9e979a19ea6500a95
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 026526a633972806f15812536ac286060a9154c0fc75cdb9e979a19ea6500a95"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/13/bookmark
Content-Type: application/json
Authorization: Bearer 3050a82926ff4fab4c1047d89d833914aed4f1bb1acf1a8b1f93f80e03813dcc
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3050a82926ff4fab4c1047d89d833914aed4f1bb1acf1a8b1f93f80e03813dcc"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer b62c8b6bad2ae15a499ecaa20d382e54f4a04b8f53fc581bc1bac247aee47c36
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b62c8b6bad2ae15a499ecaa20d382e54f4a04b8f53fc581bc1bac247aee47c36"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/5
Content-Type: application/json
Authorization: Bearer ef413c4de6fc760611d96dc4877f07c49c314c87ced1ce2dd1533d6c1e12aec2
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/15fd1c2cae38209dcb7647aacdd42d18.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T103612Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=47c5b86ffa7af07e47a91467059299540ed1f29b54de3cf2c42ff2c9e7c427e7",
    "expires_in": 86400
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
	-H "Authorization: Bearer ef413c4de6fc760611d96dc4877f07c49c314c87ced1ce2dd1533d6c1e12aec2"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer dfaea257a591abf7d76da33718afb1398af366a283c340f9294d766f53822da5
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/591bc0450bb9893abb421bb6e69e8899.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T103613Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=83114cdee186f64dea405d6fb3db9cfa67c1ec31b4d8c8f8c6901c72a68f2e4d",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/14/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfaea257a591abf7d76da33718afb1398af366a283c340f9294d766f53822da5"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 197eb1ea54f437d7d0c2d8bc9f1d2e843f47ca13d4bd7a0854bae7b1e3b4db0d
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
      "id": 893,
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
      "created_at": "2016-10-26T10:36:12.982Z",
      "updated_at": "2016-10-26T10:36:12.982Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-26T10:36:13.058Z",
    "updated_at": "2016-10-26T10:36:13.058Z",
    "course_id": 290,
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
	-H "Authorization: Bearer 197eb1ea54f437d7d0c2d8bc9f1d2e843f47ca13d4bd7a0854bae7b1e3b4db0d"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/16/matched_courses?required_cu_count=2
Authorization: Bearer 9862fe71b3a9b14f52e232fc5728ac779da4e3197a77b7c66c6175b6f5079ea0
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
      "creator_id": 943,
      "id": 304,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 289,
      "additional_university_ids": [

      ],
      "topic_id": 316,
      "discipline_id": 317,
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
      "chapters_updated_at": "2016-10-26T10:36:16.038Z",
      "updated_at": "2016-10-26T10:36:17.620Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 948,
      "id": 305,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-524aa63a-a848-4798-8dfa-61cb8d6c412d",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-524aa63a-a848-4798-8dfa-61cb8d6c412d",
      "slug": "mit-the-great-british-bake-off-524aa63a-a848-4798-8dfa-61cb8d6c412d",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "topic_id": 317,
      "discipline_id": 318,
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
      "chapters_updated_at": "2016-10-26T10:36:16.038Z",
      "updated_at": "2016-10-26T10:36:18.167Z",
      "shortname": "mit-the-great-british-bake-off-524aa63a-a848-4798-8dfa-61cb8d6c412d"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/16/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 9862fe71b3a9b14f52e232fc5728ac779da4e3197a77b7c66c6175b6f5079ea0"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/15/report
Content-Type: application/json
Authorization: Bearer a858523143ed228036e863755315a9105cdb4f8a2094fc3b63410cf27c4e4058
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
	-H "Authorization: Bearer a858523143ed228036e863755315a9105cdb4f8a2094fc3b63410cf27c4e4058"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer 6ccdee7c1aefa1d1acf9b24e76456aee09a9f2cea2435af88d80df14c5d39963
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
	-H "Authorization: Bearer 6ccdee7c1aefa1d1acf9b24e76456aee09a9f2cea2435af88d80df14c5d39963"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/86/comments
Content-Type: application/json
Authorization: Bearer 7b6b268c49fbf8c6cce8f8f748037e9696b3a26375455984d8c226c46650a706
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
    "id": 58,
    "author_id": 762,
    "reply_to_id": null,
    "created_at": "2016-10-26T10:36:02.964Z",
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
curl "api.goskive.com/v2/flashcards/86/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b6b268c49fbf8c6cce8f8f748037e9696b3a26375455984d8c226c46650a706"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/comments
Content-Type: application/json
Authorization: Bearer e293d35ec58bcf7af55f6600d7a769423537bbeb0c1f295098d6395e7142ffb0
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
    "id": 57,
    "author_id": 759,
    "reply_to_id": null,
    "created_at": "2016-10-26T10:36:02.657Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 759,
      "feedbackable_id": 85,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:02.654Z",
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
curl "api.goskive.com/v2/flashcards/85/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e293d35ec58bcf7af55f6600d7a769423537bbeb0c1f295098d6395e7142ffb0"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/88/comments
Content-Type: application/json
Authorization: Bearer 94a5caece112825185830d8ea7e8c117ee4fb186f3e52b5550c0a67917ddbb29
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
      "author_id": 772,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:36:03.446Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 771,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:36:03.431Z",
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
curl "api.goskive.com/v2/flashcards/88/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94a5caece112825185830d8ea7e8c117ee4fb186f3e52b5550c0a67917ddbb29"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/84/comments
Content-Type: application/json
Authorization: Bearer cec2f1665f522307858dba65765c397e0a02277a10a5938a60425fce4715b623
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
curl "api.goskive.com/v2/flashcards/84/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cec2f1665f522307858dba65765c397e0a02277a10a5938a60425fce4715b623"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/82/feedbacks
Content-Type: application/json
Authorization: Bearer 21f8ec6b8ab010da335cd58e87815571951be165c7be59de470148f8c5100019
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
    "id": 44,
    "user_id": 750,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T10:36:01.877Z",
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
curl "api.goskive.com/v2/flashcards/82/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21f8ec6b8ab010da335cd58e87815571951be165c7be59de470148f8c5100019"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/81/feedbacks
Content-Type: application/json
Authorization: Bearer eaf145cf289cea927de4e7c759d6eaff0434e98dc954efb11f2ca68cf5c11195
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
      "id": 43,
      "user_id": 749,
      "feedbackable_id": 81,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:01.688Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 748,
      "feedbackable_id": 81,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:36:01.677Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/81/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaf145cf289cea927de4e7c759d6eaff0434e98dc954efb11f2ca68cf5c11195"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/5/votes
Content-Type: application/json
Authorization: Bearer 3c84196f9d7f076df0271219ca26fc33c5c82edeea31c7d476def2c147a4f7b7
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
      "votable_id": 5,
      "user_id": 23
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 5,
      "user_id": 22
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 5,
      "user_id": 21
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c84196f9d7f076df0271219ca26fc33c5c82edeea31c7d476def2c147a4f7b7"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/17/republish
Content-Type: application/json
Authorization: Bearer 3a23fa84f6c7f635029b32937388d2ad29a7446923d4deb5fa685d1538b7b728
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
	-H "Authorization: Bearer 3a23fa84f6c7f635029b32937388d2ad29a7446923d4deb5fa685d1538b7b728"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/38/bookmark
Content-Type: application/json
Authorization: Bearer ca27698e3d5784f50ab2cb9cad7534b0f8c3091e667454a28f8ef9824e96864d
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca27698e3d5784f50ab2cb9cad7534b0f8c3091e667454a28f8ef9824e96864d"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/19
Content-Type: application/json
Authorization: Bearer f6bb174332266a99806f217995b2d4dd85cc42946a9fda8bcd1e0107d7c27b57
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6bb174332266a99806f217995b2d4dd85cc42946a9fda8bcd1e0107d7c27b57"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/downvote
Content-Type: application/json
Authorization: Bearer 5fae96928db961a5e6bde226062000dd2b0cacf826f19c8a62abebe6c33e9a6d
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fae96928db961a5e6bde226062000dd2b0cacf826f19c8a62abebe6c33e9a6d"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/39
Content-Type: application/json
Authorization: Bearer 73ac822f2d407e71093ced1261f843d199e2056151b63559c91b0db7e8a66330
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 345,
    "chapter_id": 51,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:35:28.327Z",
    "created_at": "2016-10-26T10:35:28.327Z",
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
curl "api.goskive.com/v2/flashcards/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73ac822f2d407e71093ced1261f843d199e2056151b63559c91b0db7e8a66330"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/report
Content-Type: application/json
Authorization: Bearer fa388526e6398e7661f3b30a7342b1cf4ff81bd9284a74ae9df6ce579a5efc6a
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa388526e6398e7661f3b30a7342b1cf4ff81bd9284a74ae9df6ce579a5efc6a"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/18/bookmark
Content-Type: application/json
Authorization: Bearer a3d92e4925fa0be5fa42fee51192ed34feca63944004154155449644d2e24424
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
	-H "Authorization: Bearer a3d92e4925fa0be5fa42fee51192ed34feca63944004154155449644d2e24424"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/20/upvote
Content-Type: application/json
Authorization: Bearer 11651c01cd74689ab368f387dbdea0bb26fc4f1ab9cc80c9cc3c78caf9480439
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/20/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11651c01cd74689ab368f387dbdea0bb26fc4f1ab9cc80c9cc3c78caf9480439"
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
    "key": "cache/7b8ae64a649dfd60ee7583fa38790009.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxMTozNTo0OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzdiOGFlNjRhNjQ5ZGZkNjBlZTc1ODNmYTM4NzkwMDA5LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjZUMTAzNTQ4WiJ9XX0=",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T103548Z",
    "x-amz-signature": "0118b9ebe9d0a7a6cdf24d934ad6687222c81405f9072b0d8c8fac176e07f378"
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
Authorization: Bearer e495976cb5d8dfec0e744aa232510d6c0d77efc7a34e96a46ff237f09a005fd6
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
	-H "Authorization: Bearer e495976cb5d8dfec0e744aa232510d6c0d77efc7a34e96a46ff237f09a005fd6"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 2e5ef506fd494862d297428e864a050139f8bc50f291ac0ed99ba34558f9ccf3
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
	-H "Authorization: Bearer 2e5ef506fd494862d297428e864a050139f8bc50f291ac0ed99ba34558f9ccf3"
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
{"password":{"reset_password_token":"ko4MrVZ5z4gRUQqajqz1","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 269,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-26T10:35:24.064Z",
  "updated_at": "2016-10-26T10:35:24.198Z",
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
  "audit_id": 3979
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"ko4MrVZ5z4gRUQqajqz1","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer 6a1e223ffdacabcbb06500a42f8aa321e7bdf6a986db5dd44f88597b07351cd6
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
    "id": 42,
    "author_id": 235,
    "reply_to_id": null,
    "created_at": "2016-10-26T10:35:20.238Z",
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
curl "api.goskive.com/v2/questions/12/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a1e223ffdacabcbb06500a42f8aa321e7bdf6a986db5dd44f88597b07351cd6"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/13/comments
Content-Type: application/json
Authorization: Bearer 5560762e897b2f5d5ba2691285f143bdf0e5cc50d249c000beaadf2951733862
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
    "id": 43,
    "author_id": 238,
    "reply_to_id": null,
    "created_at": "2016-10-26T10:35:20.916Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 238,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:20.911Z",
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
curl "api.goskive.com/v2/questions/13/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5560762e897b2f5d5ba2691285f143bdf0e5cc50d249c000beaadf2951733862"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/14/comments
Content-Type: application/json
Authorization: Bearer 811900dfec50c874ffec8d68828f17b0fd1a6a5c934fade1691d92f97360fbe8
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
      "id": 44,
      "author_id": 244,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:21.364Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 245,
      "reply_to_id": null,
      "created_at": "2016-10-26T10:35:21.379Z",
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
curl "api.goskive.com/v2/questions/14/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 811900dfec50c874ffec8d68828f17b0fd1a6a5c934fade1691d92f97360fbe8"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer b0b3d4e9a212e58b98e2336d9acbb67b6311600713347d9f35f118c830ee0ba6
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
curl "api.goskive.com/v2/questions/11/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0b3d4e9a212e58b98e2336d9acbb67b6311600713347d9f35f118c830ee0ba6"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer f0a1b5fd73f1f31a81fa7780972e84484377c01ae20418a1275a92735257826b
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
    "id": 31,
    "user_id": 687,
    "feedbackable_id": 95,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-26T10:35:58.517Z",
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
curl "api.goskive.com/v2/questions/95/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0a1b5fd73f1f31a81fa7780972e84484377c01ae20418a1275a92735257826b"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/97/feedbacks
Content-Type: application/json
Authorization: Bearer 8d0600afa8a517b4f1967bf239e10490274fb4a129535ca1109c47b19afcbb44
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
      "id": 33,
      "user_id": 697,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:59.247Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 696,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T10:35:59.237Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/97/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d0600afa8a517b4f1967bf239e10490274fb4a129535ca1109c47b19afcbb44"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/121/votes
Content-Type: application/json
Authorization: Bearer 1f24f2b2ec45ebb79a0b3589938ff5e9be23cbbf86505ee74d64fc20a1845728
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
      "votable_id": 121,
      "user_id": 926
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 925
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 924
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/121/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f24f2b2ec45ebb79a0b3589938ff5e9be23cbbf86505ee74d64fc20a1845728"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/66/republish
Content-Type: application/json
Authorization: Bearer 207be5341a6d3b790ce52b2a1e1210cd677eef32218dc0ac65c719b484e536f0
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
curl "api.goskive.com/v2/questions/66/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 207be5341a6d3b790ce52b2a1e1210cd677eef32218dc0ac65c719b484e536f0"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/48/bookmark
Content-Type: application/json
Authorization: Bearer c1530c9ee2d9394bf6934eb5d87d67f12ed3fa19d897da2d4a4f015462d453b7
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1530c9ee2d9394bf6934eb5d87d67f12ed3fa19d897da2d4a4f015462d453b7"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/71
Content-Type: application/json
Authorization: Bearer 9c1922404cbd1f56d23bf0d9efc47459aa415eba56b1dcd32b5ab7080bc570c4
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
	-H "Authorization: Bearer 9c1922404cbd1f56d23bf0d9efc47459aa415eba56b1dcd32b5ab7080bc570c4"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/49/downvote
Content-Type: application/json
Authorization: Bearer 1e2123a4b2adafc51449baa9e2495ca2d44da657a7a0a1e8056169a779c38b99
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e2123a4b2adafc51449baa9e2495ca2d44da657a7a0a1e8056169a779c38b99"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/50
Content-Type: application/json
Authorization: Bearer 5f6b52bfc2416eecd2a4df91e0a59d04ecfd5e693dff3e46ce1c6b08dfb38767
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
    "id": 50,
    "obfuscated_id": "3_Ybw_gc_HE",
    "author_id": 472,
    "chapter_id": 73,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:35:41.545Z",
    "created_at": "2016-10-26T10:35:41.433Z",
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
        "id": 99,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 100,
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
curl "api.goskive.com/v2/questions/50" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f6b52bfc2416eecd2a4df91e0a59d04ecfd5e693dff3e46ce1c6b08dfb38767"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/68/report
Content-Type: application/json
Authorization: Bearer f3a4f2a213d4fbc7ec7522d317bbbc583f9aa5bc79a26e2998e2aa8a61dcdbec
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/68/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3a4f2a213d4fbc7ec7522d317bbbc583f9aa5bc79a26e2998e2aa8a61dcdbec"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/72/bookmark
Content-Type: application/json
Authorization: Bearer 960c81016a13fa6e0f56b8e78c207ae07fe86e8694932ea969ad7614df7b3f08
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/72/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 960c81016a13fa6e0f56b8e78c207ae07fe86e8694932ea969ad7614df7b3f08"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/70
Content-Type: application/json
Authorization: Bearer fe1c35a6a5046f9e4edeb7b006c7484496f65d5f295d5ccd4602a15acf7c9d33
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":70,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T10:35:47.564Z","updated_at":"2016-10-26T10:35:47.678Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":93,"author_id":537,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 70,
    "obfuscated_id": "EDEz1xzotLc",
    "author_id": 537,
    "chapter_id": 93,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T10:35:47.785Z",
    "created_at": "2016-10-26T10:35:47.564Z",
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
    "question": "{\"id\"=>70, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-26T10:35:47.564Z\", \"updated_at\"=>\"2016-10-26T10:35:47.678Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>93, \"author_id\"=>537, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 139,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 140,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 141,
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
curl "api.goskive.com/v2/questions/70" -d '{"question":{"question":{"id":70,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T10:35:47.564Z","updated_at":"2016-10-26T10:35:47.678Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":93,"author_id":537,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe1c35a6a5046f9e4edeb7b006c7484496f65d5f295d5ccd4602a15acf7c9d33"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/69/upvote
Content-Type: application/json
Authorization: Bearer df29c10971c2e4a6626991e244b7ed79854ffc726088d64008ebb33e8d72f3c1
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/69/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df29c10971c2e4a6626991e244b7ed79854ffc726088d64008ebb33e8d72f3c1"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6dc88d4cac22ee022a8fd910c096375e0b06d9301bfb81e7bcc2393d5cb9f65c
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
      "creator_id": 252,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 91,
      "additional_university_ids": [

      ],
      "topic_id": 118,
      "discipline_id": 119,
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
      "updated_at": "2016-10-26T10:35:22.059Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dc88d4cac22ee022a8fd910c096375e0b06d9301bfb81e7bcc2393d5cb9f65c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 2e898c51b20ea924306f2500d58859261576e95eaed21b1ece9bb979fc12f215
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
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-71",
      "html_url": "https://goskive.com/university/uni-71",
      "slug": "uni-71",
      "name": "National School of Pizza",
      "short_name": "Uni 71",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3d5a61f62a572a6e31e01d1a7ab7b93b3b4b7d6b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c9556cfa37f042e4fa17340afb325403b21e9662.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T10:35:21.788Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 88,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-70",
      "html_url": "https://goskive.com/university/uni-70",
      "slug": "uni-70",
      "name": "National School of Pastry",
      "short_name": "Uni 70",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f32d52047040656ffebb1adb1fb5d2a4d0d358f1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/de92f2e5c9964fe91d7b54ad581575ec025f253d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T10:35:21.770Z",
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
	-H "Authorization: Bearer 2e898c51b20ea924306f2500d58859261576e95eaed21b1ece9bb979fc12f215"
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
      "id": 214,
      "name": "Progressive secondary budgetary management",
      "name_translations": {
        "en": "Progressive secondary budgetary management"
      },
      "discipline_id": 215
    },
    {
      "id": 215,
      "name": "Down-sized foreground analyzer",
      "name_translations": {
        "en": "Down-sized foreground analyzer"
      },
      "discipline_id": 216
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
Authorization: Bearer 2cf1fd1f42bc4c889846b2b321b0b2c4b20ae62ae3e64a5e72ee43d33ce27dcd
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
      "id": 263,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-243",
      "html_url": "https://goskive.com/university/uni-243",
      "slug": "uni-243",
      "name": "University 180",
      "short_name": "Uni 243",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/413b5def4bed88f9f63a0d5839e3294a5bd30594.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/5e73efc036b435586cda65a67e0295a70dc6ec14.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T10:36:09.569Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 264,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-244",
      "html_url": "https://goskive.com/university/uni-244",
      "slug": "uni-244",
      "name": "University 181",
      "short_name": "Uni 244",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/53969b6bbf512f062775633ae2c14f12caba136c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d9b0cc5fc00ccb81b3f8708f33fe4ac850939f42.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T10:36:09.585Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 265,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-245",
      "html_url": "https://goskive.com/university/uni-245",
      "slug": "uni-245",
      "name": "University 182",
      "short_name": "Uni 245",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/7fe036f69ce9307e152486dce09ac33327ceeb41.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/456b35d509e4ad7b67a06dd445ec6d9f41e539f8.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T10:36:09.601Z",
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
	-H "Authorization: Bearer 2cf1fd1f42bc4c889846b2b321b0b2c4b20ae62ae3e64a5e72ee43d33ce27dcd"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer de8404c398ac619ec8fa95d441158d037457191cded5a4e56b188b7447bddaac
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
    "id": 261,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e4bb50eb413d47cf17f355195ac56378dee6d240.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/767c9157f9781019ae66ff2f08a71b97220ac778.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-26T10:36:09.402Z",
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
	-H "Authorization: Bearer de8404c398ac619ec8fa95d441158d037457191cded5a4e56b188b7447bddaac"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7bb651c3f5e5ab1648e759847552bc82564c603c8eee5514009029dd38038a23
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":15,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 32,
    "id": 13,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 13,
    "additional_university_ids": [

    ],
    "topic_id": 15,
    "discipline_id": 16,
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
    "chapters_updated_at": "2016-10-26T10:35:07.113Z",
    "updated_at": "2016-10-26T10:35:07.234Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 7,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-26T10:35:07.196Z",
        "course_id": 13,
        "author_id": 32,
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
        "id": 8,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-26T10:35:07.211Z",
        "course_id": 13,
        "author_id": 32,
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
        "id": 9,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-26T10:35:07.225Z",
        "course_id": 13,
        "author_id": 32,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":15,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7bb651c3f5e5ab1648e759847552bc82564c603c8eee5514009029dd38038a23"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d398d66932fe2abd167b0640a781ac660b0068851ac618338e58d0d7310c5bf4
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":14,"published":false}}
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
    "creator_id": 31,
    "id": 12,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 12,
    "additional_university_ids": [

    ],
    "topic_id": 14,
    "discipline_id": 15,
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
    "updated_at": "2016-10-26T10:35:07.083Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":14,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d398d66932fe2abd167b0640a781ac660b0068851ac618338e58d0d7310c5bf4"
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
      "creator_id": 35,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-6",
      "html_url": "https://goskive.com/course/fu-course-6",
      "slug": "fu-course-6",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 19,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
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
      "updated_at": "2016-10-26T10:35:07.528Z",
      "shortname": "fu-course-6"
    },
    {
      "creator_id": 35,
      "id": 18,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 21,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
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
      "chapters_updated_at": "2016-10-26T10:35:07.858Z",
      "updated_at": "2016-10-26T10:35:07.864Z",
      "shortname": "fu-course-7"
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
Authorization: Bearer ed4aeaad63d9523e788571ef42054b3c8fe365c6fcf2afc03e2a82889ed2fdc6
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
      "creator_id": 42,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-14",
      "html_url": "https://goskive.com/course/fu-course-14",
      "slug": "fu-course-14",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 27,
      "discipline_id": 28,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 14",
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
      "updated_at": "2016-10-26T10:35:08.291Z",
      "shortname": "fu-course-14"
    },
    {
      "creator_id": 42,
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 18,
      "additional_university_ids": [

      ],
      "topic_id": 28,
      "discipline_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
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
      "chapters_updated_at": "2016-10-26T10:35:08.567Z",
      "updated_at": "2016-10-26T10:35:08.573Z",
      "shortname": "fu-course-15"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed4aeaad63d9523e788571ef42054b3c8fe365c6fcf2afc03e2a82889ed2fdc6"
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
      "creator_id": 40,
      "id": 21,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-10",
      "html_url": "https://goskive.com/course/fu-course-10",
      "slug": "fu-course-10",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 23,
      "discipline_id": 24,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 10",
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
      "updated_at": "2016-10-26T10:35:08.031Z",
      "shortname": "fu-course-10"
    },
    {
      "creator_id": 40,
      "id": 22,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 24,
      "discipline_id": 25,
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
      "updated_at": "2016-10-26T10:35:08.066Z",
      "shortname": "fu-course-11"
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
Authorization: Bearer 24ac0c68872202f31440bfc12a3dbb1b484d61ec4b6f2c80055e4b69f042fed2
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
      "creator_id": 48,
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-18",
      "html_url": "https://goskive.com/course/fu-course-18",
      "slug": "fu-course-18",
      "university_id": 19,
      "additional_university_ids": [

      ],
      "topic_id": 31,
      "discipline_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 18",
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
      "updated_at": "2016-10-26T10:35:08.791Z",
      "shortname": "fu-course-18"
    },
    {
      "creator_id": 48,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 19,
      "additional_university_ids": [

      ],
      "topic_id": 32,
      "discipline_id": 33,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
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
      "updated_at": "2016-10-26T10:35:08.832Z",
      "shortname": "fu-course-19"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24ac0c68872202f31440bfc12a3dbb1b484d61ec4b6f2c80055e4b69f042fed2"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 5c89cfb1c07d14e88ae7f6bbcca73d77fe8db91ab459fb2041cb32e7e903c05d
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
  "id": 860,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-26T10:36:09.688Z",
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
	-H "Authorization: Bearer 5c89cfb1c07d14e88ae7f6bbcca73d77fe8db91ab459fb2041cb32e7e903c05d"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/254
Content-Type: application/json
Authorization: Bearer 4dc2d9c6e4d080c2714b68bf7d0e52e2296357f02626c9a293682b7610ee571e
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
    "id": 254,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 93,
    "fields_of_study": [
      121,
      122
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-26T10:35:22.274Z",
    "updated_at": "2016-10-26T10:35:22.274Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/254" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4dc2d9c6e4d080c2714b68bf7d0e52e2296357f02626c9a293682b7610ee571e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/256
Content-Type: application/json
Authorization: Bearer 50ea610eef4c1eb10da2e1a1ef70e16ac59085eae06da020ac893dda7bb3fe5e
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
    "id": 256,
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
    "created_at": "2016-10-26T10:35:22.353Z",
    "updated_at": "2016-10-26T10:35:22.353Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/256" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50ea610eef4c1eb10da2e1a1ef70e16ac59085eae06da020ac893dda7bb3fe5e"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/16
Content-Type: application/json
Authorization: Bearer 744c8e8d7b0ce743ec1eb4433f42be39ccb2d22d8b4da30a0177bf18b831403c
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
	-H "Authorization: Bearer 744c8e8d7b0ce743ec1eb4433f42be39ccb2d22d8b4da30a0177bf18b831403c"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/17
Content-Type: application/json
Authorization: Bearer eb0efd2fe37da6857338af0f1d50e522d939b5c43545c9b266e8f1f08ed70150
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
    "id": 17,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 118,
    "user_id": 879
  }
}
```



```shell
curl "api.goskive.com/v2/votes/17" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb0efd2fe37da6857338af0f1d50e522d939b5c43545c9b266e8f1f08ed70150"
```
