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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7e9634a3c35475a7526494b0c95fa4a655eb18c98eaa1d3ac5f0584524ece72d","client_secret":"ffccb41c6ed2666ee944663137c754e496380f43b4dbf4906ce62bb7836be26c"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"7e9634a3c35475a7526494b0c95fa4a655eb18c98eaa1d3ac5f0584524ece72d","client_secret":"ffccb41c6ed2666ee944663137c754e496380f43b4dbf4906ce62bb7836be26c"}' -X POST \
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
Authorization: Basic NTdjYTA4ZDI2ZDUzZGI5YmI5M2UyMDQzMmI4NmI1MWRmMjk3YWI5ZjYzYTM1
YjlkYTJiODYxOWMzMmZmYTAxNjozNmExYmIzZTM3YjFlOWZkNjM5ZjBhNTdj
Y2M3NTBmY2YxZTFiNzBiMTkyN2VmNDNmNmY3YzQ2ZWVjOWFhMWZk

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
	-u 57ca08d26d53db9bb93e20432b86b51df297ab9f63a35b9da2b8619c32ffa016:36a1bb3e37b1e9fd639f0a57ccc750fcf1e1b70b1927ef43f6f7c46eec9aa1fd
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"f56b0a2e7d9e900b15644feb71be02629af82ffb33d8803ff535fb1beff2cb41","client_secret":"1430a33742736b86b0c8a70453a2b2591c3d190c6509f1b2869d24949796a49c"}
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
  "access_token": "b25c84b9a328c5250e35486797c36a293b7391fa33a7fd5fc662061bdf2c3958",
  "token_type": "bearer",
  "created_at": 1479392021
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"f56b0a2e7d9e900b15644feb71be02629af82ffb33d8803ff535fb1beff2cb41","client_secret":"1430a33742736b86b0c8a70453a2b2591c3d190c6509f1b2869d24949796a49c"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NjMxZWY5ZDk1MDlkMjRhNTE4YWRjMTBiMmRjNzIzNTljZjNkMDE0NTM4YjJi
OWQyODcyYzdmZTA5NWRhYTIxYzo4NzlkMTI1YWNhZmY3OWZiMzhhNDUyZGM2
NTZiYjAzNDQyYzBmMjg1M2IzYThmYzg1ZDAwOWRlZmVkYmVjNjVj

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
  "access_token": "8f83d7af0a39f47ea419ed34276d281c513e9995f2e46e9e65cb7a67752016fa",
  "token_type": "bearer",
  "created_at": 1479392021
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 631ef9d9509d24a518adc10b2dc72359cf3d014538b2b9d2872c7fe095daa21c:879d125acaff79fb38a452dc656bb03442c0f2853b3a8fc85d009defedbec65c
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
{"grant_type":"client_credentials","client_id":"0b1c26414317d8ace0ad97c38ca2283b29a3f6879342cd7ee59514e35a19fe69","client_secret":"c2c758a419a8e4bec603aed457c231d54c32354e2de16d9237793b02ff815a93"}
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
  "access_token": "35adceff4e74f88a9e5b05945e4a859b699602b676a608feddc573c6a949b38f",
  "token_type": "bearer",
  "created_at": 1479392021
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"0b1c26414317d8ace0ad97c38ca2283b29a3f6879342cd7ee59514e35a19fe69","client_secret":"c2c758a419a8e4bec603aed457c231d54c32354e2de16d9237793b02ff815a93"}' -X POST \
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
Authorization: Bearer a9bf737e4ce6176f62ee8c29860adb9455e043b9cf49be97eca2a55586519f8d
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
    "company_id": 9,
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
	-H "Authorization: Bearer a9bf737e4ce6176f62ee8c29860adb9455e043b9cf49be97eca2a55586519f8d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/193/flashcards
Content-Type: application/json
Authorization: Bearer a3ee124db143af23987cede356da799847c4b0b73aeedd9e570f0b48a450c183
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":193,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 92,
    "obfuscated_id": "__OphzZQiQY",
    "author_id": 883,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:54.016Z",
    "created_at": "2016-11-17T14:14:54.016Z",
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
curl "api.goskive.com/v2/chapters/193/flashcards" -d '{"flashcard":{"chapter_id":193,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3ee124db143af23987cede356da799847c4b0b73aeedd9e570f0b48a450c183"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer 0aca3ddd3f4add6c48c01732a47a07b04df8dd73f20181932c921cbdbba35ae8
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
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 884,
      "chapter_id": 194,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:54.266Z",
      "created_at": "2016-11-17T14:14:54.266Z",
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
      "id": 94,
      "obfuscated_id": "CVi6VU_nV6k",
      "author_id": 884,
      "chapter_id": 194,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:54.302Z",
      "created_at": "2016-11-17T14:14:54.302Z",
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
      "id": 95,
      "obfuscated_id": "uTOhBSQK4CI",
      "author_id": 884,
      "chapter_id": 194,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:54.338Z",
      "created_at": "2016-11-17T14:14:54.338Z",
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
curl "api.goskive.com/v2/chapters/194/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0aca3ddd3f4add6c48c01732a47a07b04df8dd73f20181932c921cbdbba35ae8"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/88/questions
Content-Type: application/json
Authorization: Bearer 09a9de36a55b6fda76304e29a69f5f60536586c2631cfc95b048cc3394f983fa
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":88,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 75,
    "obfuscated_id": "rRYuZazyhgg",
    "author_id": 438,
    "chapter_id": 88,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:14.138Z",
    "created_at": "2016-11-17T14:14:14.138Z",
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
        "id": 151,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 152,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 153,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 154,
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
curl "api.goskive.com/v2/chapters/88/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":88,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09a9de36a55b6fda76304e29a69f5f60536586c2631cfc95b048cc3394f983fa"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/89/questions
Content-Type: application/json
Authorization: Bearer 9d6520e22423370ff9991ed3792d09eb8b3c3567bc4a68b7cc88dc3eef958bc0
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":89,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 76,
    "obfuscated_id": "oK0h_-4yfUk",
    "author_id": 441,
    "chapter_id": 89,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:14.870Z",
    "created_at": "2016-11-17T14:14:14.870Z",
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
        "id": 155,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 156,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/89/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":89,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d6520e22423370ff9991ed3792d09eb8b3c3567bc4a68b7cc88dc3eef958bc0"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/90/questions
Content-Type: application/json
Authorization: Bearer b57e0a513c4a0dd4ddf71e500622a031b40c4871111ce3517686e9d387c6cc49
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":90,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 444,
    "chapter_id": 90,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:15.424Z",
    "created_at": "2016-11-17T14:14:15.424Z",
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
        "id": 157,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 158,
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
curl "api.goskive.com/v2/chapters/90/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":90,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b57e0a513c4a0dd4ddf71e500622a031b40c4871111ce3517686e9d387c6cc49"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/87/questions
Content-Type: application/json
Authorization: Bearer 65cf46f829db8498f9aabd75948e107e5de6cd17d667549a2d3dce403d9576d1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":87,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 435,
    "chapter_id": 87,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:13.591Z",
    "created_at": "2016-11-17T14:14:13.591Z",
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
        "id": 148,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 149,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 150,
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
curl "api.goskive.com/v2/chapters/87/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":87,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65cf46f829db8498f9aabd75948e107e5de6cd17d667549a2d3dce403d9576d1"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/86/questions
Content-Type: application/json
Authorization: Bearer bf21d550d96c75e58270edbe30f15ef1ddbdb125bab1d1797bfd87480ea4a5c2
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 429,
      "chapter_id": 86,
      "position": 62,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:12.918Z",
      "created_at": "2016-11-17T14:14:12.796Z",
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
    },
    {
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 430,
      "chapter_id": 86,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:13.116Z",
      "created_at": "2016-11-17T14:14:12.992Z",
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
          "id": 144,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 145,
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
      "author_id": 431,
      "chapter_id": 86,
      "position": 64,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:13.323Z",
      "created_at": "2016-11-17T14:14:13.193Z",
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
          "id": 146,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 147,
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
curl "api.goskive.com/v2/chapters/86/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf21d550d96c75e58270edbe30f15ef1ddbdb125bab1d1797bfd87480ea4a5c2"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/164
Content-Type: application/json
Authorization: Bearer 34dac3df2c0ab4f163ee4c644b8b9c163c980a0e7addc8df97c5f120193b9c19
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
curl "api.goskive.com/v2/chapters/164" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34dac3df2c0ab4f163ee4c644b8b9c163c980a0e7addc8df97c5f120193b9c19"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/165
Content-Type: application/json
Authorization: Bearer 72fe7cab657431d6edcacd58d6ed78810107030bf7d921bc3825a07c68a92725
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
curl "api.goskive.com/v2/chapters/165" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72fe7cab657431d6edcacd58d6ed78810107030bf7d921bc3825a07c68a92725"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/168
Content-Type: application/json
Authorization: Bearer a23e28963cddbd83f243e23fc20b7c809d71b30d154b87a895f29b16b020722f
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
curl "api.goskive.com/v2/chapters/168" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a23e28963cddbd83f243e23fc20b7c809d71b30d154b87a895f29b16b020722f"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/166
Content-Type: application/json
Authorization: Bearer 86e0243e555d7197757d2e98ddc062cce731fa40da78e987ba0e5d8f910c63f4
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/166" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86e0243e555d7197757d2e98ddc062cce731fa40da78e987ba0e5d8f910c63f4"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/161
Content-Type: application/json
Authorization: Bearer caf3da896f08ab03fba3aad766b44135be7f0387a3334230a6b653a4c5708212
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
    "id": 161,
    "updated_at": "2016-11-17T14:14:33.512Z",
    "course_id": 215,
    "author_id": 698,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-17T14:14:32.948Z",
    "questions_updated_at": "2016-11-17T14:14:32.948Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 702,
        "chapter_id": 161,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:33.493Z",
        "created_at": "2016-11-17T14:14:33.493Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 700,
        "chapter_id": 161,
        "position": 80,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:33.381Z",
        "created_at": "2016-11-17T14:14:33.253Z",
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
            "id": 189,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 190,
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
curl "api.goskive.com/v2/chapters/161" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer caf3da896f08ab03fba3aad766b44135be7f0387a3334230a6b653a4c5708212"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/169
Content-Type: application/json
Authorization: Bearer bea61a8b97490db9f919b87b2d2de5961b5647b60d58656592437206a42caeef
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
    "id": 169,
    "updated_at": "2016-11-17T14:14:35.705Z",
    "course_id": 223,
    "author_id": 730,
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
curl "api.goskive.com/v2/chapters/169" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bea61a8b97490db9f919b87b2d2de5961b5647b60d58656592437206a42caeef"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 2e9a234a9f3f4ef68a0c9f94ae2163ff2009b26c74c7eef53174be6e7bafd018
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
    "id": 3,
    "author_id": 47,
    "reply_to_id": 2,
    "created_at": "2016-11-17T14:13:37.540Z",
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
curl "api.goskive.com/v2/comments/2/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e9a234a9f3f4ef68a0c9f94ae2163ff2009b26c74c7eef53174be6e7bafd018"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 67ae2244edb03fc2f542dc0cf5a7feaa2e6ce6d190e727f63c737cfaca8514ec
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
curl "api.goskive.com/v2/comments/1/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67ae2244edb03fc2f542dc0cf5a7feaa2e6ce6d190e727f63c737cfaca8514ec"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/59
Content-Type: application/json
Authorization: Bearer 3fec1acedbb61ee6250cfa4a541802ecb7d4947f79ef30d37ba50a19393f98cd
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
curl "api.goskive.com/v2/comments/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fec1acedbb61ee6250cfa4a541802ecb7d4947f79ef30d37ba50a19393f98cd"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer eacbf95d2f940702048e9616f6e8f190001c6c21f50ba5b0760b1c8f6000c300
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
curl "api.goskive.com/v2/comments/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eacbf95d2f940702048e9616f6e8f190001c6c21f50ba5b0760b1c8f6000c300"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/57
Content-Type: application/json
Authorization: Bearer a3fffedfcee86ad1135ecce83e438c39de349223ed9b1fdcea88aa11a2f942ee
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3fffedfcee86ad1135ecce83e438c39de349223ed9b1fdcea88aa11a2f942ee"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 818e47be72732647373c3c75b79944098d6eee198ab1ce007235fd0b2745bd71
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 818e47be72732647373c3c75b79944098d6eee198ab1ce007235fd0b2745bd71"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 9294be5b44953d7b61d0b7ead97355dc7f8d0bca413c9f3f80aa2c690f6dc584
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
    "updated_at": "2016-11-17T14:14:42.879Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9294be5b44953d7b61d0b7ead97355dc7f8d0bca413c9f3f80aa2c690f6dc584"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 61862fb8ddcda134b0038fba82626afcea83e0ade70328dd3f1a7630fe930337
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
      "updated_at": "2016-11-17T14:14:42.818Z"
    },
    {
      "id": 34,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-17T14:14:42.822Z"
    },
    {
      "id": 35,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-17T14:14:42.826Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61862fb8ddcda134b0038fba82626afcea83e0ade70328dd3f1a7630fe930337"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/38/company_profiles
Content-Type: application/json
Authorization: Bearer 836c1b49bf1362227ac6289e3569a11edcee563670fc84f5c53845fdbdd886b3
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
curl "api.goskive.com/v2/companies/38/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 836c1b49bf1362227ac6289e3569a11edcee563670fc84f5c53845fdbdd886b3"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 65679f29ab4d7fe42aaafa03602d81c5e9dc410611a24fcb5cc7e189cb147e97
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
	-H "Authorization: Bearer 65679f29ab4d7fe42aaafa03602d81c5e9dc410611a24fcb5cc7e189cb147e97"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer f1d35f6f0e2ac8d43c50e0cbdd99f791f9a2bdda4dd6a1cfa52af19c4d1752b4
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
      "title": "Campaign 4",
      "company_id": 18,
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
    },
    {
      "id": 8,
      "title": "Campaign 7",
      "company_id": 21,
      "precluded_campaign_ids": [

      ],
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
        }
      ],
      "banners": [
        {
          "image_url_absolute": "banners/498551b0a405b9134839281bc158747e85383832.png",
          "target_url": "http://goskive.com",
          "id": 5,
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
	-H "Authorization: Bearer f1d35f6f0e2ac8d43c50e0cbdd99f791f9a2bdda4dd6a1cfa52af19c4d1752b4"
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
Authorization: Bearer 2f4c8c0617e8cb7711c012bedf2183eb3bf865795c5c472bff10d92a48884afd
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
	-H "Authorization: Bearer 2f4c8c0617e8cb7711c012bedf2183eb3bf865795c5c472bff10d92a48884afd"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5bedd0d2b2fb1e4a8356cfcd6625603d6f6bdf21426a98dcacfb6f016423b819
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
    "id": 138,
    "updated_at": "2016-11-17T14:14:22.904Z",
    "course_id": 155,
    "author_id": 573,
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
	-H "Authorization: Bearer 5bedd0d2b2fb1e4a8356cfcd6625603d6f6bdf21426a98dcacfb6f016423b819"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 02e6ed381964670b5ba2935ee03cf5b5353821179fd5dc7ad088f3306dcb4b22
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
      "id": 118,
      "updated_at": "2016-11-17T14:14:20.325Z",
      "course_id": 144,
      "author_id": 530,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 112",
      "position": 1
    },
    {
      "id": 119,
      "updated_at": "2016-11-17T14:14:20.348Z",
      "course_id": 144,
      "author_id": 531,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 113",
      "position": 2
    },
    {
      "id": 120,
      "updated_at": "2016-11-17T14:14:20.599Z",
      "course_id": 144,
      "author_id": 532,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-17T14:14:20.254Z",
      "questions_updated_at": "2016-11-17T14:14:20.254Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 114",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02e6ed381964670b5ba2935ee03cf5b5353821179fd5dc7ad088f3306dcb4b22"
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
      "id": 130,
      "updated_at": "2016-11-17T14:14:21.764Z",
      "course_id": 150,
      "author_id": 558,
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
      "id": 131,
      "updated_at": "2016-11-17T14:14:21.788Z",
      "course_id": 150,
      "author_id": 559,
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
      "id": 132,
      "updated_at": "2016-11-17T14:14:22.038Z",
      "course_id": 150,
      "author_id": 560,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-17T14:14:21.690Z",
      "questions_updated_at": "2016-11-17T14:14:21.690Z",
      "flashcards_count": 0,
      "questions_count": 1,
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
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0dc8d96b6eec768235f07506c800fd3dabe5ff75f527c6ab774f50223b2fc6a1
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
      "updated_at": "2016-11-17T14:14:20.854Z",
      "course_id": 146,
      "author_id": 539,
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
      "id": 122,
      "updated_at": "2016-11-17T14:14:20.878Z",
      "course_id": 146,
      "author_id": 540,
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
      "id": 123,
      "updated_at": "2016-11-17T14:14:20.901Z",
      "course_id": 146,
      "author_id": 541,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 117",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dc8d96b6eec768235f07506c800fd3dabe5ff75f527c6ab774f50223b2fc6a1"
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
      "id": 133,
      "updated_at": "2016-11-17T14:14:22.237Z",
      "course_id": 152,
      "author_id": 565,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 127",
      "position": 1
    },
    {
      "id": 134,
      "updated_at": "2016-11-17T14:14:22.260Z",
      "course_id": 152,
      "author_id": 566,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 128",
      "position": 2
    },
    {
      "id": 135,
      "updated_at": "2016-11-17T14:14:22.284Z",
      "course_id": 152,
      "author_id": 567,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 129",
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
Authorization: Bearer c73bf7d6dd4d8ba0fae986fc00f2189bbd55fd113677a1e2900ba242e713e6f7
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
    "course_id": 16,
    "user_id": 49,
    "updated_at": "2016-11-17T14:13:37.950Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c73bf7d6dd4d8ba0fae986fc00f2189bbd55fd113677a1e2900ba242e713e6f7"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7ffe8db6d03646ba4541df9e59cfed8dd85146fb037edccbf20bdf3418e565b9
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
      "course_id": 19,
      "user_id": 55,
      "updated_at": "2016-11-17T14:13:38.282Z"
    },
    {
      "id": 4,
      "course_id": 19,
      "user_id": 56,
      "updated_at": "2016-11-17T14:13:38.297Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ffe8db6d03646ba4541df9e59cfed8dd85146fb037edccbf20bdf3418e565b9"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/230/files
Content-Type: application/json
Authorization: Bearer a07323400a29dfa96908368557a36d9dc2e7348a5ed07db1e0be65a8f118dfb0
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
      "id": 20,
      "uploader": {
        "id": 754,
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
        "created_at": "2016-11-17T14:14:38.587Z",
        "updated_at": "2016-11-17T14:14:38.587Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T14:14:38.597Z",
      "updated_at": "2016-11-17T14:14:38.597Z",
      "course_id": 230,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 755,
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
        "created_at": "2016-11-17T14:14:38.605Z",
        "updated_at": "2016-11-17T14:14:38.605Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T14:14:38.614Z",
      "updated_at": "2016-11-17T14:14:38.614Z",
      "course_id": 230,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 22,
      "uploader": {
        "id": 756,
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
        "created_at": "2016-11-17T14:14:38.622Z",
        "updated_at": "2016-11-17T14:14:38.622Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-17T14:14:38.632Z",
      "updated_at": "2016-11-17T14:14:38.632Z",
      "course_id": 230,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/230/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a07323400a29dfa96908368557a36d9dc2e7348a5ed07db1e0be65a8f118dfb0"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/229/files
Content-Type: application/json
Authorization: Bearer 6adb2982e5195283d4ea925197aaef813e1711eadd33e497c5b5d6f6cfe373ba
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
    "id": 19,
    "uploader": {
      "id": 752,
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
      "created_at": "2016-11-17T14:14:38.424Z",
      "updated_at": "2016-11-17T14:14:38.424Z"
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
    "created_at": "2016-11-17T14:14:38.458Z",
    "updated_at": "2016-11-17T14:14:38.458Z",
    "course_id": 229,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/229/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6adb2982e5195283d4ea925197aaef813e1711eadd33e497c5b5d6f6cfe373ba"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/232/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer e60460937c7b23f583180a7d27fff844793145a47d4f7c80d3cc9ba6bb904c7c
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
    "key": "cache/883a525188f6b5b0fa6033cbfdf7dc01.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xN1QxNToxNDozOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzg4M2E1MjUxODhmNmI1YjBmYTYwMzNjYmZkZjdkYzAxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTcvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE3VDE0MTQzOFoifV19",
    "x-amz-credential": "FAKE/20161117/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161117T141438Z",
    "x-amz-signature": "1e4232b9039f31ce2aa606dbcc6cb4f7e924f1761c62e3fd68549b97677bce57"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/232/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e60460937c7b23f583180a7d27fff844793145a47d4f7c80d3cc9ba6bb904c7c"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer eeb211414d136ab477cb5553b3cfe6e8de45bc4cd42022c1000e92d2d6c8114f
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
	-H "Authorization: Bearer eeb211414d136ab477cb5553b3cfe6e8de45bc4cd42022c1000e92d2d6c8114f"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 46c274c79c1a94ad220195d8e1fc43c89329d798ff48bd520dd4f6c6fe089773
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
	-H "Authorization: Bearer 46c274c79c1a94ad220195d8e1fc43c89329d798ff48bd520dd4f6c6fe089773"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3f04e542f6066da23d4930d50294556e6f1e6968ee703dfea19ad268ea0911c8
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
	-H "Authorization: Bearer 3f04e542f6066da23d4930d50294556e6f1e6968ee703dfea19ad268ea0911c8"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer dd781567774a9c65fa67d90489c7ac25cec121454303b8db781a60976ee4e1b2
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
	-H "Authorization: Bearer dd781567774a9c65fa67d90489c7ac25cec121454303b8db781a60976ee4e1b2"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8847b7b9fa7845b2b11ec4e2fc787cc3a73add8ce5282acd86f2b2884bfdde0e
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
	-H "Authorization: Bearer 8847b7b9fa7845b2b11ec4e2fc787cc3a73add8ce5282acd86f2b2884bfdde0e"
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
    "creator_id": 855,
    "id": 268,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 253,
    "additional_university_ids": [

    ],
    "discipline_id": 276,
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
    "chapters_updated_at": "2016-11-17T14:14:48.296Z",
    "updated_at": "2016-11-17T14:14:49.799Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 116,
        "obfuscated_id": "PhHGVKqnHFA",
        "author_id": 855,
        "chapter_id": 186,
        "position": 103,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.509Z",
        "created_at": "2016-11-17T14:14:48.388Z",
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
            "id": 235,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 236,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 855,
        "chapter_id": 187,
        "position": 105,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.906Z",
        "created_at": "2016-11-17T14:14:48.777Z",
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
    ],
    "chapters": [
      {
        "id": 186,
        "updated_at": "2016-11-17T14:14:49.749Z",
        "course_id": 268,
        "author_id": 855,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T14:14:48.296Z",
        "questions_updated_at": "2016-11-17T14:14:48.296Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 165",
        "position": 1
      },
      {
        "id": 187,
        "updated_at": "2016-11-17T14:14:49.791Z",
        "course_id": 268,
        "author_id": 855,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T14:14:48.296Z",
        "questions_updated_at": "2016-11-17T14:14:48.296Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 166",
        "position": 2
      }
    ],
    "topic_id": 275,
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
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 41500efd7b3098f87e7081a51cdd4a29aa55f57ba2297b5484c25a0e2ed7527a
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
    "creator_id": 860,
    "id": 269,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 254,
    "additional_university_ids": [

    ],
    "discipline_id": 277,
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
    "chapters_updated_at": "2016-11-17T14:14:49.858Z",
    "updated_at": "2016-11-17T14:14:51.369Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 861,
        "chapter_id": 188,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:51.148Z",
        "created_at": "2016-11-17T14:14:51.148Z",
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
        "author_id": 861,
        "chapter_id": 189,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:51.225Z",
        "created_at": "2016-11-17T14:14:51.225Z",
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
        "author_id": 861,
        "chapter_id": 188,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:51.192Z",
        "created_at": "2016-11-17T14:14:51.192Z",
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
        "author_id": 861,
        "chapter_id": 189,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:51.271Z",
        "created_at": "2016-11-17T14:14:51.271Z",
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
        "id": 122,
        "obfuscated_id": "cMWZX2w28hY",
        "author_id": 861,
        "chapter_id": 188,
        "position": 109,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:50.083Z",
        "created_at": "2016-11-17T14:14:49.960Z",
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
        "author_id": 861,
        "chapter_id": 188,
        "position": 110,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:50.268Z",
        "created_at": "2016-11-17T14:14:50.151Z",
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
        "author_id": 861,
        "chapter_id": 189,
        "position": 111,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:50.480Z",
        "created_at": "2016-11-17T14:14:50.352Z",
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
        "author_id": 861,
        "chapter_id": 189,
        "position": 112,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:50.670Z",
        "created_at": "2016-11-17T14:14:50.549Z",
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
      }
    ],
    "chapters": [
      {
        "id": 188,
        "updated_at": "2016-11-17T14:14:51.322Z",
        "course_id": 269,
        "author_id": 860,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T14:14:49.858Z",
        "questions_updated_at": "2016-11-17T14:14:49.858Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 167",
        "position": 1
      },
      {
        "id": 189,
        "updated_at": "2016-11-17T14:14:51.361Z",
        "course_id": 269,
        "author_id": 860,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-17T14:14:49.858Z",
        "questions_updated_at": "2016-11-17T14:14:49.858Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 168",
        "position": 2
      }
    ],
    "topic_id": 276,
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
	-H "Authorization: Bearer 41500efd7b3098f87e7081a51cdd4a29aa55f57ba2297b5484c25a0e2ed7527a"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/262/pin
Content-Type: application/json
Authorization: Bearer 6998a82ec028aedbcd80914162e137d918f9b80eec2ba5a55db191d1ced29cb8
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/262/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6998a82ec028aedbcd80914162e137d918f9b80eec2ba5a55db191d1ced29cb8"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/271/pin
Content-Type: application/json
Authorization: Bearer a2c20d3080bc20d0c54cfd71f627254b9afbcea85b56ee7d804014777b3bab71
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/271/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2c20d3080bc20d0c54cfd71f627254b9afbcea85b56ee7d804014777b3bab71"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f1bdaeac35e915452d842ae0cb4879d54ef3f59d708bf56aede7a176407833c4
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
    "creator_id": 844,
    "id": 264,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 249,
    "additional_university_ids": [

    ],
    "discipline_id": 272,
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
    "updated_at": "2016-11-17T14:14:46.171Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 271,
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
	-H "Authorization: Bearer f1bdaeac35e915452d842ae0cb4879d54ef3f59d708bf56aede7a176407833c4"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 78469e53e2666fbd45c71ebda5be7414ae2a64f94a72790041ecdc5c701106c7
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
    "id": 983,
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
    "created_at": "2016-11-17T14:14:58.584Z",
    "updated_at": "2016-11-17T14:14:58.584Z",
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
	-H "Authorization: Bearer 78469e53e2666fbd45c71ebda5be7414ae2a64f94a72790041ecdc5c701106c7"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1fbc41e67b61ebccae288467199b6bbdfa8ae68294f9c9012f421300b75639cc
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[325]}
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
    "id": 985,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      325
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-17T14:14:58.996Z",
    "updated_at": "2016-11-17T14:14:59.031Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[325]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fbc41e67b61ebccae288467199b6bbdfa8ae68294f9c9012f421300b75639cc"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 6b65a59bbd11aa17fd1039012aefada2c443cfb71b548a3ed1cae4017b9e1885
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
    "id": 987,
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
    "created_at": "2016-11-17T14:14:59.125Z",
    "updated_at": "2016-11-17T14:14:59.125Z",
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
	-H "Authorization: Bearer 6b65a59bbd11aa17fd1039012aefada2c443cfb71b548a3ed1cae4017b9e1885"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9b0b3620fcf0888ae8ff5379d790ba806661339f2b7d2ccd2e170fe845d60e0e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[326]}
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
    "id": 986,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      326
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-17T14:14:59.074Z",
    "updated_at": "2016-11-17T14:14:59.074Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[326]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b0b3620fcf0888ae8ff5379d790ba806661339f2b7d2ccd2e170fe845d60e0e"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 82b3a338c4898cd4b8a14f87c3c674dd668421387786d26609396ed355516758
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

324
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
    "id": 984,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/a0798e20d9e1ce8773a0364ca7c6e8e0cecb750c.jpg",
    "university_id": null,
    "fields_of_study": [
      324
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-17T14:14:58.673Z",
    "updated_at": "2016-11-17T14:14:58.943Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/df607d0e8013e0ffe47f8c85c37cd043e46c18a7.jpg",
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

324
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 82b3a338c4898cd4b8a14f87c3c674dd668421387786d26609396ed355516758"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer bf360bc3f8c2257b4eae7fcf576dc4ecb3e23bdd811e953be124f4a980e3e574
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
      "bookmarkable_id": 102,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 103,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 104,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf360bc3f8c2257b4eae7fcf576dc4ecb3e23bdd811e953be124f4a980e3e574"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer e2fd725e1e22e2875c9736dca98041c532ee2642660f9c62f6a36bf55d02404f
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
      "title": "Campaign 2",
      "company_id": 5,
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
      "id": 3,
      "title": "Campaign 3",
      "company_id": 6,
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
	-H "Authorization: Bearer e2fd725e1e22e2875c9736dca98041c532ee2642660f9c62f6a36bf55d02404f"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 273dd4bb191fbeb6eebd653a0b6329d10ae987d2cd669daea8bd30cb524532ab
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 1,
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
	-H "Authorization: Bearer 273dd4bb191fbeb6eebd653a0b6329d10ae987d2cd669daea8bd30cb524532ab"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer ebe886e79844b67c6b0187a2bb1cdba9df256d7b3027ee1bcf374dd5f1914ed3
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
      "creator_id": 207,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-56",
      "html_url": "https://goskive.com/course/mit-course-56",
      "slug": "mit-course-56",
      "university_id": 62,
      "additional_university_ids": [

      ],
      "discipline_id": 62,
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
      "updated_at": "2016-11-17T14:13:52.968Z",
      "shortname": "mit-course-56",
      "topic_id": 62,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 208,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-57",
      "html_url": "https://goskive.com/course/mit-course-57",
      "slug": "mit-course-57",
      "university_id": 63,
      "additional_university_ids": [

      ],
      "discipline_id": 63,
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
      "updated_at": "2016-11-17T14:13:53.045Z",
      "shortname": "mit-course-57",
      "topic_id": 63,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebe886e79844b67c6b0187a2bb1cdba9df256d7b3027ee1bcf374dd5f1914ed3"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer e9e7a5b4458c570eb544357b1640698a0683be2815e9027a47b4703801c20b2f
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
        "id": 14,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-11-17T14:13:41.717Z",
        "updated_at": "2016-11-17T14:13:41.717Z",
        "file_url": "memory://ab64a98b4a40bc3d030734d2da6b7b17.pdf",
        "course_id": 28,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 15,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-17T14:13:41.801Z",
        "updated_at": "2016-11-17T14:13:41.801Z",
        "file_url": "memory://cdaf83b5604064ea9fccd90757b52321.pdf",
        "course_id": 29,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 16,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-17T14:13:41.876Z",
        "updated_at": "2016-11-17T14:13:41.876Z",
        "file_url": "memory://45d73157a36d67512f75f11770b3583e.pdf",
        "course_id": 30,
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
	-H "Authorization: Bearer e9e7a5b4458c570eb544357b1640698a0683be2815e9027a47b4703801c20b2f"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 853e86741abfb9fc64e2ffa4c4065aa9f5a9cfc318f8c8db9d6c6fc0f02ff2a3
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T14:14:32.798Z"
      },
      "created_at": "2016-11-17T14:14:32.801Z",
      "updated_at": "2016-11-17T14:14:32.801Z",
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
      "company_id": 16,
      "company": {
        "id": 16,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T14:14:32.809Z"
      },
      "created_at": "2016-11-17T14:14:32.813Z",
      "updated_at": "2016-11-17T14:14:32.813Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 853e86741abfb9fc64e2ffa4c4065aa9f5a9cfc318f8c8db9d6c6fc0f02ff2a3"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer df56dbeaa99b4d3461e7ea37ce03284b33dd4b465a84ea161c7a945ad5bb52a2
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
      "company_id": 11,
      "company": {
        "id": 11,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T14:14:32.624Z"
      },
      "created_at": "2016-11-17T14:14:32.629Z",
      "updated_at": "2016-11-17T14:14:32.629Z",
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
      "company_id": 12,
      "company": {
        "id": 12,
        "name": "Fake Company Name 11",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-17T14:14:32.644Z"
      },
      "created_at": "2016-11-17T14:14:32.648Z",
      "updated_at": "2016-11-17T14:14:32.648Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df56dbeaa99b4d3461e7ea37ce03284b33dd4b465a84ea161c7a945ad5bb52a2"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer aa022978d6491a523045e3176897314394a7fc3a188841c65e1f7d4c0a87aff6
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
      "id": 16,
      "created_at": "2016-11-17T14:14:23.241Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 15,
      "updated_at": "2016-11-17T14:14:23.345Z",
      "author_id": "579",
      "thread_subject_id": "157",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-11-17T14:14:23.334Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 16,
      "updated_at": "2016-11-17T14:14:23.348Z",
      "author_id": "582",
      "thread_subject_id": "158",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-11-17T14:14:23.713Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-11-17T14:14:23.713Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-11-17T14:14:24.095Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-11-17T14:14:24.095Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-11-17T14:14:24.486Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-11-17T14:14:24.486Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-11-17T14:14:24.793Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 84,
      "updated_at": "2016-11-17T14:14:24.793Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-11-17T14:14:25.103Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 85,
      "updated_at": "2016-11-17T14:14:25.103Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-11-17T14:14:25.413Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 86,
      "updated_at": "2016-11-17T14:14:25.413Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa022978d6491a523045e3176897314394a7fc3a188841c65e1f7d4c0a87aff6"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/24
Content-Type: application/json
Authorization: Bearer 8e3de606ebd9902b997a76c8ea7ee178604bef7ce4b888724b5d6b51a73aebac
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-17T14:04:25.000Z"}}
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
    "id": 24,
    "created_at": "2016-11-17T14:14:25.556Z",
    "read_at": "2016-11-17T14:04:25.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 17,
    "updated_at": "2016-11-17T14:14:25.596Z",
    "author_id": "607",
    "thread_subject_id": "165",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/24" -d '{"notification":{"read_at":"2016-11-17T14:04:25.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e3de606ebd9902b997a76c8ea7ee178604bef7ce4b888724b5d6b51a73aebac"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f6b0f9d1131645ccb4b08181b90c33dae75d6e1e5cd6df09fc2761c72ec56a63
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
      "course_id": 242,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-17T14:14:40.544Z",
      "course_published": true,
      "updated_at": "2016-11-17T14:14:40.537Z"
    },
    {
      "id": 5,
      "course_id": 243,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-17T14:14:40.624Z",
      "course_published": true,
      "updated_at": "2016-11-17T14:14:40.617Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6b0f9d1131645ccb4b08181b90c33dae75d6e1e5cd6df09fc2761c72ec56a63"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer a783e740c8a0a661e7410c2a20a428999f8306f9bc534cf37cf042cfacadff82
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
    "course_id": 241,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-17T14:14:40.398Z",
    "course_published": true,
    "updated_at": "2016-11-17T14:14:40.389Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a783e740c8a0a661e7410c2a20a428999f8306f9bc534cf37cf042cfacadff82"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer dbce155a56304fc1612832d739a9bd73c86920aa49752fdec1d10663b17a271f
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
    "course_id": 244,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-17T14:14:40.827Z",
    "course_published": true,
    "updated_at": "2016-11-17T14:14:40.817Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbce155a56304fc1612832d739a9bd73c86920aa49752fdec1d10663b17a271f"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 8c7688e413e209921f1f45184d3ffafc70520f19662436e627e2c68fcd6af284
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
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 98,
      "user_id": 733
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 99,
      "user_id": 733
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 733
    },
    {
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 101,
      "user_id": 733
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c7688e413e209921f1f45184d3ffafc70520f19662436e627e2c68fcd6af284"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/244
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
    "id": 244,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 244,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 244
      },
      {
        "id": 245,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 244
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/244" -X GET \
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
      "id": 245,
      "name": "Open-architected reciprocal moderator",
      "name_translations": {
        "en": "Open-architected reciprocal moderator"
      }
    },
    {
      "id": 246,
      "name": "Fundamental systematic hierarchy",
      "name_translations": {
        "en": "Fundamental systematic hierarchy"
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
PATCH /v2/feedbacks/26/close
Content-Type: application/json
Authorization: Bearer 0800e9ab4b0257062201794f4596475ece71f2a491d000d370594b8b9f1f066f
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
    "id": 26,
    "user_id": 344,
    "feedbackable_id": 19,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-17T14:14:05.121Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0800e9ab4b0257062201794f4596475ece71f2a491d000d370594b8b9f1f066f"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer f2714a8d876e45913aa206e308c75b2b2b42097c2fca5defd598db97b0a586fb
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
    "id": 5,
    "user_id": 253,
    "feedbackable_id": 17,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-17T14:13:58.603Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2714a8d876e45913aa206e308c75b2b2b42097c2fca5defd598db97b0a586fb"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/28
Content-Type: application/json
Authorization: Bearer 10b4376ccf454e23b58d50a20980f17c6d3710ddc9c8a34e01dfd3b36ac6702c
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
    "user_id": 354,
    "feedbackable_id": 21,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T14:14:05.747Z",
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
	-H "Authorization: Bearer 10b4376ccf454e23b58d50a20980f17c6d3710ddc9c8a34e01dfd3b36ac6702c"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/2/fix
Content-Type: application/json
Authorization: Bearer 416a0f2206511918503b4c633c4db3c4881d7682bf8ea16b3353b99586bfaf82
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
curl "api.goskive.com/v2/feedbacks/2/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 416a0f2206511918503b4c633c4db3c4881d7682bf8ea16b3353b99586bfaf82"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/fix
Content-Type: application/json
Authorization: Bearer f1beb84a15cec0f2ff07ab0420ce92368b3f6f9c756c8c7886f2fd0f4b9d2e53
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
curl "api.goskive.com/v2/feedbacks/3/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1beb84a15cec0f2ff07ab0420ce92368b3f6f9c756c8c7886f2fd0f4b9d2e53"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/close
Content-Type: application/json
Authorization: Bearer 674b97a8acd39eb568fa337095f01d231357302623b08c6773016c70a31d42fe
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
curl "api.goskive.com/v2/feedbacks/25/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 674b97a8acd39eb568fa337095f01d231357302623b08c6773016c70a31d42fe"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/29
Content-Type: application/json
Authorization: Bearer 0f93b86ac6debe13a9aae2fdaa3fc9985a9c2ba520ced03301b4f59ec4e6aebd
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
    "user_id": 359,
    "feedbackable_id": 22,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T14:14:06.086Z",
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
	-H "Authorization: Bearer 0f93b86ac6debe13a9aae2fdaa3fc9985a9c2ba520ced03301b4f59ec4e6aebd"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 31381165bc53e9027ae4986a3e90ce7f652c1c02357e8fc9d50800dd65e91d4c
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31381165bc53e9027ae4986a3e90ce7f652c1c02357e8fc9d50800dd65e91d4c"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/1/bookmark
Content-Type: application/json
Authorization: Bearer d8a347344ef3d15fbd7c6026cd0a60559cec912eb4b40ee4b5fd23298ec54fe1
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/1/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8a347344ef3d15fbd7c6026cd0a60559cec912eb4b40ee4b5fd23298ec54fe1"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer f16adb03d8ef32a1efedd944e562ba3faae5ee7e1ecbd3dec6810589937d36dc
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f16adb03d8ef32a1efedd944e562ba3faae5ee7e1ecbd3dec6810589937d36dc"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/2
Content-Type: application/json
Authorization: Bearer 185abb412e68ca8596166fbbebe40be865968944a4e89aa15c332815ffc2eac9
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/850d2b6d1419af35d23e4498cd4df091.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161117%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161117T141334Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=720e1a80bdff3ce166221ec3d405ac918e714e4b850e279e097068c005a315cd",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 185abb412e68ca8596166fbbebe40be865968944a4e89aa15c332815ffc2eac9"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/3/preview
Content-Type: application/json
Authorization: Bearer 714777c91fc0b4761f0c3d7d6aa7b3372a94f254dcd226c688a6e3f7e3fe440b
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/64ebe0147bd7a7b958d76d98b81be9a7.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161117%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161117T141334Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=9a69861e6ce3f1fc4b54e3014ec4bfd293fcdeb52ac3d3d72c282b170d5d292a",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/3/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 714777c91fc0b4761f0c3d7d6aa7b3372a94f254dcd226c688a6e3f7e3fe440b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 59a57c1a2d8796751fd20d347e4c47a0908d8392b06851ea5b104253a42493ad
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
    "id": 11,
    "uploader": {
      "id": 29,
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
      "created_at": "2016-11-17T14:13:35.577Z",
      "updated_at": "2016-11-17T14:13:35.577Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-17T14:13:35.652Z",
    "updated_at": "2016-11-17T14:13:35.652Z",
    "course_id": 11,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59a57c1a2d8796751fd20d347e4c47a0908d8392b06851ea5b104253a42493ad"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/17/matched_courses?required_cu_count=2
Authorization: Bearer 7e8ee4eed134a244013b3876725f451234c1203631cacc56f683db534765c95f
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
      "creator_id": 225,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-49fa158a-1a9a-4a3f-87e0-bd5b8313f07d",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-49fa158a-1a9a-4a3f-87e0-bd5b8313f07d",
      "slug": "mit-the-great-british-bake-off-49fa158a-1a9a-4a3f-87e0-bd5b8313f07d",
      "university_id": 68,
      "additional_university_ids": [

      ],
      "discipline_id": 68,
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
      "chapters_updated_at": "2016-11-17T14:13:53.105Z",
      "updated_at": "2016-11-17T14:13:56.628Z",
      "shortname": "mit-the-great-british-bake-off-49fa158a-1a9a-4a3f-87e0-bd5b8313f07d",
      "topic_id": 68,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 220,
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 67,
      "additional_university_ids": [

      ],
      "discipline_id": 67,
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
      "chapters_updated_at": "2016-11-17T14:13:53.105Z",
      "updated_at": "2016-11-17T14:13:56.064Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 67,
      "language_code": "en",
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
curl "api.goskive.com/v2/files/17/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 7e8ee4eed134a244013b3876725f451234c1203631cacc56f683db534765c95f"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/4/download
Content-Type: application/json
Authorization: Bearer 2d82de8c8ac3068925db19b68b6b4d43ea5b1ef11a35e4ac312abedd624cdeeb
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d82de8c8ac3068925db19b68b6b4d43ea5b1ef11a35e4ac312abedd624cdeeb"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/12/report
Content-Type: application/json
Authorization: Bearer 74b5f123b3b541f1740bd56b9fd671633f8caaf2fb6dbdfda011c09880e16f2d
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74b5f123b3b541f1740bd56b9fd671633f8caaf2fb6dbdfda011c09880e16f2d"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/5/bookmark
Content-Type: application/json
Authorization: Bearer 562342715c35aea07243fdad870cbe3b010fd761c519832db4cc3a103df048b4
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 562342715c35aea07243fdad870cbe3b010fd761c519832db4cc3a103df048b4"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/13/upvote
Content-Type: application/json
Authorization: Bearer 394f2ee450828f7c3087e61a69ed54d8fc44ad197b345712967b8213bad5edf8
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 394f2ee450828f7c3087e61a69ed54d8fc44ad197b345712967b8213bad5edf8"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/7/comments
Content-Type: application/json
Authorization: Bearer d96c60fa9ac67ce817546048c9e0534d2fe7e3d748f0781c8d7b341db40eadb6
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
    "id": 6,
    "author_id": 196,
    "reply_to_id": null,
    "created_at": "2016-11-17T14:13:52.130Z",
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
curl "api.goskive.com/v2/flashcards/7/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d96c60fa9ac67ce817546048c9e0534d2fe7e3d748f0781c8d7b341db40eadb6"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/8/comments
Content-Type: application/json
Authorization: Bearer 301e0be96b932fd9f2841a25886a984343ed54f08594da110873b267ed902a98
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
    "id": 7,
    "author_id": 199,
    "reply_to_id": null,
    "created_at": "2016-11-17T14:13:52.478Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 199,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:13:52.474Z",
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
curl "api.goskive.com/v2/flashcards/8/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 301e0be96b932fd9f2841a25886a984343ed54f08594da110873b267ed902a98"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/4/comments
Content-Type: application/json
Authorization: Bearer b7b58aeb64044847ccec346eed68450ad1d89bd1a386f6a5fb26b355b5f4f86c
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
      "author_id": 188,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:13:51.524Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 189,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:13:51.542Z",
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
curl "api.goskive.com/v2/flashcards/4/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7b58aeb64044847ccec346eed68450ad1d89bd1a386f6a5fb26b355b5f4f86c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/6/comments
Content-Type: application/json
Authorization: Bearer 36c1132488ff066bed62d8e5e98e43bc90c1df7b10be6abab3fa92ee1ed1adf1
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
curl "api.goskive.com/v2/flashcards/6/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36c1132488ff066bed62d8e5e98e43bc90c1df7b10be6abab3fa92ee1ed1adf1"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/57/feedbacks
Content-Type: application/json
Authorization: Bearer cf014a4953609ef6f4daec628ffbf462a0147ecb5238309ec559d37aff6baf36
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
    "id": 46,
    "user_id": 642,
    "feedbackable_id": 57,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-17T14:14:27.266Z",
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
curl "api.goskive.com/v2/flashcards/57/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf014a4953609ef6f4daec628ffbf462a0147ecb5238309ec559d37aff6baf36"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/53/feedbacks
Content-Type: application/json
Authorization: Bearer 90ab15b30bef17c6bfac582ef22ba7a7c8391ce4a8a53413ceca765955f37cb3
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
      "id": 42,
      "user_id": 624,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:26.287Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 623,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:26.277Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90ab15b30bef17c6bfac582ef22ba7a7c8391ce4a8a53413ceca765955f37cb3"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/2/votes
Content-Type: application/json
Authorization: Bearer 3f8116cf238c8c8fb69ec655c23f1d835ca81509734a8672a3429ece0075332a
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
      "id": 5,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 72
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 71
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 70
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f8116cf238c8c8fb69ec655c23f1d835ca81509734a8672a3429ece0075332a"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/45/republish
Content-Type: application/json
Authorization: Bearer 5a6150a8f22511f1ea5fe006730b7cc0fda3c8d07bccba556a93937575a13955
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
curl "api.goskive.com/v2/flashcards/45/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a6150a8f22511f1ea5fe006730b7cc0fda3c8d07bccba556a93937575a13955"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/bookmark
Content-Type: application/json
Authorization: Bearer 8104f811d80c46bff4e1197da92ac40b1c2af7b3e1ed55cb0e3d0165059c8d22
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
	-H "Authorization: Bearer 8104f811d80c46bff4e1197da92ac40b1c2af7b3e1ed55cb0e3d0165059c8d22"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/40
Content-Type: application/json
Authorization: Bearer d0f5634baf8a66ff61d7c57574f9b74fbbdeb8fc526ad6496fd6058014e452e1
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0f5634baf8a66ff61d7c57574f9b74fbbdeb8fc526ad6496fd6058014e452e1"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/downvote
Content-Type: application/json
Authorization: Bearer c4902e2e39ff05ac921567bd190eeeab7577ee4973fa99d2666139fbf3f338cb
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4902e2e39ff05ac921567bd190eeeab7577ee4973fa99d2666139fbf3f338cb"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/46
Content-Type: application/json
Authorization: Bearer ea47231c5a2e6e822398acd9a61782bd24cbf744a4b22038bc64742e302adca5
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
    "author_id": 519,
    "chapter_id": 114,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:14:19.859Z",
    "created_at": "2016-11-17T14:14:19.859Z",
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
	-H "Authorization: Bearer ea47231c5a2e6e822398acd9a61782bd24cbf744a4b22038bc64742e302adca5"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/report
Content-Type: application/json
Authorization: Bearer e23846f410e0522fd357cff418e04dc68f61f28363a62320e41e1f1dd4e72a03
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e23846f410e0522fd357cff418e04dc68f61f28363a62320e41e1f1dd4e72a03"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/39/bookmark
Content-Type: application/json
Authorization: Bearer 208ab86fea9bdbe52b5904f9c817106fb24c88ecf1e23f5b6548c4febfa52ca1
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 208ab86fea9bdbe52b5904f9c817106fb24c88ecf1e23f5b6548c4febfa52ca1"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/43/upvote
Content-Type: application/json
Authorization: Bearer 323c58166abc1d30efbbe767b0b0cb270c8aa24182e39ed80eac98709e24f7e0
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 323c58166abc1d30efbbe767b0b0cb270c8aa24182e39ed80eac98709e24f7e0"
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
    "key": "cache/2ec51417985b7b5d5a1ba2ac8f19ecb5.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xN1QxNToxNDozMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzJlYzUxNDE3OTg1YjdiNWQ1YTFiYTJhYzhmMTllY2I1LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExNy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMTdUMTQxNDMyWiJ9XX0=",
    "x-amz-credential": "FAKE/20161117/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161117T141432Z",
    "x-amz-signature": "31fa619a58ebed6c8ca8f2633b4887d431821c1337820e2db980ef7a2b47c66e"
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
Authorization: Bearer b088f1c19e93a3630c85643966639cf03e46c23b8bc7b914c0b389f174b6299e
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
	-H "Authorization: Bearer b088f1c19e93a3630c85643966639cf03e46c23b8bc7b914c0b389f174b6299e"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer f2c2cbbf482c23ac097d5f56fd2e8fd26a849b827be99db90e48620414df9734
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
	-H "Authorization: Bearer f2c2cbbf482c23ac097d5f56fd2e8fd26a849b827be99db90e48620414df9734"
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
{"password":{"reset_password_token":"y9cvBz8Zay1J19YxWHhk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 367,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-17T14:14:07.250Z",
  "updated_at": "2016-11-17T14:14:07.424Z",
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
  "audit_id": 4515
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"y9cvBz8Zay1J19YxWHhk","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/62/comments
Content-Type: application/json
Authorization: Bearer 8e4e60283897c3e811a9875bc060cc582c2ec942dc46d6dec4b1c259a8f5f34d
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
    "id": 12,
    "author_id": 385,
    "reply_to_id": null,
    "created_at": "2016-11-17T14:14:09.285Z",
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
curl "api.goskive.com/v2/questions/62/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e4e60283897c3e811a9875bc060cc582c2ec942dc46d6dec4b1c259a8f5f34d"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/61/comments
Content-Type: application/json
Authorization: Bearer 90afce5579928db5826613a4184294d12ffa73a30110138af782d0fa97b1a01c
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
    "id": 11,
    "author_id": 382,
    "reply_to_id": null,
    "created_at": "2016-11-17T14:14:08.807Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 30,
      "user_id": 382,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:08.805Z",
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
curl "api.goskive.com/v2/questions/61/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90afce5579928db5826613a4184294d12ffa73a30110138af782d0fa97b1a01c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/59/comments
Content-Type: application/json
Authorization: Bearer c519338f0342a52bf18abb44f93377af47e75116a2d8bb0796b59efded68ca80
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
      "id": 10,
      "author_id": 378,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:08.106Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 377,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:08.088Z",
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
curl "api.goskive.com/v2/questions/59/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c519338f0342a52bf18abb44f93377af47e75116a2d8bb0796b59efded68ca80"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/60/comments
Content-Type: application/json
Authorization: Bearer e6d0eaeb2ce7147700c1a3f7a472a8a675edb2fabd9f897c6c61a69fad2eb5e1
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
curl "api.goskive.com/v2/questions/60/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6d0eaeb2ce7147700c1a3f7a472a8a675edb2fabd9f897c6c61a69fad2eb5e1"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/70/feedbacks
Content-Type: application/json
Authorization: Bearer 5bb6ba603e11d26a8a751fb476eb17f9569f4dfdf65bce3b61eed42e7914b444
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
    "id": 38,
    "user_id": 421,
    "feedbackable_id": 70,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-17T14:14:12.402Z",
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
curl "api.goskive.com/v2/questions/70/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bb6ba603e11d26a8a751fb476eb17f9569f4dfdf65bce3b61eed42e7914b444"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/65/feedbacks
Content-Type: application/json
Authorization: Bearer 809c221a8e86e85f864a1d9c9309ae088c57db19de2868aae0cb60b42530e9f2
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
      "id": 34,
      "user_id": 400,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:10.450Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 399,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:10.438Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/65/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 809c221a8e86e85f864a1d9c9309ae088c57db19de2868aae0cb60b42530e9f2"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/105/votes
Content-Type: application/json
Authorization: Bearer 49a4bf1db37a5949b47a0a91416ddd224bb19a84967fe8aea9de871082aaed76
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
      "votable_id": 105,
      "user_id": 813
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 812
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 811
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/105/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49a4bf1db37a5949b47a0a91416ddd224bb19a84967fe8aea9de871082aaed76"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/8/republish
Content-Type: application/json
Authorization: Bearer a70cf317badfe61e4f42fd2783098e5318a4222e13e15de3edfdefdb501cf7b0
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
curl "api.goskive.com/v2/questions/8/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a70cf317badfe61e4f42fd2783098e5318a4222e13e15de3edfdefdb501cf7b0"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/6/bookmark
Content-Type: application/json
Authorization: Bearer 13f176a62c40eaa6ebcacbfd67009cbfe12904458c49fac14225ec9a88c06dc6
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/6/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13f176a62c40eaa6ebcacbfd67009cbfe12904458c49fac14225ec9a88c06dc6"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/28
Content-Type: application/json
Authorization: Bearer ff62645c07baad198fe8f159d27e7b97b900545101356176a5ef2c5572a6504d
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/28" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff62645c07baad198fe8f159d27e7b97b900545101356176a5ef2c5572a6504d"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/27/downvote
Content-Type: application/json
Authorization: Bearer 8dac5d49a6f9f028635da126a9e92c6ab47056127dce4ff7d560e8155c69fa88
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8dac5d49a6f9f028635da126a9e92c6ab47056127dce4ff7d560e8155c69fa88"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/24
Content-Type: application/json
Authorization: Bearer a5ab7ddf1039dbd2de4dd296f143377819ecc1bb550d8b7f423e0001487de0bc
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
    "id": 24,
    "obfuscated_id": "KHM5yo_z4Ds",
    "author_id": 164,
    "chapter_id": 27,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:13:48.171Z",
    "created_at": "2016-11-17T14:13:48.031Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5ab7ddf1039dbd2de4dd296f143377819ecc1bb550d8b7f423e0001487de0bc"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/26/report
Content-Type: application/json
Authorization: Bearer a84f2c1fea0a788b614c02f30ad13353451ef5120162d67a216a1f1adfb7afda
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/26/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a84f2c1fea0a788b614c02f30ad13353451ef5120162d67a216a1f1adfb7afda"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/25/bookmark
Content-Type: application/json
Authorization: Bearer 5f2bfb3c331e8c1b88c2ef5fed68eb60682401d316e71799a3133dccb3c6640c
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/25/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f2bfb3c331e8c1b88c2ef5fed68eb60682401d316e71799a3133dccb3c6640c"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/30
Content-Type: application/json
Authorization: Bearer 1a7670288a38ea0cd83dd3462857066764f4c9f1cb6453a209629cf2a10a5870
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":30,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-17T14:13:50.778Z","updated_at":"2016-11-17T14:13:50.915Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":33,"author_id":182,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 182,
    "chapter_id": 33,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-17T14:13:51.034Z",
    "created_at": "2016-11-17T14:13:50.778Z",
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
    "question": "{\"id\"=>30, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-17T14:13:50.778Z\", \"updated_at\"=>\"2016-11-17T14:13:50.915Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>33, \"author_id\"=>182, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 59,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 60,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 61,
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
curl "api.goskive.com/v2/questions/30" -d '{"question":{"question":{"id":30,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-17T14:13:50.778Z","updated_at":"2016-11-17T14:13:50.915Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":33,"author_id":182,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a7670288a38ea0cd83dd3462857066764f4c9f1cb6453a209629cf2a10a5870"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/29/upvote
Content-Type: application/json
Authorization: Bearer 63d06474294c9b5a68602745fc9d29cd152232ed0e3fd96aefb002b4e6197379
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/29/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63d06474294c9b5a68602745fc9d29cd152232ed0e3fd96aefb002b4e6197379"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer c5196c6dccf5efaebf89d8d6635eb0176adde5eec60a851210fc63306b2807e7
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
      "creator_id": 764,
      "id": 234,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 219,
      "additional_university_ids": [

      ],
      "discipline_id": 237,
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
      "updated_at": "2016-11-17T14:14:39.155Z",
      "shortname": "mit-pizza-201",
      "topic_id": 237,
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
	-H "Authorization: Bearer c5196c6dccf5efaebf89d8d6635eb0176adde5eec60a851210fc63306b2807e7"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 4e545afb01877e354b08d5e5830ed82c9fefd28e22a18aed75cc8991f5f0ea8e
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
      "id": 217,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-197",
      "html_url": "https://goskive.com/university/uni-197",
      "slug": "uni-197",
      "name": "National School of Pizza",
      "short_name": "Uni 197",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8cb4db6d7b555aba0cd49b30c54c908dfe5a1f50.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1f25aa3cef977a905b0a2b50dde4180d0b7132c9.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T14:14:38.987Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 216,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-196",
      "html_url": "https://goskive.com/university/uni-196",
      "slug": "uni-196",
      "name": "National School of Pastry",
      "short_name": "Uni 196",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d46c6532c389f77b9e21834b5e0d77da65d18530.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/fd78c270a0dfbb5020eea2eec32648f0904619f8.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T14:14:38.970Z",
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
	-H "Authorization: Bearer 4e545afb01877e354b08d5e5830ed82c9fefd28e22a18aed75cc8991f5f0ea8e"
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
      "id": 229,
      "name": "Implemented reciprocal synergy",
      "name_translations": {
        "en": "Implemented reciprocal synergy"
      },
      "discipline_id": 229
    },
    {
      "id": 230,
      "name": "Optimized mobile info-mediaries",
      "name_translations": {
        "en": "Optimized mobile info-mediaries"
      },
      "discipline_id": 230
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
GET /v2/topics/231
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
    "id": 231,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 231
  }
}
```



```shell
curl "api.goskive.com/v2/topics/231" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer b19bfdd5268daf6460e0567e54bf1fa96b4cb810561280eb5e9a99027b14b0b4
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
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-191",
      "html_url": "https://goskive.com/university/uni-191",
      "slug": "uni-191",
      "name": "University 155",
      "short_name": "Uni 191",
      "acronym": "MIT",
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
      "updated_at": "2016-11-17T14:14:38.303Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-190",
      "html_url": "https://goskive.com/university/uni-190",
      "slug": "uni-190",
      "name": "University 154",
      "short_name": "Uni 190",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/80d702cfb8e72a69d8d05f8e08a870b3bc13ea2d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/bfff9977589a73d0f8ea06b648e77142051d97bd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T14:14:38.286Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-189",
      "html_url": "https://goskive.com/university/uni-189",
      "slug": "uni-189",
      "name": "University 153",
      "short_name": "Uni 189",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/94a8023f21254ce163a5b5ede98bdc819440a3a0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6d49f3aa5d676dcd5fa043f4ff8e782f8f1ac73f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-17T14:14:38.269Z",
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
	-H "Authorization: Bearer b19bfdd5268daf6460e0567e54bf1fa96b4cb810561280eb5e9a99027b14b0b4"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1ea7a1c7d6f7d2a839647f82ac2472fbee73d1a6a2909b21d503ecf9b1352540
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
    "id": 208,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c1bcbe98f5e30a1d2c062d00e265207a3c76c1d6.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3db8b7a7fd23a5908ee95827523b8d2a965fac10.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-17T14:14:38.172Z",
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
	-H "Authorization: Bearer 1ea7a1c7d6f7d2a839647f82ac2472fbee73d1a6a2909b21d503ecf9b1352540"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ba485ae6aff30374ef135339188add45323486947815b0307afa2e9bf60f3b1d
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":175,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 646,
    "id": 175,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 175,
    "additional_university_ids": [

    ],
    "discipline_id": 175,
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
    "chapters_updated_at": "2016-11-17T14:14:27.573Z",
    "updated_at": "2016-11-17T14:14:27.721Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 153,
        "updated_at": "2016-11-17T14:14:27.677Z",
        "course_id": 175,
        "author_id": 646,
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
        "id": 154,
        "updated_at": "2016-11-17T14:14:27.695Z",
        "course_id": 175,
        "author_id": 646,
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
        "id": 155,
        "updated_at": "2016-11-17T14:14:27.712Z",
        "course_id": 175,
        "author_id": 646,
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
    "topic_id": 175,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":175,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba485ae6aff30374ef135339188add45323486947815b0307afa2e9bf60f3b1d"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5d554ebbf87efeb05685de58169ca085448c2aac84eef15e5eeca0c5f2366588
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":176,"published":false}}
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
    "creator_id": 647,
    "id": 176,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 176,
    "additional_university_ids": [

    ],
    "discipline_id": 176,
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
    "updated_at": "2016-11-17T14:14:28.057Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 176,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":176,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d554ebbf87efeb05685de58169ca085448c2aac84eef15e5eeca0c5f2366588"
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
      "creator_id": 674,
      "id": 200,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "discipline_id": 200,
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
      "updated_at": "2016-11-17T14:14:30.503Z",
      "shortname": "fu-course-163",
      "topic_id": 200,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 674,
      "id": 201,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-164",
      "html_url": "https://goskive.com/course/fu-course-164",
      "slug": "fu-course-164",
      "university_id": 186,
      "additional_university_ids": [

      ],
      "discipline_id": 201,
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
      "chapters_updated_at": "2016-11-17T14:14:30.362Z",
      "updated_at": "2016-11-17T14:14:30.805Z",
      "shortname": "fu-course-164",
      "topic_id": 201,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 164",
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
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5a5e08775ae3f6215381ffa0e3e192923c973e952b89f283bca620c725b8b726
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
      "creator_id": 681,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-171",
      "html_url": "https://goskive.com/course/fu-course-171",
      "slug": "fu-course-171",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "discipline_id": 208,
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
      "updated_at": "2016-11-17T14:14:31.259Z",
      "shortname": "fu-course-171",
      "topic_id": 208,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 171",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 681,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "discipline_id": 209,
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
      "chapters_updated_at": "2016-11-17T14:14:31.112Z",
      "updated_at": "2016-11-17T14:14:31.559Z",
      "shortname": "fu-course-172",
      "topic_id": 209,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 172",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a5e08775ae3f6215381ffa0e3e192923c973e952b89f283bca620c725b8b726"
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
      "creator_id": 679,
      "id": 204,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 188,
      "additional_university_ids": [

      ],
      "discipline_id": 204,
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
      "updated_at": "2016-11-17T14:14:31.035Z",
      "shortname": "fu-course-167",
      "topic_id": 204,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 679,
      "id": 205,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 188,
      "additional_university_ids": [

      ],
      "discipline_id": 205,
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
      "updated_at": "2016-11-17T14:14:31.077Z",
      "shortname": "fu-course-168",
      "topic_id": 205,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
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
Authorization: Bearer 8fd159096c57348e0567c6e38374206b30117f8b0d2646087fac1365e6388d65
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
      "creator_id": 688,
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-175",
      "html_url": "https://goskive.com/course/fu-course-175",
      "slug": "fu-course-175",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "discipline_id": 212,
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
      "updated_at": "2016-11-17T14:14:31.839Z",
      "shortname": "fu-course-175",
      "topic_id": 212,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 688,
      "id": 213,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "discipline_id": 213,
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
      "updated_at": "2016-11-17T14:14:31.880Z",
      "shortname": "fu-course-176",
      "topic_id": 213,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fd159096c57348e0567c6e38374206b30117f8b0d2646087fac1365e6388d65"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer a49dea9b90894e788c484606f16df7461d679010e10cd16aa7a78391801efc83
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
  "id": 690,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-17T14:14:32.001Z",
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
	-H "Authorization: Bearer a49dea9b90894e788c484606f16df7461d679010e10cd16aa7a78391801efc83"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/801
Content-Type: application/json
Authorization: Bearer a6f39071530677059767d7ebefeca9276aefc547ea0e67a8cc4f0c333af5c7b4
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
    "id": 801,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 234,
    "fields_of_study": [
      255,
      256
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-17T14:14:42.608Z",
    "updated_at": "2016-11-17T14:14:42.608Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/801" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6f39071530677059767d7ebefeca9276aefc547ea0e67a8cc4f0c333af5c7b4"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/803
Content-Type: application/json
Authorization: Bearer 449b82a1e64a0379ab7b372998adf439a43df00f6b6cdd54a892eb468bab6f72
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
    "id": 803,
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
    "created_at": "2016-11-17T14:14:42.696Z",
    "updated_at": "2016-11-17T14:14:42.696Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/803" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 449b82a1e64a0379ab7b372998adf439a43df00f6b6cdd54a892eb468bab6f72"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/7
Content-Type: application/json
Authorization: Bearer 8bc19c518754dfaaf4356d0dd319cf34fed818ca18354f9b9ec8357aea86b53e
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8bc19c518754dfaaf4356d0dd319cf34fed818ca18354f9b9ec8357aea86b53e"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/8
Content-Type: application/json
Authorization: Bearer 19ec722c5d5b3d7af14b90e7f0f3fa0ac488e14e6452f8bbbd06ca75ae1c44d4
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
    "id": 8,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 5,
    "user_id": 84
  }
}
```



```shell
curl "api.goskive.com/v2/votes/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19ec722c5d5b3d7af14b90e7f0f3fa0ac488e14e6452f8bbbd06ca75ae1c44d4"
```
