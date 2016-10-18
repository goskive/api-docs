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
Authorization: Basic YjNjZmMxNGQ4NjE4MmZiYjc0ZjY5YmU5NzYyNGJmYmE5OWYyZGQ5YjM5ZjJm
NTYxN2FmNzZjNmZjYzdkYWJmYjo5MDIyYWY5MmIxYWRiMzJkMzVlOTA0M2Iw
NzRkNTUzNmViMmRhOTY4MjA5NDMwZjk2MDgwZjJmNzM5YmJhYjgx

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
	-u b3cfc14d86182fbb74f69be97624bfba99f2dd9b39f2f5617af76c6fcc7dabfb:9022af92b1adb32d35e9043b074d5536eb2da968209430f96080f2f739bbab81
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"aa4e0d723ca2a042940d61a4f9abae2750c3b897b5c40fa4a2690f0180c3a5d2","client_secret":"c47506167b02a440448ec9a29b574d295e1c3daae4370c5e4a22e98294479dd5"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"aa4e0d723ca2a042940d61a4f9abae2750c3b897b5c40fa4a2690f0180c3a5d2","client_secret":"c47506167b02a440448ec9a29b574d295e1c3daae4370c5e4a22e98294479dd5"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDRlODg5Y2ZhZjY5OTI3NWQ2OWFlYTdjMmYyZWY0Mzk0NzRkNzQyMzNhMjA0
OWNhYjI4Y2U4MGZmNjIzNDVhYjoxYTYyYmU2ZmZmNDI5NDc2MGJkYmFhNTE1
YmFhN2JmODJkYTI4MDFkNjExNzZlMmIzNmViMzM3ZmQ1NDczZmVi

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
  "access_token": "8136cfe7630cb09296ad64c3bbefc9e8dfcbf77401503046d178426132ec9b05",
  "token_type": "bearer",
  "created_at": 1476794230
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u d4e889cfaf699275d69aea7c2f2ef439474d74233a2049cab28ce80ff62345ab:1a62be6fff4294760bdbaa515baa7bf82da2801d61176e2b36eb337fd5473feb
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"d8b0e918dfc672ff7a9ccd9f1c939e80658d7568b6100c4c088699d42bba07e4","client_secret":"a2905f3f4a8d8506468d9d0162fc4e9dc46ed3dce6d1aaa034f980765b3158a6"}
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
  "access_token": "55963555b7d6ca327654808b978a0ec4ace8d034ecdc6a90efb8af62e3b5d959",
  "token_type": "bearer",
  "created_at": 1476794230
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"d8b0e918dfc672ff7a9ccd9f1c939e80658d7568b6100c4c088699d42bba07e4","client_secret":"a2905f3f4a8d8506468d9d0162fc4e9dc46ed3dce6d1aaa034f980765b3158a6"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"5010329748816d309164fdd23be0388c6828691fd26f03d04f6e18664612bda5","client_secret":"a5e636e9fac504d17d362653fda33190d07481798c649bfa6510358fc984b408"}
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
  "access_token": "876bd94f3cf69534618a54d2e6b96083305114d0286f951c4f87058df6e7f65d",
  "token_type": "bearer",
  "created_at": 1476794230
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5010329748816d309164fdd23be0388c6828691fd26f03d04f6e18664612bda5","client_secret":"a5e636e9fac504d17d362653fda33190d07481798c649bfa6510358fc984b408"}' -X POST \
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
Authorization: Bearer fe3cd8b1f28aeb93c16652efda906ac5b9d4092b61eb98a4fbda2ed3e149caf2
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
curl "api.goskive.com/v2/campaigns/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe3cd8b1f28aeb93c16652efda906ac5b9d4092b61eb98a4fbda2ed3e149caf2"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/79/flashcards
Content-Type: application/json
Authorization: Bearer 400793f2d3cecb258ecba9d7b178b57aee65f1e0fc03833a02e67bb40cd8a4b1
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":79,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 20,
    "obfuscated_id": "4DFpearSrHk",
    "author_id": 459,
    "chapter_id": 79,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:36:57.131Z",
    "created_at": "2016-10-18T12:36:57.131Z",
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
curl "api.goskive.com/v2/chapters/79/flashcards" -d '{"flashcard":{"chapter_id":79,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 400793f2d3cecb258ecba9d7b178b57aee65f1e0fc03833a02e67bb40cd8a4b1"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/77/flashcards
Content-Type: application/json
Authorization: Bearer 554f5625d76b504a718b5814d5ac3e8d7e5ebeb1dadab25f3991440f2b9f359f
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 451,
      "chapter_id": 77,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:56.686Z",
      "created_at": "2016-10-18T12:36:56.686Z",
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
      "author_id": 451,
      "chapter_id": 77,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:56.725Z",
      "created_at": "2016-10-18T12:36:56.725Z",
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 451,
      "chapter_id": 77,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:36:56.766Z",
      "created_at": "2016-10-18T12:36:56.766Z",
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
curl "api.goskive.com/v2/chapters/77/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 554f5625d76b504a718b5814d5ac3e8d7e5ebeb1dadab25f3991440f2b9f359f"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/116/questions
Content-Type: application/json
Authorization: Bearer 2c2eb2280c74c0ce2f9ebcac330a80e524f75ae4983b565170116a4ab41c7d7d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 664,
    "chapter_id": 116,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:37:19.268Z",
    "created_at": "2016-10-18T12:37:19.268Z",
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
        "id": 200,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 201,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 202,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 203,
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
curl "api.goskive.com/v2/chapters/116/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c2eb2280c74c0ce2f9ebcac330a80e524f75ae4983b565170116a4ab41c7d7d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/117/questions
Content-Type: application/json
Authorization: Bearer cb8910bc91ed65efed2a81b02fd0efb4bb16798fe4eaf1ba2ac9adc2fa4a00ac
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":117,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 667,
    "chapter_id": 117,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:37:19.857Z",
    "created_at": "2016-10-18T12:37:19.857Z",
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
        "id": 204,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 205,
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
curl "api.goskive.com/v2/chapters/117/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":117,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb8910bc91ed65efed2a81b02fd0efb4bb16798fe4eaf1ba2ac9adc2fa4a00ac"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/118/questions
Content-Type: application/json
Authorization: Bearer 06602a0a917ac2b6436474a4af6231af7a2e60755850947781f1d036652c066d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 670,
    "chapter_id": 118,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:37:20.230Z",
    "created_at": "2016-10-18T12:37:20.230Z",
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
        "id": 206,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 207,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/118/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06602a0a917ac2b6436474a4af6231af7a2e60755850947781f1d036652c066d"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/119/questions
Content-Type: application/json
Authorization: Bearer c5f7613c64449100625b24349be5f7d3e5f832558f10b450afe3aacdcea01398
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":119,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 673,
    "chapter_id": 119,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:37:20.608Z",
    "created_at": "2016-10-18T12:37:20.608Z",
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
curl "api.goskive.com/v2/chapters/119/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":119,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5f7613c64449100625b24349be5f7d3e5f832558f10b450afe3aacdcea01398"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/114/questions
Content-Type: application/json
Authorization: Bearer 151043614e53d3ae41230f2e71d93f13f23ae1304317dbf64ae429cfb072d999
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
      "id": 97,
      "obfuscated_id": "qdTHUgSdSV8",
      "author_id": 655,
      "chapter_id": 114,
      "position": 88,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:18.414Z",
      "created_at": "2016-10-18T12:37:18.276Z",
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
          "id": 194,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 195,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 98,
      "obfuscated_id": "icApzX10lRE",
      "author_id": 656,
      "chapter_id": 114,
      "position": 89,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:18.639Z",
      "created_at": "2016-10-18T12:37:18.497Z",
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
          "id": 196,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 197,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 99,
      "obfuscated_id": "5fPQ9k37GTc",
      "author_id": 657,
      "chapter_id": 114,
      "position": 90,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T12:37:18.869Z",
      "created_at": "2016-10-18T12:37:18.723Z",
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
          "id": 198,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 199,
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
curl "api.goskive.com/v2/chapters/114/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 151043614e53d3ae41230f2e71d93f13f23ae1304317dbf64ae429cfb072d999"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/192
Content-Type: application/json
Authorization: Bearer e10c9ab398a8bc4187457e88549470938558088cbc0a41440c32e06a4fcce156
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
curl "api.goskive.com/v2/chapters/192" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e10c9ab398a8bc4187457e88549470938558088cbc0a41440c32e06a4fcce156"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/194
Content-Type: application/json
Authorization: Bearer 2e8f446e81ab5263e6c23b1f3c6e31af0eea430c24717e92d7f10aa4f917c971
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
curl "api.goskive.com/v2/chapters/194" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e8f446e81ab5263e6c23b1f3c6e31af0eea430c24717e92d7f10aa4f917c971"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/188
Content-Type: application/json
Authorization: Bearer 48efe2620f95556c75599aa58598b8658049d61751e10f98cff79863390027d9
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
curl "api.goskive.com/v2/chapters/188" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48efe2620f95556c75599aa58598b8658049d61751e10f98cff79863390027d9"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/193
Content-Type: application/json
Authorization: Bearer 818dbefb678dde2f1920ca335d1a98af059d8ab059862c4f70d184e512fd80f0
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/193" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 818dbefb678dde2f1920ca335d1a98af059d8ab059862c4f70d184e512fd80f0"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 2124db68b57c2d15227842a67b30ad26f276f4f403b1239769fe81b2d5cdb8cd
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
    "id": 190,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-18T12:37:40.727Z",
    "course_id": 302,
    "author_id": 937,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-18T12:37:40.189Z",
    "questions_updated_at": "2016-10-18T12:37:40.189Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 941,
        "chapter_id": 190,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:40.710Z",
        "created_at": "2016-10-18T12:37:40.710Z",
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
        "id": 130,
        "obfuscated_id": "N-qIf0IsvWM",
        "author_id": 939,
        "chapter_id": 190,
        "position": 117,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:40.601Z",
        "created_at": "2016-10-18T12:37:40.483Z",
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
            "id": 263,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 264,
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
curl "api.goskive.com/v2/chapters/190" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2124db68b57c2d15227842a67b30ad26f276f4f403b1239769fe81b2d5cdb8cd"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/187
Content-Type: application/json
Authorization: Bearer 01306fc7a0c07e23dd3ffa25b95b9ae05101c4fadcb70127ee7a3164311348e5
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
    "id": 187,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-18T12:37:39.864Z",
    "course_id": 299,
    "author_id": 929,
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
curl "api.goskive.com/v2/chapters/187" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01306fc7a0c07e23dd3ffa25b95b9ae05101c4fadcb70127ee7a3164311348e5"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/45/replies
Content-Type: application/json
Authorization: Bearer f5c496fb36eeba25e470d768ad3dd79a5b77b1bdfd17b4edc7dc08406d80d37f
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
    "id": 46,
    "author_id": 445,
    "reply_to_id": 45,
    "created_at": "2016-10-18T12:36:56.036Z",
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
curl "api.goskive.com/v2/comments/45/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5c496fb36eeba25e470d768ad3dd79a5b77b1bdfd17b4edc7dc08406d80d37f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/47/replies
Content-Type: application/json
Authorization: Bearer 154764bb7a2a9a6e9c810f94c42c28d0cbff90e7470fd571692672fcb7dc36a3
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
curl "api.goskive.com/v2/comments/47/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 154764bb7a2a9a6e9c810f94c42c28d0cbff90e7470fd571692672fcb7dc36a3"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/1
Content-Type: application/json
Authorization: Bearer c059212a4d9c03214856b6fc5be99655403ba727ab32fbe13a802111261405ae
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
curl "api.goskive.com/v2/comments/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c059212a4d9c03214856b6fc5be99655403ba727ab32fbe13a802111261405ae"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/40/republish
Content-Type: application/json
Authorization: Bearer 59b6a4e6f8986d91e9753ce96e26c03c25a85c02d109c24ae93379f119579f58
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
	-H "Authorization: Bearer 59b6a4e6f8986d91e9753ce96e26c03c25a85c02d109c24ae93379f119579f58"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer e4fba0e209717537f6f88b4790b0a37ca05bee552599aeac619bf505b69b6551
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
	-H "Authorization: Bearer e4fba0e209717537f6f88b4790b0a37ca05bee552599aeac619bf505b69b6551"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/4/report
Content-Type: application/json
Authorization: Bearer c2b12f1d634e67935aadea42f4083c9b9ed1df4a11e831d348ac0653ab8eb33d
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
	-H "Authorization: Bearer c2b12f1d634e67935aadea42f4083c9b9ed1df4a11e831d348ac0653ab8eb33d"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/23
Content-Type: application/json
Authorization: Bearer dd107a443cfce4f6f7ea8373c73a26a2c223846807c4e757e97bd79df4858364
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
    "id": 23,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-18T12:36:36.835Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd107a443cfce4f6f7ea8373c73a26a2c223846807c4e757e97bd79df4858364"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer c1ace44cbbe38484bf0a2d208cf33ac7e70db5f41f93e516d6acb5e0163c2be5
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
      "id": 20,
      "name": "Fake Company Name 17",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:36:36.768Z"
    },
    {
      "id": 21,
      "name": "Fake Company Name 18",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:36:36.772Z"
    },
    {
      "id": 22,
      "name": "Fake Company Name 19",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T12:36:36.776Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1ace44cbbe38484bf0a2d208cf33ac7e70db5f41f93e516d6acb5e0163c2be5"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/19/company_profiles
Content-Type: application/json
Authorization: Bearer 7b94b6a5e8f3ef570e8e82d7eba3441302815f0fec7116d44720a1ede34b6db0
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

      ]
    },
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
  ]
}
```



```shell
curl "api.goskive.com/v2/companies/19/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b94b6a5e8f3ef570e8e82d7eba3441302815f0fec7116d44720a1ede34b6db0"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/17/company_profiles
Content-Type: application/json
Authorization: Bearer e0d33276a45c7be9e12c79f35cfbef50fcfe4d8e0e0ffd61845787da575eada9
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
      "id": 4,
      "display_priority": 1,
      "published": true,
      "revision_updated_at": "2013-01-01T00:00:00.000Z",
      "header_image_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/b7227ba08020eaf424f385a68712e11390fe76a3.png",
      "header_image_hires_url": "file:///home/ubuntu/skive-backend/public/system/company_profiles/original/15a47e0f0d046fb9c95772f170325321f8fb4d6d.png",
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
curl "api.goskive.com/v2/companies/17/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0d33276a45c7be9e12c79f35cfbef50fcfe4d8e0e0ffd61845787da575eada9"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer f1c1ad219758549960e02087961fc6a8ac3037c5dc226453f55bb81164b28a2e
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
      "company_id": 25,
      "precluded_campaign_ids": [

      ],
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
      "company_id": 28,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 10,
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
	-H "Authorization: Bearer f1c1ad219758549960e02087961fc6a8ac3037c5dc226453f55bb81164b28a2e"
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
Authorization: Bearer 4d28ee89448a4369285e9fcd59db87c41854d3066a899fbcdb947d22753358da
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
	-H "Authorization: Bearer 4d28ee89448a4369285e9fcd59db87c41854d3066a899fbcdb947d22753358da"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 135ce916b0da1a71f386e60824eb56ed306c62b021b32a213b3831411e03e988
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
    "id": 174,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T12:37:34.379Z",
    "course_id": 284,
    "author_id": 872,
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
	-H "Authorization: Bearer 135ce916b0da1a71f386e60824eb56ed306c62b021b32a213b3831411e03e988"
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
      "id": 159,
      "title": "Clever Chapter Title 147",
      "position": 1,
      "updated_at": "2016-10-18T12:37:32.342Z",
      "course_id": 275,
      "author_id": 838,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 160,
      "title": "Clever Chapter Title 148",
      "position": 2,
      "updated_at": "2016-10-18T12:37:32.369Z",
      "course_id": 275,
      "author_id": 839,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 161,
      "title": "Clever Chapter Title 149",
      "position": 3,
      "updated_at": "2016-10-18T12:37:32.671Z",
      "course_id": 275,
      "author_id": 840,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T12:37:32.260Z",
      "questions_updated_at": "2016-10-18T12:37:32.260Z",
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
Authorization: Bearer 277f03eb72e683b87e8ce56be5b9a307157baceebda94b8c3f80d4d20ef3c89b
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
      "id": 165,
      "title": "Clever Chapter Title 153",
      "position": 1,
      "updated_at": "2016-10-18T12:37:33.046Z",
      "course_id": 278,
      "author_id": 849,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 166,
      "title": "Clever Chapter Title 154",
      "position": 2,
      "updated_at": "2016-10-18T12:37:33.074Z",
      "course_id": 278,
      "author_id": 850,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 167,
      "title": "Clever Chapter Title 155",
      "position": 3,
      "updated_at": "2016-10-18T12:37:33.390Z",
      "course_id": 278,
      "author_id": 851,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T12:37:32.969Z",
      "questions_updated_at": "2016-10-18T12:37:32.969Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 277f03eb72e683b87e8ce56be5b9a307157baceebda94b8c3f80d4d20ef3c89b"
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
      "id": 162,
      "title": "Clever Chapter Title 150",
      "position": 1,
      "updated_at": "2016-10-18T12:37:32.870Z",
      "course_id": 277,
      "author_id": 845,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 163,
      "title": "Clever Chapter Title 151",
      "position": 2,
      "updated_at": "2016-10-18T12:37:32.897Z",
      "course_id": 277,
      "author_id": 846,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 164,
      "title": "Clever Chapter Title 152",
      "position": 3,
      "updated_at": "2016-10-18T12:37:32.925Z",
      "course_id": 277,
      "author_id": 847,
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
Authorization: Bearer dca9c6ee90a8b56f29e7ad6b24ae3aebc2fc734400eaf6158683d0e0ff17263a
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
      "id": 168,
      "title": "Clever Chapter Title 156",
      "position": 1,
      "updated_at": "2016-10-18T12:37:33.551Z",
      "course_id": 279,
      "author_id": 856,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 169,
      "title": "Clever Chapter Title 157",
      "position": 2,
      "updated_at": "2016-10-18T12:37:33.578Z",
      "course_id": 279,
      "author_id": 857,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 170,
      "title": "Clever Chapter Title 158",
      "position": 3,
      "updated_at": "2016-10-18T12:37:33.606Z",
      "course_id": 279,
      "author_id": 858,
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
	-H "Authorization: Bearer dca9c6ee90a8b56f29e7ad6b24ae3aebc2fc734400eaf6158683d0e0ff17263a"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 3b611c233ef394e179a94f471e16ae65209864bbd52a4f10f47714cc21b6cd95
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
    "id": 7,
    "course_id": 266,
    "user_id": 807,
    "updated_at": "2016-10-18T12:37:29.934Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b611c233ef394e179a94f471e16ae65209864bbd52a4f10f47714cc21b6cd95"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7e63ef6a00cbbecc4b17ee989294bc68b17f1645868c1b79c13e6f6831c8bf62
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
      "course_id": 261,
      "user_id": 793,
      "updated_at": "2016-10-18T12:37:29.162Z"
    },
    {
      "id": 3,
      "course_id": 261,
      "user_id": 794,
      "updated_at": "2016-10-18T12:37:29.181Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e63ef6a00cbbecc4b17ee989294bc68b17f1645868c1b79c13e6f6831c8bf62"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/211/files
Content-Type: application/json
Authorization: Bearer 12b426641797522dff63302227213acd3f7f507796da3ca5f63fdc429d512c29
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
        "id": 619,
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
        "created_at": "2016-10-18T12:37:14.505Z",
        "updated_at": "2016-10-18T12:37:14.505Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:37:14.513Z",
      "updated_at": "2016-10-18T12:37:14.513Z",
      "course_id": 211,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 620,
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
        "created_at": "2016-10-18T12:37:14.520Z",
        "updated_at": "2016-10-18T12:37:14.520Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:37:14.527Z",
      "updated_at": "2016-10-18T12:37:14.527Z",
      "course_id": 211,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 10,
      "uploader": {
        "id": 621,
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
        "created_at": "2016-10-18T12:37:14.535Z",
        "updated_at": "2016-10-18T12:37:14.535Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T12:37:14.542Z",
      "updated_at": "2016-10-18T12:37:14.542Z",
      "course_id": 211,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/211/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12b426641797522dff63302227213acd3f7f507796da3ca5f63fdc429d512c29"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/214/files
Content-Type: application/json
Authorization: Bearer cbdbf79dc2a4a90246ce207c82f15bbcd4e51f3a6fb5a2f7e25d5e30c395676b
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
      "id": 628,
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
      "created_at": "2016-10-18T12:37:14.882Z",
      "updated_at": "2016-10-18T12:37:14.882Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-18T12:37:14.912Z",
    "updated_at": "2016-10-18T12:37:14.912Z",
    "course_id": 214,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/214/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbdbf79dc2a4a90246ce207c82f15bbcd4e51f3a6fb5a2f7e25d5e30c395676b"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/213/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 71153056a333cf9dc36f108788aceddb6a49f625dc8507ede092fe9cf3625f2f
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
    "key": "cache/8c5279ed3f315c9c341838d673f518b4.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMzozNzoxNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS84YzUyNzllZDNmMzE1YzljMzQxODM4ZDY3M2Y1MThiNC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMThUMTIzNzE0WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T123714Z",
    "x-amz-signature": "4b6ad0f2cff8aa890fd82c1b593a069448570227816f31ab7ca9cbadcbe09b94"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/213/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71153056a333cf9dc36f108788aceddb6a49f625dc8507ede092fe9cf3625f2f"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 9a0146c1abb6c747e51fd4b7b43f3c62b11b16a7ea200fb1b42d8a968998f295
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
	-H "Authorization: Bearer 9a0146c1abb6c747e51fd4b7b43f3c62b11b16a7ea200fb1b42d8a968998f295"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer eef64d1e4867ce52c421d2890d4d5a44c97b9add13791041f8659fc4159a3925
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
	-H "Authorization: Bearer eef64d1e4867ce52c421d2890d4d5a44c97b9add13791041f8659fc4159a3925"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7cf5ddc36e08203365b7ebeca97c6d0113757f2ec9a6eb07f218a9f6ade42b61
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
	-H "Authorization: Bearer 7cf5ddc36e08203365b7ebeca97c6d0113757f2ec9a6eb07f218a9f6ade42b61"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 687a7ceb9764c30ed9f5c90014003ab947c3786c9560c4373401ff9f745fcdf7
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
	-H "Authorization: Bearer 687a7ceb9764c30ed9f5c90014003ab947c3786c9560c4373401ff9f745fcdf7"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 90d436bdd3f1151c206e60d964d9dbdcf439bf1ab26f940f2768bf531debcd24
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
	-H "Authorization: Bearer 90d436bdd3f1151c206e60d964d9dbdcf439bf1ab26f940f2768bf531debcd24"
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
    "creator_id": 534,
    "id": 190,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 168,
    "additional_university_ids": [

    ],
    "topic_id": 198,
    "discipline_id": 198,
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
    "chapters_updated_at": "2016-10-18T12:37:04.304Z",
    "updated_at": "2016-10-18T12:37:05.924Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 92,
        "title": "Clever Chapter Title 86",
        "position": 1,
        "updated_at": "2016-10-18T12:37:05.873Z",
        "course_id": 190,
        "author_id": 534,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:37:04.304Z",
        "questions_updated_at": "2016-10-18T12:37:04.304Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 93,
        "title": "Clever Chapter Title 87",
        "position": 2,
        "updated_at": "2016-10-18T12:37:05.915Z",
        "course_id": 190,
        "author_id": 534,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:37:04.304Z",
        "questions_updated_at": "2016-10-18T12:37:04.304Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 534,
        "chapter_id": 92,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:04.536Z",
        "created_at": "2016-10-18T12:37:04.403Z",
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
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 534,
        "chapter_id": 93,
        "position": 64,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:04.978Z",
        "created_at": "2016-10-18T12:37:04.838Z",
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
Authorization: Bearer d0bfb6990a8a952bc15bc2fc708ec5679965715d9a5487708f0ec1199923fa46
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
    "creator_id": 539,
    "id": 191,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 169,
    "additional_university_ids": [

    ],
    "topic_id": 199,
    "discipline_id": 199,
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
    "chapters_updated_at": "2016-10-18T12:37:05.982Z",
    "updated_at": "2016-10-18T12:37:07.668Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 94,
        "title": "Clever Chapter Title 88",
        "position": 1,
        "updated_at": "2016-10-18T12:37:07.613Z",
        "course_id": 191,
        "author_id": 539,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:37:05.982Z",
        "questions_updated_at": "2016-10-18T12:37:05.982Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 95,
        "title": "Clever Chapter Title 89",
        "position": 2,
        "updated_at": "2016-10-18T12:37:07.659Z",
        "course_id": 191,
        "author_id": 539,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T12:37:05.982Z",
        "questions_updated_at": "2016-10-18T12:37:05.982Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 540,
        "chapter_id": 94,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:07.426Z",
        "created_at": "2016-10-18T12:37:07.426Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 540,
        "chapter_id": 95,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:07.509Z",
        "created_at": "2016-10-18T12:37:07.509Z",
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
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 540,
        "chapter_id": 94,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:07.473Z",
        "created_at": "2016-10-18T12:37:07.473Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 540,
        "chapter_id": 95,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:07.556Z",
        "created_at": "2016-10-18T12:37:07.556Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 540,
        "chapter_id": 94,
        "position": 68,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:06.226Z",
        "created_at": "2016-10-18T12:37:06.089Z",
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
            "id": 154,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 155,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 540,
        "chapter_id": 94,
        "position": 69,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:06.434Z",
        "created_at": "2016-10-18T12:37:06.302Z",
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
            "id": 156,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 157,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 540,
        "chapter_id": 95,
        "position": 70,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:06.672Z",
        "created_at": "2016-10-18T12:37:06.530Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 540,
        "chapter_id": 95,
        "position": 71,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T12:37:06.891Z",
        "created_at": "2016-10-18T12:37:06.746Z",
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
            "id": 160,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 161,
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
	-H "Authorization: Bearer d0bfb6990a8a952bc15bc2fc708ec5679965715d9a5487708f0ec1199923fa46"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/179/pin
Content-Type: application/json
Authorization: Bearer dcdec0d4a9e0fb7aa9c5ed9d50164308cbe2caa7edfbfa88939704784f05cf27
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/179/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcdec0d4a9e0fb7aa9c5ed9d50164308cbe2caa7edfbfa88939704784f05cf27"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/193/pin
Content-Type: application/json
Authorization: Bearer 8784b9f4dc7ad2ba0a78cd6df94a6aec59def15347045cf7370bfd4d4008c5fb
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/193/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8784b9f4dc7ad2ba0a78cd6df94a6aec59def15347045cf7370bfd4d4008c5fb"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 10659af7c695a741243cc1eca9a3bf4bd32f5994f2cc0be368e1cbbe2f8aab73
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
    "creator_id": 501,
    "id": 176,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 154,
    "additional_university_ids": [

    ],
    "topic_id": 184,
    "discipline_id": 184,
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
    "updated_at": "2016-10-18T12:37:00.507Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10659af7c695a741243cc1eca9a3bf4bd32f5994f2cc0be368e1cbbe2f8aab73"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 9ff32beb8503a090df7e47d31ae9b74de312c006ccbb10214e974eb8d766f7eb
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
    "id": 477,
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
    "created_at": "2016-10-18T12:36:58.399Z",
    "updated_at": "2016-10-18T12:36:58.399Z",
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
	-H "Authorization: Bearer 9ff32beb8503a090df7e47d31ae9b74de312c006ccbb10214e974eb8d766f7eb"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 70ec0e0cf6d5810be26f1ff1aebe58cc6632530aa38f4df75c707c470d805ca7
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[172]}
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
    "id": 479,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      172
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:36:58.794Z",
    "updated_at": "2016-10-18T12:36:58.829Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[172]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70ec0e0cf6d5810be26f1ff1aebe58cc6632530aa38f4df75c707c470d805ca7"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f14cec65d69d9d711621dfe13f6a2d087204d9525de5d7d7da5c26479ac30577
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
    "id": 481,
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
    "created_at": "2016-10-18T12:36:58.922Z",
    "updated_at": "2016-10-18T12:36:58.922Z",
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
	-H "Authorization: Bearer f14cec65d69d9d711621dfe13f6a2d087204d9525de5d7d7da5c26479ac30577"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a4afe1711b468ee20acace520d68d0d60bfe1aa23505f9cfd347e74972c9a7d8
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[173]}
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
    "id": 480,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      173
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:36:58.872Z",
    "updated_at": "2016-10-18T12:36:58.872Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[173]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4afe1711b468ee20acace520d68d0d60bfe1aa23505f9cfd347e74972c9a7d8"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 24ff2ac5217d8231efc38514275533161de456ecdb9bfa8f7358c9b5262a2575
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

171
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
    "id": 478,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/7064b0772ca38c608453a2995edfd67ef99f691a.jpg",
    "university_id": null,
    "fields_of_study": [
      171
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T12:36:58.494Z",
    "updated_at": "2016-10-18T12:36:58.744Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/b2656f4297366d6211f1021520c3e53dad3c73a7.jpg",
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

171
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 24ff2ac5217d8231efc38514275533161de456ecdb9bfa8f7358c9b5262a2575"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 1dc6ba535a16cc54087006c4529c68bdaf08dbbc0dc5788b07aa3f6a38e98156
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
      "bookmarkable_id": 110,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 111,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 112,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1dc6ba535a16cc54087006c4529c68bdaf08dbbc0dc5788b07aa3f6a38e98156"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 2b183e22020a8cd85606ee460d506a05f3ac541d6d100f58d8307bf175cdfd76
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
      "company_id": 13,
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
      "company_id": 14,
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
	-H "Authorization: Bearer 2b183e22020a8cd85606ee460d506a05f3ac541d6d100f58d8307bf175cdfd76"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 7d0667d29421e94452cb1425ff949019f5eb764fd479c01ed1a05b2d2c867288
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
      "company_id": 9,
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
	-H "Authorization: Bearer 7d0667d29421e94452cb1425ff949019f5eb764fd479c01ed1a05b2d2c867288"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 95ea63903c555935a6e38de4bd224566cb7607eeecbfb75b35ef6b495f45fcab
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
      "creator_id": 809,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-225",
      "html_url": "https://goskive.com/course/mit-course-225",
      "slug": "mit-course-225",
      "university_id": 251,
      "additional_university_ids": [

      ],
      "topic_id": 277,
      "discipline_id": 278,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 225",
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
      "updated_at": "2016-10-18T12:37:30.039Z",
      "shortname": "mit-course-225"
    },
    {
      "creator_id": 810,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-226",
      "html_url": "https://goskive.com/course/mit-course-226",
      "slug": "mit-course-226",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "topic_id": 278,
      "discipline_id": 279,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 226",
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
      "updated_at": "2016-10-18T12:37:30.162Z",
      "shortname": "mit-course-226"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95ea63903c555935a6e38de4bd224566cb7607eeecbfb75b35ef6b495f45fcab"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 9f7dac108aa816d8ed92de7721b32e2797f9465fb9195afdc4c85b6d6114522e
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:36:20.777Z"
      },
      "created_at": "2016-10-18T12:36:20.781Z",
      "updated_at": "2016-10-18T12:36:20.781Z",
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 7",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:36:20.791Z"
      },
      "created_at": "2016-10-18T12:36:20.795Z",
      "updated_at": "2016-10-18T12:36:20.795Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f7dac108aa816d8ed92de7721b32e2797f9465fb9195afdc4c85b6d6114522e"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 527a7cb13f72b0296e99f9a129f0b6c0994ffe2c6a18b2a534fe99b054330501
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
      "company_id": 2,
      "company": {
        "id": 2,
        "name": "Fake Company Name 2",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:36:20.284Z"
      },
      "created_at": "2016-10-18T12:36:20.289Z",
      "updated_at": "2016-10-18T12:36:20.289Z",
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
      "company_id": 3,
      "company": {
        "id": 3,
        "name": "Fake Company Name 3",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-18T12:36:20.309Z"
      },
      "created_at": "2016-10-18T12:36:20.312Z",
      "updated_at": "2016-10-18T12:36:20.312Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 527a7cb13f72b0296e99f9a129f0b6c0994ffe2c6a18b2a534fe99b054330501"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 62a70d9157e34f0ce7279880dba03ec18e7410aadae104f99748d13ead006714
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
      "id": 15,
      "created_at": "2016-10-18T12:37:21.927Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-10-18T12:37:22.038Z",
      "author_id": "684",
      "thread_subject_id": "228",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-18T12:37:22.024Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-10-18T12:37:22.041Z",
      "author_id": "687",
      "thread_subject_id": "229",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-18T12:37:22.461Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-18T12:37:22.461Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-18T12:37:22.885Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-10-18T12:37:22.885Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-18T12:37:23.310Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-18T12:37:23.310Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-18T12:37:23.638Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 107,
      "updated_at": "2016-10-18T12:37:23.638Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-18T12:37:23.979Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 108,
      "updated_at": "2016-10-18T12:37:23.979Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-18T12:37:24.345Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 109,
      "updated_at": "2016-10-18T12:37:24.345Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62a70d9157e34f0ce7279880dba03ec18e7410aadae104f99748d13ead006714"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/23
Content-Type: application/json
Authorization: Bearer 886f355be72c855ffcbe7876ba14b24c52d73b6ba31330167659dd659203232e
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-18T12:27:24.000Z"}}
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
    "id": 23,
    "created_at": "2016-10-18T12:37:24.546Z",
    "read_at": "2016-10-18T12:27:24.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 60,
    "updated_at": "2016-10-18T12:37:24.587Z",
    "author_id": "713",
    "thread_subject_id": "236",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/23" -d '{"notification":{"read_at":"2016-10-18T12:27:24.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 886f355be72c855ffcbe7876ba14b24c52d73b6ba31330167659dd659203232e"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9e72d985bd86ee836f52265a4e112dc08aa05fa5bd31d172951c6efecdcfe27f
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
      "id": 2,
      "course_id": 169,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T12:36:59.387Z",
      "course_published": true,
      "updated_at": "2016-10-18T12:36:59.378Z"
    },
    {
      "id": 3,
      "course_id": 170,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T12:36:59.471Z",
      "course_published": true,
      "updated_at": "2016-10-18T12:36:59.463Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e72d985bd86ee836f52265a4e112dc08aa05fa5bd31d172951c6efecdcfe27f"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer f547d5aa21ddcd20ae194f77431be40f1fe35996c94641381a6581efbc2a5771
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
    "course_id": 168,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T12:36:59.191Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:36:59.181Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f547d5aa21ddcd20ae194f77431be40f1fe35996c94641381a6581efbc2a5771"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 6b883e9e8fcb3b29294f5897ee9b63b5d235b532edf3ca631c635062ad324b7b
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
    "course_id": 173,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-18T12:36:59.878Z",
    "course_published": true,
    "updated_at": "2016-10-18T12:36:59.866Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b883e9e8fcb3b29294f5897ee9b63b5d235b532edf3ca631c635062ad324b7b"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer da09bc1d8d65263a9c2f3d078fb16f85f54c5479ebe8626b49caba9dca53e9c0
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
      "votable_id": 125,
      "user_id": 915
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 126,
      "user_id": 915
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 127,
      "user_id": 915
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 915
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da09bc1d8d65263a9c2f3d078fb16f85f54c5479ebe8626b49caba9dca53e9c0"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/234
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
    "id": 234,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 232,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 234
      },
      {
        "id": 233,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 234
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/234" -X GET \
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
      "id": 232,
      "name": "Function-based solution-oriented analyzer",
      "name_translations": {
        "en": "Function-based solution-oriented analyzer"
      }
    },
    {
      "id": 233,
      "name": "Reactive optimal circuit",
      "name_translations": {
        "en": "Reactive optimal circuit"
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
Authorization: Bearer 7d21da4f33712081fb64e48628618be34000dd84eeebee3ad9415aa9b0f3a4c7
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
    "user_id": 314,
    "feedbackable_id": 10,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-18T12:36:44.833Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d21da4f33712081fb64e48628618be34000dd84eeebee3ad9415aa9b0f3a4c7"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer 7b39389ba9afedc46980a25c7486dbc38500255104ad3aa061ef39cde519ea75
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
    "id": 24,
    "user_id": 304,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-18T12:36:44.279Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b39389ba9afedc46980a25c7486dbc38500255104ad3aa061ef39cde519ea75"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer d435bbfa284fa858e751ed9b470211774f09733c58069da8248f456e4d080879
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
    "id": 20,
    "user_id": 282,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:36:43.069Z",
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
curl "api.goskive.com/v2/feedbacks/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d435bbfa284fa858e751ed9b470211774f09733c58069da8248f456e4d080879"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer 77f67bf936fdc21e877b34a4706136c8284ba42eedb6824baf4b6dfb96ce93f5
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
	-H "Authorization: Bearer 77f67bf936fdc21e877b34a4706136c8284ba42eedb6824baf4b6dfb96ce93f5"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 44e7ba251f1a97a3b0d007975d27f74f0bd79e0930cfa3e2852c3a28efdb8a0b
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
	-H "Authorization: Bearer 44e7ba251f1a97a3b0d007975d27f74f0bd79e0930cfa3e2852c3a28efdb8a0b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/close
Content-Type: application/json
Authorization: Bearer baa34e47e4d6e450bcfdaaf275f0d5f5761c0db528100b7568c1329fb6bea93a
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
curl "api.goskive.com/v2/feedbacks/28/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer baa34e47e4d6e450bcfdaaf275f0d5f5761c0db528100b7568c1329fb6bea93a"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/21
Content-Type: application/json
Authorization: Bearer d1e355e8bf6563bc8e339eb5dd70da6062fba9cc056df1da35031ac726a494bb
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
    "id": 21,
    "user_id": 287,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:36:43.406Z",
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
curl "api.goskive.com/v2/feedbacks/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1e355e8bf6563bc8e339eb5dd70da6062fba9cc056df1da35031ac726a494bb"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/3
Authorization: Bearer 09284126b62826120af144c8ea673d1473976d67e75c5764d5fd9daa234ab827
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
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Authorization: Bearer 09284126b62826120af144c8ea673d1473976d67e75c5764d5fd9daa234ab827" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer 11f2569bde939417aa09130fc0bda4fa93f81c332721a2ff8ebf13f8c130449d
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Authorization: Bearer 11f2569bde939417aa09130fc0bda4fa93f81c332721a2ff8ebf13f8c130449d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/2
Authorization: Bearer 208bcdd2762b4e24212f9d574ca705508f33f7e7645fac923893a96a22daec2f
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/115b9e55a5c84f269cd66d25e6bbb423.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T123651Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=d6202c1d5095b2c6dfc1b3a4a75154ef78dd5fb645928877c0373ca244901a79"
  }
}
```



```shell
curl "api.goskive.com/v2/files/2" -X GET \
	-H "Authorization: Bearer 208bcdd2762b4e24212f9d574ca705508f33f7e7645fac923893a96a22daec2f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer 57fa6a146c5bbd8af8d38b67c0f382ae19d84e2a8fba42cabfceba02707116cd
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
      "id": 402,
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
      "created_at": "2016-10-18T12:36:52.395Z",
      "updated_at": "2016-10-18T12:36:52.395Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-18T12:36:52.470Z",
    "updated_at": "2016-10-18T12:36:52.470Z",
    "course_id": 149,
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
	-H "Authorization: Bearer 57fa6a146c5bbd8af8d38b67c0f382ae19d84e2a8fba42cabfceba02707116cd" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/13/matched_courses?required_cu_count=2
Authorization: Bearer 803bcd0c84f7cbaaf9c146e2adae1e122b9ec33c4204ae740689cd2bf0cab1c9
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
      "creator_id": 893,
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 275,
      "additional_university_ids": [

      ],
      "topic_id": 301,
      "discipline_id": 302,
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
      "chapters_updated_at": "2016-10-18T12:37:35.238Z",
      "updated_at": "2016-10-18T12:37:36.846Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 898,
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-669e8d4c-ca81-40b8-ad5a-6f328ffbc51e",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-669e8d4c-ca81-40b8-ad5a-6f328ffbc51e",
      "slug": "mit-the-great-british-bake-off-669e8d4c-ca81-40b8-ad5a-6f328ffbc51e",
      "university_id": 276,
      "additional_university_ids": [

      ],
      "topic_id": 302,
      "discipline_id": 303,
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
      "chapters_updated_at": "2016-10-18T12:37:35.238Z",
      "updated_at": "2016-10-18T12:37:37.411Z",
      "shortname": "mit-the-great-british-bake-off-669e8d4c-ca81-40b8-ad5a-6f328ffbc51e"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/13/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 803bcd0c84f7cbaaf9c146e2adae1e122b9ec33c4204ae740689cd2bf0cab1c9"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/1/preview
Authorization: Bearer 810c6ccc14f716f152839a6e8e7413f8156c00e9a4038989975797bbc78f6fb3
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/afaebdabfeb2dab413e7673e8517faad.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T123651Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=fbf443d5a4fcc11f2e4849a2b2fba9c7cd359c535a53c0f7e729220695d882e3"
  }
}
```



```shell
curl "api.goskive.com/v2/files/1/preview" -X GET \
	-H "Authorization: Bearer 810c6ccc14f716f152839a6e8e7413f8156c00e9a4038989975797bbc78f6fb3"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/6/report
Authorization: Bearer cb86464d5a6e3ce8a3f40b0671596a2dca4de88a3f039f19ae95d24a08c1e056
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
curl "api.goskive.com/v2/files/6/report" -d '' -X PUT \
	-H "Authorization: Bearer cb86464d5a6e3ce8a3f40b0671596a2dca4de88a3f039f19ae95d24a08c1e056" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/21/comments
Content-Type: application/json
Authorization: Bearer fd1835f55ab9cb8ecccbeffc55dace61d3b11e97583de4b98ac4f3f81312332f
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
    "id": 48,
    "author_id": 460,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:36:57.350Z",
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
curl "api.goskive.com/v2/flashcards/21/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd1835f55ab9cb8ecccbeffc55dace61d3b11e97583de4b98ac4f3f81312332f"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/23/comments
Content-Type: application/json
Authorization: Bearer 70322bd6c83e90945b2f0a38fb855bc27016c102f6c88d246afca314832da5cd
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
    "author_id": 466,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:36:57.852Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 466,
      "feedbackable_id": 23,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:57.849Z",
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
curl "api.goskive.com/v2/flashcards/23/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70322bd6c83e90945b2f0a38fb855bc27016c102f6c88d246afca314832da5cd"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/25/comments
Content-Type: application/json
Authorization: Bearer 5e90e9608539bebd8371e56f4b7c326f0cd6513876b758e7641f78e4e6b99b1c
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
      "id": 50,
      "author_id": 475,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:58.334Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 476,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:36:58.350Z",
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
curl "api.goskive.com/v2/flashcards/25/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e90e9608539bebd8371e56f4b7c326f0cd6513876b758e7641f78e4e6b99b1c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/22/comments
Content-Type: application/json
Authorization: Bearer a73132507c18bd585b961a8bbe2f55355cf37ac80eae82f747e72b24b10522b3
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
curl "api.goskive.com/v2/flashcards/22/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a73132507c18bd585b961a8bbe2f55355cf37ac80eae82f747e72b24b10522b3"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/52/feedbacks
Content-Type: application/json
Authorization: Bearer 715956a221d6cac42ac3e99b31297383c42dea4dba409428623463f7f8d2694a
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
    "id": 39,
    "user_id": 582,
    "feedbackable_id": 52,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:37:12.815Z",
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
curl "api.goskive.com/v2/flashcards/52/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 715956a221d6cac42ac3e99b31297383c42dea4dba409428623463f7f8d2694a"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/55/feedbacks
Content-Type: application/json
Authorization: Bearer 68b56e25d0b0abb3c0cd25b40d0ade6e308adfa62f0baaa7a5493fd2a6a3d6e2
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
      "user_id": 595,
      "feedbackable_id": 55,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:37:13.611Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 594,
      "feedbackable_id": 55,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:37:13.600Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/55/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68b56e25d0b0abb3c0cd25b40d0ade6e308adfa62f0baaa7a5493fd2a6a3d6e2"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/2/votes
Content-Type: application/json
Authorization: Bearer 9ebdfe001095978214e0b3be557fbfb2ffc8ab59998ad384896c6dd177fdb33a
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
      "votable_id": 2,
      "user_id": 12
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 11
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 2,
      "user_id": 10
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ebdfe001095978214e0b3be557fbfb2ffc8ab59998ad384896c6dd177fdb33a"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/81/republish
Content-Type: application/json
Authorization: Bearer 89568014e568128bd57f411bcb6b116a188f4f497b2a0e98219dcd8616616d92
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
curl "api.goskive.com/v2/flashcards/81/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89568014e568128bd57f411bcb6b116a188f4f497b2a0e98219dcd8616616d92"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/83/bookmark
Content-Type: application/json
Authorization: Bearer f8853c939b2745441c6c7c25063906c83bf3b7fb6f276b962fa4778d4eaf1ce4
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/83/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8853c939b2745441c6c7c25063906c83bf3b7fb6f276b962fa4778d4eaf1ce4"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/80
Content-Type: application/json
Authorization: Bearer 2202ed2285eceb9f875788391f33af08d13a9d4e9624cde46ce58847e0ca44ee
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/80" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2202ed2285eceb9f875788391f33af08d13a9d4e9624cde46ce58847e0ca44ee"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/60/downvote
Content-Type: application/json
Authorization: Bearer ae68eb1ae3a4fee46fce339f0a95bd504daab0e57eb6a0e18bb53ce4379d33b1
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
	-H "Authorization: Bearer ae68eb1ae3a4fee46fce339f0a95bd504daab0e57eb6a0e18bb53ce4379d33b1"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/78
Content-Type: application/json
Authorization: Bearer d0aa8da1ea7466ddc51391bbbe9e57d15930c10d9578f0563122a054bf98ddb0
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
    "author_id": 774,
    "chapter_id": 144,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:37:28.020Z",
    "created_at": "2016-10-18T12:37:28.020Z",
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
	-H "Authorization: Bearer d0aa8da1ea7466ddc51391bbbe9e57d15930c10d9578f0563122a054bf98ddb0"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/62/report
Content-Type: application/json
Authorization: Bearer d1641115ee3ad0cdb5dc4fca539e7f763bcca6904342ecd569d513d3d66361f7
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/62/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1641115ee3ad0cdb5dc4fca539e7f763bcca6904342ecd569d513d3d66361f7"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/61/bookmark
Content-Type: application/json
Authorization: Bearer 98dab4120d85e2098adc2db7aa0b642ebbddf29f6d35feb6671ef8f4221f9553
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98dab4120d85e2098adc2db7aa0b642ebbddf29f6d35feb6671ef8f4221f9553"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/79/upvote
Content-Type: application/json
Authorization: Bearer 4347eb3ba2060b24c039ff2c27df1c51f889a23d51c8ec91330f40e987195b10
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/79/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4347eb3ba2060b24c039ff2c27df1c51f889a23d51c8ec91330f40e987195b10"
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
    "key": "cache/c873158b013c696dd851904e11640fc3.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMzozNzozN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9jODczMTU4YjAxM2M2OTZkZDg1MTkwNGUxMTY0MGZjMy5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOFQxMjM3MzdaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T123737Z",
    "x-amz-signature": "688267c7d0e1d59c11408fb7f779865fb356d3de66333094ebfc3283dc5fa04a"
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
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer eaff4168d02e0dbc37ec0bd4c604fac288b5eaa12eaba8f598cec05ba1b493fb
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
curl "api.goskive.com/v2/me/jobs/7/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaff4168d02e0dbc37ec0bd4c604fac288b5eaa12eaba8f598cec05ba1b493fb"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 36fea23495398ed7ff51817c983bcbdc24a0d03519a1f2703bdf3f86569be65c
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
	-H "Authorization: Bearer 36fea23495398ed7ff51817c983bcbdc24a0d03519a1f2703bdf3f86569be65c"
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
{"password":{"reset_password_token":"iyCnJGrHNqbVnTJ3NrGy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 639,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-18T12:37:16.461Z",
  "updated_at": "2016-10-18T12:37:16.593Z",
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
  "audit_id": 4332
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"iyCnJGrHNqbVnTJ3NrGy","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/90/comments
Content-Type: application/json
Authorization: Bearer c42dd355fd782d9512a8ba5cea27741d756ca72e47a324787e82af6c1461d2c4
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
    "author_id": 568,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:37:11.380Z",
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
curl "api.goskive.com/v2/questions/90/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c42dd355fd782d9512a8ba5cea27741d756ca72e47a324787e82af6c1461d2c4"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/89/comments
Content-Type: application/json
Authorization: Bearer dd5df46e2bb859c81fa0347f2cb20d0dd5ddb078c496dfc3132505dc60d730e7
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
    "author_id": 565,
    "reply_to_id": null,
    "created_at": "2016-10-18T12:37:10.885Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 565,
      "feedbackable_id": 89,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:37:10.883Z",
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
curl "api.goskive.com/v2/questions/89/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd5df46e2bb859c81fa0347f2cb20d0dd5ddb078c496dfc3132505dc60d730e7"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/93/comments
Content-Type: application/json
Authorization: Bearer ba1615778cdc4b59f13826cf46f8c2483f0d16bf8b0b0e7eb15012a1885ff9e5
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
      "id": 54,
      "author_id": 580,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:37:12.555Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 581,
      "reply_to_id": null,
      "created_at": "2016-10-18T12:37:12.571Z",
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
curl "api.goskive.com/v2/questions/93/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba1615778cdc4b59f13826cf46f8c2483f0d16bf8b0b0e7eb15012a1885ff9e5"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/91/comments
Content-Type: application/json
Authorization: Bearer 861d3ea34c3c2465ea1553df5c24282ec35a5d1cf26573928ae4292b2b7b53d9
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
curl "api.goskive.com/v2/questions/91/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 861d3ea34c3c2465ea1553df5c24282ec35a5d1cf26573928ae4292b2b7b53d9"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/53/feedbacks
Content-Type: application/json
Authorization: Bearer c4fae66c2a5117861948bb3fd5bd7a820daa3ae8a6348221fd9609fc735ad481
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
    "id": 30,
    "user_id": 408,
    "feedbackable_id": 53,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-18T12:36:53.373Z",
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
curl "api.goskive.com/v2/questions/53/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4fae66c2a5117861948bb3fd5bd7a820daa3ae8a6348221fd9609fc735ad481"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/56/feedbacks
Content-Type: application/json
Authorization: Bearer fdedc796799bbc92d8909bc1d5e7cf532fe2629cd1e1f59e206484f3c156002f
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
      "user_id": 429,
      "feedbackable_id": 56,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:54.607Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 428,
      "feedbackable_id": 56,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T12:36:54.595Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/56/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdedc796799bbc92d8909bc1d5e7cf532fe2629cd1e1f59e206484f3c156002f"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/50/votes
Content-Type: application/json
Authorization: Bearer e035a90d1867360e3070d37bb11f0ddf5c9a6bc298590f87c019f654f9b9cdfd
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
      "id": 9,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 381
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 380
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 379
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/50/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e035a90d1867360e3070d37bb11f0ddf5c9a6bc298590f87c019f654f9b9cdfd"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/6/republish
Content-Type: application/json
Authorization: Bearer 27e4185b35850d3ee4fb9149a0015d56b57041abd4346830d1afbef58e3fc895
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
	-H "Authorization: Bearer 27e4185b35850d3ee4fb9149a0015d56b57041abd4346830d1afbef58e3fc895"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/23/bookmark
Content-Type: application/json
Authorization: Bearer a87a48eb78559f85c8e30fdff187eefb979c44fe0c98d9259ff1f89f7390b9e1
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/23/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a87a48eb78559f85c8e30fdff187eefb979c44fe0c98d9259ff1f89f7390b9e1"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/2
Content-Type: application/json
Authorization: Bearer 055e674d043e1c7d25651f750f6778b90aec7ee8c66252e335aaebbcf2efabc1
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 055e674d043e1c7d25651f750f6778b90aec7ee8c66252e335aaebbcf2efabc1"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/4/downvote
Content-Type: application/json
Authorization: Bearer 224a89ea3ebf6833b292d616e8e9b4de3c35a749ff9d73d69a6051976095369d
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
	-H "Authorization: Bearer 224a89ea3ebf6833b292d616e8e9b4de3c35a749ff9d73d69a6051976095369d"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/25
Content-Type: application/json
Authorization: Bearer af8f440deb4e3556b73838b64e93dc0981d028dbaa9d61714246e1f67051e5e1
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
    "id": 25,
    "obfuscated_id": "HsmcIJXdRE4",
    "author_id": 192,
    "chapter_id": 28,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:36:36.555Z",
    "created_at": "2016-10-18T12:36:36.427Z",
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
        "id": 50,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 51,
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
curl "api.goskive.com/v2/questions/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af8f440deb4e3556b73838b64e93dc0981d028dbaa9d61714246e1f67051e5e1"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/24/report
Content-Type: application/json
Authorization: Bearer 76e5f56fe12d25c70a112a9ca509fca839e34f62958f44c6ddea11ab908019c2
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76e5f56fe12d25c70a112a9ca509fca839e34f62958f44c6ddea11ab908019c2"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/22/bookmark
Content-Type: application/json
Authorization: Bearer da304fef983943c40effc802eed21e5d9dc8ea2044b09568010f633a39cbee9f
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da304fef983943c40effc802eed21e5d9dc8ea2044b09568010f633a39cbee9f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/3
Content-Type: application/json
Authorization: Bearer 06abdf22b2aaed67112d89022b0b62793454dba9918c74c6e4b6d3071f4403c3
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":3,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T12:36:28.782Z","updated_at":"2016-10-18T12:36:28.900Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":6,"author_id":121,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 3,
    "obfuscated_id": "bco7bNtr_d4",
    "author_id": 121,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T12:36:29.016Z",
    "created_at": "2016-10-18T12:36:28.782Z",
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
    "question": "{\"id\"=>3, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-18T12:36:28.782Z\", \"updated_at\"=>\"2016-10-18T12:36:28.900Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>6, \"author_id\"=>121, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 7,
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
curl "api.goskive.com/v2/questions/3" -d '{"question":{"question":{"id":3,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T12:36:28.782Z","updated_at":"2016-10-18T12:36:28.900Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":6,"author_id":121,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06abdf22b2aaed67112d89022b0b62793454dba9918c74c6e4b6d3071f4403c3"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/1/upvote
Content-Type: application/json
Authorization: Bearer 86f6983932ba56324a7644aec461c56d0ed54f6feb3e12daa4364f467fb0af00
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
	-H "Authorization: Bearer 86f6983932ba56324a7644aec461c56d0ed54f6feb3e12daa4364f467fb0af00"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer af43d01beb69af06086c3b28b13dfd4323fa257af5feecc3f37d133c240c7821
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
      "creator_id": 553,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 203,
      "discipline_id": 203,
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
      "updated_at": "2016-10-18T12:37:09.873Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af43d01beb69af06086c3b28b13dfd4323fa257af5feecc3f37d133c240c7821"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer bb3eb73464716a7fa61ddc7a1df46fdbbf3fb1fcc436300577fe94c1e33293a2
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
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-157",
      "html_url": "https://goskive.com/university/uni-157",
      "slug": "uni-157",
      "name": "National School of Pizza",
      "short_name": "Uni 157",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c72685ebea3f04f881db86f2b9321b15f17ffed1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ff1657156bbf902b7d77943d39c1ded2b6df2483.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:37:10.147Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-156",
      "html_url": "https://goskive.com/university/uni-156",
      "slug": "uni-156",
      "name": "National School of Pastry",
      "short_name": "Uni 156",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e67cdd9b547a5cb8d6c13efbfbaa282915ac7c93.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/87ea52ae18616a658b1566cb7dc9e67594f98a35.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:37:10.129Z",
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
	-H "Authorization: Bearer bb3eb73464716a7fa61ddc7a1df46fdbbf3fb1fcc436300577fe94c1e33293a2"
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
      "id": 45,
      "name": "Enterprise-wide even-keeled flexibility",
      "name_translations": {
        "en": "Enterprise-wide even-keeled flexibility"
      },
      "discipline_id": 45
    },
    {
      "id": 46,
      "name": "Advanced grid-enabled toolset",
      "name_translations": {
        "en": "Advanced grid-enabled toolset"
      },
      "discipline_id": 46
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
GET /v2/topics/47
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
    "id": 47,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 47
  }
}
```



```shell
curl "api.goskive.com/v2/topics/47" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer a54b69cc8d3e057fc3577a8d15144640d5e0711888480bc772bb8e14c7fbf8de
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
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-176",
      "html_url": "https://goskive.com/university/uni-176",
      "slug": "uni-176",
      "name": "University 153",
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
      "updated_at": "2016-10-18T12:37:14.985Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-177",
      "html_url": "https://goskive.com/university/uni-177",
      "slug": "uni-177",
      "name": "University 154",
      "short_name": "Uni 177",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/7e506ff42d87bcdeff60fae98e96c870cd0931ee.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/72fb271ab876c7696a21e499b88793615598afed.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:37:15.002Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 196,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-178",
      "html_url": "https://goskive.com/university/uni-178",
      "slug": "uni-178",
      "name": "University 155",
      "short_name": "Uni 178",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/691708776e2a02229b737f1b2a92b7e25e6e7c3c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a9f145362449dba2911e7ea22ea755d720905381.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T12:37:15.019Z",
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
	-H "Authorization: Bearer a54b69cc8d3e057fc3577a8d15144640d5e0711888480bc772bb8e14c7fbf8de"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 23767d7ff64e83af9221208a79e9316448464c2acac7a9354d04d9a90f6d4574
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
    "id": 197,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/50972f911c8fb0a0bb1619f6e718267a6cd23b42.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51d8573844e06df03da73ce266c4ec618bc3d315.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-18T12:37:15.132Z",
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
	-H "Authorization: Bearer 23767d7ff64e83af9221208a79e9316448464c2acac7a9354d04d9a90f6d4574"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a9998a2ceba0aad79841317b126386f005aa2cf513afb8f5355bacb1321cc2d6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":106,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 331,
    "id": 103,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 106,
    "discipline_id": 106,
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
    "chapters_updated_at": "2016-10-18T12:36:46.154Z",
    "updated_at": "2016-10-18T12:36:46.301Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 57,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-18T12:36:46.250Z",
        "course_id": 103,
        "author_id": 331,
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
        "id": 58,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-18T12:36:46.272Z",
        "course_id": 103,
        "author_id": 331,
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
        "id": 59,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-18T12:36:46.290Z",
        "course_id": 103,
        "author_id": 331,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":106,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9998a2ceba0aad79841317b126386f005aa2cf513afb8f5355bacb1321cc2d6"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 35830c810166645f4cc432c033379553ee23095795cfcd6b19245c2bd056d722
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":105,"published":false}}
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
    "creator_id": 330,
    "id": 102,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 102,
    "additional_university_ids": [

    ],
    "topic_id": 105,
    "discipline_id": 105,
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
    "updated_at": "2016-10-18T12:36:46.120Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":105,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35830c810166645f4cc432c033379553ee23095795cfcd6b19245c2bd056d722"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 91ca1f45396237fc82609ca189b1ff1d94cba1900552dfa102df239e97c68e25
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
      "creator_id": 337,
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "topic_id": 113,
      "discipline_id": 113,
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
      "updated_at": "2016-10-18T12:36:46.882Z",
      "shortname": "fu-course-106"
    },
    {
      "creator_id": 337,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 106,
      "additional_university_ids": [

      ],
      "topic_id": 114,
      "discipline_id": 114,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
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
      "chapters_updated_at": "2016-10-18T12:36:47.198Z",
      "updated_at": "2016-10-18T12:36:47.205Z",
      "shortname": "fu-course-107"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91ca1f45396237fc82609ca189b1ff1d94cba1900552dfa102df239e97c68e25"
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
      "creator_id": 357,
      "id": 126,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-122",
      "html_url": "https://goskive.com/course/fu-course-122",
      "slug": "fu-course-122",
      "university_id": 112,
      "additional_university_ids": [

      ],
      "topic_id": 129,
      "discipline_id": 129,
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
      "updated_at": "2016-10-18T12:36:48.735Z",
      "shortname": "fu-course-122"
    },
    {
      "creator_id": 357,
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 112,
      "additional_university_ids": [

      ],
      "topic_id": 130,
      "discipline_id": 130,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "chapters_updated_at": "2016-10-18T12:36:49.048Z",
      "updated_at": "2016-10-18T12:36:49.054Z",
      "shortname": "fu-course-123"
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
Authorization: Bearer 247dd1da12df4d35550455bc227a6f5e107760beaf92caecbe8de76fe475e912
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
      "creator_id": 343,
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "topic_id": 117,
      "discipline_id": 117,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
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
      "updated_at": "2016-10-18T12:36:47.435Z",
      "shortname": "fu-course-110"
    },
    {
      "creator_id": 343,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "topic_id": 118,
      "discipline_id": 118,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
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
      "updated_at": "2016-10-18T12:36:47.477Z",
      "shortname": "fu-course-111"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 247dd1da12df4d35550455bc227a6f5e107760beaf92caecbe8de76fe475e912"
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
      "creator_id": 362,
      "id": 130,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 114,
      "additional_university_ids": [

      ],
      "topic_id": 133,
      "discipline_id": 133,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "updated_at": "2016-10-18T12:36:49.292Z",
      "shortname": "fu-course-126"
    },
    {
      "creator_id": 362,
      "id": 131,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 114,
      "additional_university_ids": [

      ],
      "topic_id": 134,
      "discipline_id": 134,
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
      "updated_at": "2016-10-18T12:36:49.332Z",
      "shortname": "fu-course-127"
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
Authorization: Bearer 90baa64e2ab1d511d857c18dbf34c3f0003eba72b73ec538cfdfd574abce4a7c
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
  "id": 913,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-18T12:37:38.039Z",
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
	-H "Authorization: Bearer 90baa64e2ab1d511d857c18dbf34c3f0003eba72b73ec538cfdfd574abce4a7c"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/908
Content-Type: application/json
Authorization: Bearer e270889997640b5c439f4bdb6185c626bd91593413c23d0609ddc42a328ca150
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
    "id": 908,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 278,
    "fields_of_study": [
      304,
      305
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-18T12:37:37.726Z",
    "updated_at": "2016-10-18T12:37:37.726Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/908" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e270889997640b5c439f4bdb6185c626bd91593413c23d0609ddc42a328ca150"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/906
Content-Type: application/json
Authorization: Bearer 00bb221e23d9c578a618ca3510e21acf8a82d59ddadc040ff35a5d5cbc4aacc6
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
    "id": 906,
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
    "created_at": "2016-10-18T12:37:37.569Z",
    "updated_at": "2016-10-18T12:37:37.569Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/906" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00bb221e23d9c578a618ca3510e21acf8a82d59ddadc040ff35a5d5cbc4aacc6"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/11
Content-Type: application/json
Authorization: Bearer eed5db35381d3293716c7a5a9ab7ec619549fe159b9a1d9661dc9faf6ea899ab
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eed5db35381d3293716c7a5a9ab7ec619549fe159b9a1d9661dc9faf6ea899ab"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/13
Content-Type: application/json
Authorization: Bearer 910b30c318a0671d9cf8e1c8631ee88894734206531ac89851421e15393eb1cd
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
    "id": 13,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 96,
    "user_id": 649
  }
}
```



```shell
curl "api.goskive.com/v2/votes/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 910b30c318a0671d9cf8e1c8631ee88894734206531ac89851421e15393eb1cd"
```
