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
Authorization: Basic ZDQyZWFkYWI2MmZmYTAyNWI5MzE2ZGU3ZjJkYTAzYjY2MjZmMmRiYTU3ZTk5
ZmM0YzRlMzBkODUyMGVjMmE5NjpiYWQxYWE5ODNkNjNkNzk5NDU5YWQxNjI2
Yjk0N2Y3M2ExNzNlZTg1ZWFjN2FjMGVhMjMxOWY4ZWJkNmE4ZmM4

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
	-u d42eadab62ffa025b9316de7f2da03b6626f2dba57e99fc4c4e30d8520ec2a96:bad1aa983d63d799459ad1626b947f73a173ee85eac7ac0ea2319f8ebd6a8fc8
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"76c6fb6f3c2d300581723543dea2a99a18e2b4cafe4abe7ca7ea030903983fdf","client_secret":"ec8c72574532003662e5c0e73ede98659db22f58f9ae03a4083de437d8726b34"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"76c6fb6f3c2d300581723543dea2a99a18e2b4cafe4abe7ca7ea030903983fdf","client_secret":"ec8c72574532003662e5c0e73ede98659db22f58f9ae03a4083de437d8726b34"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"64cecfc9586eda1e5b4174583eb07adcaa499bb4e9af9b4b82f1f0d70335e68e","client_secret":"f0adf7469119a982cac572369aa2fecb4d10d1e2d77bbfcb730c2f1ad39b2572"}
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
  "access_token": "8a19e1eddf9a2e7931118e002d5bcdd4fc391c57c2a15938e2dfa88cf26eafc2",
  "token_type": "bearer",
  "created_at": 1479318087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"64cecfc9586eda1e5b4174583eb07adcaa499bb4e9af9b4b82f1f0d70335e68e","client_secret":"f0adf7469119a982cac572369aa2fecb4d10d1e2d77bbfcb730c2f1ad39b2572"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZWM0ZDdkN2UzMzIxMWY4ZGQxNWY2NTQ2ZjcxNDVkYzI5ZWMyYWYwMmQ2NTY0
YWNhNjE2MWI0MzUzMTU5YjcyZDowOWM5ZmE4NTJlMjVlYjQ3ZWJiNGM3OWYz
ODM3ZjU3ZDZhZWE2YzdmNzQ0NGJjMmNmYjFkNjY1NTBjMzQzMmU5

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
  "access_token": "4c5278c6f40832cdc6ba3d751ceb553f5487c32594e4810e34603d26caeb1aeb",
  "token_type": "bearer",
  "created_at": 1479318087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u ec4d7d7e33211f8dd15f6546f7145dc29ec2af02d6564aca6161b4353159b72d:09c9fa852e25eb47ebb4c79f3837f57d6aea6c7f7444bc2cfb1d66550c3432e9
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a59d33788081a7ae86a4a024d4e56ff34659dcdbddc059d6fe4075e32a8d8cd5","client_secret":"95b1dd5e492334379099f6886eb8f8c52eab3251035e84785a4bbc50610009ae"}
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
  "access_token": "b7928b6fa4d83c060be285bcaea1a20e902b15af94d0205e1a8f61c2f400890e",
  "token_type": "bearer",
  "created_at": 1479318087
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a59d33788081a7ae86a4a024d4e56ff34659dcdbddc059d6fe4075e32a8d8cd5","client_secret":"95b1dd5e492334379099f6886eb8f8c52eab3251035e84785a4bbc50610009ae"}' -X POST \
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
Authorization: Bearer f55d63849a87418abfd9278def7f7e474a00eb77700773a982417606b9d266dc
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
    "company_id": 19,
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
	-H "Authorization: Bearer f55d63849a87418abfd9278def7f7e474a00eb77700773a982417606b9d266dc"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/178/flashcards
Content-Type: application/json
Authorization: Bearer ef4f3b3cb29c13e3d22f3519741f669c6a3b6bae1813c0b7d702d560be73da12
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":178,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 913,
    "chapter_id": 178,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:41.443Z",
    "created_at": "2016-11-16T17:41:41.443Z",
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
curl "api.goskive.com/v2/chapters/178/flashcards" -d '{"flashcard":{"chapter_id":178,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef4f3b3cb29c13e3d22f3519741f669c6a3b6bae1813c0b7d702d560be73da12"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/180/flashcards
Content-Type: application/json
Authorization: Bearer e7db1432a55462de6d116e271955d263dd4a92ff893a1eba6f9b30d1da75fe85
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
      "author_id": 917,
      "chapter_id": 180,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:41.813Z",
      "created_at": "2016-11-16T17:41:41.813Z",
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
      "author_id": 917,
      "chapter_id": 180,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:41.848Z",
      "created_at": "2016-11-16T17:41:41.848Z",
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
      "author_id": 917,
      "chapter_id": 180,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:41.885Z",
      "created_at": "2016-11-16T17:41:41.885Z",
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
curl "api.goskive.com/v2/chapters/180/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7db1432a55462de6d116e271955d263dd4a92ff893a1eba6f9b30d1da75fe85"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/151/questions
Content-Type: application/json
Authorization: Bearer dac2042bfa5d21dc3fe72523080d0ce2fdfee368efd0ee27bd26ef5591c45f60
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":151,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 117,
    "obfuscated_id": "BsA8mEPn8aM",
    "author_id": 827,
    "chapter_id": 151,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:35.076Z",
    "created_at": "2016-11-16T17:41:35.076Z",
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
        "id": 234,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 235,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 236,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 237,
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
curl "api.goskive.com/v2/chapters/151/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":151,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dac2042bfa5d21dc3fe72523080d0ce2fdfee368efd0ee27bd26ef5591c45f60"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/150/questions
Content-Type: application/json
Authorization: Bearer 76e17c16e4518ac67bd25090cda761789107561f1cb0839ddf12d4805f4a61ef
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":150,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 116,
    "obfuscated_id": "PhHGVKqnHFA",
    "author_id": 824,
    "chapter_id": 150,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:34.506Z",
    "created_at": "2016-11-16T17:41:34.506Z",
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
        "id": 232,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 233,
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
curl "api.goskive.com/v2/chapters/150/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":150,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76e17c16e4518ac67bd25090cda761789107561f1cb0839ddf12d4805f4a61ef"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/152/questions
Content-Type: application/json
Authorization: Bearer 166fa4a449d94f79838a654ac9badf2ef99d21563dcb87b51c0d68f41515d7d7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":152,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 118,
    "obfuscated_id": "ET3wO26jBck",
    "author_id": 830,
    "chapter_id": 152,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:35.823Z",
    "created_at": "2016-11-16T17:41:35.823Z",
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
        "id": 238,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 239,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/152/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":152,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 166fa4a449d94f79838a654ac9badf2ef99d21563dcb87b51c0d68f41515d7d7"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/153/questions
Content-Type: application/json
Authorization: Bearer 0cde9b9e3d9b482d7b64d4968a5a43613b2fb967a9ace07ecadcdf8ba1aea9b7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":153,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 119,
    "obfuscated_id": "JRh8sWka24Y",
    "author_id": 833,
    "chapter_id": 153,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:36.392Z",
    "created_at": "2016-11-16T17:41:36.392Z",
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
        "id": 240,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 241,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 242,
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
curl "api.goskive.com/v2/chapters/153/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":153,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cde9b9e3d9b482d7b64d4968a5a43613b2fb967a9ace07ecadcdf8ba1aea9b7"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/149/questions
Content-Type: application/json
Authorization: Bearer 16e7629e2bc4bbe60b138120b0b5b7894416cf421f7c3e1bd6fee40ba59a7039
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
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 818,
      "chapter_id": 149,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:33.824Z",
      "created_at": "2016-11-16T17:41:33.687Z",
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
          "id": 226,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 227,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 819,
      "chapter_id": 149,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:34.031Z",
      "created_at": "2016-11-16T17:41:33.900Z",
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
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 820,
      "chapter_id": 149,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:41:34.244Z",
      "created_at": "2016-11-16T17:41:34.110Z",
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
          "id": 230,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 231,
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
curl "api.goskive.com/v2/chapters/149/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16e7629e2bc4bbe60b138120b0b5b7894416cf421f7c3e1bd6fee40ba59a7039"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/98
Content-Type: application/json
Authorization: Bearer 5cd32a5383f5b84a985432073a98338a8b6a343834f6c72a8f0674a3cb356795
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
curl "api.goskive.com/v2/chapters/98" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5cd32a5383f5b84a985432073a98338a8b6a343834f6c72a8f0674a3cb356795"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/100
Content-Type: application/json
Authorization: Bearer ab4076b87212779f5e76c0aa2d29fc3732cb0f7670b7513641915945b0e9ef92
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
curl "api.goskive.com/v2/chapters/100" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab4076b87212779f5e76c0aa2d29fc3732cb0f7670b7513641915945b0e9ef92"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/106
Content-Type: application/json
Authorization: Bearer 18b8aaa12cd90d09f5f12dcf1c4074617d7a6697727048cef6b06176c01305bd
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
curl "api.goskive.com/v2/chapters/106" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18b8aaa12cd90d09f5f12dcf1c4074617d7a6697727048cef6b06176c01305bd"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/101
Content-Type: application/json
Authorization: Bearer c5416be3b59d1ee77fcde8beab7c4999fd847ee7e7791742a26c8247e4db4078
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5416be3b59d1ee77fcde8beab7c4999fd847ee7e7791742a26c8247e4db4078"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/102
Content-Type: application/json
Authorization: Bearer 4137f9a7fb71491e58c5ee648ab5282409b5b07e6bab4319edc780b786129868
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
    "id": 102,
    "updated_at": "2016-11-16T17:41:01.914Z",
    "course_id": 115,
    "author_id": 431,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-16T17:41:01.355Z",
    "questions_updated_at": "2016-11-16T17:41:01.355Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 435,
        "chapter_id": 102,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:01.896Z",
        "created_at": "2016-11-16T17:41:01.896Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 433,
        "chapter_id": 102,
        "position": 61,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:01.791Z",
        "created_at": "2016-11-16T17:41:01.667Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/102" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4137f9a7fb71491e58c5ee648ab5282409b5b07e6bab4319edc780b786129868"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/104
Content-Type: application/json
Authorization: Bearer 071e3edf2e8c48e104ad52905cba49ccf80aa1136d2c3383b028daf3e23efd2a
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
    "id": 104,
    "updated_at": "2016-11-16T17:41:02.723Z",
    "course_id": 117,
    "author_id": 445,
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
curl "api.goskive.com/v2/chapters/104" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 071e3edf2e8c48e104ad52905cba49ccf80aa1136d2c3383b028daf3e23efd2a"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/52/replies
Content-Type: application/json
Authorization: Bearer 3c96bc6f94d7e4d50c03f0fd51df76a4dd8555ca5c8a2ac5abd9a017f59cd164
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
    "id": 53,
    "author_id": 773,
    "reply_to_id": 52,
    "created_at": "2016-11-16T17:41:29.549Z",
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
curl "api.goskive.com/v2/comments/52/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c96bc6f94d7e4d50c03f0fd51df76a4dd8555ca5c8a2ac5abd9a017f59cd164"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer a439b50b1ddfabb4baed912c97692a3c1500f5bbe40d4357ff068f203061b685
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
	-H "Authorization: Bearer a439b50b1ddfabb4baed912c97692a3c1500f5bbe40d4357ff068f203061b685"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer 6a81fd320bb8b8a3f17a85d428ccf2e3148d63baf3fc8dc3d2e55bed6cb83974
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
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a81fd320bb8b8a3f17a85d428ccf2e3148d63baf3fc8dc3d2e55bed6cb83974"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/9/republish
Content-Type: application/json
Authorization: Bearer 17a0930189115fc99c6d4ea70bf3a6724b7f3c061a5be3d9362cf6430a952048
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
	-H "Authorization: Bearer 17a0930189115fc99c6d4ea70bf3a6724b7f3c061a5be3d9362cf6430a952048"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer ce1573b6515af5682feaac5801e2aca39977160773ba69b11aa61aa127d0295e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce1573b6515af5682feaac5801e2aca39977160773ba69b11aa61aa127d0295e"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/10/report
Content-Type: application/json
Authorization: Bearer ba3bdb99cfa3eaafabdcd52b316da9402bb0d02f207778b6cb2181bb21833ec6
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/10/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba3bdb99cfa3eaafabdcd52b316da9402bb0d02f207778b6cb2181bb21833ec6"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/1
Content-Type: application/json
Authorization: Bearer 1f5eb79f171e111da1fdf2a3b9c67526a6a0b58722d513e253df6323da4f39ef
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
    "updated_at": "2016-11-16T17:40:39.660Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f5eb79f171e111da1fdf2a3b9c67526a6a0b58722d513e253df6323da4f39ef"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer c3553dce707198915474e5b1c2fb96596e68a067cccefc496d39c0eb17ddea2e
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
      "updated_at": "2016-11-16T17:40:39.752Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-16T17:40:39.756Z"
    },
    {
      "id": 4,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-16T17:40:39.760Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3553dce707198915474e5b1c2fb96596e68a067cccefc496d39c0eb17ddea2e"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer 05f01c04e5238d67a365b19bfd4722ca6c790508b2e3036841180f8bf71362bd
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05f01c04e5238d67a365b19bfd4722ca6c790508b2e3036841180f8bf71362bd"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer ab3bd5b0fd12635486080af1218e8a3437e4ea18e2380f0cb5cd7ce80388692b
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab3bd5b0fd12635486080af1218e8a3437e4ea18e2380f0cb5cd7ce80388692b"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 5b2a8e29edba7d2b3e18f39a87f0faf37adb652a22bc2fe35eef42959af70dd7
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
	-H "Authorization: Bearer 5b2a8e29edba7d2b3e18f39a87f0faf37adb652a22bc2fe35eef42959af70dd7"
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
Authorization: Bearer fe72033eabdd9f7cbf762ccdf385fcf2dc28b22774169b65bc11dc269e6b2d35
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
	-H "Authorization: Bearer fe72033eabdd9f7cbf762ccdf385fcf2dc28b22774169b65bc11dc269e6b2d35"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6144114817b866fbb06157d0cbd87cdea90d26f6e97b1b4b6548fa800453a9b7
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
    "id": 71,
    "updated_at": "2016-11-16T17:40:53.448Z",
    "course_id": 79,
    "author_id": 319,
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
	-H "Authorization: Bearer 6144114817b866fbb06157d0cbd87cdea90d26f6e97b1b4b6548fa800453a9b7"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 94fbc5a05985b05261d1ddade22eb5cb382fe9e29d841b59ee88f877d18a8923
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
      "id": 77,
      "updated_at": "2016-11-16T17:40:55.061Z",
      "course_id": 85,
      "author_id": 334,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 74",
      "position": 1
    },
    {
      "id": 78,
      "updated_at": "2016-11-16T17:40:55.083Z",
      "course_id": 85,
      "author_id": 335,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 75",
      "position": 2
    },
    {
      "id": 79,
      "updated_at": "2016-11-16T17:40:55.334Z",
      "course_id": 85,
      "author_id": 336,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-16T17:40:54.988Z",
      "questions_updated_at": "2016-11-16T17:40:54.988Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 76",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94fbc5a05985b05261d1ddade22eb5cb382fe9e29d841b59ee88f877d18a8923"
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
      "id": 83,
      "updated_at": "2016-11-16T17:40:55.809Z",
      "course_id": 88,
      "author_id": 348,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 80",
      "position": 1
    },
    {
      "id": 84,
      "updated_at": "2016-11-16T17:40:55.832Z",
      "course_id": 88,
      "author_id": 349,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 81",
      "position": 2
    },
    {
      "id": 85,
      "updated_at": "2016-11-16T17:40:56.084Z",
      "course_id": 88,
      "author_id": 350,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-16T17:40:55.732Z",
      "questions_updated_at": "2016-11-16T17:40:55.732Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 82",
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
Authorization: Bearer c58a8cbdac801d7fa91d7c2e8c6f0c8e79d0d6b3e57320dbb742f10fde110fc6
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
      "id": 80,
      "updated_at": "2016-11-16T17:40:55.494Z",
      "course_id": 86,
      "author_id": 341,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 77",
      "position": 1
    },
    {
      "id": 81,
      "updated_at": "2016-11-16T17:40:55.519Z",
      "course_id": 86,
      "author_id": 342,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 78",
      "position": 2
    },
    {
      "id": 82,
      "updated_at": "2016-11-16T17:40:55.544Z",
      "course_id": 86,
      "author_id": 343,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 79",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c58a8cbdac801d7fa91d7c2e8c6f0c8e79d0d6b3e57320dbb742f10fde110fc6"
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
      "id": 86,
      "updated_at": "2016-11-16T17:40:56.295Z",
      "course_id": 90,
      "author_id": 355,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 83",
      "position": 1
    },
    {
      "id": 87,
      "updated_at": "2016-11-16T17:40:56.320Z",
      "course_id": 90,
      "author_id": 356,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 84",
      "position": 2
    },
    {
      "id": 88,
      "updated_at": "2016-11-16T17:40:56.345Z",
      "course_id": 90,
      "author_id": 357,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 85",
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
Authorization: Bearer 43eb3db55f1571bfe83d8aa765c0a43212760cc08eddfc61aeb614a6c578254b
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
    "course_id": 110,
    "user_id": 417,
    "updated_at": "2016-11-16T17:41:00.304Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43eb3db55f1571bfe83d8aa765c0a43212760cc08eddfc61aeb614a6c578254b"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer a2ffa653481fcb54d511b5468cd75d1d7c2f1cb48839c19f24ea66dd06dcb887
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
      "course_id": 105,
      "user_id": 403,
      "updated_at": "2016-11-16T17:40:59.604Z"
    },
    {
      "id": 3,
      "course_id": 105,
      "user_id": 404,
      "updated_at": "2016-11-16T17:40:59.619Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2ffa653481fcb54d511b5468cd75d1d7c2f1cb48839c19f24ea66dd06dcb887"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/71/files
Content-Type: application/json
Authorization: Bearer 5024faff0328148caed21c9876d7f9e1d29033127e105df934c02d65ab3cfbc6
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
      "id": 3,
      "uploader": {
        "id": 293,
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
        "created_at": "2016-11-16T17:40:51.809Z",
        "updated_at": "2016-11-16T17:40:51.809Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:40:51.819Z",
      "updated_at": "2016-11-16T17:40:51.819Z",
      "course_id": 71,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 294,
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
        "created_at": "2016-11-16T17:40:51.826Z",
        "updated_at": "2016-11-16T17:40:51.826Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:40:51.835Z",
      "updated_at": "2016-11-16T17:40:51.835Z",
      "course_id": 71,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 295,
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
        "created_at": "2016-11-16T17:40:51.842Z",
        "updated_at": "2016-11-16T17:40:51.842Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:40:51.852Z",
      "updated_at": "2016-11-16T17:40:51.852Z",
      "course_id": 71,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/71/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5024faff0328148caed21c9876d7f9e1d29033127e105df934c02d65ab3cfbc6"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/72/files
Content-Type: application/json
Authorization: Bearer 1c8b6d0f9da3d7605e930e770057595121c6e9d66da4a959733f5a78ab4b9f34
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
      "id": 298,
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
      "created_at": "2016-11-16T17:40:51.970Z",
      "updated_at": "2016-11-16T17:40:51.970Z"
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
    "created_at": "2016-11-16T17:40:52.001Z",
    "updated_at": "2016-11-16T17:40:52.001Z",
    "course_id": 72,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/72/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c8b6d0f9da3d7605e930e770057595121c6e9d66da4a959733f5a78ab4b9f34"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/73/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer a5662bf627bb1f20aedce2dafb15ed5a56dce20ad1f4e6e2c06eb29c70eb4d1d
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
    "key": "cache/fb4e32400939725661769a3d7fba55c3.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xNlQxODo0MDo1MloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2ZiNGUzMjQwMDkzOTcyNTY2MTc2OWEzZDdmYmE1NWMzLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE2VDE3NDA1MloifV19",
    "x-amz-credential": "FAKE/20161116/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161116T174052Z",
    "x-amz-signature": "8e78b480321643d9f1b83b1bb8aaf7c37ffd671bd95c55bceaba58dad91cb910"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/73/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5662bf627bb1f20aedce2dafb15ed5a56dce20ad1f4e6e2c06eb29c70eb4d1d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 5eddda40b9c4636cd6f0ef8c269926c0f8a38f8bf399cff64d70f27ca31c38eb
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
	-H "Authorization: Bearer 5eddda40b9c4636cd6f0ef8c269926c0f8a38f8bf399cff64d70f27ca31c38eb"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8709d97e374257555bd13575ae1aee368e05c125f66fdb9ef4245782cf562abe
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
	-H "Authorization: Bearer 8709d97e374257555bd13575ae1aee368e05c125f66fdb9ef4245782cf562abe"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 45d0496e7ccc6c48a663938a90ec8cf147a7d8933d826ec9d22398f759a29a7f
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
	-H "Authorization: Bearer 45d0496e7ccc6c48a663938a90ec8cf147a7d8933d826ec9d22398f759a29a7f"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6e16b595f9edcdac9b2e4c7b53b132fe337980b19ea6918711d500160200a651
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
	-H "Authorization: Bearer 6e16b595f9edcdac9b2e4c7b53b132fe337980b19ea6918711d500160200a651"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a077ddafef0c01b42418610730de6b2eb6635e0bf095154ec6541241f4355f00
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
	-H "Authorization: Bearer a077ddafef0c01b42418610730de6b2eb6635e0bf095154ec6541241f4355f00"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 88b6fd210bcdb5c3d8f650e1d41eb383adc1f8b5b76be3a1c28cd208c2d528d4
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
    "creator_id": 545,
    "id": 149,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 150,
    "additional_university_ids": [

    ],
    "discipline_id": 162,
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
    "chapters_updated_at": "2016-11-16T17:41:11.398Z",
    "updated_at": "2016-11-16T17:41:12.954Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 546,
        "chapter_id": 117,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.737Z",
        "created_at": "2016-11-16T17:41:12.737Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 546,
        "chapter_id": 118,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.812Z",
        "created_at": "2016-11-16T17:41:12.812Z",
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
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 546,
        "chapter_id": 117,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.779Z",
        "created_at": "2016-11-16T17:41:12.779Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 546,
        "chapter_id": 118,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.854Z",
        "created_at": "2016-11-16T17:41:12.854Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 546,
        "chapter_id": 117,
        "position": 75,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:11.628Z",
        "created_at": "2016-11-16T17:41:11.503Z",
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
        "author_id": 546,
        "chapter_id": 117,
        "position": 76,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:11.816Z",
        "created_at": "2016-11-16T17:41:11.696Z",
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
            "id": 170,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 171,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 546,
        "chapter_id": 118,
        "position": 77,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.033Z",
        "created_at": "2016-11-16T17:41:11.903Z",
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
      },
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 546,
        "chapter_id": 118,
        "position": 78,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:12.253Z",
        "created_at": "2016-11-16T17:41:12.104Z",
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
            "id": 174,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 175,
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
        "id": 117,
        "updated_at": "2016-11-16T17:41:12.906Z",
        "course_id": 149,
        "author_id": 545,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:41:11.398Z",
        "questions_updated_at": "2016-11-16T17:41:11.398Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 105",
        "position": 1
      },
      {
        "id": 118,
        "updated_at": "2016-11-16T17:41:12.946Z",
        "course_id": 149,
        "author_id": 545,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:41:11.398Z",
        "questions_updated_at": "2016-11-16T17:41:11.398Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 106",
        "position": 2
      }
    ],
    "topic_id": 161,
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
	-H "Authorization: Bearer 88b6fd210bcdb5c3d8f650e1d41eb383adc1f8b5b76be3a1c28cd208c2d528d4"
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
    "creator_id": 551,
    "id": 150,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 151,
    "additional_university_ids": [

    ],
    "discipline_id": 163,
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
    "chapters_updated_at": "2016-11-16T17:41:13.078Z",
    "updated_at": "2016-11-16T17:41:14.607Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 551,
        "chapter_id": 119,
        "position": 81,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:13.296Z",
        "created_at": "2016-11-16T17:41:13.172Z",
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
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 551,
        "chapter_id": 120,
        "position": 83,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:41:13.701Z",
        "created_at": "2016-11-16T17:41:13.570Z",
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
      }
    ],
    "chapters": [
      {
        "id": 119,
        "updated_at": "2016-11-16T17:41:14.557Z",
        "course_id": 150,
        "author_id": 551,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:41:13.078Z",
        "questions_updated_at": "2016-11-16T17:41:13.078Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 107",
        "position": 1
      },
      {
        "id": 120,
        "updated_at": "2016-11-16T17:41:14.599Z",
        "course_id": 150,
        "author_id": 551,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:41:13.078Z",
        "questions_updated_at": "2016-11-16T17:41:13.078Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 108",
        "position": 2
      }
    ],
    "topic_id": 162,
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
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/137/pin
Content-Type: application/json
Authorization: Bearer a32d1dfe615871c2cae6a9cb9a6c3e3f316e69f6095ab084b02f25e69f379497
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/137/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a32d1dfe615871c2cae6a9cb9a6c3e3f316e69f6095ab084b02f25e69f379497"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/147/pin
Content-Type: application/json
Authorization: Bearer fe8df8ac1d8a8e8888c1e13895c103a93bf2a1dcd7f621f588b79be8a4e49863
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/147/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe8df8ac1d8a8e8888c1e13895c103a93bf2a1dcd7f621f588b79be8a4e49863"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 87a54f13580ae761eb08bd2186d9000b76d51f97ff2383367c57d82eb5f9f01a
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
    "creator_id": 562,
    "id": 152,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 153,
    "additional_university_ids": [

    ],
    "discipline_id": 165,
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
    "updated_at": "2016-11-16T17:41:16.415Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 164,
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
	-H "Authorization: Bearer 87a54f13580ae761eb08bd2186d9000b76d51f97ff2383367c57d82eb5f9f01a"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 4ad7117d1b92340ddc105255e2819b7f26164ff8f17db53d1cb93944a60d496c
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
    "id": 134,
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
    "created_at": "2016-11-16T17:40:28.469Z",
    "updated_at": "2016-11-16T17:40:28.469Z",
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
	-H "Authorization: Bearer 4ad7117d1b92340ddc105255e2819b7f26164ff8f17db53d1cb93944a60d496c"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1021352815994e82a1bde1618ef43371e8a07bb4207195bc753a6a0547fd39b0
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[31]}
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
    "id": 130,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      31
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-16T17:40:28.207Z",
    "updated_at": "2016-11-16T17:40:28.241Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[31]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1021352815994e82a1bde1618ef43371e8a07bb4207195bc753a6a0547fd39b0"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer db24b01cf4fbc300b69d1e57d495b6811840d88eeebf053ca1a19ce02d187bae
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
    "id": 131,
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
    "created_at": "2016-11-16T17:40:28.261Z",
    "updated_at": "2016-11-16T17:40:28.261Z",
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
	-H "Authorization: Bearer db24b01cf4fbc300b69d1e57d495b6811840d88eeebf053ca1a19ce02d187bae"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 07ca1db2849e375c3b799d163ec4f174be197764898ea24c1fcb3e94e73c75e6
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[33]}
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
    "id": 132,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      33
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-16T17:40:28.350Z",
    "updated_at": "2016-11-16T17:40:28.350Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[33]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07ca1db2849e375c3b799d163ec4f174be197764898ea24c1fcb3e94e73c75e6"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b5f860a357bbe2d25be8ad8a844c1a3296e23439544edb7258e247056e58d44f
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

30
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
    "id": 129,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/d42b275acefa555baf1361eeaba7d0828aff891c.jpg",
    "university_id": null,
    "fields_of_study": [
      30
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-16T17:40:27.885Z",
    "updated_at": "2016-11-16T17:40:28.145Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/7c03e5c8d23fcbb588b2f844eb474dc466fe590d.jpg",
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

30
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b5f860a357bbe2d25be8ad8a844c1a3296e23439544edb7258e247056e58d44f"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 6fa77990fca79e5885a6229612328163aa5b98e6e07ff7663ba573bbb987101f
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
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 65,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 66,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fa77990fca79e5885a6229612328163aa5b98e6e07ff7663ba573bbb987101f"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 6783dceccdc10565dd8f5a53e454b10219f8c723014cf2edb23c790a3893e6f2
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
      "company_id": 24,
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
      "company_id": 25,
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
	-H "Authorization: Bearer 6783dceccdc10565dd8f5a53e454b10219f8c723014cf2edb23c790a3893e6f2"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 15b545022a62746373318f0517d73447aaff97baa0b54bab0682ec1f6f52ccaf
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
      "company_id": 20,
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
	-H "Authorization: Bearer 15b545022a62746373318f0517d73447aaff97baa0b54bab0682ec1f6f52ccaf"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer aea88ea92ca735a006fba6e9a3869cc856201ef4326d1b7795625dfcd5ae92e7
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
      "creator_id": 400,
      "id": 103,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-82",
      "html_url": "https://goskive.com/course/mit-course-82",
      "slug": "mit-course-82",
      "university_id": 103,
      "additional_university_ids": [

      ],
      "discipline_id": 111,
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
      "updated_at": "2016-11-16T17:40:59.409Z",
      "shortname": "mit-course-82",
      "topic_id": 110,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 82",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 401,
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-83",
      "html_url": "https://goskive.com/course/mit-course-83",
      "slug": "mit-course-83",
      "university_id": 104,
      "additional_university_ids": [

      ],
      "discipline_id": 112,
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
      "updated_at": "2016-11-16T17:40:59.485Z",
      "shortname": "mit-course-83",
      "topic_id": 111,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 83",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aea88ea92ca735a006fba6e9a3869cc856201ef4326d1b7795625dfcd5ae92e7"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer ede9086f352634e5f192adcebde542b79f98f99bb03422f6ce39acaaaaa305d6
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
        "id": 20,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-11-16T17:41:30.586Z",
        "updated_at": "2016-11-16T17:41:30.586Z",
        "file_url": "memory://59c15ee8891acefcd6d0875f2e76ceb8.pdf",
        "course_id": 255,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 21,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-16T17:41:30.666Z",
        "updated_at": "2016-11-16T17:41:30.666Z",
        "file_url": "memory://109671dd848812c89df82f6e3fae0964.pdf",
        "course_id": 256,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 22,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-16T17:41:30.746Z",
        "updated_at": "2016-11-16T17:41:30.746Z",
        "file_url": "memory://9383b92ad4b87987c214a16b7aa1ff7c.pdf",
        "course_id": 257,
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
	-H "Authorization: Bearer ede9086f352634e5f192adcebde542b79f98f99bb03422f6ce39acaaaaa305d6"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 12aded1c0f4b54a4cb2c8dd85b134c9d3cc8d58ac24052287cfc743e93fbec2d
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-16T17:40:59.134Z"
      },
      "created_at": "2016-11-16T17:40:59.138Z",
      "updated_at": "2016-11-16T17:40:59.138Z",
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
      "company_id": 11,
      "company": {
        "id": 11,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-16T17:40:59.145Z"
      },
      "created_at": "2016-11-16T17:40:59.148Z",
      "updated_at": "2016-11-16T17:40:59.148Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12aded1c0f4b54a4cb2c8dd85b134c9d3cc8d58ac24052287cfc743e93fbec2d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 917926bc23cdaf63f6da88d7be0c688f5921cad857e5ad5beecc6e554cd85222
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 5",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-16T17:40:58.931Z"
      },
      "created_at": "2016-11-16T17:40:58.935Z",
      "updated_at": "2016-11-16T17:40:58.935Z",
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-16T17:40:58.950Z"
      },
      "created_at": "2016-11-16T17:40:58.953Z",
      "updated_at": "2016-11-16T17:40:58.953Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 917926bc23cdaf63f6da88d7be0c688f5921cad857e5ad5beecc6e554cd85222"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 7cb3d49d207bc01c37ad1e6e600894e651ad7b13eabeec4fce98d74f112f47a4
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
      "id": 20,
      "created_at": "2016-11-16T17:41:45.950Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-11-16T17:41:46.071Z",
      "author_id": "959",
      "thread_subject_id": "309",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 21,
      "created_at": "2016-11-16T17:41:46.058Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 60,
      "updated_at": "2016-11-16T17:41:46.074Z",
      "author_id": "962",
      "thread_subject_id": "310",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 22,
      "created_at": "2016-11-16T17:41:46.442Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-11-16T17:41:46.442Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 23,
      "created_at": "2016-11-16T17:41:46.847Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-11-16T17:41:46.847Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 24,
      "created_at": "2016-11-16T17:41:47.216Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 23,
      "updated_at": "2016-11-16T17:41:47.216Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 25,
      "created_at": "2016-11-16T17:41:47.513Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 132,
      "updated_at": "2016-11-16T17:41:47.513Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 26,
      "created_at": "2016-11-16T17:41:47.823Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 133,
      "updated_at": "2016-11-16T17:41:47.823Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 27,
      "created_at": "2016-11-16T17:41:48.116Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 134,
      "updated_at": "2016-11-16T17:41:48.116Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cb3d49d207bc01c37ad1e6e600894e651ad7b13eabeec4fce98d74f112f47a4"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/19
Content-Type: application/json
Authorization: Bearer 7909ff2c70a0dce8306de6a707793ef3cbdef4444c62f473876e3d1bea1a0001
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-16T17:31:45.000Z"}}
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
    "id": 19,
    "created_at": "2016-11-16T17:41:45.740Z",
    "read_at": "2016-11-16T17:31:45.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-11-16T17:41:45.797Z",
    "author_id": "954",
    "thread_subject_id": "308",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/19" -d '{"notification":{"read_at":"2016-11-16T17:31:45.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7909ff2c70a0dce8306de6a707793ef3cbdef4444c62f473876e3d1bea1a0001"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 712d55885bf3833c4b74a0ed4c8d8616a942ba76d3e4e6836bad6a5ab64f36fe
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
      "id": 1,
      "course_id": 97,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-16T17:40:58.160Z",
      "course_published": true,
      "updated_at": "2016-11-16T17:40:58.152Z"
    },
    {
      "id": 2,
      "course_id": 98,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-16T17:40:58.244Z",
      "course_published": true,
      "updated_at": "2016-11-16T17:40:58.236Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 712d55885bf3833c4b74a0ed4c8d8616a942ba76d3e4e6836bad6a5ab64f36fe"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer f49db4168c16147408b42e1211bacee31dd798960b132c1fe40478e174e3b978
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
    "id": 4,
    "course_id": 101,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-16T17:40:58.704Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:40:58.697Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f49db4168c16147408b42e1211bacee31dd798960b132c1fe40478e174e3b978"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer eb0cc623eb4090ae8d4210a00e1841a7a3e5d2d81bd44b2b30b82c96c1e58d6b
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
    "course_id": 102,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-16T17:40:58.864Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:40:58.854Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb0cc623eb4090ae8d4210a00e1841a7a3e5d2d81bd44b2b30b82c96c1e58d6b"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer a002bfd5db95e13e0a7c0ef2e631a513d8d2ecdf71452e97ee79b1fd3d7e4fa8
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
      "votable_id": 120,
      "user_id": 921
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 121,
      "user_id": 921
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 122,
      "user_id": 921
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 921
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a002bfd5db95e13e0a7c0ef2e631a513d8d2ecdf71452e97ee79b1fd3d7e4fa8"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/77
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
    "id": 77,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 75,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 77
      },
      {
        "id": 76,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 77
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/77" -X GET \
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
      "id": 75,
      "name": "Polarised interactive conglomeration",
      "name_translations": {
        "en": "Polarised interactive conglomeration"
      }
    },
    {
      "id": 76,
      "name": "Devolved regional framework",
      "name_translations": {
        "en": "Devolved regional framework"
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
Authorization: Bearer 41b192421c3149d3798095d547bc92a1f55053ab7ddc04906381b1e7cb2cc7c1
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
    "user_id": 14,
    "feedbackable_id": 3,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-16T17:40:20.294Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41b192421c3149d3798095d547bc92a1f55053ab7ddc04906381b1e7cb2cc7c1"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 85941bfc5be952ba0bb91ec5df2fd971372cfc6080291a156986877d2762539a
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
    "id": 27,
    "user_id": 122,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-16T17:40:27.477Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85941bfc5be952ba0bb91ec5df2fd971372cfc6080291a156986877d2762539a"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/23
Content-Type: application/json
Authorization: Bearer 03cee7241544902031ef85c9baccbb15fb44716bc3aea3531bf367230c91ee2c
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
    "id": 23,
    "user_id": 100,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:40:26.415Z",
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
curl "api.goskive.com/v2/feedbacks/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03cee7241544902031ef85c9baccbb15fb44716bc3aea3531bf367230c91ee2c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer 5bab0364fe615556a8556fbe384ca8bbd3c2614cfb1ac2d3845e507389a16dbb
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
	-H "Authorization: Bearer 5bab0364fe615556a8556fbe384ca8bbd3c2614cfb1ac2d3845e507389a16dbb"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer c9414994ae270ee0896e6a58d72980270b3b2505ee315af3d96e97ce94577336
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
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9414994ae270ee0896e6a58d72980270b3b2505ee315af3d96e97ce94577336"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer bfee6edc3a5accffd59bbefbf45872272c6dfeae890a927062a721c1fc4d0571
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
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfee6edc3a5accffd59bbefbf45872272c6dfeae890a927062a721c1fc4d0571"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/24
Content-Type: application/json
Authorization: Bearer 360cfca26c98697859ebe83d9ad18bd7f4a8aaf4afdb6d05f5b7f0529958b538
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
    "id": 24,
    "user_id": 105,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:40:26.714Z",
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
curl "api.goskive.com/v2/feedbacks/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 360cfca26c98697859ebe83d9ad18bd7f4a8aaf4afdb6d05f5b7f0529958b538"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 8b2ea2fb39be70b35e4a078d25dde14c40d15a05aff87417f7b7fedf9e94a1aa
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
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b2ea2fb39be70b35e4a078d25dde14c40d15a05aff87417f7b7fedf9e94a1aa"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/14/bookmark
Content-Type: application/json
Authorization: Bearer 72256384e9410e740fd578558084493591d258929d5f5644eba8e56d31c5929f
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72256384e9410e740fd578558084493591d258929d5f5644eba8e56d31c5929f"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer 0e4b37e1b43618c2769091654b221ed0d98278d3a0d64731bdac1a4d565f8d42
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e4b37e1b43618c2769091654b221ed0d98278d3a0d64731bdac1a4d565f8d42"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/13
Content-Type: application/json
Authorization: Bearer 7f88aae649faff40caa4afa6d6945eb023c23dcb1ac35f6297d20ce17b021c81
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/179cef3077945d40ff96df5835279e16.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161116%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161116T174107Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=3d84a2960652d8f514e4855b6aa03bb8f26fdf290f6fc40aea54ce3dd72c1cec",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f88aae649faff40caa4afa6d6945eb023c23dcb1ac35f6297d20ce17b021c81"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer 08936d4a77373cb26f49d41596f4da976ab50291d87c8f2fdd3bb6871d87fa98
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b52780042426d03e5d1102326e227067.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161116%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161116T174106Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b7fb46361442b13606345416fab776c12541edbdfcd2865af4a0cde7c68ee731",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08936d4a77373cb26f49d41596f4da976ab50291d87c8f2fdd3bb6871d87fa98"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer 86bb2464faf705fb69a099af1a3cdffed46eb7e4d3c29d18b0e945dd790c817d
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
      "id": 478,
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
      "created_at": "2016-11-16T17:41:05.896Z",
      "updated_at": "2016-11-16T17:41:05.896Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-16T17:41:05.971Z",
    "updated_at": "2016-11-16T17:41:05.971Z",
    "course_id": 124,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86bb2464faf705fb69a099af1a3cdffed46eb7e4d3c29d18b0e945dd790c817d"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer afcf4cab4176eb9cdafc0a6b3743c3232d78eb61e9da5812b25886fdcc463350
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
      "creator_id": 278,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 68,
      "additional_university_ids": [

      ],
      "discipline_id": 73,
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
      "chapters_updated_at": "2016-11-16T17:40:48.459Z",
      "updated_at": "2016-11-16T17:40:50.562Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 73,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 283,
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-fa618291-8864-4b31-a1a8-861b344e95af",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-fa618291-8864-4b31-a1a8-861b344e95af",
      "slug": "mit-the-great-british-bake-off-fa618291-8864-4b31-a1a8-861b344e95af",
      "university_id": 69,
      "additional_university_ids": [

      ],
      "discipline_id": 74,
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
      "chapters_updated_at": "2016-11-16T17:40:48.459Z",
      "updated_at": "2016-11-16T17:40:51.110Z",
      "shortname": "mit-the-great-british-bake-off-fa618291-8864-4b31-a1a8-861b344e95af",
      "topic_id": 74,
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
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer afcf4cab4176eb9cdafc0a6b3743c3232d78eb61e9da5812b25886fdcc463350"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/18/download
Content-Type: application/json
Authorization: Bearer d227b76c8f7c00dacf5c8d1949281511b849cf9ef135668f7995519172a22f53
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d227b76c8f7c00dacf5c8d1949281511b849cf9ef135668f7995519172a22f53"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/12/report
Content-Type: application/json
Authorization: Bearer 321418d964b1e9e44bb144f67ce585b1e9e403aef8636dbf04a10d77a51692ce
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
	-H "Authorization: Bearer 321418d964b1e9e44bb144f67ce585b1e9e403aef8636dbf04a10d77a51692ce"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/19/bookmark
Content-Type: application/json
Authorization: Bearer 65f7b29f89b17a2f9bfbabfd62cc38bfb69d41717cb9203d2230a886e733adbf
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65f7b29f89b17a2f9bfbabfd62cc38bfb69d41717cb9203d2230a886e733adbf"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/11/upvote
Content-Type: application/json
Authorization: Bearer bdf950183acb56b0a9d35efae370dea5a34cfcc7358fb17091fbb4b192059735
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdf950183acb56b0a9d35efae370dea5a34cfcc7358fb17091fbb4b192059735"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/18/comments
Content-Type: application/json
Authorization: Bearer 0535c31ca031f055e832c8dfa376b14d4e7c4c08ed70124889a43a239060e614
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
    "author_id": 315,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:40:53.186Z",
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
	-H "Authorization: Bearer 0535c31ca031f055e832c8dfa376b14d4e7c4c08ed70124889a43a239060e614"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/17/comments
Content-Type: application/json
Authorization: Bearer e284dfe58e8c9b51dd94d267d7670e98f7ee14908624bcf5d430db42676a08f5
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
    "author_id": 312,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:40:52.869Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 312,
      "feedbackable_id": 17,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:52.866Z",
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
curl "api.goskive.com/v2/flashcards/17/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e284dfe58e8c9b51dd94d267d7670e98f7ee14908624bcf5d430db42676a08f5"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/15/comments
Content-Type: application/json
Authorization: Bearer b2ce929ca65033b34b8d04150b10d8e74983723a3d2edc0f25e302f1c943bb2b
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
      "author_id": 307,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:40:52.478Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 308,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:40:52.494Z",
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
curl "api.goskive.com/v2/flashcards/15/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2ce929ca65033b34b8d04150b10d8e74983723a3d2edc0f25e302f1c943bb2b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/16/comments
Content-Type: application/json
Authorization: Bearer 3b9a95c52fe1b693945e8bdd59b2b07599d85238d5d05c7982803fdfef8652e0
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
curl "api.goskive.com/v2/flashcards/16/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b9a95c52fe1b693945e8bdd59b2b07599d85238d5d05c7982803fdfef8652e0"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/63/feedbacks
Content-Type: application/json
Authorization: Bearer 568a39effec2458605b49f561ace5ceea764af93b2c7d4e67541c9a126607641
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
    "id": 44,
    "user_id": 737,
    "feedbackable_id": 63,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:41:26.832Z",
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
curl "api.goskive.com/v2/flashcards/63/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 568a39effec2458605b49f561ace5ceea764af93b2c7d4e67541c9a126607641"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/57/feedbacks
Content-Type: application/json
Authorization: Bearer fd30cb3ffce3179329aec6041ffc1249820057291f0e66517b28c2c5b1da5e60
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
      "id": 39,
      "user_id": 711,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:41:25.643Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 38,
      "user_id": 710,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:41:25.631Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd30cb3ffce3179329aec6041ffc1249820057291f0e66517b28c2c5b1da5e60"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/67/votes
Content-Type: application/json
Authorization: Bearer 7c413729d82afce60d902ffb1156ee070c2c67cfdda153bfb85be047fb3ec351
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
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 67,
      "user_id": 763
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 67,
      "user_id": 762
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 67,
      "user_id": 761
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/67/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c413729d82afce60d902ffb1156ee070c2c67cfdda153bfb85be047fb3ec351"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/71/republish
Content-Type: application/json
Authorization: Bearer 86c200f62c40a659e5293c4de2f27e82f3de317d8a651f14003c6ebb3b670106
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
curl "api.goskive.com/v2/flashcards/71/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86c200f62c40a659e5293c4de2f27e82f3de317d8a651f14003c6ebb3b670106"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/88/bookmark
Content-Type: application/json
Authorization: Bearer ee4010b85821665fce32acad4a72b429be054ecd6fea3fbd52aefd2fa16191ef
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/88/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee4010b85821665fce32acad4a72b429be054ecd6fea3fbd52aefd2fa16191ef"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/69
Content-Type: application/json
Authorization: Bearer 576252142a1cfb2f659cd5a42db4d1bcd6f229fbb67dee6ea9fdac15f5d03142
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 576252142a1cfb2f659cd5a42db4d1bcd6f229fbb67dee6ea9fdac15f5d03142"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/89/downvote
Content-Type: application/json
Authorization: Bearer 536d68add061dd7950c157f855d182481d21a81df0c3908be1c757c75ee04e1e
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/89/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 536d68add061dd7950c157f855d182481d21a81df0c3908be1c757c75ee04e1e"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/68
Content-Type: application/json
Authorization: Bearer e4a00b784269505b3ac5221a8b4932a727e39143767ef30f52ec53ffe8f1a7bc
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
    "id": 68,
    "obfuscated_id": "yVS_7NAdP6s",
    "author_id": 834,
    "chapter_id": 154,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:41:36.959Z",
    "created_at": "2016-11-16T17:41:36.959Z",
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
curl "api.goskive.com/v2/flashcards/68" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4a00b784269505b3ac5221a8b4932a727e39143767ef30f52ec53ffe8f1a7bc"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/87/report
Content-Type: application/json
Authorization: Bearer a01969109441af7acb2aa9b1371ab5740f561d0990b521c9190346972f0e047f
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/87/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a01969109441af7acb2aa9b1371ab5740f561d0990b521c9190346972f0e047f"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/91/bookmark
Content-Type: application/json
Authorization: Bearer 9225a1a3081e703e9c073cbf2984d90d9ebf7634e68f9bb8ccff131890fa814f
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/91/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9225a1a3081e703e9c073cbf2984d90d9ebf7634e68f9bb8ccff131890fa814f"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/90/upvote
Content-Type: application/json
Authorization: Bearer ea5bd2efdf94140a301c21c3a78ee02c6ecfd428a412177f3194f70ffc36462a
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/90/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea5bd2efdf94140a301c21c3a78ee02c6ecfd428a412177f3194f70ffc36462a"
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
    "key": "cache/12b2f9f3a31a164521805bbcd10ddd4d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xNlQxODo0MDoyOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzEyYjJmOWYzYTMxYTE2NDUyMTgwNWJiY2QxMGRkZDRkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMTZUMTc0MDI4WiJ9XX0=",
    "x-amz-credential": "FAKE/20161116/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161116T174028Z",
    "x-amz-signature": "95d43b651a8b380a446b310ccfbdae378cb907bf39e8385e6d54208c33fbc8f9"
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
Authorization: Bearer b59e6905b7d42662498966129c2cdd851c0f284ee7c0471ee4218eca203043d6
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
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b59e6905b7d42662498966129c2cdd851c0f284ee7c0471ee4218eca203043d6"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer abcd5b8db45d995233e2a66f8cc1c2a38ee89b92b7b4ca15124dcbca40c24e72
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
	-H "Authorization: Bearer abcd5b8db45d995233e2a66f8cc1c2a38ee89b92b7b4ca15124dcbca40c24e72"
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
{"password":{"reset_password_token":"uE6fyyb3j1o2x32YGZCx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 221,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-16T17:40:39.446Z",
  "updated_at": "2016-11-16T17:40:39.579Z",
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
  "audit_id": 4453
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"uE6fyyb3j1o2x32YGZCx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/126/comments
Content-Type: application/json
Authorization: Bearer bc5a7d67046ea15bdda93e3450e160ecdf31888fe3de088e8134eb17bdca8b25
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
    "id": 55,
    "author_id": 941,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:41:44.841Z",
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
curl "api.goskive.com/v2/questions/126/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc5a7d67046ea15bdda93e3450e160ecdf31888fe3de088e8134eb17bdca8b25"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/125/comments
Content-Type: application/json
Authorization: Bearer 347841e0c6698e1ff8a369325fbeddc13ad1d4512adb87b1df7d7da0f6b157ee
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
    "id": 54,
    "author_id": 938,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:41:44.381Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 938,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:41:44.378Z",
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
curl "api.goskive.com/v2/questions/125/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 347841e0c6698e1ff8a369325fbeddc13ad1d4512adb87b1df7d7da0f6b157ee"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/128/comments
Content-Type: application/json
Authorization: Bearer 67f8cbbc37e0d91ba9c8f43c5e8835b4dd16b02bd3a4f70e8420f92f23d2f6ae
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
      "id": 56,
      "author_id": 950,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:45.588Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 951,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:41:45.604Z",
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
curl "api.goskive.com/v2/questions/128/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67f8cbbc37e0d91ba9c8f43c5e8835b4dd16b02bd3a4f70e8420f92f23d2f6ae"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/124/comments
Content-Type: application/json
Authorization: Bearer 4741fa327a7d2f0a607043656b607bd5cb6887993d0ac18bbdca2e2111aed476
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
curl "api.goskive.com/v2/questions/124/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4741fa327a7d2f0a607043656b607bd5cb6887993d0ac18bbdca2e2111aed476"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/52/feedbacks
Content-Type: application/json
Authorization: Bearer e01af7ebb88416d3d41a9b365fdb2b06bd6d011a98dba375f0dc98c4360a2159
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
    "user_id": 261,
    "feedbackable_id": 52,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:40:42.624Z",
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
curl "api.goskive.com/v2/questions/52/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e01af7ebb88416d3d41a9b365fdb2b06bd6d011a98dba375f0dc98c4360a2159"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/49/feedbacks
Content-Type: application/json
Authorization: Bearer ba1a97c412ae7a760e3420b5147a4c31752e94b403c009bfd2df4095d3c0219f
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
      "user_id": 254,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:41.483Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 253,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:40:41.474Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba1a97c412ae7a760e3420b5147a4c31752e94b403c009bfd2df4095d3c0219f"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/73/votes
Content-Type: application/json
Authorization: Bearer b30c61b22f14a242312ae3c960a99399cfa38ce47e2a2965c2a32713ca2ae65f
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
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 73,
      "user_id": 457
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 73,
      "user_id": 456
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 73,
      "user_id": 455
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/73/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b30c61b22f14a242312ae3c960a99399cfa38ce47e2a2965c2a32713ca2ae65f"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/41/republish
Content-Type: application/json
Authorization: Bearer 0346db3b698566773c4ffe6e285b9990f53750b0e3764f9f8a0550db5a09df40
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
	-H "Authorization: Bearer 0346db3b698566773c4ffe6e285b9990f53750b0e3764f9f8a0550db5a09df40"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/24/bookmark
Content-Type: application/json
Authorization: Bearer 8ab8244d0a098a46d5840a3fde5d3eeb0a43022fb9666b3678b84c788991c0a7
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ab8244d0a098a46d5840a3fde5d3eeb0a43022fb9666b3678b84c788991c0a7"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/40
Content-Type: application/json
Authorization: Bearer 8e63388544b5c08397a2b48fe23d66e6df387f809594d8427c8b78d21c69ab7e
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e63388544b5c08397a2b48fe23d66e6df387f809594d8427c8b78d21c69ab7e"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/22/downvote
Content-Type: application/json
Authorization: Bearer b283d5e9304e9a1178d9bb36fb52130818dc284264e70f61e78f9a99ca2c3341
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b283d5e9304e9a1178d9bb36fb52130818dc284264e70f61e78f9a99ca2c3341"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/23
Content-Type: application/json
Authorization: Bearer c515945f21edede1831ed5c4652cbd8b8b62ad93da7a9087fad0597fd87d8edd
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 146,
    "chapter_id": 32,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:40:30.344Z",
    "created_at": "2016-11-16T17:40:30.217Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 45,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 46,
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
curl "api.goskive.com/v2/questions/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c515945f21edede1831ed5c4652cbd8b8b62ad93da7a9087fad0597fd87d8edd"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/21/report
Content-Type: application/json
Authorization: Bearer 195d632f0ce1cc618e2594cfad16abe13c57ff9c6da590ab8e9175354f106d39
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/21/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 195d632f0ce1cc618e2594cfad16abe13c57ff9c6da590ab8e9175354f106d39"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/20/bookmark
Content-Type: application/json
Authorization: Bearer 9d0f3b4a18a7f14421b5c2bd190dabbf0c9e70dfc5a728787347cfa895bcfb0d
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/20/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d0f3b4a18a7f14421b5c2bd190dabbf0c9e70dfc5a728787347cfa895bcfb0d"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/44
Content-Type: application/json
Authorization: Bearer 71385dbc85cbbff67f395ab42066030dbfcc63263ce73d599308830475e5d80a
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":44,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-16T17:40:37.336Z","updated_at":"2016-11-16T17:40:37.475Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":53,"author_id":214,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 214,
    "chapter_id": 53,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:40:37.591Z",
    "created_at": "2016-11-16T17:40:37.336Z",
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
    "question": "{\"id\"=>44, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-16T17:40:37.336Z\", \"updated_at\"=>\"2016-11-16T17:40:37.475Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>53, \"author_id\"=>214, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 87,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 88,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 89,
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
curl "api.goskive.com/v2/questions/44" -d '{"question":{"question":{"id":44,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-16T17:40:37.336Z","updated_at":"2016-11-16T17:40:37.475Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":53,"author_id":214,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71385dbc85cbbff67f395ab42066030dbfcc63263ce73d599308830475e5d80a"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/43/upvote
Content-Type: application/json
Authorization: Bearer 31f47f86b4105e9080390090edcc3a88202d74a5eded1e19b75c6de95cb95978
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/43/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31f47f86b4105e9080390090edcc3a88202d74a5eded1e19b75c6de95cb95978"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 4713ba3a0ea86e9226742c2fd67afb06cc430fa7635c5afb4e437043e82babae
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
      "creator_id": 777,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 230,
      "additional_university_ids": [

      ],
      "discipline_id": 265,
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
      "updated_at": "2016-11-16T17:41:30.133Z",
      "shortname": "mit-pizza-201",
      "topic_id": 264,
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
	-H "Authorization: Bearer 4713ba3a0ea86e9226742c2fd67afb06cc430fa7635c5afb4e437043e82babae"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 4d200db90a5a652e64e59215ad8aa67821e3bf0493ef7a70b4b1aecc84a041b0
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
      "self_url": "http://api.goskive.test/api/v2/universities/uni-215",
      "html_url": "https://goskive.com/university/uni-215",
      "slug": "uni-215",
      "name": "National School of Pizza",
      "short_name": "Uni 215",
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
      "updated_at": "2016-11-16T17:41:30.444Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-214",
      "html_url": "https://goskive.com/university/uni-214",
      "slug": "uni-214",
      "name": "National School of Pastry",
      "short_name": "Uni 214",
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
      "updated_at": "2016-11-16T17:41:30.427Z",
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
	-H "Authorization: Bearer 4d200db90a5a652e64e59215ad8aa67821e3bf0493ef7a70b4b1aecc84a041b0"
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
      "id": 134,
      "name": "Diverse heuristic open system",
      "name_translations": {
        "en": "Diverse heuristic open system"
      },
      "discipline_id": 135
    },
    {
      "id": 135,
      "name": "Cross-group mission-critical access",
      "name_translations": {
        "en": "Cross-group mission-critical access"
      },
      "discipline_id": 136
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
GET /v2/topics/133
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
    "id": 133,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 134
  }
}
```



```shell
curl "api.goskive.com/v2/topics/133" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 83a43b11288b67ad5fe476f0120668b61ea7dda11fed6e4b7994276f9a270171
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
      "id": 299,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-279",
      "html_url": "https://goskive.com/university/uni-279",
      "slug": "uni-279",
      "name": "University 216",
      "short_name": "Uni 279",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8cd6d5aea41d8eca5ae7113191c5b9aa027055dd.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/31533133387dfc77bdc02710a20396dbbd591d62.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:41:48.320Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 300,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-280",
      "html_url": "https://goskive.com/university/uni-280",
      "slug": "uni-280",
      "name": "University 217",
      "short_name": "Uni 280",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cf19651f1574506778b8c62f64e3b49eca0a135e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b6e01ef93fdf3e17f5a64f6d63b26d4005f6403a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:41:48.337Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 301,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-281",
      "html_url": "https://goskive.com/university/uni-281",
      "slug": "uni-281",
      "name": "University 218",
      "short_name": "Uni 281",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e4a0b3d9dd6021d83aa576889fdefe411a09d75b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a5a1547aab920992ed2134a07dd2804771806ef2.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:41:48.354Z",
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
	-H "Authorization: Bearer 83a43b11288b67ad5fe476f0120668b61ea7dda11fed6e4b7994276f9a270171"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer c010e17e7a1eb7c489ca9ffa0a4ce9f231ab34953330f1a532e95940b3897fce
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
    "id": 298,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0d9da815095a2417b231ea70c76de3b8b6e5d857.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/50a3acdec9bd51db2c333e4b84a022ee1674296e.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-16T17:41:48.261Z",
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
	-H "Authorization: Bearer c010e17e7a1eb7c489ca9ffa0a4ce9f231ab34953330f1a532e95940b3897fce"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 46262beeb855647a7873a0ff7c0b9f02e00f845be64f3a712410931f57163ad1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":170,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 571,
    "id": 158,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 159,
    "additional_university_ids": [

    ],
    "discipline_id": 171,
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
    "chapters_updated_at": "2016-11-16T17:41:17.235Z",
    "updated_at": "2016-11-16T17:41:17.382Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 123,
        "updated_at": "2016-11-16T17:41:17.337Z",
        "course_id": 158,
        "author_id": 571,
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
        "id": 124,
        "updated_at": "2016-11-16T17:41:17.355Z",
        "course_id": 158,
        "author_id": 571,
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
        "id": 125,
        "updated_at": "2016-11-16T17:41:17.372Z",
        "course_id": 158,
        "author_id": 571,
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
    "topic_id": 170,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":170,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46262beeb855647a7873a0ff7c0b9f02e00f845be64f3a712410931f57163ad1"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a1ab4923c093d0d4384f8ce5797cee019089dc34eebdc159d4e93a44f7a2fd7d
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":169,"published":false}}
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
    "creator_id": 570,
    "id": 157,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 158,
    "additional_university_ids": [

    ],
    "discipline_id": 170,
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
    "updated_at": "2016-11-16T17:41:17.161Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 169,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":169,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1ab4923c093d0d4384f8ce5797cee019089dc34eebdc159d4e93a44f7a2fd7d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 72641deaa4638318b85710fe1027900f5a69ebc8e7c3c4bea1403ba0ece4472b
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
      "creator_id": 574,
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 175,
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
      "updated_at": "2016-11-16T17:41:17.830Z",
      "shortname": "fu-course-107",
      "topic_id": 174,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 574,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 176,
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
      "chapters_updated_at": "2016-11-16T17:41:17.687Z",
      "updated_at": "2016-11-16T17:41:18.138Z",
      "shortname": "fu-course-108",
      "topic_id": 175,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72641deaa4638318b85710fe1027900f5a69ebc8e7c3c4bea1403ba0ece4472b"
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
      "creator_id": 584,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-115",
      "html_url": "https://goskive.com/course/fu-course-115",
      "slug": "fu-course-115",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "discipline_id": 183,
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
      "updated_at": "2016-11-16T17:41:18.672Z",
      "shortname": "fu-course-115",
      "topic_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 115",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 584,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-116",
      "html_url": "https://goskive.com/course/fu-course-116",
      "slug": "fu-course-116",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "discipline_id": 184,
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
      "chapters_updated_at": "2016-11-16T17:41:18.528Z",
      "updated_at": "2016-11-16T17:41:18.983Z",
      "shortname": "fu-course-116",
      "topic_id": 183,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 116",
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
Authorization: Bearer 755494da3434a9c51f7d80da914da51bfe0f5af06c18e5b2bd238ee960570b61
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
      "creator_id": 581,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 179,
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
      "updated_at": "2016-11-16T17:41:18.413Z",
      "shortname": "fu-course-111",
      "topic_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 581,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-112",
      "html_url": "https://goskive.com/course/fu-course-112",
      "slug": "fu-course-112",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 180,
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
      "updated_at": "2016-11-16T17:41:18.453Z",
      "shortname": "fu-course-112",
      "topic_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 112",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 755494da3434a9c51f7d80da914da51bfe0f5af06c18e5b2bd238ee960570b61"
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
      "creator_id": 589,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-119",
      "html_url": "https://goskive.com/course/fu-course-119",
      "slug": "fu-course-119",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "discipline_id": 187,
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
      "updated_at": "2016-11-16T17:41:19.162Z",
      "shortname": "fu-course-119",
      "topic_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 119",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 589,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-120",
      "html_url": "https://goskive.com/course/fu-course-120",
      "slug": "fu-course-120",
      "university_id": 165,
      "additional_university_ids": [

      ],
      "discipline_id": 188,
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
      "updated_at": "2016-11-16T17:41:19.202Z",
      "shortname": "fu-course-120",
      "topic_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 120",
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
Authorization: Bearer 64f33ce038423af693a77322960a1b6c6d4ca04f2d11caeb4d2fded67e3ce9da
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
  "id": 920,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-16T17:41:42.007Z",
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
	-H "Authorization: Bearer 64f33ce038423af693a77322960a1b6c6d4ca04f2d11caeb4d2fded67e3ce9da"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/472
Content-Type: application/json
Authorization: Bearer 535cd01b1d0dc29333c9bbc2a347e5e756f9474e761eca4cf400cc0f75f3c9e4
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
    "id": 472,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 124,
    "fields_of_study": [
      131,
      132
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-16T17:41:05.122Z",
    "updated_at": "2016-11-16T17:41:05.122Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/472" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 535cd01b1d0dc29333c9bbc2a347e5e756f9474e761eca4cf400cc0f75f3c9e4"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/470
Content-Type: application/json
Authorization: Bearer 9a85c0723dce1173afafe3c2b29f468326fda533cc000c4fabd84ea6118b751c
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
    "id": 470,
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
    "created_at": "2016-11-16T17:41:04.971Z",
    "updated_at": "2016-11-16T17:41:04.971Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/470" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9a85c0723dce1173afafe3c2b29f468326fda533cc000c4fabd84ea6118b751c"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 8fc934185c4636f2628a26e5d33f223645055e341f96230db486e9a32cbcbd10
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
	-H "Authorization: Bearer 8fc934185c4636f2628a26e5d33f223645055e341f96230db486e9a32cbcbd10"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/14
Content-Type: application/json
Authorization: Bearer dd2c29ac8fa5622678e466ea4ce60bdd6c665cd0dddb723a75745ae686cb50db
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
    "votable_id": 112,
    "user_id": 809
  }
}
```



```shell
curl "api.goskive.com/v2/votes/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd2c29ac8fa5622678e466ea4ce60bdd6c665cd0dddb723a75745ae686cb50db"
```
