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
Authorization: Basic MDRiNzk1NDNlZTY2OGFjMWZiMDA3MDdhOTRkNjg5MWI0OGIxODZjNTEzZmNh
MzU2OTMzYjczMWQyZjFiN2FiMDo5N2U0YmUyMTAzZTI5MWY1ZjE2N2E4NzYz
NTZiNTI2M2I1NzAwNWUxNzlkYzY4MWIyZWJmZGQ0YTY0YTNhMzNh

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
	-u 04b79543ee668ac1fb00707a94d6891b48b186c513fca356933b731d2f1b7ab0:97e4be2103e291f5f167a876356b5263b57005e179dc681b2ebfdd4a64a3a33a
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"b648d48b1f9adb4437051e5880686216ce5b0475da1022fea2e2796e2928e6a4","client_secret":"d8ae31d547f7d1ad38525917182a717a45cc202fffefa5f0dfa6e010189ceec3"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"b648d48b1f9adb4437051e5880686216ce5b0475da1022fea2e2796e2928e6a4","client_secret":"d8ae31d547f7d1ad38525917182a717a45cc202fffefa5f0dfa6e010189ceec3"}' -X POST \
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
Authorization: Basic Mjg2OTUxNmM0MjdhNWYzZDlmYjk0MGI4M2MzZWI3MGVhZDdlNzU1ZDMyMWIz
NjE5MWNjZTVlNThhMTZiZjJlNzo3MGVhMDk4NzlmYTQ0YjRhYmNiNmYyYzdm
ZmM0YWUzMTc4YTBmYjc0MDA3MjQ0ZjRlNzQ2ZjI0ODQyNWI3ODYw

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
  "access_token": "31cea85eff965d0dcd19756f12baa69669d0fa6ad423f94fe1899fb1fdb33c9d",
  "token_type": "bearer",
  "created_at": 1476793566
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 2869516c427a5f3d9fb940b83c3eb70ead7e755d321b36191cce5e58a16bf2e7:70ea09879fa44b4abcb6f2c7ffc4ae3178a0fb74007244f4e746f248425b7860
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"abca323c6cce0ee26bfc8442650836c11b4ed6752fae61bf9ecc6640e7f6fdff","client_secret":"b033f690e1c687d990f58072ec5cf45c9527e31e2f1baac2cc7340265abbcb4f"}
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
  "access_token": "7c759d0fc240b3752ad34a352a05910738261e0d7a499cd69734f95b25b757f6",
  "token_type": "bearer",
  "created_at": 1476793566
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"abca323c6cce0ee26bfc8442650836c11b4ed6752fae61bf9ecc6640e7f6fdff","client_secret":"b033f690e1c687d990f58072ec5cf45c9527e31e2f1baac2cc7340265abbcb4f"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"04a3b02f8a0a621c20c33a865929f2f2690288157c8061c06a5fe2c7fb52e2c4","client_secret":"231d4fa1203d7d3dc1cec47801d5393eaf1786d60bf22e734de5a0e331f3b2d8"}
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
  "access_token": "97e38469aef0e55b9671fc818a5552749b238d3559f2d0612d3b0ebdd0c39d47",
  "token_type": "bearer",
  "created_at": 1476793566
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"04a3b02f8a0a621c20c33a865929f2f2690288157c8061c06a5fe2c7fb52e2c4","client_secret":"231d4fa1203d7d3dc1cec47801d5393eaf1786d60bf22e734de5a0e331f3b2d8"}' -X POST \
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
Authorization: Bearer 047edb8e65dcfe3d7c9c68f6c0735c6d4aae115f0b162ff3e4cd157d072be045
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
    "company_id": 4,
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
	-H "Authorization: Bearer 047edb8e65dcfe3d7c9c68f6c0735c6d4aae115f0b162ff3e4cd157d072be045"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/38/flashcards
Content-Type: application/json
Authorization: Bearer 0a08b7837b41e8e99dbd1ece0d441c08ec4209a85173ef72da1384fcd016a4fc
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":38,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 127,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:24:55.901Z",
    "created_at": "2016-10-18T12:24:55.901Z",
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
curl "api.goskive.com/v2/chapters/38/flashcards" -d '{"flashcard":{"chapter_id":38,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a08b7837b41e8e99dbd1ece0d441c08ec4209a85173ef72da1384fcd016a4fc"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/40/flashcards
Content-Type: application/json
Authorization: Bearer eeb8c52cee003873cb35d0fa866e9e00a303acef652be123a609143ae2976378
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
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 131,
      "chapter_id": 40,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:24:56.201Z",
      "created_at": "2016-10-18T12:24:56.201Z",
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
      "author_id": 131,
      "chapter_id": 40,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:24:56.240Z",
      "created_at": "2016-10-18T12:24:56.240Z",
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
      "author_id": 131,
      "chapter_id": 40,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:24:56.278Z",
      "created_at": "2016-10-18T12:24:56.278Z",
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
curl "api.goskive.com/v2/chapters/40/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eeb8c52cee003873cb35d0fa866e9e00a303acef652be123a609143ae2976378"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/130/questions
Content-Type: application/json
Authorization: Bearer 02bea02331bc3f91a685556a86970500fb10fd19c1eeb075411daa6a8ccbac4e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":130,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 628,
    "chapter_id": 130,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:42.339Z",
    "created_at": "2016-10-18T12:25:42.339Z",
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
        "id": 187,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 188,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 189,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 190,
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
curl "api.goskive.com/v2/chapters/130/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":130,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02bea02331bc3f91a685556a86970500fb10fd19c1eeb075411daa6a8ccbac4e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/131/questions
Content-Type: application/json
Authorization: Bearer a253322c85c9b25ef263bac258a474466f69bc7ceebc27cdd9b4e7a322bb1e69
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 94,
    "obfuscated_id": "CVi6VU_nV6k",
    "author_id": 631,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:42.882Z",
    "created_at": "2016-10-18T12:25:42.882Z",
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
        "id": 191,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 192,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/131/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a253322c85c9b25ef263bac258a474466f69bc7ceebc27cdd9b4e7a322bb1e69"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/132/questions
Content-Type: application/json
Authorization: Bearer 2581d46fd03d34b2ce0bc440b28c4f2b31b5fd40ef37dfca6692685e44b3305b
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":132,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 95,
    "obfuscated_id": "uTOhBSQK4CI",
    "author_id": 634,
    "chapter_id": 132,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:43.251Z",
    "created_at": "2016-10-18T12:25:43.251Z",
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
        "id": 193,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 194,
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
curl "api.goskive.com/v2/chapters/132/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":132,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2581d46fd03d34b2ce0bc440b28c4f2b31b5fd40ef37dfca6692685e44b3305b"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/129/questions
Content-Type: application/json
Authorization: Bearer d96a8a7b9ca0161acbdbc682295a1740a55998c927e4e5001868d8d49d53d8c8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":129,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 92,
    "obfuscated_id": "__OphzZQiQY",
    "author_id": 625,
    "chapter_id": 129,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:41.896Z",
    "created_at": "2016-10-18T12:25:41.896Z",
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
        "id": 184,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 185,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 186,
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
curl "api.goskive.com/v2/chapters/129/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":129,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d96a8a7b9ca0161acbdbc682295a1740a55998c927e4e5001868d8d49d53d8c8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/128/questions
Content-Type: application/json
Authorization: Bearer b4b2c55e5b1e976b3622f3e7ebc9ddb2eb3f083fce946bd1212bccbbfc46edf4
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 619,
      "chapter_id": 128,
      "position": 80,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:41.168Z",
      "created_at": "2016-10-18T12:25:41.042Z",
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
          "id": 178,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 179,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 620,
      "chapter_id": 128,
      "position": 81,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:41.376Z",
      "created_at": "2016-10-18T12:25:41.248Z",
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
      "author_id": 621,
      "chapter_id": 128,
      "position": 82,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:25:41.587Z",
      "created_at": "2016-10-18T12:25:41.455Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/128/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4b2c55e5b1e976b3622f3e7ebc9ddb2eb3f083fce946bd1212bccbbfc46edf4"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/137
Content-Type: application/json
Authorization: Bearer d0c08c18d2cc8e1a7b0818e503f92742b6777c4c4715d69d76e8aa7e9d3969e0
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
curl "api.goskive.com/v2/chapters/137" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0c08c18d2cc8e1a7b0818e503f92742b6777c4c4715d69d76e8aa7e9d3969e0"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/138
Content-Type: application/json
Authorization: Bearer c56d12a57d6d10013589ee93b8aaa453dfaaa64712faba5fc3f02ca7369ecde4
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
curl "api.goskive.com/v2/chapters/138" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c56d12a57d6d10013589ee93b8aaa453dfaaa64712faba5fc3f02ca7369ecde4"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/140
Content-Type: application/json
Authorization: Bearer f0d88f4cd397200d1c0558601b27342120b339c91bbf612870229a0a39fdbb52
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
curl "api.goskive.com/v2/chapters/140" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0d88f4cd397200d1c0558601b27342120b339c91bbf612870229a0a39fdbb52"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/136
Content-Type: application/json
Authorization: Bearer 552240bcddf2920162d2f4944e9bbc1dd32c6c636b13af0333a191ad2702de79
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/136" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 552240bcddf2920162d2f4944e9bbc1dd32c6c636b13af0333a191ad2702de79"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/133
Content-Type: application/json
Authorization: Bearer 85d4b7342e58c9dbb02ee27d8fddc048025de724d40acb5cf18a673b14106430
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
    "id": 133,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T12:25:45.565Z",
    "course_id": 233,
    "author_id": 654,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-18T12:25:44.988Z",
    "questions_updated_at": "2016-10-18T12:25:44.988Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 658,
        "chapter_id": 133,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:45.545Z",
        "created_at": "2016-10-18T12:25:45.545Z",
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
        "id": 97,
        "obfuscated_id": "qdTHUgSdSV8",
        "author_id": 656,
        "chapter_id": 133,
        "position": 84,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:45.428Z",
        "created_at": "2016-10-18T12:25:45.298Z",
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
            "id": 197,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 198,
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
curl "api.goskive.com/v2/chapters/133" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85d4b7342e58c9dbb02ee27d8fddc048025de724d40acb5cf18a673b14106430"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/141
Content-Type: application/json
Authorization: Bearer cd2b6719a6207943f654aeb2e28c364fe387f928f5e43a56eff2080403225985
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
    "id": 141,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T12:25:47.835Z",
    "course_id": 241,
    "author_id": 686,
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
curl "api.goskive.com/v2/chapters/141" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd2b6719a6207943f654aeb2e28c364fe387f928f5e43a56eff2080403225985"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 84d0533c7d89891e957a32e49d2fb676dddad71abb4e4eabf5e1a6ec9980ed5e
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
    "author_id": 123,
    "reply_to_id": 2,
    "created_at": "2016-10-18T12:24:55.457Z",
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
	-H "Authorization: Bearer 84d0533c7d89891e957a32e49d2fb676dddad71abb4e4eabf5e1a6ec9980ed5e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 69713d87458484119d408426faa07352a3cbb261b6d5346bcd06d73eb5180faa
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
	-H "Authorization: Bearer 69713d87458484119d408426faa07352a3cbb261b6d5346bcd06d73eb5180faa"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/43
Content-Type: application/json
Authorization: Bearer d7d0e24e0acf5b672cb20406e477b18d8ee568569f9e6cad660c2c345b1c36da
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
curl "api.goskive.com/v2/comments/43" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7d0e24e0acf5b672cb20406e477b18d8ee568569f9e6cad660c2c345b1c36da"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer a902553f2378c32f38f4991a157cfecb8b840f2d91c9c3c864a0be4e169a83a5
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
curl "api.goskive.com/v2/comments/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a902553f2378c32f38f4991a157cfecb8b840f2d91c9c3c864a0be4e169a83a5"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/42
Content-Type: application/json
Authorization: Bearer dabc93a15bd19397ca57ed211dc604ed8e76dd6d4e5dda6edd1c243ca89f5fc6
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/42" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dabc93a15bd19397ca57ed211dc604ed8e76dd6d4e5dda6edd1c243ca89f5fc6"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/41/report
Content-Type: application/json
Authorization: Bearer 48ef5dad5ec98f4b12122d05c232fcde856fb7405bc513f2cfd87180a7a2cba3
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
	-H "Authorization: Bearer 48ef5dad5ec98f4b12122d05c232fcde856fb7405bc513f2cfd87180a7a2cba3"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/8
Content-Type: application/json
Authorization: Bearer 293333b9d47ca3771c8986cd7b10a568c51386e816d0cef4118b5b26ab9a89dc
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
    "id": 8,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-18T12:25:22.760Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 293333b9d47ca3771c8986cd7b10a568c51386e816d0cef4118b5b26ab9a89dc"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f5b01e1288019a438a222534d92662cc7cb0224133193a9ccfd81d3db428c149
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
      "id": 5,
      "name": "Fake Company Name 4",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:25:22.627Z"
    },
    {
      "id": 6,
      "name": "Fake Company Name 5",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:25:22.632Z"
    },
    {
      "id": 7,
      "name": "Fake Company Name 6",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:25:22.636Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5b01e1288019a438a222534d92662cc7cb0224133193a9ccfd81d3db428c149"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/10/company_profiles
Content-Type: application/json
Authorization: Bearer fa6247029a24f5c41651b3cf947b1c8083e67c8dec841e659f854e435baa1f51
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
curl "api.goskive.com/v2/companies/10/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa6247029a24f5c41651b3cf947b1c8083e67c8dec841e659f854e435baa1f51"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/9/company_profiles
Content-Type: application/json
Authorization: Bearer ac05f6ac41134d052f54946f810691292a300ff192436e389fa93e83239f3217
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
curl "api.goskive.com/v2/companies/9/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac05f6ac41134d052f54946f810691292a300ff192436e389fa93e83239f3217"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer c9ec0b1f75321f86510df0748ede981d16219b157444540790d6baccf3bed775
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
      "company_id": 34,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
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
      "company_id": 37,
      "precluded_campaign_ids": [

      ],
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
	-H "Authorization: Bearer c9ec0b1f75321f86510df0748ede981d16219b157444540790d6baccf3bed775"
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
Authorization: Bearer bdeaba6a68cc013213aca69a7684d8380372c2ae1689fe85b4c367cde64dab71
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
	-H "Authorization: Bearer bdeaba6a68cc013213aca69a7684d8380372c2ae1689fe85b4c367cde64dab71"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 31adde93bb6fe53e228dcfa7c0e33a907b5211fae406bff6e1e4426cde1edb50
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
    "id": 8,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:24:48.422Z",
    "course_id": 11,
    "author_id": 34,
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
	-H "Authorization: Bearer 31adde93bb6fe53e228dcfa7c0e33a907b5211fae406bff6e1e4426cde1edb50"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 253576889bc9ec59f3b13c6b2753081b07dd670ba6c7287e0b7a0a02741e1036
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
      "id": 20,
      "title": "Clever Chapter Title 17",
      "position": 1,
      "updated_at": "2016-10-18T12:24:49.930Z",
      "course_id": 19,
      "author_id": 61,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 21,
      "title": "Clever Chapter Title 18",
      "position": 2,
      "updated_at": "2016-10-18T12:24:49.956Z",
      "course_id": 19,
      "author_id": 62,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 22,
      "title": "Clever Chapter Title 19",
      "position": 3,
      "updated_at": "2016-10-18T12:24:50.219Z",
      "course_id": 19,
      "author_id": 63,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T12:24:49.848Z",
      "questions_updated_at": "2016-10-18T12:24:49.848Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 253576889bc9ec59f3b13c6b2753081b07dd670ba6c7287e0b7a0a02741e1036"
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
      "id": 26,
      "title": "Clever Chapter Title 23",
      "position": 1,
      "updated_at": "2016-10-18T12:24:50.708Z",
      "course_id": 22,
      "author_id": 75,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 27,
      "title": "Clever Chapter Title 24",
      "position": 2,
      "updated_at": "2016-10-18T12:24:50.735Z",
      "course_id": 22,
      "author_id": 76,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 28,
      "title": "Clever Chapter Title 25",
      "position": 3,
      "updated_at": "2016-10-18T12:24:51.005Z",
      "course_id": 22,
      "author_id": 77,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T12:24:50.627Z",
      "questions_updated_at": "2016-10-18T12:24:50.627Z",
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
Authorization: Bearer 339a87022ddcce0880eee5ec1bdcb4410c3b06a733473881c62bc358456f05b9
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
      "id": 23,
      "title": "Clever Chapter Title 20",
      "position": 1,
      "updated_at": "2016-10-18T12:24:50.490Z",
      "course_id": 21,
      "author_id": 70,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 24,
      "title": "Clever Chapter Title 21",
      "position": 2,
      "updated_at": "2016-10-18T12:24:50.516Z",
      "course_id": 21,
      "author_id": 71,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 25,
      "title": "Clever Chapter Title 22",
      "position": 3,
      "updated_at": "2016-10-18T12:24:50.542Z",
      "course_id": 21,
      "author_id": 72,
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
	-H "Authorization: Bearer 339a87022ddcce0880eee5ec1bdcb4410c3b06a733473881c62bc358456f05b9"
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
      "id": 29,
      "title": "Clever Chapter Title 26",
      "position": 1,
      "updated_at": "2016-10-18T12:24:51.213Z",
      "course_id": 24,
      "author_id": 82,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 30,
      "title": "Clever Chapter Title 27",
      "position": 2,
      "updated_at": "2016-10-18T12:24:51.239Z",
      "course_id": 24,
      "author_id": 83,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 31,
      "title": "Clever Chapter Title 28",
      "position": 3,
      "updated_at": "2016-10-18T12:24:51.265Z",
      "course_id": 24,
      "author_id": 84,
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
Authorization: Bearer e95846bff5b5adf42a9c30b59a02006942d2a81b8609d43fee0774eaa16ec52f
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
    "course_id": 139,
    "user_id": 348,
    "updated_at": "2016-10-18T12:25:11.951Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e95846bff5b5adf42a9c30b59a02006942d2a81b8609d43fee0774eaa16ec52f"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 3d8deca1e665dae4835ee56f92d1bdc7a89e6c34d1376e620146dc91e69a2aca
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
      "user_id": 360,
      "updated_at": "2016-10-18T12:25:12.596Z"
    },
    {
      "id": 7,
      "course_id": 144,
      "user_id": 361,
      "updated_at": "2016-10-18T12:25:12.612Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d8deca1e665dae4835ee56f92d1bdc7a89e6c34d1376e620146dc91e69a2aca"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/217/files
Content-Type: application/json
Authorization: Bearer 671c182d07af718aa0e7b7275dcd34106102930dcbe9fa4af2b4d535053ca98f
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
      "id": 10,
      "uploader": {
        "id": 602,
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
        "created_at": "2016-10-18T12:25:40.085Z",
        "updated_at": "2016-10-18T12:25:40.085Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:25:40.092Z",
      "updated_at": "2016-10-18T12:25:40.092Z",
      "course_id": 217,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 11,
      "uploader": {
        "id": 603,
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
        "created_at": "2016-10-18T12:25:40.103Z",
        "updated_at": "2016-10-18T12:25:40.103Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:25:40.110Z",
      "updated_at": "2016-10-18T12:25:40.110Z",
      "course_id": 217,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 12,
      "uploader": {
        "id": 604,
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
        "created_at": "2016-10-18T12:25:40.118Z",
        "updated_at": "2016-10-18T12:25:40.118Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:25:40.125Z",
      "updated_at": "2016-10-18T12:25:40.125Z",
      "course_id": 217,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/217/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 671c182d07af718aa0e7b7275dcd34106102930dcbe9fa4af2b4d535053ca98f"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/219/files
Content-Type: application/json
Authorization: Bearer d45e8ffe0dc34f4d4f0c25fce31c0908df7c7b6a7db6ca2816df23da6d10a2f2
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
    "id": 13,
    "uploader": {
      "id": 609,
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
      "created_at": "2016-10-18T12:25:40.371Z",
      "updated_at": "2016-10-18T12:25:40.371Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-18T12:25:40.402Z",
    "updated_at": "2016-10-18T12:25:40.402Z",
    "course_id": 219,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/219/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d45e8ffe0dc34f4d4f0c25fce31c0908df7c7b6a7db6ca2816df23da6d10a2f2"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/216/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 953d99cd40fb0c2ce96296b9ed0e0fe1749eace8bf3c6c5518ebad0dc31d48d1
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
    "key": "cache/a10126ada9d8b95a80a11a31513642dd.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMzoyNTo0MFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9hMTAxMjZhZGE5ZDhiOTVhODBhMTFhMzE1MTM2NDJkZC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMThUMTIyNTQwWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T122540Z",
    "x-amz-signature": "5a6c854b7fb1843d302915849c528d896ca2b42423df087edfed4d7d0e14737b"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/216/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 953d99cd40fb0c2ce96296b9ed0e0fe1749eace8bf3c6c5518ebad0dc31d48d1"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer d965413aacdea7311d80ba7ed58c71d538f663485f9864f77f1bb46bae79ed08
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
	-H "Authorization: Bearer d965413aacdea7311d80ba7ed58c71d538f663485f9864f77f1bb46bae79ed08"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 02263a15e4f8250477386d4d01b63dd3fd96ea2999b1b0ba6ec136e01f20677d
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
	-H "Authorization: Bearer 02263a15e4f8250477386d4d01b63dd3fd96ea2999b1b0ba6ec136e01f20677d"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 70440186b35e63ed46e2e6f7448ba7a702246edd2f6581f2e1f80fb892f9a0b6
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
	-H "Authorization: Bearer 70440186b35e63ed46e2e6f7448ba7a702246edd2f6581f2e1f80fb892f9a0b6"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f98e00c35fd178d4e0344ea6cf34efe6c278b14ad2f275f02716462e8a3fbe79
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
	-H "Authorization: Bearer f98e00c35fd178d4e0344ea6cf34efe6c278b14ad2f275f02716462e8a3fbe79"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ebfc30c602dc982c7a6fe16ccd272e39676df0e37b43936c80a8944e322a4362
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
	-H "Authorization: Bearer ebfc30c602dc982c7a6fe16ccd272e39676df0e37b43936c80a8944e322a4362"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer c8f0de48183052032e313c36ed82f3680334a9eaaa46f6379da3c6d521a50be6
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
    "creator_id": 558,
    "id": 205,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 189,
    "additional_university_ids": [

    ],
    "topic_id": 212,
    "discipline_id": 213,
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
    "chapters_updated_at": "2016-10-18T12:25:31.631Z",
    "updated_at": "2016-10-18T12:25:33.503Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 117,
        "title": "Clever Chapter Title 108",
        "position": 1,
        "updated_at": "2016-10-18T12:25:33.445Z",
        "course_id": 205,
        "author_id": 558,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:25:31.631Z",
        "questions_updated_at": "2016-10-18T12:25:31.631Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 118,
        "title": "Clever Chapter Title 109",
        "position": 2,
        "updated_at": "2016-10-18T12:25:33.493Z",
        "course_id": 205,
        "author_id": 558,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:25:31.631Z",
        "questions_updated_at": "2016-10-18T12:25:31.631Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 559,
        "chapter_id": 117,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:33.250Z",
        "created_at": "2016-10-18T12:25:33.250Z",
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
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 559,
        "chapter_id": 118,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:33.337Z",
        "created_at": "2016-10-18T12:25:33.337Z",
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
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 559,
        "chapter_id": 117,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:33.299Z",
        "created_at": "2016-10-18T12:25:33.299Z",
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
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 559,
        "chapter_id": 118,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:33.387Z",
        "created_at": "2016-10-18T12:25:33.387Z",
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
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 559,
        "chapter_id": 117,
        "position": 58,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:31.896Z",
        "created_at": "2016-10-18T12:25:31.745Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 559,
        "chapter_id": 117,
        "position": 59,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:32.121Z",
        "created_at": "2016-10-18T12:25:31.975Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 559,
        "chapter_id": 118,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:32.382Z",
        "created_at": "2016-10-18T12:25:32.226Z",
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
      },
      {
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 559,
        "chapter_id": 118,
        "position": 61,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:32.616Z",
        "created_at": "2016-10-18T12:25:32.467Z",
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
            "id": 140,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 141,
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
	-H "Authorization: Bearer c8f0de48183052032e313c36ed82f3680334a9eaaa46f6379da3c6d521a50be6"
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
    "creator_id": 570,
    "id": 207,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 191,
    "additional_university_ids": [

    ],
    "topic_id": 214,
    "discipline_id": 215,
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
    "chapters_updated_at": "2016-10-18T12:25:35.527Z",
    "updated_at": "2016-10-18T12:25:37.265Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 121,
        "title": "Clever Chapter Title 112",
        "position": 1,
        "updated_at": "2016-10-18T12:25:37.214Z",
        "course_id": 207,
        "author_id": 570,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:25:35.527Z",
        "questions_updated_at": "2016-10-18T12:25:35.527Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 122,
        "title": "Clever Chapter Title 113",
        "position": 2,
        "updated_at": "2016-10-18T12:25:37.256Z",
        "course_id": 207,
        "author_id": 570,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:25:35.527Z",
        "questions_updated_at": "2016-10-18T12:25:35.527Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 570,
        "chapter_id": 121,
        "position": 70,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:35.780Z",
        "created_at": "2016-10-18T12:25:35.628Z",
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
            "id": 158,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 159,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 570,
        "chapter_id": 122,
        "position": 72,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:25:36.282Z",
        "created_at": "2016-10-18T12:25:36.124Z",
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
            "id": 162,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 163,
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
PUT /v2/courses/203/pin
Content-Type: application/json
Authorization: Bearer dcf086df9a888541416e7d1e45e30cf3377dd737720353fabe7f64f90c7be301
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/203/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcf086df9a888541416e7d1e45e30cf3377dd737720353fabe7f64f90c7be301"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/208/pin
Content-Type: application/json
Authorization: Bearer 4c32de2cba3fe5c149dc4f5da23f4c28a3f5b2d73ad96dbd438ffde1d9263e84
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/208/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c32de2cba3fe5c149dc4f5da23f4c28a3f5b2d73ad96dbd438ffde1d9263e84"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 63151b8b5e630072beedabd1f9f67817776061a0e5e189994a63269120858001
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
    "creator_id": 579,
    "id": 210,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 194,
    "additional_university_ids": [

    ],
    "topic_id": 217,
    "discipline_id": 218,
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
    "updated_at": "2016-10-18T12:25:37.697Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63151b8b5e630072beedabd1f9f67817776061a0e5e189994a63269120858001"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 652b9ed3849901a6110d97581cbca0b9bea4eb9c6e4c115b3a797e023d748cae
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
    "id": 640,
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
    "created_at": "2016-10-18T12:25:44.162Z",
    "updated_at": "2016-10-18T12:25:44.162Z",
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
	-H "Authorization: Bearer 652b9ed3849901a6110d97581cbca0b9bea4eb9c6e4c115b3a797e023d748cae"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8d3d70fcebd06162d41a6b410b2e08d1295e5d414a9f564afa003e493f27df44
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[234]}
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
    "id": 635,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      234
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:25:43.500Z",
    "updated_at": "2016-10-18T12:25:43.553Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[234]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d3d70fcebd06162d41a6b410b2e08d1295e5d414a9f564afa003e493f27df44"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 76380163dc4221db08eb0f2880d6c771a06e2d6c5f5ef6ed5adf97b2caac8dc3
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
    "id": 637,
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
    "created_at": "2016-10-18T12:25:43.663Z",
    "updated_at": "2016-10-18T12:25:43.663Z",
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
	-H "Authorization: Bearer 76380163dc4221db08eb0f2880d6c771a06e2d6c5f5ef6ed5adf97b2caac8dc3"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 33715aeb4c4fbe845a76f0a920aca6122e8daaaad4c22dd6130c3df9ceeaf373
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[235]}
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
    "id": 636,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      235
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:25:43.607Z",
    "updated_at": "2016-10-18T12:25:43.607Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[235]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33715aeb4c4fbe845a76f0a920aca6122e8daaaad4c22dd6130c3df9ceeaf373"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 76d44a08443723d7aedd9acbdcbac204231bec17eb6873a7ee6d13f64efbe760
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

238
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
    "id": 639,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/4fc8b4506de7deff9ce2cc7a8a5e222795ce0381.jpg",
    "university_id": null,
    "fields_of_study": [
      238
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:25:43.848Z",
    "updated_at": "2016-10-18T12:25:44.130Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/066f8d737dfd9a4e5c58c3a2433ba9aed3988212.jpg",
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

238
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 76d44a08443723d7aedd9acbdcbac204231bec17eb6873a7ee6d13f64efbe760"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2f61740238632fde19b6ad680b41241049ed1ce601b93e8c8ec46088b9f53257
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
      "bookmarkable_id": 22,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 23,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 24,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f61740238632fde19b6ad680b41241049ed1ce601b93e8c8ec46088b9f53257"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer cd8cfbe722d3331d56bfeb07775db06c846b041f607a8d3447d845f37c384955
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
      "id": 3,
      "title": "Campaign 2",
      "company_id": 16,
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 17,
      "score": 0.0,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "id": 8,
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "display_priority": 1,
          "published": true,
          "revision_updated_at": "2013-01-01T00:00:00.000Z",
          "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/4e8ccb4fdbb03332710724b7199bfb925ebb8588.png",
          "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/1751c1fcb04de04c20e97d74547e239755abd978.png",
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
	-H "Authorization: Bearer cd8cfbe722d3331d56bfeb07775db06c846b041f607a8d3447d845f37c384955"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a397ce4a3fc45d02a241dda38ceee32809d080ecb4070b8e1b2772f9e7d5b990
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
      "title": "Campaign 1",
      "company_id": 12,
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
	-H "Authorization: Bearer a397ce4a3fc45d02a241dda38ceee32809d080ecb4070b8e1b2772f9e7d5b990"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer ea12e1f9b3d6f46ec7cd05b81b18f0a347bef6b43dc78797e3a98695b3c1084a
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
      "creator_id": 14,
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-4",
      "html_url": "https://goskive.com/course/mit-course-4",
      "slug": "mit-course-4",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "topic_id": 4,
      "discipline_id": 4,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 4",
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
      "updated_at": "2016-10-18T12:24:31.618Z",
      "shortname": "mit-course-4"
    },
    {
      "creator_id": 15,
      "id": 5,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-5",
      "html_url": "https://goskive.com/course/mit-course-5",
      "slug": "mit-course-5",
      "university_id": 5,
      "additional_university_ids": [

      ],
      "topic_id": 5,
      "discipline_id": 5,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
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
      "updated_at": "2016-10-18T12:24:31.704Z",
      "shortname": "mit-course-5"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea12e1f9b3d6f46ec7cd05b81b18f0a347bef6b43dc78797e3a98695b3c1084a"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 354ddf13fc002609ab4d2ca056942110f710961bcdc295a8c0c9d756ac0fefc4
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
      "company_id": 25,
      "company": {
        "id": 25,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:25:48.117Z"
      },
      "created_at": "2016-10-18T12:25:48.120Z",
      "updated_at": "2016-10-18T12:25:48.120Z",
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
      "company_id": 26,
      "company": {
        "id": 26,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:25:48.129Z"
      },
      "created_at": "2016-10-18T12:25:48.132Z",
      "updated_at": "2016-10-18T12:25:48.132Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 354ddf13fc002609ab4d2ca056942110f710961bcdc295a8c0c9d756ac0fefc4"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 04042ab9ca4c27c12cc5ca4bd584b5bd2d79af3b1aab700afccdac41656213c9
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
        "name": "Fake Company Name 16",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:25:47.893Z"
      },
      "created_at": "2016-10-18T12:25:47.896Z",
      "updated_at": "2016-10-18T12:25:47.896Z",
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
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:25:47.912Z"
      },
      "created_at": "2016-10-18T12:25:47.915Z",
      "updated_at": "2016-10-18T12:25:47.915Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04042ab9ca4c27c12cc5ca4bd584b5bd2d79af3b1aab700afccdac41656213c9"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 3837e40cb1e3dbe9a556e272135e2a34242dbf6bb9707a640c118469a6a7692e
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
      "created_at": "2016-10-18T12:26:01.120Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-10-18T12:26:01.236Z",
      "author_id": "861",
      "thread_subject_id": "280",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-10-18T12:26:01.223Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-10-18T12:26:01.239Z",
      "author_id": "864",
      "thread_subject_id": "281",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-18T12:26:01.660Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-18T12:26:01.660Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-10-18T12:26:02.085Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-18T12:26:02.085Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-10-18T12:26:02.506Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-18T12:26:02.506Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-10-18T12:26:02.835Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 132,
      "updated_at": "2016-10-18T12:26:02.835Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-18T12:26:03.172Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 133,
      "updated_at": "2016-10-18T12:26:03.172Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-10-18T12:26:03.503Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 134,
      "updated_at": "2016-10-18T12:26:03.503Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3837e40cb1e3dbe9a556e272135e2a34242dbf6bb9707a640c118469a6a7692e"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/15
Content-Type: application/json
Authorization: Bearer f2518ce08a1b54ffe06b006d51469ad68ecabf720b63e87b605490b1c62b502e
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-18T12:16:00.000Z"}}
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
    "id": 15,
    "created_at": "2016-10-18T12:26:00.902Z",
    "read_at": "2016-10-18T12:16:00.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 56,
    "updated_at": "2016-10-18T12:26:00.964Z",
    "author_id": "856",
    "thread_subject_id": "279",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/15" -d '{"notification":{"read_at":"2016-10-18T12:16:00.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2518ce08a1b54ffe06b006d51469ad68ecabf720b63e87b605490b1c62b502e"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 31fd772c8cba5942be5beba387682f1c60b434734f4044cf9b30647ae9d85ce0
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
      "course_id": 231,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T12:25:44.860Z",
      "course_published": true,
      "updated_at": "2016-10-18T12:25:44.852Z"
    },
    {
      "id": 8,
      "course_id": 232,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T12:25:44.948Z",
      "course_published": true,
      "updated_at": "2016-10-18T12:25:44.939Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31fd772c8cba5942be5beba387682f1c60b434734f4044cf9b30647ae9d85ce0"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 3c7cfb2a3ab160539fbdc4edde2bcde259014a1c9e0904787da2f92a61ea8e91
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
    "course_id": 230,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T12:25:44.690Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:25:44.682Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c7cfb2a3ab160539fbdc4edde2bcde259014a1c9e0904787da2f92a61ea8e91"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 8512c34a3b2917998e8bdfa7af815bc10d8f93f0101dfc0740c5424d390aad49
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
    "course_id": 229,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-18T12:25:44.589Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:25:44.578Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8512c34a3b2917998e8bdfa7af815bc10d8f93f0101dfc0740c5424d390aad49"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 93327f6e91b0bd328cd0be70e438586715d1183c15b70948bb3fe32dc4e9f8f9
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
      "votable_id": 4,
      "user_id": 18
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 5,
      "user_id": 18
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 6,
      "user_id": 18
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 7,
      "user_id": 18
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93327f6e91b0bd328cd0be70e438586715d1183c15b70948bb3fe32dc4e9f8f9"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/174
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
    "id": 174,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 172,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 174
      },
      {
        "id": 173,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 174
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/174" -X GET \
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
      "id": 172,
      "name": "Ergonomic bifurcated definition",
      "name_translations": {
        "en": "Ergonomic bifurcated definition"
      }
    },
    {
      "id": 173,
      "name": "Multi-tiered local model",
      "name_translations": {
        "en": "Multi-tiered local model"
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
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer 07686eabedcfbd08882855968617548e67bb9290bc7420a7f4816dc4f051891e
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
    "id": 3,
    "user_id": 693,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-18T12:25:48.396Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07686eabedcfbd08882855968617548e67bb9290bc7420a7f4816dc4f051891e"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/29/fix
Content-Type: application/json
Authorization: Bearer 162abe054f465bebd1f1939bd00231fb540ccc3717fad0f16abfdeeb188af7d6
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
    "id": 29,
    "user_id": 811,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-18T12:25:56.890Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/29/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 162abe054f465bebd1f1939bd00231fb540ccc3717fad0f16abfdeeb188af7d6"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/25
Content-Type: application/json
Authorization: Bearer cefb3108155e1295829ce4d3b61be6385f53925699c8bee9eac0409225d51761
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
    "user_id": 789,
    "feedbackable_id": 78,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:25:55.935Z",
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
	-H "Authorization: Bearer cefb3108155e1295829ce4d3b61be6385f53925699c8bee9eac0409225d51761"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/close
Content-Type: application/json
Authorization: Bearer f202e6dec0e212474bf589f41c78c9b9ac51f634a38ce3f7190c1b0772e507b6
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
curl "api.goskive.com/v2/feedbacks/5/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f202e6dec0e212474bf589f41c78c9b9ac51f634a38ce3f7190c1b0772e507b6"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 9190aaa8ec4f6dfc93131fd038361a65eea474c3605306d31d7d513cb51bec9d
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
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9190aaa8ec4f6dfc93131fd038361a65eea474c3605306d31d7d513cb51bec9d"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 5e00ce8b6dd964252be6bad0e03a214976c39b467e59f93db8a5665a49e292a7
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
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e00ce8b6dd964252be6bad0e03a214976c39b467e59f93db8a5665a49e292a7"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/26
Content-Type: application/json
Authorization: Bearer 3ef0dab547b842d214224831e6aa4dcf24bae4826bcfa666690857fb1af5d732
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
    "user_id": 794,
    "feedbackable_id": 79,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:25:56.242Z",
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
	-H "Authorization: Bearer 3ef0dab547b842d214224831e6aa4dcf24bae4826bcfa666690857fb1af5d732"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Authorization: Bearer 1f8e35d6c4000fe549e133e2e5cb6cf6d714d0ec5db46101d9e0b86debc4e77e
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
	-H "Authorization: Bearer 1f8e35d6c4000fe549e133e2e5cb6cf6d714d0ec5db46101d9e0b86debc4e77e" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/9
Authorization: Bearer 5542780562f831ec99f46ff4de97534e896b80ba11512d55acb661bf4568b63f
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
	-H "Authorization: Bearer 5542780562f831ec99f46ff4de97534e896b80ba11512d55acb661bf4568b63f" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/6
Authorization: Bearer ef616c5e48a7b13bff3d6a0915c8dac4a559c279d740d07950f7d72fa020704a
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/81fdb9867e5fbcba4067c9a1171b9b17.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T122501Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=e4f46e305e866d4b346a7590f24015ff09a83fb7f5c8a6b385071a415e207e74"
  }
}
```



```shell
curl "api.goskive.com/v2/files/6" -X GET \
	-H "Authorization: Bearer ef616c5e48a7b13bff3d6a0915c8dac4a559c279d740d07950f7d72fa020704a"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Authorization: Bearer 327c7daa6d2de24bf9992f7e3b2f3da2375b4704d8eb9673c1d8585dd2817fd2
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
    "id": 5,
    "uploader": {
      "id": 236,
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
      "created_at": "2016-10-18T12:25:01.481Z",
      "updated_at": "2016-10-18T12:25:01.481Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-18T12:25:01.554Z",
    "updated_at": "2016-10-18T12:25:01.554Z",
    "course_id": 80,
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
curl "api.goskive.com/v2/files/5/metadata" -X GET \
	-H "Authorization: Bearer 327c7daa6d2de24bf9992f7e3b2f3da2375b4704d8eb9673c1d8585dd2817fd2" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer 9e4111a4c562acd52b5d38869a735a514e37835aa29075c244287fbab1bdb44d
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
      "creator_id": 95,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 27,
      "additional_university_ids": [

      ],
      "topic_id": 27,
      "discipline_id": 27,
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
      "chapters_updated_at": "2016-10-18T12:24:51.308Z",
      "updated_at": "2016-10-18T12:24:52.992Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 100,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-f37c1286-0473-41fb-8a57-5619033487e9",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-f37c1286-0473-41fb-8a57-5619033487e9",
      "slug": "mit-the-great-british-bake-off-f37c1286-0473-41fb-8a57-5619033487e9",
      "university_id": 28,
      "additional_university_ids": [

      ],
      "topic_id": 28,
      "discipline_id": 28,
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
      "chapters_updated_at": "2016-10-18T12:24:51.308Z",
      "updated_at": "2016-10-18T12:24:53.559Z",
      "shortname": "mit-the-great-british-bake-off-f37c1286-0473-41fb-8a57-5619033487e9"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 9e4111a4c562acd52b5d38869a735a514e37835aa29075c244287fbab1bdb44d"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/4/preview
Authorization: Bearer ba02b0129ed7a0b3a43acce20601b64806ece9f73ae425b4f37360e327403407
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/85434214c7aaefe1511e7a5d24d9644d.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T122501Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=b06b2ef8afd3c9f467bfbb791a20218d660cd6ae620add4a5710495de7f33301"
  }
}
```



```shell
curl "api.goskive.com/v2/files/4/preview" -X GET \
	-H "Authorization: Bearer ba02b0129ed7a0b3a43acce20601b64806ece9f73ae425b4f37360e327403407"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/3/report
Authorization: Bearer a507a303e400a5f913cd67548902742d9dc0e54d53f4ed9dda1094f56847e250
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
curl "api.goskive.com/v2/files/3/report" -d '' -X PUT \
	-H "Authorization: Bearer a507a303e400a5f913cd67548902742d9dc0e54d53f4ed9dda1094f56847e250" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/18/comments
Content-Type: application/json
Authorization: Bearer 97940dc1119742e749a76920e7b258a6d367d9499601b5070b6b2980be2aa0d8
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
    "id": 50,
    "author_id": 336,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:25:11.231Z",
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
curl "api.goskive.com/v2/flashcards/18/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97940dc1119742e749a76920e7b258a6d367d9499601b5070b6b2980be2aa0d8"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/16/comments
Content-Type: application/json
Authorization: Bearer aba270de976781a212bc11492296ffbedfddd2137c6546f6a4e893c9be39fe97
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
    "id": 49,
    "author_id": 330,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:25:10.700Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 2,
      "user_id": 330,
      "feedbackable_id": 16,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:10.697Z",
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
curl "api.goskive.com/v2/flashcards/16/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aba270de976781a212bc11492296ffbedfddd2137c6546f6a4e893c9be39fe97"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/20/comments
Content-Type: application/json
Authorization: Bearer 98fba0b7e7773130f1039c667b0e36aa07341ed940523529b813a9f807546d31
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
      "id": 51,
      "author_id": 345,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:25:11.763Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 346,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:25:11.781Z",
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
curl "api.goskive.com/v2/flashcards/20/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98fba0b7e7773130f1039c667b0e36aa07341ed940523529b813a9f807546d31"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/17/comments
Content-Type: application/json
Authorization: Bearer 51a5b6d46407083971d06de499ed89d917e992a3b6264a7dfc447165d39c5a47
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
curl "api.goskive.com/v2/flashcards/17/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51a5b6d46407083971d06de499ed89d917e992a3b6264a7dfc447165d39c5a47"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/88/feedbacks
Content-Type: application/json
Authorization: Bearer 1e26f39457f11946f4e868e1e45042f31b8be89bbeb4805d8974ba7a3c3b2c84
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
    "id": 40,
    "user_id": 924,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:26:07.472Z",
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
curl "api.goskive.com/v2/flashcards/88/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e26f39457f11946f4e868e1e45042f31b8be89bbeb4805d8974ba7a3c3b2c84"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/89/feedbacks
Content-Type: application/json
Authorization: Bearer 834f429f848a8ed98d81b4674d781eb161b9c0139426d53628aef6a7e72a1cee
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
      "user_id": 931,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:26:07.797Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 930,
      "feedbackable_id": 89,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:26:07.785Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/89/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 834f429f848a8ed98d81b4674d781eb161b9c0139426d53628aef6a7e72a1cee"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/85/votes
Content-Type: application/json
Authorization: Bearer 2c664efa8f4c17772198deff27e2d400f738b22cc03b8d19e56ec39ebc55f7f2
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 903
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 902
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 85,
      "user_id": 901
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/85/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c664efa8f4c17772198deff27e2d400f738b22cc03b8d19e56ec39ebc55f7f2"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/44/republish
Content-Type: application/json
Authorization: Bearer f1539fe851ba7748e2f9fa40eed3bee51d5915242c4571c3b09e0587840a85c7
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
curl "api.goskive.com/v2/flashcards/44/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1539fe851ba7748e2f9fa40eed3bee51d5915242c4571c3b09e0587840a85c7"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/bookmark
Content-Type: application/json
Authorization: Bearer dc9003757d11ed10cbd0bb18fa43ca52851c5f7071145330bf6c9697bc2634e3
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc9003757d11ed10cbd0bb18fa43ca52851c5f7071145330bf6c9697bc2634e3"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/23
Content-Type: application/json
Authorization: Bearer fe7832ee1a486649e1bccb1f7b7129248b8d0744798aa65c05cfe2d2acb5b0ac
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe7832ee1a486649e1bccb1f7b7129248b8d0744798aa65c05cfe2d2acb5b0ac"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/downvote
Content-Type: application/json
Authorization: Bearer a8d8a126718aea08479eb7b588b305cd4afb3edaa59c03e15d9cfde7e665a9e1
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
	-H "Authorization: Bearer a8d8a126718aea08479eb7b588b305cd4afb3edaa59c03e15d9cfde7e665a9e1"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/42
Content-Type: application/json
Authorization: Bearer 815c20552f993cb594c15272d83c727cd301b8afe48b9711de598ebf8a5977a4
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
    "id": 42,
    "obfuscated_id": "6gppIIjkzlA",
    "author_id": 518,
    "chapter_id": 108,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:26.814Z",
    "created_at": "2016-10-18T12:25:26.814Z",
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
curl "api.goskive.com/v2/flashcards/42" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 815c20552f993cb594c15272d83c727cd301b8afe48b9711de598ebf8a5977a4"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/report
Content-Type: application/json
Authorization: Bearer 3a2336f9a63a98ee57f45920444396f39e561331035c7342d6320d7057903d70
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a2336f9a63a98ee57f45920444396f39e561331035c7342d6320d7057903d70"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/22/bookmark
Content-Type: application/json
Authorization: Bearer 45367d576597b310d5b4e2c4845d03d91101b34a45e8fdc1e003a449440da2be
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/22/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45367d576597b310d5b4e2c4845d03d91101b34a45e8fdc1e003a449440da2be"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/24/upvote
Content-Type: application/json
Authorization: Bearer 0b7c5274e638fdb328939ce5dd50edec02be6989b6aad9b9cf2e6cb862eafedf
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b7c5274e638fdb328939ce5dd50edec02be6989b6aad9b9cf2e6cb862eafedf"
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
    "key": "cache/b7b86ee9fa5104fdf216c418ee8438a0.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMzoyNToyN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9iN2I4NmVlOWZhNTEwNGZkZjIxNmM0MThlZTg0MzhhMC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOFQxMjI1MjdaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T122527Z",
    "x-amz-signature": "dc500afb2805a9314b633d778710eeacc869aa2e61a555aa9a08d99f70c26c6a"
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
Authorization: Bearer 8e8421d61356f164e09443adcfc222375dd165cb04ca05b54a342db96c531789
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
	-H "Authorization: Bearer 8e8421d61356f164e09443adcfc222375dd165cb04ca05b54a342db96c531789"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 07f73311f8e85c9734f74a88d07c9d193fc68e09850c1a8ddc59c13db1230ee6
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
	-H "Authorization: Bearer 07f73311f8e85c9734f74a88d07c9d193fc68e09850c1a8ddc59c13db1230ee6"
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
{"password":{"reset_password_token":"cRxACSmXQg2tiB7RcLDv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 889,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-18T12:26:04.032Z",
  "updated_at": "2016-10-18T12:26:04.245Z",
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
  "audit_id": 4780
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"cRxACSmXQg2tiB7RcLDv","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer 71fc181b0b3bec4691386efaf887bc2c85d7a0b575054cec3179fd36a65e038a
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
    "id": 46,
    "author_id": 267,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:25:04.396Z",
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
curl "api.goskive.com/v2/questions/27/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71fc181b0b3bec4691386efaf887bc2c85d7a0b575054cec3179fd36a65e038a"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/26/comments
Content-Type: application/json
Authorization: Bearer 619dd979acd544f6cb7eced6e9bd80cab3c349bc142d6bedeca84fa32b951a3b
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
    "author_id": 264,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:25:03.860Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 264,
      "feedbackable_id": 26,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:03.856Z",
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
curl "api.goskive.com/v2/questions/26/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 619dd979acd544f6cb7eced6e9bd80cab3c349bc142d6bedeca84fa32b951a3b"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/28/comments
Content-Type: application/json
Authorization: Bearer bb3904cb877b79769e8c53496f80fb6bfc230b45a74c7aa4e79ad60647fcdfa7
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
      "author_id": 273,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:25:04.872Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 274,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:25:04.889Z",
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
curl "api.goskive.com/v2/questions/28/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb3904cb877b79769e8c53496f80fb6bfc230b45a74c7aa4e79ad60647fcdfa7"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/25/comments
Content-Type: application/json
Authorization: Bearer 4f221f9b40328b32f256d292510b811525b33d3acc14db02490c06eabf0a3968
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
curl "api.goskive.com/v2/questions/25/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f221f9b40328b32f256d292510b811525b33d3acc14db02490c06eabf0a3968"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/127/feedbacks
Content-Type: application/json
Authorization: Bearer 07bb28b7c92d5c90359fa4836931855fea0c591ba0694423c3291515643b84fe
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
    "id": 37,
    "user_id": 848,
    "feedbackable_id": 127,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:26:00.111Z",
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
curl "api.goskive.com/v2/questions/127/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07bb28b7c92d5c90359fa4836931855fea0c591ba0694423c3291515643b84fe"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/124/feedbacks
Content-Type: application/json
Authorization: Bearer d43f43ec4670b06d4cee4ae81761e5664c846edce9a6eb789c20864f91b59281
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
      "user_id": 833,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:58.916Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 832,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:25:58.905Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/124/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d43f43ec4670b06d4cee4ae81761e5664c846edce9a6eb789c20864f91b59281"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/2/votes
Content-Type: application/json
Authorization: Bearer 3cdd16a2a95af7ad4178dabd716e1a42d2a6c06b6750463338fa6f591a1a8644
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 9
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 8
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 7
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3cdd16a2a95af7ad4178dabd716e1a42d2a6c06b6750463338fa6f591a1a8644"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/35/republish
Content-Type: application/json
Authorization: Bearer c480b31de3803cff54ad5a5672b4ecca53fd2f7180b3f3110c8e3edf9862212c
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
curl "api.goskive.com/v2/questions/35/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c480b31de3803cff54ad5a5672b4ecca53fd2f7180b3f3110c8e3edf9862212c"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/39/bookmark
Content-Type: application/json
Authorization: Bearer ae489e1914136efc075a6a2fb8f8f9fd0c10d1198d9143ea3cafba6ffa107923
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/39/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae489e1914136efc075a6a2fb8f8f9fd0c10d1198d9143ea3cafba6ffa107923"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/57
Content-Type: application/json
Authorization: Bearer 40dceb42bdf381e91e3e8260e014c3beae5a8523ab6b6699a88fdaa87de01d1c
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40dceb42bdf381e91e3e8260e014c3beae5a8523ab6b6699a88fdaa87de01d1c"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/58/downvote
Content-Type: application/json
Authorization: Bearer 31f54a660a0db06c32d239c8cab52cb90be55c975788f4701bd419f530a5c72b
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/58/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31f54a660a0db06c32d239c8cab52cb90be55c975788f4701bd419f530a5c72b"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/56
Content-Type: application/json
Authorization: Bearer 3d428361e8f2a8b701a64e4b0e11b425f4554eca7adb0c45c90227d572ee46da
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
    "id": 56,
    "obfuscated_id": "PgrpyPCfpqo",
    "author_id": 434,
    "chapter_id": 84,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:21.056Z",
    "created_at": "2016-10-18T12:25:20.914Z",
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
        "id": 112,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 113,
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
curl "api.goskive.com/v2/questions/56" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d428361e8f2a8b701a64e4b0e11b425f4554eca7adb0c45c90227d572ee46da"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/37/report
Content-Type: application/json
Authorization: Bearer 3e4a95fffe0c3088f05deeecc83064867e7b9091b0026deabf8c6b27145d76b7
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/37/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e4a95fffe0c3088f05deeecc83064867e7b9091b0026deabf8c6b27145d76b7"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/55/bookmark
Content-Type: application/json
Authorization: Bearer 67aef02b0ce4ec9c7bda8d0d834794ffc62927bd912f1728982689dbd41c2483
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/55/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67aef02b0ce4ec9c7bda8d0d834794ffc62927bd912f1728982689dbd41c2483"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/38
Content-Type: application/json
Authorization: Bearer 0d9570a7fdbf32d42c12e8e71ca8e5133a260e00231a86961ed0e72b73baad08
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":38,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T12:25:14.546Z","updated_at":"2016-10-18T12:25:14.682Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":66,"author_id":375,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 38,
    "obfuscated_id": "8_YCqPYFnsI",
    "author_id": 375,
    "chapter_id": 66,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:25:14.801Z",
    "created_at": "2016-10-18T12:25:14.546Z",
    "tags": [
      {
        "id": 8,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 7,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>38, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-18T12:25:14.546Z\", \"updated_at\"=>\"2016-10-18T12:25:14.682Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>66, \"author_id\"=>375, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 77,
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
curl "api.goskive.com/v2/questions/38" -d '{"question":{"question":{"id":38,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T12:25:14.546Z","updated_at":"2016-10-18T12:25:14.682Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":66,"author_id":375,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d9570a7fdbf32d42c12e8e71ca8e5133a260e00231a86961ed0e72b73baad08"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/34/upvote
Content-Type: application/json
Authorization: Bearer 136e70f6822f5de53dffefe99ac998d9dcf453a4e3622a087274f976da460ab0
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 136e70f6822f5de53dffefe99ac998d9dcf453a4e3622a087274f976da460ab0"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer e7651268e00aa78fa8eab2c597e3445e25a01089dc7756f24b71488357abb736
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
      "creator_id": 961,
      "id": 305,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 288,
      "additional_university_ids": [

      ],
      "topic_id": 317,
      "discipline_id": 318,
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
      "updated_at": "2016-10-18T12:26:09.243Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7651268e00aa78fa8eab2c597e3445e25a01089dc7756f24b71488357abb736"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer af34d3afe5d3007f9a6d8383db02a10589478c9e15a8f46517dc00244e4d376e
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
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-271",
      "html_url": "https://goskive.com/university/uni-271",
      "slug": "uni-271",
      "name": "National School of Pizza",
      "short_name": "Uni 271",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/bd27ba3e14a65dc475bce92147a15b35bb84678e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f94654da13a014f55605131ca96388e79c0b329b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:26:09.545Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 290,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-270",
      "html_url": "https://goskive.com/university/uni-270",
      "slug": "uni-270",
      "name": "National School of Pastry",
      "short_name": "Uni 270",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/1084079aa5c54cda74ccc2533b2a7fb5ed25f898.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4c5d00318fb7c537b4d2dbd3e16f01d72ba28007.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:26:09.527Z",
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
	-H "Authorization: Bearer af34d3afe5d3007f9a6d8383db02a10589478c9e15a8f46517dc00244e4d376e"
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
      "id": 198,
      "name": "Devolved grid-enabled matrix",
      "name_translations": {
        "en": "Devolved grid-enabled matrix"
      },
      "discipline_id": 199
    },
    {
      "id": 199,
      "name": "Face to face tertiary budgetary management",
      "name_translations": {
        "en": "Face to face tertiary budgetary management"
      },
      "discipline_id": 200
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
GET /v2/topics/200
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
    "id": 200,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 201
  }
}
```



```shell
curl "api.goskive.com/v2/topics/200" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 4476d1a72cf38e11535800e8170264ed2ee28c346c16ea910c83a897c961fc7e
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
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-131",
      "html_url": "https://goskive.com/university/uni-131",
      "slug": "uni-131",
      "name": "University 107",
      "short_name": "Uni 131",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/7de22abbebc2962313fa1214c80aa7729c6a8cb4.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/153185985e728aa71bbf1b51f6e203101673dc8a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:25:22.421Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-132",
      "html_url": "https://goskive.com/university/uni-132",
      "slug": "uni-132",
      "name": "University 108",
      "short_name": "Uni 132",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f2e8bacdb569f375861d9d4fefc0d5eda870570e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b8a29419bf38bc901035e7fe1ecdfef7b976ba1d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:25:22.438Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-133",
      "html_url": "https://goskive.com/university/uni-133",
      "slug": "uni-133",
      "name": "University 109",
      "short_name": "Uni 133",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/1d2975a44a232a79e59c9757d9d176fc1335184b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/16c52dae119d771068577df0b0c5c8397a9265fd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:25:22.455Z",
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
	-H "Authorization: Bearer 4476d1a72cf38e11535800e8170264ed2ee28c346c16ea910c83a897c961fc7e"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 36f1a9d53f029281e864d62422a6fb170b69b4a11a8c9a6f98849cc343966647
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
    "id": 153,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4520ea235c0ccd922b85aa0607bacc9431645c4d.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6af1e644eed83a184febdb26f08a491678a85037.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-18T12:25:22.579Z",
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
	-H "Authorization: Bearer 36f1a9d53f029281e864d62422a6fb170b69b4a11a8c9a6f98849cc343966647"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 009a698d864afe5fa5a7235f27f7a43a06ba790ee6b0f521b4152d6a51fbaea9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":132,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 324,
    "id": 130,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 109,
    "additional_university_ids": [

    ],
    "topic_id": 132,
    "discipline_id": 132,
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
    "chapters_updated_at": "2016-10-18T12:25:09.637Z",
    "updated_at": "2016-10-18T12:25:09.783Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 54,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-18T12:25:09.734Z",
        "course_id": 130,
        "author_id": 324,
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
        "id": 55,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-18T12:25:09.753Z",
        "course_id": 130,
        "author_id": 324,
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
        "id": 56,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-18T12:25:09.772Z",
        "course_id": 130,
        "author_id": 324,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":132,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 009a698d864afe5fa5a7235f27f7a43a06ba790ee6b0f521b4152d6a51fbaea9"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 35eda4575f7c1c3f5a31121e42008418179238cf21ad2a6709bdc5ef75331039
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":133,"published":false}}
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
    "creator_id": 325,
    "id": 131,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 110,
    "additional_university_ids": [

    ],
    "topic_id": 133,
    "discipline_id": 133,
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
    "updated_at": "2016-10-18T12:25:09.936Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":133,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35eda4575f7c1c3f5a31121e42008418179238cf21ad2a6709bdc5ef75331039"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2c2c5c3310bfa0db90ca1604b1e9020066354bbd971be9d710581be8e4ae6eb9
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
      "creator_id": 293,
      "id": 103,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-79",
      "html_url": "https://goskive.com/course/fu-course-79",
      "slug": "fu-course-79",
      "university_id": 97,
      "additional_university_ids": [

      ],
      "topic_id": 105,
      "discipline_id": 105,
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
      "updated_at": "2016-10-18T12:25:06.673Z",
      "shortname": "fu-course-79"
    },
    {
      "creator_id": 293,
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-80",
      "html_url": "https://goskive.com/course/fu-course-80",
      "slug": "fu-course-80",
      "university_id": 97,
      "additional_university_ids": [

      ],
      "topic_id": 106,
      "discipline_id": 106,
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
      "chapters_updated_at": "2016-10-18T12:25:06.980Z",
      "updated_at": "2016-10-18T12:25:06.987Z",
      "shortname": "fu-course-80"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c2c5c3310bfa0db90ca1604b1e9020066354bbd971be9d710581be8e4ae6eb9"
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
      "creator_id": 303,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-87",
      "html_url": "https://goskive.com/course/fu-course-87",
      "slug": "fu-course-87",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "topic_id": 113,
      "discipline_id": 113,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 87",
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
      "updated_at": "2016-10-18T12:25:07.553Z",
      "shortname": "fu-course-87"
    },
    {
      "creator_id": 303,
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-88",
      "html_url": "https://goskive.com/course/fu-course-88",
      "slug": "fu-course-88",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "topic_id": 114,
      "discipline_id": 114,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 88",
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
      "chapters_updated_at": "2016-10-18T12:25:07.882Z",
      "updated_at": "2016-10-18T12:25:07.889Z",
      "shortname": "fu-course-88"
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
Authorization: Bearer 686da8ac2ef4d58eb83c6152b48165375f8b3a1b4707307c379c6189cbb3bb99
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
      "creator_id": 300,
      "id": 107,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-83",
      "html_url": "https://goskive.com/course/fu-course-83",
      "slug": "fu-course-83",
      "university_id": 99,
      "additional_university_ids": [

      ],
      "topic_id": 109,
      "discipline_id": 109,
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
      "updated_at": "2016-10-18T12:25:07.271Z",
      "shortname": "fu-course-83"
    },
    {
      "creator_id": 300,
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-84",
      "html_url": "https://goskive.com/course/fu-course-84",
      "slug": "fu-course-84",
      "university_id": 99,
      "additional_university_ids": [

      ],
      "topic_id": 110,
      "discipline_id": 110,
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
      "updated_at": "2016-10-18T12:25:07.313Z",
      "shortname": "fu-course-84"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 686da8ac2ef4d58eb83c6152b48165375f8b3a1b4707307c379c6189cbb3bb99"
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
      "creator_id": 308,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-91",
      "html_url": "https://goskive.com/course/fu-course-91",
      "slug": "fu-course-91",
      "university_id": 102,
      "additional_university_ids": [

      ],
      "topic_id": 117,
      "discipline_id": 117,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 91",
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
      "updated_at": "2016-10-18T12:25:08.112Z",
      "shortname": "fu-course-91"
    },
    {
      "creator_id": 308,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-92",
      "html_url": "https://goskive.com/course/fu-course-92",
      "slug": "fu-course-92",
      "university_id": 102,
      "additional_university_ids": [

      ],
      "topic_id": 118,
      "discipline_id": 118,
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
      "updated_at": "2016-10-18T12:25:08.154Z",
      "shortname": "fu-course-92"
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
Authorization: Bearer c05f1c80e7568ac0af7d7133f84d38b1f790dfcfe8d4b248cabe7889ddcf0237
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
  "id": 329,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-18T12:25:10.320Z",
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
	-H "Authorization: Bearer c05f1c80e7568ac0af7d7133f84d38b1f790dfcfe8d4b248cabe7889ddcf0237"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/280
Content-Type: application/json
Authorization: Bearer 5147e045bcc35bbcf85c21f7e51c04719f69c833332e8e081a7dfdbca4a73f87
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
    "id": 280,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 93,
    "fields_of_study": [
      93,
      94
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-18T12:25:05.449Z",
    "updated_at": "2016-10-18T12:25:05.449Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/280" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5147e045bcc35bbcf85c21f7e51c04719f69c833332e8e081a7dfdbca4a73f87"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/278
Content-Type: application/json
Authorization: Bearer 4116addcf5858d9f4089116854e5f6be4c6666fdc059343dadd443d103ee45ab
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
    "id": 278,
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
    "created_at": "2016-10-18T12:25:05.279Z",
    "updated_at": "2016-10-18T12:25:05.279Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/278" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4116addcf5858d9f4089116854e5f6be4c6666fdc059343dadd443d103ee45ab"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/14
Content-Type: application/json
Authorization: Bearer 23f2a8c19d4c991c1e93fe1286d931447d802f7b5b7e0ec58a60b5384c5a8d6e
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23f2a8c19d4c991c1e93fe1286d931447d802f7b5b7e0ec58a60b5384c5a8d6e"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/15
Content-Type: application/json
Authorization: Bearer 24d9cee0f1c819bfa6d8e03a5d61633628318492c4c925f4dc7a5ccb8b71b663
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
    "id": 15,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 87,
    "user_id": 595
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24d9cee0f1c819bfa6d8e03a5d61633628318492c4c925f4dc7a5ccb8b71b663"
```
