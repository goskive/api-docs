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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"6b918557d75be1b2ce5a8193a3c3ce0d91ccb8b0ec5c5390ee8494e1ffca479e","client_secret":"8fc2e9edf91a9db6be0094038278ccf9c605262d4664d67200b06364ff00ae17"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"6b918557d75be1b2ce5a8193a3c3ce0d91ccb8b0ec5c5390ee8494e1ffca479e","client_secret":"8fc2e9edf91a9db6be0094038278ccf9c605262d4664d67200b06364ff00ae17"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NTAzYzgxMDNlZTg0ZGNiMzhiOTEwZmRhOTkwNmQwNDdiNjJlODE2NzcyNWUz
MmY4ZWNhYTA4MzNkOGYzNzYxMTplODkwNDU4ZDI4OTE5MGM3MzRjOWY1YWMw
NTQ4ZDVkM2IzMGRmMmRmOGVmMTQyZTE1MWRmNzQxY2U1ZjgxZjk0

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
	-u 503c8103ee84dcb38b910fda9906d047b62e8167725e32f8ecaa0833d8f37611:e890458d289190c734c9f5ac0548d5d3b30df2df8ef142e151df741ce5f81f94
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
{"grant_type":"client_credentials","client_id":"88068a551d2282f11633d5192d5d9cd054f9a5cfcb454419e045b96f3a707125","client_secret":"2e8a06c69ff64d5752ffcf2070a35c25567afea9a73c5b0496307bc2d5d00780"}
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
  "access_token": "7739cd57f5835689b00d0449528c337f0c261ddc4968d926746046f50530ebbb",
  "token_type": "bearer",
  "created_at": 1477504832
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"88068a551d2282f11633d5192d5d9cd054f9a5cfcb454419e045b96f3a707125","client_secret":"2e8a06c69ff64d5752ffcf2070a35c25567afea9a73c5b0496307bc2d5d00780"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ba3707b613adb38b1e27f4dc6b7dd5d7ca795cd997cc92d0efbd66ac9c2358d4","client_secret":"d325016685d2d533aa464fdc81125d519b41465f42ab1e140ea9ce38fd6d840e"}
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
  "access_token": "e28bfeb0103097ce0cd8ef1f2ce44fb90cd54669596faabe3c1174bca58ed3e0",
  "token_type": "bearer",
  "created_at": 1477504832
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ba3707b613adb38b1e27f4dc6b7dd5d7ca795cd997cc92d0efbd66ac9c2358d4","client_secret":"d325016685d2d533aa464fdc81125d519b41465f42ab1e140ea9ce38fd6d840e"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NmMzODBkYTI0N2FiNTY2MWRmOWJjNmU3ZGFhNWE2ZTBjZWJkZTBmMTE1NGNi
ZjNjZTM5Zjg5YjU5ZDgwN2EzNzo2MmQ3ZDY2YzAzOGRiMjBhOGQ3NjUxZTRi
ZTNlMThlNTNhYzNkNDBkZGUwNzdjMmJiM2FhMTRkOGU4NWYwMmZh

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
  "access_token": "bfc7f6c61705f81e27ac94ee9ae37bd0bb3443e99130a17ef085fa9bd9702276",
  "token_type": "bearer",
  "created_at": 1477504832
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 6c380da247ab5661df9bc6e7daa5a6e0cebde0f1154cbf3ce39f89b59d807a37:62d7d66c038db20a8d7651e4be3e18e53ac3d40dde077c2bb3aa14d8e85f02fa
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
Authorization: Bearer 0773118ac122d3705d62cfd8cc49fa88bf34ad804e4248b0b7c6075d9f602810
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
    "company_id": 1,
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
	-H "Authorization: Bearer 0773118ac122d3705d62cfd8cc49fa88bf34ad804e4248b0b7c6075d9f602810"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/158/flashcards
Content-Type: application/json
Authorization: Bearer 6dc4f2ebe152032ad976bc2894209b38044476bd4cef2261eaeb262f96a1558d
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":158,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 746,
    "chapter_id": 158,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:01:21.214Z",
    "created_at": "2016-10-26T18:01:21.214Z",
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
curl "api.goskive.com/v2/chapters/158/flashcards" -d '{"flashcard":{"chapter_id":158,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dc4f2ebe152032ad976bc2894209b38044476bd4cef2261eaeb262f96a1558d"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/157/flashcards
Content-Type: application/json
Authorization: Bearer 7153e22c28c0b2522b172a1e1f777abfca9f2ac4c9ca2d191931defe57bd0699
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 741,
      "chapter_id": 157,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:20.903Z",
      "created_at": "2016-10-26T18:01:20.903Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 741,
      "chapter_id": 157,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:20.942Z",
      "created_at": "2016-10-26T18:01:20.942Z",
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
      "author_id": 741,
      "chapter_id": 157,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:20.980Z",
      "created_at": "2016-10-26T18:01:20.980Z",
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
curl "api.goskive.com/v2/chapters/157/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7153e22c28c0b2522b172a1e1f777abfca9f2ac4c9ca2d191931defe57bd0699"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/115/questions
Content-Type: application/json
Authorization: Bearer d05d7025b6c006c19a6354757f2ee61d0463f899e0a458976246674766196f8c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":115,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 69,
    "obfuscated_id": "1EDi_PBgOnI",
    "author_id": 483,
    "chapter_id": 115,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:00:56.743Z",
    "created_at": "2016-10-26T18:00:56.743Z",
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
        "id": 137,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 138,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 139,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 140,
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
curl "api.goskive.com/v2/chapters/115/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":115,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d05d7025b6c006c19a6354757f2ee61d0463f899e0a458976246674766196f8c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/116/questions
Content-Type: application/json
Authorization: Bearer e3496956317728e1442bdf53605a1ab6a3633d8082028d63a9d4bcbfa0496ae2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 70,
    "obfuscated_id": "EDEz1xzotLc",
    "author_id": 486,
    "chapter_id": 116,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:00:57.411Z",
    "created_at": "2016-10-26T18:00:57.411Z",
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
        "id": 141,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 142,
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
curl "api.goskive.com/v2/chapters/116/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3496956317728e1442bdf53605a1ab6a3633d8082028d63a9d4bcbfa0496ae2"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/117/questions
Content-Type: application/json
Authorization: Bearer b8858909ceaba1e8fb7d72331f92769e81f85aa4a2c6b2d668e2036b968c8a93
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":117,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 71,
    "obfuscated_id": "--JhLc6KEBw",
    "author_id": 489,
    "chapter_id": 117,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:00:57.824Z",
    "created_at": "2016-10-26T18:00:57.824Z",
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
        "id": 143,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 144,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/117/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":117,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8858909ceaba1e8fb7d72331f92769e81f85aa4a2c6b2d668e2036b968c8a93"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/118/questions
Content-Type: application/json
Authorization: Bearer f34d915be7a2b035b9494fa97971f5ceee5595da6e82e4fb4659aa14b928db22
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":118,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 72,
    "obfuscated_id": "oqzxOzwzIgw",
    "author_id": 492,
    "chapter_id": 118,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:00:58.240Z",
    "created_at": "2016-10-26T18:00:58.240Z",
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
        "id": 145,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 146,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 147,
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
curl "api.goskive.com/v2/chapters/118/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":118,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f34d915be7a2b035b9494fa97971f5ceee5595da6e82e4fb4659aa14b928db22"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/113/questions
Content-Type: application/json
Authorization: Bearer 893d86fe69f1dfc330df7d81ac2a380d82f618f53cf0fa2e14374617a964b5fb
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
      "author_id": 474,
      "chapter_id": 113,
      "position": 66,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:55.777Z",
      "created_at": "2016-10-26T18:00:55.615Z",
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
          "id": 131,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 132,
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
      "author_id": 475,
      "chapter_id": 113,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:56.037Z",
      "created_at": "2016-10-26T18:00:55.868Z",
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
          "id": 133,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 134,
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
      "author_id": 476,
      "chapter_id": 113,
      "position": 68,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:56.299Z",
      "created_at": "2016-10-26T18:00:56.129Z",
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
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/113/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 893d86fe69f1dfc330df7d81ac2a380d82f618f53cf0fa2e14374617a964b5fb"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/21
Content-Type: application/json
Authorization: Bearer e3ef2afbbb3467b3b3ebfb4827c1be3fc05441f035059de0990a3d5c795fbfce
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
curl "api.goskive.com/v2/chapters/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3ef2afbbb3467b3b3ebfb4827c1be3fc05441f035059de0990a3d5c795fbfce"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/23
Content-Type: application/json
Authorization: Bearer c25d2d849f801fe0d832fb4347ed46685bb2f9fd92218d872cdbda9d298ec640
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
curl "api.goskive.com/v2/chapters/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c25d2d849f801fe0d832fb4347ed46685bb2f9fd92218d872cdbda9d298ec640"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/26
Content-Type: application/json
Authorization: Bearer e171789a56273ee3a1c061acd0a8e2fb708d9343fdf22c1b6bf72697e155b077
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
curl "api.goskive.com/v2/chapters/26" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e171789a56273ee3a1c061acd0a8e2fb708d9343fdf22c1b6bf72697e155b077"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/22
Content-Type: application/json
Authorization: Bearer c130ba36dde0f993c2dab2989792934c08abf857a3282483f0a08e4a983e6c88
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c130ba36dde0f993c2dab2989792934c08abf857a3282483f0a08e4a983e6c88"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/29
Content-Type: application/json
Authorization: Bearer f9390de0f0f9f8511304e0de30e0869a0c8c1721ff1c82332946b84e26ae4812
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
    "id": 29,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T18:00:27.149Z",
    "course_id": 36,
    "author_id": 119,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-26T18:00:26.573Z",
    "questions_updated_at": "2016-10-26T18:00:26.573Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 123,
        "chapter_id": 29,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:27.128Z",
        "created_at": "2016-10-26T18:00:27.128Z",
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
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 121,
        "chapter_id": 29,
        "position": 40,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:27.015Z",
        "created_at": "2016-10-26T18:00:26.879Z",
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
            "id": 79,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 80,
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
curl "api.goskive.com/v2/chapters/29" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9390de0f0f9f8511304e0de30e0869a0c8c1721ff1c82332946b84e26ae4812"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/25
Content-Type: application/json
Authorization: Bearer 546a6a13b19f9b159956fcca3f4ee3f85d1b9f17383253fdc8dcbba6551c7e69
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
    "id": 25,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T18:00:25.585Z",
    "course_id": 32,
    "author_id": 104,
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
curl "api.goskive.com/v2/chapters/25" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 546a6a13b19f9b159956fcca3f4ee3f85d1b9f17383253fdc8dcbba6551c7e69"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer e8a596d52c2e17fe22b663613a84fadc8d69b777d31f0dbc6e5485c5eb469a72
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
    "id": 59,
    "author_id": 819,
    "reply_to_id": 58,
    "created_at": "2016-10-26T18:01:28.341Z",
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
curl "api.goskive.com/v2/comments/58/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8a596d52c2e17fe22b663613a84fadc8d69b777d31f0dbc6e5485c5eb469a72"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/57/replies
Content-Type: application/json
Authorization: Bearer 3fd5f37183e3590b9b2580dceeed9ebe1c3f522211a67b3916e4bc1dae11c0a1
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
curl "api.goskive.com/v2/comments/57/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fd5f37183e3590b9b2580dceeed9ebe1c3f522211a67b3916e4bc1dae11c0a1"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/56
Content-Type: application/json
Authorization: Bearer a9ef9c3581d5f644c9f2fbbd8c29a22bd6ba6b74f7ad0931e80472c3cb4bb63c
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
curl "api.goskive.com/v2/comments/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9ef9c3581d5f644c9f2fbbd8c29a22bd6ba6b74f7ad0931e80472c3cb4bb63c"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/52/republish
Content-Type: application/json
Authorization: Bearer d9838eb44312578d000dd0fda0edb46571435df9d9919e4d732434a6253969fd
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
curl "api.goskive.com/v2/comments/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9838eb44312578d000dd0fda0edb46571435df9d9919e4d732434a6253969fd"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer 2c01c38aa9a6fe13445befd85a66939abe8551d26912e03114c3f91c65617ad0
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
	-H "Authorization: Bearer 2c01c38aa9a6fe13445befd85a66939abe8551d26912e03114c3f91c65617ad0"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/16/report
Content-Type: application/json
Authorization: Bearer ffa31752947ce233420f937603826f4a4730dcb948d583852fbe78e54d1dd2f4
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffa31752947ce233420f937603826f4a4730dcb948d583852fbe78e54d1dd2f4"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/5
Content-Type: application/json
Authorization: Bearer ecddbefe4ec13e60d97a739f7694df231fdbe1795fd0491478035af244dc049f
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
    "id": 5,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-26T18:00:35.388Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecddbefe4ec13e60d97a739f7694df231fdbe1795fd0491478035af244dc049f"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer c6e3040bb950968f09b70b9f325557e9a675368199c71532636301cf6aea014c
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
      "id": 6,
      "name": "Fake Company Name 4",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T18:00:35.462Z"
    },
    {
      "id": 7,
      "name": "Fake Company Name 5",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T18:00:35.466Z"
    },
    {
      "id": 8,
      "name": "Fake Company Name 6",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T18:00:35.470Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6e3040bb950968f09b70b9f325557e9a675368199c71532636301cf6aea014c"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/10/company_profiles
Content-Type: application/json
Authorization: Bearer d1903965e1420649726b1efd8f58138de576b98f71a8afbe3aad46c47a431424
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
	-H "Authorization: Bearer d1903965e1420649726b1efd8f58138de576b98f71a8afbe3aad46c47a431424"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/9/company_profiles
Content-Type: application/json
Authorization: Bearer 6d44b0baee7917d3f4fe9111832f9a1e53543870c06f456ac4c83a0a132c41c5
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
	-H "Authorization: Bearer 6d44b0baee7917d3f4fe9111832f9a1e53543870c06f456ac4c83a0a132c41c5"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer fba03321eae9c15fb20702f87ff6c1a1cc81e82d49575f70ef93a5bdb5f4197d
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
      "company_id": 12,
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
      "company_id": 15,
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
	-H "Authorization: Bearer fba03321eae9c15fb20702f87ff6c1a1cc81e82d49575f70ef93a5bdb5f4197d"
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
Authorization: Bearer 4a1d51b9890c43bf1081067142c9df1c668fa6c1fdffeab0dcab259abc9e71b3
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
	-H "Authorization: Bearer 4a1d51b9890c43bf1081067142c9df1c668fa6c1fdffeab0dcab259abc9e71b3"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 58024f4b095685f7196dded2c21f81101c050ae20eef2d5355759534b6b40022
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
    "updated_at": "2016-10-26T18:00:35.925Z",
    "course_id": 61,
    "author_id": 221,
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
	-H "Authorization: Bearer 58024f4b095685f7196dded2c21f81101c050ae20eef2d5355759534b6b40022"
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
      "id": 54,
      "title": "Clever Chapter Title 42",
      "position": 1,
      "updated_at": "2016-10-26T18:00:36.457Z",
      "course_id": 65,
      "author_id": 232,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 55,
      "title": "Clever Chapter Title 43",
      "position": 2,
      "updated_at": "2016-10-26T18:00:36.484Z",
      "course_id": 65,
      "author_id": 233,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 56,
      "title": "Clever Chapter Title 44",
      "position": 3,
      "updated_at": "2016-10-26T18:00:36.803Z",
      "course_id": 65,
      "author_id": 234,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T18:00:36.381Z",
      "questions_updated_at": "2016-10-26T18:00:36.381Z",
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
Authorization: Bearer 90a80f9910ea393ca80e0332f29781bb373fe491d16b01e55f3d5d31dbb76d71
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
      "title": "Clever Chapter Title 54",
      "position": 1,
      "updated_at": "2016-10-26T18:00:37.981Z",
      "course_id": 71,
      "author_id": 257,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 67,
      "title": "Clever Chapter Title 55",
      "position": 2,
      "updated_at": "2016-10-26T18:00:38.009Z",
      "course_id": 71,
      "author_id": 258,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 68,
      "title": "Clever Chapter Title 56",
      "position": 3,
      "updated_at": "2016-10-26T18:00:38.322Z",
      "course_id": 71,
      "author_id": 259,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T18:00:37.906Z",
      "questions_updated_at": "2016-10-26T18:00:37.906Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90a80f9910ea393ca80e0332f29781bb373fe491d16b01e55f3d5d31dbb76d71"
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
      "id": 57,
      "title": "Clever Chapter Title 45",
      "position": 1,
      "updated_at": "2016-10-26T18:00:36.925Z",
      "course_id": 66,
      "author_id": 238,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 58,
      "title": "Clever Chapter Title 46",
      "position": 2,
      "updated_at": "2016-10-26T18:00:36.951Z",
      "course_id": 66,
      "author_id": 239,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 59,
      "title": "Clever Chapter Title 47",
      "position": 3,
      "updated_at": "2016-10-26T18:00:36.978Z",
      "course_id": 66,
      "author_id": 240,
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
Authorization: Bearer 096a2809a75f33504d381cfb0cadcd956814505f85b1d9ea4a95230342f1dbb6
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
      "title": "Clever Chapter Title 57",
      "position": 1,
      "updated_at": "2016-10-26T18:00:38.607Z",
      "course_id": 73,
      "author_id": 266,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 70,
      "title": "Clever Chapter Title 58",
      "position": 2,
      "updated_at": "2016-10-26T18:00:38.634Z",
      "course_id": 73,
      "author_id": 267,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 71,
      "title": "Clever Chapter Title 59",
      "position": 3,
      "updated_at": "2016-10-26T18:00:38.662Z",
      "course_id": 73,
      "author_id": 268,
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
	-H "Authorization: Bearer 096a2809a75f33504d381cfb0cadcd956814505f85b1d9ea4a95230342f1dbb6"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 49977228e8514e2aaf7c16189daf4f85e28657ddae01e4bc3aa4bb8cd1db8c89
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
    "course_id": 307,
    "user_id": 961,
    "updated_at": "2016-10-26T18:01:37.360Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49977228e8514e2aaf7c16189daf4f85e28657ddae01e4bc3aa4bb8cd1db8c89"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 486cd7a81abaaebe7fb26314380a9b2a4f9efbc56ea74aa368346bab264bb358
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
      "course_id": 303,
      "user_id": 949,
      "updated_at": "2016-10-26T18:01:36.790Z"
    },
    {
      "id": 3,
      "course_id": 303,
      "user_id": 950,
      "updated_at": "2016-10-26T18:01:36.806Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 486cd7a81abaaebe7fb26314380a9b2a4f9efbc56ea74aa368346bab264bb358"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/261/files
Content-Type: application/json
Authorization: Bearer 3bdcc67ffe0cdd71bd3f78018d6563b06b9b628f365dc67d47cf276b61c8ac66
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
      "id": 12,
      "uploader": {
        "id": 769,
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
        "created_at": "2016-10-26T18:01:24.363Z",
        "updated_at": "2016-10-26T18:01:24.363Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T18:01:24.374Z",
      "updated_at": "2016-10-26T18:01:24.374Z",
      "course_id": 261,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 770,
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
        "created_at": "2016-10-26T18:01:24.383Z",
        "updated_at": "2016-10-26T18:01:24.383Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T18:01:24.392Z",
      "updated_at": "2016-10-26T18:01:24.392Z",
      "course_id": 261,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 771,
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
        "created_at": "2016-10-26T18:01:24.399Z",
        "updated_at": "2016-10-26T18:01:24.399Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T18:01:24.409Z",
      "updated_at": "2016-10-26T18:01:24.409Z",
      "course_id": 261,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/261/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bdcc67ffe0cdd71bd3f78018d6563b06b9b628f365dc67d47cf276b61c8ac66"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/262/files
Content-Type: application/json
Authorization: Bearer 4186631f79e65b78b8f111b6f7fa94ece814a802347cb4a7609534a6b39c56ac
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
    "id": 15,
    "uploader": {
      "id": 774,
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
      "created_at": "2016-10-26T18:01:24.527Z",
      "updated_at": "2016-10-26T18:01:24.527Z"
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
    "created_at": "2016-10-26T18:01:24.553Z",
    "updated_at": "2016-10-26T18:01:24.553Z",
    "course_id": 262,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/262/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4186631f79e65b78b8f111b6f7fa94ece814a802347cb4a7609534a6b39c56ac"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/263/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer ba3fb160c11f73aed2697724410026be1919751eb36cc183fb068ad6ef765d53
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
    "key": "cache/b62ec3d7c9f7eaa4ad550ad0eac8fb61.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxOTowMToyNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I2MmVjM2Q3YzlmN2VhYTRhZDU1MGFkMGVhYzhmYjYxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI2VDE4MDEyNFoifV19",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T180124Z",
    "x-amz-signature": "70aa996c90d0cae3dc05789040e314ab8dc500774a67411a21b3c060a5a3594f"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/263/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba3fb160c11f73aed2697724410026be1919751eb36cc183fb068ad6ef765d53"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 1a27361b37584b604722f93d521f5c3684fe37333921543f27be9baabee37211
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
	-H "Authorization: Bearer 1a27361b37584b604722f93d521f5c3684fe37333921543f27be9baabee37211"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f6e49c52a3274c5ad99d658f625647fc5be33f6ce38e652bc8aa34e0592d87e7
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
	-H "Authorization: Bearer f6e49c52a3274c5ad99d658f625647fc5be33f6ce38e652bc8aa34e0592d87e7"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8ba63d08a8e07ec2ce00261c233b295cbce20538ed8aafb45a4376fae4fa5442
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
	-H "Authorization: Bearer 8ba63d08a8e07ec2ce00261c233b295cbce20538ed8aafb45a4376fae4fa5442"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ad26b1c15f402389d200eacc406a1403f45acdee6a377a7ded8182ab7148b10d
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
	-H "Authorization: Bearer ad26b1c15f402389d200eacc406a1403f45acdee6a377a7ded8182ab7148b10d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer dc080a9d200adc928569a2020af0710b86f16424fa7b9ce00ce37d428551ce61
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
	-H "Authorization: Bearer dc080a9d200adc928569a2020af0710b86f16424fa7b9ce00ce37d428551ce61"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer aad99d8aa6c647853ac6fc72dfb3654b1fb1c6329e7a170c81c9babb14e181d0
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
    "creator_id": 52,
    "id": 15,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 15,
    "additional_university_ids": [

    ],
    "topic_id": 15,
    "discipline_id": 15,
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
    "chapters_updated_at": "2016-10-26T18:00:17.791Z",
    "updated_at": "2016-10-26T18:00:19.205Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 11,
        "title": "Clever Chapter Title 11",
        "position": 1,
        "updated_at": "2016-10-26T18:00:19.161Z",
        "course_id": 15,
        "author_id": 52,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T18:00:17.791Z",
        "questions_updated_at": "2016-10-26T18:00:17.791Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 12,
        "title": "Clever Chapter Title 12",
        "position": 2,
        "updated_at": "2016-10-26T18:00:19.198Z",
        "course_id": 15,
        "author_id": 52,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T18:00:17.791Z",
        "questions_updated_at": "2016-10-26T18:00:17.791Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 53,
        "chapter_id": 11,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:19.009Z",
        "created_at": "2016-10-26T18:00:19.009Z",
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
        "author_id": 53,
        "chapter_id": 12,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:19.077Z",
        "created_at": "2016-10-26T18:00:19.077Z",
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
        "author_id": 53,
        "chapter_id": 11,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:19.047Z",
        "created_at": "2016-10-26T18:00:19.047Z",
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
        "author_id": 53,
        "chapter_id": 12,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:19.115Z",
        "created_at": "2016-10-26T18:00:19.115Z",
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
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 53,
        "chapter_id": 11,
        "position": 15,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:18.003Z",
        "created_at": "2016-10-26T18:00:17.886Z",
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
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 53,
        "chapter_id": 11,
        "position": 16,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:18.176Z",
        "created_at": "2016-10-26T18:00:18.065Z",
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
            "id": 31,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 32,
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
        "author_id": 53,
        "chapter_id": 12,
        "position": 17,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:18.379Z",
        "created_at": "2016-10-26T18:00:18.256Z",
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
      },
      {
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 53,
        "chapter_id": 12,
        "position": 18,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:18.559Z",
        "created_at": "2016-10-26T18:00:18.443Z",
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
            "id": 35,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 36,
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
	-H "Authorization: Bearer aad99d8aa6c647853ac6fc72dfb3654b1fb1c6329e7a170c81c9babb14e181d0"
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
    "creator_id": 64,
    "id": 17,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 17,
    "additional_university_ids": [

    ],
    "topic_id": 17,
    "discipline_id": 17,
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
    "chapters_updated_at": "2016-10-26T18:00:20.871Z",
    "updated_at": "2016-10-26T18:00:22.406Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 15,
        "title": "Clever Chapter Title 15",
        "position": 1,
        "updated_at": "2016-10-26T18:00:22.355Z",
        "course_id": 17,
        "author_id": 64,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T18:00:20.871Z",
        "questions_updated_at": "2016-10-26T18:00:20.871Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 16,
        "title": "Clever Chapter Title 16",
        "position": 2,
        "updated_at": "2016-10-26T18:00:22.398Z",
        "course_id": 17,
        "author_id": 64,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T18:00:20.871Z",
        "questions_updated_at": "2016-10-26T18:00:20.871Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 64,
        "chapter_id": 15,
        "position": 27,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:21.090Z",
        "created_at": "2016-10-26T18:00:20.963Z",
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
      },
      {
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 64,
        "chapter_id": 16,
        "position": 29,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:21.500Z",
        "created_at": "2016-10-26T18:00:21.367Z",
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
            "id": 57,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 58,
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
PUT /v2/courses/27/pin
Content-Type: application/json
Authorization: Bearer 6fb805b20b65f9820cb537dd202df21fdf944c35e4b74048048c5276d02196c6
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/27/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fb805b20b65f9820cb537dd202df21fdf944c35e4b74048048c5276d02196c6"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/13/pin
Content-Type: application/json
Authorization: Bearer 31a39edcf7e4f2f6ed9ddbf5b7e47cd0892c3a84435c7a1404bfda8eefbe7e95
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/13/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31a39edcf7e4f2f6ed9ddbf5b7e47cd0892c3a84435c7a1404bfda8eefbe7e95"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2ea2092b735222a955dc81544407fda5c1c988de1a96bbe8e73943035407a06e
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
    "creator_id": 39,
    "id": 10,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 10,
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
    "updated_at": "2016-10-26T18:00:15.928Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ea2092b735222a955dc81544407fda5c1c988de1a96bbe8e73943035407a06e"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 11bca6fd29a10ec0275c6f30108b7cdcb40e3ec09283431f16d454889e83fa03
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
    "id": 279,
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
    "created_at": "2016-10-26T18:00:39.623Z",
    "updated_at": "2016-10-26T18:00:39.623Z",
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
	-H "Authorization: Bearer 11bca6fd29a10ec0275c6f30108b7cdcb40e3ec09283431f16d454889e83fa03"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c4671a1bf93e783eb9f6a9e37d327c7b9373d96a322e85769aa0f7c56b15b3e4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[81]}
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
    "id": 274,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      81
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T18:00:39.000Z",
    "updated_at": "2016-10-26T18:00:39.048Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[81]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4671a1bf93e783eb9f6a9e37d327c7b9373d96a322e85769aa0f7c56b15b3e4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 67250d5b1db44cf1121cb11140b44f59f27789de76a8ff6eaaa34041d469997a
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
    "id": 275,
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
    "created_at": "2016-10-26T18:00:39.079Z",
    "updated_at": "2016-10-26T18:00:39.079Z",
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
	-H "Authorization: Bearer 67250d5b1db44cf1121cb11140b44f59f27789de76a8ff6eaaa34041d469997a"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9ab6ad8c57e9a3c6c04fa101d23538dc7097663cd8ec0b590ce72b46e7fef268
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[84]}
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
    "id": 277,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      84
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T18:00:39.245Z",
    "updated_at": "2016-10-26T18:00:39.245Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[84]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ab6ad8c57e9a3c6c04fa101d23538dc7097663cd8ec0b590ce72b46e7fef268"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer f95aab06e7914122c91ef6b968260b625c293dfb137d339285ed5cfcb60b0a07
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

85
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
    "id": 278,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/71b3559ae8017c29b22bfab4302218349bb9e630.jpg",
    "university_id": null,
    "fields_of_study": [
      85
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T18:00:39.316Z",
    "updated_at": "2016-10-26T18:00:39.593Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/3f4f1628325753281e980e60d389ee25e3054bc0.jpg",
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

85
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer f95aab06e7914122c91ef6b968260b625c293dfb137d339285ed5cfcb60b0a07"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 1d5e9a5fc05fc5d2b1e25ceef0e071dab5910ac6152b28d7b72188d1fc9c1168
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
      "bookmarkable_id": 51,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 52,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 53,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d5e9a5fc05fc5d2b1e25ceef0e071dab5910ac6152b28d7b72188d1fc9c1168"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer add399697ca2ce2cc829d7c6f523f63079ddf6b3da1f2ca3d388a198512a7f56
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
      "company_id": 28,
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
      "company_id": 29,
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
	-H "Authorization: Bearer add399697ca2ce2cc829d7c6f523f63079ddf6b3da1f2ca3d388a198512a7f56"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 51e83d89c8b79bf6ffaa4a4ac1e3ad12c107d5be12376c8fef4861b8497ea5ba
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
      "company_id": 24,
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
	-H "Authorization: Bearer 51e83d89c8b79bf6ffaa4a4ac1e3ad12c107d5be12376c8fef4861b8497ea5ba"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 95f5eaf12ad02a13cae881457ad22d711ed60e67b0fc38d8842abfdc51ebaa45
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
      "creator_id": 805,
      "id": 270,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-204",
      "html_url": "https://goskive.com/course/mit-course-204",
      "slug": "mit-course-204",
      "university_id": 255,
      "additional_university_ids": [

      ],
      "topic_id": 282,
      "discipline_id": 283,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 204",
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
      "updated_at": "2016-10-26T18:01:27.233Z",
      "shortname": "mit-course-204"
    },
    {
      "creator_id": 806,
      "id": 271,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-205",
      "html_url": "https://goskive.com/course/mit-course-205",
      "slug": "mit-course-205",
      "university_id": 256,
      "additional_university_ids": [

      ],
      "topic_id": 283,
      "discipline_id": 284,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 205",
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
      "updated_at": "2016-10-26T18:01:27.315Z",
      "shortname": "mit-course-205"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95f5eaf12ad02a13cae881457ad22d711ed60e67b0fc38d8842abfdc51ebaa45"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer b4198fa064012546cfbde3165056bb1430bd027e26018955d1a4d2d7796d3c04
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
        "updated_at": "2016-10-26T18:01:27.575Z"
      },
      "created_at": "2016-10-26T18:01:27.578Z",
      "updated_at": "2016-10-26T18:01:27.578Z",
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
        "updated_at": "2016-10-26T18:01:27.585Z"
      },
      "created_at": "2016-10-26T18:01:27.588Z",
      "updated_at": "2016-10-26T18:01:27.588Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4198fa064012546cfbde3165056bb1430bd027e26018955d1a4d2d7796d3c04"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 7e995c187e3319950bdeb6ecc494cede8394242640c9c6b91587b2d787d7f919
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
      "company_id": 33,
      "company": {
        "id": 33,
        "name": "Fake Company Name 28",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T18:01:27.378Z"
      },
      "created_at": "2016-10-26T18:01:27.381Z",
      "updated_at": "2016-10-26T18:01:27.381Z",
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
      "company_id": 34,
      "company": {
        "id": 34,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T18:01:27.395Z"
      },
      "created_at": "2016-10-26T18:01:27.399Z",
      "updated_at": "2016-10-26T18:01:27.399Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e995c187e3319950bdeb6ecc494cede8394242640c9c6b91587b2d787d7f919"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 77237099d03f0fc4e20e985aa1a06be37510c328ad82536ba490b088470fad48
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
      "created_at": "2016-10-26T18:00:27.911Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 4,
      "updated_at": "2016-10-26T18:00:28.017Z",
      "author_id": "135",
      "thread_subject_id": "39",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 5,
      "created_at": "2016-10-26T18:00:28.006Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 5,
      "updated_at": "2016-10-26T18:00:28.020Z",
      "author_id": "138",
      "thread_subject_id": "40",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-26T18:00:28.437Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-26T18:00:28.437Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-26T18:00:28.841Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-26T18:00:28.841Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 8,
      "created_at": "2016-10-26T18:00:29.266Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-26T18:00:29.266Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 9,
      "created_at": "2016-10-26T18:00:29.585Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 45,
      "updated_at": "2016-10-26T18:00:29.585Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-26T18:00:29.908Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 46,
      "updated_at": "2016-10-26T18:00:29.908Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-26T18:00:30.253Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 47,
      "updated_at": "2016-10-26T18:00:30.253Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77237099d03f0fc4e20e985aa1a06be37510c328ad82536ba490b088470fad48"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/3
Content-Type: application/json
Authorization: Bearer 054db4dcf1f7f6c24f3895332a20b46a735c987bb178299ea2abf12ea92aa48a
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-26T17:50:27.000Z"}}
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
    "created_at": "2016-10-26T18:00:27.695Z",
    "read_at": "2016-10-26T17:50:27.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 3,
    "updated_at": "2016-10-26T18:00:27.766Z",
    "author_id": "130",
    "thread_subject_id": "38",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/3" -d '{"notification":{"read_at":"2016-10-26T17:50:27.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 054db4dcf1f7f6c24f3895332a20b46a735c987bb178299ea2abf12ea92aa48a"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 09f9d6db3da95c9adb6b1bbd2e972ff7b4420e73d308a6df48e8c169b4ead5c6
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
      "course_id": 132,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T18:00:55.134Z",
      "course_published": true,
      "updated_at": "2016-10-26T18:00:55.120Z"
    },
    {
      "id": 5,
      "course_id": 133,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T18:00:55.215Z",
      "course_published": true,
      "updated_at": "2016-10-26T18:00:55.207Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09f9d6db3da95c9adb6b1bbd2e972ff7b4420e73d308a6df48e8c169b4ead5c6"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 6451194b404d2ed1f4ac6922b1506859ccd49cc4b2e44c146466b01625398adf
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
    "course_id": 131,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T18:00:55.011Z",
    "course_published": true,
    "updated_at": "2016-10-26T18:00:55.002Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6451194b404d2ed1f4ac6922b1506859ccd49cc4b2e44c146466b01625398adf"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 42c50077138ea3d1d7b51d27694fd5731272e16f02713dd135181f17c5b0a410
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
    "id": 2,
    "course_id": 130,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-26T18:00:54.909Z",
    "course_published": true,
    "updated_at": "2016-10-26T18:00:54.896Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42c50077138ea3d1d7b51d27694fd5731272e16f02713dd135181f17c5b0a410"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer b1f3d7b74e12a2bfd0b6359b3ca61b620747c31b30f233a28262e57c174aebfd
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
      "votable_id": 62,
      "user_id": 442
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 63,
      "user_id": 442
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 64,
      "user_id": 442
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 65,
      "user_id": 442
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1f3d7b74e12a2bfd0b6359b3ca61b620747c31b30f233a28262e57c174aebfd"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/61
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
    "id": 61,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 59,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 61
      },
      {
        "id": 60,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 61
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/61" -X GET \
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
      "id": 59,
      "name": "Organized well-modulated leverage",
      "name_translations": {
        "en": "Organized well-modulated leverage"
      }
    },
    {
      "id": 60,
      "name": "Re-contextualized regional matrices",
      "name_translations": {
        "en": "Re-contextualized regional matrices"
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
PATCH /v2/feedbacks/43/close
Content-Type: application/json
Authorization: Bearer aff8812732b6b5a8758c770f34b48c9482630dd97708da703edad03d6e1c0a01
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
    "id": 43,
    "user_id": 929,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-26T18:01:35.870Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/43/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aff8812732b6b5a8758c770f34b48c9482630dd97708da703edad03d6e1c0a01"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/39/fix
Content-Type: application/json
Authorization: Bearer 3a4935a0eddbec2a1d4ebff14aed757df9ca890fb598f475ceccb94c79be12a0
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
    "id": 39,
    "user_id": 909,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-26T18:01:34.837Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/39/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a4935a0eddbec2a1d4ebff14aed757df9ca890fb598f475ceccb94c79be12a0"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/45
Content-Type: application/json
Authorization: Bearer 63d285187a1d444bef0c4f9ff82f4e7fe0fdd27ae914ebaf3c5175787770a62e
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
    "id": 45,
    "user_id": 939,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T18:01:36.336Z",
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
curl "api.goskive.com/v2/feedbacks/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63d285187a1d444bef0c4f9ff82f4e7fe0fdd27ae914ebaf3c5175787770a62e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/40/fix
Content-Type: application/json
Authorization: Bearer 3df295c7bfd547a889f74358d3629a0f8dea6a546a7564016d44d9cc07d9d88a
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
	-H "Authorization: Bearer 3df295c7bfd547a889f74358d3629a0f8dea6a546a7564016d44d9cc07d9d88a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/41/fix
Content-Type: application/json
Authorization: Bearer 8e1489e752917b846e9c104a8268017c44182b70c0047fcce916c6a798a6aff0
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
curl "api.goskive.com/v2/feedbacks/41/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e1489e752917b846e9c104a8268017c44182b70c0047fcce916c6a798a6aff0"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/close
Content-Type: application/json
Authorization: Bearer cbe7d096d72a51aeb29ddf570505af447557a84048e124cbbc3409a227a8149e
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
curl "api.goskive.com/v2/feedbacks/44/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbe7d096d72a51aeb29ddf570505af447557a84048e124cbbc3409a227a8149e"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/46
Content-Type: application/json
Authorization: Bearer 6a1478c5af37d4d961be932cf1aca1aac3cb45b8fd982e04291b5ee84bcf45d0
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
    "id": 46,
    "user_id": 944,
    "feedbackable_id": 92,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T18:01:36.624Z",
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
curl "api.goskive.com/v2/feedbacks/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a1478c5af37d4d961be932cf1aca1aac3cb45b8fd982e04291b5ee84bcf45d0"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer e1ea178e3ecaa5c93a9a4bf890a8565be18c344848601e0800c3b213252f9420
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
	-H "Authorization: Bearer e1ea178e3ecaa5c93a9a4bf890a8565be18c344848601e0800c3b213252f9420"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/1/bookmark
Content-Type: application/json
Authorization: Bearer 4b93057d21bd05320273f4f01893b08835859e86aaa44ee1173b65f8f617b1f3
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
	-H "Authorization: Bearer 4b93057d21bd05320273f4f01893b08835859e86aaa44ee1173b65f8f617b1f3"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer e43233864cedc0598bb5baa813a1c12a1fba088d450f43f15327208e87bef378
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e43233864cedc0598bb5baa813a1c12a1fba088d450f43f15327208e87bef378"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/2
Content-Type: application/json
Authorization: Bearer d31c71a71f1f3177bed689cbd08080ccaa6a15b4a88b53dbcca59d3cc72b0536
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/6839479da4b16543a7816bc1832163a6.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T180042Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6ed46e37363dbd079c441ffcd85610b7fcea04eeb384c1db764f4c3661d1374b",
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
	-H "Authorization: Bearer d31c71a71f1f3177bed689cbd08080ccaa6a15b4a88b53dbcca59d3cc72b0536"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/3/preview
Content-Type: application/json
Authorization: Bearer f0c1b120f995072869ef444a9711db125b08b5d990b065f1b4e06105457239df
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/fbb574e8e36a39036611476220aa1bf6.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T180042Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e1f8bfa95a66390083933dba0436790264b682fa2d7970e2d600e115c048d539",
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
	-H "Authorization: Bearer f0c1b120f995072869ef444a9711db125b08b5d990b065f1b4e06105457239df"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Content-Type: application/json
Authorization: Bearer f4524e7bc458e5daa2a6f55095b207cd44ba06a2f0c0793f3233943e653040f8
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
      "id": 309,
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
      "created_at": "2016-10-26T18:00:42.371Z",
      "updated_at": "2016-10-26T18:00:42.371Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-26T18:00:42.445Z",
    "updated_at": "2016-10-26T18:00:42.445Z",
    "course_id": 83,
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4524e7bc458e5daa2a6f55095b207cd44ba06a2f0c0793f3233943e653040f8"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/17/matched_courses?required_cu_count=2
Authorization: Bearer cc6ff3bd620287cd27258aa031abebc3487f99eb43bc111fef7e2a6788efba7f
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
      "creator_id": 790,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 279,
      "discipline_id": 280,
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
      "chapters_updated_at": "2016-10-26T18:01:24.868Z",
      "updated_at": "2016-10-26T18:01:26.417Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 795,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-a1549061-3fba-46ae-b556-8f6dd9693f9a",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-a1549061-3fba-46ae-b556-8f6dd9693f9a",
      "slug": "mit-the-great-british-bake-off-a1549061-3fba-46ae-b556-8f6dd9693f9a",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 280,
      "discipline_id": 281,
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
      "chapters_updated_at": "2016-10-26T18:01:24.868Z",
      "updated_at": "2016-10-26T18:01:26.954Z",
      "shortname": "mit-the-great-british-bake-off-a1549061-3fba-46ae-b556-8f6dd9693f9a"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/17/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer cc6ff3bd620287cd27258aa031abebc3487f99eb43bc111fef7e2a6788efba7f"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/8/report
Content-Type: application/json
Authorization: Bearer a20229ef215b6f0a195cc77e860a32d8df99b49b7a948cb9f0f924ebc214c7e7
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a20229ef215b6f0a195cc77e860a32d8df99b49b7a948cb9f0f924ebc214c7e7"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/4/bookmark
Content-Type: application/json
Authorization: Bearer b706820551e9ec837b169edfaf06409c64959bdfa60cc04fc02d724a7df5cbe2
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b706820551e9ec837b169edfaf06409c64959bdfa60cc04fc02d724a7df5cbe2"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/33/comments
Content-Type: application/json
Authorization: Bearer 78e305b44a60719fb452eb55429f6dce4965c8da56ad314d47290bfa157e06a7
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
    "author_id": 191,
    "reply_to_id": null,
    "created_at": "2016-10-26T18:00:33.564Z",
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
curl "api.goskive.com/v2/flashcards/33/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78e305b44a60719fb452eb55429f6dce4965c8da56ad314d47290bfa157e06a7"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/31/comments
Content-Type: application/json
Authorization: Bearer 33d44cae9f913c67de50dea58582e5370a9c3a15734ee1b4c1c3c8654bd5923e
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
    "author_id": 185,
    "reply_to_id": null,
    "created_at": "2016-10-26T18:00:33.065Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 185,
      "feedbackable_id": 31,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:33.061Z",
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
curl "api.goskive.com/v2/flashcards/31/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33d44cae9f913c67de50dea58582e5370a9c3a15734ee1b4c1c3c8654bd5923e"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/34/comments
Content-Type: application/json
Authorization: Bearer f307d4e105a99184123fce6824de591a91f6a4418a5fa1a49d9a66920e318976
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
      "author_id": 197,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:00:33.896Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 198,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:00:33.911Z",
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
curl "api.goskive.com/v2/flashcards/34/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f307d4e105a99184123fce6824de591a91f6a4418a5fa1a49d9a66920e318976"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/32/comments
Content-Type: application/json
Authorization: Bearer ee4ecd139729a0f17c82bc26c93d982c8d923abcc2b47490ea67b9486987b721
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
curl "api.goskive.com/v2/flashcards/32/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee4ecd139729a0f17c82bc26c93d982c8d923abcc2b47490ea67b9486987b721"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/46/feedbacks
Content-Type: application/json
Authorization: Bearer c176f3bfbe88792212e9c20ce8beef488d2d5f8c65b294fdb18b30860c27eca1
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
    "id": 18,
    "user_id": 361,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T18:00:47.800Z",
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
curl "api.goskive.com/v2/flashcards/46/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c176f3bfbe88792212e9c20ce8beef488d2d5f8c65b294fdb18b30860c27eca1"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/43/feedbacks
Content-Type: application/json
Authorization: Bearer 4a6c06b2e35e4d41f5d01d03f11b9e86332c8218aadc80e4631d4c38a0254c92
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
      "id": 16,
      "user_id": 354,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:44.474Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 353,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:44.463Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a6c06b2e35e4d41f5d01d03f11b9e86332c8218aadc80e4631d4c38a0254c92"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/94/votes
Content-Type: application/json
Authorization: Bearer 873f64ec2c57e31c38d5cf841c31d807f0547ed842d1edfb56f9be873e0c2991
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
      "votable_id": 94,
      "user_id": 972
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 971
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 970
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/94/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 873f64ec2c57e31c38d5cf841c31d807f0547ed842d1edfb56f9be873e0c2991"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/67/republish
Content-Type: application/json
Authorization: Bearer b3aa6eddb9397d044c828eae7b3009c1b06b443e72b8bb27247025d1baef1a8c
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
curl "api.goskive.com/v2/flashcards/67/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3aa6eddb9397d044c828eae7b3009c1b06b443e72b8bb27247025d1baef1a8c"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/bookmark
Content-Type: application/json
Authorization: Bearer b260c129e888a1a060dbed88a1f088d3317a54ab6fe3975e48342a5bbafef3b1
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b260c129e888a1a060dbed88a1f088d3317a54ab6fe3975e48342a5bbafef3b1"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/63
Content-Type: application/json
Authorization: Bearer 4ad36d150cd021b63de5f360eefbd0ff702f343fceb9b3a2f246b6e9bb86e506
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ad36d150cd021b63de5f360eefbd0ff702f343fceb9b3a2f246b6e9bb86e506"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/downvote
Content-Type: application/json
Authorization: Bearer 743003a3eab6bfdfca5fc514026496e27c7d7881628d904f8491e137d28099fd
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 743003a3eab6bfdfca5fc514026496e27c7d7881628d904f8491e137d28099fd"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/66
Content-Type: application/json
Authorization: Bearer fc37adb85ee061b86bc9ab131f247fb67edbc3c04d76b192e896d08882845f9a
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 426,
    "chapter_id": 104,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:00:51.685Z",
    "created_at": "2016-10-26T18:00:51.685Z",
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
curl "api.goskive.com/v2/flashcards/66" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc37adb85ee061b86bc9ab131f247fb67edbc3c04d76b192e896d08882845f9a"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/47/report
Content-Type: application/json
Authorization: Bearer 87955d1dbf8b871121633d48d33126de26f8fe514bde29fb59852907c2c58188
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/47/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87955d1dbf8b871121633d48d33126de26f8fe514bde29fb59852907c2c58188"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/70/bookmark
Content-Type: application/json
Authorization: Bearer 1ad486277301317dec3a4e01bfa56ed9c61c757a44242e5462834fa62939f6ba
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/70/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ad486277301317dec3a4e01bfa56ed9c61c757a44242e5462834fa62939f6ba"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/upvote
Content-Type: application/json
Authorization: Bearer 3aeea60bf06e5af9ba1f6755da9cad0aa6126234f5d1bc1c35182086a85adb35
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aeea60bf06e5af9ba1f6755da9cad0aa6126234f5d1bc1c35182086a85adb35"
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
    "key": "cache/8954b5920d301ebb551e08370a0fc12c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxOTowMDozMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzg5NTRiNTkyMGQzMDFlYmI1NTFlMDgzNzBhMGZjMTJjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjZUMTgwMDMxWiJ9XX0=",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T180031Z",
    "x-amz-signature": "a02f3e849a72fb07edc74b4a090267317debcef7ef0a5273772708f010ecbe15"
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
Authorization: Bearer fed69132339d1f2a95dd7dec653125027f35f3040fe5c5d8080c432a2305ba58
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
curl "api.goskive.com/v2/me/jobs/2/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fed69132339d1f2a95dd7dec653125027f35f3040fe5c5d8080c432a2305ba58"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 859d8a6bc189a202233eb4b31b4173f1c4c6be808be7078e5ceba26ffb4c9867
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
	-H "Authorization: Bearer 859d8a6bc189a202233eb4b31b4173f1c4c6be808be7078e5ceba26ffb4c9867"
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
{"password":{"reset_password_token":"nD4UhQxxxfxnfCnKqr4x","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 759,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-26T18:01:23.643Z",
  "updated_at": "2016-10-26T18:01:23.774Z",
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
  "audit_id": 4635
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"nD4UhQxxxfxnfCnKqr4x","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/59/comments
Content-Type: application/json
Authorization: Bearer a3f052fa46f73adb0083b4e58e0faabea61e431c5e4c04985ed1298f9840b4df
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
    "id": 11,
    "author_id": 286,
    "reply_to_id": null,
    "created_at": "2016-10-26T18:00:40.866Z",
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
curl "api.goskive.com/v2/questions/59/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3f052fa46f73adb0083b4e58e0faabea61e431c5e4c04985ed1298f9840b4df"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/57/comments
Content-Type: application/json
Authorization: Bearer 5c6bb512dda9259c92ceceeb7a6c92016a10a54cba57df9ef0ecd8122d759d1c
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
    "id": 10,
    "author_id": 280,
    "reply_to_id": null,
    "created_at": "2016-10-26T18:00:40.014Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 10,
      "user_id": 280,
      "feedbackable_id": 57,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:40.011Z",
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
curl "api.goskive.com/v2/questions/57/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c6bb512dda9259c92ceceeb7a6c92016a10a54cba57df9ef0ecd8122d759d1c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/60/comments
Content-Type: application/json
Authorization: Bearer 40c0507146d250285bedb391ffcfa872c974735dd9931bf56d81cdf8b5cbd05e
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
      "id": 13,
      "author_id": 293,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:00:41.342Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 292,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:00:41.327Z",
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
curl "api.goskive.com/v2/questions/60/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40c0507146d250285bedb391ffcfa872c974735dd9931bf56d81cdf8b5cbd05e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/58/comments
Content-Type: application/json
Authorization: Bearer 08859427c9e0c9774c0c096a672e25a19e8796f3117bca348bbddf940d2038c0
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
curl "api.goskive.com/v2/questions/58/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08859427c9e0c9774c0c096a672e25a19e8796f3117bca348bbddf940d2038c0"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/1/feedbacks
Content-Type: application/json
Authorization: Bearer 14c84ecbfa612423916f167d918b51c1323ade6577950c943a17b75dd2821468
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
    "id": 1,
    "user_id": 1,
    "feedbackable_id": 1,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-26T18:00:12.838Z",
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
curl "api.goskive.com/v2/questions/1/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14c84ecbfa612423916f167d918b51c1323ade6577950c943a17b75dd2821468"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/8/feedbacks
Content-Type: application/json
Authorization: Bearer d5c637c695db0ef84bf9eb3d324a7bba22ad27fe7cf7b4e19bc1c4421aeadb56
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
      "id": 8,
      "user_id": 36,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:15.616Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 35,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:15.606Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/8/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5c637c695db0ef84bf9eb3d324a7bba22ad27fe7cf7b4e19bc1c4421aeadb56"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/75/votes
Content-Type: application/json
Authorization: Bearer 1305988f4c47cbbf65ccae5a264e1522faefa42d3b0eecee780623b2e85fbf3d
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 508
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 507
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 506
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/75/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1305988f4c47cbbf65ccae5a264e1522faefa42d3b0eecee780623b2e85fbf3d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/83/republish
Content-Type: application/json
Authorization: Bearer a48c26bc419ae5d86af14c0800c9d186edc49b3b0dd212699be99b564471a47e
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
curl "api.goskive.com/v2/questions/83/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a48c26bc419ae5d86af14c0800c9d186edc49b3b0dd212699be99b564471a47e"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/88/bookmark
Content-Type: application/json
Authorization: Bearer 314be3f44cf1aae7f6abbab3c7459310472b2ba3dc411df7831f77a6421b05eb
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/88/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 314be3f44cf1aae7f6abbab3c7459310472b2ba3dc411df7831f77a6421b05eb"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/81
Content-Type: application/json
Authorization: Bearer 959b0ebbd59193fe96a7021054c4adb6de6dc66e84bb5a673b96909ad8cb27c5
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/81" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 959b0ebbd59193fe96a7021054c4adb6de6dc66e84bb5a673b96909ad8cb27c5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/82/downvote
Content-Type: application/json
Authorization: Bearer 916ad7bd7493ca36a0152b27c084fa264cbe48ede54fa0c7ab3594afaee552b2
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/82/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 916ad7bd7493ca36a0152b27c084fa264cbe48ede54fa0c7ab3594afaee552b2"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/87
Content-Type: application/json
Authorization: Bearer ffd90fe2ca8683106c5ef02a830f7e4391be300714574fdf5b30e65876e30f6b
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
    "id": 87,
    "obfuscated_id": "Jisk1d9Nmeo",
    "author_id": 579,
    "chapter_id": 137,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:01:09.439Z",
    "created_at": "2016-10-26T18:01:09.263Z",
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
        "id": 177,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 178,
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
curl "api.goskive.com/v2/questions/87" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffd90fe2ca8683106c5ef02a830f7e4391be300714574fdf5b30e65876e30f6b"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/104/report
Content-Type: application/json
Authorization: Bearer f868f1eacd91a938129442995f2437f7bd8160157a9431027958010325628109
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/104/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f868f1eacd91a938129442995f2437f7bd8160157a9431027958010325628109"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/86/bookmark
Content-Type: application/json
Authorization: Bearer 109d6690e753847520cb4d3ef9eadbf40c0e4a3b3af6c098cb9c79fd3f7c32cf
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/86/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 109d6690e753847520cb4d3ef9eadbf40c0e4a3b3af6c098cb9c79fd3f7c32cf"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/85
Content-Type: application/json
Authorization: Bearer 3eb2ac1d442a48d50bfd90dbcae2f98ecc521f815685c7fc5894500308716b4a
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":85,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T18:01:08.160Z","updated_at":"2016-10-26T18:01:08.343Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":135,"author_id":573,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 85,
    "obfuscated_id": "xR5KgQjIo2Y",
    "author_id": 573,
    "chapter_id": 135,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T18:01:08.480Z",
    "created_at": "2016-10-26T18:01:08.160Z",
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
    "question": "{\"id\"=>85, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-26T18:01:08.160Z\", \"updated_at\"=>\"2016-10-26T18:01:08.343Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>135, \"author_id\"=>573, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 172,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 173,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 174,
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
curl "api.goskive.com/v2/questions/85" -d '{"question":{"question":{"id":85,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T18:01:08.160Z","updated_at":"2016-10-26T18:01:08.343Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":135,"author_id":573,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eb2ac1d442a48d50bfd90dbcae2f98ecc521f815685c7fc5894500308716b4a"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/105/upvote
Content-Type: application/json
Authorization: Bearer 68ee4a7efc60cbaa69c433867e26047df280ed654a57e30eea33dbd354181e69
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/105/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68ee4a7efc60cbaa69c433867e26047df280ed654a57e30eea33dbd354181e69"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 96d144f195e4aa636170ec87f3a0599454c449b099ce03a85ed6db606d81c394
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
      "creator_id": 457,
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "topic_id": 139,
      "discipline_id": 140,
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
      "updated_at": "2016-10-26T18:00:54.536Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96d144f195e4aa636170ec87f3a0599454c449b099ce03a85ed6db606d81c394"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 019adaa70bd3c185ca8fe173824940395be335ad7cb35edf39aabb3fe27be62e
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
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-128",
      "html_url": "https://goskive.com/university/uni-128",
      "slug": "uni-128",
      "name": "National School of Pizza",
      "short_name": "Uni 128",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2fc53ff5dd17139d68d0f07faced6ccc60096152.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/14beb69efa7713df2f56ef4d075848f934fe5299.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T18:00:54.377Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-127",
      "html_url": "https://goskive.com/university/uni-127",
      "slug": "uni-127",
      "name": "National School of Pastry",
      "short_name": "Uni 127",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e3ac9cd6bd67f880eec47bf6c7bd8d5c10ed6681.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2c3e8cc18d0b835e41aca1ef6a29a320b6151998.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T18:00:54.359Z",
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
	-H "Authorization: Bearer 019adaa70bd3c185ca8fe173824940395be335ad7cb35edf39aabb3fe27be62e"
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
      "id": 29,
      "name": "Expanded directional neural-net",
      "name_translations": {
        "en": "Expanded directional neural-net"
      },
      "discipline_id": 29
    },
    {
      "id": 30,
      "name": "Programmable system-worthy budgetary management",
      "name_translations": {
        "en": "Programmable system-worthy budgetary management"
      },
      "discipline_id": 30
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
GET /v2/topics/28
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
    "id": 28,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 28
  }
}
```



```shell
curl "api.goskive.com/v2/topics/28" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer f67851a517fa7aad3d543eccbef6f5b6489035606d4a825f229f0cc1e2905fff
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
      "id": 192,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-174",
      "html_url": "https://goskive.com/university/uni-174",
      "slug": "uni-174",
      "name": "University 124",
      "short_name": "Uni 174",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ec8fc83a6db082332f7c054e0db48f0526e7118a.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/83ef4b7164f93da29a9163bb936ede009b0ec181.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T18:01:16.355Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 193,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-175",
      "html_url": "https://goskive.com/university/uni-175",
      "slug": "uni-175",
      "name": "University 125",
      "short_name": "Uni 175",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5fccb91f8fe42569038ac629ad51c2b3161b592e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/604df543ce889eaaae810f264f088529d4c723c8.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T18:01:16.370Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-176",
      "html_url": "https://goskive.com/university/uni-176",
      "slug": "uni-176",
      "name": "University 126",
      "short_name": "Uni 176",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/32c91fa611326a3b9923ec963c6b2fde98a8444b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e8978e5d741013335f26737cbe8c5ea669c728ea.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T18:01:16.387Z",
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
	-H "Authorization: Bearer f67851a517fa7aad3d543eccbef6f5b6489035606d4a825f229f0cc1e2905fff"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 29c0a134c95261cf8497fba6ff868bbf5634be6399693672d9a048ff375cf677
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
    "id": 196,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/691708776e2a02229b737f1b2a92b7e25e6e7c3c.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a9f145362449dba2911e7ea22ea755d720905381.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-26T18:01:16.557Z",
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
	-H "Authorization: Bearer 29c0a134c95261cf8497fba6ff868bbf5634be6399693672d9a048ff375cf677"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 783237cd1abf484395abe289f6bf7d0ff84c7e81f21eb0de6c69f9863a580f34
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":195,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 555,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "topic_id": 195,
    "discipline_id": 196,
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
    "chapters_updated_at": "2016-10-26T18:01:05.411Z",
    "updated_at": "2016-10-26T18:01:05.557Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 127,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-26T18:01:05.501Z",
        "course_id": 183,
        "author_id": 555,
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
        "id": 128,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-26T18:01:05.523Z",
        "course_id": 183,
        "author_id": 555,
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
        "id": 129,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-26T18:01:05.544Z",
        "course_id": 183,
        "author_id": 555,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":195,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 783237cd1abf484395abe289f6bf7d0ff84c7e81f21eb0de6c69f9863a580f34"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 640d37a98c7a9f5c6985793d86d8d3b28f5b25702c540937031450dc00b91991
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":194,"published":false}}
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
    "creator_id": 554,
    "id": 182,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 162,
    "additional_university_ids": [

    ],
    "topic_id": 194,
    "discipline_id": 195,
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
    "updated_at": "2016-10-26T18:01:05.371Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":194,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 640d37a98c7a9f5c6985793d86d8d3b28f5b25702c540937031450dc00b91991"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ccf52fc8544b58c7499418895fc92e0bd43c69e5ddb1a245829581d91e08e660
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
      "creator_id": 534,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 115",
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
      "updated_at": "2016-10-26T18:01:03.296Z",
      "shortname": "fu-course-115"
    },
    {
      "creator_id": 534,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-116",
      "html_url": "https://goskive.com/course/fu-course-116",
      "slug": "fu-course-116",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 116",
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
      "chapters_updated_at": "2016-10-26T18:01:03.673Z",
      "updated_at": "2016-10-26T18:01:03.683Z",
      "shortname": "fu-course-116"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccf52fc8544b58c7499418895fc92e0bd43c69e5ddb1a245829581d91e08e660"
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
      "creator_id": 544,
      "id": 172,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "topic_id": 184,
      "discipline_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "updated_at": "2016-10-26T18:01:04.262Z",
      "shortname": "fu-course-123"
    },
    {
      "creator_id": 544,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-124",
      "html_url": "https://goskive.com/course/fu-course-124",
      "slug": "fu-course-124",
      "university_id": 157,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 124",
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
      "chapters_updated_at": "2016-10-26T18:01:04.652Z",
      "updated_at": "2016-10-26T18:01:04.663Z",
      "shortname": "fu-course-124"
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
Authorization: Bearer 4493db8d212675bc4435930244568bef6b2378adfe4e2eb86a8e692e8002a59e
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
      "creator_id": 540,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
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
      "updated_at": "2016-10-26T18:01:03.913Z",
      "shortname": "fu-course-119"
    },
    {
      "creator_id": 540,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 120",
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
      "updated_at": "2016-10-26T18:01:03.954Z",
      "shortname": "fu-course-120"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4493db8d212675bc4435930244568bef6b2378adfe4e2eb86a8e692e8002a59e"
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
      "creator_id": 549,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 188,
      "discipline_id": 189,
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
      "updated_at": "2016-10-26T18:01:04.883Z",
      "shortname": "fu-course-127"
    },
    {
      "creator_id": 549,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 159,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
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
      "updated_at": "2016-10-26T18:01:04.926Z",
      "shortname": "fu-course-128"
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
Authorization: Bearer 10f8376a0f22491fdc13e793b9c9590827e4b6ed9dae2ee2b7748f98385e41e9
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
  "id": 512,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-26T18:01:01.042Z",
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
	-H "Authorization: Bearer 10f8376a0f22491fdc13e793b9c9590827e4b6ed9dae2ee2b7748f98385e41e9"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/272
Content-Type: application/json
Authorization: Bearer e9ea01884b530efc3a0f1d25117256a4998bba9f62fdfb72c6e455399e7d9b79
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
    "id": 272,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 74,
    "fields_of_study": [
      79,
      80
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-26T18:00:38.917Z",
    "updated_at": "2016-10-26T18:00:38.917Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/272" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9ea01884b530efc3a0f1d25117256a4998bba9f62fdfb72c6e455399e7d9b79"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/270
Content-Type: application/json
Authorization: Bearer 8e006c719258534720183cab1ba9af9a30afcba123217cdb43fb4ae476a49e5b
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
    "id": 270,
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
    "created_at": "2016-10-26T18:00:38.749Z",
    "updated_at": "2016-10-26T18:00:38.749Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/270" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e006c719258534720183cab1ba9af9a30afcba123217cdb43fb4ae476a49e5b"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/4
Content-Type: application/json
Authorization: Bearer a996f22efc96eb8188f11923991882e17ccbe767183cd2b7a0569390e6fb2d40
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a996f22efc96eb8188f11923991882e17ccbe767183cd2b7a0569390e6fb2d40"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/5
Content-Type: application/json
Authorization: Bearer fd1b2f05198da2d448bf244af4f0c758912d4834a80456ce53817f808cb6e1d2
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
    "id": 5,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 49,
    "user_id": 165
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd1b2f05198da2d448bf244af4f0c758912d4834a80456ce53817f808cb6e1d2"
```
