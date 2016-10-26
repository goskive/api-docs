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
Authorization: Basic NjBmOTdiOWMzNTAyYmIzYzQxYWRjZDM4NzVjMzZhYzJkNzg4MDdlMTUyYTkw
ZTA5ZWI1NDQyMzkwOThhZGRhYjo2ZTYzNDBhZDExYjMwMTQyMDNlZWVmNDY2
NDhlOGFkZDllYTBlNGU0ZjA2ODllMzYwZjk4N2VhMzdkZTYyNDQy

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
	-u 60f97b9c3502bb3c41adcd3875c36ac2d78807e152a90e09eb544239098addab:6e6340ad11b3014203eeef46648e8add9ea0e4e4f0689e360f987ea37de62442
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"283b71dedc911f2e95a7ab5678af8bd597e696e306f653577f17ac3a0aa3701c","client_secret":"77ce0ee96da39401c33024cd05481f81aac8d73825e0f1c0b8ea797203623aa0"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"283b71dedc911f2e95a7ab5678af8bd597e696e306f653577f17ac3a0aa3701c","client_secret":"77ce0ee96da39401c33024cd05481f81aac8d73825e0f1c0b8ea797203623aa0"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"38a989bc1c5c6716bfcbf6cd27bd0811d527671a4a3b6709684732492d14a9d7","client_secret":"9bb002566bd67d22bc4ffbcb19900390cc2a6cb68fdc9b623d4ec8430455294b"}
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
  "access_token": "daeb6e5041e69bd9923fb55c1e32d0de0a60e5f5831f7c7194aa011227c4073b",
  "token_type": "bearer",
  "created_at": 1477510293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"38a989bc1c5c6716bfcbf6cd27bd0811d527671a4a3b6709684732492d14a9d7","client_secret":"9bb002566bd67d22bc4ffbcb19900390cc2a6cb68fdc9b623d4ec8430455294b"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YWJmZTk1YjRhOTljMWMyY2UxNzYzYjg3NTJjYWI4YmRmMWIxMDdmODRlMWRl
YTBhMWJhODZhODA1MjA1ZWNkZTo3OTM5M2QyNjAwZmEwMDU2NDQ1MDIzYjM0
YzIxOTlhNDYwMWU0NTdjYzM5NmQ3NmE0YTliZmZiNTQzNzRlYTJl

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
  "access_token": "470cd1adcc988c91b253ff81af2d9e47b2eec11189f3d45faeb371b17e2ecf58",
  "token_type": "bearer",
  "created_at": 1477510293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u abfe95b4a99c1c2ce1763b8752cab8bdf1b107f84e1dea0a1ba86a805205ecde:79393d2600fa0056445023b34c2199a4601e457cc396d76a4a9bffb54374ea2e
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"330a3689faade3b890fe4073d1550dbd1d7360eeaaa170aeecc53a572d9acefe","client_secret":"f4a7e4e5e82b1109548d7199c69a498d2321d3d7493f8605617a7ffdaef31545"}
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
  "access_token": "fab80b622d1842b4766955effc6fd19866a1dfe75f4a2529cf9c71eb83b9deb4",
  "token_type": "bearer",
  "created_at": 1477510293
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"330a3689faade3b890fe4073d1550dbd1d7360eeaaa170aeecc53a572d9acefe","client_secret":"f4a7e4e5e82b1109548d7199c69a498d2321d3d7493f8605617a7ffdaef31545"}' -X POST \
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
Authorization: Bearer 4db6878014d1cad4b3493f8d0a292ec400d0661536e189a44277cf49ad4296b4
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
	-H "Authorization: Bearer 4db6878014d1cad4b3493f8d0a292ec400d0661536e189a44277cf49ad4296b4"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/19/flashcards
Content-Type: application/json
Authorization: Bearer cc4070daa4930f87b3db994beca571e78fa71f6cc4284e0fe957fabd6f4e10d3
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":19,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 100,
    "chapter_id": 19,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:31:30.024Z",
    "created_at": "2016-10-26T19:31:30.024Z",
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
curl "api.goskive.com/v2/chapters/19/flashcards" -d '{"flashcard":{"chapter_id":19,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc4070daa4930f87b3db994beca571e78fa71f6cc4284e0fe957fabd6f4e10d3"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/17/flashcards
Content-Type: application/json
Authorization: Bearer 6524e5935da9eacfeff5d3b6e94cb23fd8a414f0559e5ac809e5366f8e6b92c7
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
      "author_id": 92,
      "chapter_id": 17,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:29.652Z",
      "created_at": "2016-10-26T19:31:29.652Z",
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
      "author_id": 92,
      "chapter_id": 17,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:29.687Z",
      "created_at": "2016-10-26T19:31:29.687Z",
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
      "author_id": 92,
      "chapter_id": 17,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:29.721Z",
      "created_at": "2016-10-26T19:31:29.721Z",
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
curl "api.goskive.com/v2/chapters/17/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6524e5935da9eacfeff5d3b6e94cb23fd8a414f0559e5ac809e5366f8e6b92c7"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 423981b1cd228a7cb5f20c7c9610e0e7483f2d76ef74653f3c0fc60eab7fbe54
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 20,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:31:22.889Z",
    "created_at": "2016-10-26T19:31:22.889Z",
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
        "id": 8,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 9,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 10,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 11,
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
curl "api.goskive.com/v2/chapters/4/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 423981b1cd228a7cb5f20c7c9610e0e7483f2d76ef74653f3c0fc60eab7fbe54"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/2/questions
Content-Type: application/json
Authorization: Bearer 539908e1fd56a0d886ee00bfb6f27b3e94a453c150eb6ce6c9bc25930167fbc9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":2,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 2,
    "obfuscated_id": "yHhUU9c1C7Y",
    "author_id": 14,
    "chapter_id": 2,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:31:22.279Z",
    "created_at": "2016-10-26T19:31:22.279Z",
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
        "id": 4,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 5,
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
curl "api.goskive.com/v2/chapters/2/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":2,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 539908e1fd56a0d886ee00bfb6f27b3e94a453c150eb6ce6c9bc25930167fbc9"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer 329dc577885a73483d9895100b2ec042619d7d534582597a55f10b21c2bfdb89
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
    "id": 3,
    "obfuscated_id": "bco7bNtr_d4",
    "author_id": 17,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:31:22.579Z",
    "created_at": "2016-10-26T19:31:22.579Z",
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
        "id": 6,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 7,
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
	-H "Authorization: Bearer 329dc577885a73483d9895100b2ec042619d7d534582597a55f10b21c2bfdb89"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/1/questions
Content-Type: application/json
Authorization: Bearer e3b1c115d67a17f1293b43e9714126f0df6c78a79c015ef91e13aec6aa223f63
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":1,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 1,
    "obfuscated_id": "vnOJWgI0jGc",
    "author_id": 11,
    "chapter_id": 1,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:31:21.853Z",
    "created_at": "2016-10-26T19:31:21.853Z",
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
        "id": 1,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 2,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 3,
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
curl "api.goskive.com/v2/chapters/1/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":1,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3b1c115d67a17f1293b43e9714126f0df6c78a79c015ef91e13aec6aa223f63"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer 6ea14070cf56541c22ae580a775fc9358e718311a168eb9a37cfa76cf8defc01
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
      "id": 5,
      "obfuscated_id": "iw-7peoPwEU",
      "author_id": 23,
      "chapter_id": 5,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:23.460Z",
      "created_at": "2016-10-26T19:31:23.347Z",
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
          "id": 12,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 13,
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
      "chapter_id": 5,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:23.643Z",
      "created_at": "2016-10-26T19:31:23.527Z",
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
          "id": 14,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 15,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 25,
      "chapter_id": 5,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:31:23.832Z",
      "created_at": "2016-10-26T19:31:23.716Z",
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
          "id": 16,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 17,
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
curl "api.goskive.com/v2/chapters/5/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ea14070cf56541c22ae580a775fc9358e718311a168eb9a37cfa76cf8defc01"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/66
Content-Type: application/json
Authorization: Bearer 9af74ae339967d26906018cf59a17742d75717ec6beed50e5b925d50f8930dc9
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
curl "api.goskive.com/v2/chapters/66" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9af74ae339967d26906018cf59a17742d75717ec6beed50e5b925d50f8930dc9"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/68
Content-Type: application/json
Authorization: Bearer d474e5dcebc7c11ce26401c6039a3e3bad29557354003e6e95928fa7d22a0bb5
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
curl "api.goskive.com/v2/chapters/68" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d474e5dcebc7c11ce26401c6039a3e3bad29557354003e6e95928fa7d22a0bb5"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/61
Content-Type: application/json
Authorization: Bearer 56e63862fb28907d486cf6a2ec87987f9e376fbbf96df3eba280539677c3a5cb
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
curl "api.goskive.com/v2/chapters/61" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56e63862fb28907d486cf6a2ec87987f9e376fbbf96df3eba280539677c3a5cb"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/67
Content-Type: application/json
Authorization: Bearer 0b0d7db93fdc06590eef0b5a2736d237493794a5fa49ba9f6ed1baa7346c86cc
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/67" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b0d7db93fdc06590eef0b5a2736d237493794a5fa49ba9f6ed1baa7346c86cc"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/64
Content-Type: application/json
Authorization: Bearer 29d28b3d3817a4418c4460947a1ba394a484240f91f09e3917c1a5a8e9a84c46
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
    "id": 64,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T19:31:45.432Z",
    "course_id": 113,
    "author_id": 358,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-26T19:31:44.950Z",
    "questions_updated_at": "2016-10-26T19:31:44.950Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 362,
        "chapter_id": 64,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.417Z",
        "created_at": "2016-10-26T19:31:45.417Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 360,
        "chapter_id": 64,
        "position": 31,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:45.321Z",
        "created_at": "2016-10-26T19:31:45.212Z",
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
            "id": 72,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 73,
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
curl "api.goskive.com/v2/chapters/64" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29d28b3d3817a4418c4460947a1ba394a484240f91f09e3917c1a5a8e9a84c46"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/62
Content-Type: application/json
Authorization: Bearer 5d129dd6aa8f9928c9d5b92def74963da5dfc770e83b386757df0a9be41fdbd2
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
    "id": 62,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T19:31:44.783Z",
    "course_id": 111,
    "author_id": 353,
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
curl "api.goskive.com/v2/chapters/62" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d129dd6aa8f9928c9d5b92def74963da5dfc770e83b386757df0a9be41fdbd2"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/57/replies
Content-Type: application/json
Authorization: Bearer a7fced602af46e1c251cb9731f5d890ed5b1b9d2b07cabe27d895b12a0b3be44
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
    "id": 58,
    "author_id": 853,
    "reply_to_id": 57,
    "created_at": "2016-10-26T19:32:21.736Z",
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
curl "api.goskive.com/v2/comments/57/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7fced602af46e1c251cb9731f5d890ed5b1b9d2b07cabe27d895b12a0b3be44"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer c9b034abcc894236611371f7e7f0de0b1625f0d02ffe4280aa7af711359a620b
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
curl "api.goskive.com/v2/comments/56/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9b034abcc894236611371f7e7f0de0b1625f0d02ffe4280aa7af711359a620b"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer 954a72b496e0f2cadc946585dd78423d934bdb30611791bda7e155958a3efe4d
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
curl "api.goskive.com/v2/comments/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 954a72b496e0f2cadc946585dd78423d934bdb30611791bda7e155958a3efe4d"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/9/republish
Content-Type: application/json
Authorization: Bearer d997f7d20d5c2ae76a49210e93f531813795d75f51dcebeaede76b169b16082b
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
curl "api.goskive.com/v2/comments/9/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d997f7d20d5c2ae76a49210e93f531813795d75f51dcebeaede76b169b16082b"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer b0e32b3cc77776bc874e9d5970bc89fb8daf32193f6122fb225ec5152200e4d1
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0e32b3cc77776bc874e9d5970bc89fb8daf32193f6122fb225ec5152200e4d1"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/4/report
Content-Type: application/json
Authorization: Bearer 08fa885796644d8c79630136e9f518811ce547eb1b97675a851f86626025ec68
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/4/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08fa885796644d8c79630136e9f518811ce547eb1b97675a851f86626025ec68"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/25
Content-Type: application/json
Authorization: Bearer 36e03c20dc6d6607cb3551d249eb03771c50ecd662c3101e90854b6bb59ff32a
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
    "id": 25,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-26T19:31:47.707Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36e03c20dc6d6607cb3551d249eb03771c50ecd662c3101e90854b6bb59ff32a"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 066578609e0d305f882bce43dedf6a70e69637ae0a636b9b469c46129a94eeb6
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
      "id": 22,
      "name": "Fake Company Name 21",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:31:47.593Z"
    },
    {
      "id": 23,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:31:47.597Z"
    },
    {
      "id": 24,
      "name": "Fake Company Name 23",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T19:31:47.600Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 066578609e0d305f882bce43dedf6a70e69637ae0a636b9b469c46129a94eeb6"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer 836b973c504746a496b45dea00fda135908c81f0710bec9972a32f279d388739
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
curl "api.goskive.com/v2/companies/27/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 836b973c504746a496b45dea00fda135908c81f0710bec9972a32f279d388739"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer f280a47d783741c5a183150a4c576df45f4df76918f39e7bc5974a87ddfd1d9f
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
curl "api.goskive.com/v2/companies/26/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f280a47d783741c5a183150a4c576df45f4df76918f39e7bc5974a87ddfd1d9f"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 95a868c8b6662a81dadc94f8187083bf37d066bbf6321d6ba8b11aa4f5ecab6d
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
    },
    {
      "id": 8,
      "title": "Campaign 7",
      "company_id": 13,
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
	-H "Authorization: Bearer 95a868c8b6662a81dadc94f8187083bf37d066bbf6321d6ba8b11aa4f5ecab6d"
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
Authorization: Bearer ed127feb226ccb5b1f44cc5aa085d4ca4651f45676e4668b3bbbc460cb906053
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
	-H "Authorization: Bearer ed127feb226ccb5b1f44cc5aa085d4ca4651f45676e4668b3bbbc460cb906053"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8b01c4cd15349edf4e0098b6bbdd35b598e75aa2f6dad4da9ff17b1725df2143
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
    "id": 33,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:31:40.353Z",
    "course_id": 91,
    "author_id": 278,
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
	-H "Authorization: Bearer 8b01c4cd15349edf4e0098b6bbdd35b598e75aa2f6dad4da9ff17b1725df2143"
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
      "id": 45,
      "title": "Clever Chapter Title 33",
      "position": 1,
      "updated_at": "2016-10-26T19:31:41.713Z",
      "course_id": 100,
      "author_id": 307,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 46,
      "title": "Clever Chapter Title 34",
      "position": 2,
      "updated_at": "2016-10-26T19:31:41.735Z",
      "course_id": 100,
      "author_id": 308,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 47,
      "title": "Clever Chapter Title 35",
      "position": 3,
      "updated_at": "2016-10-26T19:31:41.968Z",
      "course_id": 100,
      "author_id": 309,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T19:31:41.644Z",
      "questions_updated_at": "2016-10-26T19:31:41.644Z",
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
Authorization: Bearer b013442c34f5e30c88e93a9a04ae61ab5254bde96b2ae7aad7b54b9aaf4cfceb
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
      "id": 51,
      "title": "Clever Chapter Title 39",
      "position": 1,
      "updated_at": "2016-10-26T19:31:42.293Z",
      "course_id": 103,
      "author_id": 318,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 52,
      "title": "Clever Chapter Title 40",
      "position": 2,
      "updated_at": "2016-10-26T19:31:42.314Z",
      "course_id": 103,
      "author_id": 319,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 53,
      "title": "Clever Chapter Title 41",
      "position": 3,
      "updated_at": "2016-10-26T19:31:42.544Z",
      "course_id": 103,
      "author_id": 320,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T19:31:42.225Z",
      "questions_updated_at": "2016-10-26T19:31:42.225Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b013442c34f5e30c88e93a9a04ae61ab5254bde96b2ae7aad7b54b9aaf4cfceb"
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
      "id": 48,
      "title": "Clever Chapter Title 36",
      "position": 1,
      "updated_at": "2016-10-26T19:31:42.145Z",
      "course_id": 102,
      "author_id": 314,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 49,
      "title": "Clever Chapter Title 37",
      "position": 2,
      "updated_at": "2016-10-26T19:31:42.166Z",
      "course_id": 102,
      "author_id": 315,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 50,
      "title": "Clever Chapter Title 38",
      "position": 3,
      "updated_at": "2016-10-26T19:31:42.188Z",
      "course_id": 102,
      "author_id": 316,
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
Authorization: Bearer 86b5d4544ca51c2616f688671c50d84772dc84d44b97c45444a4d4a68d45ac10
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
      "updated_at": "2016-10-26T19:31:42.779Z",
      "course_id": 105,
      "author_id": 327,
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
      "updated_at": "2016-10-26T19:31:42.802Z",
      "course_id": 105,
      "author_id": 328,
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
      "updated_at": "2016-10-26T19:31:42.824Z",
      "course_id": 105,
      "author_id": 329,
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
	-H "Authorization: Bearer 86b5d4544ca51c2616f688671c50d84772dc84d44b97c45444a4d4a68d45ac10"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 36b693e8b8f6e1d34eee5c1e4fdda1bccff97f56512cef1762615f4bdec2762e
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
    "course_id": 275,
    "user_id": 841,
    "updated_at": "2016-10-26T19:32:20.936Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36b693e8b8f6e1d34eee5c1e4fdda1bccff97f56512cef1762615f4bdec2762e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 456b9f22fa34718c5601d0a85377754dcbe1d7d9d4e55b50c50b559e2660e20a
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
      "id": 4,
      "course_id": 273,
      "user_id": 835,
      "updated_at": "2016-10-26T19:32:20.640Z"
    },
    {
      "id": 5,
      "course_id": 273,
      "user_id": 836,
      "updated_at": "2016-10-26T19:32:20.654Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 456b9f22fa34718c5601d0a85377754dcbe1d7d9d4e55b50c50b559e2660e20a"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/68/files
Content-Type: application/json
Authorization: Bearer d1ab7e008d3f322d5f735d0fee80db4ac68fda7ae02c0a2a910e911031c16d2a
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
        "id": 207,
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
        "created_at": "2016-10-26T19:31:34.387Z",
        "updated_at": "2016-10-26T19:31:34.387Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:31:34.452Z",
      "updated_at": "2016-10-26T19:31:34.452Z",
      "course_id": 68,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 208,
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
        "created_at": "2016-10-26T19:31:34.460Z",
        "updated_at": "2016-10-26T19:31:34.460Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:31:34.469Z",
      "updated_at": "2016-10-26T19:31:34.469Z",
      "course_id": 68,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 209,
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
        "created_at": "2016-10-26T19:31:34.475Z",
        "updated_at": "2016-10-26T19:31:34.475Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T19:31:34.484Z",
      "updated_at": "2016-10-26T19:31:34.484Z",
      "course_id": 68,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/68/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1ab7e008d3f322d5f735d0fee80db4ac68fda7ae02c0a2a910e911031c16d2a"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/70/files
Content-Type: application/json
Authorization: Bearer 2abf0270ab365a13fab5e6b07152c6ecc0ddef439d52d523b5b4c803be285bec
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
      "id": 214,
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
      "created_at": "2016-10-26T19:31:34.682Z",
      "updated_at": "2016-10-26T19:31:34.682Z"
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
    "created_at": "2016-10-26T19:31:34.707Z",
    "updated_at": "2016-10-26T19:31:34.707Z",
    "course_id": 70,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/70/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2abf0270ab365a13fab5e6b07152c6ecc0ddef439d52d523b5b4c803be285bec"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/69/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 9ad03b3cee91ae289babdf89cf6879c4ffa56c85010cb5bd559a7657cb16bc02
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
    "key": "cache/91c9049abcaaa2b68b9ba171674c94c7.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQyMDozMTozNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzkxYzkwNDlhYmNhYWEyYjY4YjliYTE3MTY3NGM5NGM3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI2VDE5MzEzNFoifV19",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T193134Z",
    "x-amz-signature": "6c0178992321a3d4e6ca73dfae3e327b8b8c4f05008a059236407aa0e2c7c1b9"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/69/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ad03b3cee91ae289babdf89cf6879c4ffa56c85010cb5bd559a7657cb16bc02"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 18fe3a0c833f1294b4ae70f7d4845b3be3bbf642133110c63134a4fa6c7fc3cd
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
	-H "Authorization: Bearer 18fe3a0c833f1294b4ae70f7d4845b3be3bbf642133110c63134a4fa6c7fc3cd"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2f1f27089bd491bed5f3cc0881c2c08448256b457282e75d222eda9716f91a71
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
	-H "Authorization: Bearer 2f1f27089bd491bed5f3cc0881c2c08448256b457282e75d222eda9716f91a71"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bc3b4585b1789bdec786cc0fac4846bdbf783da55a8a72b608d3d1b58e20bcaf
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
	-H "Authorization: Bearer bc3b4585b1789bdec786cc0fac4846bdbf783da55a8a72b608d3d1b58e20bcaf"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c1aa6f0bd39aef1952ad7fdafcca9991dd24d7618028cb16a24a25ce8684737b
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
	-H "Authorization: Bearer c1aa6f0bd39aef1952ad7fdafcca9991dd24d7618028cb16a24a25ce8684737b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a14dd26acc53b05b099a8af40c06ab5909ed550f2bb6ab4bc0ac7331dfc1d36f
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
	-H "Authorization: Bearer a14dd26acc53b05b099a8af40c06ab5909ed550f2bb6ab4bc0ac7331dfc1d36f"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 226cb39d285bd9793e602628a7156ca67c277fcfa6156f5aa727a1874614d2fe
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
    "creator_id": 417,
    "id": 131,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 138,
    "additional_university_ids": [

    ],
    "topic_id": 141,
    "discipline_id": 141,
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
    "chapters_updated_at": "2016-10-26T19:31:51.041Z",
    "updated_at": "2016-10-26T19:31:52.401Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 74,
        "title": "Clever Chapter Title 53",
        "position": 1,
        "updated_at": "2016-10-26T19:31:52.358Z",
        "course_id": 131,
        "author_id": 417,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:31:51.041Z",
        "questions_updated_at": "2016-10-26T19:31:51.041Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 75,
        "title": "Clever Chapter Title 54",
        "position": 2,
        "updated_at": "2016-10-26T19:31:52.394Z",
        "course_id": 131,
        "author_id": 417,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:31:51.041Z",
        "questions_updated_at": "2016-10-26T19:31:51.041Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 418,
        "chapter_id": 74,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:52.187Z",
        "created_at": "2016-10-26T19:31:52.187Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 418,
        "chapter_id": 75,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:52.252Z",
        "created_at": "2016-10-26T19:31:52.252Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 418,
        "chapter_id": 74,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:52.224Z",
        "created_at": "2016-10-26T19:31:52.224Z",
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
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 418,
        "chapter_id": 75,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:52.289Z",
        "created_at": "2016-10-26T19:31:52.289Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 418,
        "chapter_id": 74,
        "position": 48,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:51.240Z",
        "created_at": "2016-10-26T19:31:51.132Z",
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
            "id": 106,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 107,
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
        "author_id": 418,
        "chapter_id": 74,
        "position": 49,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:51.402Z",
        "created_at": "2016-10-26T19:31:51.299Z",
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
            "id": 108,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 109,
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
        "author_id": 418,
        "chapter_id": 75,
        "position": 50,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:51.590Z",
        "created_at": "2016-10-26T19:31:51.477Z",
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
            "id": 110,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 111,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 418,
        "chapter_id": 75,
        "position": 51,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:51.760Z",
        "created_at": "2016-10-26T19:31:51.651Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 226cb39d285bd9793e602628a7156ca67c277fcfa6156f5aa727a1874614d2fe"
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
    "creator_id": 423,
    "id": 132,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 139,
    "additional_university_ids": [

    ],
    "topic_id": 142,
    "discipline_id": 142,
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
    "chapters_updated_at": "2016-10-26T19:31:52.511Z",
    "updated_at": "2016-10-26T19:31:53.827Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 76,
        "title": "Clever Chapter Title 55",
        "position": 1,
        "updated_at": "2016-10-26T19:31:53.784Z",
        "course_id": 132,
        "author_id": 423,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:31:52.511Z",
        "questions_updated_at": "2016-10-26T19:31:52.511Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 77,
        "title": "Clever Chapter Title 56",
        "position": 2,
        "updated_at": "2016-10-26T19:31:53.820Z",
        "course_id": 132,
        "author_id": 423,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T19:31:52.511Z",
        "questions_updated_at": "2016-10-26T19:31:52.511Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 423,
        "chapter_id": 76,
        "position": 54,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:52.701Z",
        "created_at": "2016-10-26T19:31:52.594Z",
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
            "id": 118,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 119,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 423,
        "chapter_id": 77,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:31:53.050Z",
        "created_at": "2016-10-26T19:31:52.938Z",
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
            "id": 122,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 123,
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
PUT /v2/courses/143/pin
Content-Type: application/json
Authorization: Bearer 13f0ac7c606ad9e8017ab4c2402e044e00f3504bba956087c0c1bb2ec8f6f412
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/143/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13f0ac7c606ad9e8017ab4c2402e044e00f3504bba956087c0c1bb2ec8f6f412"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/133/pin
Content-Type: application/json
Authorization: Bearer 4ca78811738c68cdb1137dfb07e108eee0dcfba1a606f316a00d87eb89c27e08
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/133/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ca78811738c68cdb1137dfb07e108eee0dcfba1a606f316a00d87eb89c27e08"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 254056461ea64f5fb93884b2fbc6549c8e5ccebea35aa5a0445925ed009ddc19
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
    "creator_id": 400,
    "id": 126,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 133,
    "additional_university_ids": [

    ],
    "topic_id": 136,
    "discipline_id": 136,
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
    "updated_at": "2016-10-26T19:31:47.988Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 254056461ea64f5fb93884b2fbc6549c8e5ccebea35aa5a0445925ed009ddc19"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 105c7065ad73d2fd88787204a96894bc08232b98ebdd27e3887425621fe54551
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
    "id": 76,
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
    "created_at": "2016-10-26T19:31:28.128Z",
    "updated_at": "2016-10-26T19:31:28.128Z",
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
	-H "Authorization: Bearer 105c7065ad73d2fd88787204a96894bc08232b98ebdd27e3887425621fe54551"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 4d6858fa4cc6e58d4926f7300a5e74d8e43380e24f75ccdcd70cf7777f36546e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[19]}
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
    "id": 72,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      19
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:31:27.885Z",
    "updated_at": "2016-10-26T19:31:27.918Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[19]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d6858fa4cc6e58d4926f7300a5e74d8e43380e24f75ccdcd70cf7777f36546e"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 06230d3120e19f7e63213152e7c635f55c06aa0f5437f740319f48e06e53450f
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
    "id": 74,
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
    "created_at": "2016-10-26T19:31:28.002Z",
    "updated_at": "2016-10-26T19:31:28.002Z",
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
	-H "Authorization: Bearer 06230d3120e19f7e63213152e7c635f55c06aa0f5437f740319f48e06e53450f"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 49d04f18a4a5019311d0c9d59eeb4323b42bd1bd3ed47cebbac340073833d901
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[22]}
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
    "id": 75,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      22
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:31:28.084Z",
    "updated_at": "2016-10-26T19:31:28.084Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[22]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49d04f18a4a5019311d0c9d59eeb4323b42bd1bd3ed47cebbac340073833d901"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 97806d1f939c414b91321dd305bcd558872ab5ccde9f018003ccac190767f44c
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

18
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
    "id": 71,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/79a12c5ad83e145ed83e4a7b4c776173e676377f.jpg",
    "university_id": null,
    "fields_of_study": [
      18
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T19:31:27.486Z",
    "updated_at": "2016-10-26T19:31:27.831Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/160c8752b5058f462180707be0346fb26a8012ca.jpg",
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

18
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 97806d1f939c414b91321dd305bcd558872ab5ccde9f018003ccac190767f44c"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 95c3b656cc5c1ce9b01f5b75fc06714c58131107f2d3d02581bc3aee6659c879
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
      "bookmarkable_id": 101,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 102,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 103,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95c3b656cc5c1ce9b01f5b75fc06714c58131107f2d3d02581bc3aee6659c879"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a62b5f3eee07ab66495ebc8962fa9889c58f8320d38f8fd28e46db470e34d9ae
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
	-H "Authorization: Bearer a62b5f3eee07ab66495ebc8962fa9889c58f8320d38f8fd28e46db470e34d9ae"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer c2fe9426bd4956b67775eca5509d2cd0323214020dec21734184f551d72434e1
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
	-H "Authorization: Bearer c2fe9426bd4956b67775eca5509d2cd0323214020dec21734184f551d72434e1"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 901efd2456b60c44c24213de628ea53d08c204348786e56f69b6b945e2422564
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
      "creator_id": 65,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-10",
      "html_url": "https://goskive.com/course/mit-course-10",
      "slug": "mit-course-10",
      "university_id": 16,
      "additional_university_ids": [

      ],
      "topic_id": 16,
      "discipline_id": 16,
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
      "updated_at": "2016-10-26T19:31:26.573Z",
      "shortname": "mit-course-10"
    },
    {
      "creator_id": 66,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-11",
      "html_url": "https://goskive.com/course/mit-course-11",
      "slug": "mit-course-11",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 17,
      "discipline_id": 17,
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
      "updated_at": "2016-10-26T19:31:26.671Z",
      "shortname": "mit-course-11"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 901efd2456b60c44c24213de628ea53d08c204348786e56f69b6b945e2422564"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer fd69f4da226aadaa81e85274be2e684fea3701d626ee7e1a67005677004d3666
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
        "updated_at": "2016-10-26T19:32:22.551Z"
      },
      "created_at": "2016-10-26T19:32:22.554Z",
      "updated_at": "2016-10-26T19:32:22.554Z",
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
        "updated_at": "2016-10-26T19:32:22.562Z"
      },
      "created_at": "2016-10-26T19:32:22.565Z",
      "updated_at": "2016-10-26T19:32:22.565Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd69f4da226aadaa81e85274be2e684fea3701d626ee7e1a67005677004d3666"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 83c0951f6c60425e191325798623ddd1d3ffaebea942d61dc3a9601347b1fee6
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
        "updated_at": "2016-10-26T19:32:22.353Z"
      },
      "created_at": "2016-10-26T19:32:22.357Z",
      "updated_at": "2016-10-26T19:32:22.357Z",
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
        "updated_at": "2016-10-26T19:32:22.369Z"
      },
      "created_at": "2016-10-26T19:32:22.372Z",
      "updated_at": "2016-10-26T19:32:22.372Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83c0951f6c60425e191325798623ddd1d3ffaebea942d61dc3a9601347b1fee6"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 7809b865573a6db784d7a4d8e33eb886597cfea56c85675435970d51cad7d9c3
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
      "id": 1,
      "created_at": "2016-10-26T19:31:24.218Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 1,
      "updated_at": "2016-10-26T19:31:24.332Z",
      "author_id": "32",
      "thread_subject_id": "7",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 2,
      "created_at": "2016-10-26T19:31:24.322Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-26T19:31:24.335Z",
      "author_id": "35",
      "thread_subject_id": "8",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 3,
      "created_at": "2016-10-26T19:31:24.704Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-26T19:31:24.704Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-10-26T19:31:25.053Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-26T19:31:25.053Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 5,
      "created_at": "2016-10-26T19:31:25.412Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-26T19:31:25.412Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 6,
      "created_at": "2016-10-26T19:31:25.683Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 11,
      "updated_at": "2016-10-26T19:31:25.683Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 7,
      "created_at": "2016-10-26T19:31:25.956Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 12,
      "updated_at": "2016-10-26T19:31:25.956Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-10-26T19:31:26.221Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 13,
      "updated_at": "2016-10-26T19:31:26.221Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7809b865573a6db784d7a4d8e33eb886597cfea56c85675435970d51cad7d9c3"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/9
Content-Type: application/json
Authorization: Bearer cedb96f1fc554146a00aee7a71479f9084830116a94d27af28f2ed5872cb3275
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-26T19:21:26.000Z"}}
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
    "id": 9,
    "created_at": "2016-10-26T19:31:26.402Z",
    "read_at": "2016-10-26T19:21:26.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 3,
    "updated_at": "2016-10-26T19:31:26.435Z",
    "author_id": "61",
    "thread_subject_id": "15",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/9" -d '{"notification":{"read_at":"2016-10-26T19:21:26.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cedb96f1fc554146a00aee7a71479f9084830116a94d27af28f2ed5872cb3275"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer d76d0b629a2d01a5b845496738c2344e6b06b0140714435a79e8c64175b52f57
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
      "course_id": 121,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T19:31:47.250Z",
      "course_published": true,
      "updated_at": "2016-10-26T19:31:47.243Z"
    },
    {
      "id": 5,
      "course_id": 122,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T19:31:47.322Z",
      "course_published": true,
      "updated_at": "2016-10-26T19:31:47.316Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d76d0b629a2d01a5b845496738c2344e6b06b0140714435a79e8c64175b52f57"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 4f33f841435b38cf5c53813547ab57e87e531d4cb792e0e4b9f111c31eaca177
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
    "course_id": 123,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T19:31:47.430Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:31:47.423Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f33f841435b38cf5c53813547ab57e87e531d4cb792e0e4b9f111c31eaca177"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 75588981d22c3c24d7da8cd835995eb282b527a06a75e650dec7e3b3a41e0984
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
    "course_id": 124,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-26T19:31:47.577Z",
    "course_published": true,
    "updated_at": "2016-10-26T19:31:47.567Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75588981d22c3c24d7da8cd835995eb282b527a06a75e650dec7e3b3a41e0984"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 4e051f50ff24c6b1d8cc35be03f04391b3dc50fa3e5b581be318752d42a22ba3
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
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 30,
      "user_id": 332
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 31,
      "user_id": 332
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 332
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 33,
      "user_id": 332
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e051f50ff24c6b1d8cc35be03f04391b3dc50fa3e5b581be318752d42a22ba3"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/168
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
    "id": 168,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 166,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 168
      },
      {
        "id": 167,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 168
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/168" -X GET \
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
      "id": 166,
      "name": "Multi-tiered methodical alliance",
      "name_translations": {
        "en": "Multi-tiered methodical alliance"
      }
    },
    {
      "id": 167,
      "name": "Secured scalable pricing structure",
      "name_translations": {
        "en": "Secured scalable pricing structure"
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
PATCH /v2/feedbacks/10/close
Content-Type: application/json
Authorization: Bearer 3912c1a86d246c691bca974ddfd29debe07e00b1437f263a9a802498e07c4185
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
    "id": 10,
    "user_id": 550,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-26T19:32:02.480Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/10/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3912c1a86d246c691bca974ddfd29debe07e00b1437f263a9a802498e07c4185"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/fix
Content-Type: application/json
Authorization: Bearer 5dfe49ca19b2f3034b6aaac4b3a91361c2ac660307afbd13ad0ec32f82224468
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
    "id": 16,
    "user_id": 582,
    "feedbackable_id": 52,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-26T19:32:04.059Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/16/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5dfe49ca19b2f3034b6aaac4b3a91361c2ac660307afbd13ad0ec32f82224468"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/13
Content-Type: application/json
Authorization: Bearer 16064762b1704dba6a76f81b7d6839dab043f3047aa38b33f37fa9b45313d061
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
    "id": 13,
    "user_id": 565,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:32:03.278Z",
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
curl "api.goskive.com/v2/feedbacks/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16064762b1704dba6a76f81b7d6839dab043f3047aa38b33f37fa9b45313d061"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/close
Content-Type: application/json
Authorization: Bearer 4265b45632ce4eb8649edbfe4aae20912e0ca51038179214ec8400136b58b336
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
curl "api.goskive.com/v2/feedbacks/12/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4265b45632ce4eb8649edbfe4aae20912e0ca51038179214ec8400136b58b336"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/17/fix
Content-Type: application/json
Authorization: Bearer 9540b4e8d9a67baca00a6c253c9ae7621e0c452c5affdbda3f4130c8de413476
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
curl "api.goskive.com/v2/feedbacks/17/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9540b4e8d9a67baca00a6c253c9ae7621e0c452c5affdbda3f4130c8de413476"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/18/fix
Content-Type: application/json
Authorization: Bearer e678b6bfd6352c5d3797692c4d051d7ebe643ee3ec806bc7521979db1217e146
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
curl "api.goskive.com/v2/feedbacks/18/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e678b6bfd6352c5d3797692c4d051d7ebe643ee3ec806bc7521979db1217e146"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/14
Content-Type: application/json
Authorization: Bearer 84d10efc52da71671303f1858872c8b513cacfe10817ab3e49fe0a583de553de
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
    "id": 14,
    "user_id": 570,
    "feedbackable_id": 50,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:32:03.535Z",
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
curl "api.goskive.com/v2/feedbacks/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84d10efc52da71671303f1858872c8b513cacfe10817ab3e49fe0a583de553de"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer 141665e80c587e2582f26f6d6e00e8ae81449806684b6cb37cb2c9114184ac20
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
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 141665e80c587e2582f26f6d6e00e8ae81449806684b6cb37cb2c9114184ac20"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/9/bookmark
Content-Type: application/json
Authorization: Bearer ce2c314cdb3352c3bb30917ad4996403a4b935508b1413811480d632636ca6a3
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/9/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce2c314cdb3352c3bb30917ad4996403a4b935508b1413811480d632636ca6a3"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer b1b6528c0fa1b22aadbe22fda520c47c8e37f1ddfb8ba662b382425ec802240a
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1b6528c0fa1b22aadbe22fda520c47c8e37f1ddfb8ba662b382425ec802240a"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer 6786d441da05bb7eb4265ca6517cb264f59647ba9d8af31625e0f40154356625
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/61ac7a9bcee3dce0055c9ed434f0a279.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T193156Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=da4b1a521acd50c2abb3c66952b871124af0dd79068a017a1c4a827faf8b1d16",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6786d441da05bb7eb4265ca6517cb264f59647ba9d8af31625e0f40154356625"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/15/preview
Content-Type: application/json
Authorization: Bearer 6cd3744b495a1c345505414ed20957cd3f60800fd78bde1acd32b3af1a8350be
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/13bdc54a983d93baf09c3b272e4f90a7.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T193156Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ccce48700d1c56f511313e8649dc20fe44e5319881fb7acd0a5f36de02d2142d",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/15/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cd3744b495a1c345505414ed20957cd3f60800fd78bde1acd32b3af1a8350be"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 46f82574ecfa8c587918f8972166b1436bd0d586e0125b7e366bd21a59bb5d51
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
    "id": 14,
    "uploader": {
      "id": 477,
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
      "created_at": "2016-10-26T19:31:56.754Z",
      "updated_at": "2016-10-26T19:31:56.754Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-26T19:31:56.821Z",
    "updated_at": "2016-10-26T19:31:56.821Z",
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
curl "api.goskive.com/v2/files/14/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46f82574ecfa8c587918f8972166b1436bd0d586e0125b7e366bd21a59bb5d51"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/17/matched_courses?required_cu_count=2
Authorization: Bearer 235522ff5f6fd011d1c2810491e7a6dc59238eb11ff1f6378601fe603e2eed9d
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
      "creator_id": 534,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 174,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 180,
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
      "chapters_updated_at": "2016-10-26T19:32:00.141Z",
      "updated_at": "2016-10-26T19:32:01.656Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 539,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-df7df360-41ef-405a-aa00-b8bec1d74b6b",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-df7df360-41ef-405a-aa00-b8bec1d74b6b",
      "slug": "mit-the-great-british-bake-off-df7df360-41ef-405a-aa00-b8bec1d74b6b",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 181,
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
      "chapters_updated_at": "2016-10-26T19:32:00.141Z",
      "updated_at": "2016-10-26T19:32:02.199Z",
      "shortname": "mit-the-great-british-bake-off-df7df360-41ef-405a-aa00-b8bec1d74b6b"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/17/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 235522ff5f6fd011d1c2810491e7a6dc59238eb11ff1f6378601fe603e2eed9d"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 36358a846ed606ce6beb22abee5ad13bceedc1ae8b824c66394d05f8dcb9c87a
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36358a846ed606ce6beb22abee5ad13bceedc1ae8b824c66394d05f8dcb9c87a"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/5/bookmark
Content-Type: application/json
Authorization: Bearer 64cfe28ef1ddedbe54b7cea39c8634dab4a3208ee1296bb70441462988a76645
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
	-H "Authorization: Bearer 64cfe28ef1ddedbe54b7cea39c8634dab4a3208ee1296bb70441462988a76645"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/59/comments
Content-Type: application/json
Authorization: Bearer c9f0ca38eac606cd21a6db35008b3b053060f95f75d03f847f1b1708a6fc2fb0
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
    "id": 55,
    "author_id": 703,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:32:12.433Z",
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
curl "api.goskive.com/v2/flashcards/59/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9f0ca38eac606cd21a6db35008b3b053060f95f75d03f847f1b1708a6fc2fb0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/58/comments
Content-Type: application/json
Authorization: Bearer 278e53f99519255dd34d5a4d62cc19cc8c1bd6d0b42c1edb3572e1b7cc7f6075
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
    "id": 54,
    "author_id": 700,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:32:12.141Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 700,
      "feedbackable_id": 58,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:12.138Z",
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
	-H "Authorization: Bearer 278e53f99519255dd34d5a4d62cc19cc8c1bd6d0b42c1edb3572e1b7cc7f6075"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/55/comments
Content-Type: application/json
Authorization: Bearer 0461e656ebb344ef084bbc25d3bd9d428f91d79c09a05082bd302b307a2c38e5
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
      "id": 53,
      "author_id": 693,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:32:11.628Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 692,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:32:11.613Z",
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
	-H "Authorization: Bearer 0461e656ebb344ef084bbc25d3bd9d428f91d79c09a05082bd302b307a2c38e5"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/57/comments
Content-Type: application/json
Authorization: Bearer 4eba572a8d8a519d4b4c769218437d082d62649a7dbf8c5c0acaac56593763ce
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
curl "api.goskive.com/v2/flashcards/57/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eba572a8d8a519d4b4c769218437d082d62649a7dbf8c5c0acaac56593763ce"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/89/feedbacks
Content-Type: application/json
Authorization: Bearer 23366bc26788433ca95c3e9c22ec39c0eb3eae18c55e2a72c3ec30f44f36c5b5
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
    "user_id": 943,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:32:31.205Z",
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
curl "api.goskive.com/v2/flashcards/89/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23366bc26788433ca95c3e9c22ec39c0eb3eae18c55e2a72c3ec30f44f36c5b5"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/92/feedbacks
Content-Type: application/json
Authorization: Bearer 8941cc0647ba9f1532d613a565ce34a00cb606a05c9053ed1b6c7c008e98e744
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
      "id": 44,
      "user_id": 958,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:31.870Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 957,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:32:31.859Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/92/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8941cc0647ba9f1532d613a565ce34a00cb606a05c9053ed1b6c7c008e98e744"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/7/votes
Content-Type: application/json
Authorization: Bearer c956af50cdfbfb0c30c2cdeb1d53ac4e21766dda0c14ef82eb29a2f6741964b4
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
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 7,
      "user_id": 232
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 7,
      "user_id": 231
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 7,
      "user_id": 230
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/7/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c956af50cdfbfb0c30c2cdeb1d53ac4e21766dda0c14ef82eb29a2f6741964b4"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/62/republish
Content-Type: application/json
Authorization: Bearer abb01d145ab85481860138abb359b7c5fb28319ba58f1911cf4d922990b00e91
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
curl "api.goskive.com/v2/flashcards/62/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abb01d145ab85481860138abb359b7c5fb28319ba58f1911cf4d922990b00e91"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/66/bookmark
Content-Type: application/json
Authorization: Bearer 03b2613d4ec55fdb0f590de7b8c992a988714e5d0393e400d8bb26fc57f68888
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03b2613d4ec55fdb0f590de7b8c992a988714e5d0393e400d8bb26fc57f68888"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/61
Content-Type: application/json
Authorization: Bearer 6da915d789c5295a4a5f540fb3de68d938d3dc2ca24afb02a4ff1d0109995dc6
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6da915d789c5295a4a5f540fb3de68d938d3dc2ca24afb02a4ff1d0109995dc6"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/60/downvote
Content-Type: application/json
Authorization: Bearer 889269658c620c7de5bdd959e26a1e6ea848ddbf49b2ae61652abd91aa850a0b
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/60/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 889269658c620c7de5bdd959e26a1e6ea848ddbf49b2ae61652abd91aa850a0b"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/64
Content-Type: application/json
Authorization: Bearer 6fed1ee7f92cf9b32f8b449d114dbdde7a84c0721f20301909464e6a5ade484e
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
    "id": 64,
    "obfuscated_id": "H-V851w7HZg",
    "author_id": 718,
    "chapter_id": 134,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:32:13.375Z",
    "created_at": "2016-10-26T19:32:13.375Z",
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
curl "api.goskive.com/v2/flashcards/64" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fed1ee7f92cf9b32f8b449d114dbdde7a84c0721f20301909464e6a5ade484e"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/83/report
Content-Type: application/json
Authorization: Bearer b750f7145432da298d85df082ff899fa8b8129b50b02a1b38db00d95bee2ea8a
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/83/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b750f7145432da298d85df082ff899fa8b8129b50b02a1b38db00d95bee2ea8a"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/82/bookmark
Content-Type: application/json
Authorization: Bearer 2dc85fe04a5004b8de4fff2208b7b39348aab3a54919ab93d75124a0c704d7c2
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/82/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dc85fe04a5004b8de4fff2208b7b39348aab3a54919ab93d75124a0c704d7c2"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/upvote
Content-Type: application/json
Authorization: Bearer 1227a5b24dfb9bc23ef94ae7f0f94edc69d47adccd32c75c0d416026fba0de65
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1227a5b24dfb9bc23ef94ae7f0f94edc69d47adccd32c75c0d416026fba0de65"
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
    "key": "cache/4640c6cab8b769d28599342e39015cd6.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQyMDozMTo0NFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzQ2NDBjNmNhYjhiNzY5ZDI4NTk5MzQyZTM5MDE1Y2Q2LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjZUMTkzMTQ0WiJ9XX0=",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T193144Z",
    "x-amz-signature": "8b238fc0d6af9b0631f7d032c13cee0d1e1fd358a71f79b95f00e4736890e132"
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
Authorization: Bearer 6e077f2fa293f74a344d18df55ff59f474102d9326e1f8fdefbd47251208f58f
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
	-H "Authorization: Bearer 6e077f2fa293f74a344d18df55ff59f474102d9326e1f8fdefbd47251208f58f"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer eed85d533d22cd35b16b1903cfe88b10a989781bda33dfac5cc17c1a4bf0c42e
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
	-H "Authorization: Bearer eed85d533d22cd35b16b1903cfe88b10a989781bda33dfac5cc17c1a4bf0c42e"
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
{"password":{"reset_password_token":"rnGTYtsMDprRUSkhR5UQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 3,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-26T19:31:19.597Z",
  "updated_at": "2016-10-26T19:31:19.981Z",
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
  "audit_id": 2929
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"rnGTYtsMDprRUSkhR5UQ","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/20/comments
Content-Type: application/json
Authorization: Bearer bc5efcd8760577203b747cd03b9752cfd4e1b0bfb3041b8eb277603900a02beb
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
    "id": 45,
    "author_id": 239,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:31:36.958Z",
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
curl "api.goskive.com/v2/questions/20/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc5efcd8760577203b747cd03b9752cfd4e1b0bfb3041b8eb277603900a02beb"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/21/comments
Content-Type: application/json
Authorization: Bearer 5215eeb7d5dfb718718b3b7347edf98393d579c20f3dcdfe63c52652f80a1352
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
    "id": 46,
    "author_id": 242,
    "reply_to_id": null,
    "created_at": "2016-10-26T19:31:37.390Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 242,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:31:37.386Z",
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
curl "api.goskive.com/v2/questions/21/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5215eeb7d5dfb718718b3b7347edf98393d579c20f3dcdfe63c52652f80a1352"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/23/comments
Content-Type: application/json
Authorization: Bearer ad0ee64a42441ee802cfefc5a48a0ad2e7518a6a31afcda580a8f445b7e4bb2a
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
      "author_id": 251,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:38.087Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 252,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:31:38.101Z",
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
curl "api.goskive.com/v2/questions/23/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad0ee64a42441ee802cfefc5a48a0ad2e7518a6a31afcda580a8f445b7e4bb2a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/19/comments
Content-Type: application/json
Authorization: Bearer 68959c749754b7517dca2228cbf519affe7b1b201bc58e7647b39191be7502a1
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
curl "api.goskive.com/v2/questions/19/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68959c749754b7517dca2228cbf519affe7b1b201bc58e7647b39191be7502a1"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/72/feedbacks
Content-Type: application/json
Authorization: Bearer 9505ebcbeebbf91823afff8d2ba4e2184b3e9ca8008e88e46f0cda7a2bfb7d6c
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
    "id": 8,
    "user_id": 515,
    "feedbackable_id": 72,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-26T19:31:59.443Z",
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
curl "api.goskive.com/v2/questions/72/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9505ebcbeebbf91823afff8d2ba4e2184b3e9ca8008e88e46f0cda7a2bfb7d6c"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/67/feedbacks
Content-Type: application/json
Authorization: Bearer 4a352bd891838f0a1cd3c97f493109490297a8b8c35284f7de443647ffe72c33
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
      "id": 3,
      "user_id": 492,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:31:57.823Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 491,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:31:57.813Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/67/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a352bd891838f0a1cd3c97f493109490297a8b8c35284f7de443647ffe72c33"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/16/votes
Content-Type: application/json
Authorization: Bearer c0880a01fbf6c5263ea6e2d2c176cbf74b77807dce609b0583feb75d107ae9bc
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
      "votable_id": 16,
      "user_id": 91
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 16,
      "user_id": 90
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 16,
      "user_id": 89
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/16/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0880a01fbf6c5263ea6e2d2c176cbf74b77807dce609b0583feb75d107ae9bc"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/112/republish
Content-Type: application/json
Authorization: Bearer 133a1f98ba7e6c72419bfceacd3b999e7de9bf11a2c4dab35ecacee07788b5d4
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
curl "api.goskive.com/v2/questions/112/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 133a1f98ba7e6c72419bfceacd3b999e7de9bf11a2c4dab35ecacee07788b5d4"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/132/bookmark
Content-Type: application/json
Authorization: Bearer 29b86028e3d26c933401422478c4366fb726efcfd2d393df1bb10307bec25391
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/132/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29b86028e3d26c933401422478c4366fb726efcfd2d393df1bb10307bec25391"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/114
Content-Type: application/json
Authorization: Bearer 588fd7ef281dbf56ee439445fa0236de4217eaf5e452bc427afb4c10f377ba39
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 588fd7ef281dbf56ee439445fa0236de4217eaf5e452bc427afb4c10f377ba39"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/134/downvote
Content-Type: application/json
Authorization: Bearer 9f82bc2e3fdeb3e54abefbe5ed7e2eb7bd9264ca55fd127591ae25f7fce77fc2
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/134/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f82bc2e3fdeb3e54abefbe5ed7e2eb7bd9264ca55fd127591ae25f7fce77fc2"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/113
Content-Type: application/json
Authorization: Bearer 83cb14f8d6798593193327115d376ae3759c6977db9cc2342ec0ae6005ac8fe5
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
    "id": 113,
    "obfuscated_id": "pcyz_ZHBlMU",
    "author_id": 869,
    "chapter_id": 166,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:32:23.849Z",
    "created_at": "2016-10-26T19:32:23.737Z",
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
        "id": 228,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 229,
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
curl "api.goskive.com/v2/questions/113" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83cb14f8d6798593193327115d376ae3759c6977db9cc2342ec0ae6005ac8fe5"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/133/report
Content-Type: application/json
Authorization: Bearer 3ee117c2dea4d6546934bdf613f1d045bc76e2ba5c0a6c366f3688404353f1e3
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/133/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ee117c2dea4d6546934bdf613f1d045bc76e2ba5c0a6c366f3688404353f1e3"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/115/bookmark
Content-Type: application/json
Authorization: Bearer f8a8a0b420c0061198dad7b1b5c4e943dbf589b025c41ec2eaf32732aec2008b
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8a8a0b420c0061198dad7b1b5c4e943dbf589b025c41ec2eaf32732aec2008b"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/131
Content-Type: application/json
Authorization: Bearer 84689ac2dc1ffb3c5a55912afbca67019db2e8c8bf39e9f1319d9d5065a3a28e
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":131,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T19:32:29.229Z","updated_at":"2016-10-26T19:32:29.342Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":184,"author_id":928,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 131,
    "obfuscated_id": "gCw8isdgMKE",
    "author_id": 928,
    "chapter_id": 184,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T19:32:29.446Z",
    "created_at": "2016-10-26T19:32:29.229Z",
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
    "question": "{\"id\"=>131, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-26T19:32:29.229Z\", \"updated_at\"=>\"2016-10-26T19:32:29.342Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>184, \"author_id\"=>928, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 264,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 265,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 266,
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
curl "api.goskive.com/v2/questions/131" -d '{"question":{"question":{"id":131,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T19:32:29.229Z","updated_at":"2016-10-26T19:32:29.342Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":184,"author_id":928,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84689ac2dc1ffb3c5a55912afbca67019db2e8c8bf39e9f1319d9d5065a3a28e"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/110/upvote
Content-Type: application/json
Authorization: Bearer f5de8728e5c11aefb03f0fff876098cf48f29eb6d7e7a5b6d719c3c751f141c9
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5de8728e5c11aefb03f0fff876098cf48f29eb6d7e7a5b6d719c3c751f141c9"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 2bc2cc1b60a2d4473de41c05c4251d3f082c204f5e60d166ef8411f3d9c2758a
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
      "creator_id": 220,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "topic_id": 81,
      "discipline_id": 81,
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
      "updated_at": "2016-10-26T19:31:35.261Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bc2cc1b60a2d4473de41c05c4251d3f082c204f5e60d166ef8411f3d9c2758a"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer accd19454f9a54f7655a8e3cf5f2d97f49d3bb7578f43aafc70eea9e6145d9cb
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
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-75",
      "html_url": "https://goskive.com/university/uni-75",
      "slug": "uni-75",
      "name": "National School of Pizza",
      "short_name": "Uni 75",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2f8af7cfd34b79907d70212c94decefc62b88ac5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8c7d639ffdd2f7c4104668f024cac41bcabf5f59.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:31:35.430Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-74",
      "html_url": "https://goskive.com/university/uni-74",
      "slug": "uni-74",
      "name": "National School of Pastry",
      "short_name": "Uni 74",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cb2a218358d44a5056fe2e55e738cd09577c8a5c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b5ad29aed1943ad0d14839f7d56c62a22a0b6452.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:31:35.415Z",
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
	-H "Authorization: Bearer accd19454f9a54f7655a8e3cf5f2d97f49d3bb7578f43aafc70eea9e6145d9cb"
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
      "id": 31,
      "name": "Right-sized content-based focus group",
      "name_translations": {
        "en": "Right-sized content-based focus group"
      },
      "discipline_id": 31
    },
    {
      "id": 32,
      "name": "Adaptive 5th generation structure",
      "name_translations": {
        "en": "Adaptive 5th generation structure"
      },
      "discipline_id": 32
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
GET /v2/topics/30
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
    "id": 30,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 30
  }
}
```



```shell
curl "api.goskive.com/v2/topics/30" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 13471384c85222d249a4f243d8cfc4c4001acedc715336aa548f5980825ba3cd
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
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-114",
      "html_url": "https://goskive.com/university/uni-114",
      "slug": "uni-114",
      "name": "University 81",
      "short_name": "Uni 114",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2dc4c4be71f6370d25534de80e196fcd34c1c4e7.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/32738d47df494288ae89963c215b73c487fa2655.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:31:44.480Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-113",
      "html_url": "https://goskive.com/university/uni-113",
      "slug": "uni-113",
      "name": "University 80",
      "short_name": "Uni 113",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c81a8aee7b08da0c8fa2e528a434d06f079b9f35.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d9bc74d3abf8eee0a816b125076abff2b517b77b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:31:44.464Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-112",
      "html_url": "https://goskive.com/university/uni-112",
      "slug": "uni-112",
      "name": "University 79",
      "short_name": "Uni 112",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/226077c8a53a441f63f708cc445f0e8b8c0c0785.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2f9b3edea5422a0b21c56f310f6f46844af3f1b2.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T19:31:44.448Z",
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
	-H "Authorization: Bearer 13471384c85222d249a4f243d8cfc4c4001acedc715336aa548f5980825ba3cd"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 023bd21b547ed52349ef6aee82e0f9bd7e2785569b6fd6389af709bbe2cc1bef
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
    "id": 113,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0094eccb9bd9629a76a147d9a37af3a72de4f83e.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/113ce34c1f4ce8c6241d9ab1a97426bd39d1712c.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-26T19:31:44.393Z",
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
	-H "Authorization: Bearer 023bd21b547ed52349ef6aee82e0f9bd7e2785569b6fd6389af709bbe2cc1bef"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 83fd57a05bbfa44ceb0c488bff5ab04f9b7bbbb47b93d79e932bc5dae86bf40e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":281,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 826,
    "id": 269,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 254,
    "additional_university_ids": [

    ],
    "topic_id": 281,
    "discipline_id": 282,
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
    "chapters_updated_at": "2016-10-26T19:32:20.014Z",
    "updated_at": "2016-10-26T19:32:20.136Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 158,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-26T19:32:20.096Z",
        "course_id": 269,
        "author_id": 826,
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
        "id": 159,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-26T19:32:20.112Z",
        "course_id": 269,
        "author_id": 826,
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
        "id": 160,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-26T19:32:20.127Z",
        "course_id": 269,
        "author_id": 826,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":281,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83fd57a05bbfa44ceb0c488bff5ab04f9b7bbbb47b93d79e932bc5dae86bf40e"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 85da09060a5ba0917d2f6d09e8b8d5f06ffb62b4c7a231369f9b30d4148632b5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":280,"published":false}}
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
    "creator_id": 825,
    "id": 268,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 253,
    "additional_university_ids": [

    ],
    "topic_id": 280,
    "discipline_id": 281,
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
    "updated_at": "2016-10-26T19:32:19.981Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":280,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85da09060a5ba0917d2f6d09e8b8d5f06ffb62b4c7a231369f9b30d4148632b5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f65f566b4d1107310c29586c48f71a63d3c4bdb3fab2742c47081a21f420c4c5
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
      "creator_id": 788,
      "id": 237,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-175",
      "html_url": "https://goskive.com/course/fu-course-175",
      "slug": "fu-course-175",
      "university_id": 240,
      "additional_university_ids": [

      ],
      "topic_id": 249,
      "discipline_id": 250,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
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
      "updated_at": "2016-10-26T19:32:16.774Z",
      "shortname": "fu-course-175"
    },
    {
      "creator_id": 788,
      "id": 238,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 240,
      "additional_university_ids": [

      ],
      "topic_id": 250,
      "discipline_id": 251,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "chapters_updated_at": "2016-10-26T19:32:17.079Z",
      "updated_at": "2016-10-26T19:32:17.085Z",
      "shortname": "fu-course-176"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f65f566b4d1107310c29586c48f71a63d3c4bdb3fab2742c47081a21f420c4c5"
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
      "creator_id": 808,
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 246,
      "additional_university_ids": [

      ],
      "topic_id": 265,
      "discipline_id": 266,
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
      "updated_at": "2016-10-26T19:32:18.417Z",
      "shortname": "fu-course-191"
    },
    {
      "creator_id": 808,
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 246,
      "additional_university_ids": [

      ],
      "topic_id": 266,
      "discipline_id": 267,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
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
      "chapters_updated_at": "2016-10-26T19:32:18.719Z",
      "updated_at": "2016-10-26T19:32:18.725Z",
      "shortname": "fu-course-192"
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
Authorization: Bearer 7337f2eddd9c8966f7612ffd6459ddf148af56f8e14512c29f83d23f4afb8665
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
      "creator_id": 795,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-179",
      "html_url": "https://goskive.com/course/fu-course-179",
      "slug": "fu-course-179",
      "university_id": 242,
      "additional_university_ids": [

      ],
      "topic_id": 253,
      "discipline_id": 254,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
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
      "updated_at": "2016-10-26T19:32:17.352Z",
      "shortname": "fu-course-179"
    },
    {
      "creator_id": 795,
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-180",
      "html_url": "https://goskive.com/course/fu-course-180",
      "slug": "fu-course-180",
      "university_id": 242,
      "additional_university_ids": [

      ],
      "topic_id": 254,
      "discipline_id": 255,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 180",
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
      "updated_at": "2016-10-26T19:32:17.389Z",
      "shortname": "fu-course-180"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7337f2eddd9c8966f7612ffd6459ddf148af56f8e14512c29f83d23f4afb8665"
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
      "creator_id": 813,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 248,
      "additional_university_ids": [

      ],
      "topic_id": 269,
      "discipline_id": 270,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
      "updated_at": "2016-10-26T19:32:18.928Z",
      "shortname": "fu-course-195"
    },
    {
      "creator_id": 813,
      "id": 258,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 248,
      "additional_university_ids": [

      ],
      "topic_id": 270,
      "discipline_id": 271,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
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
      "updated_at": "2016-10-26T19:32:18.965Z",
      "shortname": "fu-course-196"
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
Authorization: Bearer c5908b12234ad3b3782791639ec5e7bb7ade80c26ae476a5904302a0171b0de9
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
  "id": 70,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-26T19:31:27.263Z",
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
	-H "Authorization: Bearer c5908b12234ad3b3782791639ec5e7bb7ade80c26ae476a5904302a0171b0de9"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/255
Content-Type: application/json
Authorization: Bearer be49335b4bc99f3903c2069dc1b742c125f0f8d7118c2024e4725677504fe063
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
    "id": 255,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 85,
    "fields_of_study": [
      92,
      93
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-26T19:31:38.289Z",
    "updated_at": "2016-10-26T19:31:38.289Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/255" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be49335b4bc99f3903c2069dc1b742c125f0f8d7118c2024e4725677504fe063"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/253
Content-Type: application/json
Authorization: Bearer b409da7e1524b60a7f19ef88995c93d70001069c8391ee6e683691d22cf16dab
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
    "id": 253,
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
    "created_at": "2016-10-26T19:31:38.143Z",
    "updated_at": "2016-10-26T19:31:38.143Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/253" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b409da7e1524b60a7f19ef88995c93d70001069c8391ee6e683691d22cf16dab"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/13
Content-Type: application/json
Authorization: Bearer 528588c3be75af9ecd8ce0dea78e35cee92cfc8d2c7bd8229341d35281a2c47b
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 528588c3be75af9ecd8ce0dea78e35cee92cfc8d2c7bd8229341d35281a2c47b"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer b5a18d23e05f02c10c6ba3d7044bc775f52dd2a3ccbe56240cc32d92ee045b48
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
    "votable_id": 26,
    "user_id": 265
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5a18d23e05f02c10c6ba3d7044bc775f52dd2a3ccbe56240cc32d92ee045b48"
```
