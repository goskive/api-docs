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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"858f735a0f14179be4e888e73e0e28508b2b36000d2785881d808792b38aa803","client_secret":"a1b0fe83fac618fcdccc47736ee699fe501b8a1cd83bb5829c8f161581749a43"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"858f735a0f14179be4e888e73e0e28508b2b36000d2785881d808792b38aa803","client_secret":"a1b0fe83fac618fcdccc47736ee699fe501b8a1cd83bb5829c8f161581749a43"}' -X POST \
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
Authorization: Basic NDdiZTdlYjg0NTdmYTdjNGY4YWE5YjI2MTIwOTA5YzAxZTE1YTFlMGE5MmE2
M2QyMGI1MDUxMWY1YmI4OWQ4OTozZWRhOTAyNzAzOGNiYWQyM2ZkODMzYTk2
YjA2YjZiZjg1OTllM2RjNTFmMzBmYTk3YjlmZGM3MGYwMTU4NzQw

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
	-u 47be7eb8457fa7c4f8aa9b26120909c01e15a1e0a92a63d20b50511f5bb89d89:3eda9027038cbad23fd833a96b06b6bf8599e3dc51f30fa97b9fdc70f0158740
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
{"grant_type":"client_credentials","client_id":"275e6dbc17a16bf8f63c1fd97d206bd7c9fa0e959abdc5ae616e1bcc38a518c6","client_secret":"add89f04249569f75dcbb85a615accdc82c22562a2ac8a069134cf2d3e68011b"}
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
  "access_token": "704ae55be1ab6628529e17e17ee7b4c33ba2f988c47a8119c6266b27981dc176",
  "token_type": "bearer",
  "created_at": 1477588495
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"275e6dbc17a16bf8f63c1fd97d206bd7c9fa0e959abdc5ae616e1bcc38a518c6","client_secret":"add89f04249569f75dcbb85a615accdc82c22562a2ac8a069134cf2d3e68011b"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"6542e13edc2aedb6f1c0f76b87ef6d2dc282f8dd8d4b63f96e894d33a2433d87","client_secret":"725f04623f6ddba2f0228e5614d3ec1dba97b9286395fbe36f890e6c678f53d3"}
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
  "access_token": "5d9bb89c844a657ef71d942b7844122b67cdc1578f650d0d3a7593bf2fc61b11",
  "token_type": "bearer",
  "created_at": 1477588495
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"6542e13edc2aedb6f1c0f76b87ef6d2dc282f8dd8d4b63f96e894d33a2433d87","client_secret":"725f04623f6ddba2f0228e5614d3ec1dba97b9286395fbe36f890e6c678f53d3"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MTlhMGU5NTEwZDZhY2YzZjMyNGUwNmQ2OGYwYmUwYTA0M2E4ODA1MjZmNWU4
MTNhMzhlY2E1NDViZmY2M2E1NDozMTEwMTA1NGQzYWE5NWJhNjQ3YjgwNjE0
YjI0ZGQxYmE5Y2M5NjU5YmEwZTM0ZDQ1YThjZTUxOTRkNGE0ZTAz

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
  "access_token": "9f96fe7171763c1c6b721bf0e78df880e4bf4c572fc898f07aa9bf9b9bc2164a",
  "token_type": "bearer",
  "created_at": 1477588495
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 19a0e9510d6acf3f324e06d68f0be0a043a880526f5e813a38eca545bff63a54:31101054d3aa95ba647b80614b24dd1ba9cc9659ba0e34d45a8ce5194d4a4e03
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
Authorization: Bearer 37154c0bd196699ec717c8328aa742205688244bc6a54e5a98d8b03d632cde1d
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
    "company_id": 5,
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
	-H "Authorization: Bearer 37154c0bd196699ec717c8328aa742205688244bc6a54e5a98d8b03d632cde1d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/131/flashcards
Content-Type: application/json
Authorization: Bearer a71abdac1b8e120e53ca50fd12b529f7cd16268aba4665395ac360d92d3c0984
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":131,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 48,
    "obfuscated_id": "oqXJ8Hi_AE4",
    "author_id": 513,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:15:33.869Z",
    "created_at": "2016-10-27T17:15:33.869Z",
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
curl "api.goskive.com/v2/chapters/131/flashcards" -d '{"flashcard":{"chapter_id":131,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a71abdac1b8e120e53ca50fd12b529f7cd16268aba4665395ac360d92d3c0984"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/132/flashcards
Content-Type: application/json
Authorization: Bearer db5b0e9b3a4b641af445188613c4623f297287378bddd34393923b7db546a4de
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 514,
      "chapter_id": 132,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:34.017Z",
      "created_at": "2016-10-27T17:15:34.017Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 514,
      "chapter_id": 132,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:34.057Z",
      "created_at": "2016-10-27T17:15:34.057Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 514,
      "chapter_id": 132,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:34.096Z",
      "created_at": "2016-10-27T17:15:34.096Z",
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
curl "api.goskive.com/v2/chapters/132/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db5b0e9b3a4b641af445188613c4623f297287378bddd34393923b7db546a4de"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/6/questions
Content-Type: application/json
Authorization: Bearer 34b67f4c83802442aa659ee362dfb86d4f55cf81c0702006aa9a9ecab8daa5d1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 7,
    "obfuscated_id": "XFkue8saGAM",
    "author_id": 21,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:14:54.906Z",
    "created_at": "2016-10-27T17:14:54.906Z",
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
        "id": 14,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 15,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 16,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 17,
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
curl "api.goskive.com/v2/chapters/6/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34b67f4c83802442aa659ee362dfb86d4f55cf81c0702006aa9a9ecab8daa5d1"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer 385aceaeffde1f90856b91939cb6b2d23aad8eade0dce3716c2fe5ef41072a4a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 12,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:14:53.852Z",
    "created_at": "2016-10-27T17:14:53.852Z",
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
        "id": 7,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 8,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/3/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 385aceaeffde1f90856b91939cb6b2d23aad8eade0dce3716c2fe5ef41072a4a"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 05e63a707ed015256213948dc5b99eb5d764b2b887386dc0e6125bf6beb77bb5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 15,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:14:54.186Z",
    "created_at": "2016-10-27T17:14:54.186Z",
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
        "id": 9,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 10,
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
curl "api.goskive.com/v2/chapters/4/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05e63a707ed015256213948dc5b99eb5d764b2b887386dc0e6125bf6beb77bb5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer 18201b31979489d7f37e919c655d52cfec63ea6b2942d05dd0c0162361b4a921
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":5,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 6,
    "obfuscated_id": "eyxYPTvoIb8",
    "author_id": 18,
    "chapter_id": 5,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:14:54.506Z",
    "created_at": "2016-10-27T17:14:54.506Z",
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
        "id": 11,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 12,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 13,
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
curl "api.goskive.com/v2/chapters/5/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":5,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18201b31979489d7f37e919c655d52cfec63ea6b2942d05dd0c0162361b4a921"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/2/questions
Content-Type: application/json
Authorization: Bearer 6954020a13858d480664cb28d541f07dc836b3b848e8d48832295a6c564f41de
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
      "id": 1,
      "obfuscated_id": "vnOJWgI0jGc",
      "author_id": 6,
      "chapter_id": 2,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:14:53.226Z",
      "created_at": "2016-10-27T17:14:53.105Z",
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
          "id": 1,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 2,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 7,
      "chapter_id": 2,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:14:53.409Z",
      "created_at": "2016-10-27T17:14:53.296Z",
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
          "id": 3,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 4,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 8,
      "chapter_id": 2,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:14:53.593Z",
      "created_at": "2016-10-27T17:14:53.477Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6954020a13858d480664cb28d541f07dc836b3b848e8d48832295a6c564f41de"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/80
Content-Type: application/json
Authorization: Bearer ba14c435e4a0d5bf79a9713eb3d4cf7649874e471805874cbc1da41ae8b581c7
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
curl "api.goskive.com/v2/chapters/80" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba14c435e4a0d5bf79a9713eb3d4cf7649874e471805874cbc1da41ae8b581c7"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/82
Content-Type: application/json
Authorization: Bearer 1c5598783f9c2440f0af5291c1163ab8049eb362809af4675586d54599a51a44
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
curl "api.goskive.com/v2/chapters/82" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c5598783f9c2440f0af5291c1163ab8049eb362809af4675586d54599a51a44"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/75
Content-Type: application/json
Authorization: Bearer 6ef692926d66fdb68d5232ac5f32bc6976ac6f8a3b72016faa3ea57a87c4b444
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
curl "api.goskive.com/v2/chapters/75" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ef692926d66fdb68d5232ac5f32bc6976ac6f8a3b72016faa3ea57a87c4b444"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/81
Content-Type: application/json
Authorization: Bearer c483009e572ac6d69e7e392fa06cc13f5b103f8ce5c8cfd8bf84c0db5d7fb8bc
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/81" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c483009e572ac6d69e7e392fa06cc13f5b103f8ce5c8cfd8bf84c0db5d7fb8bc"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/79
Content-Type: application/json
Authorization: Bearer c7bd55f80dd24b79e12596de37e55cd6b2cedf59a63bf8324824de194282b49b
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
    "id": 79,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-27T17:15:18.868Z",
    "course_id": 84,
    "author_id": 310,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-27T17:15:18.294Z",
    "questions_updated_at": "2016-10-27T17:15:18.294Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 314,
        "chapter_id": 79,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:18.848Z",
        "created_at": "2016-10-27T17:15:18.848Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 312,
        "chapter_id": 79,
        "position": 39,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:18.732Z",
        "created_at": "2016-10-27T17:15:18.601Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/79" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7bd55f80dd24b79e12596de37e55cd6b2cedf59a63bf8324824de194282b49b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/76
Content-Type: application/json
Authorization: Bearer eedc862d8b54f6340b1e68c273279ac910185af75d87d6b1dd21688fe26017c2
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
    "id": 76,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-27T17:15:17.449Z",
    "course_id": 81,
    "author_id": 298,
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
curl "api.goskive.com/v2/chapters/76" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eedc862d8b54f6340b1e68c273279ac910185af75d87d6b1dd21688fe26017c2"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer e28ace256bbad33179a9a801846b8e0cf85dacb63fae167b630e90246a95cd8e
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
    "author_id": 40,
    "reply_to_id": 2,
    "created_at": "2016-10-27T17:14:56.354Z",
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
	-H "Authorization: Bearer e28ace256bbad33179a9a801846b8e0cf85dacb63fae167b630e90246a95cd8e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 934d6cce5a49c55e2c69baf958f12baf90de480a9ed1bc38653df4d42d19e668
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
	-H "Authorization: Bearer 934d6cce5a49c55e2c69baf958f12baf90de480a9ed1bc38653df4d42d19e668"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/21
Content-Type: application/json
Authorization: Bearer 05e9698d4579c2d2254f3cb5233615e39858cb657615fac8d9d2847e30ded93d
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
curl "api.goskive.com/v2/comments/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05e9698d4579c2d2254f3cb5233615e39858cb657615fac8d9d2847e30ded93d"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/24/republish
Content-Type: application/json
Authorization: Bearer 5dd601c78314c4c890cfb9a38687a03d95db12623fc8e12763e9f057ad18f209
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
curl "api.goskive.com/v2/comments/24/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5dd601c78314c4c890cfb9a38687a03d95db12623fc8e12763e9f057ad18f209"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer ad9788ef5a78b0731b9d6aa240f4f33734ddd932690268136e59802d95440ba0
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad9788ef5a78b0731b9d6aa240f4f33734ddd932690268136e59802d95440ba0"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer ab0d0975a6d935894ec97d50abee33c6ec3d8d25b56f9bacb5c9ee7608c814b1
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
	-H "Authorization: Bearer ab0d0975a6d935894ec97d50abee33c6ec3d8d25b56f9bacb5c9ee7608c814b1"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/1
Content-Type: application/json
Authorization: Bearer 261da490a4275322a3bc9b8de8da8e405da383921feb8c61f5485f0916f9c49b
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
    "updated_at": "2016-10-27T17:14:55.475Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 261da490a4275322a3bc9b8de8da8e405da383921feb8c61f5485f0916f9c49b"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 9f6ac58255eaade532d776bf51dfab4d0633241f0121e2501e2fbd226e905881
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
      "updated_at": "2016-10-27T17:14:55.592Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-27T17:14:55.596Z"
    },
    {
      "id": 4,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-27T17:14:55.599Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f6ac58255eaade532d776bf51dfab4d0633241f0121e2501e2fbd226e905881"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/7/company_profiles
Content-Type: application/json
Authorization: Bearer 3c315691d4d6a66a0a59dbb66ec79aabf79f8cc30af9d37c5a9abb27db7e7a01
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
curl "api.goskive.com/v2/companies/7/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c315691d4d6a66a0a59dbb66ec79aabf79f8cc30af9d37c5a9abb27db7e7a01"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/6/company_profiles
Content-Type: application/json
Authorization: Bearer cc571f6c7ddd103306540d725f2e5f374dc9ec90db24c79d8cf1dd7af4e77a95
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
curl "api.goskive.com/v2/companies/6/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc571f6c7ddd103306540d725f2e5f374dc9ec90db24c79d8cf1dd7af4e77a95"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 991488f7b27805482fc0343aecbb4439f04fd59180fec0cf343e1baca572f828
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
	-H "Authorization: Bearer 991488f7b27805482fc0343aecbb4439f04fd59180fec0cf343e1baca572f828"
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
Authorization: Bearer a98b3c9281d413da6740310f3bafb8716dc6efced0cef587ebfcd712a23f972d
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
	-H "Authorization: Bearer a98b3c9281d413da6740310f3bafb8716dc6efced0cef587ebfcd712a23f972d"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 64e5bc28af597466c79fd4468402f488061fc7ecc50f68c5162673c3ea24c120
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
    "id": 92,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-27T17:15:23.702Z",
    "course_id": 103,
    "author_id": 370,
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
	-H "Authorization: Bearer 64e5bc28af597466c79fd4468402f488061fc7ecc50f68c5162673c3ea24c120"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 446ecfc2b0a8642014240dface50e54fec8639eeff62549348bf4c72dd318128
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
      "id": 97,
      "title": "Clever Chapter Title 79",
      "position": 1,
      "updated_at": "2016-10-27T17:15:24.361Z",
      "course_id": 108,
      "author_id": 383,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 98,
      "title": "Clever Chapter Title 80",
      "position": 2,
      "updated_at": "2016-10-27T17:15:24.384Z",
      "course_id": 108,
      "author_id": 384,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 99,
      "title": "Clever Chapter Title 81",
      "position": 3,
      "updated_at": "2016-10-27T17:15:24.647Z",
      "course_id": 108,
      "author_id": 385,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-27T17:15:24.266Z",
      "questions_updated_at": "2016-10-27T17:15:24.266Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 446ecfc2b0a8642014240dface50e54fec8639eeff62549348bf4c72dd318128"
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
      "id": 109,
      "title": "Clever Chapter Title 91",
      "position": 1,
      "updated_at": "2016-10-27T17:15:25.955Z",
      "course_id": 114,
      "author_id": 411,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 110,
      "title": "Clever Chapter Title 92",
      "position": 2,
      "updated_at": "2016-10-27T17:15:25.981Z",
      "course_id": 114,
      "author_id": 412,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 111,
      "title": "Clever Chapter Title 93",
      "position": 3,
      "updated_at": "2016-10-27T17:15:26.258Z",
      "course_id": 114,
      "author_id": 413,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-27T17:15:25.882Z",
      "questions_updated_at": "2016-10-27T17:15:25.882Z",
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
Authorization: Bearer d88ac7e5cdc77666c1d04f4d0b23c49d7406d057d75d16b2db9d1cb430b85b4b
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
      "id": 100,
      "title": "Clever Chapter Title 82",
      "position": 1,
      "updated_at": "2016-10-27T17:15:24.794Z",
      "course_id": 109,
      "author_id": 390,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 101,
      "title": "Clever Chapter Title 83",
      "position": 2,
      "updated_at": "2016-10-27T17:15:24.819Z",
      "course_id": 109,
      "author_id": 391,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 102,
      "title": "Clever Chapter Title 84",
      "position": 3,
      "updated_at": "2016-10-27T17:15:24.844Z",
      "course_id": 109,
      "author_id": 392,
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
	-H "Authorization: Bearer d88ac7e5cdc77666c1d04f4d0b23c49d7406d057d75d16b2db9d1cb430b85b4b"
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
      "id": 112,
      "title": "Clever Chapter Title 94",
      "position": 1,
      "updated_at": "2016-10-27T17:15:26.385Z",
      "course_id": 115,
      "author_id": 417,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 113,
      "title": "Clever Chapter Title 95",
      "position": 2,
      "updated_at": "2016-10-27T17:15:26.412Z",
      "course_id": 115,
      "author_id": 418,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 114,
      "title": "Clever Chapter Title 96",
      "position": 3,
      "updated_at": "2016-10-27T17:15:26.439Z",
      "course_id": 115,
      "author_id": 419,
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
Authorization: Bearer 3867479c6ffb0e9a1fbf678110ad0e83331ecb80d3d3d02a7079d598bd223778
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
    "course_id": 230,
    "user_id": 754,
    "updated_at": "2016-10-27T17:15:57.529Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3867479c6ffb0e9a1fbf678110ad0e83331ecb80d3d3d02a7079d598bd223778"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer cf7ac0781be19365036622669d4abff86b58c21e6f485c5ad57fe8e5e1094950
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
      "course_id": 232,
      "user_id": 758,
      "updated_at": "2016-10-27T17:15:57.731Z"
    },
    {
      "id": 4,
      "course_id": 232,
      "user_id": 759,
      "updated_at": "2016-10-27T17:15:57.746Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf7ac0781be19365036622669d4abff86b58c21e6f485c5ad57fe8e5e1094950"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/253/files
Content-Type: application/json
Authorization: Bearer f0349b0299558aa479ff41432e9897652f29d2d29c75f7713f9b9c100ab27553
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
      "id": 7,
      "uploader": {
        "id": 830,
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
        "created_at": "2016-10-27T17:16:05.652Z",
        "updated_at": "2016-10-27T17:16:05.652Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:16:05.662Z",
      "updated_at": "2016-10-27T17:16:05.662Z",
      "course_id": 253,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 8,
      "uploader": {
        "id": 831,
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
        "created_at": "2016-10-27T17:16:05.670Z",
        "updated_at": "2016-10-27T17:16:05.670Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:16:05.680Z",
      "updated_at": "2016-10-27T17:16:05.680Z",
      "course_id": 253,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 832,
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
        "created_at": "2016-10-27T17:16:05.688Z",
        "updated_at": "2016-10-27T17:16:05.688Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:16:05.698Z",
      "updated_at": "2016-10-27T17:16:05.698Z",
      "course_id": 253,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/253/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0349b0299558aa479ff41432e9897652f29d2d29c75f7713f9b9c100ab27553"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/252/files
Content-Type: application/json
Authorization: Bearer d797494372f219979ea3ccdf6c7a9c8fed8aba12923734403a5befa10a29163c
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
    "id": 6,
    "uploader": {
      "id": 828,
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
      "created_at": "2016-10-27T17:16:05.431Z",
      "updated_at": "2016-10-27T17:16:05.431Z"
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
    "created_at": "2016-10-27T17:16:05.478Z",
    "updated_at": "2016-10-27T17:16:05.478Z",
    "course_id": 252,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/252/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d797494372f219979ea3ccdf6c7a9c8fed8aba12923734403a5befa10a29163c"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/251/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 2b90d772da7dac4068554673ccd1d63c80801ef2884b8e4e0e32ccd4d8123d69
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
    "key": "cache/e2df19932b4db386bda5f95522ad59ff.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yN1QxODoxNjowNVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2UyZGYxOTkzMmI0ZGIzODZiZGE1Zjk1NTIyYWQ1OWZmLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjcvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI3VDE3MTYwNVoifV19",
    "x-amz-credential": "FAKE/20161027/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161027T171605Z",
    "x-amz-signature": "003c4256eaf30884b97d03f9c42b7243a2f3678743b52d4c54cea173f88ea50a"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/251/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b90d772da7dac4068554673ccd1d63c80801ef2884b8e4e0e32ccd4d8123d69"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 0c9268e29d42a92a1e4f7bc7dc5d5bdab3159a52c8d042c3f9b5a70ff125d758
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
	-H "Authorization: Bearer 0c9268e29d42a92a1e4f7bc7dc5d5bdab3159a52c8d042c3f9b5a70ff125d758"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer fcd17b492c9610ecb58d690e1e8eb6a8ade9085e8570c83c7d2466bc8c167b27
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
	-H "Authorization: Bearer fcd17b492c9610ecb58d690e1e8eb6a8ade9085e8570c83c7d2466bc8c167b27"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 803518a18ff542ef759c8420162d5e8b4c159fd44d4eb09b51e4d79ff3e42225
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
	-H "Authorization: Bearer 803518a18ff542ef759c8420162d5e8b4c159fd44d4eb09b51e4d79ff3e42225"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5c7400ab966668af94c5eb2d40e2cf451db26288aa470592abb27e533f6ff1b9
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
	-H "Authorization: Bearer 5c7400ab966668af94c5eb2d40e2cf451db26288aa470592abb27e533f6ff1b9"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2e51a208fc5b31d631f70007309b4217532de21bdd63905058509ab0dc8819c8
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
	-H "Authorization: Bearer 2e51a208fc5b31d631f70007309b4217532de21bdd63905058509ab0dc8819c8"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer bf9ff47f8006e51c95a4ca8551e97af367bbcfe4015be251045e0e1d67d13d85
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
    "creator_id": 561,
    "id": 181,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "topic_id": 191,
    "discipline_id": 191,
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
    "chapters_updated_at": "2016-10-27T17:15:37.540Z",
    "updated_at": "2016-10-27T17:15:39.117Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 139,
        "title": "Clever Chapter Title 115",
        "position": 1,
        "updated_at": "2016-10-27T17:15:39.069Z",
        "course_id": 181,
        "author_id": 561,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:15:37.540Z",
        "questions_updated_at": "2016-10-27T17:15:37.540Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 140,
        "title": "Clever Chapter Title 116",
        "position": 2,
        "updated_at": "2016-10-27T17:15:39.109Z",
        "course_id": 181,
        "author_id": 561,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:15:37.540Z",
        "questions_updated_at": "2016-10-27T17:15:37.540Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 562,
        "chapter_id": 139,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:38.902Z",
        "created_at": "2016-10-27T17:15:38.902Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 562,
        "chapter_id": 140,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:38.978Z",
        "created_at": "2016-10-27T17:15:38.978Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 562,
        "chapter_id": 139,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:38.945Z",
        "created_at": "2016-10-27T17:15:38.945Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 562,
        "chapter_id": 140,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:39.020Z",
        "created_at": "2016-10-27T17:15:39.020Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 562,
        "chapter_id": 139,
        "position": 56,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:37.774Z",
        "created_at": "2016-10-27T17:15:37.638Z",
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
            "id": 141,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 142,
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
        "author_id": 562,
        "chapter_id": 139,
        "position": 57,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:37.978Z",
        "created_at": "2016-10-27T17:15:37.845Z",
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
        "author_id": 562,
        "chapter_id": 140,
        "position": 58,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:38.205Z",
        "created_at": "2016-10-27T17:15:38.068Z",
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
        "author_id": 562,
        "chapter_id": 140,
        "position": 59,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:38.405Z",
        "created_at": "2016-10-27T17:15:38.277Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf9ff47f8006e51c95a4ca8551e97af367bbcfe4015be251045e0e1d67d13d85"
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
    "creator_id": 567,
    "id": 182,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 166,
    "additional_university_ids": [

    ],
    "topic_id": 192,
    "discipline_id": 192,
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
    "chapters_updated_at": "2016-10-27T17:15:39.230Z",
    "updated_at": "2016-10-27T17:15:40.822Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 141,
        "title": "Clever Chapter Title 117",
        "position": 1,
        "updated_at": "2016-10-27T17:15:40.775Z",
        "course_id": 182,
        "author_id": 567,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:15:39.230Z",
        "questions_updated_at": "2016-10-27T17:15:39.230Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 142,
        "title": "Clever Chapter Title 118",
        "position": 2,
        "updated_at": "2016-10-27T17:15:40.814Z",
        "course_id": 182,
        "author_id": 567,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:15:39.230Z",
        "questions_updated_at": "2016-10-27T17:15:39.230Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 567,
        "chapter_id": 141,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:39.449Z",
        "created_at": "2016-10-27T17:15:39.317Z",
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
            "id": 153,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 154,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 567,
        "chapter_id": 142,
        "position": 64,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:39.899Z",
        "created_at": "2016-10-27T17:15:39.745Z",
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
            "id": 157,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 158,
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
PUT /v2/courses/195/pin
Content-Type: application/json
Authorization: Bearer 2503859553f2af81d17f35a9baebbc29c5cbf330bb4968835adf7fa9d7abbd69
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/195/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2503859553f2af81d17f35a9baebbc29c5cbf330bb4968835adf7fa9d7abbd69"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/194/pin
Content-Type: application/json
Authorization: Bearer a407e972dc0c59ff07b2cfd3300d9a48d315feed967928bdd4c3cf73621e0292
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/194/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a407e972dc0c59ff07b2cfd3300d9a48d315feed967928bdd4c3cf73621e0292"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f6c66dae3ea554b286b829a5c487b6af29f9a3b8f228782ea62f6ee30d4f5247
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
    "creator_id": 560,
    "id": 180,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "topic_id": 190,
    "discipline_id": 190,
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
    "updated_at": "2016-10-27T17:15:37.510Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6c66dae3ea554b286b829a5c487b6af29f9a3b8f228782ea62f6ee30d4f5247"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 3ff707bf18b00a321ef8f0c5f1b3812c566aada9f2d43b118afcdeb6c6caf209
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
    "id": 548,
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
    "created_at": "2016-10-27T17:15:36.309Z",
    "updated_at": "2016-10-27T17:15:36.309Z",
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
	-H "Authorization: Bearer 3ff707bf18b00a321ef8f0c5f1b3812c566aada9f2d43b118afcdeb6c6caf209"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 18f31580ea2e9bf30c166c4c56328bf8090ccff852879d7ad5b930b2a6a965ea
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[183]}
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
    "id": 550,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      183
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:15:36.780Z",
    "updated_at": "2016-10-27T17:15:36.813Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[183]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18f31580ea2e9bf30c166c4c56328bf8090ccff852879d7ad5b930b2a6a965ea"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer afdd8c736116e36b88b672279be81fc38f71d5172c11148acddd1f7ea2a08869
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
    "id": 551,
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
    "created_at": "2016-10-27T17:15:36.834Z",
    "updated_at": "2016-10-27T17:15:36.834Z",
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
	-H "Authorization: Bearer afdd8c736116e36b88b672279be81fc38f71d5172c11148acddd1f7ea2a08869"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b93bf86b17a0aed971b4332e9c2d784e798c69052ee1bc88daccdc331cfc69f9
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[185]}
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
    "id": 552,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      185
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:15:36.926Z",
    "updated_at": "2016-10-27T17:15:36.926Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[185]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b93bf86b17a0aed971b4332e9c2d784e798c69052ee1bc88daccdc331cfc69f9"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer cee784ac79536cfc821d8eecd46e20b57b6a61b54dc8f4cbfc53dfa472bc66f7
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

182
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
    "id": 549,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/0b4e1d499b95c72c072f27e6f62e0eb9256559f0.jpg",
    "university_id": null,
    "fields_of_study": [
      182
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:15:36.404Z",
    "updated_at": "2016-10-27T17:15:36.727Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/d44bc4c1894a4fcc72dce90ddc7dccd4a2829096.jpg",
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

182
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer cee784ac79536cfc821d8eecd46e20b57b6a61b54dc8f4cbfc53dfa472bc66f7"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 7014e251e0bb602ba1cb25e2491b051ac755c2e5fbeadcb4ab70695d6d34dfe9
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
      "id": 4,
      "bookmarkable_id": 56,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 57,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 58,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7014e251e0bb602ba1cb25e2491b051ac755c2e5fbeadcb4ab70695d6d34dfe9"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 628b06d9189c84cf184b64eba6ecfb07f6d46a3fc7369cbb13817fad07de978d
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
	-H "Authorization: Bearer 628b06d9189c84cf184b64eba6ecfb07f6d46a3fc7369cbb13817fad07de978d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8a2dc0d9ed1e5eea78cb0de3038879fc5251491c17c20cadd07411433b1bffde
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
	-H "Authorization: Bearer 8a2dc0d9ed1e5eea78cb0de3038879fc5251491c17c20cadd07411433b1bffde"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 486c51d7723dcd94b815f5d4fd92ac7b35947ec0df2f13ff3c646ed943883bad
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
      "creator_id": 160,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-36",
      "html_url": "https://goskive.com/course/mit-course-36",
      "slug": "mit-course-36",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 44,
      "discipline_id": 44,
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
      "updated_at": "2016-10-27T17:15:04.080Z",
      "shortname": "mit-course-36"
    },
    {
      "creator_id": 161,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-37",
      "html_url": "https://goskive.com/course/mit-course-37",
      "slug": "mit-course-37",
      "university_id": 44,
      "additional_university_ids": [

      ],
      "topic_id": 45,
      "discipline_id": 45,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 37",
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
      "updated_at": "2016-10-27T17:15:04.153Z",
      "shortname": "mit-course-37"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 486c51d7723dcd94b815f5d4fd92ac7b35947ec0df2f13ff3c646ed943883bad"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer dc68eb8856107eb83ef5d7f12393c093ae1d369e22c7555134b5c7183ad72d8d
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
        "created_at": "2016-10-27T17:15:34.393Z",
        "updated_at": "2016-10-27T17:15:34.393Z",
        "file_url": "memory://8ef805abe56beb9b96c86b1d98cc834b.pdf",
        "course_id": 169,
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
        "created_at": "2016-10-27T17:15:34.475Z",
        "updated_at": "2016-10-27T17:15:34.475Z",
        "file_url": "memory://dc2b022aee208706ad11b1d59c8968c0.pdf",
        "course_id": 170,
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
        "created_at": "2016-10-27T17:15:34.553Z",
        "updated_at": "2016-10-27T17:15:34.553Z",
        "file_url": "memory://13b2ee49df18a9cf4f2c089d52cdd68b.pdf",
        "course_id": 171,
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
	-H "Authorization: Bearer dc68eb8856107eb83ef5d7f12393c093ae1d369e22c7555134b5c7183ad72d8d"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 4b72608e8614b9f1fe4ff58ee3b1a860885377d981a44a4c79372abb7990d88d
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
        "updated_at": "2016-10-27T17:15:33.568Z"
      },
      "created_at": "2016-10-27T17:15:33.571Z",
      "updated_at": "2016-10-27T17:15:33.571Z",
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
        "updated_at": "2016-10-27T17:15:33.579Z"
      },
      "created_at": "2016-10-27T17:15:33.582Z",
      "updated_at": "2016-10-27T17:15:33.582Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b72608e8614b9f1fe4ff58ee3b1a860885377d981a44a4c79372abb7990d88d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer b1e0e9ec4e698fe7bd4f997ed2fb205e3ad4fda564a67f9f9e612172bbeec126
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
        "updated_at": "2016-10-27T17:15:33.406Z"
      },
      "created_at": "2016-10-27T17:15:33.409Z",
      "updated_at": "2016-10-27T17:15:33.409Z",
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
        "updated_at": "2016-10-27T17:15:33.423Z"
      },
      "created_at": "2016-10-27T17:15:33.426Z",
      "updated_at": "2016-10-27T17:15:33.426Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1e0e9ec4e698fe7bd4f997ed2fb205e3ad4fda564a67f9f9e612172bbeec126"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer e7593ad59bf5c74f3b9157802e3c52b1703ed7c80cc7ee18ed210e707a288948
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
      "id": 3,
      "created_at": "2016-10-27T17:14:57.650Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 5,
      "updated_at": "2016-10-27T17:14:57.774Z",
      "author_id": "51",
      "thread_subject_id": "10",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 4,
      "created_at": "2016-10-27T17:14:57.762Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-10-27T17:14:57.778Z",
      "author_id": "54",
      "thread_subject_id": "11",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-10-27T17:14:58.189Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-27T17:14:58.189Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-27T17:14:58.613Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-27T17:14:58.613Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 7,
      "created_at": "2016-10-27T17:14:58.997Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-27T17:14:58.997Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 8,
      "created_at": "2016-10-27T17:14:59.304Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 13,
      "updated_at": "2016-10-27T17:14:59.304Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-10-27T17:14:59.589Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 14,
      "updated_at": "2016-10-27T17:14:59.589Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-27T17:14:59.869Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 15,
      "updated_at": "2016-10-27T17:14:59.869Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7593ad59bf5c74f3b9157802e3c52b1703ed7c80cc7ee18ed210e707a288948"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/2
Content-Type: application/json
Authorization: Bearer 86dbb9d51eb1b787ae0472996dabc36f84114a57a8e1a787c5070a3e73f267d7
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-27T17:04:57.000Z"}}
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
    "id": 2,
    "created_at": "2016-10-27T17:14:57.467Z",
    "read_at": "2016-10-27T17:04:57.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 4,
    "updated_at": "2016-10-27T17:14:57.534Z",
    "author_id": "47",
    "thread_subject_id": "9",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/2" -d '{"notification":{"read_at":"2016-10-27T17:04:57.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86dbb9d51eb1b787ae0472996dabc36f84114a57a8e1a787c5070a3e73f267d7"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 87a932ff9a8d48ad2c310cbd549032cfa6a86376ae9034990ba1d950c26f523c
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
      "course_id": 93,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-27T17:15:21.473Z",
      "course_published": true,
      "updated_at": "2016-10-27T17:15:21.464Z"
    },
    {
      "id": 4,
      "course_id": 94,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-27T17:15:21.551Z",
      "course_published": true,
      "updated_at": "2016-10-27T17:15:21.543Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87a932ff9a8d48ad2c310cbd549032cfa6a86376ae9034990ba1d950c26f523c"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 915ed26838c47333197021cd36956d123b5f33327ca9e8ade326aa98eddbabb5
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
    "course_id": 98,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T17:15:22.015Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:15:22.007Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 915ed26838c47333197021cd36956d123b5f33327ca9e8ade326aa98eddbabb5"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer b1f495da0cc4ee92c64de0c32208725e245298f7c78c49cb618d1cad791eb428
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
    "course_id": 97,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-27T17:15:21.920Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:15:21.909Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1f495da0cc4ee92c64de0c32208725e245298f7c78c49cb618d1cad791eb428"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer a1019a283862ef7c7badadc1a7b12b9bcce07063f9bcf5cdff8b1276b19fbda5
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
      "votable_id": 131,
      "user_id": 972
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 132,
      "user_id": 972
    },
    {
      "id": 22,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 972
    },
    {
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 134,
      "user_id": 972
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1019a283862ef7c7badadc1a7b12b9bcce07063f9bcf5cdff8b1276b19fbda5"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/263
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
    "id": 263,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 261,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 263
      },
      {
        "id": 262,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 263
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/263" -X GET \
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
      "id": 261,
      "name": "Customizable heuristic Graphic Interface",
      "name_translations": {
        "en": "Customizable heuristic Graphic Interface"
      }
    },
    {
      "id": 262,
      "name": "Team-oriented asynchronous toolset",
      "name_translations": {
        "en": "Team-oriented asynchronous toolset"
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
PATCH /v2/feedbacks/39/close
Content-Type: application/json
Authorization: Bearer 87c3877587269582668431ca1906432028236b9211a885697a26cdfaf4887562
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
    "id": 39,
    "user_id": 717,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-27T17:15:55.310Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/39/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87c3877587269582668431ca1906432028236b9211a885697a26cdfaf4887562"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/40/fix
Content-Type: application/json
Authorization: Bearer 0a4564574fe35f11d4a367c94653f69789280bff92a74b796e3765932bc6a006
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
    "id": 40,
    "user_id": 722,
    "feedbackable_id": 86,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-27T17:15:55.623Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/40/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a4564574fe35f11d4a367c94653f69789280bff92a74b796e3765932bc6a006"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/44
Content-Type: application/json
Authorization: Bearer e8fcfbef2a4a35735b5d80708df0a2faf75d8e73932c5c019dddf0516a27270b
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
    "id": 44,
    "user_id": 742,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:15:56.885Z",
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
curl "api.goskive.com/v2/feedbacks/44" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8fcfbef2a4a35735b5d80708df0a2faf75d8e73932c5c019dddf0516a27270b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/37/close
Content-Type: application/json
Authorization: Bearer a41c50c81a098d8773cd2cf00d8414065f9db84e7d68b820d0128f28a0f1b8da
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
curl "api.goskive.com/v2/feedbacks/37/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a41c50c81a098d8773cd2cf00d8414065f9db84e7d68b820d0128f28a0f1b8da"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/fix
Content-Type: application/json
Authorization: Bearer 9f85439bf77aeefc8f764ca867fc20edbf80769d1210a5d6c5f660cb5caff82c
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
curl "api.goskive.com/v2/feedbacks/42/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f85439bf77aeefc8f764ca867fc20edbf80769d1210a5d6c5f660cb5caff82c"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 300e44e6df18b5ab7d41cd735b25d6bdcc9afb1752a41b10305489315d87f870
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
	-H "Authorization: Bearer 300e44e6df18b5ab7d41cd735b25d6bdcc9afb1752a41b10305489315d87f870"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/45
Content-Type: application/json
Authorization: Bearer 44baedfea7709c52c8757220a1cc11c7b2ad20293a24994f45daca17061bef9c
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
    "user_id": 747,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:15:57.201Z",
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
curl "api.goskive.com/v2/feedbacks/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44baedfea7709c52c8757220a1cc11c7b2ad20293a24994f45daca17061bef9c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer fb2844b1ed0df5766967415c4efd2f5ab648f15c2ac32acef018df88042f29ed
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
	-H "Authorization: Bearer fb2844b1ed0df5766967415c4efd2f5ab648f15c2ac32acef018df88042f29ed"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/20/bookmark
Content-Type: application/json
Authorization: Bearer be198714ded171fbda6637d9577a1f73f465fbc7d12831e792ce866d7f7f47c3
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be198714ded171fbda6637d9577a1f73f465fbc7d12831e792ce866d7f7f47c3"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 5384b50217b098e607e73e0b29695cddd52e86b10152f4fc3ffce11c2ef30c1c
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
	-H "Authorization: Bearer 5384b50217b098e607e73e0b29695cddd52e86b10152f4fc3ffce11c2ef30c1c"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/15
Content-Type: application/json
Authorization: Bearer 78f9da6aff31a288b957b906cd8bccf9937edbe5d8ea74d0612f73c6e72c64cb
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b8e4c25fb69c030755e6d7c3f9dab1c0.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161027%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161027T171611Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2004f009786ce0faecfadb3382595bf24306df47c49fb125c0880ac5dd276c8a",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78f9da6aff31a288b957b906cd8bccf9937edbe5d8ea74d0612f73c6e72c64cb"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/19/preview
Content-Type: application/json
Authorization: Bearer a86b244c4c47efb03437ba863ebcb6b66c61cd5fd07e21f9d21ea9f22e1296a4
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/914f23f5b55fd3ea4afcbbba488f12d5.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161027%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161027T171612Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=94532334203786118cb8569f76f44d83436fbfa6b2048141798e87cfcaccb5d9",
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
	-H "Authorization: Bearer a86b244c4c47efb03437ba863ebcb6b66c61cd5fd07e21f9d21ea9f22e1296a4"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/16/metadata
Content-Type: application/json
Authorization: Bearer 40401699088b642e7d723888d18d272941a4db797ea9e0516f6d9b294c1bacca
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
    "id": 16,
    "uploader": {
      "id": 955,
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
      "created_at": "2016-10-27T17:16:11.695Z",
      "updated_at": "2016-10-27T17:16:11.695Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-27T17:16:11.774Z",
    "updated_at": "2016-10-27T17:16:11.774Z",
    "course_id": 306,
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
curl "api.goskive.com/v2/files/16/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40401699088b642e7d723888d18d272941a4db797ea9e0516f6d9b294c1bacca"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/4/matched_courses?required_cu_count=2
Authorization: Bearer cc75963be17578ec65e68b592c20c1611ab466cb2ae4f34efddc51ab0f23b91c
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
      "creator_id": 794,
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "topic_id": 252,
      "discipline_id": 252,
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
      "chapters_updated_at": "2016-10-27T17:16:00.194Z",
      "updated_at": "2016-10-27T17:16:01.781Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 799,
      "id": 243,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-9b854f49-8007-42f2-8d78-7757ace22425",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-9b854f49-8007-42f2-8d78-7757ace22425",
      "slug": "mit-the-great-british-bake-off-9b854f49-8007-42f2-8d78-7757ace22425",
      "university_id": 227,
      "additional_university_ids": [

      ],
      "topic_id": 253,
      "discipline_id": 253,
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
      "chapters_updated_at": "2016-10-27T17:16:00.194Z",
      "updated_at": "2016-10-27T17:16:02.342Z",
      "shortname": "mit-the-great-british-bake-off-9b854f49-8007-42f2-8d78-7757ace22425"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/4/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer cc75963be17578ec65e68b592c20c1611ab466cb2ae4f34efddc51ab0f23b91c"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/21/report
Content-Type: application/json
Authorization: Bearer 7b9dd359f7fbe0d01072d7067d2be0afd57923659f7536f055bddd4979b2c452
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b9dd359f7fbe0d01072d7067d2be0afd57923659f7536f055bddd4979b2c452"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/14/bookmark
Content-Type: application/json
Authorization: Bearer 3ae62cfbcfebe973301eb2ec5cbc4cb1196ce13c119b502c81becf4c703fa8ce
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ae62cfbcfebe973301eb2ec5cbc4cb1196ce13c119b502c81becf4c703fa8ce"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/10/upvote
Content-Type: application/json
Authorization: Bearer 1a0b935eea66e53d1f91f77478df060ede161bb59a0d1a66b0aa8bd2569ad101
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a0b935eea66e53d1f91f77478df060ede161bb59a0d1a66b0aa8bd2569ad101"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/53/comments
Content-Type: application/json
Authorization: Bearer eb1a63c9d65b48a5dfe42cdebbbc9395f0538cf3f9e95edd058fe59cbea3a81c
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
    "id": 11,
    "author_id": 534,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:15:35.306Z",
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
curl "api.goskive.com/v2/flashcards/53/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb1a63c9d65b48a5dfe42cdebbbc9395f0538cf3f9e95edd058fe59cbea3a81c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/54/comments
Content-Type: application/json
Authorization: Bearer 413dbe5bae63801a84ec8b4243717f4c059656fd61e157740b87e185acc7a26c
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
    "id": 12,
    "author_id": 537,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:15:35.627Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 17,
      "user_id": 537,
      "feedbackable_id": 54,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:35.623Z",
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
curl "api.goskive.com/v2/flashcards/54/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 413dbe5bae63801a84ec8b4243717f4c059656fd61e157740b87e185acc7a26c"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/56/comments
Content-Type: application/json
Authorization: Bearer 2cf46ab64510a43f78f6856979b2be26a318624990bfa3d818e85b79ad090f8a
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
      "author_id": 546,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:15:36.096Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 547,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:15:36.112Z",
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
curl "api.goskive.com/v2/flashcards/56/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cf46ab64510a43f78f6856979b2be26a318624990bfa3d818e85b79ad090f8a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/52/comments
Content-Type: application/json
Authorization: Bearer e2281f4796def2e886ecf97e9ca77457891089cb00e5ce140f1322c8cfebf934
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
curl "api.goskive.com/v2/flashcards/52/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2281f4796def2e886ecf97e9ca77457891089cb00e5ce140f1322c8cfebf934"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/39/feedbacks
Content-Type: application/json
Authorization: Bearer 48453aebe2860b4363fb30c7a2489f81c488c8c95e520131cc548d46f94fd448
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
    "id": 9,
    "user_id": 469,
    "feedbackable_id": 39,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:15:31.598Z",
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
curl "api.goskive.com/v2/flashcards/39/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48453aebe2860b4363fb30c7a2489f81c488c8c95e520131cc548d46f94fd448"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/45/feedbacks
Content-Type: application/json
Authorization: Bearer cee09cad728c4cdf302f0cb35e6ee02f6ba655bbd0b1de9691daf901a3a84f87
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
      "user_id": 501,
      "feedbackable_id": 45,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:33.015Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 500,
      "feedbackable_id": 45,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:33.004Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/45/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cee09cad728c4cdf302f0cb35e6ee02f6ba655bbd0b1de9691daf901a3a84f87"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer 3da7125c6a40f9654426bebbae0fb8d6e3c8b5963e56db4b0d5deb44b879df00
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
      "votable_id": 27,
      "user_id": 213
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 212
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 211
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3da7125c6a40f9654426bebbae0fb8d6e3c8b5963e56db4b0d5deb44b879df00"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/2/republish
Content-Type: application/json
Authorization: Bearer df6500e7430269b8cac06fa5c58f976fbcb4e4ad4564981faf5bbe3fee81a299
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
curl "api.goskive.com/v2/flashcards/2/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df6500e7430269b8cac06fa5c58f976fbcb4e4ad4564981faf5bbe3fee81a299"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/8/bookmark
Content-Type: application/json
Authorization: Bearer f5fe2d047a09fe0e530258f26edb3bc14db4279a92c3f18007c1ccf04d1a7a1c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/8/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5fe2d047a09fe0e530258f26edb3bc14db4279a92c3f18007c1ccf04d1a7a1c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/4
Content-Type: application/json
Authorization: Bearer d093544f0fee7ef2dc3c121b80fd2b8618bcafb35d44f236716c756eb0b33519
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d093544f0fee7ef2dc3c121b80fd2b8618bcafb35d44f236716c756eb0b33519"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/3/downvote
Content-Type: application/json
Authorization: Bearer 2b3a993505f48a8091666408a6f44c81d485330db693de0e135e505bef9a89ed
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/3/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b3a993505f48a8091666408a6f44c81d485330db693de0e135e505bef9a89ed"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/24
Content-Type: application/json
Authorization: Bearer 27bb80609c5c98336611def80a36c17b66b9fc888d44e8d9e74544226b95482c
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
    "id": 24,
    "obfuscated_id": "KHM5yo_z4Ds",
    "author_id": 152,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:15:03.716Z",
    "created_at": "2016-10-27T17:15:03.716Z",
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
curl "api.goskive.com/v2/flashcards/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27bb80609c5c98336611def80a36c17b66b9fc888d44e8d9e74544226b95482c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/7/report
Content-Type: application/json
Authorization: Bearer 1660ca2e98fcc5ec148697dba16bb9d4c404894ac9095b3c47f368e0d0a2cb9c
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/7/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1660ca2e98fcc5ec148697dba16bb9d4c404894ac9095b3c47f368e0d0a2cb9c"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/5/bookmark
Content-Type: application/json
Authorization: Bearer 2efb94f47acc14f199961f97592b14b122dde95a5eb13471ac5d4d2e12f67350
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/5/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2efb94f47acc14f199961f97592b14b122dde95a5eb13471ac5d4d2e12f67350"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/6/upvote
Content-Type: application/json
Authorization: Bearer 405b81cf5e22f6aed7ffb1c97cc0f747aa739664a762535bccdf9a1539f61b4c
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/6/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 405b81cf5e22f6aed7ffb1c97cc0f747aa739664a762535bccdf9a1539f61b4c"
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
    "key": "cache/f7855b6aefc637e6437c66710e1221d9.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yN1QxODoxNDo1NVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Y3ODU1YjZhZWZjNjM3ZTY0MzdjNjY3MTBlMTIyMWQ5LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjdUMTcxNDU1WiJ9XX0=",
    "x-amz-credential": "FAKE/20161027/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161027T171455Z",
    "x-amz-signature": "e203bb5fdc1d50d7e54c4d7ed65ca13513a3053b8951b6b950980200a41ff2fe"
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
Authorization: Bearer c8e83479e8f3dffc7c47761fd2d2c552ec67479e26ff61448318f5b6a99f8493
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
	-H "Authorization: Bearer c8e83479e8f3dffc7c47761fd2d2c552ec67479e26ff61448318f5b6a99f8493"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer ff65a3a0ed14c0837033a3ffc74761db55f6be9b3bce05007deffc63c22b1daa
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
	-H "Authorization: Bearer ff65a3a0ed14c0837033a3ffc74761db55f6be9b3bce05007deffc63c22b1daa"
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
{"password":{"reset_password_token":"YzusHs5pUx2VZYv_bH7m","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 819,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-27T17:16:03.882Z",
  "updated_at": "2016-10-27T17:16:04.057Z",
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
  "audit_id": 4504
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"YzusHs5pUx2VZYv_bH7m","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/118/comments
Content-Type: application/json
Authorization: Bearer 91eb6e8fb4846f3c914818fc32e5eb362683f05497882f2eb0f2533d500b18e2
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
    "id": 16,
    "author_id": 767,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:15:58.430Z",
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
curl "api.goskive.com/v2/questions/118/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91eb6e8fb4846f3c914818fc32e5eb362683f05497882f2eb0f2533d500b18e2"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/119/comments
Content-Type: application/json
Authorization: Bearer e4bd36fe02139e8e0e7f8f2d6f39ea402d62348be2971b87841b693be5a7fb05
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
    "id": 17,
    "author_id": 770,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:15:58.966Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 770,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:58.962Z",
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
curl "api.goskive.com/v2/questions/119/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4bd36fe02139e8e0e7f8f2d6f39ea402d62348be2971b87841b693be5a7fb05"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/122/comments
Content-Type: application/json
Authorization: Bearer 95c101d7fb3edabbd3bc3d537f21db7abfab81a8c14b411e6b867d59a37a5495
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
      "id": 19,
      "author_id": 783,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:00.152Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 782,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:00.134Z",
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
curl "api.goskive.com/v2/questions/122/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95c101d7fb3edabbd3bc3d537f21db7abfab81a8c14b411e6b867d59a37a5495"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/120/comments
Content-Type: application/json
Authorization: Bearer 47741865e8a252132406ae0c3fbb44c590e197954c2a967c5813d9a8d5e4c0d5
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
curl "api.goskive.com/v2/questions/120/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47741865e8a252132406ae0c3fbb44c590e197954c2a967c5813d9a8d5e4c0d5"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/16/feedbacks
Content-Type: application/json
Authorization: Bearer e48eefb5ec36c2d3558ec27f618ed9698c355bc142e4bc7de7982e28d2ea3ae7
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
    "user_id": 163,
    "feedbackable_id": 16,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:15:04.590Z",
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
curl "api.goskive.com/v2/questions/16/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e48eefb5ec36c2d3558ec27f618ed9698c355bc142e4bc7de7982e28d2ea3ae7"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/18/feedbacks
Content-Type: application/json
Authorization: Bearer 2ced41c7aa6496c6c2eebd54c2a03ae4f29f443d8f52fec6f340f6c425d59274
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
      "id": 4,
      "user_id": 173,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:05.527Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 172,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:05.516Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/18/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ced41c7aa6496c6c2eebd54c2a03ae4f29f443d8f52fec6f340f6c425d59274"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/97/votes
Content-Type: application/json
Authorization: Bearer 3bd8b14367d202688539dd428ccf2a6a2f0007a050b3645c242ea9578f92c76d
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
      "votable_id": 97,
      "user_id": 619
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 618
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 617
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/97/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bd8b14367d202688539dd428ccf2a6a2f0007a050b3645c242ea9578f92c76d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/41/republish
Content-Type: application/json
Authorization: Bearer d266cd92112af8147132f1c0f56b5145c75c789d21a46b26927b0cbb00f529fc
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
curl "api.goskive.com/v2/questions/41/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d266cd92112af8147132f1c0f56b5145c75c789d21a46b26927b0cbb00f529fc"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/46/bookmark
Content-Type: application/json
Authorization: Bearer de9f9da99df57d2ee5bb0eb4bde11a1bdac2d7b70163ea2cac572394a5b2567b
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de9f9da99df57d2ee5bb0eb4bde11a1bdac2d7b70163ea2cac572394a5b2567b"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/48
Content-Type: application/json
Authorization: Bearer 1a6459c539f20e795da70c69d63e2121f4b69a2953556053118d603c7a5465af
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a6459c539f20e795da70c69d63e2121f4b69a2953556053118d603c7a5465af"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/39/downvote
Content-Type: application/json
Authorization: Bearer a7acff3b6bc51c38d23dd4dc4f75bd24b1f7f1763d672c04dc35b95c00db3abf
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/39/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7acff3b6bc51c38d23dd4dc4f75bd24b1f7f1763d672c04dc35b95c00db3abf"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/47
Content-Type: application/json
Authorization: Bearer a36b71c1d35502bd41125d034f9f2a24bad0d1b74d625e57b3cd44c60a37dc9e
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
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 288,
    "chapter_id": 73,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:15:16.527Z",
    "created_at": "2016-10-27T17:15:16.398Z",
    "tags": [
      {
        "id": 16,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 15,
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
        "id": 97,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 98,
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
curl "api.goskive.com/v2/questions/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a36b71c1d35502bd41125d034f9f2a24bad0d1b74d625e57b3cd44c60a37dc9e"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/45/report
Content-Type: application/json
Authorization: Bearer bd0e7f985a5400e2aed56b7881c4c25c2dfee37965743d68dc32d008425a20bb
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd0e7f985a5400e2aed56b7881c4c25c2dfee37965743d68dc32d008425a20bb"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/43/bookmark
Content-Type: application/json
Authorization: Bearer 1cf43368b6770e0dfe827e7defed773f058c7653dc1328dd076017f29af01916
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/43/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cf43368b6770e0dfe827e7defed773f058c7653dc1328dd076017f29af01916"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/40
Content-Type: application/json
Authorization: Bearer 393e77984e4669280ba5c2ae018e62c173124826d3187a186fb8a771c5154a07
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":40,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-27T17:15:13.538Z","updated_at":"2016-10-27T17:15:13.664Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":66,"author_id":267,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 40,
    "obfuscated_id": "lir5nwklJts",
    "author_id": 267,
    "chapter_id": 66,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:15:13.790Z",
    "created_at": "2016-10-27T17:15:13.538Z",
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
    "question": "{\"id\"=>40, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-27T17:15:13.538Z\", \"updated_at\"=>\"2016-10-27T17:15:13.664Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>66, \"author_id\"=>267, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 82,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 83,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 84,
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
curl "api.goskive.com/v2/questions/40" -d '{"question":{"question":{"id":40,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-27T17:15:13.538Z","updated_at":"2016-10-27T17:15:13.664Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":66,"author_id":267,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 393e77984e4669280ba5c2ae018e62c173124826d3187a186fb8a771c5154a07"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/44/upvote
Content-Type: application/json
Authorization: Bearer f04ca3a0b0d5f38c3e658b1590f484bd38ba911af92c4ae944d1c90f84865a30
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/44/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f04ca3a0b0d5f38c3e658b1590f484bd38ba911af92c4ae944d1c90f84865a30"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6acb8c7d48f9801f155e9d9f2f626c685836ab2fcb1ae059853bbc23fe90ae45
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
      "creator_id": 811,
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 230,
      "additional_university_ids": [

      ],
      "topic_id": 257,
      "discipline_id": 257,
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
      "updated_at": "2016-10-27T17:16:02.865Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6acb8c7d48f9801f155e9d9f2f626c685836ab2fcb1ae059853bbc23fe90ae45"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b7c98a18c4fe7ace66721690ed6027b79bf592332b918686237a0a5ed9166219
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
      "id": 233,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-213",
      "html_url": "https://goskive.com/university/uni-213",
      "slug": "uni-213",
      "name": "National School of Pizza",
      "short_name": "Uni 213",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/056624c9b9724e01f88a2e82a8c0d2301c2e1fd3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7fc387c55c3478f4ca1f3d725d2459c24177576c.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:16:03.052Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-212",
      "html_url": "https://goskive.com/university/uni-212",
      "slug": "uni-212",
      "name": "National School of Pastry",
      "short_name": "Uni 212",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e3c25452a8f78367bc32efa4ea977b71615d7273.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7da07f7b8704f71e12bbcbf01452cb69cd6d1972.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:16:03.036Z",
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
	-H "Authorization: Bearer b7c98a18c4fe7ace66721690ed6027b79bf592332b918686237a0a5ed9166219"
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
      "id": 179,
      "name": "Progressive attitude-oriented customer loyalty",
      "name_translations": {
        "en": "Progressive attitude-oriented customer loyalty"
      },
      "discipline_id": 179
    },
    {
      "id": 180,
      "name": "Networked responsive migration",
      "name_translations": {
        "en": "Networked responsive migration"
      },
      "discipline_id": 180
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
GET /v2/topics/181
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
    "id": 181,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 181
  }
}
```



```shell
curl "api.goskive.com/v2/topics/181" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 52004955acc327791b1c19be146eb3e17ed6c5753747bd78300b22ce70051e66
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
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-133",
      "html_url": "https://goskive.com/university/uni-133",
      "slug": "uni-133",
      "name": "University 100",
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
      "updated_at": "2016-10-27T17:15:34.750Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-134",
      "html_url": "https://goskive.com/university/uni-134",
      "slug": "uni-134",
      "name": "University 101",
      "short_name": "Uni 134",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ab1fa002b5157a8d0e8cdf4fb91be789314d3a74.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/006b99b20587e0ba79520101356408798adf17ca.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:15:34.767Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 153,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-135",
      "html_url": "https://goskive.com/university/uni-135",
      "slug": "uni-135",
      "name": "University 102",
      "short_name": "Uni 135",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4520ea235c0ccd922b85aa0607bacc9431645c4d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6af1e644eed83a184febdb26f08a491678a85037.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:15:34.784Z",
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
	-H "Authorization: Bearer 52004955acc327791b1c19be146eb3e17ed6c5753747bd78300b22ce70051e66"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 4e90bfe82f5a0c420b0ab001f8c7cd9c8828aed7d68ed2a6944b2c3b32939dfd
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
    "id": 154,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/82209c04b509cddbfeda6575ab0366139533962d.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a4cde97d8829882baba49a939ea99fc343a352a7.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-27T17:15:34.846Z",
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
	-H "Authorization: Bearer 4e90bfe82f5a0c420b0ab001f8c7cd9c8828aed7d68ed2a6944b2c3b32939dfd"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a20978e2366a86812b5d151a5cbd25000298b626c0e726dbfdf152c073a06d95
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":156,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 463,
    "id": 154,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 133,
    "additional_university_ids": [

    ],
    "topic_id": 156,
    "discipline_id": 156,
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
    "chapters_updated_at": "2016-10-27T17:15:30.472Z",
    "updated_at": "2016-10-27T17:15:30.609Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 119,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-27T17:15:30.562Z",
        "course_id": 154,
        "author_id": 463,
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
        "id": 120,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-27T17:15:30.581Z",
        "course_id": 154,
        "author_id": 463,
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
        "id": 121,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-27T17:15:30.598Z",
        "course_id": 154,
        "author_id": 463,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":156,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a20978e2366a86812b5d151a5cbd25000298b626c0e726dbfdf152c073a06d95"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6d55af655255a6e510057386533d601b81514623790c19e62eecea66a986b266
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":155,"published":false}}
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
    "creator_id": 462,
    "id": 153,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 132,
    "additional_university_ids": [

    ],
    "topic_id": 155,
    "discipline_id": 155,
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
    "updated_at": "2016-10-27T17:15:30.437Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":155,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d55af655255a6e510057386533d601b81514623790c19e62eecea66a986b266"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 747b702196baa81bb0f58705962d67cb6917ac8a5d6ea3b441f6b44927bc9519
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
      "creator_id": 436,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-101",
      "html_url": "https://goskive.com/course/fu-course-101",
      "slug": "fu-course-101",
      "university_id": 123,
      "additional_university_ids": [

      ],
      "topic_id": 133,
      "discipline_id": 133,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 101",
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
      "updated_at": "2016-10-27T17:15:27.992Z",
      "shortname": "fu-course-101"
    },
    {
      "creator_id": 436,
      "id": 132,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 123,
      "additional_university_ids": [

      ],
      "topic_id": 134,
      "discipline_id": 134,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
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
      "chapters_updated_at": "2016-10-27T17:15:28.301Z",
      "updated_at": "2016-10-27T17:15:28.309Z",
      "shortname": "fu-course-102"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 747b702196baa81bb0f58705962d67cb6917ac8a5d6ea3b441f6b44927bc9519"
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
      "creator_id": 456,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-117",
      "html_url": "https://goskive.com/course/fu-course-117",
      "slug": "fu-course-117",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "topic_id": 149,
      "discipline_id": 149,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 117",
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
      "updated_at": "2016-10-27T17:15:29.747Z",
      "shortname": "fu-course-117"
    },
    {
      "creator_id": 456,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-118",
      "html_url": "https://goskive.com/course/fu-course-118",
      "slug": "fu-course-118",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "topic_id": 150,
      "discipline_id": 150,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 118",
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
      "chapters_updated_at": "2016-10-27T17:15:30.055Z",
      "updated_at": "2016-10-27T17:15:30.063Z",
      "shortname": "fu-course-118"
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
Authorization: Bearer 987790176a9f4fa7d8f0080b1d5e8b88148a4420a11a8e9ab1cd894b290ef14a
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
      "creator_id": 442,
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 124,
      "additional_university_ids": [

      ],
      "topic_id": 137,
      "discipline_id": 137,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
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
      "updated_at": "2016-10-27T17:15:28.526Z",
      "shortname": "fu-course-105"
    },
    {
      "creator_id": 442,
      "id": 136,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 124,
      "additional_university_ids": [

      ],
      "topic_id": 138,
      "discipline_id": 138,
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
      "updated_at": "2016-10-27T17:15:28.566Z",
      "shortname": "fu-course-106"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 987790176a9f4fa7d8f0080b1d5e8b88148a4420a11a8e9ab1cd894b290ef14a"
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
      "creator_id": 461,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-121",
      "html_url": "https://goskive.com/course/fu-course-121",
      "slug": "fu-course-121",
      "university_id": 131,
      "additional_university_ids": [

      ],
      "topic_id": 153,
      "discipline_id": 153,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 121",
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
      "updated_at": "2016-10-27T17:15:30.275Z",
      "shortname": "fu-course-121"
    },
    {
      "creator_id": 461,
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 131,
      "additional_university_ids": [

      ],
      "topic_id": 154,
      "discipline_id": 154,
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
      "updated_at": "2016-10-27T17:15:30.316Z",
      "shortname": "fu-course-122"
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
Authorization: Bearer bb0f8e575ac224001236082a822fae0495b05722ec85c711031854aa75d6bf8f
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
  "id": 937,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-27T17:16:10.671Z",
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
	-H "Authorization: Bearer bb0f8e575ac224001236082a822fae0495b05722ec85c711031854aa75d6bf8f"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/155
Content-Type: application/json
Authorization: Bearer 46203feacc31eca27861b8d9eefea4c45f4ff48ca55bd8d7df24b178e38f548e
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
    "id": 155,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 42,
    "fields_of_study": [
      42,
      43
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-27T17:15:03.860Z",
    "updated_at": "2016-10-27T17:15:03.860Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/155" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46203feacc31eca27861b8d9eefea4c45f4ff48ca55bd8d7df24b178e38f548e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/157
Content-Type: application/json
Authorization: Bearer 0a039677521e88b60b93769fbd18d94198e2fa651136042bf719308efd66e7a4
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
    "id": 157,
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
    "created_at": "2016-10-27T17:15:03.944Z",
    "updated_at": "2016-10-27T17:15:03.944Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/157" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a039677521e88b60b93769fbd18d94198e2fa651136042bf719308efd66e7a4"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 190ab7247d48a5ecd44d84cd2f96cc56939be512ed4169b27fab461e933ac8d5
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 190ab7247d48a5ecd44d84cd2f96cc56939be512ed4169b27fab461e933ac8d5"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer 7f066fc2cd503c97f70e7c6f83a0d95d6727cd1e988f4bd418fbbe912ccac35d
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
    "id": 14,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 61,
    "user_id": 363
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f066fc2cd503c97f70e7c6f83a0d95d6727cd1e988f4bd418fbbe912ccac35d"
```
