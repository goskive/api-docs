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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"86132b279ad71a632feedbf07b6d3e7e5f24bd3f6e21ca41b61e904f920e3850","client_secret":"ca9a080a493cb401e07e07fc1270c204dd4238c405384f8fa2c10cf7d5635b77"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"86132b279ad71a632feedbf07b6d3e7e5f24bd3f6e21ca41b61e904f920e3850","client_secret":"ca9a080a493cb401e07e07fc1270c204dd4238c405384f8fa2c10cf7d5635b77"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ODgyNWU4Nzg0NDdmNmRlM2VmNDVjOTRmNWJiMWNlZmMxMWMzZjRhZDM2YzY5
YzM5OTgwMzBiZWExOTJiYzc3ZTpmMmFhOWZhZjMyMDBhMzU1MDBlOTRkM2Ux
OWZmNWVkNGZkMWI5ZGRlMzM3ZTMxNmRmMzg0MGMwNDQ5YWIyYTNk

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
	-u 8825e878447f6de3ef45c94f5bb1cefc11c3f4ad36c69c3998030bea192bc77e:f2aa9faf3200a35500e94d3e19ff5ed4fd1b9dde337e316df3840c0449ab2a3d
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"89f2c4ecc76303bbdb2870eecb6c67bda72b7f7834d653625789b8e8148f4df4","client_secret":"d228de856c3bc1d7912f4d20b148fce4967b88a92449c1c2a5bbcbcca853c4a6"}
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
  "access_token": "6dbff7aef734b2a6ba8b8c05ea801e625f0d7ea57caab075cd252aaa7bce8f89",
  "token_type": "bearer",
  "created_at": 1477590178
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"89f2c4ecc76303bbdb2870eecb6c67bda72b7f7834d653625789b8e8148f4df4","client_secret":"d228de856c3bc1d7912f4d20b148fce4967b88a92449c1c2a5bbcbcca853c4a6"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YjgxODJhZGMxODhmOTU2MTBkNTUxZTMyOWUwZTM4NTIwYjg2Yzk3MTJhNzFi
MDVmNzg0YTkyODA2ODZmODFmNjowNDAwODc0MTZiMjgyMTQ1YzdiNTA2MDlm
MDJlNTE1ZGIzMGRhNGIzMWRlYmE1MDQ0NWIyMzFiODhkNjNjOWUx

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
  "access_token": "d1855bf735443c3a976f17191831314931136fd0014f461200c6dd77c8fc2a73",
  "token_type": "bearer",
  "created_at": 1477590178
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u b8182adc188f95610d551e329e0e38520b86c9712a71b05f784a9280686f81f6:040087416b282145c7b50609f02e515db30da4b31deba50445b231b88d63c9e1
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
{"grant_type":"client_credentials","client_id":"c4ee32a0ecf38f80350e476aa681ed507b15ba0c32dc5205df5e08641ee9f1e8","client_secret":"6b3663703fe73d2db70212a6666ae054ffa3c526e2fd9c982401cfa14d4b014d"}
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
  "access_token": "959f84a7670611cfc3a001659905817344080e3b51c1e58a49b56be8a6df357a",
  "token_type": "bearer",
  "created_at": 1477590178
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"c4ee32a0ecf38f80350e476aa681ed507b15ba0c32dc5205df5e08641ee9f1e8","client_secret":"6b3663703fe73d2db70212a6666ae054ffa3c526e2fd9c982401cfa14d4b014d"}' -X POST \
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
Authorization: Bearer 5d853a4eda4780169a9af7f5be7706039bc7186cf674c2051221c1bf58b6803f
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
	-H "Authorization: Bearer 5d853a4eda4780169a9af7f5be7706039bc7186cf674c2051221c1bf58b6803f"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/11/flashcards
Content-Type: application/json
Authorization: Bearer 5d25d6fc5c6ebab08debfcd7baacc1e8d858f5f5cb09d9203f93dfe8e19c8ca4
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":11,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 145,
    "chapter_id": 11,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:43:03.727Z",
    "created_at": "2016-10-27T17:43:03.727Z",
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
curl "api.goskive.com/v2/chapters/11/flashcards" -d '{"flashcard":{"chapter_id":11,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d25d6fc5c6ebab08debfcd7baacc1e8d858f5f5cb09d9203f93dfe8e19c8ca4"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/12/flashcards
Content-Type: application/json
Authorization: Bearer 00e06a71079cda94a9d73ce1dbb159d5ec5697b085f7fa53071ef0749d423f2f
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
      "author_id": 146,
      "chapter_id": 12,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:03.875Z",
      "created_at": "2016-10-27T17:43:03.875Z",
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
      "author_id": 146,
      "chapter_id": 12,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:03.912Z",
      "created_at": "2016-10-27T17:43:03.912Z",
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
      "author_id": 146,
      "chapter_id": 12,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:03.948Z",
      "created_at": "2016-10-27T17:43:03.948Z",
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
curl "api.goskive.com/v2/chapters/12/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00e06a71079cda94a9d73ce1dbb159d5ec5697b085f7fa53071ef0749d423f2f"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 5197a91b78e36c9b1aa611e7c8848e14483d5b7115d5ca1da7a099a324de8ef0
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
    "author_id": 12,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:42:55.736Z",
    "created_at": "2016-10-27T17:42:55.736Z",
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
	-H "Authorization: Bearer 5197a91b78e36c9b1aa611e7c8848e14483d5b7115d5ca1da7a099a324de8ef0"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/2/questions
Content-Type: application/json
Authorization: Bearer 55f46e5e95771b6c5dc97718bc33069390f255c0532229813b0d71d2309f334a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":2,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 6,
    "chapter_id": 2,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:42:55.098Z",
    "created_at": "2016-10-27T17:42:55.098Z",
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
        "id": 4,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 5,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/2/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":2,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55f46e5e95771b6c5dc97718bc33069390f255c0532229813b0d71d2309f334a"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer 1e7da350ea9330977955915ffa901251debaedf5d98cfb26ef37ae3e10fe5b45
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 9,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:42:55.413Z",
    "created_at": "2016-10-27T17:42:55.413Z",
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
        "id": 6,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 7,
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
curl "api.goskive.com/v2/chapters/3/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e7da350ea9330977955915ffa901251debaedf5d98cfb26ef37ae3e10fe5b45"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/1/questions
Content-Type: application/json
Authorization: Bearer 50d52f06dc63979e45124fbf9ecf61c13581a3910a3b2ac881926dc4f8d70538
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
    "author_id": 3,
    "chapter_id": 1,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:42:54.662Z",
    "created_at": "2016-10-27T17:42:54.662Z",
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
	-H "Authorization: Bearer 50d52f06dc63979e45124fbf9ecf61c13581a3910a3b2ac881926dc4f8d70538"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer c5109b0c8dfa0ff0eb575e267e1b10e7c5a13da6cee8a7cf970083e5f1d863f4
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
      "author_id": 15,
      "chapter_id": 5,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:42:56.323Z",
      "created_at": "2016-10-27T17:42:56.208Z",
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
      "author_id": 16,
      "chapter_id": 5,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:42:56.507Z",
      "created_at": "2016-10-27T17:42:56.391Z",
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
      "author_id": 17,
      "chapter_id": 5,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:42:56.694Z",
      "created_at": "2016-10-27T17:42:56.576Z",
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
	-H "Authorization: Bearer c5109b0c8dfa0ff0eb575e267e1b10e7c5a13da6cee8a7cf970083e5f1d863f4"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/70
Content-Type: application/json
Authorization: Bearer ed0d153480b76d32da27e819f66d0569cd5ad9c6b64ef2371c531c197c2e5794
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
curl "api.goskive.com/v2/chapters/70" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed0d153480b76d32da27e819f66d0569cd5ad9c6b64ef2371c531c197c2e5794"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/73
Content-Type: application/json
Authorization: Bearer 5e4bf094a399bbce09ae7893a8c6c8dbe09bbb06c4004c34c28c6bcfab8393c6
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
curl "api.goskive.com/v2/chapters/73" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e4bf094a399bbce09ae7893a8c6c8dbe09bbb06c4004c34c28c6bcfab8393c6"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/76
Content-Type: application/json
Authorization: Bearer 39a1d4d874dd2a3f1ac6c7f18dbba1f487db29fca03df240848b5128f18f8961
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
curl "api.goskive.com/v2/chapters/76" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 39a1d4d874dd2a3f1ac6c7f18dbba1f487db29fca03df240848b5128f18f8961"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/72
Content-Type: application/json
Authorization: Bearer f84d9e7dd2f551249b4c85035f36c1d9a6bc8f7f4de9d4d71dee02573867f8de
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/72" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f84d9e7dd2f551249b4c85035f36c1d9a6bc8f7f4de9d4d71dee02573867f8de"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/77
Content-Type: application/json
Authorization: Bearer a207f4934fc49a5cb7ab0b2319356716631640e47a08d74be90506ff4016a813
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
    "id": 77,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-27T17:43:26.861Z",
    "course_id": 132,
    "author_id": 406,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-27T17:43:26.339Z",
    "questions_updated_at": "2016-10-27T17:43:26.339Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 410,
        "chapter_id": 77,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:26.844Z",
        "created_at": "2016-10-27T17:43:26.844Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 408,
        "chapter_id": 77,
        "position": 55,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:26.738Z",
        "created_at": "2016-10-27T17:43:26.623Z",
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
            "id": 120,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 121,
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
curl "api.goskive.com/v2/chapters/77" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a207f4934fc49a5cb7ab0b2319356716631640e47a08d74be90506ff4016a813"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/74
Content-Type: application/json
Authorization: Bearer 71d02879011bd97041325a09f3f98ea8b1431cd9f13f5206c1a0b7d4ee3919d2
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
    "updated_at": "2016-10-27T17:43:26.029Z",
    "course_id": 129,
    "author_id": 398,
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
	-H "Authorization: Bearer 71d02879011bd97041325a09f3f98ea8b1431cd9f13f5206c1a0b7d4ee3919d2"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/49/replies
Content-Type: application/json
Authorization: Bearer 96eef4643286e773deaf287f7609a4c2f0f3326614c19d6e015b8a3679884dde
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
    "author_id": 379,
    "reply_to_id": 49,
    "created_at": "2016-10-27T17:43:24.509Z",
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
	-H "Authorization: Bearer 96eef4643286e773deaf287f7609a4c2f0f3326614c19d6e015b8a3679884dde"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer d1b992d110c7e6da4a028b8fbee42af3c5cd4550dee1120c2dde0aa5d6a2751b
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
	-H "Authorization: Bearer d1b992d110c7e6da4a028b8fbee42af3c5cd4550dee1120c2dde0aa5d6a2751b"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer 1ed154575ea2609d7d3419d9cc09eea4dbcf49d8d5877562dda6031463e204a9
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
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ed154575ea2609d7d3419d9cc09eea4dbcf49d8d5877562dda6031463e204a9"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer f6b43bf5c064b8eef01ffc128546861bf13d7288a867d85a984814a6667e6f88
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
	-H "Authorization: Bearer f6b43bf5c064b8eef01ffc128546861bf13d7288a867d85a984814a6667e6f88"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer fa492cef937a0117c6a1846931c73426ef577e83a81d567d1b66c162fb067cc2
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
	-H "Authorization: Bearer fa492cef937a0117c6a1846931c73426ef577e83a81d567d1b66c162fb067cc2"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/6/report
Content-Type: application/json
Authorization: Bearer 7ff7ddca408dd2f3e7589ff7fd5e187b0d72e3e9fee83bdacfcf06130b20e6eb
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ff7ddca408dd2f3e7589ff7fd5e187b0d72e3e9fee83bdacfcf06130b20e6eb"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/17
Content-Type: application/json
Authorization: Bearer 9bec38af9d21af13705ef33f8f122551a2a3dd4e3e9e06a8a0ecb6c449d8d65a
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
    "id": 17,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-27T17:43:22.742Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/17" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bec38af9d21af13705ef33f8f122551a2a3dd4e3e9e06a8a0ecb6c449d8d65a"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 2b091c1f853d2a1d54bb6ee94b883c05c975413bca8e8fbfd710ff7df4dfb26a
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
      "id": 14,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-27T17:43:22.620Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-27T17:43:22.624Z"
    },
    {
      "id": 16,
      "name": "Fake Company Name 15",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-27T17:43:22.628Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b091c1f853d2a1d54bb6ee94b883c05c975413bca8e8fbfd710ff7df4dfb26a"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/19/company_profiles
Content-Type: application/json
Authorization: Bearer e80db881d981e7cf6ff4dd10d5fff1339d251ac1774e900a1e239c55a179750b
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
curl "api.goskive.com/v2/companies/19/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e80db881d981e7cf6ff4dd10d5fff1339d251ac1774e900a1e239c55a179750b"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/18/company_profiles
Content-Type: application/json
Authorization: Bearer 34487b857ec4f8116cb7c2252410af1cd9d692e87626ea6d0b9968ced25bc094
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
curl "api.goskive.com/v2/companies/18/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34487b857ec4f8116cb7c2252410af1cd9d692e87626ea6d0b9968ced25bc094"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 7ab2c73a4a62aeedccecd7e104fc822679f52fd53afa2ea9d8260881720ef9eb
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
      "company_id": 2,
      "precluded_campaign_ids": [

      ],
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
      "company_id": 5,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
        {
          "country_codes": [
            "DE",
            "EN"
          ],
          "language_code": "en",
          "id": 2,
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
	-H "Authorization: Bearer 7ab2c73a4a62aeedccecd7e104fc822679f52fd53afa2ea9d8260881720ef9eb"
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
Authorization: Bearer e8aa3baace059f00179a85c5701f3d8e2350d835752e28e83e84ce6fbca1e12e
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
	-H "Authorization: Bearer e8aa3baace059f00179a85c5701f3d8e2350d835752e28e83e84ce6fbca1e12e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer efd3b7439c838b5ad10feaf3a4518c53b1e13336eb683eb68359319822807a46
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
    "id": 36,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-27T17:43:07.046Z",
    "course_id": 67,
    "author_id": 202,
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
	-H "Authorization: Bearer efd3b7439c838b5ad10feaf3a4518c53b1e13336eb683eb68359319822807a46"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 388abf09beca0364d532709265852c5a75a94ce0124e0e437da764f52a50c63b
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
      "title": "Clever Chapter Title 14",
      "position": 1,
      "updated_at": "2016-10-27T17:43:05.526Z",
      "course_id": 60,
      "author_id": 175,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 24,
      "title": "Clever Chapter Title 15",
      "position": 2,
      "updated_at": "2016-10-27T17:43:05.549Z",
      "course_id": 60,
      "author_id": 176,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 25,
      "title": "Clever Chapter Title 16",
      "position": 3,
      "updated_at": "2016-10-27T17:43:05.802Z",
      "course_id": 60,
      "author_id": 177,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-27T17:43:05.453Z",
      "questions_updated_at": "2016-10-27T17:43:05.453Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 388abf09beca0364d532709265852c5a75a94ce0124e0e437da764f52a50c63b"
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
      "id": 29,
      "title": "Clever Chapter Title 20",
      "position": 1,
      "updated_at": "2016-10-27T17:43:06.228Z",
      "course_id": 63,
      "author_id": 189,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 30,
      "title": "Clever Chapter Title 21",
      "position": 2,
      "updated_at": "2016-10-27T17:43:06.252Z",
      "course_id": 63,
      "author_id": 190,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 31,
      "title": "Clever Chapter Title 22",
      "position": 3,
      "updated_at": "2016-10-27T17:43:06.503Z",
      "course_id": 63,
      "author_id": 191,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-27T17:43:06.156Z",
      "questions_updated_at": "2016-10-27T17:43:06.156Z",
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
Authorization: Bearer 26e85402f3a1d22d8d7935969d22be9f12b12071c90f8ee804da5f5f3d54f4c6
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
      "title": "Clever Chapter Title 17",
      "position": 1,
      "updated_at": "2016-10-27T17:43:05.946Z",
      "course_id": 61,
      "author_id": 182,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 27,
      "title": "Clever Chapter Title 18",
      "position": 2,
      "updated_at": "2016-10-27T17:43:05.969Z",
      "course_id": 61,
      "author_id": 183,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 28,
      "title": "Clever Chapter Title 19",
      "position": 3,
      "updated_at": "2016-10-27T17:43:05.991Z",
      "course_id": 61,
      "author_id": 184,
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
	-H "Authorization: Bearer 26e85402f3a1d22d8d7935969d22be9f12b12071c90f8ee804da5f5f3d54f4c6"
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
      "id": 32,
      "title": "Clever Chapter Title 23",
      "position": 1,
      "updated_at": "2016-10-27T17:43:06.638Z",
      "course_id": 64,
      "author_id": 195,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 33,
      "title": "Clever Chapter Title 24",
      "position": 2,
      "updated_at": "2016-10-27T17:43:06.661Z",
      "course_id": 64,
      "author_id": 196,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 34,
      "title": "Clever Chapter Title 25",
      "position": 3,
      "updated_at": "2016-10-27T17:43:06.684Z",
      "course_id": 64,
      "author_id": 197,
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
Authorization: Bearer 4650c5daa4f2e3222d32c0874a947d92b547e7de545e45dd4ee56c18a7a58c14
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
    "course_id": 118,
    "user_id": 357,
    "updated_at": "2016-10-27T17:43:22.485Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4650c5daa4f2e3222d32c0874a947d92b547e7de545e45dd4ee56c18a7a58c14"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 557caa1cda00e55b361d8b717491aac109cd22cfdf4f1a8fd44405d0231b7647
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
      "course_id": 115,
      "user_id": 347,
      "updated_at": "2016-10-27T17:43:22.038Z"
    },
    {
      "id": 2,
      "course_id": 115,
      "user_id": 348,
      "updated_at": "2016-10-27T17:43:22.054Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 557caa1cda00e55b361d8b717491aac109cd22cfdf4f1a8fd44405d0231b7647"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/194/files
Content-Type: application/json
Authorization: Bearer 747b26e40f25e5b24569dc1cf7d83073af4fe082126ec2b12aa9324c2f1dcb46
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
      "id": 5,
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
        "created_at": "2016-10-27T17:43:43.658Z",
        "updated_at": "2016-10-27T17:43:43.658Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:43:43.672Z",
      "updated_at": "2016-10-27T17:43:43.672Z",
      "course_id": 194,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 622,
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
        "created_at": "2016-10-27T17:43:43.681Z",
        "updated_at": "2016-10-27T17:43:43.681Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:43:43.691Z",
      "updated_at": "2016-10-27T17:43:43.691Z",
      "course_id": 194,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 7,
      "uploader": {
        "id": 623,
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
        "created_at": "2016-10-27T17:43:43.698Z",
        "updated_at": "2016-10-27T17:43:43.698Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-27T17:43:43.708Z",
      "updated_at": "2016-10-27T17:43:43.708Z",
      "course_id": 194,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/194/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 747b26e40f25e5b24569dc1cf7d83073af4fe082126ec2b12aa9324c2f1dcb46"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/193/files
Content-Type: application/json
Authorization: Bearer 97ac9aeff0dc090d328c04143cda4e7a178eeaa4948196e65e8e3f56434eff62
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
    "id": 4,
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
      "created_at": "2016-10-27T17:43:43.407Z",
      "updated_at": "2016-10-27T17:43:43.407Z"
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
    "created_at": "2016-10-27T17:43:43.462Z",
    "updated_at": "2016-10-27T17:43:43.462Z",
    "course_id": 193,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/193/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97ac9aeff0dc090d328c04143cda4e7a178eeaa4948196e65e8e3f56434eff62"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/196/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 92893de46f0567fd0a2ce730faa949b2e88854e61862ad6ca58d2dcc8bf9f2a7
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
    "key": "cache/c2855e2b391ac2a92ef6e8a0fd0faac4.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yN1QxODo0Mzo0M1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2MyODU1ZTJiMzkxYWMyYTkyZWY2ZThhMGZkMGZhYWM0LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjcvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI3VDE3NDM0M1oifV19",
    "x-amz-credential": "FAKE/20161027/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161027T174343Z",
    "x-amz-signature": "73b2d2f9810019ac8b528bbd56eb5b68b7b8f7c459090c51e23935d6febee7e4"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/196/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92893de46f0567fd0a2ce730faa949b2e88854e61862ad6ca58d2dcc8bf9f2a7"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer c6411f66b1b994b26a37b32607c68ee9cb8ac27dd6eb1818a307bb5a0abc6199
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
	-H "Authorization: Bearer c6411f66b1b994b26a37b32607c68ee9cb8ac27dd6eb1818a307bb5a0abc6199"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 70aea6f13af71dabb2aaac39bb70d602e557503f70b9aedb0f5efa4a81e5d524
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
	-H "Authorization: Bearer 70aea6f13af71dabb2aaac39bb70d602e557503f70b9aedb0f5efa4a81e5d524"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 33502d1057fe3dcd439d4265cc828280ed5dfecc382415f17eaa0d1ccfe5182a
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
	-H "Authorization: Bearer 33502d1057fe3dcd439d4265cc828280ed5dfecc382415f17eaa0d1ccfe5182a"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 87b265dea32ed816ca97a28ec21cc07194029580998325f7462903e0f50354d4
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
	-H "Authorization: Bearer 87b265dea32ed816ca97a28ec21cc07194029580998325f7462903e0f50354d4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 494426b83f281130fd2791b1a25f3f832d666e0716c7a723bea9def98da49c6c
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
	-H "Authorization: Bearer 494426b83f281130fd2791b1a25f3f832d666e0716c7a723bea9def98da49c6c"
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
    "creator_id": 304,
    "id": 102,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 102,
    "additional_university_ids": [

    ],
    "topic_id": 112,
    "discipline_id": 113,
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
    "chapters_updated_at": "2016-10-27T17:43:15.666Z",
    "updated_at": "2016-10-27T17:43:17.058Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 59,
        "title": "Clever Chapter Title 47",
        "position": 1,
        "updated_at": "2016-10-27T17:43:17.010Z",
        "course_id": 102,
        "author_id": 304,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:43:15.666Z",
        "questions_updated_at": "2016-10-27T17:43:15.666Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 60,
        "title": "Clever Chapter Title 48",
        "position": 2,
        "updated_at": "2016-10-27T17:43:17.050Z",
        "course_id": 102,
        "author_id": 304,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:43:15.666Z",
        "questions_updated_at": "2016-10-27T17:43:15.666Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 304,
        "chapter_id": 59,
        "position": 29,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:15.887Z",
        "created_at": "2016-10-27T17:43:15.774Z",
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
            "id": 68,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 69,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 304,
        "chapter_id": 60,
        "position": 31,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:16.257Z",
        "created_at": "2016-10-27T17:43:16.139Z",
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
Authorization: Bearer 759c2e2dcd9b4f31af750476989cdb66c7bed85add648dcebf7a0de73fffbc94
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
    "creator_id": 309,
    "id": 103,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 113,
    "discipline_id": 114,
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
    "chapters_updated_at": "2016-10-27T17:43:17.140Z",
    "updated_at": "2016-10-27T17:43:18.511Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 61,
        "title": "Clever Chapter Title 49",
        "position": 1,
        "updated_at": "2016-10-27T17:43:18.467Z",
        "course_id": 103,
        "author_id": 309,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:43:17.140Z",
        "questions_updated_at": "2016-10-27T17:43:17.140Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 62,
        "title": "Clever Chapter Title 50",
        "position": 2,
        "updated_at": "2016-10-27T17:43:18.504Z",
        "course_id": 103,
        "author_id": 309,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-27T17:43:17.140Z",
        "questions_updated_at": "2016-10-27T17:43:17.140Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 310,
        "chapter_id": 61,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:18.317Z",
        "created_at": "2016-10-27T17:43:18.317Z",
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
        "author_id": 310,
        "chapter_id": 62,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:18.383Z",
        "created_at": "2016-10-27T17:43:18.383Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 310,
        "chapter_id": 61,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:18.354Z",
        "created_at": "2016-10-27T17:43:18.354Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 310,
        "chapter_id": 62,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:18.420Z",
        "created_at": "2016-10-27T17:43:18.420Z",
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
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 310,
        "chapter_id": 61,
        "position": 35,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:17.354Z",
        "created_at": "2016-10-27T17:43:17.242Z",
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
            "id": 80,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 81,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 310,
        "chapter_id": 61,
        "position": 36,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:17.523Z",
        "created_at": "2016-10-27T17:43:17.416Z",
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
          }
        ]
      },
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 310,
        "chapter_id": 62,
        "position": 37,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:17.720Z",
        "created_at": "2016-10-27T17:43:17.604Z",
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
            "id": 84,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 85,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 310,
        "chapter_id": 62,
        "position": 38,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:17.890Z",
        "created_at": "2016-10-27T17:43:17.783Z",
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
            "id": 86,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 87,
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
	-H "Authorization: Bearer 759c2e2dcd9b4f31af750476989cdb66c7bed85add648dcebf7a0de73fffbc94"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/105/pin
Content-Type: application/json
Authorization: Bearer 3ebc65d3808fa36d8fd1aef7930ac97cf54031ff9a383f1de6fe72085ecbd254
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/105/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ebc65d3808fa36d8fd1aef7930ac97cf54031ff9a383f1de6fe72085ecbd254"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/106/pin
Content-Type: application/json
Authorization: Bearer f1e1673b7e021ada12468c6e26304cc1d64c56d15fc55c8893c5b558579e119a
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/106/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1e1673b7e021ada12468c6e26304cc1d64c56d15fc55c8893c5b558579e119a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b3095150c882700641fa2b5f3ac4b5354ffd3b6e9137460760328330c8f318a7
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
    "creator_id": 297,
    "id": 100,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 100,
    "additional_university_ids": [

    ],
    "topic_id": 110,
    "discipline_id": 111,
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
    "updated_at": "2016-10-27T17:43:14.196Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3095150c882700641fa2b5f3ac4b5354ffd3b6e9137460760328330c8f318a7"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer bd2ed0c12769f1c1f6e8e797f3b1fab0dc71a70d602c3dbe61615c0eb1795b64
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
    "id": 23,
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
    "created_at": "2016-10-27T17:42:57.355Z",
    "updated_at": "2016-10-27T17:42:57.355Z",
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
	-H "Authorization: Bearer bd2ed0c12769f1c1f6e8e797f3b1fab0dc71a70d602c3dbe61615c0eb1795b64"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c9bcf00a4564fc98ec3b3ff4547281ae5bf7edc296093143f8848c91d4479130
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[10]}
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
    "id": 25,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      10
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:42:57.766Z",
    "updated_at": "2016-10-27T17:42:57.799Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[10]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9bcf00a4564fc98ec3b3ff4547281ae5bf7edc296093143f8848c91d4479130"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7c214db22c390bef6b53ccda1690d61f39cfbfa373511444ec0cd52a6aebb817
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
    "id": 28,
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
    "created_at": "2016-10-27T17:42:57.958Z",
    "updated_at": "2016-10-27T17:42:57.958Z",
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
	-H "Authorization: Bearer 7c214db22c390bef6b53ccda1690d61f39cfbfa373511444ec0cd52a6aebb817"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0de117a4e44ed234f2109073fcc3d54ded8c76f20231eb872f068f0a0e45b394
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[12]}
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
    "id": 27,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      12
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:42:57.910Z",
    "updated_at": "2016-10-27T17:42:57.910Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[12]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0de117a4e44ed234f2109073fcc3d54ded8c76f20231eb872f068f0a0e45b394"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 364dad23b36a484ce795e0fdafcbf33c84e5a1d23f4818f24003f990e9640295
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

9
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
    "id": 24,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/932cd9698784b6443c1c5cc89a4e98b21aea52d1.jpg",
    "university_id": null,
    "fields_of_study": [
      9
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-27T17:42:57.487Z",
    "updated_at": "2016-10-27T17:42:57.713Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/4e967ebc7dcf3813b0f2462274d6920e4f6ae1fb.jpg",
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

9
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 364dad23b36a484ce795e0fdafcbf33c84e5a1d23f4818f24003f990e9640295"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2ae2aef3ae39248899dfcddbdd019e629526b3929a34fab26267983134cd5171
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
      "bookmarkable_id": 9,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 10,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 11,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ae2aef3ae39248899dfcddbdd019e629526b3929a34fab26267983134cd5171"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 399fe7714f2aba058004c683802f17437c60dfe2ef82199c038f707b3c0c262b
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
	-H "Authorization: Bearer 399fe7714f2aba058004c683802f17437c60dfe2ef82199c038f707b3c0c262b"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 704aa06b09dc7a56925ecc2b01d07e3a9e101030fdccfbe0bf46c415d1b63608
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
	-H "Authorization: Bearer 704aa06b09dc7a56925ecc2b01d07e3a9e101030fdccfbe0bf46c415d1b63608"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer c6f9e2bc551ca10bbd214ae31680258e623f62cdcea1b4607754e24a660cc556
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
      "creator_id": 769,
      "id": 260,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-188",
      "html_url": "https://goskive.com/course/mit-course-188",
      "slug": "mit-course-188",
      "university_id": 245,
      "additional_university_ids": [

      ],
      "topic_id": 272,
      "discipline_id": 273,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 188",
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
      "updated_at": "2016-10-27T17:43:57.856Z",
      "shortname": "mit-course-188"
    },
    {
      "creator_id": 770,
      "id": 261,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-189",
      "html_url": "https://goskive.com/course/mit-course-189",
      "slug": "mit-course-189",
      "university_id": 246,
      "additional_university_ids": [

      ],
      "topic_id": 273,
      "discipline_id": 274,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 189",
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
      "updated_at": "2016-10-27T17:43:57.935Z",
      "shortname": "mit-course-189"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6f9e2bc551ca10bbd214ae31680258e623f62cdcea1b4607754e24a660cc556"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 80ef0976886ffdc9673313281b6048ca73b037065339a7084bdf4f1abe5c1803
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
        "created_at": "2016-10-27T17:43:21.580Z",
        "updated_at": "2016-10-27T17:43:21.580Z",
        "file_url": "memory://5f911f24636adb4dd8434ca9edd46397.pdf",
        "course_id": 111,
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
        "created_at": "2016-10-27T17:43:21.659Z",
        "updated_at": "2016-10-27T17:43:21.659Z",
        "file_url": "memory://4b485d2c27d5ba40b2075404439be191.pdf",
        "course_id": 112,
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
        "created_at": "2016-10-27T17:43:21.739Z",
        "updated_at": "2016-10-27T17:43:21.739Z",
        "file_url": "memory://b6c8c6d32ed18c734724e2cdf124bbc8.pdf",
        "course_id": 113,
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
	-H "Authorization: Bearer 80ef0976886ffdc9673313281b6048ca73b037065339a7084bdf4f1abe5c1803"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 7325c149492aad6b12581b7658fddacc5be3c055e0be335750611622059b2783
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
        "updated_at": "2016-10-27T17:43:57.602Z"
      },
      "created_at": "2016-10-27T17:43:57.605Z",
      "updated_at": "2016-10-27T17:43:57.605Z",
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
        "updated_at": "2016-10-27T17:43:57.614Z"
      },
      "created_at": "2016-10-27T17:43:57.617Z",
      "updated_at": "2016-10-27T17:43:57.617Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7325c149492aad6b12581b7658fddacc5be3c055e0be335750611622059b2783"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 30a85afbb2e0a2f3433fbff2d482768415a002e4f211a76e3bda2a193674fd7c
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
        "updated_at": "2016-10-27T17:43:57.386Z"
      },
      "created_at": "2016-10-27T17:43:57.391Z",
      "updated_at": "2016-10-27T17:43:57.391Z",
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
        "updated_at": "2016-10-27T17:43:57.404Z"
      },
      "created_at": "2016-10-27T17:43:57.407Z",
      "updated_at": "2016-10-27T17:43:57.407Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30a85afbb2e0a2f3433fbff2d482768415a002e4f211a76e3bda2a193674fd7c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer d1fc7811fa03675206cfc0e38fce9a8895d43b472b190f3f1b7609eb0ab92834
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
      "created_at": "2016-10-27T17:43:08.831Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 47,
      "updated_at": "2016-10-27T17:43:08.928Z",
      "author_id": "231",
      "thread_subject_id": "76",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 5,
      "created_at": "2016-10-27T17:43:08.918Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 48,
      "updated_at": "2016-10-27T17:43:08.931Z",
      "author_id": "234",
      "thread_subject_id": "77",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-27T17:43:09.283Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-27T17:43:09.283Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-27T17:43:09.638Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-27T17:43:09.638Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 8,
      "created_at": "2016-10-27T17:43:09.984Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-27T17:43:09.984Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 9,
      "created_at": "2016-10-27T17:43:10.250Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 18,
      "updated_at": "2016-10-27T17:43:10.250Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-27T17:43:10.520Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 19,
      "updated_at": "2016-10-27T17:43:10.520Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-27T17:43:10.781Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-10-27T17:43:10.781Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1fc7811fa03675206cfc0e38fce9a8895d43b472b190f3f1b7609eb0ab92834"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/3
Content-Type: application/json
Authorization: Bearer ed5d29690f841ca3c9db886eae32055ada6618577b87032cf9905e7279a1eca5
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-27T17:33:08.000Z"}}
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
    "created_at": "2016-10-27T17:43:08.645Z",
    "read_at": "2016-10-27T17:33:08.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 46,
    "updated_at": "2016-10-27T17:43:08.696Z",
    "author_id": "226",
    "thread_subject_id": "75",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/3" -d '{"notification":{"read_at":"2016-10-27T17:33:08.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed5d29690f841ca3c9db886eae32055ada6618577b87032cf9905e7279a1eca5"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 9c7666676a799d9ce75aadc47ef91b69c765f876892534aada3dfd1628d465a0
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
      "course_id": 197,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-27T17:43:44.054Z",
      "course_published": true,
      "updated_at": "2016-10-27T17:43:44.045Z"
    },
    {
      "id": 3,
      "course_id": 198,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-27T17:43:44.136Z",
      "course_published": true,
      "updated_at": "2016-10-27T17:43:44.128Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c7666676a799d9ce75aadc47ef91b69c765f876892534aada3dfd1628d465a0"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 072a2305182a038daf76bff1b007c349e286b4024fdc7a0c353234149a632301
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
    "course_id": 201,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-27T17:43:44.574Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:43:44.566Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 072a2305182a038daf76bff1b007c349e286b4024fdc7a0c353234149a632301"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 35907c19931f40eebb9b29bba08d7c2c241ee948fd6bd8d282508bee79ca8f5f
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
    "course_id": 202,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-27T17:43:44.743Z",
    "course_published": true,
    "updated_at": "2016-10-27T17:43:44.732Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35907c19931f40eebb9b29bba08d7c2c241ee948fd6bd8d282508bee79ca8f5f"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer da1ef99ffcd2c0afb3a341b946c804d3384840ba5f9f4b8ea65820ebb691b68a
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
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 21,
      "user_id": 257
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 22,
      "user_id": 257
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 23,
      "user_id": 257
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 24,
      "user_id": 257
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da1ef99ffcd2c0afb3a341b946c804d3384840ba5f9f4b8ea65820ebb691b68a"
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
      "name": "Cross-platform tertiary focus group",
      "name_translations": {
        "en": "Cross-platform tertiary focus group"
      }
    },
    {
      "id": 2,
      "name": "Secured disintermediate strategy",
      "name_translations": {
        "en": "Secured disintermediate strategy"
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
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer 80ebb22e5fb9e6d2b0cf6ac763e5dfffc7976e3d6f144dbbe5d4222e6fde02c6
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
    "id": 21,
    "user_id": 873,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-27T17:44:04.069Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/21/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80ebb22e5fb9e6d2b0cf6ac763e5dfffc7976e3d6f144dbbe5d4222e6fde02c6"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/fix
Content-Type: application/json
Authorization: Bearer b7a7782d932bb34d8aae39b3cf2b8f2acbd6e5781ef4ea6e0321047a61d95c5a
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
    "id": 44,
    "user_id": 974,
    "feedbackable_id": 93,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-27T17:44:10.974Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/44/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7a7782d932bb34d8aae39b3cf2b8f2acbd6e5781ef4ea6e0321047a61d95c5a"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer 323312aee65e95283e7003a03d45a8a30c2220736d172c4b59a598eba5de2c4f
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
    "id": 19,
    "user_id": 861,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:44:03.623Z",
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
curl "api.goskive.com/v2/feedbacks/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 323312aee65e95283e7003a03d45a8a30c2220736d172c4b59a598eba5de2c4f"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer eaa08eb1d797ef9431eb8f2a09ffd7cbbf651cb81c25c721752287fd1b1797c3
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
curl "api.goskive.com/v2/feedbacks/23/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaa08eb1d797ef9431eb8f2a09ffd7cbbf651cb81c25c721752287fd1b1797c3"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 997f14e82f4a1ec7d15ec8d17bcdc046223dca81d1a9ae2eb8495950011299af
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
	-H "Authorization: Bearer 997f14e82f4a1ec7d15ec8d17bcdc046223dca81d1a9ae2eb8495950011299af"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/fix
Content-Type: application/json
Authorization: Bearer 9f86322eb5aa9b2c831091579429d9e03aa0ea61ea9f3f27bf548a6e197c4163
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
curl "api.goskive.com/v2/feedbacks/46/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f86322eb5aa9b2c831091579429d9e03aa0ea61ea9f3f27bf548a6e197c4163"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 5159d59487920c22e07f883505ee1052ded07997150f1dba323d59bcf76e4de7
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
    "user_id": 866,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:44:03.891Z",
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
curl "api.goskive.com/v2/feedbacks/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5159d59487920c22e07f883505ee1052ded07997150f1dba323d59bcf76e4de7"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/20
Content-Type: application/json
Authorization: Bearer e9102abe4349c30cb718d08a44e3079151675522bb327d340c345cb4c97cd2d7
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
curl "api.goskive.com/v2/files/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9102abe4349c30cb718d08a44e3079151675522bb327d340c345cb4c97cd2d7"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/21/bookmark
Content-Type: application/json
Authorization: Bearer d0b6dabc6f5abcf20d0e4f62f9c9a71dd8f69e18b40fbc00fefcabf20c634b19
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
	-H "Authorization: Bearer d0b6dabc6f5abcf20d0e4f62f9c9a71dd8f69e18b40fbc00fefcabf20c634b19"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer ea82e0d2faed6b637779d5bf26e18508bbd8214358555fc5435ab7c5e748a6dc
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
	-H "Authorization: Bearer ea82e0d2faed6b637779d5bf26e18508bbd8214358555fc5435ab7c5e748a6dc"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer 35d4aa337a9a575ab864b0818339a1bb2fe3a2bc54e05102932ffe629237c48a
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/08027e3ee613b8c07c571fc3c44457fb.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161027%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161027T174400Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=9d03d84dfbc89a10b9ecd404f0308198280713b7ce320e604f0713a5b6a2cd8d",
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
	-H "Authorization: Bearer 35d4aa337a9a575ab864b0818339a1bb2fe3a2bc54e05102932ffe629237c48a"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/16/preview
Content-Type: application/json
Authorization: Bearer 466fd2aaa85a8febb2012ad76e3b0234cd11a3acc5727418aa6555c9ef732f14
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/4b449866bb4208088734d0342a20c1db.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161027%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161027T174401Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=c5e57df08e0708ca36ee02ff5c65e1c32859f2bcff905c5277ce7e89d54d8d0e",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/16/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 466fd2aaa85a8febb2012ad76e3b0234cd11a3acc5727418aa6555c9ef732f14"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 202f78df2d313e7d46c39471412ae764fbc78274fe5e95288887edecb0d91692
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
      "id": 799,
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
      "created_at": "2016-10-27T17:44:00.678Z",
      "updated_at": "2016-10-27T17:44:00.678Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-27T17:44:00.752Z",
    "updated_at": "2016-10-27T17:44:00.752Z",
    "course_id": 271,
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
curl "api.goskive.com/v2/files/14/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 202f78df2d313e7d46c39471412ae764fbc78274fe5e95288887edecb0d91692"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer 8bdcb845387239283928a47a2f86ec1bb7455667e34c54514f61b364eefbc595
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
      "creator_id": 681,
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 216,
      "additional_university_ids": [

      ],
      "topic_id": 221,
      "discipline_id": 222,
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
      "chapters_updated_at": "2016-10-27T17:43:47.565Z",
      "updated_at": "2016-10-27T17:43:49.146Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 686,
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-a6d5bba9-5c3d-4301-90bd-b7f8e08240f0",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-a6d5bba9-5c3d-4301-90bd-b7f8e08240f0",
      "slug": "mit-the-great-british-bake-off-a6d5bba9-5c3d-4301-90bd-b7f8e08240f0",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "topic_id": 222,
      "discipline_id": 223,
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
      "chapters_updated_at": "2016-10-27T17:43:47.565Z",
      "updated_at": "2016-10-27T17:43:49.673Z",
      "shortname": "mit-the-great-british-bake-off-a6d5bba9-5c3d-4301-90bd-b7f8e08240f0"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/8/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 8bdcb845387239283928a47a2f86ec1bb7455667e34c54514f61b364eefbc595"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 1bdd79b7714409889f994beab9dcffd3f8abdf31af848d2224fbc06ddd2d21d6
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
	-H "Authorization: Bearer 1bdd79b7714409889f994beab9dcffd3f8abdf31af848d2224fbc06ddd2d21d6"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/17/bookmark
Content-Type: application/json
Authorization: Bearer 548ceb395e23a7617f2985c4b5e43c88e9c189f5a9aec2e2e073a5ae67de5579
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 548ceb395e23a7617f2985c4b5e43c88e9c189f5a9aec2e2e073a5ae67de5579"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/15/upvote
Content-Type: application/json
Authorization: Bearer e2b07bd3a545d2eed4655fd60ddd4702620d3587eb7f974242a51a9c4ac7836e
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2b07bd3a545d2eed4655fd60ddd4702620d3587eb7f974242a51a9c4ac7836e"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/8/comments
Content-Type: application/json
Authorization: Bearer 2bb466e9077f230ea44ee4f34774d6283886aa78dfe2fd5057ab9ac0f377cf1d
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
    "id": 42,
    "author_id": 207,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:43:07.478Z",
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
curl "api.goskive.com/v2/flashcards/8/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bb466e9077f230ea44ee4f34774d6283886aa78dfe2fd5057ab9ac0f377cf1d"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer 2780e4e4606ed48381c3b5836e46fa43492e05335f5f394f5820948e4d935066
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
    "id": 43,
    "author_id": 210,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:43:07.826Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 210,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:07.822Z",
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
curl "api.goskive.com/v2/flashcards/9/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2780e4e4606ed48381c3b5836e46fa43492e05335f5f394f5820948e4d935066"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer adace461cb77d70daa907060f047388539f1f0686703e32bf58591765ad2713d
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
      "id": 44,
      "author_id": 222,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:08.499Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 223,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:08.514Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adace461cb77d70daa907060f047388539f1f0686703e32bf58591765ad2713d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer 91b2ca1c866b5a25f592205c8c2105bb835f1daadcee219593c37d98062ba55c
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
curl "api.goskive.com/v2/flashcards/10/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91b2ca1c866b5a25f592205c8c2105bb835f1daadcee219593c37d98062ba55c"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/79/feedbacks
Content-Type: application/json
Authorization: Bearer 09883e6a981feec308a6a93fd35018668884e3e8a7a945ac6011b163d86ff646
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
    "id": 11,
    "user_id": 822,
    "feedbackable_id": 79,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:44:01.896Z",
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
curl "api.goskive.com/v2/flashcards/79/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09883e6a981feec308a6a93fd35018668884e3e8a7a945ac6011b163d86ff646"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/82/feedbacks
Content-Type: application/json
Authorization: Bearer 7039623b729575a1817516d6afbedb87db6d17a13d881d6c74a858f35c958bd3
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
      "id": 14,
      "user_id": 835,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:02.656Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 834,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:02.645Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7039623b729575a1817516d6afbedb87db6d17a13d881d6c74a858f35c958bd3"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/69/votes
Content-Type: application/json
Authorization: Bearer 71bf7f357156bbd10ca1f8ea2d77513991689fbb76e3f2742c532ba259b081bf
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
      "votable_id": 69,
      "user_id": 664
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 69,
      "user_id": 663
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 69,
      "user_id": 662
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/69/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71bf7f357156bbd10ca1f8ea2d77513991689fbb76e3f2742c532ba259b081bf"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/62/republish
Content-Type: application/json
Authorization: Bearer 7be9c2a072480def51089ffed2bcdf118014926e4bb097480edd1e87222c1134
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
	-H "Authorization: Bearer 7be9c2a072480def51089ffed2bcdf118014926e4bb097480edd1e87222c1134"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/61/bookmark
Content-Type: application/json
Authorization: Bearer 2ce97c16d2273bdd3a2dcca1c74444655ad48c212ea8aad4a07e8924d53a0ce0
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ce97c16d2273bdd3a2dcca1c74444655ad48c212ea8aad4a07e8924d53a0ce0"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/65
Content-Type: application/json
Authorization: Bearer 1f24e33866d12c9f1a4f164ad3728807f563349536f0f3f1ed76c085b895a1d5
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f24e33866d12c9f1a4f164ad3728807f563349536f0f3f1ed76c085b895a1d5"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/43/downvote
Content-Type: application/json
Authorization: Bearer 4a87e6b8f77abb2b41cc2eae62f033ea9cbeb9ab21d43a78087c2f5384ead81f
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a87e6b8f77abb2b41cc2eae62f033ea9cbeb9ab21d43a78087c2f5384ead81f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/64
Content-Type: application/json
Authorization: Bearer 6d8a75fb9bc238d545ad791065d206b0c79fa6e7a192d208d4a9d81f3c2ed0fc
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
    "author_id": 567,
    "chapter_id": 125,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:43:39.437Z",
    "created_at": "2016-10-27T17:43:39.437Z",
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
	-H "Authorization: Bearer 6d8a75fb9bc238d545ad791065d206b0c79fa6e7a192d208d4a9d81f3c2ed0fc"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/60/report
Content-Type: application/json
Authorization: Bearer fc4a5b6210c318ac107a6eee8e4acf67efaf9ebe506a45104d82b9756b151cf8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/60/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc4a5b6210c318ac107a6eee8e4acf67efaf9ebe506a45104d82b9756b151cf8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/66/bookmark
Content-Type: application/json
Authorization: Bearer 4f73b79837e1be00a2af93c4fd357e8a8fc566f438f24fe73729b635dbc775a7
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f73b79837e1be00a2af93c4fd357e8a8fc566f438f24fe73729b635dbc775a7"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/upvote
Content-Type: application/json
Authorization: Bearer 4039716db70c9302b1b9cc4df752832d6f91c17b1a5946d28380e33060e2c43e
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4039716db70c9302b1b9cc4df752832d6f91c17b1a5946d28380e33060e2c43e"
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
    "key": "cache/d64e4dc8fc037f2a9ea386b112eeea38.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yN1QxODo0Mzo0NFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Q2NGU0ZGM4ZmMwMzdmMmE5ZWEzODZiMTEyZWVlYTM4LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjdUMTc0MzQ0WiJ9XX0=",
    "x-amz-credential": "FAKE/20161027/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161027T174344Z",
    "x-amz-signature": "943d04e035e596e7dd9370f15ac4ada347f6e3a749f7224a679f951e1f7ed8d3"
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
Authorization: Bearer f300d0e3118b29574f2c2e96fe518d2013850533148a41e82b7efe255f70ce28
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
	-H "Authorization: Bearer f300d0e3118b29574f2c2e96fe518d2013850533148a41e82b7efe255f70ce28"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 149a4a53896abb2e4bfbd06bee0b040bbae381a7e89880e8d08d753d8bb83085
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
	-H "Authorization: Bearer 149a4a53896abb2e4bfbd06bee0b040bbae381a7e89880e8d08d753d8bb83085"
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
{"password":{"reset_password_token":"5ztkZazzWJXDq2yZMzMC","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 748,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-27T17:43:55.994Z",
  "updated_at": "2016-10-27T17:43:56.161Z",
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
  "audit_id": 4395
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"5ztkZazzWJXDq2yZMzMC","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Authorization: Bearer af7464ce1fe8f214f70508175ace0694c67d7dfd6bd34eed18cdeed1a7194b61
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
    "id": 56,
    "author_id": 779,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:43:58.942Z",
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
	-H "Authorization: Bearer af7464ce1fe8f214f70508175ace0694c67d7dfd6bd34eed18cdeed1a7194b61"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/115/comments
Content-Type: application/json
Authorization: Bearer 932856a740c4910a9e583041c5ba380c57801b0dd3fde2bd5d5c0c1d9e296d9f
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
    "id": 57,
    "author_id": 785,
    "reply_to_id": null,
    "created_at": "2016-10-27T17:43:59.734Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 10,
      "user_id": 785,
      "feedbackable_id": 115,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:59.731Z",
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
curl "api.goskive.com/v2/questions/115/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 932856a740c4910a9e583041c5ba380c57801b0dd3fde2bd5d5c0c1d9e296d9f"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/112/comments
Content-Type: application/json
Authorization: Bearer 2c6724260045db7768725cc3c22e77bf8e5bf824dba43edc8468362533fd2450
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
      "author_id": 777,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:58.577Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 778,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:58.595Z",
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
curl "api.goskive.com/v2/questions/112/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c6724260045db7768725cc3c22e77bf8e5bf824dba43edc8468362533fd2450"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/114/comments
Content-Type: application/json
Authorization: Bearer 46fd113bf0e3d57e2ff3b729f1a28c85d97d87d4aaf4740213d831f698dec1fd
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
	-H "Authorization: Bearer 46fd113bf0e3d57e2ff3b729f1a28c85d97d87d4aaf4740213d831f698dec1fd"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/88/feedbacks
Content-Type: application/json
Authorization: Bearer bc7d55b63a69c5ffa8cf118c693bd29378b54156548e590cfc69d7d79c6a7404
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
    "user_id": 582,
    "feedbackable_id": 88,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-27T17:43:40.669Z",
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
curl "api.goskive.com/v2/questions/88/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc7d55b63a69c5ffa8cf118c693bd29378b54156548e590cfc69d7d79c6a7404"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer 31cc67168240770ff88f21e1032679f989b68ede086f5d5dfb853bd05842a637
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
      "id": 9,
      "user_id": 617,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:43.297Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 616,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:43.286Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/95/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31cc67168240770ff88f21e1032679f989b68ede086f5d5dfb853bd05842a637"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/97/votes
Content-Type: application/json
Authorization: Bearer 213acb7ff42dadb3f2028590299bc98c1b92f2fe7559d96140d3188ae2e3d48d
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
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 649
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 648
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 647
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/97/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 213acb7ff42dadb3f2028590299bc98c1b92f2fe7559d96140d3188ae2e3d48d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/68/republish
Content-Type: application/json
Authorization: Bearer 00b383248988fd05976abb777e96f491c3336fd9a7e801a1faa40311b2c2ca71
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
curl "api.goskive.com/v2/questions/68/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00b383248988fd05976abb777e96f491c3336fd9a7e801a1faa40311b2c2ca71"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/86/bookmark
Content-Type: application/json
Authorization: Bearer b81bb3acc6550806a4fbdcae25ba678b7f3ff11ab698a9cdb84b54ecb77c9d13
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/86/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b81bb3acc6550806a4fbdcae25ba678b7f3ff11ab698a9cdb84b54ecb77c9d13"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/62
Content-Type: application/json
Authorization: Bearer d2e64f68ceb4852ccbc12fc7f01cbce41f9843690a5746fa2482c051b5918dd9
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/62" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2e64f68ceb4852ccbc12fc7f01cbce41f9843690a5746fa2482c051b5918dd9"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/69/downvote
Content-Type: application/json
Authorization: Bearer 8be53fe7dd1b6ec80b3fc9b84dfe250e24213f7d6f50e90b0a6a9cee177cdcdf
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/69/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8be53fe7dd1b6ec80b3fc9b84dfe250e24213f7d6f50e90b0a6a9cee177cdcdf"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/66
Content-Type: application/json
Authorization: Bearer ea7e2bfd1019ee6b6cec7ae836aa428d497e4797910acdb9625b048d296299f3
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 431,
    "chapter_id": 83,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:43:29.686Z",
    "created_at": "2016-10-27T17:43:29.572Z",
    "tags": [
      {
        "id": 10,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 9,
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
}
```



```shell
curl "api.goskive.com/v2/questions/66" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea7e2bfd1019ee6b6cec7ae836aa428d497e4797910acdb9625b048d296299f3"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/64/report
Content-Type: application/json
Authorization: Bearer 472030cd6ca82a21e77afa432e5613044fdae1ad1c9d83bc13ee377c5451e247
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/64/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 472030cd6ca82a21e77afa432e5613044fdae1ad1c9d83bc13ee377c5451e247"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/63/bookmark
Content-Type: application/json
Authorization: Bearer a3125a5440e04e2f90aa7023ae730b81f6f2d4810adb678bd937446527bb7c56
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/63/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3125a5440e04e2f90aa7023ae730b81f6f2d4810adb678bd937446527bb7c56"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/65
Content-Type: application/json
Authorization: Bearer bb654abc3b9c5f1b521601904c86660c5d4b117ccbb336a736be33c31f11f806
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":65,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-27T17:43:29.083Z","updated_at":"2016-10-27T17:43:29.200Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":82,"author_id":428,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 65,
    "obfuscated_id": "Pu1fo5_Q1vk",
    "author_id": 428,
    "chapter_id": 82,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-27T17:43:29.311Z",
    "created_at": "2016-10-27T17:43:29.083Z",
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
    "question": "{\"id\"=>65, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-27T17:43:29.083Z\", \"updated_at\"=>\"2016-10-27T17:43:29.200Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>82, \"author_id\"=>428, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 132,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 133,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 134,
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
curl "api.goskive.com/v2/questions/65" -d '{"question":{"question":{"id":65,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-27T17:43:29.083Z","updated_at":"2016-10-27T17:43:29.200Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":82,"author_id":428,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb654abc3b9c5f1b521601904c86660c5d4b117ccbb336a736be33c31f11f806"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/70/upvote
Content-Type: application/json
Authorization: Bearer 2850a29f370f4bb0218270e5d89405380d7dcceb7b56312102c51e56ffb33109
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/70/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2850a29f370f4bb0218270e5d89405380d7dcceb7b56312102c51e56ffb33109"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer eecfcb3a2f7af7ae81124606c615e888e28bbd08782794f30fb42c5db3939186
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
      "creator_id": 753,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 239,
      "additional_university_ids": [

      ],
      "topic_id": 267,
      "discipline_id": 268,
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
      "updated_at": "2016-10-27T17:43:56.384Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eecfcb3a2f7af7ae81124606c615e888e28bbd08782794f30fb42c5db3939186"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 6d362f9a320ea21423da6811a02479cf02771b8d09c75725467d09744449a52b
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
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-222",
      "html_url": "https://goskive.com/university/uni-222",
      "slug": "uni-222",
      "name": "National School of Pizza",
      "short_name": "Uni 222",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cff67873362ee3a29d561042c7facb3260161ded.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/92aec2a9b06ccfdaec1185e21c9f1b64ee851392.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:43:56.580Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-221",
      "html_url": "https://goskive.com/university/uni-221",
      "slug": "uni-221",
      "name": "National School of Pastry",
      "short_name": "Uni 221",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/48a2378f71bf32b4659c203b40668d09183285f6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6167303c927184e4d13783875ec6336736353ae3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:43:56.563Z",
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
	-H "Authorization: Bearer 6d362f9a320ea21423da6811a02479cf02771b8d09c75725467d09744449a52b"
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
      "id": 62,
      "name": "Optimized tangible framework",
      "name_translations": {
        "en": "Optimized tangible framework"
      },
      "discipline_id": 63
    },
    {
      "id": 63,
      "name": "Expanded eco-centric attitude",
      "name_translations": {
        "en": "Expanded eco-centric attitude"
      },
      "discipline_id": 64
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
GET /v2/topics/64
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
    "id": 64,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 65
  }
}
```



```shell
curl "api.goskive.com/v2/topics/64" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 9f109688e534175aaeded34984291a0000653a98b4c0959fef499c0fa796c768
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
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-109",
      "html_url": "https://goskive.com/university/uni-109",
      "slug": "uni-109",
      "name": "University 70",
      "short_name": "Uni 109",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/29fc8bca362837c836a5d6d8a1501019fb32da53.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/af2ae58961d5fa915fb5470017502a41936bf8a7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:43:20.537Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-108",
      "html_url": "https://goskive.com/university/uni-108",
      "slug": "uni-108",
      "name": "University 69",
      "short_name": "Uni 108",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/82018de485d26c9bc27540446774b49169a40672.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/185a914e401fa48a03ae327e11f997764d72b2a1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:43:20.521Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-107",
      "html_url": "https://goskive.com/university/uni-107",
      "slug": "uni-107",
      "name": "University 68",
      "short_name": "Uni 107",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4bb8ec2c77619620225b3baa5e95c92743b5375d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2d8a95d4c289fcc26bc01926bad682d4733c5159.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-27T17:43:20.503Z",
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
	-H "Authorization: Bearer 9f109688e534175aaeded34984291a0000653a98b4c0959fef499c0fa796c768"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 441bb96603e3a62d3145d52053287f5e5689f6ef5425f620e8fd71017d1156c0
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
    "id": 107,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/47501c30005ace1e8cf5ce8d311d35f8e8031d1e.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8701d988977fa68699c888ee61dc7050e74864f5.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-27T17:43:20.355Z",
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
	-H "Authorization: Bearer 441bb96603e3a62d3145d52053287f5e5689f6ef5425f620e8fd71017d1156c0"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5355a35db1b12155b6b4293b4b29468a1f7329587a48157fbb28238892053743
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":261,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 738,
    "id": 251,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 234,
    "additional_university_ids": [

    ],
    "topic_id": 261,
    "discipline_id": 262,
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
    "chapters_updated_at": "2016-10-27T17:43:53.744Z",
    "updated_at": "2016-10-27T17:43:53.883Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 152,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-27T17:43:53.838Z",
        "course_id": 251,
        "author_id": 738,
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
        "id": 153,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-27T17:43:53.856Z",
        "course_id": 251,
        "author_id": 738,
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
        "id": 154,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-27T17:43:53.873Z",
        "course_id": 251,
        "author_id": 738,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":261,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5355a35db1b12155b6b4293b4b29468a1f7329587a48157fbb28238892053743"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d39b863958b34170d485490e41baf747e5cd9ad875b22317f54059e88a569209
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":262,"published":false}}
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
    "creator_id": 739,
    "id": 252,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 235,
    "additional_university_ids": [

    ],
    "topic_id": 262,
    "discipline_id": 263,
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
    "updated_at": "2016-10-27T17:43:54.038Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":262,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d39b863958b34170d485490e41baf747e5cd9ad875b22317f54059e88a569209"
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
      "creator_id": 708,
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-161",
      "html_url": "https://goskive.com/course/fu-course-161",
      "slug": "fu-course-161",
      "university_id": 223,
      "additional_university_ids": [

      ],
      "topic_id": 235,
      "discipline_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 161",
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
      "updated_at": "2016-10-27T17:43:51.064Z",
      "shortname": "fu-course-161"
    },
    {
      "creator_id": 708,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 223,
      "additional_university_ids": [

      ],
      "topic_id": 236,
      "discipline_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 162",
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
      "chapters_updated_at": "2016-10-27T17:43:51.360Z",
      "updated_at": "2016-10-27T17:43:51.366Z",
      "shortname": "fu-course-162"
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
Authorization: Bearer d3656868408d15c5a4c825d73e164d428d2e7da6235e6e1ff6b8150c50374fea
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
      "creator_id": 715,
      "id": 233,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "topic_id": 243,
      "discipline_id": 244,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
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
      "updated_at": "2016-10-27T17:43:51.811Z",
      "shortname": "fu-course-169"
    },
    {
      "creator_id": 715,
      "id": 234,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-170",
      "html_url": "https://goskive.com/course/fu-course-170",
      "slug": "fu-course-170",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "topic_id": 244,
      "discipline_id": 245,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 170",
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
      "chapters_updated_at": "2016-10-27T17:43:52.105Z",
      "updated_at": "2016-10-27T17:43:52.112Z",
      "shortname": "fu-course-170"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3656868408d15c5a4c825d73e164d428d2e7da6235e6e1ff6b8150c50374fea"
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
      "creator_id": 713,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 225,
      "additional_university_ids": [

      ],
      "topic_id": 239,
      "discipline_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
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
      "updated_at": "2016-10-27T17:43:51.586Z",
      "shortname": "fu-course-165"
    },
    {
      "creator_id": 713,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 225,
      "additional_university_ids": [

      ],
      "topic_id": 240,
      "discipline_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
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
      "updated_at": "2016-10-27T17:43:51.629Z",
      "shortname": "fu-course-166"
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
Authorization: Bearer 3f926411558ff167dd3446a9e311902ab09f632e32dcd5536864db308629ba6e
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
      "id": 237,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-173",
      "html_url": "https://goskive.com/course/fu-course-173",
      "slug": "fu-course-173",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 247,
      "discipline_id": 248,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
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
      "updated_at": "2016-10-27T17:43:52.423Z",
      "shortname": "fu-course-173"
    },
    {
      "creator_id": 722,
      "id": 238,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-174",
      "html_url": "https://goskive.com/course/fu-course-174",
      "slug": "fu-course-174",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 248,
      "discipline_id": 249,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 174",
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
      "updated_at": "2016-10-27T17:43:52.464Z",
      "shortname": "fu-course-174"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f926411558ff167dd3446a9e311902ab09f632e32dcd5536864db308629ba6e"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 93ef2cd710dbf9e8c0a4ad7e1479a399b40b012a4cf1662e5445508a1459e5d6
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
  "id": 22,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-27T17:42:56.980Z",
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
	-H "Authorization: Bearer 93ef2cd710dbf9e8c0a4ad7e1479a399b40b012a4cf1662e5445508a1459e5d6"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/757
Content-Type: application/json
Authorization: Bearer 67c0dfa62485200a800a64a28fceeb8deb58417eb5b1f3aeab8d330ac2a5f4cf
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
    "id": 757,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 244,
    "fields_of_study": [
      270,
      271
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-27T17:43:56.788Z",
    "updated_at": "2016-10-27T17:43:56.788Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/757" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67c0dfa62485200a800a64a28fceeb8deb58417eb5b1f3aeab8d330ac2a5f4cf"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/759
Content-Type: application/json
Authorization: Bearer 956961c4d2072dbc5588e5744befe185e8c19578302db34fb59bedb4094c0675
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
    "id": 759,
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
    "created_at": "2016-10-27T17:43:56.880Z",
    "updated_at": "2016-10-27T17:43:56.880Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/759" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 956961c4d2072dbc5588e5744befe185e8c19578302db34fb59bedb4094c0675"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/8
Content-Type: application/json
Authorization: Bearer aeccb142ba0382321e34bca3bb4927a2fb277d87d7475d003567ffe0a820f489
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aeccb142ba0382321e34bca3bb4927a2fb277d87d7475d003567ffe0a820f489"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/10
Content-Type: application/json
Authorization: Bearer 0c5adee004b67d97df3057f69a5e3175bf16d4b93a842a22294a82179355c113
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
    "votable_id": 53,
    "user_id": 371
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c5adee004b67d97df3057f69a5e3175bf16d4b93a842a22294a82179355c113"
```
