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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"742dfebfd0a5cc77f70da94e74eeaebcbfa5e2bb8619e3f9669b0e6437f956c2","client_secret":"d7ce0001e21f800443f1e6caad78146574876d4335df5069d2533c86fa95b2d7"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"742dfebfd0a5cc77f70da94e74eeaebcbfa5e2bb8619e3f9669b0e6437f956c2","client_secret":"d7ce0001e21f800443f1e6caad78146574876d4335df5069d2533c86fa95b2d7"}' -X POST \
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
Authorization: Basic ODNhZmVjMjRjZmEwMDVmMjhiZGU3NGMyM2QyMDY0MWFlOTYzNjZlMjEyMzJm
MjNmZjBjZDljOGYwNjIxYjI5ZDo0YmFmYmI4ZTc1NTU2NmQyZmUyMjc0ZTY3
ZDE0MGIyNGY2MzA4OGM0ZjZjNjBiODU0YmM0YzRkMGZmZjljY2Uz

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
	-u 83afec24cfa005f28bde74c23d20641ae96366e21232f23ff0cd9c8f0621b29d:4bafbb8e755566d2fe2274e67d140b24f63088c4f6c60b854bc4c4d0fff9cce3
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
{"grant_type":"client_credentials","client_id":"f5cc9cbc10323a54ecd3e82e6881f146377d17130e806d08fa766fe18bea4bf2","client_secret":"361b0e7246404737b32e7517b6720ab173cd8ff4c30cc19214b96933c14b7895"}
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
  "access_token": "abf5374cf35433023f1c215a4f6e5f2fc5ef37c63a21a4b70ab293e0ab0d22b9",
  "token_type": "bearer",
  "created_at": 1478697870
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"f5cc9cbc10323a54ecd3e82e6881f146377d17130e806d08fa766fe18bea4bf2","client_secret":"361b0e7246404737b32e7517b6720ab173cd8ff4c30cc19214b96933c14b7895"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"b9c9c4687897690f9c9bf91d7d55a1fef79ccdeab41df5652d50ab5ce9227dd4","client_secret":"b5185478a509414c49fde0451ed65657aae22613fba383782c026d10f0d997c3"}
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
  "access_token": "f0cd2d23e1b942a00de52f775741c03bd6415246293c41685ca38647664aa58f",
  "token_type": "bearer",
  "created_at": 1478697870
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"b9c9c4687897690f9c9bf91d7d55a1fef79ccdeab41df5652d50ab5ce9227dd4","client_secret":"b5185478a509414c49fde0451ed65657aae22613fba383782c026d10f0d997c3"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MWI0Mzk0MDI2ZDcyZmI4NTY1ZTg0NGE0ZDMwOGY5NDE0ZTQzNmU1MDJkZjJj
NTc2NGUwMGIyY2VmNDljMzM2YTpiMWQ1ZTQwYmI3YWYyYTRjODc0MTE0ZmI4
Njg4MDg0ZTI5OTY3YmY1NWFjNzJmNWQxM2RlNzQ4Y2E5NGY5YjY4

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
  "access_token": "d380b4df7faf408306e538e576e83a53d9351530d84a4425a6730af25bf00769",
  "token_type": "bearer",
  "created_at": 1478697871
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 1b4394026d72fb8565e844a4d308f9414e436e502df2c5764e00b2cef49c336a:b1d5e40bb7af2a4c874114fb8688084e29967bf55ac72f5d13de748ca94f9b68
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
Authorization: Bearer e96028393a44992a53332f94c6990b58f72df8879981bcc7930574a5c5d4c1f5
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
    "company_id": 36,
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
	-H "Authorization: Bearer e96028393a44992a53332f94c6990b58f72df8879981bcc7930574a5c5d4c1f5"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/165/flashcards
Content-Type: application/json
Authorization: Bearer c8313a512016dd7801f3e118abda331bde1d92bec7dcffaea98e980c4eb3af8e
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":165,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 71,
    "obfuscated_id": "--JhLc6KEBw",
    "author_id": 888,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:24:36.502Z",
    "created_at": "2016-11-09T13:24:36.502Z",
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
curl "api.goskive.com/v2/chapters/165/flashcards" -d '{"flashcard":{"chapter_id":165,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8313a512016dd7801f3e118abda331bde1d92bec7dcffaea98e980c4eb3af8e"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/164/flashcards
Content-Type: application/json
Authorization: Bearer b13cbaed2de5f44b5ba02777cff83f72ee6705267d6dfee7383bee8f75f6d2ec
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 883,
      "chapter_id": 164,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:36.197Z",
      "created_at": "2016-11-09T13:24:36.197Z",
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
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 883,
      "chapter_id": 164,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:36.239Z",
      "created_at": "2016-11-09T13:24:36.239Z",
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
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 883,
      "chapter_id": 164,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:24:36.279Z",
      "created_at": "2016-11-09T13:24:36.279Z",
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
curl "api.goskive.com/v2/chapters/164/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b13cbaed2de5f44b5ba02777cff83f72ee6705267d6dfee7383bee8f75f6d2ec"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/37/questions
Content-Type: application/json
Authorization: Bearer 0cfd28d9b702703a176d71602eb9c7c2a8bff507002396368c2ac771cef27feb
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":37,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 35,
    "obfuscated_id": "soCS52BooV0",
    "author_id": 138,
    "chapter_id": 37,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:31.570Z",
    "created_at": "2016-11-09T13:23:31.570Z",
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
        "id": 71,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 72,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 73,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 74,
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
curl "api.goskive.com/v2/chapters/37/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":37,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cfd28d9b702703a176d71602eb9c7c2a8bff507002396368c2ac771cef27feb"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/36/questions
Content-Type: application/json
Authorization: Bearer 39b156d6b5375fc58a36cfd35d43d966af6df7b814b05a3544b5358c5f895a6e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 34,
    "obfuscated_id": "LRSQf_NrQzE",
    "author_id": 135,
    "chapter_id": 36,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:30.975Z",
    "created_at": "2016-11-09T13:23:30.975Z",
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
        "id": 69,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 70,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/36/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39b156d6b5375fc58a36cfd35d43d966af6df7b814b05a3544b5358c5f895a6e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/38/questions
Content-Type: application/json
Authorization: Bearer 8432a56016efc0a68153e80ee66e053e1a841585e954545d7ab5ac0a66bc6cd0
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 36,
    "obfuscated_id": "01Tx8eTrCOA",
    "author_id": 141,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:32.337Z",
    "created_at": "2016-11-09T13:23:32.337Z",
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
        "id": 75,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 76,
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
curl "api.goskive.com/v2/chapters/38/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8432a56016efc0a68153e80ee66e053e1a841585e954545d7ab5ac0a66bc6cd0"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/35/questions
Content-Type: application/json
Authorization: Bearer c31b4a4e3d699abedf307fd38d2e6ebd3a4fef1cfa63a6e9e7db7cdcc19578ed
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":35,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 33,
    "obfuscated_id": "sjAD-GXxS8o",
    "author_id": 132,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:30.325Z",
    "created_at": "2016-11-09T13:23:30.325Z",
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
        "id": 66,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 67,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 68,
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
curl "api.goskive.com/v2/chapters/35/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":35,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c31b4a4e3d699abedf307fd38d2e6ebd3a4fef1cfa63a6e9e7db7cdcc19578ed"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/34/questions
Content-Type: application/json
Authorization: Bearer 86bedfac3fd85d097ce224e258c2f35436e6b7389b9a4efab95c58a5f0377a89
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 126,
      "chapter_id": 34,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:29.620Z",
      "created_at": "2016-11-09T13:23:29.485Z",
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
          "id": 60,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 61,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 127,
      "chapter_id": 34,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:29.831Z",
      "created_at": "2016-11-09T13:23:29.699Z",
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
          "id": 62,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 63,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 128,
      "chapter_id": 34,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:23:30.045Z",
      "created_at": "2016-11-09T13:23:29.910Z",
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
          "id": 64,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 65,
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
curl "api.goskive.com/v2/chapters/34/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86bedfac3fd85d097ce224e258c2f35436e6b7389b9a4efab95c58a5f0377a89"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/53
Content-Type: application/json
Authorization: Bearer c58709ccd0bdbcdbd86adb6b371611f6d8c2962458603f465ec0e59be4d4979a
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
curl "api.goskive.com/v2/chapters/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c58709ccd0bdbcdbd86adb6b371611f6d8c2962458603f465ec0e59be4d4979a"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/56
Content-Type: application/json
Authorization: Bearer 62683015275f478eb613e05f331094b9c6150ef55460ded00b60c90b0466d7db
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
curl "api.goskive.com/v2/chapters/56" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62683015275f478eb613e05f331094b9c6150ef55460ded00b60c90b0466d7db"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/58
Content-Type: application/json
Authorization: Bearer 0bb1fc79f75fcb8ff4ed009ecfebcd924ffdbd9b412c0bbe767e839c3b2c89dc
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
curl "api.goskive.com/v2/chapters/58" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bb1fc79f75fcb8ff4ed009ecfebcd924ffdbd9b412c0bbe767e839c3b2c89dc"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/55
Content-Type: application/json
Authorization: Bearer 38089537191d33bbe61e949368e10b3cb338214f95cfff752227e1a2e1c7122d
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38089537191d33bbe61e949368e10b3cb338214f95cfff752227e1a2e1c7122d"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/60
Content-Type: application/json
Authorization: Bearer 726bd2f20e23ce34eeaee97569dd9a9d73ef6eae874a5f628a87658963d44681
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
    "id": 60,
    "updated_at": "2016-11-09T13:23:46.096Z",
    "course_id": 72,
    "author_id": 233,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-09T13:23:45.490Z",
    "questions_updated_at": "2016-11-09T13:23:45.490Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 237,
        "chapter_id": 60,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:46.074Z",
        "created_at": "2016-11-09T13:23:46.074Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 235,
        "chapter_id": 60,
        "position": 55,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:45.956Z",
        "created_at": "2016-11-09T13:23:45.815Z",
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
curl "api.goskive.com/v2/chapters/60" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 726bd2f20e23ce34eeaee97569dd9a9d73ef6eae874a5f628a87658963d44681"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/59
Content-Type: application/json
Authorization: Bearer 8e52a3299d1f0f55f3679c1e95c1d04b1149c2ee5371d086deb4677118df0b78
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
    "id": 59,
    "updated_at": "2016-11-09T13:23:45.413Z",
    "course_id": 71,
    "author_id": 231,
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
curl "api.goskive.com/v2/chapters/59" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e52a3299d1f0f55f3679c1e95c1d04b1149c2ee5371d086deb4677118df0b78"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer dcc8fe1eb6d8a2a7bcaaac34ee2f958c9c0b5f4912df316dca90708ec8f875bf
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
    "id": 2,
    "author_id": 202,
    "reply_to_id": 1,
    "created_at": "2016-11-09T13:23:42.863Z",
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
curl "api.goskive.com/v2/comments/1/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcc8fe1eb6d8a2a7bcaaac34ee2f958c9c0b5f4912df316dca90708ec8f875bf"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 803802679a6e3d26db58676678839c79bff194b8bbfcb8b35b0881955360060c
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
curl "api.goskive.com/v2/comments/3/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 803802679a6e3d26db58676678839c79bff194b8bbfcb8b35b0881955360060c"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/13
Content-Type: application/json
Authorization: Bearer 73a690ca054979d412983da266d555eaec98afd6d91b131665263c7a59f2c884
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
curl "api.goskive.com/v2/comments/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73a690ca054979d412983da266d555eaec98afd6d91b131665263c7a59f2c884"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/10/republish
Content-Type: application/json
Authorization: Bearer d54090e3907f919a2f40cde98308d27c4f4f4cdb82b26fb5188b025141ede827
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
curl "api.goskive.com/v2/comments/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d54090e3907f919a2f40cde98308d27c4f4f4cdb82b26fb5188b025141ede827"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/14
Content-Type: application/json
Authorization: Bearer 69e47e83b3c467b92cbb50a7449e42c4e3546e76540f4982938f224644bf2abc
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69e47e83b3c467b92cbb50a7449e42c4e3546e76540f4982938f224644bf2abc"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/11/report
Content-Type: application/json
Authorization: Bearer b36889e20f484bff2c52f889118d1c617ac82bbe23e42bb0532e8c5d31e4282f
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b36889e20f484bff2c52f889118d1c617ac82bbe23e42bb0532e8c5d31e4282f"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/35
Content-Type: application/json
Authorization: Bearer 604f519981e8a1fe3a69af81e84863f8036e9be351b004023b210971896f0b22
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
    "id": 35,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-09T13:24:14.709Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 604f519981e8a1fe3a69af81e84863f8036e9be351b004023b210971896f0b22"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 3a5652b4f984152f4e8621192b19d60650df1d3dd4259a06391d9c39c003dc2c
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
      "id": 32,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/4827d71e510ab6acd29eb9520c31ac72b53161f6.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T13:24:14.648Z"
    },
    {
      "id": 33,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T13:24:14.653Z"
    },
    {
      "id": 34,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-09T13:24:14.656Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a5652b4f984152f4e8621192b19d60650df1d3dd4259a06391d9c39c003dc2c"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/38/company_profiles
Content-Type: application/json
Authorization: Bearer 3d4326e7553403394f8bd98948c72a26ec85310b4805eb5b58d3eb73f95d776c
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
	-H "Authorization: Bearer 3d4326e7553403394f8bd98948c72a26ec85310b4805eb5b58d3eb73f95d776c"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 9bd0812975d9743f68cc966c3633f4326675ee78b26b00ee66d53ab06c121e9f
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
	-H "Authorization: Bearer 9bd0812975d9743f68cc966c3633f4326675ee78b26b00ee66d53ab06c121e9f"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer cb5c5a3cb3e346b6d078995a9b7876a34a72f52e3d4f3024b907b9064335e0fc
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
	-H "Authorization: Bearer cb5c5a3cb3e346b6d078995a9b7876a34a72f52e3d4f3024b907b9064335e0fc"
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
Authorization: Bearer 7fca3eedd547944de22bb56d5cde1761d703ea1c705c90733d851e744140be9b
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
	-H "Authorization: Bearer 7fca3eedd547944de22bb56d5cde1761d703ea1c705c90733d851e744140be9b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1b1df3677fcad907cf9415a5caac588fca682b075a93d2b323ba9b114ca3fa45
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
    "updated_at": "2016-11-09T13:23:56.965Z",
    "course_id": 105,
    "author_id": 379,
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
	-H "Authorization: Bearer 1b1df3677fcad907cf9415a5caac588fca682b075a93d2b323ba9b114ca3fa45"
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
      "id": 96,
      "updated_at": "2016-11-09T13:23:57.519Z",
      "course_id": 109,
      "author_id": 390,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 78",
      "position": 1
    },
    {
      "id": 97,
      "updated_at": "2016-11-09T13:23:57.543Z",
      "course_id": 109,
      "author_id": 391,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 79",
      "position": 2
    },
    {
      "id": 98,
      "updated_at": "2016-11-09T13:23:57.823Z",
      "course_id": 109,
      "author_id": 392,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-09T13:23:57.447Z",
      "questions_updated_at": "2016-11-09T13:23:57.447Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 80",
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
Authorization: Bearer a3b8f09a470c19c6f2266e3604f215334589baa2947bae77bc206a0603dc6927
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
      "id": 102,
      "updated_at": "2016-11-09T13:23:58.192Z",
      "course_id": 112,
      "author_id": 401,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 84",
      "position": 1
    },
    {
      "id": 103,
      "updated_at": "2016-11-09T13:23:58.216Z",
      "course_id": 112,
      "author_id": 402,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 85",
      "position": 2
    },
    {
      "id": 104,
      "updated_at": "2016-11-09T13:23:58.497Z",
      "course_id": 112,
      "author_id": 403,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-09T13:23:58.119Z",
      "questions_updated_at": "2016-11-09T13:23:58.119Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 86",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3b8f09a470c19c6f2266e3604f215334589baa2947bae77bc206a0603dc6927"
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
      "id": 99,
      "updated_at": "2016-11-09T13:23:57.945Z",
      "course_id": 110,
      "author_id": 396,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 81",
      "position": 1
    },
    {
      "id": 100,
      "updated_at": "2016-11-09T13:23:57.970Z",
      "course_id": 110,
      "author_id": 397,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 82",
      "position": 2
    },
    {
      "id": 101,
      "updated_at": "2016-11-09T13:23:57.995Z",
      "course_id": 110,
      "author_id": 398,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 83",
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
Authorization: Bearer a63624cd2298307769463889d6adbc47f2e3bad18c3e9a585b242c3dd508c6fe
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
      "id": 105,
      "updated_at": "2016-11-09T13:23:58.718Z",
      "course_id": 113,
      "author_id": 408,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 87",
      "position": 1
    },
    {
      "id": 106,
      "updated_at": "2016-11-09T13:23:58.743Z",
      "course_id": 113,
      "author_id": 409,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 88",
      "position": 2
    },
    {
      "id": 107,
      "updated_at": "2016-11-09T13:23:58.768Z",
      "course_id": 113,
      "author_id": 410,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 89",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a63624cd2298307769463889d6adbc47f2e3bad18c3e9a585b242c3dd508c6fe"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 16d5d60ad265f3ea1a8f6d50c2b54331861093ad57839cc38b1d801116e3221e
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
    "course_id": 246,
    "user_id": 765,
    "updated_at": "2016-11-09T13:24:27.753Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16d5d60ad265f3ea1a8f6d50c2b54331861093ad57839cc38b1d801116e3221e"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d74d8e3c86be64711fe22129dbcefde1f65396fe4935b705a0e99c3e1b2fb902
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
      "course_id": 242,
      "user_id": 753,
      "updated_at": "2016-11-09T13:24:27.190Z"
    },
    {
      "id": 3,
      "course_id": 242,
      "user_id": 754,
      "updated_at": "2016-11-09T13:24:27.205Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d74d8e3c86be64711fe22129dbcefde1f65396fe4935b705a0e99c3e1b2fb902"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/31/files
Content-Type: application/json
Authorization: Bearer 15c64414c5116c7076bb12d33969a817062c8fa863919fd1eb1d9f727fdac8f1
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
        "id": 98,
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
        "created_at": "2016-11-09T13:23:26.697Z",
        "updated_at": "2016-11-09T13:23:26.697Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T13:23:26.711Z",
      "updated_at": "2016-11-09T13:23:26.711Z",
      "course_id": 31,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 99,
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
        "created_at": "2016-11-09T13:23:26.719Z",
        "updated_at": "2016-11-09T13:23:26.719Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T13:23:26.729Z",
      "updated_at": "2016-11-09T13:23:26.729Z",
      "course_id": 31,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 100,
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
        "created_at": "2016-11-09T13:23:26.737Z",
        "updated_at": "2016-11-09T13:23:26.737Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-09T13:23:26.746Z",
      "updated_at": "2016-11-09T13:23:26.746Z",
      "course_id": 31,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/31/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15c64414c5116c7076bb12d33969a817062c8fa863919fd1eb1d9f727fdac8f1"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/30/files
Content-Type: application/json
Authorization: Bearer d4a40ec8b7d5321c1bee4a63cc1168889f778c2fb7976654a852e9adbc590f7f
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
      "id": 96,
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
      "created_at": "2016-11-09T13:23:26.426Z",
      "updated_at": "2016-11-09T13:23:26.426Z"
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
    "created_at": "2016-11-09T13:23:26.489Z",
    "updated_at": "2016-11-09T13:23:26.489Z",
    "course_id": 30,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/30/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4a40ec8b7d5321c1bee4a63cc1168889f778c2fb7976654a852e9adbc590f7f"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/29/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer f3b9d4ecac84629919bde87868f39a2b9cd6380da0455ffe5d36e7fc69a055e6
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
    "key": "cache/bf5bf9a9cb255a7de6559bd6b0c0067b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOVQxNDoyMzoyNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2JmNWJmOWE5Y2IyNTVhN2RlNjU1OWJkNmIwYzAwNjdiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDkvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA5VDEzMjMyNloifV19",
    "x-amz-credential": "FAKE/20161109/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161109T132326Z",
    "x-amz-signature": "aea454509c86c797993e20c8641478dae667e1dbd1e6661c33573e2f9ccb27b5"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/29/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3b9d4ecac84629919bde87868f39a2b9cd6380da0455ffe5d36e7fc69a055e6"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 13ab386928b8ca91cd0aa83189f961828d16d63a45c5c2130cfde4f72d77bcb4
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
	-H "Authorization: Bearer 13ab386928b8ca91cd0aa83189f961828d16d63a45c5c2130cfde4f72d77bcb4"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ea9cbd1c49171775fd55d17d789e83289555d8b66d962e4f4f2c0770dafcb467
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
	-H "Authorization: Bearer ea9cbd1c49171775fd55d17d789e83289555d8b66d962e4f4f2c0770dafcb467"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 17b4afc2fea1b3d7fc6f56bee2da0838ddd2f7405efe9fd45b35ebbf2bfac287
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
	-H "Authorization: Bearer 17b4afc2fea1b3d7fc6f56bee2da0838ddd2f7405efe9fd45b35ebbf2bfac287"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cc19b8e4323b5950105292f3b74e58333f186f0e5cbf162e929f9a41074fbb1e
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
	-H "Authorization: Bearer cc19b8e4323b5950105292f3b74e58333f186f0e5cbf162e929f9a41074fbb1e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3b4018847bc09ad832ce59289242e55c46ac98c47daf05886eab942e75c01258
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
	-H "Authorization: Bearer 3b4018847bc09ad832ce59289242e55c46ac98c47daf05886eab942e75c01258"
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
    "creator_id": 148,
    "id": 44,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 44,
    "additional_university_ids": [

    ],
    "discipline_id": 47,
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
    "chapters_updated_at": "2016-11-09T13:23:34.477Z",
    "updated_at": "2016-11-09T13:23:35.968Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 148,
        "chapter_id": 41,
        "position": 30,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:34.710Z",
        "created_at": "2016-11-09T13:23:34.590Z",
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
            "id": 89,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 90,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 148,
        "chapter_id": 42,
        "position": 32,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:35.101Z",
        "created_at": "2016-11-09T13:23:34.971Z",
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
            "id": 93,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 94,
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
        "id": 41,
        "updated_at": "2016-11-09T13:23:35.922Z",
        "course_id": 44,
        "author_id": 148,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T13:23:34.477Z",
        "questions_updated_at": "2016-11-09T13:23:34.477Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 35",
        "position": 1
      },
      {
        "id": 42,
        "updated_at": "2016-11-09T13:23:35.960Z",
        "course_id": 44,
        "author_id": 148,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T13:23:34.477Z",
        "questions_updated_at": "2016-11-09T13:23:34.477Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 36",
        "position": 2
      }
    ],
    "topic_id": 47,
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
Authorization: Bearer a4d5bcf1a59329c187d28d6ae0c1f87b66a46addb30408ca72b713d8ec637adb
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
    "creator_id": 153,
    "id": 45,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 45,
    "additional_university_ids": [

    ],
    "discipline_id": 48,
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
    "chapters_updated_at": "2016-11-09T13:23:36.022Z",
    "updated_at": "2016-11-09T13:23:37.665Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 154,
        "chapter_id": 43,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:37.441Z",
        "created_at": "2016-11-09T13:23:37.441Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 154,
        "chapter_id": 44,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:37.518Z",
        "created_at": "2016-11-09T13:23:37.518Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 154,
        "chapter_id": 43,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:37.485Z",
        "created_at": "2016-11-09T13:23:37.485Z",
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
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 154,
        "chapter_id": 44,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:37.562Z",
        "created_at": "2016-11-09T13:23:37.562Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 154,
        "chapter_id": 43,
        "position": 36,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:36.267Z",
        "created_at": "2016-11-09T13:23:36.136Z",
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
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 154,
        "chapter_id": 43,
        "position": 37,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:36.461Z",
        "created_at": "2016-11-09T13:23:36.336Z",
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
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 154,
        "chapter_id": 44,
        "position": 38,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:36.700Z",
        "created_at": "2016-11-09T13:23:36.557Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 154,
        "chapter_id": 44,
        "position": 39,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:23:36.917Z",
        "created_at": "2016-11-09T13:23:36.778Z",
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
        "id": 43,
        "updated_at": "2016-11-09T13:23:37.615Z",
        "course_id": 45,
        "author_id": 153,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T13:23:36.022Z",
        "questions_updated_at": "2016-11-09T13:23:36.022Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 37",
        "position": 1
      },
      {
        "id": 44,
        "updated_at": "2016-11-09T13:23:37.657Z",
        "course_id": 45,
        "author_id": 153,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-09T13:23:36.022Z",
        "questions_updated_at": "2016-11-09T13:23:36.022Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 38",
        "position": 2
      }
    ],
    "topic_id": 48,
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
	-H "Authorization: Bearer a4d5bcf1a59329c187d28d6ae0c1f87b66a46addb30408ca72b713d8ec637adb"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/51/pin
Content-Type: application/json
Authorization: Bearer ad2b249ac1adcff562cdcdc372cfb5bbbb7a0b26ac90d4e1f8d4b85f1efc2ade
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/51/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad2b249ac1adcff562cdcdc372cfb5bbbb7a0b26ac90d4e1f8d4b85f1efc2ade"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/61/pin
Content-Type: application/json
Authorization: Bearer 617f5b4e39a555e6d0b3122a3e38f08d9223151b1657f6cab12aad14592a8236
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/61/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 617f5b4e39a555e6d0b3122a3e38f08d9223151b1657f6cab12aad14592a8236"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4b25dfe4cd273ed3f52103287eeddcfb6bcc166093d7692083ccba836bbbcf2b
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
    "creator_id": 169,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 49,
    "additional_university_ids": [

    ],
    "discipline_id": 52,
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
    "updated_at": "2016-11-09T13:23:40.035Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 52,
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
	-H "Authorization: Bearer 4b25dfe4cd273ed3f52103287eeddcfb6bcc166093d7692083ccba836bbbcf2b"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 454fcbd83848af08e0aef170dc4fce9ec21d80b00006a08ad4380b44d78d29bc
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
    "id": 442,
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
    "created_at": "2016-11-09T13:24:00.647Z",
    "updated_at": "2016-11-09T13:24:00.647Z",
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
	-H "Authorization: Bearer 454fcbd83848af08e0aef170dc4fce9ec21d80b00006a08ad4380b44d78d29bc"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7556b13b0eb99b72e240ea3fc2491cd3dc1e3af5a65c92d7ba32e46d1cfded9b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[129]}
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
    "id": 443,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      129
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T13:24:00.745Z",
    "updated_at": "2016-11-09T13:24:00.787Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[129]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7556b13b0eb99b72e240ea3fc2491cd3dc1e3af5a65c92d7ba32e46d1cfded9b"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer dfd4c7c342f1ddeedfb2cc2a285c23b329e612449b1da814026fd43e647ce6bd
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
    "id": 445,
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
    "created_at": "2016-11-09T13:24:00.892Z",
    "updated_at": "2016-11-09T13:24:00.892Z",
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
	-H "Authorization: Bearer dfd4c7c342f1ddeedfb2cc2a285c23b329e612449b1da814026fd43e647ce6bd"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7de76c6c302fe5d98e94336dd8d7deef87ac1099e95803c5bf7c038db03b7b4e
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[132]}
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
    "id": 446,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      132
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T13:24:00.994Z",
    "updated_at": "2016-11-09T13:24:00.994Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[132]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7de76c6c302fe5d98e94336dd8d7deef87ac1099e95803c5bf7c038db03b7b4e"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 5a39d4dd3cd06f564a793ed3a6b5f9dd6c9dab4d447b39b84b1ac9e9b6b2f583
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

133
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
    "id": 447,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/8dda378f612321244ad62f9c0caf8d21a4647ca0.jpg",
    "university_id": null,
    "fields_of_study": [
      133
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-09T13:24:01.068Z",
    "updated_at": "2016-11-09T13:24:01.344Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/5d5b5cec27b9defc32cd0fffbbb3ec77df4cb5d1.jpg",
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

133
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 5a39d4dd3cd06f564a793ed3a6b5f9dd6c9dab4d447b39b84b1ac9e9b6b2f583"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer b5c581db65a9311576b585dc5722870b3d614dca1dc119fce308b46e9418c697
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
      "id": 8,
      "bookmarkable_id": 132,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 133,
      "bookmarkable_type": "Question"
    },
    {
      "id": 10,
      "bookmarkable_id": 134,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5c581db65a9311576b585dc5722870b3d614dca1dc119fce308b46e9418c697"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 2867e56c848e8bf32c8ba4b6917b24d41d3c0a5fcba38cf51e58dcfbc609f715
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
      "company_id": 28,
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
      "company_id": 29,
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
	-H "Authorization: Bearer 2867e56c848e8bf32c8ba4b6917b24d41d3c0a5fcba38cf51e58dcfbc609f715"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer c86c2d6754be6efe83a7aafedc2c2719e379366ff2a60749772b1337fa3593ad
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
      "company_id": 24,
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
	-H "Authorization: Bearer c86c2d6754be6efe83a7aafedc2c2719e379366ff2a60749772b1337fa3593ad"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d72b0197ae0d6306788d53639f4c10b4f71d6702f901c1f018b782fc402882e4
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
      "creator_id": 430,
      "id": 118,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-73",
      "html_url": "https://goskive.com/course/mit-course-73",
      "slug": "mit-course-73",
      "university_id": 123,
      "additional_university_ids": [

      ],
      "discipline_id": 124,
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
      "updated_at": "2016-11-09T13:23:59.907Z",
      "shortname": "mit-course-73",
      "topic_id": 123,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 73",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 431,
      "id": 119,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-74",
      "html_url": "https://goskive.com/course/mit-course-74",
      "slug": "mit-course-74",
      "university_id": 124,
      "additional_university_ids": [

      ],
      "discipline_id": 125,
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
      "updated_at": "2016-11-09T13:23:59.990Z",
      "shortname": "mit-course-74",
      "topic_id": 124,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 74",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d72b0197ae0d6306788d53639f4c10b4f71d6702f901c1f018b782fc402882e4"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer d5141b8e4120251ff74d45556410efafb8f8d875fa2d7782d9605f2193b301f0
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
        "created_at": "2016-11-09T13:24:00.122Z",
        "updated_at": "2016-11-09T13:24:00.122Z",
        "file_url": "memory://240ca21c13c045149f8a15b607a9758b.pdf",
        "course_id": 120,
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
        "created_at": "2016-11-09T13:24:00.206Z",
        "updated_at": "2016-11-09T13:24:00.206Z",
        "file_url": "memory://f2c49e72fd2a40dd71a1ebc2df3b3232.pdf",
        "course_id": 121,
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
        "created_at": "2016-11-09T13:24:00.292Z",
        "updated_at": "2016-11-09T13:24:00.292Z",
        "file_url": "memory://6b2f09bb9e2217e55b343a9aa98230f2.pdf",
        "course_id": 122,
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
	-H "Authorization: Bearer d5141b8e4120251ff74d45556410efafb8f8d875fa2d7782d9605f2193b301f0"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 2d176330d08353049f58d4a412deb97867cc44151f304f373b346b26a0566812
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
      "company_id": 9,
      "company": {
        "id": 9,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T13:24:01.623Z"
      },
      "created_at": "2016-11-09T13:24:01.626Z",
      "updated_at": "2016-11-09T13:24:01.626Z",
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T13:24:01.634Z"
      },
      "created_at": "2016-11-09T13:24:01.638Z",
      "updated_at": "2016-11-09T13:24:01.638Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d176330d08353049f58d4a412deb97867cc44151f304f373b346b26a0566812"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer de1e11fc4e04e3a4d3a29b31f7c1e06c1ed2d429948c71f70fb78f431344134c
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
      "company_id": 5,
      "company": {
        "id": 5,
        "name": "Fake Company Name 5",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T13:24:01.401Z"
      },
      "created_at": "2016-11-09T13:24:01.404Z",
      "updated_at": "2016-11-09T13:24:01.404Z",
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-09T13:24:01.420Z"
      },
      "created_at": "2016-11-09T13:24:01.424Z",
      "updated_at": "2016-11-09T13:24:01.424Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de1e11fc4e04e3a4d3a29b31f7c1e06c1ed2d429948c71f70fb78f431344134c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 1f2d129f32f1a77e073a4a23895ed3aefdfbb78b77fa17ee2857f2d5bfbb82b7
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
      "created_at": "2016-11-09T13:24:33.348Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-11-09T13:24:33.463Z",
      "author_id": "849",
      "thread_subject_id": "275",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-11-09T13:24:33.452Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-11-09T13:24:33.467Z",
      "author_id": "852",
      "thread_subject_id": "276",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-11-09T13:24:33.848Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-11-09T13:24:33.848Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-11-09T13:24:34.235Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-09T13:24:34.235Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-11-09T13:24:34.631Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-11-09T13:24:34.631Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-11-09T13:24:34.970Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 126,
      "updated_at": "2016-11-09T13:24:34.970Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-11-09T13:24:35.302Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 127,
      "updated_at": "2016-11-09T13:24:35.302Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-11-09T13:24:35.623Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 128,
      "updated_at": "2016-11-09T13:24:35.623Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f2d129f32f1a77e073a4a23895ed3aefdfbb78b77fa17ee2857f2d5bfbb82b7"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/24
Content-Type: application/json
Authorization: Bearer d68514ce9f824364040a0456f4de3a404e3ee0d4bb546c74ebd54c3cf97631ac
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-09T13:14:35.000Z"}}
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
    "created_at": "2016-11-09T13:24:35.834Z",
    "read_at": "2016-11-09T13:14:35.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 60,
    "updated_at": "2016-11-09T13:24:35.876Z",
    "author_id": "878",
    "thread_subject_id": "283",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/24" -d '{"notification":{"read_at":"2016-11-09T13:14:35.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d68514ce9f824364040a0456f4de3a404e3ee0d4bb546c74ebd54c3cf97631ac"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f3b05c0986fa746b25844a2a0142f2b60199aa5615677da55f21f8294260715a
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
      "id": 6,
      "course_id": 251,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-09T13:24:28.552Z",
      "course_published": true,
      "updated_at": "2016-11-09T13:24:28.544Z"
    },
    {
      "id": 7,
      "course_id": 252,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-09T13:24:28.630Z",
      "course_published": true,
      "updated_at": "2016-11-09T13:24:28.623Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3b05c0986fa746b25844a2a0142f2b60199aa5615677da55f21f8294260715a"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 72586d8449b23b623b1337d81cad7fc884ee86e4efced3e7ee8d2d644da7c244
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
    "course_id": 250,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-09T13:24:28.428Z",
    "course_published": true,
    "updated_at": "2016-11-09T13:24:28.421Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72586d8449b23b623b1337d81cad7fc884ee86e4efced3e7ee8d2d644da7c244"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 6a3e2929f5749ac892b3740ac4328d59193d54f10f5465f3ed2f74535762cd06
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
    "id": 4,
    "course_id": 249,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-09T13:24:28.327Z",
    "course_published": true,
    "updated_at": "2016-11-09T13:24:28.315Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a3e2929f5749ac892b3740ac4328d59193d54f10f5465f3ed2f74535762cd06"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 4fede5d9570ff958f6884e63b737ce1ba918a14bde07fa908c0d47da38ef0b65
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
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 26,
      "user_id": 108
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 27,
      "user_id": 108
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 108
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 29,
      "user_id": 108
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fede5d9570ff958f6884e63b737ce1ba918a14bde07fa908c0d47da38ef0b65"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/79
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
    "id": 79,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 77,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 79
      },
      {
        "id": 78,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 79
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/79" -X GET \
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
      "id": 77,
      "name": "Open-source clear-thinking capability",
      "name_translations": {
        "en": "Open-source clear-thinking capability"
      }
    },
    {
      "id": 78,
      "name": "Function-based object-oriented orchestration",
      "name_translations": {
        "en": "Function-based object-oriented orchestration"
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
Authorization: Bearer d90cb950ccd49bbd52885474cd5eb0b5b3194c5b3b39f1d88cf669e375475876
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
    "user_id": 259,
    "feedbackable_id": 36,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-09T13:23:47.839Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d90cb950ccd49bbd52885474cd5eb0b5b3194c5b3b39f1d88cf669e375475876"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer c93324970c30ef8e32eed6bb280a715adfea7223ec503bed3a51d22f5fcef4c4
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
    "id": 28,
    "user_id": 372,
    "feedbackable_id": 42,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-09T13:23:56.320Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c93324970c30ef8e32eed6bb280a715adfea7223ec503bed3a51d22f5fcef4c4"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/4
Content-Type: application/json
Authorization: Bearer a756b4b927b201586e27ac6ed512dfb48d67a8a72c6857f4d4f1e1e444200a47
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
    "id": 4,
    "user_id": 264,
    "feedbackable_id": 37,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T13:23:48.166Z",
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
curl "api.goskive.com/v2/feedbacks/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a756b4b927b201586e27ac6ed512dfb48d67a8a72c6857f4d4f1e1e444200a47"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer 1d44904cde3d9df94bd001d442bea9db1c702d444eeffcab6d9c1a773327db4d
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
curl "api.goskive.com/v2/feedbacks/1/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d44904cde3d9df94bd001d442bea9db1c702d444eeffcab6d9c1a773327db4d"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 230354a0f75c15e00edcae0dcc427f15b09a897d3dcda2485ea585c7ebcba7e3
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
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 230354a0f75c15e00edcae0dcc427f15b09a897d3dcda2485ea585c7ebcba7e3"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer 6dc06517b74ba68ed3c8a86cf44dd80c73d1f3a6d0f00a68079177e6e82b8e04
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
curl "api.goskive.com/v2/feedbacks/26/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dc06517b74ba68ed3c8a86cf44dd80c73d1f3a6d0f00a68079177e6e82b8e04"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer f401fbe14dad2a912d92caff369ca91bc606c34064e498d60804546a7ecc8c13
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
    "id": 5,
    "user_id": 269,
    "feedbackable_id": 38,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T13:23:48.468Z",
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
curl "api.goskive.com/v2/feedbacks/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f401fbe14dad2a912d92caff369ca91bc606c34064e498d60804546a7ecc8c13"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 9bddc6cd7efcd36ef03e358754c3b7f7614f856ff47217a919e917763bbb4c36
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
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bddc6cd7efcd36ef03e358754c3b7f7614f856ff47217a919e917763bbb4c36"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/21/bookmark
Content-Type: application/json
Authorization: Bearer 35053ddd5ad064909b9d561573bc13d4e4002f95777fc85cbcc99c119ff4f105
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35053ddd5ad064909b9d561573bc13d4e4002f95777fc85cbcc99c119ff4f105"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer f6fbf405e0fc57b8e3a03738f343e1f4d6da2fbbc503de17ce8d95800c507833
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6fbf405e0fc57b8e3a03738f343e1f4d6da2fbbc503de17ce8d95800c507833"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/20
Content-Type: application/json
Authorization: Bearer da6060c42ad7e4d2ecd8e09d3efeb2fd486e1509b2282c22ff79002866268625
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/12240bb81939a873f2f6363441a94fb7.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161109%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161109T132430Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=9de395186ea1fa7aae7f4f0f99d058f6c04a87b5a2f66ed0796aa2a219deb361",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da6060c42ad7e4d2ecd8e09d3efeb2fd486e1509b2282c22ff79002866268625"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/19/preview
Content-Type: application/json
Authorization: Bearer 5238800edb17efbbfb71805d0ba1294959b64fbbd854c4a7b99b5b56d720e11b
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/7b5b213140f903bb5e262d28b6a4940a.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161109%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161109T132430Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b76aadfaefb3ea01d394b8139071edc625b711af50d682253025ec31e923f225",
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
	-H "Authorization: Bearer 5238800edb17efbbfb71805d0ba1294959b64fbbd854c4a7b99b5b56d720e11b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer 89ec3f86596eb3798460bd04f70f7c8f42fdb34dc7cd7addca94cb48a36c5c8b
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
    "id": 12,
    "uploader": {
      "id": 790,
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
      "created_at": "2016-11-09T13:24:29.563Z",
      "updated_at": "2016-11-09T13:24:29.563Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-09T13:24:29.640Z",
    "updated_at": "2016-11-09T13:24:29.640Z",
    "course_id": 257,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89ec3f86596eb3798460bd04f70f7c8f42fdb34dc7cd7addca94cb48a36c5c8b"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer 47a5fa138e2b97b6a9534008e6ac8bed56160d9ec59ff1105164ac4ecbb49e7e
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
      "creator_id": 566,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-a8787eca-a6f8-4635-94bd-8c7716c5c508",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-a8787eca-a6f8-4635-94bd-8c7716c5c508",
      "slug": "mit-the-great-british-bake-off-a8787eca-a6f8-4635-94bd-8c7716c5c508",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "discipline_id": 162,
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
      "chapters_updated_at": "2016-11-09T13:24:10.675Z",
      "updated_at": "2016-11-09T13:24:13.748Z",
      "shortname": "mit-the-great-british-bake-off-a8787eca-a6f8-4635-94bd-8c7716c5c508",
      "topic_id": 161,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 561,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "discipline_id": 161,
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
      "chapters_updated_at": "2016-11-09T13:24:10.675Z",
      "updated_at": "2016-11-09T13:24:13.120Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 160,
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
curl "api.goskive.com/v2/files/8/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 47a5fa138e2b97b6a9534008e6ac8bed56160d9ec59ff1105164ac4ecbb49e7e"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/15/download
Content-Type: application/json
Authorization: Bearer e3781ce6014a013cff60d6f465985a9163da01248456ae9e9d7a3d8672347f39
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3781ce6014a013cff60d6f465985a9163da01248456ae9e9d7a3d8672347f39"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 9231ee8e05f907c421cf5f114c4d057b906b51782ed59818c0b89590e68a561f
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
	-H "Authorization: Bearer 9231ee8e05f907c421cf5f114c4d057b906b51782ed59818c0b89590e68a561f"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/10/bookmark
Content-Type: application/json
Authorization: Bearer 97ac71e2394b80177993196459322305828397a2dace93929154ae8d0c19d158
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97ac71e2394b80177993196459322305828397a2dace93929154ae8d0c19d158"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/22/upvote
Content-Type: application/json
Authorization: Bearer 0c9beba64f232815b4a1d2f131345c480c2b1da54797b97e6aa4cede21a00cda
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/22/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c9beba64f232815b4a1d2f131345c480c2b1da54797b97e6aa4cede21a00cda"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/62/comments
Content-Type: application/json
Authorization: Bearer 8d1932822e413c32e6c7767c487903f36355b030c01ee29a34c9c83d700b5bcc
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
    "author_id": 701,
    "reply_to_id": null,
    "created_at": "2016-11-09T13:24:22.094Z",
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
curl "api.goskive.com/v2/flashcards/62/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d1932822e413c32e6c7767c487903f36355b030c01ee29a34c9c83d700b5bcc"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/63/comments
Content-Type: application/json
Authorization: Bearer 0b39f6e5ec361f40540715281e5d25fea3a2cf1147c1df798df41aba789b5e75
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
    "author_id": 704,
    "reply_to_id": null,
    "created_at": "2016-11-09T13:24:22.427Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 704,
      "feedbackable_id": 63,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:22.423Z",
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
curl "api.goskive.com/v2/flashcards/63/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b39f6e5ec361f40540715281e5d25fea3a2cf1147c1df798df41aba789b5e75"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/60/comments
Content-Type: application/json
Authorization: Bearer 6e1b79cc1b3fe63c6c415050b56b5293395159a85b995f3d7f2763605395824f
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
      "author_id": 696,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:21.689Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 697,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:21.705Z",
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
curl "api.goskive.com/v2/flashcards/60/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e1b79cc1b3fe63c6c415050b56b5293395159a85b995f3d7f2763605395824f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/61/comments
Content-Type: application/json
Authorization: Bearer 1e22e19c492dded808de30efbf3873fdb5e0a3940d7bc636d2d337e6c064781f
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
curl "api.goskive.com/v2/flashcards/61/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e22e19c492dded808de30efbf3873fdb5e0a3940d7bc636d2d337e6c064781f"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/48/feedbacks
Content-Type: application/json
Authorization: Bearer 76183310645576f89598e8fc69c4d972c149cc1e9343b51d80975c01eaa700b8
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
    "user_id": 502,
    "feedbackable_id": 48,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-09T13:24:07.192Z",
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
	-H "Authorization: Bearer 76183310645576f89598e8fc69c4d972c149cc1e9343b51d80975c01eaa700b8"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/50/feedbacks
Content-Type: application/json
Authorization: Bearer 0b60ae598b7d999416ef95eec02798298ba87aae2323e3b611f0e40205665ac2
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
      "user_id": 512,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:07.687Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 511,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:07.676Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b60ae598b7d999416ef95eec02798298ba87aae2323e3b611f0e40205665ac2"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/2/votes
Content-Type: application/json
Authorization: Bearer e0990141d25cdc37fb557f1df7ac25bbf5079ee9dec700e206d40b92e95df03f
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
      "id": 6,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 89
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 88
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 87
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0990141d25cdc37fb557f1df7ac25bbf5079ee9dec700e206d40b92e95df03f"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/93/republish
Content-Type: application/json
Authorization: Bearer fb9d9add31079d84b9beda32f527334dcb06978d648bfd8e9bfc59c8b4ce925b
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
curl "api.goskive.com/v2/flashcards/93/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb9d9add31079d84b9beda32f527334dcb06978d648bfd8e9bfc59c8b4ce925b"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/91/bookmark
Content-Type: application/json
Authorization: Bearer d81f0ba0a729e7fb49491de7efc777d39c179441eef1af2460a5481642c03bb3
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/91/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d81f0ba0a729e7fb49491de7efc777d39c179441eef1af2460a5481642c03bb3"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/73
Content-Type: application/json
Authorization: Bearer 8b2602127244df27990bfa06a36de80a1990e7ec40a2576b13713436321e3bc5
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
	-H "Authorization: Bearer 8b2602127244df27990bfa06a36de80a1990e7ec40a2576b13713436321e3bc5"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/90/downvote
Content-Type: application/json
Authorization: Bearer 6d46de40634c5376d70a96b1bfaf31f019be17d8e3b428710fc2e0f0a49e633c
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/90/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d46de40634c5376d70a96b1bfaf31f019be17d8e3b428710fc2e0f0a49e633c"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/95
Content-Type: application/json
Authorization: Bearer 3c850739c71ed1f30f8f55c992fb1484a9b7735931ef509dc85d73d9454ff02e
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
    "id": 95,
    "obfuscated_id": "uTOhBSQK4CI",
    "author_id": 963,
    "chapter_id": 189,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:24:41.299Z",
    "created_at": "2016-11-09T13:24:41.299Z",
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
curl "api.goskive.com/v2/flashcards/95" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c850739c71ed1f30f8f55c992fb1484a9b7735931ef509dc85d73d9454ff02e"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/report
Content-Type: application/json
Authorization: Bearer aeb62241086516d29b4d628bf1bdb05109e96a90afbc29723f7359409608931e
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aeb62241086516d29b4d628bf1bdb05109e96a90afbc29723f7359409608931e"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/72/bookmark
Content-Type: application/json
Authorization: Bearer fa39e142a0c172b159c69f9f4d14a489a1d75a213d3f3792921e714c305ee60b
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa39e142a0c172b159c69f9f4d14a489a1d75a213d3f3792921e714c305ee60b"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/94/upvote
Content-Type: application/json
Authorization: Bearer 3f1b9131cd9c50d8c04c7a4cfaeb0918af8db6b711fb8f987373db37bd903a88
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/94/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f1b9131cd9c50d8c04c7a4cfaeb0918af8db6b711fb8f987373db37bd903a88"
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
    "key": "cache/fc6cf17f650e7ab34c821ea635b3f703.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOVQxNDoyMzoyOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2ZjNmNmMTdmNjUwZTdhYjM0YzgyMWVhNjM1YjNmNzAzLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwOS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDlUMTMyMzI5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161109/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161109T132329Z",
    "x-amz-signature": "b104cb926b2f823b4ec04a5c0fd39cd91393dbe3daaf79da94bbe382275d8a7e"
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
Authorization: Bearer bc94ad5ed187b1760f682e2af33ac6c5240cfeb71b2bf074a7819ee9bf273ce9
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
	-H "Authorization: Bearer bc94ad5ed187b1760f682e2af33ac6c5240cfeb71b2bf074a7819ee9bf273ce9"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 64b8a54443bc4cf7678048996afc1f6028246b6fce9ecade5126bfdd44a94e1c
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
	-H "Authorization: Bearer 64b8a54443bc4cf7678048996afc1f6028246b6fce9ecade5126bfdd44a94e1c"
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
{"password":{"reset_password_token":"thNNUXpSZrxpxWiXj4tT","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 541,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-09T13:24:09.941Z",
  "updated_at": "2016-11-09T13:24:10.077Z",
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
  "audit_id": 4838
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"thNNUXpSZrxpxWiXj4tT","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/113/comments
Content-Type: application/json
Authorization: Bearer b4764ac4f63edddc57acc1f1115d63143fa3a542f5726e9d436dd6c4440c3cd9
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
    "id": 53,
    "author_id": 683,
    "reply_to_id": null,
    "created_at": "2016-11-09T13:24:20.775Z",
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
curl "api.goskive.com/v2/questions/113/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4764ac4f63edddc57acc1f1115d63143fa3a542f5726e9d436dd6c4440c3cd9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/112/comments
Content-Type: application/json
Authorization: Bearer a9b877cfd815551f292773f29fb01922306f67a8105b33bda54d6d87c40bea4f
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
    "id": 52,
    "author_id": 680,
    "reply_to_id": null,
    "created_at": "2016-11-09T13:24:20.275Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 45,
      "user_id": 680,
      "feedbackable_id": 112,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:20.270Z",
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
curl "api.goskive.com/v2/questions/112/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9b877cfd815551f292773f29fb01922306f67a8105b33bda54d6d87c40bea4f"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/110/comments
Content-Type: application/json
Authorization: Bearer edf1dc690f32dc7867c06c003318bb9e6c8db4e221b5c5b31d479b3feaf53737
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
      "id": 50,
      "author_id": 675,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:19.552Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 676,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:24:19.568Z",
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
curl "api.goskive.com/v2/questions/110/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edf1dc690f32dc7867c06c003318bb9e6c8db4e221b5c5b31d479b3feaf53737"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/114/comments
Content-Type: application/json
Authorization: Bearer 2b4fee5163fa8e15c207bb6e1c32168d0546cc4015c0033af50964461f234bb7
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
curl "api.goskive.com/v2/questions/114/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b4fee5163fa8e15c207bb6e1c32168d0546cc4015c0033af50964461f234bb7"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/100/feedbacks
Content-Type: application/json
Authorization: Bearer 0fdaca50d8f6ac97c9ee57fe998f57e7816b30b3abcf3d310e5fd408b232eceb
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
    "id": 36,
    "user_id": 493,
    "feedbackable_id": 100,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-09T13:24:06.149Z",
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
curl "api.goskive.com/v2/questions/100/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fdaca50d8f6ac97c9ee57fe998f57e7816b30b3abcf3d310e5fd408b232eceb"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer d9a4aae5b2e477627a1027a35e3eea7e9a41927bb6c1c72ce4c081361b69abab
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
      "id": 32,
      "user_id": 472,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:03.991Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 471,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:24:03.980Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/95/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9a4aae5b2e477627a1027a35e3eea7e9a41927bb6c1c72ce4c081361b69abab"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/121/votes
Content-Type: application/json
Authorization: Bearer d88ea54efceeef53dd19df817e40ef336194864f52757ed65c6be034d8cf8d59
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
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 843
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 842
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 841
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/121/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d88ea54efceeef53dd19df817e40ef336194864f52757ed65c6be034d8cf8d59"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/6/republish
Content-Type: application/json
Authorization: Bearer 63e51d60ae683978026141dfcf7d0a29d8fcaa7995e002e93938caf95492e1fa
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
curl "api.goskive.com/v2/questions/6/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63e51d60ae683978026141dfcf7d0a29d8fcaa7995e002e93938caf95492e1fa"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/2/bookmark
Content-Type: application/json
Authorization: Bearer 57fc16a534be219856b53ec6eedfac929a6844828258d9b2860c066c2234fda6
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/2/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57fc16a534be219856b53ec6eedfac929a6844828258d9b2860c066c2234fda6"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/10
Content-Type: application/json
Authorization: Bearer 92140db0d99137c100989a6897c29049a62fbda372a8c10c98e9b95475709a8d
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92140db0d99137c100989a6897c29049a62fbda372a8c10c98e9b95475709a8d"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/4/downvote
Content-Type: application/json
Authorization: Bearer fa6c0792a7b49ce0ccfd5cc60db5bb00b2147e78ae918bd1296f56074705366e
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/4/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa6c0792a7b49ce0ccfd5cc60db5bb00b2147e78ae918bd1296f56074705366e"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/9
Content-Type: application/json
Authorization: Bearer 00b4b9414fd0cbb77dcafd98c7b5b99949d6a50f424aa61368b20a00948f064f
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
    "id": 9,
    "obfuscated_id": "DMbUb8tMXMw",
    "author_id": 25,
    "chapter_id": 9,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:19.999Z",
    "created_at": "2016-11-09T13:23:19.870Z",
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
        "id": 18,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 19,
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
curl "api.goskive.com/v2/questions/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00b4b9414fd0cbb77dcafd98c7b5b99949d6a50f424aa61368b20a00948f064f"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/8/report
Content-Type: application/json
Authorization: Bearer cfe8aa9f6e8b7928ebfc27f0c3de01c12a219ca2ed6febcd8e3f5717d042d6fb
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/8/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfe8aa9f6e8b7928ebfc27f0c3de01c12a219ca2ed6febcd8e3f5717d042d6fb"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/3/bookmark
Content-Type: application/json
Authorization: Bearer d9504d66f09fc87fd29225aae1d4de32cbbe358b5ff1c2974312d839f77890e8
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/3/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9504d66f09fc87fd29225aae1d4de32cbbe358b5ff1c2974312d839f77890e8"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/7
Content-Type: application/json
Authorization: Bearer 4568f685b978849035785e602b19a43eeee7ac03505bc854bcf5b98f77f26731
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":7,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-09T13:23:18.261Z","updated_at":"2016-11-09T13:23:18.386Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":7,"author_id":19,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 7,
    "obfuscated_id": "XFkue8saGAM",
    "author_id": 19,
    "chapter_id": 7,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-09T13:23:18.495Z",
    "created_at": "2016-11-09T13:23:18.261Z",
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
    "question": "{\"id\"=>7, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-09T13:23:18.261Z\", \"updated_at\"=>\"2016-11-09T13:23:18.386Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>7, \"author_id\"=>19, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 15,
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
curl "api.goskive.com/v2/questions/7" -d '{"question":{"question":{"id":7,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-09T13:23:18.261Z","updated_at":"2016-11-09T13:23:18.386Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":7,"author_id":19,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4568f685b978849035785e602b19a43eeee7ac03505bc854bcf5b98f77f26731"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/1/upvote
Content-Type: application/json
Authorization: Bearer 7f778eb5e93034e3610234964c28079557c63d19d76b58bb4db7e7220db19e6c
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/1/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f778eb5e93034e3610234964c28079557c63d19d76b58bb4db7e7220db19e6c"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 756f19f940cf6705f8ac65f92c2c08dd834dc538faad924d96cea5a8e2cf3440
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
      "creator_id": 828,
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "discipline_id": 282,
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
      "updated_at": "2016-11-09T13:24:31.260Z",
      "shortname": "mit-pizza-201",
      "topic_id": 281,
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
	-H "Authorization: Bearer 756f19f940cf6705f8ac65f92c2c08dd834dc538faad924d96cea5a8e2cf3440"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b2ea8f77419357bf1442e5f0b23be5eda710d975896c51b7b3578b040ae2c773
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
      "id": 255,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-235",
      "html_url": "https://goskive.com/university/uni-235",
      "slug": "uni-235",
      "name": "National School of Pizza",
      "short_name": "Uni 235",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2cc15b104b1aaaeb845f9022ab59cb670ca01071.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8197d7d874c9a5ab4677d076428184f2d5e4e863.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T13:24:31.551Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-234",
      "html_url": "https://goskive.com/university/uni-234",
      "slug": "uni-234",
      "name": "National School of Pastry",
      "short_name": "Uni 234",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8c788a95dfad28c588d3608260beb198473036c0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/396bffed646beae206609bfc9db67f86bea55c6a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T13:24:31.533Z",
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
	-H "Authorization: Bearer b2ea8f77419357bf1442e5f0b23be5eda710d975896c51b7b3578b040ae2c773"
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
      "id": 34,
      "name": "Versatile optimizing groupware",
      "name_translations": {
        "en": "Versatile optimizing groupware"
      },
      "discipline_id": 34
    },
    {
      "id": 35,
      "name": "Universal multi-state middleware",
      "name_translations": {
        "en": "Universal multi-state middleware"
      },
      "discipline_id": 35
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
GET /v2/topics/33
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
    "id": 33,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 33
  }
}
```



```shell
curl "api.goskive.com/v2/topics/33" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 844b3254eb0a9bc2c5eb3257f5b968dcddbca19a8bf155874890d2e5e78a4629
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
      "id": 67,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-65",
      "html_url": "https://goskive.com/university/uni-65",
      "slug": "uni-65",
      "name": "University 44",
      "short_name": "Uni 65",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9f2d41a18511a2bab0b208f8d4f94d96036b52a5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/008381d2042e430be1fc7c898823f8fcf7e9cf5f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T13:23:43.613Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-66",
      "html_url": "https://goskive.com/university/uni-66",
      "slug": "uni-66",
      "name": "University 45",
      "short_name": "Uni 66",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6405465ad0fc3c2d3eaf0635e889b20638a175ec.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2327e16c6fba86bf7ae8283984f0c576a64406f3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T13:23:43.630Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-67",
      "html_url": "https://goskive.com/university/uni-67",
      "slug": "uni-67",
      "name": "University 46",
      "short_name": "Uni 67",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/708a005b52f81ade5d5c9481071b7a8cff7c4cd9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/822e4ae5676b385680a75a35bb9799eaca85f11e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-09T13:23:43.647Z",
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
	-H "Authorization: Bearer 844b3254eb0a9bc2c5eb3257f5b968dcddbca19a8bf155874890d2e5e78a4629"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 9d6dc8526b6e0f422d2172b12c718229f871b0b61ef701aed878b3d1bcc3c2fc
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
    "id": 65,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0b554848511eb0c693e5b33d9e9f705745f9f331.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/fabb93546afe8266713ab5e9a36016b55dab1bfd.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-09T13:23:43.429Z",
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
	-H "Authorization: Bearer 9d6dc8526b6e0f422d2172b12c718229f871b0b61ef701aed878b3d1bcc3c2fc"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b17c8cc3b917e0ae1fbbfcb34fe91b475c2e5931f60d36c77072f73d0edb8f53
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":252,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 750,
    "id": 240,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 224,
    "additional_university_ids": [

    ],
    "discipline_id": 253,
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
    "chapters_updated_at": "2016-11-09T13:24:26.705Z",
    "updated_at": "2016-11-09T13:24:26.851Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 150,
        "updated_at": "2016-11-09T13:24:26.806Z",
        "course_id": 240,
        "author_id": 750,
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
        "id": 151,
        "updated_at": "2016-11-09T13:24:26.823Z",
        "course_id": 240,
        "author_id": 750,
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
        "id": 152,
        "updated_at": "2016-11-09T13:24:26.840Z",
        "course_id": 240,
        "author_id": 750,
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
    "topic_id": 252,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":252,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b17c8cc3b917e0ae1fbbfcb34fe91b475c2e5931f60d36c77072f73d0edb8f53"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5faadd4b7d5d34d879d217c7ade03429cba7df76b2621143b0b173959e5ecd8c
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":253,"published":false}}
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
    "id": 241,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 225,
    "additional_university_ids": [

    ],
    "discipline_id": 254,
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
    "updated_at": "2016-11-09T13:24:27.047Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 253,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":253,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5faadd4b7d5d34d879d217c7ade03429cba7df76b2621143b0b173959e5ecd8c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c2492396b37551ded4b59143fe657a6a1045b652753fc7e6b499101efa0dec7b
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
      "creator_id": 712,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 210,
      "additional_university_ids": [

      ],
      "discipline_id": 221,
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
      "updated_at": "2016-11-09T13:24:23.176Z",
      "shortname": "fu-course-153",
      "topic_id": 220,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 153",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 712,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-154",
      "html_url": "https://goskive.com/course/fu-course-154",
      "slug": "fu-course-154",
      "university_id": 210,
      "additional_university_ids": [

      ],
      "discipline_id": 222,
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
      "chapters_updated_at": "2016-11-09T13:24:23.027Z",
      "updated_at": "2016-11-09T13:24:23.492Z",
      "shortname": "fu-course-154",
      "topic_id": 221,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 154",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2492396b37551ded4b59143fe657a6a1045b652753fc7e6b499101efa0dec7b"
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
      "creator_id": 722,
      "id": 216,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-161",
      "html_url": "https://goskive.com/course/fu-course-161",
      "slug": "fu-course-161",
      "university_id": 213,
      "additional_university_ids": [

      ],
      "discipline_id": 229,
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
      "updated_at": "2016-11-09T13:24:24.085Z",
      "shortname": "fu-course-161",
      "topic_id": 228,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 161",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 722,
      "id": 217,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 213,
      "additional_university_ids": [

      ],
      "discipline_id": 230,
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
      "chapters_updated_at": "2016-11-09T13:24:23.931Z",
      "updated_at": "2016-11-09T13:24:24.390Z",
      "shortname": "fu-course-162",
      "topic_id": 229,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 162",
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
Authorization: Bearer 2e99b8b8c04ca182063aac43f6349fcde53b339599d5e22a1a2bb40f1384452e
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
      "creator_id": 719,
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-157",
      "html_url": "https://goskive.com/course/fu-course-157",
      "slug": "fu-course-157",
      "university_id": 212,
      "additional_university_ids": [

      ],
      "discipline_id": 225,
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
      "updated_at": "2016-11-09T13:24:23.809Z",
      "shortname": "fu-course-157",
      "topic_id": 224,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 157",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 719,
      "id": 213,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-158",
      "html_url": "https://goskive.com/course/fu-course-158",
      "slug": "fu-course-158",
      "university_id": 212,
      "additional_university_ids": [

      ],
      "discipline_id": 226,
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
      "updated_at": "2016-11-09T13:24:23.851Z",
      "shortname": "fu-course-158",
      "topic_id": 225,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 158",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e99b8b8c04ca182063aac43f6349fcde53b339599d5e22a1a2bb40f1384452e"
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
      "creator_id": 727,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 215,
      "additional_university_ids": [

      ],
      "discipline_id": 233,
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
      "updated_at": "2016-11-09T13:24:24.604Z",
      "shortname": "fu-course-165",
      "topic_id": 232,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 727,
      "id": 221,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 215,
      "additional_university_ids": [

      ],
      "discipline_id": 234,
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
      "updated_at": "2016-11-09T13:24:24.643Z",
      "shortname": "fu-course-166",
      "topic_id": 233,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
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
Authorization: Bearer fa7cdf4ad891ad67bc8ade6d28ea149e0327e81867fc9cc2ccd698cb735a10ff
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
  "id": 451,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-09T13:24:01.814Z",
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
	-H "Authorization: Bearer fa7cdf4ad891ad67bc8ade6d28ea149e0327e81867fc9cc2ccd698cb735a10ff"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/543
Content-Type: application/json
Authorization: Bearer 8d6a3a52780541b85e08c13dda49665a2a3dd5c1add517e65b5fb7b492bdcd4a
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
    "id": 543,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 150,
    "fields_of_study": [
      155,
      156
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-09T13:24:10.168Z",
    "updated_at": "2016-11-09T13:24:10.168Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/543" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d6a3a52780541b85e08c13dda49665a2a3dd5c1add517e65b5fb7b492bdcd4a"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/545
Content-Type: application/json
Authorization: Bearer bc9dc4cc8e9bfef260ac6026b9f00c8f640434823c0dbee5f2f05ea4c55debff
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
    "id": 545,
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
    "created_at": "2016-11-09T13:24:10.252Z",
    "updated_at": "2016-11-09T13:24:10.252Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/545" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc9dc4cc8e9bfef260ac6026b9f00c8f640434823c0dbee5f2f05ea4c55debff"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/22
Content-Type: application/json
Authorization: Bearer e7cdf3e562e41be437ac075de542799d64683fdd178503eb24aaaa45f1d7a636
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7cdf3e562e41be437ac075de542799d64683fdd178503eb24aaaa45f1d7a636"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/21
Content-Type: application/json
Authorization: Bearer 37f9b0ab1e7abf496975beccfea4db3576a9538f1860c0f69f286853a5858b0e
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
    "id": 21,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 129,
    "user_id": 966
  }
}
```



```shell
curl "api.goskive.com/v2/votes/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37f9b0ab1e7abf496975beccfea4db3576a9538f1860c0f69f286853a5858b0e"
```
