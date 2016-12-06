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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"59cc362d7acb54015bf70ad92069874eb917925c404a01c86ba4ce27cb0c7512","client_secret":"4eb6b66a337ccadd6f79a3b8b2563824eda9d2bb8f9fccee33167a64a6ea1412"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"59cc362d7acb54015bf70ad92069874eb917925c404a01c86ba4ce27cb0c7512","client_secret":"4eb6b66a337ccadd6f79a3b8b2563824eda9d2bb8f9fccee33167a64a6ea1412"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NWFhNjY1ZmY2MDk4Y2Y1NWQyZWJiYTNjNmZmNmIzMDExMjVkMWQxNTU4NzA0
NmRjNzg3N2UyMzEwMDZkMTgyMjo3YmI2YWVmMGEwYzY1YzlkYmFkOTJlOGRj
MjFlYmRjMjAzZjRjZTZjYmYyMGZjMWUyZjNjOTdhNDhiYjQxZGY3

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
	-u 5aa665ff6098cf55d2ebba3c6ff6b301125d1d15587046dc7877e231006d1822:7bb6aef0a0c65c9dbad92e8dc21ebdc203f4ce6cbf20fc1e2f3c97a48bb41df7
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a05ea717047bef42705f7977d362dcb1be0a2a2fef88245ddb9d4336c77ea363","client_secret":"a2c32669ed04afa33ac4a2c7c770ca6a451684fc8d306396197a2fbd9d62e2c9"}
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
  "access_token": "e8ee8b6f16ffba4bf9211a1cefc04220e8764eca1583528396ef73e52d243cff",
  "token_type": "bearer",
  "created_at": 1481048279
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a05ea717047bef42705f7977d362dcb1be0a2a2fef88245ddb9d4336c77ea363","client_secret":"a2c32669ed04afa33ac4a2c7c770ca6a451684fc8d306396197a2fbd9d62e2c9"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MmY3MTdmNjgzNWQ4OGE0OTI2NGQ3YzUwMTlkMzY4ZDhhOWM4NjhkNjdjZjhh
ZmVjMDI0MzYzOGViYzFmY2U5ZTozZmU3OTQ3ZTRmNDBlZGFiMjgyYjU5ODY2
NWRlMjI1ZWI4MmRkZWY5MzIxZDJmNmQ3M2VhNzUwOTE3ZjI2MzRm

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
  "access_token": "84b2beb8259fc95839b7978957d74bc872fb8a2b4ed39896ba92c2281c94c975",
  "token_type": "bearer",
  "created_at": 1481048279
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 2f717f6835d88a49264d7c5019d368d8a9c868d67cf8afec0243638ebc1fce9e:3fe7947e4f40edab282b598665de225eb82ddef9321d2f6d73ea750917f2634f
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
{"grant_type":"client_credentials","client_id":"a3bf6fe8a52a51bcf331455867b15a6365f81375c37a0c96e9df68a7d21ff1bc","client_secret":"d13b783f2f71c4051e147c365500e11cde8d0eb62ed504ceae97555bb447334a"}
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
  "access_token": "b3464ff4e4b95930ae67743ed3804079d1e91c2c62f36196c94e501cb154b181",
  "token_type": "bearer",
  "created_at": 1481048279
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"a3bf6fe8a52a51bcf331455867b15a6365f81375c37a0c96e9df68a7d21ff1bc","client_secret":"d13b783f2f71c4051e147c365500e11cde8d0eb62ed504ceae97555bb447334a"}' -X POST \
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
Authorization: Bearer 389716989b717243ecb0d56bf7b89955c2281ef6d737d08de8ee12bf084aa5e6
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
	-H "Authorization: Bearer 389716989b717243ecb0d56bf7b89955c2281ef6d737d08de8ee12bf084aa5e6"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/193/flashcards
Content-Type: application/json
Authorization: Bearer 92ae72c56c5c9a2844980922c9e45b37a2e719d0ad5ea34dfbb11ea96ddd5f79
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
    "author_id": 969,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:17:58.723Z",
    "created_at": "2016-12-06T18:17:58.723Z",
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
	-H "Authorization: Bearer 92ae72c56c5c9a2844980922c9e45b37a2e719d0ad5ea34dfbb11ea96ddd5f79"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/194/flashcards
Content-Type: application/json
Authorization: Bearer 207bd73d332b40813bb746b4ff7430800807e1017c19f89da29af037038289fb
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
      "author_id": 970,
      "chapter_id": 194,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:17:58.984Z",
      "created_at": "2016-12-06T18:17:58.984Z",
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
      "author_id": 970,
      "chapter_id": 194,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:17:59.018Z",
      "created_at": "2016-12-06T18:17:59.018Z",
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
      "author_id": 970,
      "chapter_id": 194,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:17:59.051Z",
      "created_at": "2016-12-06T18:17:59.051Z",
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
	-H "Authorization: Bearer 207bd73d332b40813bb746b4ff7430800807e1017c19f89da29af037038289fb"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/9/questions
Content-Type: application/json
Authorization: Bearer b52e0cd1301bf084c77810f0ba80386215d0041501273aa1255a3f33dff580ca
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":9,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 10,
    "obfuscated_id": "aY5v9ahzH5c",
    "author_id": 33,
    "chapter_id": 9,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:16:44.743Z",
    "created_at": "2016-12-06T18:16:44.743Z",
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
        "id": 20,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 21,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 22,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 23,
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
curl "api.goskive.com/v2/chapters/9/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":9,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b52e0cd1301bf084c77810f0ba80386215d0041501273aa1255a3f33dff580ca"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/6/questions
Content-Type: application/json
Authorization: Bearer a5cedb38c5bffaeab3989de3887551ae9ee7ca038e9594f18d6deca6dfc8811f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 24,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:16:43.150Z",
    "created_at": "2016-12-06T18:16:43.150Z",
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
        "id": 13,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 14,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/6/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5cedb38c5bffaeab3989de3887551ae9ee7ca038e9594f18d6deca6dfc8811f"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/7/questions
Content-Type: application/json
Authorization: Bearer c86389bde6a049779cf3aec8c815fe554fb5d3f5f73bca6a28716061487d6b0c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":7,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 27,
    "chapter_id": 7,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:16:43.693Z",
    "created_at": "2016-12-06T18:16:43.693Z",
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
        "id": 15,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 16,
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
curl "api.goskive.com/v2/chapters/7/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":7,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c86389bde6a049779cf3aec8c815fe554fb5d3f5f73bca6a28716061487d6b0c"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/8/questions
Content-Type: application/json
Authorization: Bearer 14a521f0c78a03cc2012426e70df707ed39744283e9a5c1a67bbb68fbdf8012d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":8,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 9,
    "obfuscated_id": "DMbUb8tMXMw",
    "author_id": 30,
    "chapter_id": 8,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:16:44.222Z",
    "created_at": "2016-12-06T18:16:44.222Z",
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
        "id": 17,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 18,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 19,
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
curl "api.goskive.com/v2/chapters/8/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":8,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14a521f0c78a03cc2012426e70df707ed39744283e9a5c1a67bbb68fbdf8012d"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer 8a6e89b093da04036e3f5d89038fd4edae50aea18115be9c4430e230020c0f0b
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
      "id": 4,
      "obfuscated_id": "SaV_gL1ycAY",
      "author_id": 18,
      "chapter_id": 5,
      "position": 4,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:42.517Z",
      "created_at": "2016-12-06T18:16:42.400Z",
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
          "id": 7,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 8,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 5,
      "obfuscated_id": "iw-7peoPwEU",
      "author_id": 19,
      "chapter_id": 5,
      "position": 5,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:42.703Z",
      "created_at": "2016-12-06T18:16:42.585Z",
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
          "id": 9,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 10,
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
      "author_id": 20,
      "chapter_id": 5,
      "position": 6,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:42.894Z",
      "created_at": "2016-12-06T18:16:42.773Z",
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
          "id": 11,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 12,
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
	-H "Authorization: Bearer 8a6e89b093da04036e3f5d89038fd4edae50aea18115be9c4430e230020c0f0b"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/161
Content-Type: application/json
Authorization: Bearer 278606f042129360f2cc7ed7002d8ed0d22337b929603813c5ae2afb793af3bc
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
curl "api.goskive.com/v2/chapters/161" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 278606f042129360f2cc7ed7002d8ed0d22337b929603813c5ae2afb793af3bc"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/162
Content-Type: application/json
Authorization: Bearer bd694925d89f412abb8e44c2e3ec0fd7886846e6c420024249f818ba65ee0953
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
curl "api.goskive.com/v2/chapters/162" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd694925d89f412abb8e44c2e3ec0fd7886846e6c420024249f818ba65ee0953"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/158
Content-Type: application/json
Authorization: Bearer 38eac50c6679caa5f499915806e00c14eaff16f88e7b0d02c9d7dd8647cbf25f
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
curl "api.goskive.com/v2/chapters/158" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38eac50c6679caa5f499915806e00c14eaff16f88e7b0d02c9d7dd8647cbf25f"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/163
Content-Type: application/json
Authorization: Bearer b6190d1a8723c49f11b8dc90682e9408d24c901f3f2979428690e15610c02824
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/163" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6190d1a8723c49f11b8dc90682e9408d24c901f3f2979428690e15610c02824"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/157
Content-Type: application/json
Authorization: Bearer f5dc47f6d6c776334dd61f840b3023855a0f40fbc5a50932fc0eb2d45f90589a
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
    "id": 157,
    "updated_at": "2016-12-06T18:17:47.149Z",
    "course_id": 258,
    "author_id": 777,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-06T18:17:46.635Z",
    "questions_updated_at": "2016-12-06T18:17:46.635Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 781,
        "chapter_id": 157,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:47.131Z",
        "created_at": "2016-12-06T18:17:47.131Z",
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
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 779,
        "chapter_id": 157,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:47.028Z",
        "created_at": "2016-12-06T18:17:46.912Z",
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
            "id": 229,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 230,
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
curl "api.goskive.com/v2/chapters/157" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5dc47f6d6c776334dd61f840b3023855a0f40fbc5a50932fc0eb2d45f90589a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/159
Content-Type: application/json
Authorization: Bearer 6795a328877abf9085f88e5a995ec891bd50a2e4ab281d7d57d87a825476e0ad
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
    "id": 159,
    "updated_at": "2016-12-06T18:17:47.449Z",
    "course_id": 260,
    "author_id": 787,
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
curl "api.goskive.com/v2/chapters/159" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6795a328877abf9085f88e5a995ec891bd50a2e4ab281d7d57d87a825476e0ad"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer 754efcf35151cd9fd9e66e44e723c89758cbc17299ead0fd840698072a06b78d
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
    "author_id": 43,
    "reply_to_id": 2,
    "created_at": "2016-12-06T18:16:46.074Z",
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
	-H "Authorization: Bearer 754efcf35151cd9fd9e66e44e723c89758cbc17299ead0fd840698072a06b78d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 4d294e35e8c98cd32bfdf08d6cec48619b540e9a7b0bccd2ff45cda76e829c26
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
	-H "Authorization: Bearer 4d294e35e8c98cd32bfdf08d6cec48619b540e9a7b0bccd2ff45cda76e829c26"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/10
Content-Type: application/json
Authorization: Bearer 3b064fc048243bd754c960d1ea2732c3e83a107d0e9298b02f0eb738a4e6022a
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
curl "api.goskive.com/v2/comments/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b064fc048243bd754c960d1ea2732c3e83a107d0e9298b02f0eb738a4e6022a"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/47/republish
Content-Type: application/json
Authorization: Bearer 359cad89cb19d4f1fb9c472bcf0258db61447957cd88de4268e52e1a2aa49941
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
curl "api.goskive.com/v2/comments/47/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 359cad89cb19d4f1fb9c472bcf0258db61447957cd88de4268e52e1a2aa49941"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/9
Content-Type: application/json
Authorization: Bearer c9d2297b2565f999960e83a8ff9422dc6cf8181a78ea64f05337b0c10e12a86d
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c9d2297b2565f999960e83a8ff9422dc6cf8181a78ea64f05337b0c10e12a86d"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/46/report
Content-Type: application/json
Authorization: Bearer 70f171d89cac133f470fa9d8a6df7db2a808739455decc6e40a2e15cd182bb21
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70f171d89cac133f470fa9d8a6df7db2a808739455decc6e40a2e15cd182bb21"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/1
Content-Type: application/json
Authorization: Bearer 8a36a53f25cbace70cba6eb2fe261c56d2dc11c5602b78b28d4d94313ba1d5cd
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
    "updated_at": "2016-12-06T18:17:05.426Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a36a53f25cbace70cba6eb2fe261c56d2dc11c5602b78b28d4d94313ba1d5cd"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 6f97ba57a75196e3e3776224062f5b329f72026d8efdeefd8e9a44a1d9e57916
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
      "updated_at": "2016-12-06T18:17:05.577Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-06T18:17:05.582Z"
    },
    {
      "id": 4,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-06T18:17:05.586Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f97ba57a75196e3e3776224062f5b329f72026d8efdeefd8e9a44a1d9e57916"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer 64c6107715359dc7bb79890ecee71e5cc10a8346a1d8f262ec7b7d0a95113d83
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
curl "api.goskive.com/v2/companies/27/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64c6107715359dc7bb79890ecee71e5cc10a8346a1d8f262ec7b7d0a95113d83"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 1a55e31c1e50f969ed7ce24ccf3bdd108f26b28ef63720e24a706125844e65c4
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
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a55e31c1e50f969ed7ce24ccf3bdd108f26b28ef63720e24a706125844e65c4"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer c65ef9778cba1ccfbf52a462a34b3d7e962bee21f3f10744871dc497358d515b
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
      "company_id": 31,
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
	-H "Authorization: Bearer c65ef9778cba1ccfbf52a462a34b3d7e962bee21f3f10744871dc497358d515b"
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
Authorization: Bearer cfc7825be69412e1bc082b6db391885fc1239183e059e62f69a6b74434eda76a
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
	-H "Authorization: Bearer cfc7825be69412e1bc082b6db391885fc1239183e059e62f69a6b74434eda76a"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f185e5dfafe51e3687bce3c700950454c48b797c823fbbe2a3a300e29c611689
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
    "id": 139,
    "updated_at": "2016-12-06T18:17:39.215Z",
    "course_id": 221,
    "author_id": 648,
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
	-H "Authorization: Bearer f185e5dfafe51e3687bce3c700950454c48b797c823fbbe2a3a300e29c611689"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5509785dd33f98fada3379c5498d2e233f1910d3b676d5cba48b875e8674741c
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
      "updated_at": "2016-12-06T18:17:36.490Z",
      "course_id": 208,
      "author_id": 598,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 108",
      "position": 1
    },
    {
      "id": 118,
      "updated_at": "2016-12-06T18:17:36.512Z",
      "course_id": 208,
      "author_id": 599,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 109",
      "position": 2
    },
    {
      "id": 119,
      "updated_at": "2016-12-06T18:17:36.754Z",
      "course_id": 208,
      "author_id": 600,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-06T18:17:36.419Z",
      "questions_updated_at": "2016-12-06T18:17:36.419Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 110",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5509785dd33f98fada3379c5498d2e233f1910d3b676d5cba48b875e8674741c"
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
      "id": 123,
      "updated_at": "2016-12-06T18:17:37.213Z",
      "course_id": 211,
      "author_id": 612,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 114",
      "position": 1
    },
    {
      "id": 124,
      "updated_at": "2016-12-06T18:17:37.235Z",
      "course_id": 211,
      "author_id": 613,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 115",
      "position": 2
    },
    {
      "id": 125,
      "updated_at": "2016-12-06T18:17:37.476Z",
      "course_id": 211,
      "author_id": 614,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-06T18:17:37.142Z",
      "questions_updated_at": "2016-12-06T18:17:37.142Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 116",
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
Authorization: Bearer b6c1f5aaf88f01445ab282e43b44088ff5e4e0ac6263fd9d237eb5599db7d558
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
      "updated_at": "2016-12-06T18:17:36.922Z",
      "course_id": 209,
      "author_id": 605,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 111",
      "position": 1
    },
    {
      "id": 121,
      "updated_at": "2016-12-06T18:17:36.944Z",
      "course_id": 209,
      "author_id": 606,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 112",
      "position": 2
    },
    {
      "id": 122,
      "updated_at": "2016-12-06T18:17:36.967Z",
      "course_id": 209,
      "author_id": 607,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 113",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6c1f5aaf88f01445ab282e43b44088ff5e4e0ac6263fd9d237eb5599db7d558"
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
      "id": 126,
      "updated_at": "2016-12-06T18:17:37.747Z",
      "course_id": 213,
      "author_id": 619,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 117",
      "position": 1
    },
    {
      "id": 127,
      "updated_at": "2016-12-06T18:17:37.775Z",
      "course_id": 213,
      "author_id": 620,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 118",
      "position": 2
    },
    {
      "id": 128,
      "updated_at": "2016-12-06T18:17:37.799Z",
      "course_id": 213,
      "author_id": 621,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 119",
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
Authorization: Bearer be09b0aa229c036540166b154597ddfce34d7481585511cc57c5157d8edec722
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
    "course_id": 275,
    "user_id": 826,
    "updated_at": "2016-12-06T18:17:49.944Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be09b0aa229c036540166b154597ddfce34d7481585511cc57c5157d8edec722"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7fa90a1ad21cb0fa3157b53e64416b1faabb4ffa119ba1a341bd291f193110bf
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
      "course_id": 271,
      "user_id": 814,
      "updated_at": "2016-12-06T18:17:49.407Z"
    },
    {
      "id": 3,
      "course_id": 271,
      "user_id": 815,
      "updated_at": "2016-12-06T18:17:49.421Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7fa90a1ad21cb0fa3157b53e64416b1faabb4ffa119ba1a341bd291f193110bf"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/235/files
Content-Type: application/json
Authorization: Bearer 120734526e7fe750d9a66cd96e1a1020100c182203e326c95dacdb27beb7f63c
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
      "id": 4,
      "uploader": {
        "id": 700,
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
        "created_at": "2016-12-06T18:17:41.984Z",
        "updated_at": "2016-12-06T18:17:41.984Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-06T18:17:41.994Z",
      "updated_at": "2016-12-06T18:17:41.994Z",
      "course_id": 235,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 701,
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
        "created_at": "2016-12-06T18:17:42.003Z",
        "updated_at": "2016-12-06T18:17:42.003Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-06T18:17:42.012Z",
      "updated_at": "2016-12-06T18:17:42.012Z",
      "course_id": 235,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 702,
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
        "created_at": "2016-12-06T18:17:42.021Z",
        "updated_at": "2016-12-06T18:17:42.021Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-06T18:17:42.029Z",
      "updated_at": "2016-12-06T18:17:42.029Z",
      "course_id": 235,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/235/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 120734526e7fe750d9a66cd96e1a1020100c182203e326c95dacdb27beb7f63c"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/234/files
Content-Type: application/json
Authorization: Bearer 18f0a354a9795d9091934463757b1e053afc4dc9538e60d8158153a992e26ade
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
    "id": 3,
    "uploader": {
      "id": 698,
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
      "created_at": "2016-12-06T18:17:41.800Z",
      "updated_at": "2016-12-06T18:17:41.800Z"
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
    "created_at": "2016-12-06T18:17:41.844Z",
    "updated_at": "2016-12-06T18:17:41.844Z",
    "course_id": 234,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/234/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18f0a354a9795d9091934463757b1e053afc4dc9538e60d8158153a992e26ade"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/233/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer f6d60c69d1938e858e6ebc06c6da83da28aeef9a28bece1717681efe1e904077
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
    "key": "cache/9982aee17e1f52c6ece8064e5e0e2741.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wNlQxOToxNzo0MVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzk5ODJhZWUxN2UxZjUyYzZlY2U4MDY0ZTVlMGUyNzQxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA2VDE4MTc0MVoifV19",
    "x-amz-credential": "FAKE/20161206/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161206T181741Z",
    "x-amz-signature": "b9512b128dfef8e19f6e2b4c6b569f29d87eb3a5778d84abdd8bc6607a38c5ee"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/233/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6d60c69d1938e858e6ebc06c6da83da28aeef9a28bece1717681efe1e904077"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 81275b1d4b735c9e8911352aa4b943d723376a6d230ec63ea4ba5a32b7f4f89c
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
	-H "Authorization: Bearer 81275b1d4b735c9e8911352aa4b943d723376a6d230ec63ea4ba5a32b7f4f89c"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5c9d3810f68d68392d222904a2bf973a131d703486341f5b248b121b509cb34f
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
	-H "Authorization: Bearer 5c9d3810f68d68392d222904a2bf973a131d703486341f5b248b121b509cb34f"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1e9588651e2da8522e2fab6c9c25f659d34cdd4672d165462ff630aaeaa874cf
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
	-H "Authorization: Bearer 1e9588651e2da8522e2fab6c9c25f659d34cdd4672d165462ff630aaeaa874cf"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f3ba34a58c730936dc9835bb467ccf78a0430482fe2d019790df32858a77c2f6
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
	-H "Authorization: Bearer f3ba34a58c730936dc9835bb467ccf78a0430482fe2d019790df32858a77c2f6"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4a1b9b88dec2e84a8ab6cd7baca62a0b9054db93f47f2577cf5debd8f7e91589
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
	-H "Authorization: Bearer 4a1b9b88dec2e84a8ab6cd7baca62a0b9054db93f47f2577cf5debd8f7e91589"
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
    "creator_id": 364,
    "id": 119,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 120,
    "additional_university_ids": [

    ],
    "discipline_id": 126,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 2,
    "questions_count": 2,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-06T18:17:10.217Z",
    "updated_at": "2016-12-06T18:17:11.690Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 364,
        "chapter_id": 71,
        "position": 39,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:10.428Z",
        "created_at": "2016-12-06T18:17:10.308Z",
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
      },
      {
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 364,
        "chapter_id": 72,
        "position": 41,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:10.821Z",
        "created_at": "2016-12-06T18:17:10.697Z",
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
            "id": 111,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 112,
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
        "id": 71,
        "updated_at": "2016-12-06T18:17:11.641Z",
        "course_id": 119,
        "author_id": 364,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-06T18:17:10.217Z",
        "questions_updated_at": "2016-12-06T18:17:10.217Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 65",
        "position": 1
      },
      {
        "id": 72,
        "updated_at": "2016-12-06T18:17:11.682Z",
        "course_id": 119,
        "author_id": 364,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-06T18:17:10.217Z",
        "questions_updated_at": "2016-12-06T18:17:10.217Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 66",
        "position": 2
      }
    ],
    "topic_id": 126,
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
Authorization: Bearer ac67865c665f4f7ce2d7fc3d92dcc578761d8dcc75cb5b5673433d0b9e73c5e7
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
    "creator_id": 369,
    "id": 120,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 121,
    "additional_university_ids": [

    ],
    "discipline_id": 127,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 4,
    "questions_count": 4,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-06T18:17:11.750Z",
    "updated_at": "2016-12-06T18:17:13.258Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 370,
        "chapter_id": 73,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:13.044Z",
        "created_at": "2016-12-06T18:17:13.044Z",
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
        "author_id": 370,
        "chapter_id": 74,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:13.118Z",
        "created_at": "2016-12-06T18:17:13.118Z",
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
        "author_id": 370,
        "chapter_id": 73,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:13.086Z",
        "created_at": "2016-12-06T18:17:13.086Z",
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
        "author_id": 370,
        "chapter_id": 74,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:13.159Z",
        "created_at": "2016-12-06T18:17:13.159Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 370,
        "chapter_id": 73,
        "position": 45,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:11.966Z",
        "created_at": "2016-12-06T18:17:11.846Z",
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
            "id": 119,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 120,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 370,
        "chapter_id": 73,
        "position": 46,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:12.146Z",
        "created_at": "2016-12-06T18:17:12.032Z",
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
            "id": 121,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 122,
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
        "author_id": 370,
        "chapter_id": 74,
        "position": 47,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:12.359Z",
        "created_at": "2016-12-06T18:17:12.231Z",
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
            "id": 123,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 124,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 370,
        "chapter_id": 74,
        "position": 48,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:12.548Z",
        "created_at": "2016-12-06T18:17:12.427Z",
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
            "id": 125,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 126,
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
        "id": 73,
        "updated_at": "2016-12-06T18:17:13.210Z",
        "course_id": 120,
        "author_id": 369,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-06T18:17:11.750Z",
        "questions_updated_at": "2016-12-06T18:17:11.750Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 67",
        "position": 1
      },
      {
        "id": 74,
        "updated_at": "2016-12-06T18:17:13.250Z",
        "course_id": 120,
        "author_id": 369,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-06T18:17:11.750Z",
        "questions_updated_at": "2016-12-06T18:17:11.750Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 68",
        "position": 2
      }
    ],
    "topic_id": 127,
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
	-H "Authorization: Bearer ac67865c665f4f7ce2d7fc3d92dcc578761d8dcc75cb5b5673433d0b9e73c5e7"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/118/pin
Content-Type: application/json
Authorization: Bearer 5ece985d9016be42a247a140fe9eb8b28195aaf2d4d32654bbe079bc1ccd6e77
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/118/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ece985d9016be42a247a140fe9eb8b28195aaf2d4d32654bbe079bc1ccd6e77"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/132/pin
Content-Type: application/json
Authorization: Bearer 3964440d9fbf6e87f70a18a13c858fb9fd946ba2165e0635c3bfa813ca5dbce9
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/132/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3964440d9fbf6e87f70a18a13c858fb9fd946ba2165e0635c3bfa813ca5dbce9"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 447089bc83215c6f47445b9b57c080b3c8271496075cc54edaa164adb35d04c9
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
    "creator_id": 361,
    "id": 117,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 118,
    "additional_university_ids": [

    ],
    "discipline_id": 124,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-06T18:17:10.051Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 124,
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
	-H "Authorization: Bearer 447089bc83215c6f47445b9b57c080b3c8271496075cc54edaa164adb35d04c9"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 24a0524fb92473342dccca7e6bdc0b484eb1f74ed9d2b252c37ae7bb38a8d24d
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
    "id": 344,
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
    "created_at": "2016-12-06T18:17:08.280Z",
    "updated_at": "2016-12-06T18:17:08.280Z",
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
	-H "Authorization: Bearer 24a0524fb92473342dccca7e6bdc0b484eb1f74ed9d2b252c37ae7bb38a8d24d"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c28f08dab34bf74ac3adf2f258bf3fa8ef6ec0778031d60a18cd4e25f5b0f3c4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[115]}
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
    "id": 345,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      115
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-06T18:17:08.381Z",
    "updated_at": "2016-12-06T18:17:08.418Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[115]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c28f08dab34bf74ac3adf2f258bf3fa8ef6ec0778031d60a18cd4e25f5b0f3c4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 04f33aa3fbcb255a1c4c82eaff97b55a2028a4f66fe1011f9b9280c4376f536b
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
    "id": 346,
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
    "created_at": "2016-12-06T18:17:08.442Z",
    "updated_at": "2016-12-06T18:17:08.442Z",
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
	-H "Authorization: Bearer 04f33aa3fbcb255a1c4c82eaff97b55a2028a4f66fe1011f9b9280c4376f536b"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer cdb9861f10bbe9e41a62e11e9ce23eadace5d5d42b463f1b5c0703de51611310
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[117]}
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
    "id": 347,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      117
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-06T18:17:08.534Z",
    "updated_at": "2016-12-06T18:17:08.534Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[117]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdb9861f10bbe9e41a62e11e9ce23eadace5d5d42b463f1b5c0703de51611310"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 708ea4720d18abf0f2a922b498ac7f4150ec92ec3f8c14b5579fb2cd15056ab8
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

119
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
    "id": 349,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/a4b554ef595154b407140198fc4e2cf723b4f83e.jpg",
    "university_id": null,
    "fields_of_study": [
      119
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-06T18:17:08.680Z",
    "updated_at": "2016-12-06T18:17:08.954Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/fb6b62fd7b67e5bf97676eeb5901bdc1a03b569a.jpg",
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

119
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 708ea4720d18abf0f2a922b498ac7f4150ec92ec3f8c14b5579fb2cd15056ab8"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 679723f97664b6a18fb29993fb6550f19379ef88c7ee97f15a409581f348bceb
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
	-H "Authorization: Bearer 679723f97664b6a18fb29993fb6550f19379ef88c7ee97f15a409581f348bceb"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer df1613f0ad6ec0a7b5cbfcc0bbf630b6fa3a47d1eb0b9f3f3f6768d8ed9b4ab6
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
      "company_id": 21,
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 22,
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
	-H "Authorization: Bearer df1613f0ad6ec0a7b5cbfcc0bbf630b6fa3a47d1eb0b9f3f3f6768d8ed9b4ab6"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer f94de5106c9bcaf0e34570239de19a90586a11fb3ae7b97443e40da00dd1bd35
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
      "company_id": 17,
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
	-H "Authorization: Bearer f94de5106c9bcaf0e34570239de19a90586a11fb3ae7b97443e40da00dd1bd35"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 2e4f808b53d48de3bb571de08542820f3b16f55cdb98b31a31585611178e8571
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
      "creator_id": 657,
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-173",
      "html_url": "https://goskive.com/course/mit-course-173",
      "slug": "mit-course-173",
      "university_id": 208,
      "additional_university_ids": [

      ],
      "discipline_id": 233,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:39.802Z",
      "shortname": "mit-course-173",
      "topic_id": 233,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 658,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-174",
      "html_url": "https://goskive.com/course/mit-course-174",
      "slug": "mit-course-174",
      "university_id": 209,
      "additional_university_ids": [

      ],
      "discipline_id": 234,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:39.878Z",
      "shortname": "mit-course-174",
      "topic_id": 234,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 174",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e4f808b53d48de3bb571de08542820f3b16f55cdb98b31a31585611178e8571"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer b9da314e9b739d5333027cc178d9f1e357c9eb41be91e990b0c7ea281cf06d86
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
        "created_at": "2016-12-06T18:17:59.548Z",
        "updated_at": "2016-12-06T18:17:59.548Z",
        "file_url": "memory://d7d87dd6652ec955bb761dd5a3064d01.pdf",
        "course_id": 314,
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
        "created_at": "2016-12-06T18:17:59.623Z",
        "updated_at": "2016-12-06T18:17:59.623Z",
        "file_url": "memory://9821a59b3932e80e23a159bb015a290a.pdf",
        "course_id": 315,
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
        "created_at": "2016-12-06T18:17:59.697Z",
        "updated_at": "2016-12-06T18:17:59.697Z",
        "file_url": "memory://2788728c49363b0629936d3d9fbf361a.pdf",
        "course_id": 316,
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
	-H "Authorization: Bearer b9da314e9b739d5333027cc178d9f1e357c9eb41be91e990b0c7ea281cf06d86"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 0d49ff03b4d383036f6baaf487fa1b41a2324f19d886ca1000162e43dc464ec2
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 12",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-06T18:17:32.853Z"
      },
      "created_at": "2016-12-06T18:17:32.857Z",
      "updated_at": "2016-12-06T18:17:32.857Z",
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 13",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-06T18:17:32.865Z"
      },
      "created_at": "2016-12-06T18:17:32.868Z",
      "updated_at": "2016-12-06T18:17:32.868Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d49ff03b4d383036f6baaf487fa1b41a2324f19d886ca1000162e43dc464ec2"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 18e3b2e6e5dedc8a82f0a1e66b3ad28e0333f9791cc417959186530b30f284eb
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
        "name": "Fake Company Name 8",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-06T18:17:32.610Z"
      },
      "created_at": "2016-12-06T18:17:32.613Z",
      "updated_at": "2016-12-06T18:17:32.613Z",
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
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-06T18:17:32.627Z"
      },
      "created_at": "2016-12-06T18:17:32.631Z",
      "updated_at": "2016-12-06T18:17:32.631Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18e3b2e6e5dedc8a82f0a1e66b3ad28e0333f9791cc417959186530b30f284eb"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 455b2d7eb3c83c567c9ec26db8be38c7a7926bbf80416121f0355a8f38b1e5f1
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
      "id": 12,
      "created_at": "2016-12-06T18:17:21.388Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 49,
      "updated_at": "2016-12-06T18:17:21.501Z",
      "author_id": "443",
      "thread_subject_id": "143",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 13,
      "created_at": "2016-12-06T18:17:21.490Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 50,
      "updated_at": "2016-12-06T18:17:21.505Z",
      "author_id": "446",
      "thread_subject_id": "144",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-12-06T18:17:21.920Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-12-06T18:17:21.920Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 15,
      "created_at": "2016-12-06T18:17:22.319Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-12-06T18:17:22.319Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 16,
      "created_at": "2016-12-06T18:17:22.693Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-12-06T18:17:22.693Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 17,
      "created_at": "2016-12-06T18:17:22.984Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 84,
      "updated_at": "2016-12-06T18:17:22.984Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-12-06T18:17:23.289Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 85,
      "updated_at": "2016-12-06T18:17:23.289Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 19,
      "created_at": "2016-12-06T18:17:23.584Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 86,
      "updated_at": "2016-12-06T18:17:23.584Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 455b2d7eb3c83c567c9ec26db8be38c7a7926bbf80416121f0355a8f38b1e5f1"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/20
Content-Type: application/json
Authorization: Bearer 1b45901644494b37808da2c5c515265ac66ce35227502d5403ce90ea3d0c37c1
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-06T18:07:23.000Z"}}
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
    "id": 20,
    "created_at": "2016-12-06T18:17:23.771Z",
    "read_at": "2016-12-06T18:07:23.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 51,
    "updated_at": "2016-12-06T18:17:23.809Z",
    "author_id": "472",
    "thread_subject_id": "151",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/20" -d '{"notification":{"read_at":"2016-12-06T18:07:23.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b45901644494b37808da2c5c515265ac66ce35227502d5403ce90ea3d0c37c1"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 34086fce37320edd4648ad585cea56915f6084729308367d59ca253aedf66213
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
      "course_id": 280,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-06T18:17:50.487Z",
      "course_published": true,
      "updated_at": "2016-12-06T18:17:50.480Z"
    },
    {
      "id": 8,
      "course_id": 281,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-06T18:17:50.561Z",
      "course_published": true,
      "updated_at": "2016-12-06T18:17:50.554Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34086fce37320edd4648ad585cea56915f6084729308367d59ca253aedf66213"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer a66c89533e254795d1a7ae89ec057432db2721b61320049215f956680f670077
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
    "course_id": 276,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-06T18:17:50.030Z",
    "course_published": true,
    "updated_at": "2016-12-06T18:17:50.023Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a66c89533e254795d1a7ae89ec057432db2721b61320049215f956680f670077"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 8a7acd716868f24e49e914cc927f12b2e6a14870195f7c20ce7922410466808f
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
    "course_id": 279,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-06T18:17:50.398Z",
    "course_published": true,
    "updated_at": "2016-12-06T18:17:50.388Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a7acd716868f24e49e914cc927f12b2e6a14870195f7c20ce7922410466808f"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 7461c3583a7a3c2e611e1054fcfcce30386032457a9b22aa769599542fa482ec
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
      "votable_id": 95,
      "user_id": 510
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 96,
      "user_id": 510
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 97,
      "user_id": 510
    },
    {
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 98,
      "user_id": 510
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7461c3583a7a3c2e611e1054fcfcce30386032457a9b22aa769599542fa482ec"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/253
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
    "id": 253,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 253,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 253
      },
      {
        "id": 254,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 253
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/253" -X GET \
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
      "id": 254,
      "name": "Expanded global open architecture",
      "name_translations": {
        "en": "Expanded global open architecture"
      }
    },
    {
      "id": 255,
      "name": "Exclusive context-sensitive throughput",
      "name_translations": {
        "en": "Exclusive context-sensitive throughput"
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
Authorization: Bearer 406c533081858fad9ec114b93eeebf3caab375161ed90906d1f88d9d1d17d1a2
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
    "user_id": 879,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-06T18:17:52.478Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 406c533081858fad9ec114b93eeebf3caab375161ed90906d1f88d9d1d17d1a2"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer 1c50ea26d197b1cda1964d4b0cdcb81ba790aee893e39df68a6306e561d831ab
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
    "id": 21,
    "user_id": 852,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-06T18:17:51.317Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c50ea26d197b1cda1964d4b0cdcb81ba790aee893e39df68a6306e561d831ab"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/23
Content-Type: application/json
Authorization: Bearer c92a1dce0975a180831dc025ffad7fc0e87e6413d82cfa47bb55f0728cae896d
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
    "user_id": 862,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-06T18:17:51.870Z",
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
	-H "Authorization: Bearer c92a1dce0975a180831dc025ffad7fc0e87e6413d82cfa47bb55f0728cae896d"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/fix
Content-Type: application/json
Authorization: Bearer b92176a8a5bb5942d4be0236aa30b594012f9c971d6fcd7143a6f5a217404119
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
curl "api.goskive.com/v2/feedbacks/19/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b92176a8a5bb5942d4be0236aa30b594012f9c971d6fcd7143a6f5a217404119"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer d81283d3a532f78fbe9b13ba6f1deb929c8efc06ff892f40e707e8436daeb722
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
	-H "Authorization: Bearer d81283d3a532f78fbe9b13ba6f1deb929c8efc06ff892f40e707e8436daeb722"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/close
Content-Type: application/json
Authorization: Bearer f6eb0c9bbbcea239f4a1a9dc631f5ec95a87961abdc49c20c09dd3fa1c88b78e
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
	-H "Authorization: Bearer f6eb0c9bbbcea239f4a1a9dc631f5ec95a87961abdc49c20c09dd3fa1c88b78e"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/24
Content-Type: application/json
Authorization: Bearer dd174738ee362c9dd0abc109d0172d60191c28176845abed89ea6e18fea4ca8d
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
    "user_id": 867,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-06T18:17:52.131Z",
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
	-H "Authorization: Bearer dd174738ee362c9dd0abc109d0172d60191c28176845abed89ea6e18fea4ca8d"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer a9cd49f1ae87c040f64945bf39ee8c957273b7aaf34705551828ff062993706b
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
curl "api.goskive.com/v2/files/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9cd49f1ae87c040f64945bf39ee8c957273b7aaf34705551828ff062993706b"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/8/bookmark
Content-Type: application/json
Authorization: Bearer 5c03e2a0bc300b1f8f636fd67e48c87509731b4d5271ff57798b699a4cf86e77
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c03e2a0bc300b1f8f636fd67e48c87509731b4d5271ff57798b699a4cf86e77"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer a32c9f48981ac33ed197de13b36cba914fee4334efc570227bac9c9fe31879f1
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a32c9f48981ac33ed197de13b36cba914fee4334efc570227bac9c9fe31879f1"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/12
Content-Type: application/json
Authorization: Bearer c3f9c00281e7b5e98e2daf301d01b06d5ac3df48f0e007a0a75b136466ef36bc
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/85ed40bb6063a541c14c70c78486ca70.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161206%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161206T181744Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2eabdd9d594c0cb3f2a4031682a3448a0afeaef082cd7742076148861fd461ad",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3f9c00281e7b5e98e2daf301d01b06d5ac3df48f0e007a0a75b136466ef36bc"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/19/preview
Content-Type: application/json
Authorization: Bearer 2117471be40ad2231f6abd0c82a387dbe4d80aa572f90cffc6f21ff7c7f3c54f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/1730bb510619e644227d0904c85e97aa.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161206%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161206T181745Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7a5fb2a3bf5855b50d050b91591fa1a2017cc1347c4caef89e7b75c3e4a30cda",
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
	-H "Authorization: Bearer 2117471be40ad2231f6abd0c82a387dbe4d80aa572f90cffc6f21ff7c7f3c54f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer a461c2f8f0ee13d1fd74908862fb62de4f8589f732c644ccdca35732eaae5f5f
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
      "id": 737,
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
      "created_at": "2016-12-06T18:17:44.084Z",
      "updated_at": "2016-12-06T18:17:44.084Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-06T18:17:44.152Z",
    "updated_at": "2016-12-06T18:17:44.152Z",
    "course_id": 247,
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
	-H "Authorization: Bearer a461c2f8f0ee13d1fd74908862fb62de4f8589f732c644ccdca35732eaae5f5f"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer d174d0efca6b9611b05a94186c3b92f5818b59b89cd3a94f33c40265be74fb81
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
      "creator_id": 328,
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 110,
      "additional_university_ids": [

      ],
      "discipline_id": 111,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-06T18:17:05.640Z",
      "updated_at": "2016-12-06T18:17:07.278Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 111,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 333,
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-38ccb264-48f3-4e92-9488-cba181d2eb58",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-38ccb264-48f3-4e92-9488-cba181d2eb58",
      "slug": "mit-the-great-british-bake-off-38ccb264-48f3-4e92-9488-cba181d2eb58",
      "university_id": 111,
      "additional_university_ids": [

      ],
      "discipline_id": 112,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-06T18:17:05.640Z",
      "updated_at": "2016-12-06T18:17:07.847Z",
      "shortname": "mit-the-great-british-bake-off-38ccb264-48f3-4e92-9488-cba181d2eb58",
      "topic_id": 112,
      "language_code": "de",
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
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer d174d0efca6b9611b05a94186c3b92f5818b59b89cd3a94f33c40265be74fb81"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/13/download
Content-Type: application/json
Authorization: Bearer 6ad78d556237840f59cc77996bd7347866f162bc8b4ea03fb9b4e5cd0634e51f
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ad78d556237840f59cc77996bd7347866f162bc8b4ea03fb9b4e5cd0634e51f"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/14/report
Content-Type: application/json
Authorization: Bearer d57641c93df9c7cf8d6daea0984b533fe94840d2f7f987290380374f433dca60
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d57641c93df9c7cf8d6daea0984b533fe94840d2f7f987290380374f433dca60"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/15/bookmark
Content-Type: application/json
Authorization: Bearer d89dbbb1c1da1f12a6cf8fc182632cc52e9b797e58a8895de94343a0280b99b5
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d89dbbb1c1da1f12a6cf8fc182632cc52e9b797e58a8895de94343a0280b99b5"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/7/upvote
Content-Type: application/json
Authorization: Bearer 2cd070ed33ade0837268e7a62adfb3f86f856367b7960fa7e86ccc3facc18b5e
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cd070ed33ade0837268e7a62adfb3f86f856367b7960fa7e86ccc3facc18b5e"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/75/comments
Content-Type: application/json
Authorization: Bearer c51de64e56e32a4ff9e9cb26325fb86b3208277d104d4abb4105c216b9536bd9
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
    "id": 57,
    "author_id": 712,
    "reply_to_id": null,
    "created_at": "2016-12-06T18:17:42.815Z",
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
curl "api.goskive.com/v2/flashcards/75/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c51de64e56e32a4ff9e9cb26325fb86b3208277d104d4abb4105c216b9536bd9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/73/comments
Content-Type: application/json
Authorization: Bearer 5b97e8ab12341dc880e42f34b26f5d247beba5db86bcc4d8d7f539560dbd797a
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
    "id": 56,
    "author_id": 706,
    "reply_to_id": null,
    "created_at": "2016-12-06T18:17:42.335Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 18,
      "user_id": 706,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:42.333Z",
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
curl "api.goskive.com/v2/flashcards/73/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b97e8ab12341dc880e42f34b26f5d247beba5db86bcc4d8d7f539560dbd797a"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/77/comments
Content-Type: application/json
Authorization: Bearer 47d398d8ba5bdba009327f909cde6ca717f85bdd7c1a015fb9f4a3b6697a33a6
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
      "id": 58,
      "author_id": 721,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:17:43.240Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 722,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:17:43.255Z",
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
curl "api.goskive.com/v2/flashcards/77/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47d398d8ba5bdba009327f909cde6ca717f85bdd7c1a015fb9f4a3b6697a33a6"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/74/comments
Content-Type: application/json
Authorization: Bearer 576c29994d6b1d22b725f0e5fc7633d16c6ea2125c2592b7cd242a160cffb115
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
curl "api.goskive.com/v2/flashcards/74/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 576c29994d6b1d22b725f0e5fc7633d16c6ea2125c2592b7cd242a160cffb115"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/71/feedbacks
Content-Type: application/json
Authorization: Bearer c57cd59790c72fbe8b43edf3ebdf6f4e71ea8e264107c0e639b1deafe5fcf356
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
    "id": 16,
    "user_id": 689,
    "feedbackable_id": 71,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-06T18:17:41.203Z",
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
curl "api.goskive.com/v2/flashcards/71/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c57cd59790c72fbe8b43edf3ebdf6f4e71ea8e264107c0e639b1deafe5fcf356"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/68/feedbacks
Content-Type: application/json
Authorization: Bearer b694f68615697088ccc787743a55600b0ffd62058088f0540f49bef47b098dc4
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
      "id": 13,
      "user_id": 674,
      "feedbackable_id": 68,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:40.628Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 673,
      "feedbackable_id": 68,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:40.617Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/68/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b694f68615697088ccc787743a55600b0ffd62058088f0540f49bef47b098dc4"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/56/votes
Content-Type: application/json
Authorization: Bearer a0734b4abdcf5566c087e5dd7385b3674161ca26bc0e04c71effb344c776769d
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
      "votable_id": 56,
      "user_id": 432
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 431
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 430
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0734b4abdcf5566c087e5dd7385b3674161ca26bc0e04c71effb344c776769d"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/2/republish
Content-Type: application/json
Authorization: Bearer c53ae5535d3d54d1685e03e4b417f64b1a3a451d260e19073f4465b2f206cd6a
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
	-H "Authorization: Bearer c53ae5535d3d54d1685e03e4b417f64b1a3a451d260e19073f4465b2f206cd6a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/bookmark
Content-Type: application/json
Authorization: Bearer 9690a7a57fe19db712ee2aa14f62da4f70b7ecc331ada382ab4d7c69ba714971
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9690a7a57fe19db712ee2aa14f62da4f70b7ecc331ada382ab4d7c69ba714971"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/24
Content-Type: application/json
Authorization: Bearer 1b01f4bb1697e248b3108e11f9d05defce3ff5472f59a56ec0184f0ceb8ddb8b
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
	-H "Authorization: Bearer 1b01f4bb1697e248b3108e11f9d05defce3ff5472f59a56ec0184f0ceb8ddb8b"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/downvote
Content-Type: application/json
Authorization: Bearer 14598759b376b69ae3c1a87e89e5e3b5fd19d193d9f290672ec62a980fc71918
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14598759b376b69ae3c1a87e89e5e3b5fd19d193d9f290672ec62a980fc71918"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/22
Content-Type: application/json
Authorization: Bearer 2267c3bea18b2b05e4419d89f4b63c7f699d5be555a10e6918f6499dac706d9d
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
    "id": 22,
    "obfuscated_id": "V2ZFfduV4jE",
    "author_id": 222,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:16:56.056Z",
    "created_at": "2016-12-06T18:16:56.056Z",
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
curl "api.goskive.com/v2/flashcards/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2267c3bea18b2b05e4419d89f4b63c7f699d5be555a10e6918f6499dac706d9d"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/4/report
Content-Type: application/json
Authorization: Bearer 5827129d45b70b6e942f37dfe261f27e3f3cca5509a09a8e5da6d8c9fd2d4dc0
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/4/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5827129d45b70b6e942f37dfe261f27e3f3cca5509a09a8e5da6d8c9fd2d4dc0"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/20/bookmark
Content-Type: application/json
Authorization: Bearer 85f5d08cdd8c3c289b3f4d08a3743077ab7a43d0faaf511ec7bf848f07b9ea1a
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
	-H "Authorization: Bearer 85f5d08cdd8c3c289b3f4d08a3743077ab7a43d0faaf511ec7bf848f07b9ea1a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/1/upvote
Content-Type: application/json
Authorization: Bearer 1bc5bf95751b6220e8bcf404ec2b18eb1b35bfd750af6c11b80f63d4229c012d
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/1/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bc5bf95751b6220e8bcf404ec2b18eb1b35bfd750af6c11b80f63d4229c012d"
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
    "key": "cache/c9c8589f96db330d2ee007c13404ce4d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wNlQxOToxNzo1OVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2M5Yzg1ODlmOTZkYjMzMGQyZWUwMDdjMTM0MDRjZTRkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDZUMTgxNzU5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161206/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161206T181759Z",
    "x-amz-signature": "4d6eb1580aea9f9bb779066597e8bb3bf3a8d0d109ade9e6bf3a46ea3e640997"
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
Authorization: Bearer 5902074b4f47b6686155d15590a26fb33037a1659077d4ec5e3a48ae03ef2e17
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
	-H "Authorization: Bearer 5902074b4f47b6686155d15590a26fb33037a1659077d4ec5e3a48ae03ef2e17"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer ee30ccff3c4dec92edf38b46f171bb758522ec96045671321bcbca661418dbce
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
	-H "Authorization: Bearer ee30ccff3c4dec92edf38b46f171bb758522ec96045671321bcbca661418dbce"
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
{"password":{"reset_password_token":"Rf4T1TjEa3DTQhZpcafg","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 574,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-12-06T18:17:33.408Z",
  "updated_at": "2016-12-06T18:17:33.607Z",
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
  "audit_id": 8282
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"Rf4T1TjEa3DTQhZpcafg","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/17/comments
Content-Type: application/json
Authorization: Bearer c2e00856728a3317034c09cec663a373e44786301e40951d48cdc79150557acd
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
    "id": 7,
    "author_id": 58,
    "reply_to_id": null,
    "created_at": "2016-12-06T18:16:48.531Z",
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
curl "api.goskive.com/v2/questions/17/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2e00856728a3317034c09cec663a373e44786301e40951d48cdc79150557acd"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/15/comments
Content-Type: application/json
Authorization: Bearer 2ca9a048eac797a61c627c35535495130b12560a2ab042f561398df684c1fca8
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
    "id": 6,
    "author_id": 52,
    "reply_to_id": null,
    "created_at": "2016-12-06T18:16:47.677Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 52,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:16:47.672Z",
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
curl "api.goskive.com/v2/questions/15/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ca9a048eac797a61c627c35535495130b12560a2ab042f561398df684c1fca8"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/14/comments
Content-Type: application/json
Authorization: Bearer ab0705693e4bbc92bbc132db2c7f02af7beb78e8024bf66f25fdb826cb304abd
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
      "id": 4,
      "author_id": 50,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:47.266Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 51,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:47.283Z",
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
curl "api.goskive.com/v2/questions/14/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab0705693e4bbc92bbc132db2c7f02af7beb78e8024bf66f25fdb826cb304abd"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/16/comments
Content-Type: application/json
Authorization: Bearer e0399b5f46c67969dd5d1e06465b6d4b63944e192680cbb62785e49042e557a1
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
curl "api.goskive.com/v2/questions/16/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0399b5f46c67969dd5d1e06465b6d4b63944e192680cbb62785e49042e557a1"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/93/feedbacks
Content-Type: application/json
Authorization: Bearer ec8f0778e0444c8d9f14ea60c86b1702d850e4d78a8a5cc8e0863529779defba
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
    "user_id": 504,
    "feedbackable_id": 93,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-06T18:17:26.170Z",
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
curl "api.goskive.com/v2/questions/93/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec8f0778e0444c8d9f14ea60c86b1702d850e4d78a8a5cc8e0863529779defba"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/92/feedbacks
Content-Type: application/json
Authorization: Bearer 81294a90644a74bf4ab6d32e20002245cb09d8fa772b66a83fcbafa3b1eb5771
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
      "id": 7,
      "user_id": 503,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:25.818Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 502,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:25.806Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/92/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81294a90644a74bf4ab6d32e20002245cb09d8fa772b66a83fcbafa3b1eb5771"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/3/votes
Content-Type: application/json
Authorization: Bearer c8649c639dd0958de01d42a2dda7aa1785ede772038de8dd9ffac0c600ab358f
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
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 3,
      "user_id": 12
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 3,
      "user_id": 11
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 3,
      "user_id": 10
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/3/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8649c639dd0958de01d42a2dda7aa1785ede772038de8dd9ffac0c600ab358f"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/39/republish
Content-Type: application/json
Authorization: Bearer 5f15692a0e35a96c13efaebe08fc6a777ec3cb4a4185336e6e734e229bd3c010
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
curl "api.goskive.com/v2/questions/39/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f15692a0e35a96c13efaebe08fc6a777ec3cb4a4185336e6e734e229bd3c010"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/41/bookmark
Content-Type: application/json
Authorization: Bearer 85dd4a1b1c93408263a5067f7ebdf0f548842c18c7bdce7ed84411eaa8d3f009
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/41/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85dd4a1b1c93408263a5067f7ebdf0f548842c18c7bdce7ed84411eaa8d3f009"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/34
Content-Type: application/json
Authorization: Bearer 547068c3742b0b86d8a3ff93a6433180b4aaffd1a9b98895f706ca3e829486c0
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 547068c3742b0b86d8a3ff93a6433180b4aaffd1a9b98895f706ca3e829486c0"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/37/downvote
Content-Type: application/json
Authorization: Bearer d6d59acba5f4d834ffa6847c9682bc4b45401ab68a93327112e598f185ec5bd4
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/37/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6d59acba5f4d834ffa6847c9682bc4b45401ab68a93327112e598f185ec5bd4"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/38
Content-Type: application/json
Authorization: Bearer ed98e06122f34bc573fededa9b006bf617aea2a509a919752b9bb3d2d46e7b1a
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
    "id": 38,
    "obfuscated_id": "8_YCqPYFnsI",
    "author_id": 296,
    "chapter_id": 61,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:17:03.524Z",
    "created_at": "2016-12-06T18:17:03.404Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed98e06122f34bc573fededa9b006bf617aea2a509a919752b9bb3d2d46e7b1a"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/42/report
Content-Type: application/json
Authorization: Bearer a102ca2aa72b6cfd979fbd9d568b090a1f0e8811c0f3e8987dc0065565da154c
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a102ca2aa72b6cfd979fbd9d568b090a1f0e8811c0f3e8987dc0065565da154c"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/35/bookmark
Content-Type: application/json
Authorization: Bearer d118fe75740b0bed79b219fe2b2da7bdb679000387d080311374b72d2b77cf86
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/35/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d118fe75740b0bed79b219fe2b2da7bdb679000387d080311374b72d2b77cf86"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/33
Content-Type: application/json
Authorization: Bearer 95c7959b5707d4d095b1895aab62d38dae7168bc0f198d4f4603dad1a014bf62
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":33,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-06T18:17:01.146Z","updated_at":"2016-12-06T18:17:01.266Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":56,"author_id":281,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 33,
    "obfuscated_id": "sjAD-GXxS8o",
    "author_id": 281,
    "chapter_id": 56,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-06T18:17:01.392Z",
    "created_at": "2016-12-06T18:17:01.146Z",
    "tags": [
      {
        "id": 2,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 1,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>33, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-12-06T18:17:01.146Z\", \"updated_at\"=>\"2016-12-06T18:17:01.266Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>56, \"author_id\"=>281, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 70,
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
curl "api.goskive.com/v2/questions/33" -d '{"question":{"question":{"id":33,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-06T18:17:01.146Z","updated_at":"2016-12-06T18:17:01.266Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":56,"author_id":281,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95c7959b5707d4d095b1895aab62d38dae7168bc0f198d4f4603dad1a014bf62"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/36/upvote
Content-Type: application/json
Authorization: Bearer 496260afc6ae6166d449a9ea7c50dab30b22a45a5306cceb19ceddc38b0a7504
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/36/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 496260afc6ae6166d449a9ea7c50dab30b22a45a5306cceb19ceddc38b0a7504"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7d8bd8f7d9a3cf63e7f8ebe52fc39cefb6f816ca0cc1d3cc7481771446e0cdfa
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
      "creator_id": 436,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 140,
      "additional_university_ids": [

      ],
      "discipline_id": 150,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:20.913Z",
      "shortname": "mit-pizza-201",
      "topic_id": 150,
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
	-H "Authorization: Bearer 7d8bd8f7d9a3cf63e7f8ebe52fc39cefb6f816ca0cc1d3cc7481771446e0cdfa"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 6a3a10c9515769c83fcf071a82cf876bf59a2a9936a77ec488492982b0fd9f4f
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
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-143",
      "html_url": "https://goskive.com/university/uni-143",
      "slug": "uni-143",
      "name": "National School of Pizza",
      "short_name": "Uni 143",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a58445f18da323c32d6a01ee13edfd8e910335cc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2fe7ca1fa741826191cad0989815045dbd19a0b6.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-06T18:17:21.163Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-142",
      "html_url": "https://goskive.com/university/uni-142",
      "slug": "uni-142",
      "name": "National School of Pastry",
      "short_name": "Uni 142",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4e8c460abbec499dd99d478cc172f1e311637150.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cd0031c8786d89a75fa1088367b50eae39532c27.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-06T18:17:21.146Z",
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
	-H "Authorization: Bearer 6a3a10c9515769c83fcf071a82cf876bf59a2a9936a77ec488492982b0fd9f4f"
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
      "id": 144,
      "name": "Ameliorated national support",
      "name_translations": {
        "en": "Ameliorated national support"
      },
      "discipline_id": 144
    },
    {
      "id": 145,
      "name": "Integrated regional benchmark",
      "name_translations": {
        "en": "Integrated regional benchmark"
      },
      "discipline_id": 145
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
GET /v2/topics/143
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
    "id": 143,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 143
  }
}
```



```shell
curl "api.goskive.com/v2/topics/143" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer a0cb86b3bf77fe8c0fc88040ea95744a664e45a261aa93e49fe28b809df77ab6
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
      "id": 205,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-185",
      "html_url": "https://goskive.com/university/uni-185",
      "slug": "uni-185",
      "name": "University 144",
      "short_name": "Uni 185",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/251a3379388b624d381a43405118f30764fe4f9f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7ed7b255515aee55da5cb2e74b72737d8381795f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-06T18:17:39.585Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 206,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-186",
      "html_url": "https://goskive.com/university/uni-186",
      "slug": "uni-186",
      "name": "University 145",
      "short_name": "Uni 186",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a36fbc0bd48ae8bee6e678b93910414091dbd802.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8515796eb7ecb81973d9773a1c1704993f65c185.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-06T18:17:39.602Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-187",
      "html_url": "https://goskive.com/university/uni-187",
      "slug": "uni-187",
      "name": "University 146",
      "short_name": "Uni 187",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d49d24f5d0070561e7d4979d39ae424d6987e402.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/5e31fbf583340c7e443c78afcb4da7e62af53ad7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-06T18:17:39.619Z",
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
	-H "Authorization: Bearer a0cb86b3bf77fe8c0fc88040ea95744a664e45a261aa93e49fe28b809df77ab6"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 320c6e488c8bc1b599e202bbc309782e4b38cc1dc27387cb1c93cf965d7dca2d
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
    "id": 203,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0787bd81d62837873bedc17bd0d5aeee4e9334b9.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ff1205fa3f7bcacb835982cda574c9a4b422b51f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-06T18:17:39.406Z",
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
	-H "Authorization: Bearer 320c6e488c8bc1b599e202bbc309782e4b38cc1dc27387cb1c93cf965d7dca2d"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a1cfd528ad51406009f447f63b6722398b5229668c4abf6f47027e8da178048c
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":176,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 526,
    "id": 166,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 168,
    "additional_university_ids": [

    ],
    "discipline_id": 176,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 3,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-06T18:17:28.623Z",
    "updated_at": "2016-12-06T18:17:28.766Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 107,
        "updated_at": "2016-12-06T18:17:28.720Z",
        "course_id": 166,
        "author_id": 526,
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
        "id": 108,
        "updated_at": "2016-12-06T18:17:28.738Z",
        "course_id": 166,
        "author_id": 526,
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
        "id": 109,
        "updated_at": "2016-12-06T18:17:28.756Z",
        "course_id": 166,
        "author_id": 526,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":176,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1cfd528ad51406009f447f63b6722398b5229668c4abf6f47027e8da178048c"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer dee3db9b18cb1a77c1b355fb7ca7fd5c0fbfde2ab1fa70ea66a66feadd02861e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":175,"published":false}}
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
    "creator_id": 525,
    "id": 165,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 167,
    "additional_university_ids": [

    ],
    "discipline_id": 175,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-06T18:17:28.588Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":175,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dee3db9b18cb1a77c1b355fb7ca7fd5c0fbfde2ab1fa70ea66a66feadd02861e"
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
      "creator_id": 553,
      "id": 190,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-155",
      "html_url": "https://goskive.com/course/fu-course-155",
      "slug": "fu-course-155",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "discipline_id": 200,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:31.178Z",
      "shortname": "fu-course-155",
      "topic_id": 200,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 553,
      "id": 191,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "discipline_id": 201,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-06T18:17:31.032Z",
      "updated_at": "2016-12-06T18:17:31.472Z",
      "shortname": "fu-course-156",
      "topic_id": 201,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 156",
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
Authorization: Bearer 84f2cb81ac396babdd694f01d219b1cb18b217475ca661e6274d5daa6b7ed93a
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
      "creator_id": 560,
      "id": 198,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 181,
      "additional_university_ids": [

      ],
      "discipline_id": 208,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:31.885Z",
      "shortname": "fu-course-163",
      "topic_id": 208,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 560,
      "id": 199,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-164",
      "html_url": "https://goskive.com/course/fu-course-164",
      "slug": "fu-course-164",
      "university_id": 181,
      "additional_university_ids": [

      ],
      "discipline_id": 209,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-06T18:17:31.745Z",
      "updated_at": "2016-12-06T18:17:32.187Z",
      "shortname": "fu-course-164",
      "topic_id": 209,
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
	-H "Authorization: Bearer 84f2cb81ac396babdd694f01d219b1cb18b217475ca661e6274d5daa6b7ed93a"
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
      "creator_id": 558,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-159",
      "html_url": "https://goskive.com/course/fu-course-159",
      "slug": "fu-course-159",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 204,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:31.672Z",
      "shortname": "fu-course-159",
      "topic_id": 204,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 159",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 558,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-160",
      "html_url": "https://goskive.com/course/fu-course-160",
      "slug": "fu-course-160",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 205,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:31.711Z",
      "shortname": "fu-course-160",
      "topic_id": 205,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 160",
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
Authorization: Bearer 989e4ad25632ebbddf2f5f51bfbb017e025af641d06a16fe768d19518023a11c
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
      "creator_id": 567,
      "id": 202,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "discipline_id": 212,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:32.467Z",
      "shortname": "fu-course-167",
      "topic_id": 212,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 567,
      "id": 203,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 183,
      "additional_university_ids": [

      ],
      "discipline_id": 213,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-06T18:17:32.506Z",
      "shortname": "fu-course-168",
      "topic_id": 213,
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
	-H "Authorization: Bearer 989e4ad25632ebbddf2f5f51bfbb017e025af641d06a16fe768d19518023a11c"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 058b17dfaae79d76a4f747fd6dc32c4273c1053e45b146cac4ad86ae6433ce3c
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
  "id": 354,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-06T18:17:09.359Z",
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
	-H "Authorization: Bearer 058b17dfaae79d76a4f747fd6dc32c4273c1053e45b146cac4ad86ae6433ce3c"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/311
Content-Type: application/json
Authorization: Bearer 7f91ce365eb8b2138f71825bb1e2aff1747da546999966a748bea1f1cfdaa971
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
    "id": 311,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 107,
    "fields_of_study": [
      107,
      108
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-06T18:17:05.253Z",
    "updated_at": "2016-12-06T18:17:05.253Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/311" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f91ce365eb8b2138f71825bb1e2aff1747da546999966a748bea1f1cfdaa971"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/313
Content-Type: application/json
Authorization: Bearer ecb380ece99291747b4a2d047dfc5597d3d8ba05a9f5b1e893a1798918c48261
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
    "id": 313,
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
    "created_at": "2016-12-06T18:17:05.344Z",
    "updated_at": "2016-12-06T18:17:05.344Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/313" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecb380ece99291747b4a2d047dfc5597d3d8ba05a9f5b1e893a1798918c48261"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer aa81c2c57cbc2867e8be44e9f3b390e09069dc8a4860a72fad7862c83054dc83
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa81c2c57cbc2867e8be44e9f3b390e09069dc8a4860a72fad7862c83054dc83"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/20
Content-Type: application/json
Authorization: Bearer 72fc3b90199e37553d73a99d7ca435912f937f401fec6208621df75aba285350
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
    "id": 20,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 103,
    "user_id": 580
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72fc3b90199e37553d73a99d7ca435912f937f401fec6208621df75aba285350"
```
