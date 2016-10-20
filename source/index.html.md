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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5362de738797b6d5fb04e67cbe2ca4b351dc9db50f5882edd121e00aa3f47f02","client_secret":"83a7b5975ea3bddd795ddb261e7a6938928765aa36ac98ef4533e951499c71bc"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5362de738797b6d5fb04e67cbe2ca4b351dc9db50f5882edd121e00aa3f47f02","client_secret":"83a7b5975ea3bddd795ddb261e7a6938928765aa36ac98ef4533e951499c71bc"}' -X POST \
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
Authorization: Basic MGUzNjJiZmEwN2EwYmMxNjY4MGNjYzZhZTcwNjE4YjQ5YzRiYjhjYWMxOGM3
NWNmOTNhYmY0NDBjYWM4NWE4ZTplNDNjYzBkNzRiMTFmYjBlZWUxMjI1N2Mz
ZGY4OGYwMWU0NmJjN2MwMmQ1ZDIzOTQyYjQ4NTFkNDFlYTc0Zjli

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
	-u 0e362bfa07a0bc16680ccc6ae70618b49c4bb8cac18c75cf93abf440cac85a8e:e43cc0d74b11fb0eee12257c3df88f01e46bc7c02d5d23942b4851d41ea74f9b
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a7d1431ae71b7b40a395d394f6543119df08694d98da6c304c5e7a8409f955e2","client_secret":"c35eec457f52104b2a01ea5d9ecf866979a215f77c0a30cd8c2eb400db11874b"}
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
  "access_token": "497dc965205017b9d0ac90a909ae36ad821d9dc30c2a7b91e5ebaa744eea9480",
  "token_type": "bearer",
  "created_at": 1476956759
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a7d1431ae71b7b40a395d394f6543119df08694d98da6c304c5e7a8409f955e2","client_secret":"c35eec457f52104b2a01ea5d9ecf866979a215f77c0a30cd8c2eb400db11874b"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTMwMzBmZDM2OTU1NTk2NDg1ZWM3ZGZjODQxYjA2NThmNWZlZWE1NzUzOTM3
ZWFjMmFjMGIzZTA5MjM1ZTFhYzo1NDdlZGRhNWQ5MDVmMjVlMTQyYWU5YzAw
NzNhNzkyZTAzNDdhYTQ2YWVhZDViYjMwMWY2MGViZDNhMzExYmUz

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
  "access_token": "90f6947117736cda9bd5a6a20c7ac2390864e1079c2862a4ffd4c85a3c1077e0",
  "token_type": "bearer",
  "created_at": 1476956759
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u a3030fd36955596485ec7dfc841b0658f5feea5753937eac2ac0b3e09235e1ac:547edda5d905f25e142ae9c0073a792e0347aa46aead5bb301f60ebd3a311be3
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
{"grant_type":"client_credentials","client_id":"3ee187c9b0e260db82015bdeb000f955e20e6c508421a8bd27c8f2ba1d1a9ca8","client_secret":"659724ef64dd9baab274112d6be0e74366f02d9a06118efeb8bdceddca005b86"}
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
  "access_token": "9a257e4fa21b04390ebd567b310b53364924fbccef51fdbf51134bb4d29f82f6",
  "token_type": "bearer",
  "created_at": 1476956759
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"3ee187c9b0e260db82015bdeb000f955e20e6c508421a8bd27c8f2ba1d1a9ca8","client_secret":"659724ef64dd9baab274112d6be0e74366f02d9a06118efeb8bdceddca005b86"}' -X POST \
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
GET /v2/campaigns/12
Content-Type: application/json
Authorization: Bearer fb78e034f48cb1b8bbe557c4f22d578e9eee9840da939adcd9dba510ae8ae9d4
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
    "company_id": 21,
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
	-H "Authorization: Bearer fb78e034f48cb1b8bbe557c4f22d578e9eee9840da939adcd9dba510ae8ae9d4"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/152/flashcards
Content-Type: application/json
Authorization: Bearer 83d9c70af7a58298959fd2f2a3b776075968c48fc92c924de5c237892a2f4eca
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":152,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 65,
    "obfuscated_id": "Pu1fo5_Q1vk",
    "author_id": 799,
    "chapter_id": 152,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:41.065Z",
    "created_at": "2016-10-20T09:46:41.065Z",
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
curl "api.goskive.com/v2/chapters/152/flashcards" -d '{"flashcard":{"chapter_id":152,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83d9c70af7a58298959fd2f2a3b776075968c48fc92c924de5c237892a2f4eca"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/153/flashcards
Content-Type: application/json
Authorization: Bearer 720e12e5207b99e0305f6ddff21bf6226b8512974b123540dd66287232052c94
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 800,
      "chapter_id": 153,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:41.209Z",
      "created_at": "2016-10-20T09:46:41.209Z",
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 800,
      "chapter_id": 153,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:41.248Z",
      "created_at": "2016-10-20T09:46:41.248Z",
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 800,
      "chapter_id": 153,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:41.283Z",
      "created_at": "2016-10-20T09:46:41.283Z",
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
curl "api.goskive.com/v2/chapters/153/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 720e12e5207b99e0305f6ddff21bf6226b8512974b123540dd66287232052c94"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/139/questions
Content-Type: application/json
Authorization: Bearer fbb3f90e34354db4fb23445aa0b0c4b045846156c68433a2e2d97a6823bbdb11
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":139,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 67,
    "obfuscated_id": "btMCNJVyvlA",
    "author_id": 725,
    "chapter_id": 139,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:34.046Z",
    "created_at": "2016-10-20T09:46:34.046Z",
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
        "id": 133,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 134,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 135,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 136,
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
curl "api.goskive.com/v2/chapters/139/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":139,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbb3f90e34354db4fb23445aa0b0c4b045846156c68433a2e2d97a6823bbdb11"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/140/questions
Content-Type: application/json
Authorization: Bearer 2f98f7ac46dc752abe2c91b2dba20c31a0901699176b84ebe884a5f0cdbe55d3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":140,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 728,
    "chapter_id": 140,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:34.595Z",
    "created_at": "2016-10-20T09:46:34.595Z",
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
        "id": 137,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 138,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/140/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":140,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f98f7ac46dc752abe2c91b2dba20c31a0901699176b84ebe884a5f0cdbe55d3"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/141/questions
Content-Type: application/json
Authorization: Bearer 26f0b3710bbc7a73ea0647d4789657dfe76629eec348564212e336ccb5eddba5
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":141,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 731,
    "chapter_id": 141,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:34.924Z",
    "created_at": "2016-10-20T09:46:34.924Z",
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
        "id": 139,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 140,
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
curl "api.goskive.com/v2/chapters/141/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":141,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26f0b3710bbc7a73ea0647d4789657dfe76629eec348564212e336ccb5eddba5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/142/questions
Content-Type: application/json
Authorization: Bearer 669aa67e140460423a963ffc30874b3cd944a1245642098931cd02fa4a024c3d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":142,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 734,
    "chapter_id": 142,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:35.252Z",
    "created_at": "2016-10-20T09:46:35.252Z",
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
        "id": 141,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 142,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 143,
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
curl "api.goskive.com/v2/chapters/142/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":142,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 669aa67e140460423a963ffc30874b3cd944a1245642098931cd02fa4a024c3d"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/144/questions
Content-Type: application/json
Authorization: Bearer fa518f5923e632622cc8721e001874bfca6e697e21f5c4a74a419ed076f2d338
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
      "author_id": 740,
      "chapter_id": 144,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:35.886Z",
      "created_at": "2016-10-20T09:46:35.771Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 741,
      "chapter_id": 144,
      "position": 68,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:36.073Z",
      "created_at": "2016-10-20T09:46:35.957Z",
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
    },
    {
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 742,
      "chapter_id": 144,
      "position": 69,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:36.262Z",
      "created_at": "2016-10-20T09:46:36.144Z",
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
          "id": 148,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 149,
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
curl "api.goskive.com/v2/chapters/144/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa518f5923e632622cc8721e001874bfca6e697e21f5c4a74a419ed076f2d338"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/78
Content-Type: application/json
Authorization: Bearer 7683a19d95f490b31d05fdab4221e52bf8436b7dbc7c01522e323afac031e660
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
curl "api.goskive.com/v2/chapters/78" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7683a19d95f490b31d05fdab4221e52bf8436b7dbc7c01522e323afac031e660"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/81
Content-Type: application/json
Authorization: Bearer 8e41bf664990d4bcf9f5ec0e691fbc32f24e27035eaf05570e9ecc115974a934
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
curl "api.goskive.com/v2/chapters/81" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e41bf664990d4bcf9f5ec0e691fbc32f24e27035eaf05570e9ecc115974a934"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/73
Content-Type: application/json
Authorization: Bearer 90258f4bc3a18384cbfc0633033174a7864dfa6a86cc062738e18e3755f5e912
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
curl "api.goskive.com/v2/chapters/73" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90258f4bc3a18384cbfc0633033174a7864dfa6a86cc062738e18e3755f5e912"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/80
Content-Type: application/json
Authorization: Bearer b1b217ac951ef03e5a8ecb66caa3cba6e8d1cfeb994b4ae938b7d7d7bc09baeb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/80" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1b217ac951ef03e5a8ecb66caa3cba6e8d1cfeb994b4ae938b7d7d7bc09baeb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/76
Content-Type: application/json
Authorization: Bearer d92459e382cd002ad9af34f473fc3274cdff98019ef62cc955de504c106eec15
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
    "id": 76,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-20T09:46:13.565Z",
    "course_id": 130,
    "author_id": 446,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-20T09:46:12.951Z",
    "questions_updated_at": "2016-10-20T09:46:12.951Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 450,
        "chapter_id": 76,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:13.544Z",
        "created_at": "2016-10-20T09:46:13.544Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 448,
        "chapter_id": 76,
        "position": 37,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:13.425Z",
        "created_at": "2016-10-20T09:46:13.285Z",
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
            "id": 73,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 74,
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
curl "api.goskive.com/v2/chapters/76" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d92459e382cd002ad9af34f473fc3274cdff98019ef62cc955de504c106eec15"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/74
Content-Type: application/json
Authorization: Bearer 3a26cc8322769dafc942303e137a3e30aa50ce697fd02249506f5c367eab9a1a
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
    "id": 74,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-20T09:46:12.747Z",
    "course_id": 128,
    "author_id": 441,
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
curl "api.goskive.com/v2/chapters/74" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a26cc8322769dafc942303e137a3e30aa50ce697fd02249506f5c367eab9a1a"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer 3c907fffe5cf03b8542d8ebf09a6f5465c90e16b774bd5ef923453747d802027
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
    "id": 57,
    "author_id": 686,
    "reply_to_id": 56,
    "created_at": "2016-10-20T09:46:31.057Z",
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
curl "api.goskive.com/v2/comments/56/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c907fffe5cf03b8542d8ebf09a6f5465c90e16b774bd5ef923453747d802027"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/55/replies
Content-Type: application/json
Authorization: Bearer 2980959313ad0ee0f1534b4ca2d944fb67041e89b594432b4346efe6bbef4838
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
curl "api.goskive.com/v2/comments/55/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2980959313ad0ee0f1534b4ca2d944fb67041e89b594432b4346efe6bbef4838"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 9a71de28c1183644aeb5f48588ca3eb646c114bfa1876b2d26b8b891c3b539e5
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
curl "api.goskive.com/v2/comments/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a71de28c1183644aeb5f48588ca3eb646c114bfa1876b2d26b8b891c3b539e5"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer 7acaba0fc37614d7acc428cc60f18e8548255ea4c774330643fef38ba33dd31f
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
curl "api.goskive.com/v2/comments/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7acaba0fc37614d7acc428cc60f18e8548255ea4c774330643fef38ba33dd31f"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 8cab42befaa9c704e80410e1569c922ddcb806d769d73197424129306006518c
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
	-H "Authorization: Bearer 8cab42befaa9c704e80410e1569c922ddcb806d769d73197424129306006518c"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/9/report
Content-Type: application/json
Authorization: Bearer cae3ec00a9b4572322319237f313acb8bdfc0b3adf8331913deb61b7c0ef85db
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cae3ec00a9b4572322319237f313acb8bdfc0b3adf8331913deb61b7c0ef85db"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/25
Content-Type: application/json
Authorization: Bearer 3d6ff56b7ee513aee512b844d4115e6ad5c4986ce14d0fb1a1eb72fa0a1cd2ac
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
    "updated_at": "2016-10-20T09:46:31.366Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d6ff56b7ee513aee512b844d4115e6ad5c4986ce14d0fb1a1eb72fa0a1cd2ac"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer bc947e079d8324c8961e4b7935be2b2014cd69ea57c6525d2a066d295c56f2be
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
      "updated_at": "2016-10-20T09:46:31.232Z"
    },
    {
      "id": 23,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-20T09:46:31.237Z"
    },
    {
      "id": 24,
      "name": "Fake Company Name 23",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-20T09:46:31.241Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc947e079d8324c8961e4b7935be2b2014cd69ea57c6525d2a066d295c56f2be"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/28/company_profiles
Content-Type: application/json
Authorization: Bearer 2f3db96b54f9a0da500d8754402f9917f3f675c644ac736cc71a029cb8a8342b
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
curl "api.goskive.com/v2/companies/28/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f3db96b54f9a0da500d8754402f9917f3f675c644ac736cc71a029cb8a8342b"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 1f8bfb2bc8c14a353241dc5ab2203bc894fdbadbdaa7d95da801132dec18aceb
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
	-H "Authorization: Bearer 1f8bfb2bc8c14a353241dc5ab2203bc894fdbadbdaa7d95da801132dec18aceb"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 4fdac404bcb4a108642bd95c87ab99604f926bf1055d1e272002cb45468eb8c3
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
      "id": 4,
      "title": "Campaign 4",
      "company_id": 9,
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
      "id": 7,
      "title": "Campaign 7",
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
	-H "Authorization: Bearer 4fdac404bcb4a108642bd95c87ab99604f926bf1055d1e272002cb45468eb8c3"
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
Authorization: Bearer a5dd5de06579bc4814d69470a56d1c0e6f83125a4583255ce1dd792490f82f6b
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
	-H "Authorization: Bearer a5dd5de06579bc4814d69470a56d1c0e6f83125a4583255ce1dd792490f82f6b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2b5aa183cd2dd726413f1b102f7d4a842058948d7ae47115155e3789ca708367
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
    "id": 102,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T09:46:25.725Z",
    "course_id": 203,
    "author_id": 609,
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
	-H "Authorization: Bearer 2b5aa183cd2dd726413f1b102f7d4a842058948d7ae47115155e3789ca708367"
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
      "id": 111,
      "title": "Clever Chapter Title 96",
      "position": 1,
      "updated_at": "2016-10-20T09:46:26.848Z",
      "course_id": 209,
      "author_id": 629,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 112,
      "title": "Clever Chapter Title 97",
      "position": 2,
      "updated_at": "2016-10-20T09:46:26.873Z",
      "course_id": 209,
      "author_id": 630,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 113,
      "title": "Clever Chapter Title 98",
      "position": 3,
      "updated_at": "2016-10-20T09:46:27.122Z",
      "course_id": 209,
      "author_id": 631,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-20T09:46:26.741Z",
      "questions_updated_at": "2016-10-20T09:46:26.741Z",
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
Authorization: Bearer d8776f9f8111a82afa533fe3db422d14f73b4e07a90c2ede7da6df98f0bcadd4
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
      "id": 117,
      "title": "Clever Chapter Title 102",
      "position": 1,
      "updated_at": "2016-10-20T09:46:27.485Z",
      "course_id": 212,
      "author_id": 640,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 118,
      "title": "Clever Chapter Title 103",
      "position": 2,
      "updated_at": "2016-10-20T09:46:27.509Z",
      "course_id": 212,
      "author_id": 641,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 119,
      "title": "Clever Chapter Title 104",
      "position": 3,
      "updated_at": "2016-10-20T09:46:27.756Z",
      "course_id": 212,
      "author_id": 642,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-20T09:46:27.410Z",
      "questions_updated_at": "2016-10-20T09:46:27.410Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8776f9f8111a82afa533fe3db422d14f73b4e07a90c2ede7da6df98f0bcadd4"
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
      "id": 114,
      "title": "Clever Chapter Title 99",
      "position": 1,
      "updated_at": "2016-10-20T09:46:27.318Z",
      "course_id": 211,
      "author_id": 636,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 115,
      "title": "Clever Chapter Title 100",
      "position": 2,
      "updated_at": "2016-10-20T09:46:27.342Z",
      "course_id": 211,
      "author_id": 637,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 116,
      "title": "Clever Chapter Title 101",
      "position": 3,
      "updated_at": "2016-10-20T09:46:27.369Z",
      "course_id": 211,
      "author_id": 638,
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
Authorization: Bearer d9afd88282ad68e31fd6e23eceb74a74adba87852651e7174e83199c9b3e6b23
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
      "id": 120,
      "title": "Clever Chapter Title 105",
      "position": 1,
      "updated_at": "2016-10-20T09:46:27.911Z",
      "course_id": 213,
      "author_id": 647,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 121,
      "title": "Clever Chapter Title 106",
      "position": 2,
      "updated_at": "2016-10-20T09:46:27.934Z",
      "course_id": 213,
      "author_id": 648,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 122,
      "title": "Clever Chapter Title 107",
      "position": 3,
      "updated_at": "2016-10-20T09:46:27.957Z",
      "course_id": 213,
      "author_id": 649,
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
	-H "Authorization: Bearer d9afd88282ad68e31fd6e23eceb74a74adba87852651e7174e83199c9b3e6b23"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer abe22f180c91c333386c1f46ded97afa99e06c6ad80ed691c89a61a5280da44d
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
    "id": 5,
    "course_id": 244,
    "user_id": 764,
    "updated_at": "2016-10-20T09:46:37.820Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abe22f180c91c333386c1f46ded97afa99e06c6ad80ed691c89a61a5280da44d"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 58d3c84622f26adaabd9d2a31a8a616edfe9054db1ae11edf01560740133693c
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
      "id": 1,
      "course_id": 241,
      "user_id": 754,
      "updated_at": "2016-10-20T09:46:37.361Z"
    },
    {
      "id": 2,
      "course_id": 241,
      "user_id": 755,
      "updated_at": "2016-10-20T09:46:37.377Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58d3c84622f26adaabd9d2a31a8a616edfe9054db1ae11edf01560740133693c"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/195/files
Content-Type: application/json
Authorization: Bearer d192d623dea3dfb3706b1e7b19ab90f826a29e4c519abe0982eb2296934fd5de
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
        "id": 584,
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
        "created_at": "2016-10-20T09:46:23.608Z",
        "updated_at": "2016-10-20T09:46:23.608Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T09:46:23.615Z",
      "updated_at": "2016-10-20T09:46:23.615Z",
      "course_id": 195,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 585,
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
        "created_at": "2016-10-20T09:46:23.622Z",
        "updated_at": "2016-10-20T09:46:23.622Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T09:46:23.628Z",
      "updated_at": "2016-10-20T09:46:23.628Z",
      "course_id": 195,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 586,
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
        "created_at": "2016-10-20T09:46:23.635Z",
        "updated_at": "2016-10-20T09:46:23.635Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T09:46:23.641Z",
      "updated_at": "2016-10-20T09:46:23.641Z",
      "course_id": 195,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/195/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d192d623dea3dfb3706b1e7b19ab90f826a29e4c519abe0982eb2296934fd5de"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/197/files
Content-Type: application/json
Authorization: Bearer bbb9940aec850ebfdd155f993796b73c23288b9088d62e5c2cb9134fbfee8e7f
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
      "id": 591,
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
      "created_at": "2016-10-20T09:46:23.854Z",
      "updated_at": "2016-10-20T09:46:23.854Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-20T09:46:23.883Z",
    "updated_at": "2016-10-20T09:46:23.883Z",
    "course_id": 197,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/197/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbb9940aec850ebfdd155f993796b73c23288b9088d62e5c2cb9134fbfee8e7f"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/196/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer b5454032cfd00ed330242d1bc68e1cbad4d6ce1826c88ae127e0f74f9fee3ee4
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
    "key": "cache/af05d5ce8945b4114731202a22ca4548.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMFQxMDo0NjoyM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9hZjA1ZDVjZTg5NDViNDExNDczMTIwMmEyMmNhNDU0OC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAyMC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjBUMDk0NjIzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161020/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161020T094623Z",
    "x-amz-signature": "20741560cf028b03b31ec044be834431e6bc78b75b449b3c2e07b8fa89fd9114"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/196/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5454032cfd00ed330242d1bc68e1cbad4d6ce1826c88ae127e0f74f9fee3ee4"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer a1762548873ae4ec12461aa7ec4f3f8100962f6a3e34090abaa4400c83a08262
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
	-H "Authorization: Bearer a1762548873ae4ec12461aa7ec4f3f8100962f6a3e34090abaa4400c83a08262"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b6de1cac9f7408e5fe8f793893566843ecb611b3d60c149672067aedbd9fe617
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
	-H "Authorization: Bearer b6de1cac9f7408e5fe8f793893566843ecb611b3d60c149672067aedbd9fe617"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 035477edb33b47bbd6e8faf799eadbd42238fe89125cb1d07fd4cf0ba80dab14
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
	-H "Authorization: Bearer 035477edb33b47bbd6e8faf799eadbd42238fe89125cb1d07fd4cf0ba80dab14"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bf013a437709809e618e784636d704f2d6b83dc4267b01fa507749b0c4f57467
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
	-H "Authorization: Bearer bf013a437709809e618e784636d704f2d6b83dc4267b01fa507749b0c4f57467"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 39cd012b467754484a57bf992e093ee759353e33027810793a2322e6e6a88faa
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
	-H "Authorization: Bearer 39cd012b467754484a57bf992e093ee759353e33027810793a2322e6e6a88faa"
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
    "creator_id": 844,
    "id": 273,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 257,
    "additional_university_ids": [

    ],
    "topic_id": 285,
    "discipline_id": 286,
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
    "chapters_updated_at": "2016-10-20T09:46:44.249Z",
    "updated_at": "2016-10-20T09:46:45.720Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 160,
        "title": "Clever Chapter Title 136",
        "position": 1,
        "updated_at": "2016-10-20T09:46:45.675Z",
        "course_id": 273,
        "author_id": 844,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T09:46:44.249Z",
        "questions_updated_at": "2016-10-20T09:46:44.249Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 161,
        "title": "Clever Chapter Title 137",
        "position": 2,
        "updated_at": "2016-10-20T09:46:45.713Z",
        "course_id": 273,
        "author_id": 844,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T09:46:44.249Z",
        "questions_updated_at": "2016-10-20T09:46:44.249Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 844,
        "chapter_id": 160,
        "position": 79,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:44.473Z",
        "created_at": "2016-10-20T09:46:44.353Z",
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
            "id": 168,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 169,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 844,
        "chapter_id": 161,
        "position": 81,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:44.856Z",
        "created_at": "2016-10-20T09:46:44.733Z",
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
Authorization: Bearer a99dabd7303626edbe1af55176cf157ef3b4749d5a21b669e7639869dcaef3cb
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
    "creator_id": 849,
    "id": 274,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 258,
    "additional_university_ids": [

    ],
    "topic_id": 286,
    "discipline_id": 287,
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
    "chapters_updated_at": "2016-10-20T09:46:45.776Z",
    "updated_at": "2016-10-20T09:46:47.221Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 162,
        "title": "Clever Chapter Title 138",
        "position": 1,
        "updated_at": "2016-10-20T09:46:47.174Z",
        "course_id": 274,
        "author_id": 849,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T09:46:45.776Z",
        "questions_updated_at": "2016-10-20T09:46:45.776Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 163,
        "title": "Clever Chapter Title 139",
        "position": 2,
        "updated_at": "2016-10-20T09:46:47.214Z",
        "course_id": 274,
        "author_id": 849,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T09:46:45.776Z",
        "questions_updated_at": "2016-10-20T09:46:45.776Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 850,
        "chapter_id": 162,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:47.011Z",
        "created_at": "2016-10-20T09:46:47.011Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 850,
        "chapter_id": 163,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:47.084Z",
        "created_at": "2016-10-20T09:46:47.084Z",
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
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 850,
        "chapter_id": 162,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:47.053Z",
        "created_at": "2016-10-20T09:46:47.053Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 850,
        "chapter_id": 163,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:47.124Z",
        "created_at": "2016-10-20T09:46:47.124Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 850,
        "chapter_id": 162,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:45.995Z",
        "created_at": "2016-10-20T09:46:45.882Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 850,
        "chapter_id": 162,
        "position": 86,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:46.169Z",
        "created_at": "2016-10-20T09:46:46.060Z",
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
      },
      {
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 850,
        "chapter_id": 163,
        "position": 87,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:46.379Z",
        "created_at": "2016-10-20T09:46:46.258Z",
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
            "id": 184,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 185,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 850,
        "chapter_id": 163,
        "position": 88,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:46.559Z",
        "created_at": "2016-10-20T09:46:46.446Z",
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
            "id": 186,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 187,
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
	-H "Authorization: Bearer a99dabd7303626edbe1af55176cf157ef3b4749d5a21b669e7639869dcaef3cb"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/271/pin
Content-Type: application/json
Authorization: Bearer 4206b3f61d36bee7e3a4816d8dde2f030e317ad737b7616fda62e9f8a50099c5
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/271/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4206b3f61d36bee7e3a4816d8dde2f030e317ad737b7616fda62e9f8a50099c5"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/272/pin
Content-Type: application/json
Authorization: Bearer 424d19f4f5fb9726343ea443c0c6f9d0ec99a7ae7d9dded17d8dfa817b95e820
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/272/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 424d19f4f5fb9726343ea443c0c6f9d0ec99a7ae7d9dded17d8dfa817b95e820"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0845e36b6d797850356aba72af56bcbd3f6c7421d1d20eb3cc43c1a9d7878275
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
    "creator_id": 837,
    "id": 269,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 253,
    "additional_university_ids": [

    ],
    "topic_id": 281,
    "discipline_id": 282,
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
    "updated_at": "2016-10-20T09:46:43.846Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0845e36b6d797850356aba72af56bcbd3f6c7421d1d20eb3cc43c1a9d7878275"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 4e36d8786d05c00f894a68c39a5907efc1b4560b0b4fa01d601bbb873af7cb76
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
    "id": 431,
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
    "created_at": "2016-10-20T09:46:11.783Z",
    "updated_at": "2016-10-20T09:46:11.783Z",
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
	-H "Authorization: Bearer 4e36d8786d05c00f894a68c39a5907efc1b4560b0b4fa01d601bbb873af7cb76"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 70a544e0e55e31bcee57a2d668fa2e860a48005e419602eb861bacbc68846473
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[130]}
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
    "id": 433,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      130
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T09:46:12.220Z",
    "updated_at": "2016-10-20T09:46:12.255Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[130]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70a544e0e55e31bcee57a2d668fa2e860a48005e419602eb861bacbc68846473"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer bb155ff256e054dcbe24488e8b9023352222cfeefe60281767082ff09ba87bd5
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
    "id": 435,
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
    "created_at": "2016-10-20T09:46:12.345Z",
    "updated_at": "2016-10-20T09:46:12.345Z",
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
	-H "Authorization: Bearer bb155ff256e054dcbe24488e8b9023352222cfeefe60281767082ff09ba87bd5"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 981b99a4836d2cb316a2493e0a9a54d19097ded4ceaba71ea766a1ab08470a84
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[131]}
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
    "id": 434,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      131
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T09:46:12.295Z",
    "updated_at": "2016-10-20T09:46:12.295Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[131]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 981b99a4836d2cb316a2493e0a9a54d19097ded4ceaba71ea766a1ab08470a84"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer dca9a381edf6549c8e47df67670df12ca42880320929f8edf7cbd27be20c2d4b
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

129
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
    "id": 432,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/c11afb91f92b8f7ba18e73395464b1284eb97913.jpg",
    "university_id": null,
    "fields_of_study": [
      129
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T09:46:11.874Z",
    "updated_at": "2016-10-20T09:46:12.169Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/60a19764f045cf004e8c1febe52bb94cf5c29098.jpg",
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

129
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer dca9a381edf6549c8e47df67670df12ca42880320929f8edf7cbd27be20c2d4b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 355bcebf4d845e8e649c54235ee91ae555113313b7e39d584c042b6434864dc2
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
      "bookmarkable_id": 78,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 79,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 80,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 355bcebf4d845e8e649c54235ee91ae555113313b7e39d584c042b6434864dc2"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer fdfa17f2a8163c5a01f56a39a595a53a8b8b842f8fa66a083df0b43208784565
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
	-H "Authorization: Bearer fdfa17f2a8163c5a01f56a39a595a53a8b8b842f8fa66a083df0b43208784565"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 74f351c716f6c12aadf4efa6deef97f308cf3e7d80c9aa23579a8adec88c780f
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
	-H "Authorization: Bearer 74f351c716f6c12aadf4efa6deef97f308cf3e7d80c9aa23579a8adec88c780f"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer a171cf9ad0c8e9bce338ce603e679811b91db2d701b12637549d8540cb3c28dd
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
      "creator_id": 811,
      "id": 256,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-203",
      "html_url": "https://goskive.com/course/mit-course-203",
      "slug": "mit-course-203",
      "university_id": 240,
      "additional_university_ids": [

      ],
      "topic_id": 268,
      "discipline_id": 269,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
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
      "updated_at": "2016-10-20T09:46:41.824Z",
      "shortname": "mit-course-203"
    },
    {
      "creator_id": 812,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-204",
      "html_url": "https://goskive.com/course/mit-course-204",
      "slug": "mit-course-204",
      "university_id": 241,
      "additional_university_ids": [

      ],
      "topic_id": 269,
      "discipline_id": 270,
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
      "updated_at": "2016-10-20T09:46:41.903Z",
      "shortname": "mit-course-204"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a171cf9ad0c8e9bce338ce603e679811b91db2d701b12637549d8540cb3c28dd"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 03422d698a4fdf4ec378d8a9a692e02cadf40cea4163da98625afb647c14b8a3
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
        "updated_at": "2016-10-20T09:47:00.525Z"
      },
      "created_at": "2016-10-20T09:47:00.529Z",
      "updated_at": "2016-10-20T09:47:00.529Z",
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
        "updated_at": "2016-10-20T09:47:00.537Z"
      },
      "created_at": "2016-10-20T09:47:00.541Z",
      "updated_at": "2016-10-20T09:47:00.541Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03422d698a4fdf4ec378d8a9a692e02cadf40cea4163da98625afb647c14b8a3"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 255c7db7f21e02334fbf4ae4a0a6e9ed9609091fd9f9009b51fec4be056f8739
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
        "updated_at": "2016-10-20T09:47:00.357Z"
      },
      "created_at": "2016-10-20T09:47:00.360Z",
      "updated_at": "2016-10-20T09:47:00.360Z",
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
        "updated_at": "2016-10-20T09:47:00.375Z"
      },
      "created_at": "2016-10-20T09:47:00.378Z",
      "updated_at": "2016-10-20T09:47:00.378Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 255c7db7f21e02334fbf4ae4a0a6e9ed9609091fd9f9009b51fec4be056f8739"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 82ecde156029c5ae3fdfe937c9eb8c02e36cfa0e3432ca718c9f7453c7b2427c
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
      "created_at": "2016-10-20T09:46:31.718Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-10-20T09:46:31.829Z",
      "author_id": "697",
      "thread_subject_id": "225",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-20T09:46:31.815Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 60,
      "updated_at": "2016-10-20T09:46:31.833Z",
      "author_id": "700",
      "thread_subject_id": "226",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-20T09:46:32.199Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-10-20T09:46:32.199Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-20T09:46:32.571Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-20T09:46:32.571Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-20T09:46:32.943Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-10-20T09:46:32.943Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-20T09:46:33.239Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 64,
      "updated_at": "2016-10-20T09:46:33.239Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-20T09:46:33.549Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 65,
      "updated_at": "2016-10-20T09:46:33.549Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-20T09:46:33.848Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 66,
      "updated_at": "2016-10-20T09:46:33.848Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82ecde156029c5ae3fdfe937c9eb8c02e36cfa0e3432ca718c9f7453c7b2427c"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer ac02bb4d99a133cba7672118b1fa14750d2856098b29791469841f533d6479bd
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-20T09:36:31.000Z"}}
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
    "id": 14,
    "created_at": "2016-10-20T09:46:31.513Z",
    "read_at": "2016-10-20T09:36:31.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-10-20T09:46:31.571Z",
    "author_id": "692",
    "thread_subject_id": "224",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-10-20T09:36:31.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac02bb4d99a133cba7672118b1fa14750d2856098b29791469841f533d6479bd"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 00c4d1915f3c754a706b01777728c25151319c4d17e3ea0e68858c9678407cd2
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
      "course_id": 39,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-20T09:45:54.572Z",
      "course_published": true,
      "updated_at": "2016-10-20T09:45:54.564Z"
    },
    {
      "id": 3,
      "course_id": 40,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-20T09:45:54.649Z",
      "course_published": true,
      "updated_at": "2016-10-20T09:45:54.641Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00c4d1915f3c754a706b01777728c25151319c4d17e3ea0e68858c9678407cd2"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer e3c5d20c17994a3050e224d3666306825d104a56f44d3447522291dc207d2b9b
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
    "course_id": 38,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-20T09:45:54.381Z",
    "course_published": true,
    "updated_at": "2016-10-20T09:45:54.372Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3c5d20c17994a3050e224d3666306825d104a56f44d3447522291dc207d2b9b"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 2f490e12c7731df907214ad957e158a6221ed279a2531ad9f37dc02a2ca2d69f
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
    "course_id": 43,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-20T09:45:55.030Z",
    "course_published": true,
    "updated_at": "2016-10-20T09:45:55.019Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f490e12c7731df907214ad957e158a6221ed279a2531ad9f37dc02a2ca2d69f"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 61d6f27ab1b8aa08a08ca8da9b6a8253ac54439e575fb7039fff4a4a5c3f7567
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
      "votable_id": 47,
      "user_id": 592
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 48,
      "user_id": 592
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 592
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 592
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61d6f27ab1b8aa08a08ca8da9b6a8253ac54439e575fb7039fff4a4a5c3f7567"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/252
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
    "id": 252,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 250,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 252
      },
      {
        "id": 251,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 252
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/252" -X GET \
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
      "id": 250,
      "name": "Synergistic web-enabled orchestration",
      "name_translations": {
        "en": "Synergistic web-enabled orchestration"
      }
    },
    {
      "id": 251,
      "name": "Synergistic scalable moratorium",
      "name_translations": {
        "en": "Synergistic scalable moratorium"
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
PATCH /v2/feedbacks/2/close
Content-Type: application/json
Authorization: Bearer cb84a54cab9904e10bf6305425ec5e69ea5553b1cb544cbe120c4710d9a9c1b2
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
    "id": 2,
    "user_id": 9,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-20T09:45:43.179Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb84a54cab9904e10bf6305425ec5e69ea5553b1cb544cbe120c4710d9a9c1b2"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/7/fix
Content-Type: application/json
Authorization: Bearer 2d7e0d8e4f8a75fdf9d0a460377cd7719cb0ccd23087b65a300be5d919b40cbe
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
    "id": 7,
    "user_id": 34,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-20T09:45:44.755Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/7/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d7e0d8e4f8a75fdf9d0a460377cd7719cb0ccd23087b65a300be5d919b40cbe"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/8
Content-Type: application/json
Authorization: Bearer abb6074e1573b2c26709547c97729fe8c958c38ef8e5b891e810b3d4fe6a9a76
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
    "id": 8,
    "user_id": 39,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T09:45:45.092Z",
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
curl "api.goskive.com/v2/feedbacks/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abb6074e1573b2c26709547c97729fe8c958c38ef8e5b891e810b3d4fe6a9a76"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer c23ad8ac5bbed461c884a05793e237448ddd7ff0b281d29316d04cb1586bb3a6
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
	-H "Authorization: Bearer c23ad8ac5bbed461c884a05793e237448ddd7ff0b281d29316d04cb1586bb3a6"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer c94570f887ce3acc2bfd1d44d71c8dacbc02bcf9d45337ed827a88d2cac0f156
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
	-H "Authorization: Bearer c94570f887ce3acc2bfd1d44d71c8dacbc02bcf9d45337ed827a88d2cac0f156"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/fix
Content-Type: application/json
Authorization: Bearer 2027bc86afa7ef9225ad37b804903c56d511851e5c81e620da07cff49e073a00
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
curl "api.goskive.com/v2/feedbacks/5/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2027bc86afa7ef9225ad37b804903c56d511851e5c81e620da07cff49e073a00"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/9
Content-Type: application/json
Authorization: Bearer cb45e102bdb9b74fc042cdd01f076754e9c88fabae5c2a4bc3e0fffccf6a4202
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
    "id": 9,
    "user_id": 44,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T09:45:45.399Z",
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
curl "api.goskive.com/v2/feedbacks/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb45e102bdb9b74fc042cdd01f076754e9c88fabae5c2a4bc3e0fffccf6a4202"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/5
Content-Type: application/json
Authorization: Bearer c93718f448f65708d0b9b55df44ff0ef5c0385bf7eb6ca85fcc230d5aadd2e00
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c93718f448f65708d0b9b55df44ff0ef5c0385bf7eb6ca85fcc230d5aadd2e00"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/3
Content-Type: application/json
Authorization: Bearer 8796cb06b5e4674d068efcc4e50a2002dd0bab647b712ce76fd57901b8456c99
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8796cb06b5e4674d068efcc4e50a2002dd0bab647b712ce76fd57901b8456c99"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer 812fb12281f5910497d559964941432bbf685baeefbe5d5906fa7036de445bb5
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/8038d2b9bd7f479806088d50a5edc910.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161020%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161020T094623Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=7a3e7a59aaf996993617f71ccf59fec61050847ca72042e749443c9689b7ad76"
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
	-H "Authorization: Bearer 812fb12281f5910497d559964941432bbf685baeefbe5d5906fa7036de445bb5"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/11/preview
Content-Type: application/json
Authorization: Bearer f674ed3d9b010c02971e45a8c9b42d32e667867a1bd4e941feae0659f0b94e50
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/79e0da4349493f007980bb22a47cd837.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161020%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161020T094623Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=5df6d4baf8cf3744daa5e0b62148861727c56637cfb8cdc201e9ccc1ccb37a57"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/11/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f674ed3d9b010c02971e45a8c9b42d32e667867a1bd4e941feae0659f0b94e50"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 548abce2e2d72d689283667325a667d3216bd0f1a2e32e01f818d5e67ea06b1a
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
      "id": 566,
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
      "created_at": "2016-10-20T09:46:22.497Z",
      "updated_at": "2016-10-20T09:46:22.497Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-20T09:46:22.567Z",
    "updated_at": "2016-10-20T09:46:22.567Z",
    "course_id": 189,
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
	-H "Authorization: Bearer 548abce2e2d72d689283667325a667d3216bd0f1a2e32e01f818d5e67ea06b1a"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer ced5f31ec9fe937d928709f8420fa592d652c98d2202f297f69db1f4068bda6d
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
      "creator_id": 326,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 97,
      "additional_university_ids": [

      ],
      "topic_id": 98,
      "discipline_id": 98,
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
      "chapters_updated_at": "2016-10-20T09:46:03.839Z",
      "updated_at": "2016-10-20T09:46:05.560Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 331,
      "id": 97,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-c0df8f18-b5d1-4a99-8fa9-aee88061ea8f",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-c0df8f18-b5d1-4a99-8fa9-aee88061ea8f",
      "slug": "mit-the-great-british-bake-off-c0df8f18-b5d1-4a99-8fa9-aee88061ea8f",
      "university_id": 98,
      "additional_university_ids": [

      ],
      "topic_id": 99,
      "discipline_id": 99,
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
      "chapters_updated_at": "2016-10-20T09:46:03.839Z",
      "updated_at": "2016-10-20T09:46:06.153Z",
      "shortname": "mit-the-great-british-bake-off-c0df8f18-b5d1-4a99-8fa9-aee88061ea8f"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer ced5f31ec9fe937d928709f8420fa592d652c98d2202f297f69db1f4068bda6d"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/9/report
Content-Type: application/json
Authorization: Bearer 5a88ced240df7bb8f6ee30109f2c256789b9483a73c8b1edbb8c20c321a816aa
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a88ced240df7bb8f6ee30109f2c256789b9483a73c8b1edbb8c20c321a816aa"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer 664db63837b189f594102306715b2da3c4bfb6a6d8b7dbacf2d7fe1781fc6285
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
    "id": 46,
    "author_id": 293,
    "reply_to_id": null,
    "created_at": "2016-10-20T09:46:01.151Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 664db63837b189f594102306715b2da3c4bfb6a6d8b7dbacf2d7fe1781fc6285"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer 0e987547f34ed371099cbc67b59e94ab86710a530cfe080d30c4aaaf13dcedd1
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
    "id": 45,
    "author_id": 287,
    "reply_to_id": null,
    "created_at": "2016-10-20T09:46:00.661Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 287,
      "feedbackable_id": 10,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:00.659Z",
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
curl "api.goskive.com/v2/flashcards/10/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e987547f34ed371099cbc67b59e94ab86710a530cfe080d30c4aaaf13dcedd1"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/14/comments
Content-Type: application/json
Authorization: Bearer 1ab4ebe568b0db40162e886d569faa8cef8bd4b2c6ceafe407c2805ad4644164
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
      "id": 47,
      "author_id": 302,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:46:01.620Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 303,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:46:01.636Z",
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
curl "api.goskive.com/v2/flashcards/14/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ab4ebe568b0db40162e886d569faa8cef8bd4b2c6ceafe407c2805ad4644164"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer a295f0653393fe1da902e565139017d137affc6d9a07269a413a1e8071436f15
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
curl "api.goskive.com/v2/flashcards/11/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a295f0653393fe1da902e565139017d137affc6d9a07269a413a1e8071436f15"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/51/feedbacks
Content-Type: application/json
Authorization: Bearer 63fe8e00d3560699d0ec496a896cc8fe102701ef2024c1cb25614eab29a06646
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
    "user_id": 474,
    "feedbackable_id": 51,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T09:46:15.895Z",
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
curl "api.goskive.com/v2/flashcards/51/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63fe8e00d3560699d0ec496a896cc8fe102701ef2024c1cb25614eab29a06646"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/53/feedbacks
Content-Type: application/json
Authorization: Bearer 2bf9793642ccf897ce6140cf256c77542f3df5dbdffb7deb66b922e30b02e68e
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
      "id": 41,
      "user_id": 484,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:16.359Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 483,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:16.348Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bf9793642ccf897ce6140cf256c77542f3df5dbdffb7deb66b922e30b02e68e"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/44/votes
Content-Type: application/json
Authorization: Bearer feb0127007e3c05a1e77171b3f9327618eebd79b69dd4e183ccc792f76469ab1
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
      "votable_id": 44,
      "user_id": 427
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 44,
      "user_id": 426
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 44,
      "user_id": 425
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/44/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer feb0127007e3c05a1e77171b3f9327618eebd79b69dd4e183ccc792f76469ab1"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/22/republish
Content-Type: application/json
Authorization: Bearer 9280c66af05b22222580a6bc9c49ead37ad83375d8b987e26d1803bafcf66704
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
curl "api.goskive.com/v2/flashcards/22/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9280c66af05b22222580a6bc9c49ead37ad83375d8b987e26d1803bafcf66704"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/19/bookmark
Content-Type: application/json
Authorization: Bearer 90f8c1cd14978767f21c596b5b0842a8cbc291c595804cbea19566cad982283d
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/19/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90f8c1cd14978767f21c596b5b0842a8cbc291c595804cbea19566cad982283d"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/24
Content-Type: application/json
Authorization: Bearer dba658849b8833f6ab792eedf18e8dc9a3cacc78cf45ea40b0c9446b1d92b58e
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dba658849b8833f6ab792eedf18e8dc9a3cacc78cf45ea40b0c9446b1d92b58e"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/27/downvote
Content-Type: application/json
Authorization: Bearer 4ab667def2d1c6a661058c703b5577b924d68db0db9c5227ec77288cc7c3ae6c
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/27/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ab667def2d1c6a661058c703b5577b924d68db0db9c5227ec77288cc7c3ae6c"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/25
Content-Type: application/json
Authorization: Bearer 72793317ea08a8e1456dcbfeacdcc33a7b246aa6b8cc97a7cf5a0518c26466ff
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
    "id": 25,
    "obfuscated_id": "HsmcIJXdRE4",
    "author_id": 360,
    "chapter_id": 52,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:07.803Z",
    "created_at": "2016-10-20T09:46:07.803Z",
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
curl "api.goskive.com/v2/flashcards/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72793317ea08a8e1456dcbfeacdcc33a7b246aa6b8cc97a7cf5a0518c26466ff"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/report
Content-Type: application/json
Authorization: Bearer 792bf7a3549d76fabc1ac2459b95319ad95987c75312f834f58b59e35039435a
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/26/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 792bf7a3549d76fabc1ac2459b95319ad95987c75312f834f58b59e35039435a"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/20/bookmark
Content-Type: application/json
Authorization: Bearer 646389b43ec59304bf57f530f15c24e8046f5dda741dea7fc37df770cd1691ab
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/20/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 646389b43ec59304bf57f530f15c24e8046f5dda741dea7fc37df770cd1691ab"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/upvote
Content-Type: application/json
Authorization: Bearer e9d0ee54018a2a8a64b3a562f155e233ef0e22232a3586710435bf37cfa176ec
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9d0ee54018a2a8a64b3a562f155e233ef0e22232a3586710435bf37cfa176ec"
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
    "key": "cache/f5cabfcb374a618f2ce4bc3646aed634.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMFQxMDo0NjozNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9mNWNhYmZjYjM3NGE2MThmMmNlNGJjMzY0NmFlZDYzNC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDIwL2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAyMFQwOTQ2MzZaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161020/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161020T094636Z",
    "x-amz-signature": "3dce5f8fbbcf7c3e68cfd639c7508284ceeb3b3e2ef113b663f114b9f91923d9"
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
Authorization: Bearer 6dd508dfb8203a300b4607fd7c1975980224c88080e94c46528a5cabdc9b6872
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
	-H "Authorization: Bearer 6dd508dfb8203a300b4607fd7c1975980224c88080e94c46528a5cabdc9b6872"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer ae6c7c075e21763146e51c7fc5bcdb963ffb3be6efe1c19bb1c6d92eaf757733
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
	-H "Authorization: Bearer ae6c7c075e21763146e51c7fc5bcdb963ffb3be6efe1c19bb1c6d92eaf757733"
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
{"password":{"reset_password_token":"kquoexe13DZsGv41WJGP","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 310,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-20T09:46:02.343Z",
  "updated_at": "2016-10-20T09:46:02.511Z",
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
  "audit_id": 4030
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"kquoexe13DZsGv41WJGP","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/55/comments
Content-Type: application/json
Authorization: Bearer fa6a245e8f4f8145cff3a5d323554df672f324b8da96572744e5b856cd70d553
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
    "id": 51,
    "author_id": 663,
    "reply_to_id": null,
    "created_at": "2016-10-20T09:46:29.059Z",
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
curl "api.goskive.com/v2/questions/55/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa6a245e8f4f8145cff3a5d323554df672f324b8da96572744e5b856cd70d553"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/56/comments
Content-Type: application/json
Authorization: Bearer 0da77e0d390d2a76972315688f5463f82e4ad03c4c161fd36398ff7f18371837
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
    "author_id": 666,
    "reply_to_id": null,
    "created_at": "2016-10-20T09:46:29.518Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 666,
      "feedbackable_id": 56,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:29.514Z",
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
curl "api.goskive.com/v2/questions/56/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0da77e0d390d2a76972315688f5463f82e4ad03c4c161fd36398ff7f18371837"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/58/comments
Content-Type: application/json
Authorization: Bearer 4b611eaa92e27cb50a0a97dd8b6b80a4de4345190143e8c31e5ed1a7f1d702d2
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
      "author_id": 676,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:46:30.302Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 675,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:46:30.284Z",
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
curl "api.goskive.com/v2/questions/58/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b611eaa92e27cb50a0a97dd8b6b80a4de4345190143e8c31e5ed1a7f1d702d2"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/54/comments
Content-Type: application/json
Authorization: Bearer a05259c2a22b20b13f3f6e7d3c71222f97c56dfabea5e9c21b45cb29e70263eb
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
curl "api.goskive.com/v2/questions/54/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a05259c2a22b20b13f3f6e7d3c71222f97c56dfabea5e9c21b45cb29e70263eb"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/21/feedbacks
Content-Type: application/json
Authorization: Bearer 2e5f201d30e2b7b0402561d3de9ebd4b6cddf7f9a8101c283ddaa88b5b880623
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
    "user_id": 132,
    "feedbackable_id": 21,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-20T09:45:52.058Z",
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
curl "api.goskive.com/v2/questions/21/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e5f201d30e2b7b0402561d3de9ebd4b6cddf7f9a8101c283ddaa88b5b880623"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/23/feedbacks
Content-Type: application/json
Authorization: Bearer 2c5639b94c5c021ae5a20587d275e1b82aa76e7a22019e2ff23092923637a922
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
      "user_id": 142,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:52.860Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 141,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:52.849Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/23/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c5639b94c5c021ae5a20587d275e1b82aa76e7a22019e2ff23092923637a922"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/75/votes
Content-Type: application/json
Authorization: Bearer c266dfb72dd97e74d75f8d4893b174724699a0d810579067c2716b6c0d2a2d80
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
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 779
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 778
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 75,
      "user_id": 777
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/75/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c266dfb72dd97e74d75f8d4893b174724699a0d810579067c2716b6c0d2a2d80"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/124/republish
Content-Type: application/json
Authorization: Bearer 78851c268362523d95c31ed37dda45981e902924b3a6fe5efab058c6f2233103
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
curl "api.goskive.com/v2/questions/124/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78851c268362523d95c31ed37dda45981e902924b3a6fe5efab058c6f2233103"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/125/bookmark
Content-Type: application/json
Authorization: Bearer f6d6112edc855253c7f215e82b02f29b6304286fec0b0332730ff3f6fa526c35
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/125/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6d6112edc855253c7f215e82b02f29b6304286fec0b0332730ff3f6fa526c35"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/126
Content-Type: application/json
Authorization: Bearer 3b66f0c42508acaadaaeca68d5e3d753b4a9cd76c9ed87b1fd3e3e0f6d9dd814
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/126" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b66f0c42508acaadaaeca68d5e3d753b4a9cd76c9ed87b1fd3e3e0f6d9dd814"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/107/downvote
Content-Type: application/json
Authorization: Bearer 48a8620c0f6ec6f1c6a43299c3ae2d46a8b5629e2f6db571d3c66d67c9689d2e
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/107/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48a8620c0f6ec6f1c6a43299c3ae2d46a8b5629e2f6db571d3c66d67c9689d2e"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/131
Content-Type: application/json
Authorization: Bearer d70666c8bd1bd197b585edd97f775a6e1b407de09cb1679827864bb622457544
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
    "id": 131,
    "obfuscated_id": "gCw8isdgMKE",
    "author_id": 944,
    "chapter_id": 192,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:58.647Z",
    "created_at": "2016-10-20T09:46:58.535Z",
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
        "id": 265,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 266,
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
curl "api.goskive.com/v2/questions/131" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d70666c8bd1bd197b585edd97f775a6e1b407de09cb1679827864bb622457544"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/128/report
Content-Type: application/json
Authorization: Bearer 104dec39bd2c46183e5e5f3f053740bd6b53255fa1f980ddc5458ef4594e936c
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/128/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 104dec39bd2c46183e5e5f3f053740bd6b53255fa1f980ddc5458ef4594e936c"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/129/bookmark
Content-Type: application/json
Authorization: Bearer 0f15c2dada0655b4134be846a911801aa55c1d5b06e6b6b289ea40e841efa559
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/129/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f15c2dada0655b4134be846a911801aa55c1d5b06e6b6b289ea40e841efa559"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/130
Content-Type: application/json
Authorization: Bearer 16de19efe13e3d142981d9b97b8cc135e73aba7b8c74ca0177be425c01855a51
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":130,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-20T09:46:58.059Z","updated_at":"2016-10-20T09:46:58.172Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":191,"author_id":941,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 130,
    "obfuscated_id": "N-qIf0IsvWM",
    "author_id": 941,
    "chapter_id": 191,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T09:46:58.278Z",
    "created_at": "2016-10-20T09:46:58.059Z",
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
    "question": "{\"id\"=>130, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-20T09:46:58.059Z\", \"updated_at\"=>\"2016-10-20T09:46:58.172Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>191, \"author_id\"=>941, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 262,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 263,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 264,
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
curl "api.goskive.com/v2/questions/130" -d '{"question":{"question":{"id":130,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-20T09:46:58.059Z","updated_at":"2016-10-20T09:46:58.172Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":191,"author_id":941,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16de19efe13e3d142981d9b97b8cc135e73aba7b8c74ca0177be425c01855a51"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/127/upvote
Content-Type: application/json
Authorization: Bearer a9ce6798b93bbaf4ea8a6a93473ae0347cdf4be151acef6b7fe210688a2d372f
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/127/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9ce6798b93bbaf4ea8a6a93473ae0347cdf4be151acef6b7fe210688a2d372f"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6d8269262d81ff141bde085abb3ab5853d0d5c4fa0bb11b6a2945586466c008a
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
      "creator_id": 967,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 293,
      "additional_university_ids": [

      ],
      "topic_id": 319,
      "discipline_id": 320,
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
      "updated_at": "2016-10-20T09:47:01.067Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d8269262d81ff141bde085abb3ab5853d0d5c4fa0bb11b6a2945586466c008a"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer a44630bfccb0b5469ba3ddccb916c6ebf431bf791e5d3c41a8f09b5395ed72c9
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
      "updated_at": "2016-10-20T09:47:00.832Z",
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
      "updated_at": "2016-10-20T09:47:00.813Z",
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
	-H "Authorization: Bearer a44630bfccb0b5469ba3ddccb916c6ebf431bf791e5d3c41a8f09b5395ed72c9"
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
      "id": 209,
      "name": "Synergistic reciprocal help-desk",
      "name_translations": {
        "en": "Synergistic reciprocal help-desk"
      },
      "discipline_id": 209
    },
    {
      "id": 210,
      "name": "User-friendly zero defect functionalities",
      "name_translations": {
        "en": "User-friendly zero defect functionalities"
      },
      "discipline_id": 210
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
GET /v2/topics/211
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
    "id": 211,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 211
  }
}
```



```shell
curl "api.goskive.com/v2/topics/211" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 5accafca9b5b81d029077b45dab95ed53361933bfa47998b36045fed60037311
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
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-207",
      "html_url": "https://goskive.com/university/uni-207",
      "slug": "uni-207",
      "name": "University 167",
      "short_name": "Uni 207",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/1cdbf673f30f67c61b7ace90db9e91933e78fb37.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b7335e35f7e7beb9bb3b01e562574b256268a503.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T09:46:38.538Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-208",
      "html_url": "https://goskive.com/university/uni-208",
      "slug": "uni-208",
      "name": "University 168",
      "short_name": "Uni 208",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8845f9dd62b4591fcf4eee8e4da13bb47f55ee9a.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d2e0e3fabe19bda9a917a5eb9f64113cd317619e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T09:46:38.555Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-209",
      "html_url": "https://goskive.com/university/uni-209",
      "slug": "uni-209",
      "name": "University 169",
      "short_name": "Uni 209",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d4a93c927995b518f0ed147705cc1adcbcba7302.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c601cc4c49af77397e019500f54613c65ddac27e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T09:46:38.571Z",
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
	-H "Authorization: Bearer 5accafca9b5b81d029077b45dab95ed53361933bfa47998b36045fed60037311"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer ae07b57b8537fb79e9920f5ad81c83fa1391a228930cd09bd1e1f274dd8d7ff9
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
    "id": 229,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3a5cfcda6927c38a5f855943a8a66eeef6616188.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c0bde4774cc0523fbdfa23f0a4e671be0fbfe4c0.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-20T09:46:38.690Z",
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
	-H "Authorization: Bearer ae07b57b8537fb79e9920f5ad81c83fa1391a228930cd09bd1e1f274dd8d7ff9"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d388b16d2f02e22200a521cf15bf7a07aaab49afc8629ce3cba015c91947f10e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":152,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 508,
    "id": 145,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 146,
    "additional_university_ids": [

    ],
    "topic_id": 152,
    "discipline_id": 152,
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
    "chapters_updated_at": "2016-10-20T09:46:17.326Z",
    "updated_at": "2016-10-20T09:46:17.496Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 90,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-20T09:46:17.447Z",
        "course_id": 145,
        "author_id": 508,
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
        "id": 91,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-20T09:46:17.466Z",
        "course_id": 145,
        "author_id": 508,
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
        "id": 92,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-20T09:46:17.485Z",
        "course_id": 145,
        "author_id": 508,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":152,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d388b16d2f02e22200a521cf15bf7a07aaab49afc8629ce3cba015c91947f10e"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 067b28cd670ff3fb6338ac742d35c621db7ccceb14c129479d52f6f98c9ef341
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":151,"published":false}}
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
    "creator_id": 507,
    "id": 144,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 145,
    "additional_university_ids": [

    ],
    "topic_id": 151,
    "discipline_id": 151,
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
    "updated_at": "2016-10-20T09:46:17.282Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":151,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 067b28cd670ff3fb6338ac742d35c621db7ccceb14c129479d52f6f98c9ef341"
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
      "creator_id": 522,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "discipline_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "updated_at": "2016-10-20T09:46:18.854Z",
      "shortname": "fu-course-135"
    },
    {
      "creator_id": 522,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 152,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 166,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
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
      "chapters_updated_at": "2016-10-20T09:46:19.179Z",
      "updated_at": "2016-10-20T09:46:19.187Z",
      "shortname": "fu-course-136"
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
Authorization: Bearer b802b9d040a2098ca04d9005016d1c73e225bfc519453de666d416d82293adc6
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
      "creator_id": 539,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 158,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
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
      "updated_at": "2016-10-20T09:46:20.605Z",
      "shortname": "fu-course-151"
    },
    {
      "creator_id": 539,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 158,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
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
      "chapters_updated_at": "2016-10-20T09:46:20.906Z",
      "updated_at": "2016-10-20T09:46:20.913Z",
      "shortname": "fu-course-152"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b802b9d040a2098ca04d9005016d1c73e225bfc519453de666d416d82293adc6"
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
      "creator_id": 527,
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 169,
      "discipline_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
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
      "updated_at": "2016-10-20T09:46:19.396Z",
      "shortname": "fu-course-139"
    },
    {
      "creator_id": 527,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-140",
      "html_url": "https://goskive.com/course/fu-course-140",
      "slug": "fu-course-140",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 170,
      "discipline_id": 170,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 140",
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
      "updated_at": "2016-10-20T09:46:19.436Z",
      "shortname": "fu-course-140"
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
Authorization: Bearer 5fb2dc75dd7dc58beacbc9850e2b067ecc469ff061305b4edab400727d8f7e20
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
      "creator_id": 546,
      "id": 178,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-155",
      "html_url": "https://goskive.com/course/fu-course-155",
      "slug": "fu-course-155",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
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
      "updated_at": "2016-10-20T09:46:21.191Z",
      "shortname": "fu-course-155"
    },
    {
      "creator_id": 546,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 160,
      "additional_university_ids": [

      ],
      "topic_id": 186,
      "discipline_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 156",
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
      "updated_at": "2016-10-20T09:46:21.232Z",
      "shortname": "fu-course-156"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fb2dc75dd7dc58beacbc9850e2b067ecc469ff061305b4edab400727d8f7e20"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer e1d93e4a8f1e6897abf599dcc0940465ca1b461f56b0ecc8a9d6d534cd2270bd
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
  "id": 947,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-20T09:46:58.799Z",
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
	-H "Authorization: Bearer e1d93e4a8f1e6897abf599dcc0940465ca1b461f56b0ecc8a9d6d534cd2270bd"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/306
Content-Type: application/json
Authorization: Bearer 25f77e7420381d6e7c0a2ef8d01c93d41dc1ae8bbd195c160dc5f48e8c7adc9c
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
    "id": 306,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 94,
    "fields_of_study": [
      94,
      95
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-20T09:46:01.830Z",
    "updated_at": "2016-10-20T09:46:01.830Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/306" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25f77e7420381d6e7c0a2ef8d01c93d41dc1ae8bbd195c160dc5f48e8c7adc9c"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/304
Content-Type: application/json
Authorization: Bearer 3c66a5924d31883dce56b51dd1dcd2d62b631e33f3b784dd09df6022d3d6b830
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
    "id": 304,
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
    "created_at": "2016-10-20T09:46:01.681Z",
    "updated_at": "2016-10-20T09:46:01.681Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/304" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c66a5924d31883dce56b51dd1dcd2d62b631e33f3b784dd09df6022d3d6b830"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/22
Content-Type: application/json
Authorization: Bearer 5b3edc74f2a21b5191582fe9e9b44b66ff88f7e88f30e29dc2b6445fc993d090
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
	-H "Authorization: Bearer 5b3edc74f2a21b5191582fe9e9b44b66ff88f7e88f30e29dc2b6445fc993d090"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/21
Content-Type: application/json
Authorization: Bearer dceebb33dbabb7de52b762a5904b033d0938969afd5cf2123dbb6ea2bf2321df
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
    "votable_id": 133,
    "user_id": 952
  }
}
```



```shell
curl "api.goskive.com/v2/votes/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dceebb33dbabb7de52b762a5904b033d0938969afd5cf2123dbb6ea2bf2321df"
```
