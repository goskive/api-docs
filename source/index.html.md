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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"af5476328fc8d20f6904debce66bfc622ae2d5a13c9b54590e6813f9bc5d866e","client_secret":"d00d53278ace38b21badaa0e8fa5d1d3f383b9cb6fdad7987178d31067ed2043"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"af5476328fc8d20f6904debce66bfc622ae2d5a13c9b54590e6813f9bc5d866e","client_secret":"d00d53278ace38b21badaa0e8fa5d1d3f383b9cb6fdad7987178d31067ed2043"}' -X POST \
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
Authorization: Basic NzNhNWJjZGQ1ZDc2OGI0ZDA2ZmI1ZDUwZjdiNTczMjJhOTc5NTQ2NGIxMWEz
MDcwOTUxNzc3Y2M1N2Q1ZTYzZjpkZWMyMjlkNTAyOGQ3M2VhZDBhZjEyNmY3
NmM0YmIzODNlMmU1N2IzZjJhNjZkYzU3ZGIwMDMwYTNkMTI2NDVi

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
	-u 73a5bcdd5d768b4d06fb5d50f7b57322a9795464b11a3070951777cc57d5e63f:dec229d5028d73ead0af126f76c4bb383e2e57b3f2a66dc57db0030a3d12645b
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
{"grant_type":"client_credentials","client_id":"0c8f31ecae996c5e680310f870de93cae1c5713fddbf689ebc91168128a72a39","client_secret":"aa094f2fc0445edc8673656c734d944ff0e8bace7b1f71c23bf327f99d6a9c49"}
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
  "access_token": "576ae8cf3431aebb2f5ffb97845196987998ce7ccb07eb1b61f3a3d5983096ec",
  "token_type": "bearer",
  "created_at": 1476782900
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"0c8f31ecae996c5e680310f870de93cae1c5713fddbf689ebc91168128a72a39","client_secret":"aa094f2fc0445edc8673656c734d944ff0e8bace7b1f71c23bf327f99d6a9c49"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"97ac32dad969a5ed67cf9be6b981f69f601e1cdf019c7166e316275017c9f965","client_secret":"c913f9c4473018fac53c52e2f31df912e1ac4bbf3ec78a3feccd687ed661a5b9"}
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
  "access_token": "b57385c562475de27f13e62c156271dc862af31c7931247e5de2d1390407fd46",
  "token_type": "bearer",
  "created_at": 1476782901
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"97ac32dad969a5ed67cf9be6b981f69f601e1cdf019c7166e316275017c9f965","client_secret":"c913f9c4473018fac53c52e2f31df912e1ac4bbf3ec78a3feccd687ed661a5b9"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTM2NTk5NjZlYzM1YTUzY2JjYTQ4ZGEzYzMwYzg4ZDIwZmY5YjJjNTU2YjRl
N2VlYTNlNGM5YWNlYTA4ZTc4ZTo0ZGMzNDNiZDkwMjVlMDY1ZjgxNjE5MGQ3
MWM1YTc3MDM5ZDM0Nzc2MzkzODA0OTE4YTM1YmQ5NzUzYWM3ZmYw

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
  "access_token": "30808869ad0a1da78423d3e07c7b6c0aeb44733bd8b5464913256d3022e4f82d",
  "token_type": "bearer",
  "created_at": 1476782901
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 93659966ec35a53cbca48da3c30c88d20ff9b2c556b4e7eea3e4c9acea08e78e:4dc343bd9025e065f816190d71c5a77039d34776393804918a35bd9753ac7ff0
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
Authorization: Bearer de35ab7c5002c056aed397f8a2327e1d3e7e1c32f8fa5f745381fe37701ac19f
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
    "company_id": 39,
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
	-H "Authorization: Bearer de35ab7c5002c056aed397f8a2327e1d3e7e1c32f8fa5f745381fe37701ac19f"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/7/flashcards
Content-Type: application/json
Authorization: Bearer 8b8e5513ce67ad90140e28dfa7cf94f188b196449cfac82d6b16b736185688db
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":7,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 7,
    "obfuscated_id": "XFkue8saGAM",
    "author_id": 25,
    "chapter_id": 7,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:27:38.021Z",
    "created_at": "2016-10-18T09:27:38.021Z",
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
curl "api.goskive.com/v2/chapters/7/flashcards" -d '{"flashcard":{"chapter_id":7,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b8e5513ce67ad90140e28dfa7cf94f188b196449cfac82d6b16b736185688db"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/5/flashcards
Content-Type: application/json
Authorization: Bearer d358637db9a8262d3bea9879637f73fa9361a90af4e1a091b3ce0a5295fae696
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
      "id": 4,
      "obfuscated_id": "SaV_gL1ycAY",
      "author_id": 17,
      "chapter_id": 5,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:27:37.581Z",
      "created_at": "2016-10-18T09:27:37.581Z",
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
      "author_id": 17,
      "chapter_id": 5,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:27:37.617Z",
      "created_at": "2016-10-18T09:27:37.617Z",
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
      "id": 6,
      "obfuscated_id": "eyxYPTvoIb8",
      "author_id": 17,
      "chapter_id": 5,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:27:37.653Z",
      "created_at": "2016-10-18T09:27:37.653Z",
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
curl "api.goskive.com/v2/chapters/5/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d358637db9a8262d3bea9879637f73fa9361a90af4e1a091b3ce0a5295fae696"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/106/questions
Content-Type: application/json
Authorization: Bearer 333178574e2d6f75fffa4dfee0ec3b12430109062904fe813c27523836761ca9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":106,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 102,
    "obfuscated_id": "jFy90P7ldB4",
    "author_id": 593,
    "chapter_id": 106,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:32.072Z",
    "created_at": "2016-10-18T09:28:32.072Z",
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
        "id": 204,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 205,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 206,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 207,
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
curl "api.goskive.com/v2/chapters/106/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":106,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 333178574e2d6f75fffa4dfee0ec3b12430109062904fe813c27523836761ca9"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/104/questions
Content-Type: application/json
Authorization: Bearer f647936279ff58574bd54f940b268e30b4733f1bbcc4e3a790fb67651bd67349
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":104,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 100,
    "obfuscated_id": "erXmBhoMZFI",
    "author_id": 587,
    "chapter_id": 104,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:31.251Z",
    "created_at": "2016-10-18T09:28:31.251Z",
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
        "id": 200,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 201,
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
curl "api.goskive.com/v2/chapters/104/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":104,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f647936279ff58574bd54f940b268e30b4733f1bbcc4e3a790fb67651bd67349"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/105/questions
Content-Type: application/json
Authorization: Bearer 8b0da600f8e27c286d597c905737f742549489d019562129c133bd96c8efc7e3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 101,
    "obfuscated_id": "PprZyBVq_gc",
    "author_id": 590,
    "chapter_id": 105,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:31.646Z",
    "created_at": "2016-10-18T09:28:31.646Z",
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
        "id": 202,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 203,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/105/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b0da600f8e27c286d597c905737f742549489d019562129c133bd96c8efc7e3"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/107/questions
Content-Type: application/json
Authorization: Bearer c1815706343038f30a2b74af28245b15eb6cf83a1504e3f5283ff4e80d1fd9c8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":107,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 103,
    "obfuscated_id": "AVhVflMAvL0",
    "author_id": 596,
    "chapter_id": 107,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:32.692Z",
    "created_at": "2016-10-18T09:28:32.692Z",
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
        "id": 208,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 209,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 210,
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
curl "api.goskive.com/v2/chapters/107/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":107,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1815706343038f30a2b74af28245b15eb6cf83a1504e3f5283ff4e80d1fd9c8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/108/questions
Content-Type: application/json
Authorization: Bearer 28c64e4fe8f9aae1c6723a10ff754884d6fc49d70234bcbccbded6eff9e22792
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
      "id": 104,
      "obfuscated_id": "nIg2bhYRjos",
      "author_id": 599,
      "chapter_id": 108,
      "position": 91,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:33.363Z",
      "created_at": "2016-10-18T09:28:33.186Z",
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
    },
    {
      "id": 105,
      "obfuscated_id": "3yX9LpVrF_M",
      "author_id": 600,
      "chapter_id": 108,
      "position": 92,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:33.617Z",
      "created_at": "2016-10-18T09:28:33.457Z",
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
          "id": 213,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 214,
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
      "author_id": 601,
      "chapter_id": 108,
      "position": 93,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T09:28:33.875Z",
      "created_at": "2016-10-18T09:28:33.711Z",
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
          "id": 215,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 216,
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
curl "api.goskive.com/v2/chapters/108/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28c64e4fe8f9aae1c6723a10ff754884d6fc49d70234bcbccbded6eff9e22792"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/113
Content-Type: application/json
Authorization: Bearer e473f2db3d1396192843298b2c03d26ab13a42ebe53231d8231bc2e74c787f55
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
curl "api.goskive.com/v2/chapters/113" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e473f2db3d1396192843298b2c03d26ab13a42ebe53231d8231bc2e74c787f55"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/115
Content-Type: application/json
Authorization: Bearer 56b39418ea7d7e407f9a45fb63e581b8632a84d224b849224da3fa0411f9854d
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
curl "api.goskive.com/v2/chapters/115" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56b39418ea7d7e407f9a45fb63e581b8632a84d224b849224da3fa0411f9854d"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/112
Content-Type: application/json
Authorization: Bearer 382d0822394582bbb32b45deafa581916e185271fd6ee785d8b2dc228521c672
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
curl "api.goskive.com/v2/chapters/112" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 382d0822394582bbb32b45deafa581916e185271fd6ee785d8b2dc228521c672"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/116
Content-Type: application/json
Authorization: Bearer 366ed819bdf50fb55e89bbacc52b45a0fcd3434c47d9e1d992a6ad599bf657c9
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/116" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 366ed819bdf50fb55e89bbacc52b45a0fcd3434c47d9e1d992a6ad599bf657c9"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/118
Content-Type: application/json
Authorization: Bearer 9917b948d4493fa6f8a3db5b5e473e048baee498782a9e383d160871934e8349
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
    "id": 118,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T09:28:37.324Z",
    "course_id": 216,
    "author_id": 634,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-18T09:28:36.634Z",
    "questions_updated_at": "2016-10-18T09:28:36.634Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 638,
        "chapter_id": 118,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:37.300Z",
        "created_at": "2016-10-18T09:28:37.300Z",
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
        "id": 112,
        "obfuscated_id": "7Qwj1ZvbWUI",
        "author_id": 636,
        "chapter_id": 118,
        "position": 99,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:28:37.165Z",
        "created_at": "2016-10-18T09:28:36.997Z",
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
}
```



```shell
curl "api.goskive.com/v2/chapters/118" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9917b948d4493fa6f8a3db5b5e473e048baee498782a9e383d160871934e8349"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/110
Content-Type: application/json
Authorization: Bearer ca6627e7a29beef4bb7fa11c34f2c88609b4112592e89485f7c78d8da8f072fa
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
    "id": 110,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T09:28:34.399Z",
    "course_id": 208,
    "author_id": 607,
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
curl "api.goskive.com/v2/chapters/110" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca6627e7a29beef4bb7fa11c34f2c88609b4112592e89485f7c78d8da8f072fa"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/49/replies
Content-Type: application/json
Authorization: Bearer 61d9be153c6204ab0dc9202637e3676f4d7e5b35ad60e9b55d4ab81168434b6c
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
    "author_id": 691,
    "reply_to_id": 49,
    "created_at": "2016-10-18T09:28:42.789Z",
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
	-H "Authorization: Bearer 61d9be153c6204ab0dc9202637e3676f4d7e5b35ad60e9b55d4ab81168434b6c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/48/replies
Content-Type: application/json
Authorization: Bearer 89185c70579f4ceac3d7a7f18a51e32e537387abe3ff6c4748c63adef185679d
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
curl "api.goskive.com/v2/comments/48/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89185c70579f4ceac3d7a7f18a51e32e537387abe3ff6c4748c63adef185679d"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer 5dacd37b278d69dce43a73675717b59de3d4bab35bc8edf68e4fd34206d95cb5
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
curl "api.goskive.com/v2/comments/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5dacd37b278d69dce43a73675717b59de3d4bab35bc8edf68e4fd34206d95cb5"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/40/republish
Content-Type: application/json
Authorization: Bearer 8b0d9a46f9fa02d02639792bdd25f7621b896c3d62dfcbbdf2663efca5c74053
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
curl "api.goskive.com/v2/comments/40/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b0d9a46f9fa02d02639792bdd25f7621b896c3d62dfcbbdf2663efca5c74053"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 33885c68cda433b661840f2fe8429a81b8afc43a59dc2cfbf8e0525b985951fe
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
	-H "Authorization: Bearer 33885c68cda433b661840f2fe8429a81b8afc43a59dc2cfbf8e0525b985951fe"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/41/report
Content-Type: application/json
Authorization: Bearer 314579090365dd6bdd0b5eec901c981dac5008209bbe4643cea6f7e7898f1ed6
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
	-H "Authorization: Bearer 314579090365dd6bdd0b5eec901c981dac5008209bbe4643cea6f7e7898f1ed6"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/16
Content-Type: application/json
Authorization: Bearer 08ecec5f760312acbbd1db0c27153a5d8d71ebd19102eae192767daa4a6b9347
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
    "id": 16,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-18T09:27:45.239Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08ecec5f760312acbbd1db0c27153a5d8d71ebd19102eae192767daa4a6b9347"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f8d8689346d2accd24aa5f0e24dbd534fa7291cc039dbb1cd742e1cab0924411
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
      "id": 13,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:27:45.179Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:27:45.183Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T09:27:45.187Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8d8689346d2accd24aa5f0e24dbd534fa7291cc039dbb1cd742e1cab0924411"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer dcfa7763eec91dbd30be39bec405539dff8635438b61926f6ddd1e17522d10b9
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
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcfa7763eec91dbd30be39bec405539dff8635438b61926f6ddd1e17522d10b9"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/28/company_profiles
Content-Type: application/json
Authorization: Bearer 974e62b42dc8b74db49599cfd60c89024d7c5efa096eaedc0999bea3c188c9ba
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
curl "api.goskive.com/v2/companies/28/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 974e62b42dc8b74db49599cfd60c89024d7c5efa096eaedc0999bea3c188c9ba"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer df358ed217ddd7aa1da23bbffb384f56b3f92f59746d7a3de01f80729f28e37d
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
	-H "Authorization: Bearer df358ed217ddd7aa1da23bbffb384f56b3f92f59746d7a3de01f80729f28e37d"
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
Authorization: Bearer 992d5a2d0254e3032769e735d4fe5ce7dc010d03765b17af26524c8323c44776
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
	-H "Authorization: Bearer 992d5a2d0254e3032769e735d4fe5ce7dc010d03765b17af26524c8323c44776"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e5ba7df732faf8ed13b1f33b530a884c75ef00f86b980b09d09bfd1e1159a70a
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
    "id": 167,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T09:28:55.405Z",
    "course_id": 282,
    "author_id": 874,
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
	-H "Authorization: Bearer e5ba7df732faf8ed13b1f33b530a884c75ef00f86b980b09d09bfd1e1159a70a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 128e404e85b85afeaf2c8a8bfca852967510e8bf59bd27fcfa0719bf2944f9d0
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
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-18T09:28:56.099Z",
      "course_id": 287,
      "author_id": 887,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 173,
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-18T09:28:56.130Z",
      "course_id": 287,
      "author_id": 888,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 174,
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-18T09:28:56.487Z",
      "course_id": 287,
      "author_id": 889,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T09:28:56.022Z",
      "questions_updated_at": "2016-10-18T09:28:56.022Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 128e404e85b85afeaf2c8a8bfca852967510e8bf59bd27fcfa0719bf2944f9d0"
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
      "id": 178,
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-18T09:28:57.002Z",
      "course_id": 290,
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
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-18T09:28:57.035Z",
      "course_id": 290,
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
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-18T09:28:57.406Z",
      "course_id": 290,
      "author_id": 903,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T09:28:56.919Z",
      "questions_updated_at": "2016-10-18T09:28:56.919Z",
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
Authorization: Bearer 31633ec88a8e1f967c9f9272d0f1bf8cb533f155a7067e191046cafbe0d08493
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-18T09:28:56.751Z",
      "course_id": 289,
      "author_id": 896,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 176,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-18T09:28:56.780Z",
      "course_id": 289,
      "author_id": 897,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 177,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-18T09:28:56.810Z",
      "course_id": 289,
      "author_id": 898,
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
	-H "Authorization: Bearer 31633ec88a8e1f967c9f9272d0f1bf8cb533f155a7067e191046cafbe0d08493"
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
      "id": 181,
      "title": "Clever Chapter Title 157",
      "position": 1,
      "updated_at": "2016-10-18T09:28:57.536Z",
      "course_id": 291,
      "author_id": 907,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 182,
      "title": "Clever Chapter Title 158",
      "position": 2,
      "updated_at": "2016-10-18T09:28:57.565Z",
      "course_id": 291,
      "author_id": 908,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 183,
      "title": "Clever Chapter Title 159",
      "position": 3,
      "updated_at": "2016-10-18T09:28:57.593Z",
      "course_id": 291,
      "author_id": 909,
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
Authorization: Bearer 84b149ee8c8b222abca1ab38436bfd5de648fc2722b19f763a800c72ed70a36e
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
    "course_id": 302,
    "user_id": 949,
    "updated_at": "2016-10-18T09:29:01.145Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84b149ee8c8b222abca1ab38436bfd5de648fc2722b19f763a800c72ed70a36e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 605f6d27a9ec0c6f798a55f3175ba28b8a277f1a0e1b29df5e7b28ebf365d70b
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
      "course_id": 306,
      "user_id": 959,
      "updated_at": "2016-10-18T09:29:01.637Z"
    },
    {
      "id": 7,
      "course_id": 306,
      "user_id": 960,
      "updated_at": "2016-10-18T09:29:01.653Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 605f6d27a9ec0c6f798a55f3175ba28b8a277f1a0e1b29df5e7b28ebf365d70b"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/133/files
Content-Type: application/json
Authorization: Bearer 3a108a6cfec77b69a930f61f66cff9b58d3cbb51b8c81d0d0035ab25b69bb558
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
      "id": 1,
      "uploader": {
        "id": 300,
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
        "created_at": "2016-10-18T09:28:02.674Z",
        "updated_at": "2016-10-18T09:28:02.674Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:28:02.688Z",
      "updated_at": "2016-10-18T09:28:02.688Z",
      "course_id": 133,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 301,
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
        "created_at": "2016-10-18T09:28:02.697Z",
        "updated_at": "2016-10-18T09:28:02.697Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:28:02.705Z",
      "updated_at": "2016-10-18T09:28:02.705Z",
      "course_id": 133,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 302,
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
        "created_at": "2016-10-18T09:28:02.712Z",
        "updated_at": "2016-10-18T09:28:02.712Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T09:28:02.719Z",
      "updated_at": "2016-10-18T09:28:02.719Z",
      "course_id": 133,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/133/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a108a6cfec77b69a930f61f66cff9b58d3cbb51b8c81d0d0035ab25b69bb558"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/135/files
Content-Type: application/json
Authorization: Bearer 691ccce0062f26e61e349ff98a05390f543818133e3853d08141ee50ff926626
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
    "id": 4,
    "uploader": {
      "id": 307,
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
      "created_at": "2016-10-18T09:28:02.978Z",
      "updated_at": "2016-10-18T09:28:02.978Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-18T09:28:03.006Z",
    "updated_at": "2016-10-18T09:28:03.006Z",
    "course_id": 135,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/135/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 691ccce0062f26e61e349ff98a05390f543818133e3853d08141ee50ff926626"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/132/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 08bcad5ede6e5cf0fd44c044eb462710f94af524e668f3bc5e7e5915cdc7d5bf
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
    "key": "cache/3ea333416302b8847255afe530267db9.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMDoyODowMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8zZWEzMzM0MTYzMDJiODg0NzI1NWFmZTUzMDI2N2RiOS5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMThUMDkyODAyWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T092802Z",
    "x-amz-signature": "6f932f186316b54754c054f9985524e1e8c2afafb49206f1772856a7a73b959d"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/132/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08bcad5ede6e5cf0fd44c044eb462710f94af524e668f3bc5e7e5915cdc7d5bf"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer a8614d13979e4231238c84a38445b5b409a0e0e76ec6407b38ee5740b41b2616
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
	-H "Authorization: Bearer a8614d13979e4231238c84a38445b5b409a0e0e76ec6407b38ee5740b41b2616"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7a2f0ec090732996974e97fcd2b022d552968b310c8c5203c5f0d97ce2e8141e
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
	-H "Authorization: Bearer 7a2f0ec090732996974e97fcd2b022d552968b310c8c5203c5f0d97ce2e8141e"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 731fdde06018ca25539cede70f8a9da93c4a6948186e8890497e11fb5f1ec849
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
	-H "Authorization: Bearer 731fdde06018ca25539cede70f8a9da93c4a6948186e8890497e11fb5f1ec849"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5c8f9ed4347d56018da3ce16303d935c8faac56ad147f132d815f899d51e9709
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
	-H "Authorization: Bearer 5c8f9ed4347d56018da3ce16303d935c8faac56ad147f132d815f899d51e9709"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d105fc8061396cf62f76817ca811557ed7ecb3c15ba9d4bdfdda38c2d4aea9c0
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
	-H "Authorization: Bearer d105fc8061396cf62f76817ca811557ed7ecb3c15ba9d4bdfdda38c2d4aea9c0"
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
    "creator_id": 217,
    "id": 108,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 88,
    "additional_university_ids": [

    ],
    "topic_id": 110,
    "discipline_id": 110,
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
    "chapters_updated_at": "2016-10-18T09:27:51.457Z",
    "updated_at": "2016-10-18T09:27:52.942Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 21,
        "title": "Clever Chapter Title 15",
        "position": 1,
        "updated_at": "2016-10-18T09:27:52.893Z",
        "course_id": 108,
        "author_id": 217,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:27:51.457Z",
        "questions_updated_at": "2016-10-18T09:27:51.457Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 22,
        "title": "Clever Chapter Title 16",
        "position": 2,
        "updated_at": "2016-10-18T09:27:52.934Z",
        "course_id": 108,
        "author_id": 217,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:27:51.457Z",
        "questions_updated_at": "2016-10-18T09:27:51.457Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 217,
        "chapter_id": 21,
        "position": 12,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:51.668Z",
        "created_at": "2016-10-18T09:27:51.546Z",
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
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 217,
        "chapter_id": 22,
        "position": 14,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:52.058Z",
        "created_at": "2016-10-18T09:27:51.930Z",
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
            "id": 27,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 28,
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
Authorization: Bearer 5163da46b28e5d3ffe2676d72abf5ec7e405508a6dd2b265a0b1262918479041
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
    "creator_id": 228,
    "id": 110,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 90,
    "additional_university_ids": [

    ],
    "topic_id": 112,
    "discipline_id": 112,
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
    "chapters_updated_at": "2016-10-18T09:27:54.646Z",
    "updated_at": "2016-10-18T09:27:56.235Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 25,
        "title": "Clever Chapter Title 19",
        "position": 1,
        "updated_at": "2016-10-18T09:27:56.187Z",
        "course_id": 110,
        "author_id": 228,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:27:54.646Z",
        "questions_updated_at": "2016-10-18T09:27:54.646Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 26,
        "title": "Clever Chapter Title 20",
        "position": 2,
        "updated_at": "2016-10-18T09:27:56.227Z",
        "course_id": 110,
        "author_id": 228,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T09:27:54.646Z",
        "questions_updated_at": "2016-10-18T09:27:54.646Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 229,
        "chapter_id": 25,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:56.014Z",
        "created_at": "2016-10-18T09:27:56.014Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 229,
        "chapter_id": 26,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:56.090Z",
        "created_at": "2016-10-18T09:27:56.090Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 229,
        "chapter_id": 25,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:56.058Z",
        "created_at": "2016-10-18T09:27:56.058Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 229,
        "chapter_id": 26,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:56.134Z",
        "created_at": "2016-10-18T09:27:56.134Z",
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
        "author_id": 229,
        "chapter_id": 25,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:54.875Z",
        "created_at": "2016-10-18T09:27:54.746Z",
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
        "author_id": 229,
        "chapter_id": 25,
        "position": 25,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:55.068Z",
        "created_at": "2016-10-18T09:27:54.946Z",
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
        "author_id": 229,
        "chapter_id": 26,
        "position": 26,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:55.303Z",
        "created_at": "2016-10-18T09:27:55.159Z",
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
        "author_id": 229,
        "chapter_id": 26,
        "position": 27,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T09:27:55.512Z",
        "created_at": "2016-10-18T09:27:55.381Z",
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
	-H "Authorization: Bearer 5163da46b28e5d3ffe2676d72abf5ec7e405508a6dd2b265a0b1262918479041"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/122/pin
Content-Type: application/json
Authorization: Bearer e6b0dd18423ac488065a68e7aa5a4faecb47f8a65f0aa1dbe370c33b329ba403
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/122/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6b0dd18423ac488065a68e7aa5a4faecb47f8a65f0aa1dbe370c33b329ba403"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/112/pin
Content-Type: application/json
Authorization: Bearer bf22b1e42f6bcfadd64667ee83ca8c9de35f5d2ec9d8d6a3b93456655eefa462
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/112/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf22b1e42f6bcfadd64667ee83ca8c9de35f5d2ec9d8d6a3b93456655eefa462"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5d0c23dfc5e48de0a1fde52ed8d5fd68c96144752a4a9325c5be68bd37a34d70
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
    "creator_id": 212,
    "id": 105,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 85,
    "additional_university_ids": [

    ],
    "topic_id": 107,
    "discipline_id": 107,
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
    "updated_at": "2016-10-18T09:27:51.195Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d0c23dfc5e48de0a1fde52ed8d5fd68c96144752a4a9325c5be68bd37a34d70"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 2ea9df5b35e6cc2954942e436215c9c7a48b27457f81e7901279c5ebf049ccdb
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
    "id": 432,
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
    "created_at": "2016-10-18T09:28:16.689Z",
    "updated_at": "2016-10-18T09:28:16.689Z",
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
	-H "Authorization: Bearer 2ea9df5b35e6cc2954942e436215c9c7a48b27457f81e7901279c5ebf049ccdb"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b6914244485ae7e3b8419985b4e2920cf677dd64b48dc59b2683d13fdbed9949
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[171]}
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
    "id": 427,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      171
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:28:16.120Z",
    "updated_at": "2016-10-18T09:28:16.173Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[171]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6914244485ae7e3b8419985b4e2920cf677dd64b48dc59b2683d13fdbed9949"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ecb39767ac120f0f43bdfed71cdf9d90ab760aa29058caa51fc00313f4fbe800
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
    "id": 429,
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
    "created_at": "2016-10-18T09:28:16.280Z",
    "updated_at": "2016-10-18T09:28:16.280Z",
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
	-H "Authorization: Bearer ecb39767ac120f0f43bdfed71cdf9d90ab760aa29058caa51fc00313f4fbe800"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1e49d871da32d57601966e13ed421a67b70f300596e494ad82ace98d8b55f7e5
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[174]}
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
    "id": 430,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      174
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:28:16.375Z",
    "updated_at": "2016-10-18T09:28:16.375Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[174]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e49d871da32d57601966e13ed421a67b70f300596e494ad82ace98d8b55f7e5"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 8ec4263d8d2911c3b6787f4c427db11335215b6dd0dcbf10e792b5a65c46a521
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

175
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
    "id": 431,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/12a5f5ca5088899ee60a5c21a3f397c84ac416c6.jpg",
    "university_id": null,
    "fields_of_study": [
      175
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T09:28:16.446Z",
    "updated_at": "2016-10-18T09:28:16.660Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/aed753a9547670d6ac6b7a16a17be1c5e820657f.jpg",
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

175
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 8ec4263d8d2911c3b6787f4c427db11335215b6dd0dcbf10e792b5a65c46a521"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 6badf0ab227e4d668fa6318cc6da6610854dd6f90bd1b76e62f1162071b8b7d3
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
      "bookmarkable_id": 123,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 124,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 125,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6badf0ab227e4d668fa6318cc6da6610854dd6f90bd1b76e62f1162071b8b7d3"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 9ef787988e97e3b4ae8a17b3fc2c6ffc2ae421d57d2160a50cce7449a6895657
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
      "company_id": 24,
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
      "company_id": 25,
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
	-H "Authorization: Bearer 9ef787988e97e3b4ae8a17b3fc2c6ffc2ae421d57d2160a50cce7449a6895657"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 83cfc340f7833585f987eb4579a7251deddf0e028075e81fb40153a30060644a
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
      "company_id": 20,
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
	-H "Authorization: Bearer 83cfc340f7833585f987eb4579a7251deddf0e028075e81fb40153a30060644a"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer ac4dc17716c41381e80b27cbc1a038be9b8578502c8af2270118647c7bf4247d
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
      "creator_id": 866,
      "id": 278,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-227",
      "html_url": "https://goskive.com/course/mit-course-227",
      "slug": "mit-course-227",
      "university_id": 263,
      "additional_university_ids": [

      ],
      "topic_id": 290,
      "discipline_id": 291,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 227",
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
      "updated_at": "2016-10-18T09:28:54.843Z",
      "shortname": "mit-course-227"
    },
    {
      "creator_id": 867,
      "id": 279,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-228",
      "html_url": "https://goskive.com/course/mit-course-228",
      "slug": "mit-course-228",
      "university_id": 264,
      "additional_university_ids": [

      ],
      "topic_id": 291,
      "discipline_id": 292,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 228",
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
      "updated_at": "2016-10-18T09:28:54.927Z",
      "shortname": "mit-course-228"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac4dc17716c41381e80b27cbc1a038be9b8578502c8af2270118647c7bf4247d"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8c6cb192a10672eb5a2398e624df5377ab24c6731a0f4f58b37e7514def881af
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
      "company_id": 36,
      "company": {
        "id": 36,
        "name": "Fake Company Name 32",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T09:28:58.822Z"
      },
      "created_at": "2016-10-18T09:28:58.825Z",
      "updated_at": "2016-10-18T09:28:58.825Z",
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
      "company_id": 37,
      "company": {
        "id": 37,
        "name": "Fake Company Name 33",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T09:28:58.833Z"
      },
      "created_at": "2016-10-18T09:28:58.837Z",
      "updated_at": "2016-10-18T09:28:58.837Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c6cb192a10672eb5a2398e624df5377ab24c6731a0f4f58b37e7514def881af"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 0fb6ceccbcec95db7144bc155eb5769014e0d370c73a981ea7e1bbd0ab97df0e
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
      "company_id": 32,
      "company": {
        "id": 32,
        "name": "Fake Company Name 28",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/4827d71e510ab6acd29eb9520c31ac72b53161f6.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T09:28:58.616Z"
      },
      "created_at": "2016-10-18T09:28:58.620Z",
      "updated_at": "2016-10-18T09:28:58.620Z",
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
      "company_id": 33,
      "company": {
        "id": 33,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T09:28:58.633Z"
      },
      "created_at": "2016-10-18T09:28:58.637Z",
      "updated_at": "2016-10-18T09:28:58.637Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fb6ceccbcec95db7144bc155eb5769014e0d370c73a981ea7e1bbd0ab97df0e"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 8154480a225bdaab00490b14a4edf14bd5431bc9cb2da8b2bb21e3efa5bf8cd2
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
      "created_at": "2016-10-18T09:28:00.247Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 43,
      "updated_at": "2016-10-18T09:28:00.357Z",
      "author_id": "270",
      "thread_subject_id": "124",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 5,
      "created_at": "2016-10-18T09:28:00.345Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 44,
      "updated_at": "2016-10-18T09:28:00.360Z",
      "author_id": "273",
      "thread_subject_id": "125",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-18T09:28:00.735Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-18T09:28:00.735Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-18T09:28:01.109Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-10-18T09:28:01.109Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 8,
      "created_at": "2016-10-18T09:28:01.501Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-18T09:28:01.501Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 9,
      "created_at": "2016-10-18T09:28:01.803Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 41,
      "updated_at": "2016-10-18T09:28:01.803Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-18T09:28:02.107Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 42,
      "updated_at": "2016-10-18T09:28:02.107Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-18T09:28:02.405Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 43,
      "updated_at": "2016-10-18T09:28:02.405Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8154480a225bdaab00490b14a4edf14bd5431bc9cb2da8b2bb21e3efa5bf8cd2"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/3
Content-Type: application/json
Authorization: Bearer 1b6adc02020d30984f633666671c26a6e5d9d057f2f62c2d0ee0b4623b52e7d1
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-18T09:17:59.000Z"}}
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
    "id": 3,
    "created_at": "2016-10-18T09:28:00.072Z",
    "read_at": "2016-10-18T09:17:59.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 42,
    "updated_at": "2016-10-18T09:28:00.136Z",
    "author_id": "266",
    "thread_subject_id": "123",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/3" -d '{"notification":{"read_at":"2016-10-18T09:17:59.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b6adc02020d30984f633666671c26a6e5d9d057f2f62c2d0ee0b4623b52e7d1"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 20cc19a1f5ba64264c13856288c82ed9501dd3dcd44e27d31ac3ca754a8f651f
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
      "course_id": 225,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T09:28:41.275Z",
      "course_published": true,
      "updated_at": "2016-10-18T09:28:41.266Z"
    },
    {
      "id": 4,
      "course_id": 226,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T09:28:41.361Z",
      "course_published": true,
      "updated_at": "2016-10-18T09:28:41.352Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20cc19a1f5ba64264c13856288c82ed9501dd3dcd44e27d31ac3ca754a8f651f"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer daf26f42e817ef9ead6f04e109f98c472be56de91138b1159e30ad23b55d3e71
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
    "course_id": 228,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T09:28:41.668Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:28:41.659Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daf26f42e817ef9ead6f04e109f98c472be56de91138b1159e30ad23b55d3e71"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 6c0f946d4e7215662f05245051031a2a59f4f1b4df4fcf552c2eec9bafc7969c
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
    "course_id": 227,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-18T09:28:41.569Z",
    "course_published": true,
    "updated_at": "2016-10-18T09:28:41.556Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c0f946d4e7215662f05245051031a2a59f4f1b4df4fcf552c2eec9bafc7969c"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 8b35edc616d6adbcf43d0aedf047d3d9525afe71652b9abe0273a3e6f398e3d8
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
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 77,
      "user_id": 434
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 78,
      "user_id": 434
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 79,
      "user_id": 434
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 80,
      "user_id": 434
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b35edc616d6adbcf43d0aedf047d3d9525afe71652b9abe0273a3e6f398e3d8"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/215
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
    "id": 215,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 215,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 215
      },
      {
        "id": 216,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 215
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/215" -X GET \
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
      "id": 216,
      "name": "Stand-alone motivating complexity",
      "name_translations": {
        "en": "Stand-alone motivating complexity"
      }
    },
    {
      "id": 217,
      "name": "Object-based content-based infrastructure",
      "name_translations": {
        "en": "Object-based content-based infrastructure"
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
Authorization: Bearer d875ad1c0b641d4f269dd28f92582cc621b6b6e232a782f6bda35f84d920a33b
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
    "user_id": 481,
    "feedbackable_id": 43,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-18T09:28:22.866Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/14/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d875ad1c0b641d4f269dd28f92582cc621b6b6e232a782f6bda35f84d920a33b"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer 6cd480084139bdc4f5b4ad5d4ed427b0289494e827e9b2c60fc0d0b1eea38ba8
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
    "user_id": 471,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-18T09:28:22.155Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cd480084139bdc4f5b4ad5d4ed427b0289494e827e9b2c60fc0d0b1eea38ba8"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/16
Content-Type: application/json
Authorization: Bearer e6cdc1a1ac14ff457a1f556e6fa79e5a7cdd03518b795ca5ad77b5b5d1a43215
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
    "id": 16,
    "user_id": 491,
    "feedbackable_id": 45,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:28:23.367Z",
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
curl "api.goskive.com/v2/feedbacks/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6cdc1a1ac14ff457a1f556e6fa79e5a7cdd03518b795ca5ad77b5b5d1a43215"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/9/fix
Content-Type: application/json
Authorization: Bearer 92ad73b27363ec857ce0250e040b2f4952c70cbab936ef1291359396a7470a7c
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
curl "api.goskive.com/v2/feedbacks/9/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92ad73b27363ec857ce0250e040b2f4952c70cbab936ef1291359396a7470a7c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/10/fix
Content-Type: application/json
Authorization: Bearer 7c231bba84a601e4fc4db2fe012779729f2b654a6966591a9587ddcec677bc50
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
curl "api.goskive.com/v2/feedbacks/10/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c231bba84a601e4fc4db2fe012779729f2b654a6966591a9587ddcec677bc50"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/15/close
Content-Type: application/json
Authorization: Bearer 285c8e99ce74bb286f22441385ac170225efd0ef12eb503f982650ea412a475f
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
curl "api.goskive.com/v2/feedbacks/15/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 285c8e99ce74bb286f22441385ac170225efd0ef12eb503f982650ea412a475f"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/17
Content-Type: application/json
Authorization: Bearer ec80b2c589185c04dc1f0c96d142f93d21f694663cadce541438377b99e22740
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
    "id": 17,
    "user_id": 496,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:28:23.660Z",
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
curl "api.goskive.com/v2/feedbacks/17" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec80b2c589185c04dc1f0c96d142f93d21f694663cadce541438377b99e22740"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/10
Authorization: Bearer 987b3edf57e090cc5294acfcaf4585c47c9b15b0ebdfad0a9c4374fef937088e
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
	-H "Authorization: Bearer 987b3edf57e090cc5294acfcaf4585c47c9b15b0ebdfad0a9c4374fef937088e" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Authorization: Bearer ce509cea04f87d97e43ab25c31bec8e2ce87072ee1f63a992da11873bdd789fe
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
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Authorization: Bearer ce509cea04f87d97e43ab25c31bec8e2ce87072ee1f63a992da11873bdd789fe" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/7
Authorization: Bearer 8ad9c621e7ecd2a94cfc0a483c4b0610c98ee750d3b4d081d9190ba5a85793fb
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/ceab344c9c076b03705022dc62f7e2e1.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T092845Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=480e88966e0afdb1eb01374a2bf12f5dfe792ee3a61991cb24c203594c43aaa8"
  }
}
```



```shell
curl "api.goskive.com/v2/files/7" -X GET \
	-H "Authorization: Bearer 8ad9c621e7ecd2a94cfc0a483c4b0610c98ee750d3b4d081d9190ba5a85793fb"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Authorization: Bearer 4d227bf98176d40e5d18b55e34ec8c43144d565a538889b01a5d049810c86fd4
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
      "id": 728,
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
      "created_at": "2016-10-18T09:28:46.546Z",
      "updated_at": "2016-10-18T09:28:46.546Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-18T09:28:46.616Z",
    "updated_at": "2016-10-18T09:28:46.616Z",
    "course_id": 240,
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
	-H "Authorization: Bearer 4d227bf98176d40e5d18b55e34ec8c43144d565a538889b01a5d049810c86fd4" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/6/matched_courses?required_cu_count=2
Authorization: Bearer 90b5043e82cc04c293ed9c7435b1efede71705100bfb71f64c23d789fcd42f24
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
      "creator_id": 656,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 205,
      "additional_university_ids": [

      ],
      "topic_id": 229,
      "discipline_id": 230,
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
      "chapters_updated_at": "2016-10-18T09:28:37.986Z",
      "updated_at": "2016-10-18T09:28:40.059Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 661,
      "id": 221,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-4277034c-4923-4b86-9fe3-4b0aaeebe8e4",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-4277034c-4923-4b86-9fe3-4b0aaeebe8e4",
      "slug": "mit-the-great-british-bake-off-4277034c-4923-4b86-9fe3-4b0aaeebe8e4",
      "university_id": 206,
      "additional_university_ids": [

      ],
      "topic_id": 230,
      "discipline_id": 231,
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
      "chapters_updated_at": "2016-10-18T09:28:37.986Z",
      "updated_at": "2016-10-18T09:28:40.762Z",
      "shortname": "mit-the-great-british-bake-off-4277034c-4923-4b86-9fe3-4b0aaeebe8e4"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/6/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 90b5043e82cc04c293ed9c7435b1efede71705100bfb71f64c23d789fcd42f24"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/8/preview
Authorization: Bearer 6d96d134829f29d7526e0e0183fabca2f2df8fcddbd7f913de30d998c7a8782f
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/fa51e7e830bd9aae2c89a48fef51aec2.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T092846Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=2c98b9f7a0e84d7a740dc2e2ec5c64e113ede45b1c557fa1293e51924d5c26d2"
  }
}
```



```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Authorization: Bearer 6d96d134829f29d7526e0e0183fabca2f2df8fcddbd7f913de30d998c7a8782f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/12/report
Authorization: Bearer 689e04051bfe7a0fe33a222965add75d6e7d69b1001baa02186df3a0890b6949
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
	-H "Authorization: Bearer 689e04051bfe7a0fe33a222965add75d6e7d69b1001baa02186df3a0890b6949" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/90/comments
Content-Type: application/json
Authorization: Bearer 0b8710811617628ec860dd28f6a37c4eafbcdbfb51a12a1693c1e386f75a8f8c
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
    "id": 56,
    "author_id": 858,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:28:54.336Z",
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
curl "api.goskive.com/v2/flashcards/90/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b8710811617628ec860dd28f6a37c4eafbcdbfb51a12a1693c1e386f75a8f8c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/89/comments
Content-Type: application/json
Authorization: Bearer ba280d2705d706edf4d23ef94ed6c5572bd9b3a47c47e782cad611ef05221c95
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
    "id": 55,
    "author_id": 855,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:28:54.002Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 45,
      "user_id": 855,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:53.999Z",
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
curl "api.goskive.com/v2/flashcards/89/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba280d2705d706edf4d23ef94ed6c5572bd9b3a47c47e782cad611ef05221c95"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/87/comments
Content-Type: application/json
Authorization: Bearer 217ec023d5146a5debc5ffa38a5cf4edad982fe8bcc172767a9b18975bebdfd2
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
      "id": 54,
      "author_id": 851,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:28:53.587Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 850,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:28:53.571Z",
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
curl "api.goskive.com/v2/flashcards/87/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 217ec023d5146a5debc5ffa38a5cf4edad982fe8bcc172767a9b18975bebdfd2"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/91/comments
Content-Type: application/json
Authorization: Bearer 44df6ae17bce1a0951b77cb9a8cfd26b3545635f161ee5f08809013eb00e8780
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
curl "api.goskive.com/v2/flashcards/91/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44df6ae17bce1a0951b77cb9a8cfd26b3545635f161ee5f08809013eb00e8780"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/80/feedbacks
Content-Type: application/json
Authorization: Bearer 3f50d22c76e1dcdb07c55562f14a15a115d4481ccdfeffce8aa0e64f21947365
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
    "id": 38,
    "user_id": 814,
    "feedbackable_id": 80,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:28:51.981Z",
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
curl "api.goskive.com/v2/flashcards/80/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f50d22c76e1dcdb07c55562f14a15a115d4481ccdfeffce8aa0e64f21947365"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/82/feedbacks
Content-Type: application/json
Authorization: Bearer d93e77f7d2637a5ad5be0b83a5ffdb85f803615b27e4e115731b9d152aa65b7d
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
      "id": 40,
      "user_id": 824,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:52.514Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 823,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:52.501Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d93e77f7d2637a5ad5be0b83a5ffdb85f803615b27e4e115731b9d152aa65b7d"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/3/votes
Content-Type: application/json
Authorization: Bearer 4860793c76740eb0fb7a44f090da75714ca3238af9571de92654dc2e30d6e236
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
      "votable_id": 3,
      "user_id": 16
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 3,
      "user_id": 15
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 3,
      "user_id": 14
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4860793c76740eb0fb7a44f090da75714ca3238af9571de92654dc2e30d6e236"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/76/republish
Content-Type: application/json
Authorization: Bearer 266f78d8aa8e630ccd42054ba286d48a7ab351135e7dfab07f1de416badd09c9
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
curl "api.goskive.com/v2/flashcards/76/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 266f78d8aa8e630ccd42054ba286d48a7ab351135e7dfab07f1de416badd09c9"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/77/bookmark
Content-Type: application/json
Authorization: Bearer 26e9791d8bb8381dfd90965c322e8dac08afc97ef1810905b53b4d00203cb990
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/77/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26e9791d8bb8381dfd90965c322e8dac08afc97ef1810905b53b4d00203cb990"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/73
Content-Type: application/json
Authorization: Bearer 6929edf2971abb9a792632772a556422f3a9712b19fae18a30c58689a218412b
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6929edf2971abb9a792632772a556422f3a9712b19fae18a30c58689a218412b"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/downvote
Content-Type: application/json
Authorization: Bearer f81fa9e13a887b7e08b1b164edbc6cd35fb98152722771f90b029eb512221f95
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f81fa9e13a887b7e08b1b164edbc6cd35fb98152722771f90b029eb512221f95"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/78
Content-Type: application/json
Authorization: Bearer 2d1467b5a940fff2c417d1abb7c43546c2b1bda8eb26839eb13a7ac496f1c1b2
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
    "id": 78,
    "obfuscated_id": "-wsYNe2w7uo",
    "author_id": 805,
    "chapter_id": 151,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:51.088Z",
    "created_at": "2016-10-18T09:28:51.088Z",
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
curl "api.goskive.com/v2/flashcards/78" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d1467b5a940fff2c417d1abb7c43546c2b1bda8eb26839eb13a7ac496f1c1b2"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/report
Content-Type: application/json
Authorization: Bearer cd871cc527d14a35b5f96b12e9237d7b9e67e92ca6bf9b5c963a25efeb140766
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
	-H "Authorization: Bearer cd871cc527d14a35b5f96b12e9237d7b9e67e92ca6bf9b5c963a25efeb140766"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/55/bookmark
Content-Type: application/json
Authorization: Bearer c755bf6803ab811c124c3d2d86a8038a445cc78aecb71aee7dcd2d821a5a8edf
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
	-H "Authorization: Bearer c755bf6803ab811c124c3d2d86a8038a445cc78aecb71aee7dcd2d821a5a8edf"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/72/upvote
Content-Type: application/json
Authorization: Bearer 89d46362d164b77603dd486132ad3f09670e4ec61bed8cee13f6a32e8410b500
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89d46362d164b77603dd486132ad3f09670e4ec61bed8cee13f6a32e8410b500"
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
    "key": "cache/1498acbc0054cc8fd46ce3bd34e9a434.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMDoyODo1MVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8xNDk4YWNiYzAwNTRjYzhmZDQ2Y2UzYmQzNGU5YTQzNC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOFQwOTI4NTFaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T092851Z",
    "x-amz-signature": "0e6c9a135f35e78ed76936ee1495b47462b7d0d730573c587950e37c5b964d29"
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
Authorization: Bearer e3917f1b55ec1d3be0013a49ea38ef1d35e2ef09e74006ba316254b521f81809
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
	-H "Authorization: Bearer e3917f1b55ec1d3be0013a49ea38ef1d35e2ef09e74006ba316254b521f81809"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 2ee9eccee059cf1c7b1c33a5d7197ddbb65a84cbf4e895d792d60f16a244b778
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
	-H "Authorization: Bearer 2ee9eccee059cf1c7b1c33a5d7197ddbb65a84cbf4e895d792d60f16a244b778"
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
{"password":{"reset_password_token":"pzek4wFXeEA4pp_Af3Gk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 692,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-18T09:28:43.063Z",
  "updated_at": "2016-10-18T09:28:43.690Z",
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
  "audit_id": 4487
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"pzek4wFXeEA4pp_Af3Gk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/133/comments
Content-Type: application/json
Authorization: Bearer dbe883c6db41e9979738d522efd841fcd88b6032d0f4e00cdfac01e4b8cc74e0
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
    "id": 60,
    "author_id": 943,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:29:00.752Z",
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
curl "api.goskive.com/v2/questions/133/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbe883c6db41e9979738d522efd841fcd88b6032d0f4e00cdfac01e4b8cc74e0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/131/comments
Content-Type: application/json
Authorization: Bearer 0fbd35a0204d7539b8b025a381e87a1a938a544e39dcb983d12f68d1f451e586
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
    "id": 59,
    "author_id": 937,
    "reply_to_id": null,
    "created_at": "2016-10-18T09:28:59.954Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 937,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:59.950Z",
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
	-H "Authorization: Bearer 0fbd35a0204d7539b8b025a381e87a1a938a544e39dcb983d12f68d1f451e586"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/129/comments
Content-Type: application/json
Authorization: Bearer ba03da339794457dd608f74f2db81e5fb37bf22b15d5bd4fae5864dca3d5544d
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
      "author_id": 933,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:28:59.288Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 932,
      "reply_to_id": null,
      "created_at": "2016-10-18T09:28:59.271Z",
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
curl "api.goskive.com/v2/questions/129/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba03da339794457dd608f74f2db81e5fb37bf22b15d5bd4fae5864dca3d5544d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/132/comments
Content-Type: application/json
Authorization: Bearer a9e4415076547ae818ecb7c2be17706b4356b02b6b846ea2478cd6f1f34793a8
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
curl "api.goskive.com/v2/questions/132/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9e4415076547ae818ecb7c2be17706b4356b02b6b846ea2478cd6f1f34793a8"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/45/feedbacks
Content-Type: application/json
Authorization: Bearer 841605b6617df898dad8b8dd293d9e7bf2488840d48afda73cba0d477d2a74c5
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
    "user_id": 311,
    "feedbackable_id": 45,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-18T09:28:04.232Z",
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
curl "api.goskive.com/v2/questions/45/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 841605b6617df898dad8b8dd293d9e7bf2488840d48afda73cba0d477d2a74c5"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/48/feedbacks
Content-Type: application/json
Authorization: Bearer 809c81191dec8e9fd481a922afbbf79f83415c5b6832568a07efa1870e1da501
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
      "id": 6,
      "user_id": 326,
      "feedbackable_id": 48,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:05.458Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 325,
      "feedbackable_id": 48,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T09:28:05.447Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/48/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 809c81191dec8e9fd481a922afbbf79f83415c5b6832568a07efa1870e1da501"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/6/votes
Content-Type: application/json
Authorization: Bearer ff84516be4e3393f3b1f951ae0a13028abd05ed25d33d63dd235f49b838b93f7
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
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 6,
      "user_id": 91
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 6,
      "user_id": 90
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 6,
      "user_id": 89
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/6/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff84516be4e3393f3b1f951ae0a13028abd05ed25d33d63dd235f49b838b93f7"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/57/republish
Content-Type: application/json
Authorization: Bearer 4becc11b0c02989402915538ec45010e735519b42a2314a42d4cf28eb2657abc
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
curl "api.goskive.com/v2/questions/57/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4becc11b0c02989402915538ec45010e735519b42a2314a42d4cf28eb2657abc"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/52/bookmark
Content-Type: application/json
Authorization: Bearer bf146c63f942c78a326ff7a30255782b433519f7a4e774e82c796693f1ba512f
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/52/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf146c63f942c78a326ff7a30255782b433519f7a4e774e82c796693f1ba512f"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/54
Content-Type: application/json
Authorization: Bearer e79cdef80b533bd368f31ba0ec38e601b3917031bcef7bfd7438117a7cfb18a2
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e79cdef80b533bd368f31ba0ec38e601b3917031bcef7bfd7438117a7cfb18a2"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/55/downvote
Content-Type: application/json
Authorization: Bearer 320fa2290c433998a47fd8f31c65a606e7b6f24b710e556882591b15f15a7e7b
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/55/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 320fa2290c433998a47fd8f31c65a606e7b6f24b710e556882591b15f15a7e7b"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/58
Content-Type: application/json
Authorization: Bearer 9064f557efd782c7512b43454a8e76cc8fd40dd6fe488a03f4e8df08fe68f379
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
    "id": 58,
    "obfuscated_id": "_S2mxc1kfck",
    "author_id": 362,
    "chapter_id": 53,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:09.364Z",
    "created_at": "2016-10-18T09:28:09.231Z",
    "tags": [
      {
        "id": 12,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 11,
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/58" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9064f557efd782c7512b43454a8e76cc8fd40dd6fe488a03f4e8df08fe68f379"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/53/report
Content-Type: application/json
Authorization: Bearer 32f5ab2daaec91d001b73db369940811a12385111b11792d8d2ec678115d00e7
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/53/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32f5ab2daaec91d001b73db369940811a12385111b11792d8d2ec678115d00e7"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/59/bookmark
Content-Type: application/json
Authorization: Bearer 083ad595e5186cf462415d473b43f5b9d297a12885ebd27de07dfcfa2bfdb3dd
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/59/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 083ad595e5186cf462415d473b43f5b9d297a12885ebd27de07dfcfa2bfdb3dd"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/61
Content-Type: application/json
Authorization: Bearer d0cccf109b99485bbc6f2e0185422814b16ccca801a7c837becbd98e17db7864
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":61,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T09:28:10.302Z","updated_at":"2016-10-18T09:28:10.434Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":56,"author_id":371,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 61,
    "obfuscated_id": "Acd5zhQoy8g",
    "author_id": 371,
    "chapter_id": 56,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T09:28:10.546Z",
    "created_at": "2016-10-18T09:28:10.302Z",
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
    "question": "{\"id\"=>61, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-18T09:28:10.302Z\", \"updated_at\"=>\"2016-10-18T09:28:10.434Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>56, \"author_id\"=>371, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 121,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 122,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 123,
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
curl "api.goskive.com/v2/questions/61" -d '{"question":{"question":{"id":61,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T09:28:10.302Z","updated_at":"2016-10-18T09:28:10.434Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":56,"author_id":371,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0cccf109b99485bbc6f2e0185422814b16ccca801a7c837becbd98e17db7864"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/60/upvote
Content-Type: application/json
Authorization: Bearer fbf43bb9fdff2cab5c95f3aa320e9c046ae0acc41a069b4b7f50800291677597
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/60/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbf43bb9fdff2cab5c95f3aa320e9c046ae0acc41a069b4b7f50800291677597"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 0d1e04bf109cda2a345fd64807c80b8705e3834c144cf9857f061fcc4229ff78
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
      "creator_id": 27,
      "id": 9,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "topic_id": 9,
      "discipline_id": 9,
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
      "updated_at": "2016-10-18T09:27:38.229Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d1e04bf109cda2a345fd64807c80b8705e3834c144cf9857f061fcc4229ff78"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 5987d1561665ada346e3fced69eda2b3df3ae5d8ed2dc768e606fc58357d7426
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
      "updated_at": "2016-10-18T09:27:38.486Z",
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
      "updated_at": "2016-10-18T09:27:38.470Z",
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
	-H "Authorization: Bearer 5987d1561665ada346e3fced69eda2b3df3ae5d8ed2dc768e606fc58357d7426"
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
      "id": 240,
      "name": "Upgradable coherent Graphic Interface",
      "name_translations": {
        "en": "Upgradable coherent Graphic Interface"
      },
      "discipline_id": 241
    },
    {
      "id": 241,
      "name": "Innovative scalable forecast",
      "name_translations": {
        "en": "Innovative scalable forecast"
      },
      "discipline_id": 242
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
GET /v2/topics/242
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
    "id": 242,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 243
  }
}
```



```shell
curl "api.goskive.com/v2/topics/242" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 12e9a190e34b4e550ad60364ed5b1f1063648725c5560ca4414ef6792560668e
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
      "id": 182,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-164",
      "html_url": "https://goskive.com/university/uni-164",
      "slug": "uni-164",
      "name": "University 137",
      "short_name": "Uni 164",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/35fdeedf6255422331db7bb84396b90a7952dcfc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b43f0fc540c9471e4abb2ff21d649b3e419c0430.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:28:30.918Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-165",
      "html_url": "https://goskive.com/university/uni-165",
      "slug": "uni-165",
      "name": "University 138",
      "short_name": "Uni 165",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d147cc37498808cd35f7673777a7fbb370abba91.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/74a83b395da37a337bff4bb35a86fe88eb73f10a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:28:30.934Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-166",
      "html_url": "https://goskive.com/university/uni-166",
      "slug": "uni-166",
      "name": "University 139",
      "short_name": "Uni 166",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9e34f731a42888a0b05110ae5cef1dab517f5ad3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c39445b96e218aae7f8d5a5187898d4d19659d13.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T09:28:30.950Z",
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
	-H "Authorization: Bearer 12e9a190e34b4e550ad60364ed5b1f1063648725c5560ca4414ef6792560668e"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer beeb29443ac6c0d39e84704048f9c33d28d9fc617d0efda6c35ffa9284a1f2f7
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
    "id": 186,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6585fabf4d63fed65a3d578a9eaf6020a5352492.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1cb4077eb7d4842b2ab7c203de4528f2888a4b7d.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-18T09:28:31.070Z",
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
	-H "Authorization: Bearer beeb29443ac6c0d39e84704048f9c33d28d9fc617d0efda6c35ffa9284a1f2f7"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f3025c08de48500d4d9d2432f07fe0923251d6fd72827b5434196075945ec6bf
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":48,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 72,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 27,
    "additional_university_ids": [

    ],
    "topic_id": 48,
    "discipline_id": 48,
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
    "chapters_updated_at": "2016-10-18T09:27:42.264Z",
    "updated_at": "2016-10-18T09:27:42.401Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 12,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-18T09:27:42.357Z",
        "course_id": 48,
        "author_id": 72,
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
        "id": 13,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-18T09:27:42.374Z",
        "course_id": 48,
        "author_id": 72,
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
        "id": 14,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-18T09:27:42.391Z",
        "course_id": 48,
        "author_id": 72,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":48,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3025c08de48500d4d9d2432f07fe0923251d6fd72827b5434196075945ec6bf"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 68faca3322c40f3d9f80fdcaa313d9f01ab53d6120e5eadae5be45c8be12a24a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":49,"published":false}}
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
    "creator_id": 73,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 28,
    "additional_university_ids": [

    ],
    "topic_id": 49,
    "discipline_id": 49,
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
    "updated_at": "2016-10-18T09:27:42.553Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":49,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68faca3322c40f3d9f80fdcaa313d9f01ab53d6120e5eadae5be45c8be12a24a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6b809d16fd1cf6bac88ab871d49c0a3668cf791674140ea854b75e2cf8d395d8
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
      "creator_id": 32,
      "id": 14,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 14,
      "discipline_id": 14,
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
      "updated_at": "2016-10-18T09:27:38.725Z",
      "shortname": "fu-course-7"
    },
    {
      "creator_id": 32,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 15,
      "discipline_id": 15,
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
      "chapters_updated_at": "2016-10-18T09:27:39.008Z",
      "updated_at": "2016-10-18T09:27:39.014Z",
      "shortname": "fu-course-8"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b809d16fd1cf6bac88ab871d49c0a3668cf791674140ea854b75e2cf8d395d8"
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
      "creator_id": 62,
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "topic_id": 38,
      "discipline_id": 38,
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
      "updated_at": "2016-10-18T09:27:41.344Z",
      "shortname": "fu-course-31"
    },
    {
      "creator_id": 62,
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 22,
      "additional_university_ids": [

      ],
      "topic_id": 39,
      "discipline_id": 39,
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
      "chapters_updated_at": "2016-10-18T09:27:41.649Z",
      "updated_at": "2016-10-18T09:27:41.655Z",
      "shortname": "fu-course-32"
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
Authorization: Bearer 83d20a622d2c80b8158acd13f4d9714a223eac62f8db14a6273c2a7651d09bbb
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
      "creator_id": 39,
      "id": 18,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 18,
      "discipline_id": 18,
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
      "updated_at": "2016-10-18T09:27:39.320Z",
      "shortname": "fu-course-11"
    },
    {
      "creator_id": 39,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 19,
      "discipline_id": 19,
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
      "updated_at": "2016-10-18T09:27:39.358Z",
      "shortname": "fu-course-12"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83d20a622d2c80b8158acd13f4d9714a223eac62f8db14a6273c2a7651d09bbb"
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
      "creator_id": 67,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-35",
      "html_url": "https://goskive.com/course/fu-course-35",
      "slug": "fu-course-35",
      "university_id": 23,
      "additional_university_ids": [

      ],
      "topic_id": 42,
      "discipline_id": 42,
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
      "updated_at": "2016-10-18T09:27:41.843Z",
      "shortname": "fu-course-35"
    },
    {
      "creator_id": 67,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-36",
      "html_url": "https://goskive.com/course/fu-course-36",
      "slug": "fu-course-36",
      "university_id": 23,
      "additional_university_ids": [

      ],
      "topic_id": 43,
      "discipline_id": 43,
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
      "updated_at": "2016-10-18T09:27:41.881Z",
      "shortname": "fu-course-36"
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
Authorization: Bearer 4f72bcf010220c59cbbfae2ac2c2d9042119232f86eda8660be1f7c3c5c01e8a
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
  "id": 681,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-18T09:28:41.752Z",
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
	-H "Authorization: Bearer 4f72bcf010220c59cbbfae2ac2c2d9042119232f86eda8660be1f7c3c5c01e8a"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/206
Content-Type: application/json
Authorization: Bearer aab0c6efcd22570a58eade9fcebae650ac183bd80950e8a1c592f4ca9d53169e
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
    "id": 206,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 83,
    "fields_of_study": [
      104,
      105
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-18T09:27:50.825Z",
    "updated_at": "2016-10-18T09:27:50.825Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/206" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aab0c6efcd22570a58eade9fcebae650ac183bd80950e8a1c592f4ca9d53169e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/208
Content-Type: application/json
Authorization: Bearer 889e5615dcc80a2c702ce7f781d6aca8b5fe29102d3e541d6288bcfaaabd5cf6
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
    "id": 208,
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
    "created_at": "2016-10-18T09:27:50.911Z",
    "updated_at": "2016-10-18T09:27:50.911Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/208" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 889e5615dcc80a2c702ce7f781d6aca8b5fe29102d3e541d6288bcfaaabd5cf6"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/9
Content-Type: application/json
Authorization: Bearer 7e8b7e92c9f45a68303ae112a3a33f2caf6d44dd8f0612cb25ab19bcac27cf32
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e8b7e92c9f45a68303ae112a3a33f2caf6d44dd8f0612cb25ab19bcac27cf32"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/10
Content-Type: application/json
Authorization: Bearer 67a0f1856d58d53f57af8a961fa958ec4d64ecc955bc03b219c4e59e05b197a9
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
    "id": 10,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 10,
    "user_id": 198
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67a0f1856d58d53f57af8a961fa958ec4d64ecc955bc03b219c4e59e05b197a9"
```
