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
Authorization: Basic OGM0OTU0NzUwOWMwNmZiYmRmZmNlODA1ODU2M2E3YjAwNzVjZjBmM2Q0NDQw
ZmI2N2RiNjc3Y2YyZDM2OTM1YTpjNzk0YzgwM2RhZmZiNDI2NTQ4ZTQ4Y2Yx
Nzg2NTJlM2I3YzI1Y2NiMGJkN2NjZjdlYjBiMTRiNWUxYTQyMmQ4

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
	-u 8c49547509c06fbbdffce8058563a7b0075cf0f3d4440fb67db677cf2d36935a:c794c803daffb426548e48cf178652e3b7c25ccb0bd7ccf7eb0b14b5e1a422d8
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e94fab6753baac221500dd6a394f699fdebd2a3f21e590e8df31529382e40b89","client_secret":"6c7a99363f39b8aeb43baa91871d48cac1d9609e87e92fec2506325ca4e40127"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"e94fab6753baac221500dd6a394f699fdebd2a3f21e590e8df31529382e40b89","client_secret":"6c7a99363f39b8aeb43baa91871d48cac1d9609e87e92fec2506325ca4e40127"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZTc2OWQ5NmRkZDk1OGUyMjE5MzQ2ZGQyNDA4YWMyZDdhMzU4ZDg2MDc2M2Yw
NDAzNDI5N2E3YmNkNDhiYjQ0ZToyZWJmZGVhMDdlYmUxZjRlMTk4MTJhZTAw
ZjhmYmMzNDczZDQxYWMzZDkxMzFlNDQ4ZjFmNzI2M2I3NDhmMzNl

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
  "access_token": "999a50e24328e75f7af1a050155d0a138966bd96feb1ccdbbdca9e4298c2b01b",
  "token_type": "bearer",
  "created_at": 1479462501
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u e769d96ddd958e2219346dd2408ac2d7a358d860763f04034297a7bcd48bb44e:2ebfdea07ebe1f4e19812ae00f8fbc3473d41ac3d9131e448f1f7263b748f33e
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"c7083ecb134b1b1e85199eb480defd829f9e4ff2b581960ff068ed9f0b7c5aaf","client_secret":"69fda650decc03125c68b34bdba971d3771cb9cf7a2adc79a1fcb41f5443ad3f"}
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
  "access_token": "d274204b00a0894e34c2217658c56e3153a2e53071d28bcb10f8dd617a7e2d6e",
  "token_type": "bearer",
  "created_at": 1479462501
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"c7083ecb134b1b1e85199eb480defd829f9e4ff2b581960ff068ed9f0b7c5aaf","client_secret":"69fda650decc03125c68b34bdba971d3771cb9cf7a2adc79a1fcb41f5443ad3f"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"5ce5c1c29c881ad56924bc983b44a236e3ef6b221e5b38b07bee6d6cf1906503","client_secret":"bc28b55ee93b9f922cc7417e1a24f44a7bc8ed5a1c7c9981e51503279f72b851"}
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
  "access_token": "5d91753bd3ce25989eb9d4a8ce20e27d4d95a6dbb076485d7d1bcaa7dc4f6008",
  "token_type": "bearer",
  "created_at": 1479462501
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5ce5c1c29c881ad56924bc983b44a236e3ef6b221e5b38b07bee6d6cf1906503","client_secret":"bc28b55ee93b9f922cc7417e1a24f44a7bc8ed5a1c7c9981e51503279f72b851"}' -X POST \
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
Authorization: Bearer d2c7a1c6478fbf6ebf5cd21cde12a60389d359b7f91af2ff76f6ceee8b3d4943
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
    "company_id": 29,
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
	-H "Authorization: Bearer d2c7a1c6478fbf6ebf5cd21cde12a60389d359b7f91af2ff76f6ceee8b3d4943"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/70/flashcards
Content-Type: application/json
Authorization: Bearer 5142cb0827e480ce7447a4a430a5ef2a099f2236d3a349df1da7bde883077171
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":70,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 33,
    "obfuscated_id": "sjAD-GXxS8o",
    "author_id": 476,
    "chapter_id": 70,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T09:48:17.536Z",
    "created_at": "2016-11-18T09:48:17.536Z",
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
curl "api.goskive.com/v2/chapters/70/flashcards" -d '{"flashcard":{"chapter_id":70,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5142cb0827e480ce7447a4a430a5ef2a099f2236d3a349df1da7bde883077171"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/68/flashcards
Content-Type: application/json
Authorization: Bearer 093d2546c9d04712573a28311b72f7dab26a4517bd0d9d257d9a08ba449e01e7
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
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 468,
      "chapter_id": 68,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:17.070Z",
      "created_at": "2016-11-18T09:48:17.070Z",
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 468,
      "chapter_id": 68,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:17.116Z",
      "created_at": "2016-11-18T09:48:17.116Z",
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 468,
      "chapter_id": 68,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:17.163Z",
      "created_at": "2016-11-18T09:48:17.163Z",
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
curl "api.goskive.com/v2/chapters/68/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 093d2546c9d04712573a28311b72f7dab26a4517bd0d9d257d9a08ba449e01e7"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer a2de581346ad12921452e87d70f186dbac690560fbf6e4e5641bd0003351aff1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "updated_at": "2016-11-18T09:47:36.169Z",
    "created_at": "2016-11-18T09:47:36.169Z",
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
        "id": 7,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 8,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 9,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 10,
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
curl "api.goskive.com/v2/chapters/3/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":3,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2de581346ad12921452e87d70f186dbac690560fbf6e4e5641bd0003351aff1"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 249393696e712412ddf252785d6c25c257827349adcc8b7fe7d062efe396d76c
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
    "updated_at": "2016-11-18T09:47:36.917Z",
    "created_at": "2016-11-18T09:47:36.917Z",
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
        "id": 11,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 12,
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
	-H "Authorization: Bearer 249393696e712412ddf252785d6c25c257827349adcc8b7fe7d062efe396d76c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer f4519102dcca5a5b993cea902364e2c37e3bf9721002e12f92f65a4657b75145
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "updated_at": "2016-11-18T09:47:37.464Z",
    "created_at": "2016-11-18T09:47:37.464Z",
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
curl "api.goskive.com/v2/chapters/5/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4519102dcca5a5b993cea902364e2c37e3bf9721002e12f92f65a4657b75145"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/6/questions
Content-Type: application/json
Authorization: Bearer 3e1a0f67b8868f8e6665001cf9aade92363987133b554a6c5c3a1cefaedee46c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":6,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "updated_at": "2016-11-18T09:47:38.027Z",
    "created_at": "2016-11-18T09:47:38.027Z",
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
        "id": 15,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 16,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 17,
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
curl "api.goskive.com/v2/chapters/6/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":6,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e1a0f67b8868f8e6665001cf9aade92363987133b554a6c5c3a1cefaedee46c"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/2/questions
Content-Type: application/json
Authorization: Bearer c54522ba899a8ea72978fa811afa749290465c9975d5269d9124789abb793ff3
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
      "updated_at": "2016-11-18T09:47:35.491Z",
      "created_at": "2016-11-18T09:47:35.360Z",
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
      "updated_at": "2016-11-18T09:47:35.689Z",
      "created_at": "2016-11-18T09:47:35.565Z",
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
      "updated_at": "2016-11-18T09:47:35.888Z",
      "created_at": "2016-11-18T09:47:35.763Z",
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
	-H "Authorization: Bearer c54522ba899a8ea72978fa811afa749290465c9975d5269d9124789abb793ff3"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/56
Content-Type: application/json
Authorization: Bearer e49151b741eff40c103a8864170b80361714aa8e89f0de418f73b580d0274576
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
	-H "Authorization: Bearer e49151b741eff40c103a8864170b80361714aa8e89f0de418f73b580d0274576"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/58
Content-Type: application/json
Authorization: Bearer 80879363e943efd8fcaec77cf4f9e7e5f269d13db48fd28716848b88a32127de
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
curl "api.goskive.com/v2/chapters/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80879363e943efd8fcaec77cf4f9e7e5f269d13db48fd28716848b88a32127de"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/52
Content-Type: application/json
Authorization: Bearer 2973b1c4fef7a086cd2d6c85ade74e60563e2ce840c4c98ea6675e76c4ace4a8
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
curl "api.goskive.com/v2/chapters/52" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2973b1c4fef7a086cd2d6c85ade74e60563e2ce840c4c98ea6675e76c4ace4a8"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/59
Content-Type: application/json
Authorization: Bearer 2d750c18c3ce353cfcc175ee74dbe864b03388fadeec32408c8371824a476417
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d750c18c3ce353cfcc175ee74dbe864b03388fadeec32408c8371824a476417"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/55
Content-Type: application/json
Authorization: Bearer a142a26a9fb395ee474a137917050e64f350b2e1c079674429eade12c3ebfb34
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
    "id": 55,
    "updated_at": "2016-11-18T09:48:06.660Z",
    "course_id": 111,
    "author_id": 302,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-18T09:48:06.014Z",
    "questions_updated_at": "2016-11-18T09:48:06.014Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 306,
        "chapter_id": 55,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:06.639Z",
        "created_at": "2016-11-18T09:48:06.639Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 304,
        "chapter_id": 55,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:06.512Z",
        "created_at": "2016-11-18T09:48:06.357Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/55" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a142a26a9fb395ee474a137917050e64f350b2e1c079674429eade12c3ebfb34"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/53
Content-Type: application/json
Authorization: Bearer 435cbfbae3f9a09ba718dd0f7fbb237778810cf33424d4bc07ab4ab72f7aff15
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
    "id": 53,
    "updated_at": "2016-11-18T09:48:05.194Z",
    "course_id": 109,
    "author_id": 293,
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
curl "api.goskive.com/v2/chapters/53" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 435cbfbae3f9a09ba718dd0f7fbb237778810cf33424d4bc07ab4ab72f7aff15"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/14/replies
Content-Type: application/json
Authorization: Bearer 09906367286a13ab29c870c828e019f4d713d20ab6c5dae6ff84230953387ee1
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
    "id": 15,
    "author_id": 364,
    "reply_to_id": 14,
    "created_at": "2016-11-18T09:48:11.871Z",
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
curl "api.goskive.com/v2/comments/14/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09906367286a13ab29c870c828e019f4d713d20ab6c5dae6ff84230953387ee1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/13/replies
Content-Type: application/json
Authorization: Bearer 85d28049aeec56b30f177c755f02080e008d8f45ebd9c3738a02846f195afae2
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
curl "api.goskive.com/v2/comments/13/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85d28049aeec56b30f177c755f02080e008d8f45ebd9c3738a02846f195afae2"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/17
Content-Type: application/json
Authorization: Bearer 403ee3d9907377a491b8e5af694e08da7b7ec80ae958881e83d914183c67df86
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
curl "api.goskive.com/v2/comments/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 403ee3d9907377a491b8e5af694e08da7b7ec80ae958881e83d914183c67df86"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer 657ba62b60f85f9703041f6a8b65b2ce070a2c54eadc9c9854023dbd367648ea
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
curl "api.goskive.com/v2/comments/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 657ba62b60f85f9703041f6a8b65b2ce070a2c54eadc9c9854023dbd367648ea"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/18
Content-Type: application/json
Authorization: Bearer 4e05528b03f3b6b68c7cab2df3ffada585fdbe75252a5952ac4f32cb9bad3de0
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e05528b03f3b6b68c7cab2df3ffada585fdbe75252a5952ac4f32cb9bad3de0"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/56/report
Content-Type: application/json
Authorization: Bearer 3b0ba333a26bd2360b1f5defa219d9974ff4fa0fc1bdd798194b240f2f6da22c
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b0ba333a26bd2360b1f5defa219d9974ff4fa0fc1bdd798194b240f2f6da22c"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 9c3592ff4ee23a83cc6ea8d336e3bbcc4f5517f3c10ca00e77486731b991a364
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
    "id": 36,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-18T09:49:04.817Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c3592ff4ee23a83cc6ea8d336e3bbcc4f5517f3c10ca00e77486731b991a364"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer f12be1f7938c826c0743de48b8e1db08b47c52733c7844073266a972a0c6ae8b
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
      "id": 37,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T09:49:04.944Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T09:49:04.948Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T09:49:04.952Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f12be1f7938c826c0743de48b8e1db08b47c52733c7844073266a972a0c6ae8b"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/32/company_profiles
Content-Type: application/json
Authorization: Bearer ae247ed2e622e45ad0ddf34627bd00c62466ab5a6db237fb35061e4c1edf3b15
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
curl "api.goskive.com/v2/companies/32/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae247ed2e622e45ad0ddf34627bd00c62466ab5a6db237fb35061e4c1edf3b15"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/30/company_profiles
Content-Type: application/json
Authorization: Bearer 8c7262bbb0198f7c2cf4d0423790d2ef68525e7f868169ec1a332ced1224749c
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
curl "api.goskive.com/v2/companies/30/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c7262bbb0198f7c2cf4d0423790d2ef68525e7f868169ec1a332ced1224749c"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 917c36805325884c658d78e3246395018decbe62191484ba6e926c582a494312
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
      "id": 8,
      "title": "Campaign 8",
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
      "id": 11,
      "title": "Campaign 11",
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
	-H "Authorization: Bearer 917c36805325884c658d78e3246395018decbe62191484ba6e926c582a494312"
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
Authorization: Bearer 6f3c6f20a4862d4c34009cdf60649131f69a94b2be8205c72f3d601d39d31544
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
	-H "Authorization: Bearer 6f3c6f20a4862d4c34009cdf60649131f69a94b2be8205c72f3d601d39d31544"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 37b7cb85b0ddf31f433f7417a102140a3430ff1dc1e9eb742dc10c8782455c2b
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
    "id": 94,
    "updated_at": "2016-11-18T09:48:21.332Z",
    "course_id": 188,
    "author_id": 531,
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
	-H "Authorization: Bearer 37b7cb85b0ddf31f433f7417a102140a3430ff1dc1e9eb742dc10c8782455c2b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4b0db36d2ba2ada98bbba94b8748f180bfd5547181ad7a95fa00df4f93f5d8ca
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
      "id": 71,
      "updated_at": "2016-11-18T09:48:18.100Z",
      "course_id": 175,
      "author_id": 481,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 50",
      "position": 1
    },
    {
      "id": 72,
      "updated_at": "2016-11-18T09:48:18.128Z",
      "course_id": 175,
      "author_id": 482,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 51",
      "position": 2
    },
    {
      "id": 73,
      "updated_at": "2016-11-18T09:48:18.456Z",
      "course_id": 175,
      "author_id": 483,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-18T09:48:18.020Z",
      "questions_updated_at": "2016-11-18T09:48:18.020Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 52",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b0db36d2ba2ada98bbba94b8748f180bfd5547181ad7a95fa00df4f93f5d8ca"
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
      "updated_at": "2016-11-18T09:48:19.824Z",
      "course_id": 181,
      "author_id": 509,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 62",
      "position": 1
    },
    {
      "id": 84,
      "updated_at": "2016-11-18T09:48:19.852Z",
      "course_id": 181,
      "author_id": 510,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 63",
      "position": 2
    },
    {
      "id": 85,
      "updated_at": "2016-11-18T09:48:20.182Z",
      "course_id": 181,
      "author_id": 511,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-18T09:48:19.746Z",
      "questions_updated_at": "2016-11-18T09:48:19.746Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 64",
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
Authorization: Bearer 765dd99908f4a1fe106baca28dd95f852e2f70ca8c9ab4b43aaef4cd8c6b4e64
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
      "id": 74,
      "updated_at": "2016-11-18T09:48:18.768Z",
      "course_id": 177,
      "author_id": 490,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 53",
      "position": 1
    },
    {
      "id": 75,
      "updated_at": "2016-11-18T09:48:18.795Z",
      "course_id": 177,
      "author_id": 491,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 54",
      "position": 2
    },
    {
      "id": 76,
      "updated_at": "2016-11-18T09:48:18.823Z",
      "course_id": 177,
      "author_id": 492,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 55",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 765dd99908f4a1fe106baca28dd95f852e2f70ca8c9ab4b43aaef4cd8c6b4e64"
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
      "updated_at": "2016-11-18T09:48:20.312Z",
      "course_id": 182,
      "author_id": 515,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 65",
      "position": 1
    },
    {
      "id": 87,
      "updated_at": "2016-11-18T09:48:20.340Z",
      "course_id": 182,
      "author_id": 516,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 66",
      "position": 2
    },
    {
      "id": 88,
      "updated_at": "2016-11-18T09:48:20.368Z",
      "course_id": 182,
      "author_id": 517,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 67",
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
Authorization: Bearer 359ab801794f205b6c09afa39386df2418c748fda2d8cbb12523ed24d5ffb8b0
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
    "course_id": 190,
    "user_id": 541,
    "updated_at": "2016-11-18T09:48:21.847Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 359ab801794f205b6c09afa39386df2418c748fda2d8cbb12523ed24d5ffb8b0"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer e96681c52071eeb0f248424eacabbdb2d24586dcdf19cf3877730eaabf1332cb
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
      "course_id": 193,
      "user_id": 547,
      "updated_at": "2016-11-18T09:48:22.235Z"
    },
    {
      "id": 5,
      "course_id": 193,
      "user_id": 548,
      "updated_at": "2016-11-18T09:48:22.251Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e96681c52071eeb0f248424eacabbdb2d24586dcdf19cf3877730eaabf1332cb"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/120/files
Content-Type: application/json
Authorization: Bearer b464fa913d914741f465831221de44b4c32266f474145e01251105e1a3d1c013
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
      "id": 17,
      "uploader": {
        "id": 335,
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
        "created_at": "2016-11-18T09:48:09.164Z",
        "updated_at": "2016-11-18T09:48:09.164Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T09:48:09.175Z",
      "updated_at": "2016-11-18T09:48:09.175Z",
      "course_id": 120,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 18,
      "uploader": {
        "id": 336,
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
        "created_at": "2016-11-18T09:48:09.183Z",
        "updated_at": "2016-11-18T09:48:09.183Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T09:48:09.193Z",
      "updated_at": "2016-11-18T09:48:09.193Z",
      "course_id": 120,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 19,
      "uploader": {
        "id": 337,
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
        "created_at": "2016-11-18T09:48:09.201Z",
        "updated_at": "2016-11-18T09:48:09.201Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T09:48:09.211Z",
      "updated_at": "2016-11-18T09:48:09.211Z",
      "course_id": 120,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/120/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b464fa913d914741f465831221de44b4c32266f474145e01251105e1a3d1c013"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/119/files
Content-Type: application/json
Authorization: Bearer 5e4d96e478df228a2c238177224c677c3062c61870aeb1ce8fcfcd630ae2fb48
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
    "id": 16,
    "uploader": {
      "id": 333,
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
      "created_at": "2016-11-18T09:48:08.993Z",
      "updated_at": "2016-11-18T09:48:08.993Z"
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
    "created_at": "2016-11-18T09:48:09.030Z",
    "updated_at": "2016-11-18T09:48:09.030Z",
    "course_id": 119,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/119/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e4d96e478df228a2c238177224c677c3062c61870aeb1ce8fcfcd630ae2fb48"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/122/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 3c1ab8aebc80d817b6447e9b08b53c767425d5985e4da6b118f3f5e0bec0f64d
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
    "key": "cache/6047a42872d3f14b021d04a7e94f870d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xOFQxMDo0ODowOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzYwNDdhNDI4NzJkM2YxNGIwMjFkMDRhN2U5NGY4NzBkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE4VDA5NDgwOVoifV19",
    "x-amz-credential": "FAKE/20161118/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161118T094809Z",
    "x-amz-signature": "cb10b10a9dea74df45955d9294980401158efe31f984227dc6b6dca0a60ec882"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/122/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c1ab8aebc80d817b6447e9b08b53c767425d5985e4da6b118f3f5e0bec0f64d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 3d393d43527eb1ff765f61ebc659b1838f7b9f713b46f992059b0b63041f6ecc
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
	-H "Authorization: Bearer 3d393d43527eb1ff765f61ebc659b1838f7b9f713b46f992059b0b63041f6ecc"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9da7fdb22ab7c58ab55703fc1bb762c4e368d138e593b077cb04e6057cd9fd2c
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
	-H "Authorization: Bearer 9da7fdb22ab7c58ab55703fc1bb762c4e368d138e593b077cb04e6057cd9fd2c"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 29b9f20adb3bccff88351c2e345595eab45dc789eec75fb1760364c1970d7f4c
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
	-H "Authorization: Bearer 29b9f20adb3bccff88351c2e345595eab45dc789eec75fb1760364c1970d7f4c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9f2b437c3773de5d2150b18071e3a903b3861c6a86f9b0922f2eda27fade78a8
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
	-H "Authorization: Bearer 9f2b437c3773de5d2150b18071e3a903b3861c6a86f9b0922f2eda27fade78a8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a4150916681b07d2cbbccd0e86874c286a58d08918f0124bd4c7d079a12036ba
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
	-H "Authorization: Bearer a4150916681b07d2cbbccd0e86874c286a58d08918f0124bd4c7d079a12036ba"
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
    "creator_id": 891,
    "id": 286,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 271,
    "additional_university_ids": [

    ],
    "discipline_id": 299,
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
    "chapters_updated_at": "2016-11-18T09:48:52.393Z",
    "updated_at": "2016-11-18T09:48:53.935Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 103,
        "obfuscated_id": "AVhVflMAvL0",
        "author_id": 891,
        "chapter_id": 178,
        "position": 90,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:52.614Z",
        "created_at": "2016-11-18T09:48:52.491Z",
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
            "id": 209,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 210,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 105,
        "obfuscated_id": "3yX9LpVrF_M",
        "author_id": 891,
        "chapter_id": 179,
        "position": 92,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:53.021Z",
        "created_at": "2016-11-18T09:48:52.891Z",
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
            "id": 213,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 214,
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
        "id": 178,
        "updated_at": "2016-11-18T09:48:53.885Z",
        "course_id": 286,
        "author_id": 891,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T09:48:52.393Z",
        "questions_updated_at": "2016-11-18T09:48:52.393Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 154",
        "position": 1
      },
      {
        "id": 179,
        "updated_at": "2016-11-18T09:48:53.927Z",
        "course_id": 286,
        "author_id": 891,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T09:48:52.393Z",
        "questions_updated_at": "2016-11-18T09:48:52.393Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 155",
        "position": 2
      }
    ],
    "topic_id": 298,
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
Authorization: Bearer 4f5a9ca5ac01288eed9521839af8760504f9321dd097f3d9ab85c97e36c16341
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
    "creator_id": 902,
    "id": 288,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 273,
    "additional_university_ids": [

    ],
    "discipline_id": 301,
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
    "chapters_updated_at": "2016-11-18T09:48:55.649Z",
    "updated_at": "2016-11-18T09:48:57.192Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 903,
        "chapter_id": 182,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:56.971Z",
        "created_at": "2016-11-18T09:48:56.971Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 903,
        "chapter_id": 183,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:57.047Z",
        "created_at": "2016-11-18T09:48:57.047Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 903,
        "chapter_id": 182,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:57.013Z",
        "created_at": "2016-11-18T09:48:57.013Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 903,
        "chapter_id": 183,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:57.089Z",
        "created_at": "2016-11-18T09:48:57.089Z",
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
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 903,
        "chapter_id": 182,
        "position": 102,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.884Z",
        "created_at": "2016-11-18T09:48:55.758Z",
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
            "id": 233,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 234,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 116,
        "obfuscated_id": "PhHGVKqnHFA",
        "author_id": 903,
        "chapter_id": 182,
        "position": 103,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:56.071Z",
        "created_at": "2016-11-18T09:48:55.952Z",
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
            "id": 235,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 236,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 117,
        "obfuscated_id": "BsA8mEPn8aM",
        "author_id": 903,
        "chapter_id": 183,
        "position": 104,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:56.289Z",
        "created_at": "2016-11-18T09:48:56.159Z",
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
            "id": 237,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 238,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 903,
        "chapter_id": 183,
        "position": 105,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:56.483Z",
        "created_at": "2016-11-18T09:48:56.360Z",
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
            "id": 239,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 240,
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
        "id": 182,
        "updated_at": "2016-11-18T09:48:57.143Z",
        "course_id": 288,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T09:48:55.649Z",
        "questions_updated_at": "2016-11-18T09:48:55.649Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 158",
        "position": 1
      },
      {
        "id": 183,
        "updated_at": "2016-11-18T09:48:57.184Z",
        "course_id": 288,
        "author_id": 902,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T09:48:55.649Z",
        "questions_updated_at": "2016-11-18T09:48:55.649Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 159",
        "position": 2
      }
    ],
    "topic_id": 300,
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
	-H "Authorization: Bearer 4f5a9ca5ac01288eed9521839af8760504f9321dd097f3d9ab85c97e36c16341"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/290/pin
Content-Type: application/json
Authorization: Bearer 0b107a22888f511a1739471b3e5c7fc3c1f8bf0757ffb933f708a536e524c307
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/290/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b107a22888f511a1739471b3e5c7fc3c1f8bf0757ffb933f708a536e524c307"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/291/pin
Content-Type: application/json
Authorization: Bearer 65b9d017faa45d711a4f2c4e0324f7ed7b71f2d37825c89eaff6a02d425e1732
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/291/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65b9d017faa45d711a4f2c4e0324f7ed7b71f2d37825c89eaff6a02d425e1732"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ca5181034062462fbfd8109ac9d23fc1ae9348b2e0d37fe0795caf173e00c569
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
    "creator_id": 920,
    "id": 293,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 278,
    "additional_university_ids": [

    ],
    "discipline_id": 306,
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
    "updated_at": "2016-11-18T09:48:59.483Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 305,
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
	-H "Authorization: Bearer ca5181034062462fbfd8109ac9d23fc1ae9348b2e0d37fe0795caf173e00c569"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 79af3a9de2a7b3830c8136483f844c13ecf82993ce94c33f3913c2adbef603a7
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
    "id": 250,
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
    "created_at": "2016-11-18T09:47:59.000Z",
    "updated_at": "2016-11-18T09:47:59.000Z",
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
	-H "Authorization: Bearer 79af3a9de2a7b3830c8136483f844c13ecf82993ce94c33f3913c2adbef603a7"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b66c9b70ccf4cc6279bf092597769130bce1a02569bf6c964be02dd153c41e37
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[103]}
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
    "id": 252,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      103
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T09:47:59.408Z",
    "updated_at": "2016-11-18T09:47:59.443Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[103]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b66c9b70ccf4cc6279bf092597769130bce1a02569bf6c964be02dd153c41e37"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 52513bea7b78850fd84c2a42c244f52fbb52cff908751b66c8c8a00fc29f1372
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
    "id": 255,
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
    "created_at": "2016-11-18T09:47:59.613Z",
    "updated_at": "2016-11-18T09:47:59.613Z",
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
	-H "Authorization: Bearer 52513bea7b78850fd84c2a42c244f52fbb52cff908751b66c8c8a00fc29f1372"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 3ef272c547cabc877b52369ee110fb4ae30e5288ce10913f28d56f7b1fae0ed9
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[104]}
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
    "id": 253,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      104
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T09:47:59.486Z",
    "updated_at": "2016-11-18T09:47:59.486Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[104]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ef272c547cabc877b52369ee110fb4ae30e5288ce10913f28d56f7b1fae0ed9"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 5f742a0c422253d70a0543d01f5a46592f7c681c161d94d2db9559e2811acd98
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

102
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
    "id": 251,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/5c0c88ff4c48305239764a0d39e5ba36b4989a2d.jpg",
    "university_id": null,
    "fields_of_study": [
      102
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T09:47:59.096Z",
    "updated_at": "2016-11-18T09:47:59.354Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/990787f6bda6b42366b144a2424fb6bc13dbf208.jpg",
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

102
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 5f742a0c422253d70a0543d01f5a46592f7c681c161d94d2db9559e2811acd98"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 718a36edae4472b3202c8e2faf0857018992b1e7efcd55c1d995ca5ba2cc6408
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
      "id": 6,
      "bookmarkable_id": 75,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 76,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 77,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 718a36edae4472b3202c8e2faf0857018992b1e7efcd55c1d995ca5ba2cc6408"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer f13c0034ed00fd702738b901760b12395e2c029b5f2aa59be7c084dd599708ea
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
	-H "Authorization: Bearer f13c0034ed00fd702738b901760b12395e2c029b5f2aa59be7c084dd599708ea"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 3a81393a4cfcdc1e6828637cdcd12761cbd16f137ffc8b798e1ad508a1a53aa3
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
	-H "Authorization: Bearer 3a81393a4cfcdc1e6828637cdcd12761cbd16f137ffc8b798e1ad508a1a53aa3"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 1827e261d46a6c52ca497371b96dedbe5934f89f108df309373fcd2606e51e1f
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
      "creator_id": 366,
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-95",
      "html_url": "https://goskive.com/course/mit-course-95",
      "slug": "mit-course-95",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "discipline_id": 136,
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
      "updated_at": "2016-11-18T09:48:12.125Z",
      "shortname": "mit-course-95",
      "topic_id": 135,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 95",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 367,
      "id": 129,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-96",
      "html_url": "https://goskive.com/course/mit-course-96",
      "slug": "mit-course-96",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "discipline_id": 137,
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
      "updated_at": "2016-11-18T09:48:12.214Z",
      "shortname": "mit-course-96",
      "topic_id": 136,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 96",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1827e261d46a6c52ca497371b96dedbe5934f89f108df309373fcd2606e51e1f"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer a858d22f15c1a3c784a49e02a84225eb9f5e3cb9043dafc02d40c7bcc7bd1da5
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
        "created_at": "2016-11-18T09:49:01.939Z",
        "updated_at": "2016-11-18T09:49:01.939Z",
        "file_url": "memory://7eab44e6be72400e9855df74b2615f25.pdf",
        "course_id": 305,
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
        "created_at": "2016-11-18T09:49:02.026Z",
        "updated_at": "2016-11-18T09:49:02.026Z",
        "file_url": "memory://bdf2232db74c919d9f9346ab7789ab02.pdf",
        "course_id": 306,
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
        "created_at": "2016-11-18T09:49:02.112Z",
        "updated_at": "2016-11-18T09:49:02.112Z",
        "file_url": "memory://d8a9aa20730a7a68c1289411316af3ae.pdf",
        "course_id": 307,
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
	-H "Authorization: Bearer a858d22f15c1a3c784a49e02a84225eb9f5e3cb9043dafc02d40c7bcc7bd1da5"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 62926e4519aa332a38b5b5473a6c2e0e88f4f59931427dc3ff66cfe62af70da6
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
      "company_id": 26,
      "company": {
        "id": 26,
        "name": "Fake Company Name 26",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T09:47:51.079Z"
      },
      "created_at": "2016-11-18T09:47:51.083Z",
      "updated_at": "2016-11-18T09:47:51.083Z",
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
      "company_id": 27,
      "company": {
        "id": 27,
        "name": "Fake Company Name 27",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T09:47:51.091Z"
      },
      "created_at": "2016-11-18T09:47:51.094Z",
      "updated_at": "2016-11-18T09:47:51.094Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62926e4519aa332a38b5b5473a6c2e0e88f4f59931427dc3ff66cfe62af70da6"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer f0de5fbdb08a71c9f1c15129e9376276a55ee407ad02279cfbb87d3fd3ae1ffa
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T09:47:50.901Z"
      },
      "created_at": "2016-11-18T09:47:50.906Z",
      "updated_at": "2016-11-18T09:47:50.906Z",
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
      "company_id": 23,
      "company": {
        "id": 23,
        "name": "Fake Company Name 23",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T09:47:50.920Z"
      },
      "created_at": "2016-11-18T09:47:50.924Z",
      "updated_at": "2016-11-18T09:47:50.924Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0de5fbdb08a71c9f1c15129e9376276a55ee407ad02279cfbb87d3fd3ae1ffa"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer b146c5b6eacb491d4381ad1e0e7b799f0691c9c3f8785240f5d061d1f6d4fd7e
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
      "created_at": "2016-11-18T09:49:02.456Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-11-18T09:49:02.571Z",
      "author_id": "959",
      "thread_subject_id": "309",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 21,
      "created_at": "2016-11-18T09:49:02.559Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 60,
      "updated_at": "2016-11-18T09:49:02.574Z",
      "author_id": "962",
      "thread_subject_id": "310",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 22,
      "created_at": "2016-11-18T09:49:02.970Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-11-18T09:49:02.970Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 23,
      "created_at": "2016-11-18T09:49:03.361Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-11-18T09:49:03.361Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 24,
      "created_at": "2016-11-18T09:49:03.765Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 23,
      "updated_at": "2016-11-18T09:49:03.765Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 25,
      "created_at": "2016-11-18T09:49:04.090Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 132,
      "updated_at": "2016-11-18T09:49:04.090Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 26,
      "created_at": "2016-11-18T09:49:04.410Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 133,
      "updated_at": "2016-11-18T09:49:04.410Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 27,
      "created_at": "2016-11-18T09:49:04.732Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 134,
      "updated_at": "2016-11-18T09:49:04.732Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b146c5b6eacb491d4381ad1e0e7b799f0691c9c3f8785240f5d061d1f6d4fd7e"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/19
Content-Type: application/json
Authorization: Bearer d916967eab237288988b2b7e3a9360b6147ecd60227cb44b61be709e2f3a76b7
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-18T09:39:02.000Z"}}
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
    "created_at": "2016-11-18T09:49:02.276Z",
    "read_at": "2016-11-18T09:39:02.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-11-18T09:49:02.337Z",
    "author_id": "955",
    "thread_subject_id": "308",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/19" -d '{"notification":{"read_at":"2016-11-18T09:39:02.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d916967eab237288988b2b7e3a9360b6147ecd60227cb44b61be709e2f3a76b7"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b54dd7ef0c07637b17fdb42a94a55e3e0b1bc26a574b6c20353981dde5ba80bd
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
      "id": 5,
      "course_id": 257,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-18T09:48:40.555Z",
      "course_published": true,
      "updated_at": "2016-11-18T09:48:40.547Z"
    },
    {
      "id": 6,
      "course_id": 258,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-18T09:48:40.639Z",
      "course_published": true,
      "updated_at": "2016-11-18T09:48:40.631Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b54dd7ef0c07637b17fdb42a94a55e3e0b1bc26a574b6c20353981dde5ba80bd"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 4de9067897467c20d9c669434fe9f7052843d807c7e933adf9d2e45a6665b9e3
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
    "course_id": 256,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-18T09:48:40.387Z",
    "course_published": true,
    "updated_at": "2016-11-18T09:48:40.379Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4de9067897467c20d9c669434fe9f7052843d807c7e933adf9d2e45a6665b9e3"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 424574606a5e20fd5980b485eaf397ceb83943895cd1200a8e2189b8223ed76c
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
    "id": 3,
    "course_id": 255,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-18T09:48:40.279Z",
    "course_published": true,
    "updated_at": "2016-11-18T09:48:40.267Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 424574606a5e20fd5980b485eaf397ceb83943895cd1200a8e2189b8223ed76c"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer bc20f26fb1a3dfbc46c05138b6c1e1ee521440ac533bcf8ffbfd17a0329f2aac
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
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 25,
      "user_id": 229
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 26,
      "user_id": 229
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 27,
      "user_id": 229
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 229
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc20f26fb1a3dfbc46c05138b6c1e1ee521440ac533bcf8ffbfd17a0329f2aac"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/19
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
    "id": 19,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 17,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 19
      },
      {
        "id": 18,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 19
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/19" -X GET \
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
      "id": 17,
      "name": "Automated well-modulated analyzer",
      "name_translations": {
        "en": "Automated well-modulated analyzer"
      }
    },
    {
      "id": 18,
      "name": "Future-proofed global application",
      "name_translations": {
        "en": "Future-proofed global application"
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
PATCH /v2/feedbacks/40/close
Content-Type: application/json
Authorization: Bearer 08f163bc710020407af89202ed986ed9092c1c0c307df49ab17f4d8e58afa887
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
    "id": 40,
    "user_id": 652,
    "feedbackable_id": 39,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-18T09:48:30.897Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/40/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08f163bc710020407af89202ed986ed9092c1c0c307df49ab17f4d8e58afa887"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/44/fix
Content-Type: application/json
Authorization: Bearer 8acaa61176fb77a1701daa4d9179998539278c71681ccb774250cf3afe22ada8
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
    "user_id": 672,
    "feedbackable_id": 43,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-18T09:48:32.312Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/44/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8acaa61176fb77a1701daa4d9179998539278c71681ccb774250cf3afe22ada8"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/38
Content-Type: application/json
Authorization: Bearer adc273f00765a3875dfbc1fdfb00585d1293d2812d8086a21549efd81452b524
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
    "id": 38,
    "user_id": 640,
    "feedbackable_id": 37,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T09:48:30.379Z",
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
curl "api.goskive.com/v2/feedbacks/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adc273f00765a3875dfbc1fdfb00585d1293d2812d8086a21549efd81452b524"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/close
Content-Type: application/json
Authorization: Bearer c02ed9b6226b9addd1b116819b2ab9a38a6b42155d2a21884e61e022ebd064c1
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
curl "api.goskive.com/v2/feedbacks/42/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c02ed9b6226b9addd1b116819b2ab9a38a6b42155d2a21884e61e022ebd064c1"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/45/fix
Content-Type: application/json
Authorization: Bearer ebfd25c020f0a2faf1286ffd6870d3dd6977844cfa62bf9cbe9cafb7e3de499f
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
curl "api.goskive.com/v2/feedbacks/45/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebfd25c020f0a2faf1286ffd6870d3dd6977844cfa62bf9cbe9cafb7e3de499f"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/fix
Content-Type: application/json
Authorization: Bearer d0fb39c2fe27622da2f9f167d571de5a871c7007056447e2d98387ada2de6959
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
curl "api.goskive.com/v2/feedbacks/46/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0fb39c2fe27622da2f9f167d571de5a871c7007056447e2d98387ada2de6959"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/39
Content-Type: application/json
Authorization: Bearer c3fc32338ad64ca071cb3eccad468970d66cedc0e4f652de16c435d4ddeed462
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
    "id": 39,
    "user_id": 645,
    "feedbackable_id": 38,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T09:48:30.685Z",
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
curl "api.goskive.com/v2/feedbacks/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3fc32338ad64ca071cb3eccad468970d66cedc0e4f652de16c435d4ddeed462"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 5ff7499095564dcdae7bd47ff2c1f71d7ec9422115f38dfebdcd97998ee0682b
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
	-H "Authorization: Bearer 5ff7499095564dcdae7bd47ff2c1f71d7ec9422115f38dfebdcd97998ee0682b"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/7/bookmark
Content-Type: application/json
Authorization: Bearer 1b979048be5a6aba9dc8a2c93862de3dcbd9a3f7f3aac8a6cc243116fd7554b0
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b979048be5a6aba9dc8a2c93862de3dcbd9a3f7f3aac8a6cc243116fd7554b0"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer 71153883f0c8a36ac9a3584c5147e5514d87a9333dbeac9ad985cad1a47ae142
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
	-H "Authorization: Bearer 71153883f0c8a36ac9a3584c5147e5514d87a9333dbeac9ad985cad1a47ae142"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/11
Content-Type: application/json
Authorization: Bearer e6099a3f4fab66853a848c1dc44cf6b7bae5f9cdacb26cfcc4e1a554308de45d
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/3b1dde1dd8d1461b48ae16abb4ccce58.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161118%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161118T094755Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=43ed63ef90444e0a00eaa46d3f9774033a2c7668c6c3f98c549091dcbe2c8c90",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6099a3f4fab66853a848c1dc44cf6b7bae5f9cdacb26cfcc4e1a554308de45d"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/6/preview
Content-Type: application/json
Authorization: Bearer 886d364c9c3ccc8c94152a0d025b13bec9ee10577462dbee422e99335964783f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5cf6e1292cbbb4eb149c3f7c9e6416ae.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161118%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161118T094755Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=aa28303e517e248e55275506c87f02bc31de12884e7e29d06f78ad2be879c6ae",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/6/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 886d364c9c3ccc8c94152a0d025b13bec9ee10577462dbee422e99335964783f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/4/metadata
Content-Type: application/json
Authorization: Bearer fd55b11a0353fd52da746e5dc02d2af13db99667d686e26af39f9e04af5be2d1
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
    "id": 4,
    "uploader": {
      "id": 200,
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
      "created_at": "2016-11-18T09:47:54.913Z",
      "updated_at": "2016-11-18T09:47:54.913Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-18T09:47:54.990Z",
    "updated_at": "2016-11-18T09:47:54.990Z",
    "course_id": 84,
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
curl "api.goskive.com/v2/files/4/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd55b11a0353fd52da746e5dc02d2af13db99667d686e26af39f9e04af5be2d1"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/14/matched_courses?required_cu_count=2
Authorization: Bearer 972aaf83e893dbb033bbf9fdad3e6363053cac9aab23f672beaa5f3fac2d78ba
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
      "creator_id": 267,
      "id": 103,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 82,
      "additional_university_ids": [

      ],
      "discipline_id": 111,
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
      "chapters_updated_at": "2016-11-18T09:47:59.687Z",
      "updated_at": "2016-11-18T09:48:02.123Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 110,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 272,
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-0f77803e-331e-428d-afa2-01d7e65eabdb",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-0f77803e-331e-428d-afa2-01d7e65eabdb",
      "slug": "mit-the-great-british-bake-off-0f77803e-331e-428d-afa2-01d7e65eabdb",
      "university_id": 83,
      "additional_university_ids": [

      ],
      "discipline_id": 112,
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
      "chapters_updated_at": "2016-11-18T09:47:59.687Z",
      "updated_at": "2016-11-18T09:48:02.771Z",
      "shortname": "mit-the-great-british-bake-off-0f77803e-331e-428d-afa2-01d7e65eabdb",
      "topic_id": 111,
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
curl "api.goskive.com/v2/files/14/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 972aaf83e893dbb033bbf9fdad3e6363053cac9aab23f672beaa5f3fac2d78ba"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/13/download
Content-Type: application/json
Authorization: Bearer 9b522dbd79cd3b0ee1f13974bc7e5aae09c8e7298e88c703caf98a6a11aa4097
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
	-H "Authorization: Bearer 9b522dbd79cd3b0ee1f13974bc7e5aae09c8e7298e88c703caf98a6a11aa4097"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/12/report
Content-Type: application/json
Authorization: Bearer 256ee80be1060a2780e185de7fc2b4f0983cac0d4d57b9fa9c96609763dc6ead
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
	-H "Authorization: Bearer 256ee80be1060a2780e185de7fc2b4f0983cac0d4d57b9fa9c96609763dc6ead"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/1/bookmark
Content-Type: application/json
Authorization: Bearer cf6fa16b56b43ee0b885a5dfffbed38db6a978b9c053678c0c3657ceb3e114fd
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/1/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf6fa16b56b43ee0b885a5dfffbed38db6a978b9c053678c0c3657ceb3e114fd"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/5/upvote
Content-Type: application/json
Authorization: Bearer 50e7255f42ab12230a1deb45b537a37ca4c412a45e102706e3044823cf61278b
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50e7255f42ab12230a1deb45b537a37ca4c412a45e102706e3044823cf61278b"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/3/comments
Content-Type: application/json
Authorization: Bearer 10cb106db3fb9fd048d7706d46941509afb5f23a33f7883d34f3cb50c223a257
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
    "id": 2,
    "author_id": 28,
    "reply_to_id": null,
    "created_at": "2016-11-18T09:47:39.805Z",
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
curl "api.goskive.com/v2/flashcards/3/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10cb106db3fb9fd048d7706d46941509afb5f23a33f7883d34f3cb50c223a257"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/2/comments
Content-Type: application/json
Authorization: Bearer 66997658f09ff096bcc397555c49a2acfc74e3d0ec5c7812b69fff5760ea4989
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
    "id": 1,
    "author_id": 25,
    "reply_to_id": null,
    "created_at": "2016-11-18T09:47:38.957Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 25,
      "feedbackable_id": 2,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:38.952Z",
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
curl "api.goskive.com/v2/flashcards/2/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66997658f09ff096bcc397555c49a2acfc74e3d0ec5c7812b69fff5760ea4989"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/4/comments
Content-Type: application/json
Authorization: Bearer 4acd24aee713b362beab06636cd97e347f6e11039514528d781a0c6c03ba5626
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
      "author_id": 35,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:47:40.194Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 34,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:47:40.176Z",
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
curl "api.goskive.com/v2/flashcards/4/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4acd24aee713b362beab06636cd97e347f6e11039514528d781a0c6c03ba5626"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/1/comments
Content-Type: application/json
Authorization: Bearer 49d806f22bf364800f7b488af1ea4321d035da1f5af1620164aeb4ce7cbd681a
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
curl "api.goskive.com/v2/flashcards/1/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49d806f22bf364800f7b488af1ea4321d035da1f5af1620164aeb4ce7cbd681a"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/11/feedbacks
Content-Type: application/json
Authorization: Bearer e2904a19a5fb31597e49c7a878c2fc88d65cb5f9c0c74b9fa78fe2e88dd8ab6e
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
    "id": 4,
    "user_id": 120,
    "feedbackable_id": 11,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T09:47:49.500Z",
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
curl "api.goskive.com/v2/flashcards/11/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2904a19a5fb31597e49c7a878c2fc88d65cb5f9c0c74b9fa78fe2e88dd8ab6e"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/15/feedbacks
Content-Type: application/json
Authorization: Bearer c1eb69a6fd56d3677e50ca1633eb375491a41a6bd13645521426a58884c18a66
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
      "id": 8,
      "user_id": 144,
      "feedbackable_id": 15,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:50.454Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 143,
      "feedbackable_id": 15,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:50.443Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/15/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1eb69a6fd56d3677e50ca1633eb375491a41a6bd13645521426a58884c18a66"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer 225cd13c49844c3b04ba011ee6ed62dc91dcf16e5539fccab8e28d9fb191064a
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
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 325
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 324
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 323
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 225cd13c49844c3b04ba011ee6ed62dc91dcf16e5539fccab8e28d9fb191064a"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/65/republish
Content-Type: application/json
Authorization: Bearer f2bebbe56cfa3ca8464ce27a1a5710fae255e39124f90255e1b4af65c7afad0a
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
curl "api.goskive.com/v2/flashcards/65/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2bebbe56cfa3ca8464ce27a1a5710fae255e39124f90255e1b4af65c7afad0a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/67/bookmark
Content-Type: application/json
Authorization: Bearer 08c9d0fba1e60209e0fd0aeaac086745411d9d07ae404c2a6b6bfc390f49c38d
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/67/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08c9d0fba1e60209e0fd0aeaac086745411d9d07ae404c2a6b6bfc390f49c38d"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/63
Content-Type: application/json
Authorization: Bearer 38bbf55782c92c7268d5f5fac7d85095445f4769b3f7d7465bdb5a8332036bcc
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
	-H "Authorization: Bearer 38bbf55782c92c7268d5f5fac7d85095445f4769b3f7d7465bdb5a8332036bcc"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/68/downvote
Content-Type: application/json
Authorization: Bearer e51c7d86331e498010cc0635eb2b6f8a920b422239556ab511c1f1753306466f
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/68/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e51c7d86331e498010cc0635eb2b6f8a920b422239556ab511c1f1753306466f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/47
Content-Type: application/json
Authorization: Bearer 62ce0296b4d46d5bc095780fd5d9bb334214a045d98f43ae1aeabd85421da20e
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
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 703,
    "chapter_id": 127,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T09:48:34.966Z",
    "created_at": "2016-11-18T09:48:34.966Z",
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
curl "api.goskive.com/v2/flashcards/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62ce0296b4d46d5bc095780fd5d9bb334214a045d98f43ae1aeabd85421da20e"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/report
Content-Type: application/json
Authorization: Bearer eb651bf750bd3c14dcd6257238ed0dd91ee8993629745e3ce3c058a58e629f51
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb651bf750bd3c14dcd6257238ed0dd91ee8993629745e3ce3c058a58e629f51"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/46/bookmark
Content-Type: application/json
Authorization: Bearer 016ffebd03f1997a1df23bc5c586f6b3a03999c0ccc7f6e9cb52030221b30554
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/46/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 016ffebd03f1997a1df23bc5c586f6b3a03999c0ccc7f6e9cb52030221b30554"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/64/upvote
Content-Type: application/json
Authorization: Bearer 3072569f4cd920760a8ced6a6741227498ff7c8100efc552425909713463b246
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/64/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3072569f4cd920760a8ced6a6741227498ff7c8100efc552425909713463b246"
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
    "key": "cache/de7de0183f66de43260ca2b1da19671c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xOFQxMDo0OTowMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2RlN2RlMDE4M2Y2NmRlNDMyNjBjYTJiMWRhMTk2NzFjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMThUMDk0OTAxWiJ9XX0=",
    "x-amz-credential": "FAKE/20161118/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161118T094901Z",
    "x-amz-signature": "bbf6842d4a6d487a03c3d66039328671069bb1c150c96244a78edea8d1492f84"
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
Authorization: Bearer 63cc3c63d50d41a02931431f809aacc942cbc347096289acd7368dc4377bc60d
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
	-H "Authorization: Bearer 63cc3c63d50d41a02931431f809aacc942cbc347096289acd7368dc4377bc60d"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 7d3a0f2942c22a1d729438e2dc0d2adcee9334f0983f83b2fd733c144e6d870e
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
	-H "Authorization: Bearer 7d3a0f2942c22a1d729438e2dc0d2adcee9334f0983f83b2fd733c144e6d870e"
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
{"password":{"reset_password_token":"PE9wNGxziFVxTb6VnWsf","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 807,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-18T09:48:43.000Z",
  "updated_at": "2016-11-18T09:48:43.144Z",
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
  "audit_id": 5207
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"PE9wNGxziFVxTb6VnWsf","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/9/comments
Content-Type: application/json
Authorization: Bearer cf4fa9e4a8e4e9aadaa57abdd8de127adb7033dfaa47c8e5d20bf98607308226
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
    "id": 6,
    "author_id": 45,
    "reply_to_id": null,
    "created_at": "2016-11-18T09:47:41.827Z",
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
curl "api.goskive.com/v2/questions/9/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf4fa9e4a8e4e9aadaa57abdd8de127adb7033dfaa47c8e5d20bf98607308226"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/8/comments
Content-Type: application/json
Authorization: Bearer dffc5dfa6b29ce924142ac67c10262e0d2d98e708c345566252f294dae7c4aed
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
    "id": 5,
    "author_id": 42,
    "reply_to_id": null,
    "created_at": "2016-11-18T09:47:41.350Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 2,
      "user_id": 42,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:41.348Z",
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
curl "api.goskive.com/v2/questions/8/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dffc5dfa6b29ce924142ac67c10262e0d2d98e708c345566252f294dae7c4aed"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer 0a03f0a1be4303faf4e725876ab99077d9e5e52e3e96c6af0f7e7aca897229e6
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
      "id": 8,
      "author_id": 55,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:47:42.626Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 54,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:47:42.611Z",
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
curl "api.goskive.com/v2/questions/11/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a03f0a1be4303faf4e725876ab99077d9e5e52e3e96c6af0f7e7aca897229e6"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/10/comments
Content-Type: application/json
Authorization: Bearer e4a2e68c4817f20649e5e919e944a7a55a24bf6d7a67504dbc3068a5cb22bc54
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
curl "api.goskive.com/v2/questions/10/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4a2e68c4817f20649e5e919e944a7a55a24bf6d7a67504dbc3068a5cb22bc54"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/23/feedbacks
Content-Type: application/json
Authorization: Bearer 3131f599c54ce7b7523c803986d804391c885317651917ecd11697ac281ffc5b
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
    "id": 17,
    "user_id": 186,
    "feedbackable_id": 23,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-18T09:47:53.741Z",
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
curl "api.goskive.com/v2/questions/23/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3131f599c54ce7b7523c803986d804391c885317651917ecd11697ac281ffc5b"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/19/feedbacks
Content-Type: application/json
Authorization: Bearer 1704a4c1abb81076d2a7c063edcdf58036b7557340c477cc021474119fd482ef
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
      "id": 14,
      "user_id": 174,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:52.322Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 173,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:52.311Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/19/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1704a4c1abb81076d2a7c063edcdf58036b7557340c477cc021474119fd482ef"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/46/votes
Content-Type: application/json
Authorization: Bearer 4a0393c0cca336a5536aece610a0491cc6dd4c3603c63910ba4375270cb5b134
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
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 46,
      "user_id": 351
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 46,
      "user_id": 350
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 46,
      "user_id": 349
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/46/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a0393c0cca336a5536aece610a0491cc6dd4c3603c63910ba4375270cb5b134"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/98/republish
Content-Type: application/json
Authorization: Bearer ba81be3a4901cd2cadb3551cf2929e7f3ea3be582d73148b31e0b47b6ada1171
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
curl "api.goskive.com/v2/questions/98/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba81be3a4901cd2cadb3551cf2929e7f3ea3be582d73148b31e0b47b6ada1171"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/80/bookmark
Content-Type: application/json
Authorization: Bearer 13254e6e4aa4169ea2118fde0edab97cdabd83beb7f415b60a2d4423fc2d5a93
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/80/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13254e6e4aa4169ea2118fde0edab97cdabd83beb7f415b60a2d4423fc2d5a93"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/102
Content-Type: application/json
Authorization: Bearer fd9099833b20bb34dedd41799156b2e2617e67dcd299f9966c14df2ba18b6604
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/102" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd9099833b20bb34dedd41799156b2e2617e67dcd299f9966c14df2ba18b6604"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/101/downvote
Content-Type: application/json
Authorization: Bearer eb72b181230b43dd413412f1f7e505beb85a041a5f15c3a729b4e447a79b8374
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/101/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb72b181230b43dd413412f1f7e505beb85a041a5f15c3a729b4e447a79b8374"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/99
Content-Type: application/json
Authorization: Bearer 97a12b6759b44351e2162474b1b5c4ace5ad50bf3bdbddf258fafc2bf43c7033
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
    "id": 99,
    "obfuscated_id": "5fPQ9k37GTc",
    "author_id": 879,
    "chapter_id": 174,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T09:48:50.597Z",
    "created_at": "2016-11-18T09:48:50.472Z",
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
        "id": 200,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 201,
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
curl "api.goskive.com/v2/questions/99" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97a12b6759b44351e2162474b1b5c4ace5ad50bf3bdbddf258fafc2bf43c7033"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/96/report
Content-Type: application/json
Authorization: Bearer de3a209a2f003c85450a72bb39abab8f06816a3c92c02450c845c6afd66c583b
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/96/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de3a209a2f003c85450a72bb39abab8f06816a3c92c02450c845c6afd66c583b"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/78/bookmark
Content-Type: application/json
Authorization: Bearer 1d793d11c9bf83c6827fbb8e1ecf6d8c619a60a2048e838582da45f33d018e2c
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/78/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d793d11c9bf83c6827fbb8e1ecf6d8c619a60a2048e838582da45f33d018e2c"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/100
Content-Type: application/json
Authorization: Bearer ef5056ce80b0747e8206a2627a6b2a65693663b8fdf16d07caa1492383d5ca02
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-18T09:48:50.829Z","updated_at":"2016-11-18T09:48:50.953Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":175,"author_id":882,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 100,
    "obfuscated_id": "erXmBhoMZFI",
    "author_id": 882,
    "chapter_id": 175,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T09:48:51.072Z",
    "created_at": "2016-11-18T09:48:50.829Z",
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
    "question": "{\"id\"=>100, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-18T09:48:50.829Z\", \"updated_at\"=>\"2016-11-18T09:48:50.953Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>175, \"author_id\"=>882, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 202,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 203,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 204,
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
curl "api.goskive.com/v2/questions/100" -d '{"question":{"question":{"id":100,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-18T09:48:50.829Z","updated_at":"2016-11-18T09:48:50.953Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":175,"author_id":882,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef5056ce80b0747e8206a2627a6b2a65693663b8fdf16d07caa1492383d5ca02"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/79/upvote
Content-Type: application/json
Authorization: Bearer 70009f90812c8642d30c321930bf23901bd4bf11b51a6cfde1b3043043a566b3
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/79/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70009f90812c8642d30c321930bf23901bd4bf11b51a6cfde1b3043043a566b3"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 9a3641a5696dcfbc731246a63bce08490a4ef9a87a1c75981ebbeb2ea21143a4
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
      "creator_id": 113,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 39,
      "additional_university_ids": [

      ],
      "discipline_id": 65,
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
      "updated_at": "2016-11-18T09:47:48.663Z",
      "shortname": "mit-pizza-201",
      "topic_id": 64,
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
	-H "Authorization: Bearer 9a3641a5696dcfbc731246a63bce08490a4ef9a87a1c75981ebbeb2ea21143a4"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 0cde2493f4732a26c3b1678999b24bd19b7f6061365a9a99990114943fd41af3
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
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-24",
      "html_url": "https://goskive.com/university/uni-24",
      "slug": "uni-24",
      "name": "National School of Pizza",
      "short_name": "Uni 24",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a7373949a1cda4c5a16c5e7ea1d0302115644a89.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e0ce9b75009e6ad70c288bb4cba677fff124c601.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T09:47:48.912Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-23",
      "html_url": "https://goskive.com/university/uni-23",
      "slug": "uni-23",
      "name": "National School of Pastry",
      "short_name": "Uni 23",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/76b80440855be14f7b79e084332d34b2a704d6ba.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b9507216c93bc95ed5b763cc8a6259161a6f5496.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T09:47:48.894Z",
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
	-H "Authorization: Bearer 0cde2493f4732a26c3b1678999b24bd19b7f6061365a9a99990114943fd41af3"
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
      "id": 262,
      "name": "Organized 24 hour matrices",
      "name_translations": {
        "en": "Organized 24 hour matrices"
      },
      "discipline_id": 263
    },
    {
      "id": 263,
      "name": "Virtual global neural-net",
      "name_translations": {
        "en": "Virtual global neural-net"
      },
      "discipline_id": 264
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
GET /v2/topics/261
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
    "id": 261,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 262
  }
}
```



```shell
curl "api.goskive.com/v2/topics/261" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 9f0cc942f5a2725ab8e68835f826f0a968a2c8e92c49c1ea27de4cc21732ec94
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
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-187",
      "html_url": "https://goskive.com/university/uni-187",
      "slug": "uni-187",
      "name": "University 139",
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
      "updated_at": "2016-11-18T09:48:33.166Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-188",
      "html_url": "https://goskive.com/university/uni-188",
      "slug": "uni-188",
      "name": "University 140",
      "short_name": "Uni 188",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c1bcbe98f5e30a1d2c062d00e265207a3c76c1d6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3db8b7a7fd23a5908ee95827523b8d2a965fac10.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T09:48:33.184Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-189",
      "html_url": "https://goskive.com/university/uni-189",
      "slug": "uni-189",
      "name": "University 141",
      "short_name": "Uni 189",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/94a8023f21254ce163a5b5ede98bdc819440a3a0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6d49f3aa5d676dcd5fa043f4ff8e782f8f1ac73f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T09:48:33.201Z",
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
	-H "Authorization: Bearer 9f0cc942f5a2725ab8e68835f826f0a968a2c8e92c49c1ea27de4cc21732ec94"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 626bd731da8708dcda73596212390b911dfab5f8f6a1705bbb29c78625eec4e1
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
    "id": 205,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/251a3379388b624d381a43405118f30764fe4f9f.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7ed7b255515aee55da5cb2e74b72737d8381795f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-18T09:48:32.986Z",
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
	-H "Authorization: Bearer 626bd731da8708dcda73596212390b911dfab5f8f6a1705bbb29c78625eec4e1"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer aad8000ca65a8bba8192d3fc463b59c4fbddaade7d337f669bd7098289191f23
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":24,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 68,
    "id": 22,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 22,
    "additional_university_ids": [

    ],
    "discipline_id": 25,
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
    "chapters_updated_at": "2016-11-18T09:47:44.117Z",
    "updated_at": "2016-11-18T09:47:44.265Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 17,
        "updated_at": "2016-11-18T09:47:44.221Z",
        "course_id": 22,
        "author_id": 68,
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
        "id": 18,
        "updated_at": "2016-11-18T09:47:44.238Z",
        "course_id": 22,
        "author_id": 68,
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
        "id": 19,
        "updated_at": "2016-11-18T09:47:44.255Z",
        "course_id": 22,
        "author_id": 68,
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
    "topic_id": 24,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":24,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aad8000ca65a8bba8192d3fc463b59c4fbddaade7d337f669bd7098289191f23"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4175ee5ef3918ecfd9c3b087592d48224a963e5c6f60b4123bd0c4f8416e1bc9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":25,"published":false}}
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
    "creator_id": 69,
    "id": 23,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 23,
    "additional_university_ids": [

    ],
    "discipline_id": 26,
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
    "updated_at": "2016-11-18T09:47:44.475Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 25,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":25,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4175ee5ef3918ecfd9c3b087592d48224a963e5c6f60b4123bd0c4f8416e1bc9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 12cb0605c1e7b88d9e69a41ac8c750468cef0e30782584cda6f7de85f2d735d4
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
      "creator_id": 72,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-13",
      "html_url": "https://goskive.com/course/fu-course-13",
      "slug": "fu-course-13",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "discipline_id": 30,
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
      "updated_at": "2016-11-18T09:47:44.878Z",
      "shortname": "fu-course-13",
      "topic_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 13",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 72,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-14",
      "html_url": "https://goskive.com/course/fu-course-14",
      "slug": "fu-course-14",
      "university_id": 25,
      "additional_university_ids": [

      ],
      "discipline_id": 31,
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
      "chapters_updated_at": "2016-11-18T09:47:44.722Z",
      "updated_at": "2016-11-18T09:47:45.209Z",
      "shortname": "fu-course-14",
      "topic_id": 30,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 14",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12cb0605c1e7b88d9e69a41ac8c750468cef0e30782584cda6f7de85f2d735d4"
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
      "creator_id": 102,
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-37",
      "html_url": "https://goskive.com/course/fu-course-37",
      "slug": "fu-course-37",
      "university_id": 34,
      "additional_university_ids": [

      ],
      "discipline_id": 54,
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
      "updated_at": "2016-11-18T09:47:47.579Z",
      "shortname": "fu-course-37",
      "topic_id": 53,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 37",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 102,
      "id": 52,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-38",
      "html_url": "https://goskive.com/course/fu-course-38",
      "slug": "fu-course-38",
      "university_id": 34,
      "additional_university_ids": [

      ],
      "discipline_id": 55,
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
      "chapters_updated_at": "2016-11-18T09:47:47.429Z",
      "updated_at": "2016-11-18T09:47:47.899Z",
      "shortname": "fu-course-38",
      "topic_id": 54,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 38",
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
Authorization: Bearer bb840dd3f58e3cd7021ebb65d75ee2f799b5aaf7f6a68cdfca070cc19e32183e
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
      "creator_id": 79,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-17",
      "html_url": "https://goskive.com/course/fu-course-17",
      "slug": "fu-course-17",
      "university_id": 27,
      "additional_university_ids": [

      ],
      "discipline_id": 34,
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
      "updated_at": "2016-11-18T09:47:45.503Z",
      "shortname": "fu-course-17",
      "topic_id": 33,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 17",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 79,
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-18",
      "html_url": "https://goskive.com/course/fu-course-18",
      "slug": "fu-course-18",
      "university_id": 27,
      "additional_university_ids": [

      ],
      "discipline_id": 35,
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
      "updated_at": "2016-11-18T09:47:45.545Z",
      "shortname": "fu-course-18",
      "topic_id": 34,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 18",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb840dd3f58e3cd7021ebb65d75ee2f799b5aaf7f6a68cdfca070cc19e32183e"
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
      "creator_id": 107,
      "id": 55,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 36,
      "additional_university_ids": [

      ],
      "discipline_id": 58,
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
      "updated_at": "2016-11-18T09:47:48.110Z",
      "shortname": "fu-course-41",
      "topic_id": 57,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 107,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 36,
      "additional_university_ids": [

      ],
      "discipline_id": 59,
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
      "updated_at": "2016-11-18T09:47:48.149Z",
      "shortname": "fu-course-42",
      "topic_id": 58,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
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
Authorization: Bearer c709683f01e73b9f45de3711f9d2b454e8766967c0a3948c69d17af86af29870
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
  "id": 945,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-18T09:49:01.546Z",
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
	-H "Authorization: Bearer c709683f01e73b9f45de3711f9d2b454e8766967c0a3948c69d17af86af29870"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/464
Content-Type: application/json
Authorization: Bearer ff34f000fa662c207790df6373a34f5fe759c18a1642204ae62c15d0a03ae57f
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
    "id": 464,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 150,
    "fields_of_study": [
      178,
      179
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-18T09:48:16.722Z",
    "updated_at": "2016-11-18T09:48:16.722Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/464" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff34f000fa662c207790df6373a34f5fe759c18a1642204ae62c15d0a03ae57f"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/462
Content-Type: application/json
Authorization: Bearer 02b471191fc2854e77e1c3011e3d05221e58907d59e3a60c7c74935188a9d3a5
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
    "id": 462,
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
    "created_at": "2016-11-18T09:48:16.564Z",
    "updated_at": "2016-11-18T09:48:16.564Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/462" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02b471191fc2854e77e1c3011e3d05221e58907d59e3a60c7c74935188a9d3a5"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/16
Content-Type: application/json
Authorization: Bearer b5d8131310f1cc20aa1e75202688cc25f24f302fb125b14fe1f75631fcd0d418
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5d8131310f1cc20aa1e75202688cc25f24f302fb125b14fe1f75631fcd0d418"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/15
Content-Type: application/json
Authorization: Bearer 10db8ad62951bc693f2c1bd22591df0dcda5d18fa5a48e2175046aa362756615
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
    "votable_id": 73,
    "user_id": 692
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10db8ad62951bc693f2c1bd22591df0dcda5d18fa5a48e2175046aa362756615"
```
