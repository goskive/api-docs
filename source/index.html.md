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
Authorization: Basic MWQwZDE0ZDdhODNkYjgxMzJmMTFlZWFhZWEyMzVkOTI4MDIwZTdjMjJiOTNj
YzlkZmVkYjc4MWY3NDdhYjk3OTo4NjE0ZGRmNzhhYjFmYjA0MmQzMjgzYjUw
MGVjMTljNTYwNzk2YjA4ZWI4MjAzNWFlOTkxYzUzZjk4ZjZhNjUx

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
	-u 1d0d14d7a83db8132f11eeaaea235d928020e7c22b93cc9dfedb781f747ab979:8614ddf78ab1fb042d3283b500ec19c560796b08eb82035ae991c53f98f6a651
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
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"61eb518909e2c24845b51875b3d5f16b324332ce943b79af07656df982e57582","client_secret":"2889384596738ff3c87ffb293231cee3fb07938914268db50c699948e226f420"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"61eb518909e2c24845b51875b3d5f16b324332ce943b79af07656df982e57582","client_secret":"2889384596738ff3c87ffb293231cee3fb07938914268db50c699948e226f420"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NGU2YjRlOGQzMTRjMWU1MmEwYTc4OWFiMWUzNjMxNWZiNzRmNDI4Y2JlMTM3
YzY2YjdmZjYwOWU0OTg2MTQwODpmOTNmMjc2YTFlZDQ4NmFlMzQ3ZDgxYWQ3
YWYwNWNkOGRhZmI2ZmZiMjY0YWFkOWUyNTdmMTg0ZjdjY2ZmMjEy

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
  "access_token": "4e5cc37e95c07405b5f1e39228aa76f462cd773e1c776b09c0fd51f0c988f6be",
  "token_type": "bearer",
  "created_at": 1479316992
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 4e6b4e8d314c1e52a0a789ab1e36315fb74f428cbe137c66b7ff609e49861408:f93f276a1ed486ae347d81ad7af05cd8dafb6ffb264aad9e257f184f7ccff212
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"73f4d03c22fa86e5a52ef307fc6eee0d6ca327df33463010f2682127c1d01616","client_secret":"c23869fb132c287c28c3d006fcd7207d58215d3e16a5149e14845ca2bd199f21"}
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
  "access_token": "21580d31a22356be91fd1a3139eaa32d67729eec40560837c93abc87706e74ec",
  "token_type": "bearer",
  "created_at": 1479316992
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"73f4d03c22fa86e5a52ef307fc6eee0d6ca327df33463010f2682127c1d01616","client_secret":"c23869fb132c287c28c3d006fcd7207d58215d3e16a5149e14845ca2bd199f21"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"7473bb1a8b4aa0028dd368b34c9c87079f0a097d2183959de18442dcc651fcfe","client_secret":"c5a69955ec3de1ca9838e6d76046ae77615a19b0c95027fdf63b8e763666d2cf"}
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
  "access_token": "fd71cef3ce28f7c4bd4fa4b8aa7d92e4d9d6c9eb027ef59345b1704543cb05cf",
  "token_type": "bearer",
  "created_at": 1479316992
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"7473bb1a8b4aa0028dd368b34c9c87079f0a097d2183959de18442dcc651fcfe","client_secret":"c5a69955ec3de1ca9838e6d76046ae77615a19b0c95027fdf63b8e763666d2cf"}' -X POST \
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
Authorization: Bearer 8f180358537e52b5ee1f29d9ea5dc9a9e27071bde5686b7f7e3dbfc1da6cfca9
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
    "company_id": 27,
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
	-H "Authorization: Bearer 8f180358537e52b5ee1f29d9ea5dc9a9e27071bde5686b7f7e3dbfc1da6cfca9"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/50/flashcards
Content-Type: application/json
Authorization: Bearer f0e391083f3f82f7cb0d6b093507590641308f98cb20e31562a2391fe13ce651
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":50,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 21,
    "obfuscated_id": "XIvx1qd7-fY",
    "author_id": 378,
    "chapter_id": 50,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:24.627Z",
    "created_at": "2016-11-16T17:23:24.627Z",
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
curl "api.goskive.com/v2/chapters/50/flashcards" -d '{"flashcard":{"chapter_id":50,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0e391083f3f82f7cb0d6b093507590641308f98cb20e31562a2391fe13ce651"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/49/flashcards
Content-Type: application/json
Authorization: Bearer 83ccb1ddb959f752b53cb69dd24baa37041f803708f25a48448d1d8bf811a2a4
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 373,
      "chapter_id": 49,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:24.355Z",
      "created_at": "2016-11-16T17:23:24.355Z",
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
      "author_id": 373,
      "chapter_id": 49,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:24.392Z",
      "created_at": "2016-11-16T17:23:24.392Z",
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 373,
      "chapter_id": 49,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:24.429Z",
      "created_at": "2016-11-16T17:23:24.429Z",
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
curl "api.goskive.com/v2/chapters/49/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83ccb1ddb959f752b53cb69dd24baa37041f803708f25a48448d1d8bf811a2a4"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/10/questions
Content-Type: application/json
Authorization: Bearer df5a1b9bffcc282632e6d52ceee6c148649a076d7140de5e58411c3fbc434c34
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":10,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 155,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:05.650Z",
    "created_at": "2016-11-16T17:23:05.650Z",
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
        "id": 9,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 10,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 11,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 12,
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
curl "api.goskive.com/v2/chapters/10/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":10,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df5a1b9bffcc282632e6d52ceee6c148649a076d7140de5e58411c3fbc434c34"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/8/questions
Content-Type: application/json
Authorization: Bearer c770485cc0c81d704d158464f89be5f491d569ea1d2bdc2bdb51dbaed537bf03
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":8,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 149,
    "chapter_id": 8,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:04.567Z",
    "created_at": "2016-11-16T17:23:04.567Z",
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
        "id": 5,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 6,
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
curl "api.goskive.com/v2/chapters/8/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":8,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c770485cc0c81d704d158464f89be5f491d569ea1d2bdc2bdb51dbaed537bf03"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/9/questions
Content-Type: application/json
Authorization: Bearer 8179be41d7eb91cbc6c73e41c3295a270a16a86cc9ab75331f9939ba69456e9d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":9,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 152,
    "chapter_id": 9,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:05.127Z",
    "created_at": "2016-11-16T17:23:05.127Z",
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
curl "api.goskive.com/v2/chapters/9/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":9,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8179be41d7eb91cbc6c73e41c3295a270a16a86cc9ab75331f9939ba69456e9d"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/11/questions
Content-Type: application/json
Authorization: Bearer 3fec09ba2b4ac4c8d3fa518a2ab99ff296a95aefa23d8cfea959c2c08223f482
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":11,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 158,
    "chapter_id": 11,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:06.328Z",
    "created_at": "2016-11-16T17:23:06.328Z",
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
        "id": 13,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 14,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 15,
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
curl "api.goskive.com/v2/chapters/11/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":11,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fec09ba2b4ac4c8d3fa518a2ab99ff296a95aefa23d8cfea959c2c08223f482"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/13/questions
Content-Type: application/json
Authorization: Bearer 9ed34b4c309e8f38e91dfdcb7e4c6b2b9ec92420960ddb0d5d173442df8763c9
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
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 164,
      "chapter_id": 13,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:07.058Z",
      "created_at": "2016-11-16T17:23:06.939Z",
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
    },
    {
      "id": 8,
      "obfuscated_id": "X2B_8FVuFe8",
      "author_id": 165,
      "chapter_id": 13,
      "position": 4,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:07.251Z",
      "created_at": "2016-11-16T17:23:07.128Z",
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
    },
    {
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 166,
      "chapter_id": 13,
      "position": 5,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-16T17:23:07.451Z",
      "created_at": "2016-11-16T17:23:07.323Z",
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
          "id": 20,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 21,
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
curl "api.goskive.com/v2/chapters/13/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ed34b4c309e8f38e91dfdcb7e4c6b2b9ec92420960ddb0d5d173442df8763c9"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/122
Content-Type: application/json
Authorization: Bearer c47612d184b97dce8e0e639624f83bae808d06f364a91718af6f1bc2a5ad2c1b
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
curl "api.goskive.com/v2/chapters/122" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c47612d184b97dce8e0e639624f83bae808d06f364a91718af6f1bc2a5ad2c1b"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/124
Content-Type: application/json
Authorization: Bearer 36b0a7d554d4b3fcb5882287536911eaa56324787fa41436efe8efec289f8e69
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
curl "api.goskive.com/v2/chapters/124" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36b0a7d554d4b3fcb5882287536911eaa56324787fa41436efe8efec289f8e69"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/125
Content-Type: application/json
Authorization: Bearer 8e26ea7a8dd989adb030ffa4e1522340e4a1f084db48b6c1be3425e86bbd6399
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
curl "api.goskive.com/v2/chapters/125" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e26ea7a8dd989adb030ffa4e1522340e4a1f084db48b6c1be3425e86bbd6399"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/121
Content-Type: application/json
Authorization: Bearer 71ffb614da4f0dfff642fb83c168033db7b5302b93fdd0764664ee222a6b739a
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/121" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71ffb614da4f0dfff642fb83c168033db7b5302b93fdd0764664ee222a6b739a"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/120
Content-Type: application/json
Authorization: Bearer 5a25affca5d6656a40445a73153a08c2b2bd459103f1aa45cd0aa17a5f51dd5f
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
    "id": 120,
    "updated_at": "2016-11-16T17:23:53.853Z",
    "course_id": 237,
    "author_id": 675,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-16T17:23:53.324Z",
    "questions_updated_at": "2016-11-16T17:23:53.324Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 679,
        "chapter_id": 120,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:53.837Z",
        "created_at": "2016-11-16T17:23:53.837Z",
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
        "id": 98,
        "obfuscated_id": "icApzX10lRE",
        "author_id": 677,
        "chapter_id": 120,
        "position": 85,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:53.727Z",
        "created_at": "2016-11-16T17:23:53.610Z",
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
            "id": 199,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 200,
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
curl "api.goskive.com/v2/chapters/120" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a25affca5d6656a40445a73153a08c2b2bd459103f1aa45cd0aa17a5f51dd5f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/127
Content-Type: application/json
Authorization: Bearer 4c6834b2ad65a47cacdabb089c9a19b169a91680c2e37db896db4d985d04827d
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
    "id": 127,
    "updated_at": "2016-11-16T17:23:55.364Z",
    "course_id": 244,
    "author_id": 700,
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
curl "api.goskive.com/v2/chapters/127" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c6834b2ad65a47cacdabb089c9a19b169a91680c2e37db896db4d985d04827d"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/2/replies
Content-Type: application/json
Authorization: Bearer a228027d5fd10f5e0503252a827fb858f317c667065b9770b64cb7d24c591fb1
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
    "author_id": 15,
    "reply_to_id": 2,
    "created_at": "2016-11-16T17:22:56.782Z",
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
	-H "Authorization: Bearer a228027d5fd10f5e0503252a827fb858f317c667065b9770b64cb7d24c591fb1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/1/replies
Content-Type: application/json
Authorization: Bearer 3f5dc3332b6e0b6757f2775f05ae8f92d23d0c22d8c26be1d4b3d55ed76a519c
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
	-H "Authorization: Bearer 3f5dc3332b6e0b6757f2775f05ae8f92d23d0c22d8c26be1d4b3d55ed76a519c"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/42
Content-Type: application/json
Authorization: Bearer 4d251ff8bdac113d3fc0e8f6b808e4b23142cbe312462477eae99c70cb835419
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
curl "api.goskive.com/v2/comments/42" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d251ff8bdac113d3fc0e8f6b808e4b23142cbe312462477eae99c70cb835419"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/4/republish
Content-Type: application/json
Authorization: Bearer cdbe75ac54ac0fc801c04adb101097f30b36eb10b58d34aa4350aa4d28095223
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
	-H "Authorization: Bearer cdbe75ac54ac0fc801c04adb101097f30b36eb10b58d34aa4350aa4d28095223"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/44
Content-Type: application/json
Authorization: Bearer 2c840b10ed1eb917b95cff9c3107cdb18f29694ee8c08777e27fdd04c4d704aa
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c840b10ed1eb917b95cff9c3107cdb18f29694ee8c08777e27fdd04c4d704aa"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/6/report
Content-Type: application/json
Authorization: Bearer ab1f6595b466e0d18348c16eefb07f744801bfb0d7ecab35c6cdd013f0484d1b
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
	-H "Authorization: Bearer ab1f6595b466e0d18348c16eefb07f744801bfb0d7ecab35c6cdd013f0484d1b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/28
Content-Type: application/json
Authorization: Bearer d2faea2e0c02d0c39a10d0e87c980c3f7b609493a3f121c94756d6e81a28ec64
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
    "id": 28,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-16T17:23:39.670Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2faea2e0c02d0c39a10d0e87c980c3f7b609493a3f121c94756d6e81a28ec64"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer edb8b4d20d4a3c59930a7f5015103bbe75016bc06662c37a7257dd6d974659fc
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
      "id": 29,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/eb30fd9939333e805126ba26a8736769f7ca2ba6.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-16T17:23:39.740Z"
    },
    {
      "id": 30,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-16T17:23:39.744Z"
    },
    {
      "id": 31,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/0df235007210ab1331461f6a10296cd43f327e64.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-16T17:23:39.748Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edb8b4d20d4a3c59930a7f5015103bbe75016bc06662c37a7257dd6d974659fc"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/3/company_profiles
Content-Type: application/json
Authorization: Bearer 97c42b036f605f637f42f76b30300a75c3d7f771932b776878f4a365b8c38797
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
curl "api.goskive.com/v2/companies/3/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97c42b036f605f637f42f76b30300a75c3d7f771932b776878f4a365b8c38797"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/1/company_profiles
Content-Type: application/json
Authorization: Bearer 5efa2385abc356e93db49fd6ba752e2dfb4cb9ee077a5fc212bc936ab4cea409
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
curl "api.goskive.com/v2/companies/1/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5efa2385abc356e93db49fd6ba752e2dfb4cb9ee077a5fc212bc936ab4cea409"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 7e52274186d6502ce1ff9070ef7b29751dd473d54fe2cf8e1dd67dd245386d62
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
          "id": 8,
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e52274186d6502ce1ff9070ef7b29751dd473d54fe2cf8e1dd67dd245386d62"
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
Authorization: Bearer b3588c053e5d4f9dbbebe29c4cc8f9a5ded5f365f2a057740b75170a2f9049ed
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
	-H "Authorization: Bearer b3588c053e5d4f9dbbebe29c4cc8f9a5ded5f365f2a057740b75170a2f9049ed"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7bd7a952e282f1ddd5d25ed646c7d4f24d7d8a27c82edea57f8086f951f66f25
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
    "id": 51,
    "updated_at": "2016-11-16T17:23:24.877Z",
    "course_id": 149,
    "author_id": 380,
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
	-H "Authorization: Bearer 7bd7a952e282f1ddd5d25ed646c7d4f24d7d8a27c82edea57f8086f951f66f25"
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
      "id": 60,
      "updated_at": "2016-11-16T17:23:26.298Z",
      "course_id": 156,
      "author_id": 402,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 45",
      "position": 1
    },
    {
      "id": 61,
      "updated_at": "2016-11-16T17:23:26.320Z",
      "course_id": 156,
      "author_id": 403,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 46",
      "position": 2
    },
    {
      "id": 62,
      "updated_at": "2016-11-16T17:23:26.559Z",
      "course_id": 156,
      "author_id": 404,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-16T17:23:26.228Z",
      "questions_updated_at": "2016-11-16T17:23:26.228Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 47",
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
Authorization: Bearer 99a55593c9781aa7b6de7e62fc68c47cbb082f18eefe1111c884c7ba8c7a703c
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
      "updated_at": "2016-11-16T17:23:26.910Z",
      "course_id": 159,
      "author_id": 413,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 51",
      "position": 1
    },
    {
      "id": 67,
      "updated_at": "2016-11-16T17:23:26.933Z",
      "course_id": 159,
      "author_id": 414,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 52",
      "position": 2
    },
    {
      "id": 68,
      "updated_at": "2016-11-16T17:23:27.173Z",
      "course_id": 159,
      "author_id": 415,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-16T17:23:26.838Z",
      "questions_updated_at": "2016-11-16T17:23:26.838Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 53",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99a55593c9781aa7b6de7e62fc68c47cbb082f18eefe1111c884c7ba8c7a703c"
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
      "id": 63,
      "updated_at": "2016-11-16T17:23:26.674Z",
      "course_id": 157,
      "author_id": 408,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 48",
      "position": 1
    },
    {
      "id": 64,
      "updated_at": "2016-11-16T17:23:26.697Z",
      "course_id": 157,
      "author_id": 409,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 49",
      "position": 2
    },
    {
      "id": 65,
      "updated_at": "2016-11-16T17:23:26.720Z",
      "course_id": 157,
      "author_id": 410,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 50",
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
Authorization: Bearer 80c1381112ff33bbd34c6497e3a55b40bbc001be79570f82c6fde40b00ec8570
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
      "updated_at": "2016-11-16T17:23:27.326Z",
      "course_id": 160,
      "author_id": 420,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 54",
      "position": 1
    },
    {
      "id": 70,
      "updated_at": "2016-11-16T17:23:27.349Z",
      "course_id": 160,
      "author_id": 421,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 55",
      "position": 2
    },
    {
      "id": 71,
      "updated_at": "2016-11-16T17:23:27.370Z",
      "course_id": 160,
      "author_id": 422,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 56",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80c1381112ff33bbd34c6497e3a55b40bbc001be79570f82c6fde40b00ec8570"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0198e55dde2f65e669567be579fecb1c6c9002713611ff795742d3f00c406f48
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
    "course_id": 138,
    "user_id": 345,
    "updated_at": "2016-11-16T17:23:22.205Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0198e55dde2f65e669567be579fecb1c6c9002713611ff795742d3f00c406f48"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 5845bca62544ba6b545edba6c1e43ba0feed8d021df741630cbeb60530b35825
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
      "course_id": 133,
      "user_id": 331,
      "updated_at": "2016-11-16T17:23:21.416Z"
    },
    {
      "id": 2,
      "course_id": 133,
      "user_id": 332,
      "updated_at": "2016-11-16T17:23:21.433Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5845bca62544ba6b545edba6c1e43ba0feed8d021df741630cbeb60530b35825"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/143/files
Content-Type: application/json
Authorization: Bearer b54b8ee4ded3c6618fb1db51c6763df46c08d29485dafdeaa341e8d6c52f0d38
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
        "id": 362,
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
        "created_at": "2016-11-16T17:23:23.665Z",
        "updated_at": "2016-11-16T17:23:23.665Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:23:23.727Z",
      "updated_at": "2016-11-16T17:23:23.727Z",
      "course_id": 143,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 363,
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
        "created_at": "2016-11-16T17:23:23.736Z",
        "updated_at": "2016-11-16T17:23:23.736Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:23:23.751Z",
      "updated_at": "2016-11-16T17:23:23.751Z",
      "course_id": 143,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 364,
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
        "created_at": "2016-11-16T17:23:23.758Z",
        "updated_at": "2016-11-16T17:23:23.758Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-16T17:23:23.767Z",
      "updated_at": "2016-11-16T17:23:23.767Z",
      "course_id": 143,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/143/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b54b8ee4ded3c6618fb1db51c6763df46c08d29485dafdeaa341e8d6c52f0d38"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/145/files
Content-Type: application/json
Authorization: Bearer 4fe95163f05627c551f9370d50bae11b5fdd21d387aea7aa03f8811614a4c89c
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
    "id": 7,
    "uploader": {
      "id": 369,
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
      "created_at": "2016-11-16T17:23:24.016Z",
      "updated_at": "2016-11-16T17:23:24.016Z"
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
    "created_at": "2016-11-16T17:23:24.046Z",
    "updated_at": "2016-11-16T17:23:24.046Z",
    "course_id": 145,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/145/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fe95163f05627c551f9370d50bae11b5fdd21d387aea7aa03f8811614a4c89c"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/142/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 44d0bca3639eb5b822b238f8bfadb1fdf07445a1b3f8aec6d700f021e16f441e
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
    "key": "cache/b4cb7354e68cfd737921725496b0263c.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xNlQxODoyMzoyM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I0Y2I3MzU0ZTY4Y2ZkNzM3OTIxNzI1NDk2YjAyNjNjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE2VDE3MjMyM1oifV19",
    "x-amz-credential": "FAKE/20161116/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161116T172323Z",
    "x-amz-signature": "8adef7c069b498b3d34c40a2e7443310511663aa5195db845db8be6a69322586"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/142/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44d0bca3639eb5b822b238f8bfadb1fdf07445a1b3f8aec6d700f021e16f441e"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 6d7fcc7131685755bc0590c5bc9df2a9bd5ddb3082a6342794a387d8474d2cc5
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
	-H "Authorization: Bearer 6d7fcc7131685755bc0590c5bc9df2a9bd5ddb3082a6342794a387d8474d2cc5"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4ceb06d1cb40de7e56b11a33030b7b7478cfbee6e1ae552508a05e31071f7f4a
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
	-H "Authorization: Bearer 4ceb06d1cb40de7e56b11a33030b7b7478cfbee6e1ae552508a05e31071f7f4a"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bdc1083dbee76a7cc330d6d51af002a434a8682c6621462404ad45ba74b9fc19
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
	-H "Authorization: Bearer bdc1083dbee76a7cc330d6d51af002a434a8682c6621462404ad45ba74b9fc19"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0a09a0b532dc487751578ba599db01cd28034d0575288207fd3233d33845703b
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
	-H "Authorization: Bearer 0a09a0b532dc487751578ba599db01cd28034d0575288207fd3233d33845703b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9fd46faf37f682b762e79647a3f0b3f0dbaeac6c66bebbb69fb10f3fb63151e3
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
	-H "Authorization: Bearer 9fd46faf37f682b762e79647a3f0b3f0dbaeac6c66bebbb69fb10f3fb63151e3"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 1bfc685762511d29e3104323654dfa7dbf9e2da34a5831f00101d7e7f01b4338
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
    "creator_id": 587,
    "id": 207,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 192,
    "additional_university_ids": [

    ],
    "discipline_id": 217,
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
    "chapters_updated_at": "2016-11-16T17:23:42.875Z",
    "updated_at": "2016-11-16T17:23:44.281Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 588,
        "chapter_id": 107,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.086Z",
        "created_at": "2016-11-16T17:23:44.086Z",
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
        "author_id": 588,
        "chapter_id": 108,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.153Z",
        "created_at": "2016-11-16T17:23:44.153Z",
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
        "author_id": 588,
        "chapter_id": 107,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.125Z",
        "created_at": "2016-11-16T17:23:44.125Z",
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
        "author_id": 588,
        "chapter_id": 108,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.191Z",
        "created_at": "2016-11-16T17:23:44.191Z",
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
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 588,
        "chapter_id": 107,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:43.086Z",
        "created_at": "2016-11-16T17:23:42.972Z",
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
            "id": 149,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 150,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 588,
        "chapter_id": 107,
        "position": 61,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:43.259Z",
        "created_at": "2016-11-16T17:23:43.149Z",
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
            "id": 151,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 152,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 588,
        "chapter_id": 108,
        "position": 62,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:43.464Z",
        "created_at": "2016-11-16T17:23:43.341Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 588,
        "chapter_id": 108,
        "position": 63,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:43.640Z",
        "created_at": "2016-11-16T17:23:43.528Z",
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
            "id": 155,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 156,
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
        "id": 107,
        "updated_at": "2016-11-16T17:23:44.237Z",
        "course_id": 207,
        "author_id": 587,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:23:42.875Z",
        "questions_updated_at": "2016-11-16T17:23:42.875Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 92",
        "position": 1
      },
      {
        "id": 108,
        "updated_at": "2016-11-16T17:23:44.274Z",
        "course_id": 207,
        "author_id": 587,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:23:42.875Z",
        "questions_updated_at": "2016-11-16T17:23:42.875Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 93",
        "position": 2
      }
    ],
    "topic_id": 216,
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
	-H "Authorization: Bearer 1bfc685762511d29e3104323654dfa7dbf9e2da34a5831f00101d7e7f01b4338"
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
    "creator_id": 593,
    "id": 208,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 193,
    "additional_university_ids": [

    ],
    "discipline_id": 218,
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
    "chapters_updated_at": "2016-11-16T17:23:44.398Z",
    "updated_at": "2016-11-16T17:23:45.816Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 593,
        "chapter_id": 109,
        "position": 66,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.597Z",
        "created_at": "2016-11-16T17:23:44.485Z",
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
            "id": 161,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 162,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 593,
        "chapter_id": 110,
        "position": 68,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-16T17:23:44.974Z",
        "created_at": "2016-11-16T17:23:44.849Z",
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
            "id": 165,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 166,
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
        "id": 109,
        "updated_at": "2016-11-16T17:23:45.768Z",
        "course_id": 208,
        "author_id": 593,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:23:44.398Z",
        "questions_updated_at": "2016-11-16T17:23:44.398Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 94",
        "position": 1
      },
      {
        "id": 110,
        "updated_at": "2016-11-16T17:23:45.808Z",
        "course_id": 208,
        "author_id": 593,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-16T17:23:44.398Z",
        "questions_updated_at": "2016-11-16T17:23:44.398Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 95",
        "position": 2
      }
    ],
    "topic_id": 217,
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
PUT /v2/courses/223/pin
Content-Type: application/json
Authorization: Bearer a6e2ddfba526c6d0fdf03358da299934d6dd0c95a558180645ffbff30eb5fc3a
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/223/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6e2ddfba526c6d0fdf03358da299934d6dd0c95a558180645ffbff30eb5fc3a"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/218/pin
Content-Type: application/json
Authorization: Bearer 7bdd4a56da027ed29210f4f59d01a5dcfcbd60d88ca2e715f40fe91c72e32d42
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/218/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7bdd4a56da027ed29210f4f59d01a5dcfcbd60d88ca2e715f40fe91c72e32d42"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a7f5311b40d295b2e9678f885543c4493486374067d8913c00409c65fa5eb25a
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
    "creator_id": 624,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 206,
    "additional_university_ids": [

    ],
    "discipline_id": 231,
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
    "updated_at": "2016-11-16T17:23:47.985Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 230,
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
	-H "Authorization: Bearer a7f5311b40d295b2e9678f885543c4493486374067d8913c00409c65fa5eb25a"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer c977e3707176219241e827e8ace1a0bc47c121f73f781ab52037fcfc41c444ab
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
    "created_at": "2016-11-16T17:23:28.632Z",
    "updated_at": "2016-11-16T17:23:28.632Z",
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
	-H "Authorization: Bearer c977e3707176219241e827e8ace1a0bc47c121f73f781ab52037fcfc41c444ab"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d0f6d13af97068d4d267c37132261d9619d7c9b0aa2e98cbfaabdf9aae398169
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[169]}
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
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      169
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-16T17:23:28.721Z",
    "updated_at": "2016-11-16T17:23:28.760Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[169]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0f6d13af97068d4d267c37132261d9619d7c9b0aa2e98cbfaabdf9aae398169"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c5c7da5954fa4d231d1b0a3b977d59bca8992ce4b304fc70f3a2e55751a27db0
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
    "id": 448,
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
    "created_at": "2016-11-16T17:23:28.855Z",
    "updated_at": "2016-11-16T17:23:28.855Z",
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
	-H "Authorization: Bearer c5c7da5954fa4d231d1b0a3b977d59bca8992ce4b304fc70f3a2e55751a27db0"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0fc1eb144e23c64c640c98fc0557fb466c10211cb4e8421e0bdccfba123df471
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[172]}
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
    "id": 449,
    "first_name": "Magnus",
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
    "created_at": "2016-11-16T17:23:28.947Z",
    "updated_at": "2016-11-16T17:23:28.947Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[172]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fc1eb144e23c64c640c98fc0557fb466c10211cb4e8421e0bdccfba123df471"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 382910378064375906f6740d4b8817c751e8fad9b905a7d098b4cc39a3b19524
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

173
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
    "id": 450,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/f384919190b085e4eb77fba7e7554b0ca419ef14.jpg",
    "university_id": null,
    "fields_of_study": [
      173
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-16T17:23:29.016Z",
    "updated_at": "2016-11-16T17:23:29.240Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/418451baffccf851f1f7b49031e7723918a0f3b5.jpg",
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

173
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 382910378064375906f6740d4b8817c751e8fad9b905a7d098b4cc39a3b19524"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer e6484986e55811a9c9011d6c8978e0c485177051387b89561f0542268fedd077
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
      "id": 7,
      "bookmarkable_id": 132,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 133,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 134,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6484986e55811a9c9011d6c8978e0c485177051387b89561f0542268fedd077"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b9b6c7f5f4982effacb64a362cc6b356317026dec54230f3b876392595f83bc9
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
      "company_id": 20,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 21,
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
	-H "Authorization: Bearer b9b6c7f5f4982effacb64a362cc6b356317026dec54230f3b876392595f83bc9"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 59156a3899f681908ff743561b4d6213d8bd586d7770212fc3cdf581a50131d3
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
      "company_id": 16,
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
	-H "Authorization: Bearer 59156a3899f681908ff743561b4d6213d8bd586d7770212fc3cdf581a50131d3"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 5519209a591809f5d2dcb7210d757fcfa694c5ecf71458895fd403a51646fcb9
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
      "creator_id": 979,
      "id": 315,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-243",
      "html_url": "https://goskive.com/course/mit-course-243",
      "slug": "mit-course-243",
      "university_id": 300,
      "additional_university_ids": [

      ],
      "discipline_id": 328,
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
      "updated_at": "2016-11-16T17:24:14.345Z",
      "shortname": "mit-course-243",
      "topic_id": 327,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 243",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 980,
      "id": 316,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-244",
      "html_url": "https://goskive.com/course/mit-course-244",
      "slug": "mit-course-244",
      "university_id": 301,
      "additional_university_ids": [

      ],
      "discipline_id": 329,
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
      "updated_at": "2016-11-16T17:24:14.423Z",
      "shortname": "mit-course-244",
      "topic_id": 328,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 244",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5519209a591809f5d2dcb7210d757fcfa694c5ecf71458895fd403a51646fcb9"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer fc73a4ff93b3f289a387619aee47a50f554031c59aaa1a9807726de8b017e578
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
        "created_at": "2016-11-16T17:23:03.654Z",
        "updated_at": "2016-11-16T17:23:03.654Z",
        "file_url": "memory://c01fd2fa94150b81546fe1f16a9ef4c3.pdf",
        "course_id": 57,
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
        "created_at": "2016-11-16T17:23:03.743Z",
        "updated_at": "2016-11-16T17:23:03.743Z",
        "file_url": "memory://2be6fe1ce59fa907e56bcb8baa3de43b.pdf",
        "course_id": 58,
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
        "created_at": "2016-11-16T17:23:03.825Z",
        "updated_at": "2016-11-16T17:23:03.825Z",
        "file_url": "memory://c2bc6ede852200022014a4032f71cdc1.pdf",
        "course_id": 59,
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
	-H "Authorization: Bearer fc73a4ff93b3f289a387619aee47a50f554031c59aaa1a9807726de8b017e578"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer c4dfdcd4411842f592266de2daf0c4b55f4aff10af37e3f3ade00c8cc7fc91e0
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
        "updated_at": "2016-11-16T17:24:04.084Z"
      },
      "created_at": "2016-11-16T17:24:04.088Z",
      "updated_at": "2016-11-16T17:24:04.088Z",
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
        "updated_at": "2016-11-16T17:24:04.095Z"
      },
      "created_at": "2016-11-16T17:24:04.098Z",
      "updated_at": "2016-11-16T17:24:04.098Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4dfdcd4411842f592266de2daf0c4b55f4aff10af37e3f3ade00c8cc7fc91e0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 119a0ddf74b80e16b81524df93a4f6f45401908388b439de7f15ac770cc51a03
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
        "updated_at": "2016-11-16T17:24:03.917Z"
      },
      "created_at": "2016-11-16T17:24:03.920Z",
      "updated_at": "2016-11-16T17:24:03.920Z",
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
        "updated_at": "2016-11-16T17:24:03.935Z"
      },
      "created_at": "2016-11-16T17:24:03.938Z",
      "updated_at": "2016-11-16T17:24:03.938Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 119a0ddf74b80e16b81524df93a4f6f45401908388b439de7f15ac770cc51a03"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 298adc85fc5f8c9445e56b14b156c270446890955613365c63544e25acaf9d27
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
      "id": 6,
      "created_at": "2016-11-16T17:23:09.665Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 53,
      "updated_at": "2016-11-16T17:23:09.763Z",
      "author_id": "187",
      "thread_subject_id": "71",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 7,
      "created_at": "2016-11-16T17:23:09.753Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 54,
      "updated_at": "2016-11-16T17:23:09.766Z",
      "author_id": "190",
      "thread_subject_id": "72",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-11-16T17:23:10.149Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-11-16T17:23:10.149Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 9,
      "created_at": "2016-11-16T17:23:10.527Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-11-16T17:23:10.527Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 10,
      "created_at": "2016-11-16T17:23:10.916Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-11-16T17:23:10.916Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 11,
      "created_at": "2016-11-16T17:23:11.216Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 18,
      "updated_at": "2016-11-16T17:23:11.216Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-11-16T17:23:11.515Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 19,
      "updated_at": "2016-11-16T17:23:11.515Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 13,
      "created_at": "2016-11-16T17:23:11.805Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 20,
      "updated_at": "2016-11-16T17:23:11.805Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 298adc85fc5f8c9445e56b14b156c270446890955613365c63544e25acaf9d27"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer e56118d70eb13e19548e331f6872fad6363091582169445a717ca763e630bfd5
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-16T17:13:11.000Z"}}
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
    "created_at": "2016-11-16T17:23:11.993Z",
    "read_at": "2016-11-16T17:13:11.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 55,
    "updated_at": "2016-11-16T17:23:12.033Z",
    "author_id": "216",
    "thread_subject_id": "79",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-11-16T17:13:11.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e56118d70eb13e19548e331f6872fad6363091582169445a717ca763e630bfd5"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b8fc08718ed0b4dbccfd0b02eea8d153d53bab821b107c2bd0f3580731326770
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
      "course_id": 231,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-16T17:23:52.195Z",
      "course_published": true,
      "updated_at": "2016-11-16T17:23:52.187Z"
    },
    {
      "id": 4,
      "course_id": 232,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-16T17:23:52.276Z",
      "course_published": true,
      "updated_at": "2016-11-16T17:23:52.268Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8fc08718ed0b4dbccfd0b02eea8d153d53bab821b107c2bd0f3580731326770"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 6bba39fedf496336524afce6783c2be76b3c6752c237a1d8badc6a7b2f832432
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
    "id": 2,
    "course_id": 230,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-16T17:23:52.003Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:23:51.995Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bba39fedf496336524afce6783c2be76b3c6752c237a1d8badc6a7b2f832432"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 65c42b0e168fd73ad27bd1f3633f4f176a48fae216eb583c8ab5089101215b44
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
    "course_id": 235,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-16T17:23:52.661Z",
    "course_published": true,
    "updated_at": "2016-11-16T17:23:52.650Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65c42b0e168fd73ad27bd1f3633f4f176a48fae216eb583c8ab5089101215b44"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 23a9b0deda09d473ef248986f096989b91d4a817ebf9d9dbb500c9ad5e012183
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
      "user_id": 225
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 22,
      "user_id": 225
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 23,
      "user_id": 225
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 24,
      "user_id": 225
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23a9b0deda09d473ef248986f096989b91d4a817ebf9d9dbb500c9ad5e012183"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/73
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
    "id": 73,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 71,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 73
      },
      {
        "id": 72,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 73
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/73" -X GET \
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
      "id": 71,
      "name": "Fundamental reciprocal hardware",
      "name_translations": {
        "en": "Fundamental reciprocal hardware"
      }
    },
    {
      "id": 72,
      "name": "Face to face interactive extranet",
      "name_translations": {
        "en": "Face to face interactive extranet"
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
PATCH /v2/feedbacks/36/close
Content-Type: application/json
Authorization: Bearer 3c27e2ce768001deff3e645b05bda76f5cdde9bf44ef6cc20cfb68d1d5f8174e
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
    "id": 36,
    "user_id": 819,
    "feedbackable_id": 68,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-16T17:24:03.246Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/36/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c27e2ce768001deff3e645b05bda76f5cdde9bf44ef6cc20cfb68d1d5f8174e"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer 946484b312704c991f650b08c3e02c4ee808d86a20c85cc8a9fc9d778e5344e8
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
    "id": 12,
    "user_id": 711,
    "feedbackable_id": 63,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-16T17:23:55.928Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 946484b312704c991f650b08c3e02c4ee808d86a20c85cc8a9fc9d778e5344e8"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/15
Content-Type: application/json
Authorization: Bearer ff6611c7f7b10ec4fa65d6fa38abfdcc1cbba1f9a726235658270a759d66dca7
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
    "id": 15,
    "user_id": 726,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:23:56.848Z",
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
curl "api.goskive.com/v2/feedbacks/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff6611c7f7b10ec4fa65d6fa38abfdcc1cbba1f9a726235658270a759d66dca7"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/11/fix
Content-Type: application/json
Authorization: Bearer d022fec20468efa02e689b6843b190daa1ec5224c001c3c708e4dd421c9dd8b2
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
curl "api.goskive.com/v2/feedbacks/11/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d022fec20468efa02e689b6843b190daa1ec5224c001c3c708e4dd421c9dd8b2"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/14/fix
Content-Type: application/json
Authorization: Bearer a9b039fa6c6737fde7354ada2742001a45852689c343ba4c2581d77dd664637f
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
curl "api.goskive.com/v2/feedbacks/14/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9b039fa6c6737fde7354ada2742001a45852689c343ba4c2581d77dd664637f"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/38/close
Content-Type: application/json
Authorization: Bearer f379b8b09a62632a882732d81bf8e9e2c62b8f7b885702692017ed54ee16c9c0
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
curl "api.goskive.com/v2/feedbacks/38/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f379b8b09a62632a882732d81bf8e9e2c62b8f7b885702692017ed54ee16c9c0"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/16
Content-Type: application/json
Authorization: Bearer 5642656d6730f3e9b192f4c36adda13c06fa86651ef3c13c8af70744cea9d00d
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
    "id": 16,
    "user_id": 731,
    "feedbackable_id": 67,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:23:57.123Z",
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
curl "api.goskive.com/v2/feedbacks/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5642656d6730f3e9b192f4c36adda13c06fa86651ef3c13c8af70744cea9d00d"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer 66500670351d1b7340934d3a8e97de090a928b88a96d4f13c081710e154dacaa
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
	-H "Authorization: Bearer 66500670351d1b7340934d3a8e97de090a928b88a96d4f13c081710e154dacaa"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer ed194ca6ba3c68cf82291221019898ca131f7f2d53ce9ae6fdcc19cd3a5249b1
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed194ca6ba3c68cf82291221019898ca131f7f2d53ce9ae6fdcc19cd3a5249b1"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer bc10afb2ba595640034174a48354a602bfba26815f239f68af1efbff63d2635b
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc10afb2ba595640034174a48354a602bfba26815f239f68af1efbff63d2635b"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/8
Content-Type: application/json
Authorization: Bearer 724abb49ea31cc32b9f8132f42939a2f20e8b51fe84eff10f85abdc8c03ec152
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/77d2da54e7638af6209d91ac2af89e9c.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161116%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161116T172337Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a6af6a183d883ea6cd26eaead8d1993f9f6c0938b038b37e20583fe85b07567c",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 724abb49ea31cc32b9f8132f42939a2f20e8b51fe84eff10f85abdc8c03ec152"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/9/preview
Content-Type: application/json
Authorization: Bearer b2776cd7fdcb144a797b04ceb678e4a4690d0781117b27291cb2b29cdc77340e
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/e9f163a58aefc750aa0783068ac9807a.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161116%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161116T172338Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8ecbb5e50b7298a7fae4525c74ab7b7df44c5fa277ea0a137525446559600f81",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/9/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2776cd7fdcb144a797b04ceb678e4a4690d0781117b27291cb2b29cdc77340e"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer f61c924733cf930a8730fda92b343dd973a7f4dd5562589611884e13d5eba13d
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
      "id": 552,
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
      "created_at": "2016-11-16T17:23:38.580Z",
      "updated_at": "2016-11-16T17:23:38.580Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-16T17:23:38.650Z",
    "updated_at": "2016-11-16T17:23:38.650Z",
    "course_id": 198,
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
	-H "Authorization: Bearer f61c924733cf930a8730fda92b343dd973a7f4dd5562589611884e13d5eba13d"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/22/matched_courses?required_cu_count=2
Authorization: Bearer b9bcd173cff356f5b655803bacd772bf7ab04e65937881159292a0cddceaef05
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
      "creator_id": 648,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-38b3d01b-15c8-4db0-b5ef-71651bef0e8b",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-38b3d01b-15c8-4db0-b5ef-71651bef0e8b",
      "slug": "mit-the-great-british-bake-off-38b3d01b-15c8-4db0-b5ef-71651bef0e8b",
      "university_id": 214,
      "additional_university_ids": [

      ],
      "discipline_id": 239,
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
      "chapters_updated_at": "2016-11-16T17:23:48.931Z",
      "updated_at": "2016-11-16T17:23:51.661Z",
      "shortname": "mit-the-great-british-bake-off-38b3d01b-15c8-4db0-b5ef-71651bef0e8b",
      "topic_id": 238,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 643,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 213,
      "additional_university_ids": [

      ],
      "discipline_id": 238,
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
      "chapters_updated_at": "2016-11-16T17:23:48.931Z",
      "updated_at": "2016-11-16T17:23:51.090Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 237,
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
curl "api.goskive.com/v2/files/22/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer b9bcd173cff356f5b655803bacd772bf7ab04e65937881159292a0cddceaef05"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/19/download
Content-Type: application/json
Authorization: Bearer a6fb59580b9d7eca0d69d757d32abe83c6db295c5b479abddaefad9df8fc7f04
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6fb59580b9d7eca0d69d757d32abe83c6db295c5b479abddaefad9df8fc7f04"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/15/report
Content-Type: application/json
Authorization: Bearer 8724da8a493926f16473debcc0f36b4706727cb11995e63c35b9ff09ef7f57f9
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8724da8a493926f16473debcc0f36b4706727cb11995e63c35b9ff09ef7f57f9"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/20/bookmark
Content-Type: application/json
Authorization: Bearer 2b4faed42f7f17c4177dbb8be4c04c01905d9415183c3f0682a64589fd4f2c8a
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b4faed42f7f17c4177dbb8be4c04c01905d9415183c3f0682a64589fd4f2c8a"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/10/upvote
Content-Type: application/json
Authorization: Bearer 65318252cad69510d8dc8b382094763f426766d14fe5a2dd41dfe77eee0bf297
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
	-H "Authorization: Bearer 65318252cad69510d8dc8b382094763f426766d14fe5a2dd41dfe77eee0bf297"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/2/comments
Content-Type: application/json
Authorization: Bearer a8144529fcb97f0e71822ace54bec563844cac0e5eae19e9ddc07694be90d8e1
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
    "author_id": 112,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:23:01.705Z",
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
curl "api.goskive.com/v2/flashcards/2/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8144529fcb97f0e71822ace54bec563844cac0e5eae19e9ddc07694be90d8e1"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/comments
Content-Type: application/json
Authorization: Bearer 234b589df8ec33fe5f010063fcf33b4418bcab7a29df943af0d349b9ec982352
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
    "author_id": 109,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:23:01.368Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 109,
      "feedbackable_id": 1,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:01.364Z",
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
curl "api.goskive.com/v2/flashcards/1/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 234b589df8ec33fe5f010063fcf33b4418bcab7a29df943af0d349b9ec982352"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/5/comments
Content-Type: application/json
Authorization: Bearer cf7311e337e56a708ec71aa04e5d0f4f260d628481c64910a79ff7b00952870b
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
      "author_id": 124,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:02.349Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 125,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:02.364Z",
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
curl "api.goskive.com/v2/flashcards/5/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf7311e337e56a708ec71aa04e5d0f4f260d628481c64910a79ff7b00952870b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/3/comments
Content-Type: application/json
Authorization: Bearer c57171a493c9ca3546a03d46b07b85091c6c4e45c465f9b3d80e6204c579c590
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
curl "api.goskive.com/v2/flashcards/3/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c57171a493c9ca3546a03d46b07b85091c6c4e45c465f9b3d80e6204c579c590"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/7/feedbacks
Content-Type: application/json
Authorization: Bearer c8b595a2133f1a7ca4bda4a88ef917ec82b27441c6a29e7528cd29a4c4b161cc
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
    "user_id": 244,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:23:14.805Z",
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
curl "api.goskive.com/v2/flashcards/7/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8b595a2133f1a7ca4bda4a88ef917ec82b27441c6a29e7528cd29a4c4b161cc"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/13/feedbacks
Content-Type: application/json
Authorization: Bearer cbeb1d81e83371179ba60894640ba279a0500585a319ced23629597cafc5acc6
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
      "id": 10,
      "user_id": 276,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:16.012Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 275,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:16.002Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/13/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbeb1d81e83371179ba60894640ba279a0500585a319ced23629597cafc5acc6"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/27/votes
Content-Type: application/json
Authorization: Bearer a40c459c302e5a3a8559fc29d1b1ea1196fc7a70337093075c159cb9f8434b4a
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 444
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 443
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 27,
      "user_id": 442
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/27/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a40c459c302e5a3a8559fc29d1b1ea1196fc7a70337093075c159cb9f8434b4a"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/95/republish
Content-Type: application/json
Authorization: Bearer 4056cb32c59c3574ef16b770a22e43774dd89c5c6a0a446376e54ee612838393
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
curl "api.goskive.com/v2/flashcards/95/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4056cb32c59c3574ef16b770a22e43774dd89c5c6a0a446376e54ee612838393"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/bookmark
Content-Type: application/json
Authorization: Bearer 0c3a015f55881bd61c89bab3e39411ba040dfeb4a772678c5cce5f989156dec1
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c3a015f55881bd61c89bab3e39411ba040dfeb4a772678c5cce5f989156dec1"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/93
Content-Type: application/json
Authorization: Bearer 161b69c358c13db4289a1d43790c98c4c9ac1af5a5a708a60ef084451949bad1
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/93" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 161b69c358c13db4289a1d43790c98c4c9ac1af5a5a708a60ef084451949bad1"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/75/downvote
Content-Type: application/json
Authorization: Bearer 3e26510f2bb5e396119619574c0c746b8538fa0259473d7b2d7f842ddf2e1702
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e26510f2bb5e396119619574c0c746b8538fa0259473d7b2d7f842ddf2e1702"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/76
Content-Type: application/json
Authorization: Bearer ec6bebb7cc734c4e6f8c8f7e97d78e9969fa4baa13c0f77539d9e9f969f37272
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
    "id": 76,
    "obfuscated_id": "oK0h_-4yfUk",
    "author_id": 912,
    "chapter_id": 176,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:24:10.783Z",
    "created_at": "2016-11-16T17:24:10.783Z",
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
curl "api.goskive.com/v2/flashcards/76" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec6bebb7cc734c4e6f8c8f7e97d78e9969fa4baa13c0f77539d9e9f969f37272"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/92/report
Content-Type: application/json
Authorization: Bearer 3d20ccd0e903dcde9b460d11601535c22d2cb93dc5b7f10d3c631d6166736bc8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/92/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d20ccd0e903dcde9b460d11601535c22d2cb93dc5b7f10d3c631d6166736bc8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/73/bookmark
Content-Type: application/json
Authorization: Bearer 9ca162abfe70c867e9ec14c8f509051516293d366969073ab8e772116569f744
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ca162abfe70c867e9ec14c8f509051516293d366969073ab8e772116569f744"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/72/upvote
Content-Type: application/json
Authorization: Bearer bca0360572ed6169b17a59fe0dc790db8eb9d79ddb4a57fb96525b9314347a0a
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bca0360572ed6169b17a59fe0dc790db8eb9d79ddb4a57fb96525b9314347a0a"
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
    "key": "cache/abe794bc43c8489a460df95698d447a7.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xNlQxODoyMzowMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2FiZTc5NGJjNDNjODQ4OWE0NjBkZjk1Njk4ZDQ0N2E3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMTZUMTcyMzAyWiJ9XX0=",
    "x-amz-credential": "FAKE/20161116/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161116T172302Z",
    "x-amz-signature": "592de2454cbabe477bbbb3b75f52c5732982a832b0f53987abc01fdae3e2def1"
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
Authorization: Bearer 78fcf9383acb639bf47f63d49500a7d9a34798426bf24b611c6002f8c80544de
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
	-H "Authorization: Bearer 78fcf9383acb639bf47f63d49500a7d9a34798426bf24b611c6002f8c80544de"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 33bbce51045ab7c15e6aa4f16a30f6659d55a99a0729ab699cf54ed785893274
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
	-H "Authorization: Bearer 33bbce51045ab7c15e6aa4f16a30f6659d55a99a0729ab699cf54ed785893274"
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
{"password":{"reset_password_token":"s3yFfXNoCCtY2cicTjk3","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 985,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-16T17:24:15.871Z",
  "updated_at": "2016-11-16T17:24:16.009Z",
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
  "audit_id": 5736
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"s3yFfXNoCCtY2cicTjk3","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer ac4626c3a9f72482fa328a642ceefd5687813d4b0ad69966d3b31a4a3645fb1e
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
    "id": 50,
    "author_id": 174,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:23:08.636Z",
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
curl "api.goskive.com/v2/questions/12/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac4626c3a9f72482fa328a642ceefd5687813d4b0ad69966d3b31a4a3645fb1e"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/10/comments
Content-Type: application/json
Authorization: Bearer b8a2f1b49b6b8195eca2a2800da586cdb22ad71517d89f3bceb6a0dd1f643dfd
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
    "id": 49,
    "author_id": 168,
    "reply_to_id": null,
    "created_at": "2016-11-16T17:23:07.883Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 2,
      "user_id": 168,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:23:07.880Z",
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
curl "api.goskive.com/v2/questions/10/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8a2f1b49b6b8195eca2a2800da586cdb22ad71517d89f3bceb6a0dd1f643dfd"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/14/comments
Content-Type: application/json
Authorization: Bearer c66295f4d48f8a8306bb98ca1a68dc78e3b0be5be0bb9456cdbbd8f8475a0e0d
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
      "id": 51,
      "author_id": 183,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:09.398Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 184,
      "reply_to_id": null,
      "created_at": "2016-11-16T17:23:09.414Z",
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
	-H "Authorization: Bearer c66295f4d48f8a8306bb98ca1a68dc78e3b0be5be0bb9456cdbbd8f8475a0e0d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/11/comments
Content-Type: application/json
Authorization: Bearer 7142ee9de60f097f738d99641c0e80083a5dc08948a209a3bf2d9962c2b548cf
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
curl "api.goskive.com/v2/questions/11/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7142ee9de60f097f738d99641c0e80083a5dc08948a209a3bf2d9962c2b548cf"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/121/feedbacks
Content-Type: application/json
Authorization: Bearer 034ae9276bf48b517604e140de6029d0d4b5d27b36dfdd54fe13927b6a7252ab
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
    "id": 39,
    "user_id": 841,
    "feedbackable_id": 121,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-16T17:24:05.062Z",
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
curl "api.goskive.com/v2/questions/121/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 034ae9276bf48b517604e140de6029d0d4b5d27b36dfdd54fe13927b6a7252ab"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/126/feedbacks
Content-Type: application/json
Authorization: Bearer 0496858718a29784c932a6989ed5bd4a4265c32fa8b9e3c6ae2b703315b65ee0
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
      "id": 44,
      "user_id": 862,
      "feedbackable_id": 126,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:06.904Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 861,
      "feedbackable_id": 126,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-16T17:24:06.894Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/126/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0496858718a29784c932a6989ed5bd4a4265c32fa8b9e3c6ae2b703315b65ee0"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/32/votes
Content-Type: application/json
Authorization: Bearer 64ab820a0e9bad707488030d9660ab6a7c3c1e6efa7d630eafa0cdb9b0ad973c
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
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 357
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 356
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 355
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/32/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64ab820a0e9bad707488030d9660ab6a7c3c1e6efa7d630eafa0cdb9b0ad973c"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/56/republish
Content-Type: application/json
Authorization: Bearer 44e4fa53e3b0816126af450d928b97e3409a753aa46f0f7d4e40c3d7690badec
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
curl "api.goskive.com/v2/questions/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44e4fa53e3b0816126af450d928b97e3409a753aa46f0f7d4e40c3d7690badec"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/58/bookmark
Content-Type: application/json
Authorization: Bearer 13b351b9ffff12d388c35d783a3f4a75693934297d6714583e61b9c30a702cf7
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/58/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13b351b9ffff12d388c35d783a3f4a75693934297d6714583e61b9c30a702cf7"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/59
Content-Type: application/json
Authorization: Bearer 7e40aabfbac210004fca6c5d5adb226704edaaca2f271dd6e905dca2d98f8698
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e40aabfbac210004fca6c5d5adb226704edaaca2f271dd6e905dca2d98f8698"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/40/downvote
Content-Type: application/json
Authorization: Bearer e640622a6119dc018b6d5d03eda28b2841c558ca900c57be83aba7974b8e2c02
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/40/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e640622a6119dc018b6d5d03eda28b2841c558ca900c57be83aba7974b8e2c02"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/39
Content-Type: application/json
Authorization: Bearer cc174f74a4bcb91d81eae8413a728a65b92db613b3b1b565a29386b21421b62d
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 460,
    "chapter_id": 81,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:30.982Z",
    "created_at": "2016-11-16T17:23:30.867Z",
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
        "id": 81,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 82,
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
curl "api.goskive.com/v2/questions/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc174f74a4bcb91d81eae8413a728a65b92db613b3b1b565a29386b21421b62d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/36/report
Content-Type: application/json
Authorization: Bearer c445d3bb9b5515b2d590b172e42620e23b1f215d0de9104b682975fb814f3a4d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/36/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c445d3bb9b5515b2d590b172e42620e23b1f215d0de9104b682975fb814f3a4d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/60/bookmark
Content-Type: application/json
Authorization: Bearer 4d69e08f62e2b5ca606f165b316a527d2fb1cef19255c55960237c10cc4fcf9e
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/60/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d69e08f62e2b5ca606f165b316a527d2fb1cef19255c55960237c10cc4fcf9e"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/37
Content-Type: application/json
Authorization: Bearer d63adfd37e1a3bd5bbd92c67781928811f2e9378b8daa9831b801389768a1520
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":37,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-16T17:23:29.957Z","updated_at":"2016-11-16T17:23:30.071Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":79,"author_id":454,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 37,
    "obfuscated_id": "95m_4XdR9PU",
    "author_id": 454,
    "chapter_id": 79,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-16T17:23:30.178Z",
    "created_at": "2016-11-16T17:23:29.957Z",
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
    "question": "{\"id\"=>37, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-16T17:23:29.957Z\", \"updated_at\"=>\"2016-11-16T17:23:30.071Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>79, \"author_id\"=>454, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 76,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 77,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 78,
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
curl "api.goskive.com/v2/questions/37" -d '{"question":{"question":{"id":37,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-16T17:23:29.957Z","updated_at":"2016-11-16T17:23:30.071Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":79,"author_id":454,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d63adfd37e1a3bd5bbd92c67781928811f2e9378b8daa9831b801389768a1520"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/38/upvote
Content-Type: application/json
Authorization: Bearer 21092b407dc2a953b39644bd263462e41ff979eb80f4faa1b5f74b33560fb199
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/38/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21092b407dc2a953b39644bd263462e41ff979eb80f4faa1b5f74b33560fb199"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 24e464bd5f41915099bef1a65933a070082aebadeaeabd00aa3161b1af63030e
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
      "creator_id": 1,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "discipline_id": 2,
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
      "updated_at": "2016-11-16T17:22:55.507Z",
      "shortname": "mit-pizza-201",
      "topic_id": 2,
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
	-H "Authorization: Bearer 24e464bd5f41915099bef1a65933a070082aebadeaeabd00aa3161b1af63030e"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 85379161edb5b3dac6c1deb4888e574f7f21333bc0330aee55a77eb9bf221833
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
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-4",
      "html_url": "https://goskive.com/university/uni-4",
      "slug": "uni-4",
      "name": "National School of Pizza",
      "short_name": "Uni 4",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:22:55.951Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-3",
      "html_url": "https://goskive.com/university/uni-3",
      "slug": "uni-3",
      "name": "National School of Pastry",
      "short_name": "Uni 3",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0178e4c1b8a1e0379f3158851027049f94ddc463.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51e7a1f572cf9347372a35d5e9ae2cc89f48eb30.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:22:55.936Z",
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
	-H "Authorization: Bearer 85379161edb5b3dac6c1deb4888e574f7f21333bc0330aee55a77eb9bf221833"
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
      "id": 325,
      "name": "Fundamental multi-tasking policy",
      "name_translations": {
        "en": "Fundamental multi-tasking policy"
      },
      "discipline_id": 326
    },
    {
      "id": 326,
      "name": "Robust context-sensitive core",
      "name_translations": {
        "en": "Robust context-sensitive core"
      },
      "discipline_id": 327
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
GET /v2/topics/324
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
    "id": 324,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 325
  }
}
```



```shell
curl "api.goskive.com/v2/topics/324" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 83a21929f15a0949c033a063c35af35b23937aba1a3942a9b1751e03ba994739
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
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-94",
      "html_url": "https://goskive.com/university/uni-94",
      "slug": "uni-94",
      "name": "University 79",
      "short_name": "Uni 94",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3587f09ccbcc321f7f63c35b7e737171f83e68af.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a71c5926eacc7efc335b877c4910cd8c4e3565b7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:23:16.100Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-95",
      "html_url": "https://goskive.com/university/uni-95",
      "slug": "uni-95",
      "name": "University 80",
      "short_name": "Uni 95",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dc8f2469ecddd5af6505d9db2042b45f53ad683e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c9a133dca397548adb89a35bebfdaee19823cf8d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:23:16.115Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-93",
      "html_url": "https://goskive.com/university/uni-93",
      "slug": "uni-93",
      "name": "University 78",
      "short_name": "Uni 93",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b4bec54a7f7cd323d36919c55d64b5b5c335955f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c663f9415e0a293c066cadc042878bf2842ce887.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-16T17:23:16.085Z",
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
	-H "Authorization: Bearer 83a21929f15a0949c033a063c35af35b23937aba1a3942a9b1751e03ba994739"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer abeb68333ba7b40bf2fa3d3c4ba7439c6a6ba6dd566e942963f370e12673ecf3
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
    "id": 96,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dd45b8e274d1d0e55b5afff67d218d948442eaca.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ed3aed27ec2abf05787537f4c8572fb9080bbebf.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-16T17:23:16.224Z",
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
	-H "Authorization: Bearer abeb68333ba7b40bf2fa3d3c4ba7439c6a6ba6dd566e942963f370e12673ecf3"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 08d26db033fac0d45ee75861234c4ff1d66a7bf4ff02a5d6e2d1373c89a7eb10
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":132,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 326,
    "id": 130,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 114,
    "additional_university_ids": [

    ],
    "discipline_id": 133,
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
    "chapters_updated_at": "2016-11-16T17:23:20.550Z",
    "updated_at": "2016-11-16T17:23:20.696Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 42,
        "updated_at": "2016-11-16T17:23:20.650Z",
        "course_id": 130,
        "author_id": 326,
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
        "id": 43,
        "updated_at": "2016-11-16T17:23:20.668Z",
        "course_id": 130,
        "author_id": 326,
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
        "id": 44,
        "updated_at": "2016-11-16T17:23:20.685Z",
        "course_id": 130,
        "author_id": 326,
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
    "topic_id": 132,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":132,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08d26db033fac0d45ee75861234c4ff1d66a7bf4ff02a5d6e2d1373c89a7eb10"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8c7a1136aa46729aadab84c9869c6b56b5666d7f72cfbc04dbf753c5dcbe60cc
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":133,"published":false}}
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
    "creator_id": 327,
    "id": 131,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "discipline_id": 134,
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
    "updated_at": "2016-11-16T17:23:20.893Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 133,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":133,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c7a1136aa46729aadab84c9869c6b56b5666d7f72cfbc04dbf753c5dcbe60cc"
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
      "creator_id": 285,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-81",
      "html_url": "https://goskive.com/course/fu-course-81",
      "slug": "fu-course-81",
      "university_id": 99,
      "additional_university_ids": [

      ],
      "discipline_id": 98,
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
      "updated_at": "2016-11-16T17:23:16.800Z",
      "shortname": "fu-course-81",
      "topic_id": 97,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 81",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 285,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-82",
      "html_url": "https://goskive.com/course/fu-course-82",
      "slug": "fu-course-82",
      "university_id": 99,
      "additional_university_ids": [

      ],
      "discipline_id": 99,
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
      "chapters_updated_at": "2016-11-16T17:23:16.664Z",
      "updated_at": "2016-11-16T17:23:17.117Z",
      "shortname": "fu-course-82",
      "topic_id": 98,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 82",
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
Authorization: Bearer 6a59931207ddb5542d96d14a8eda296042dc53132c3bfaafb67bc7202bb736ad
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
      "creator_id": 302,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-97",
      "html_url": "https://goskive.com/course/fu-course-97",
      "slug": "fu-course-97",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 114,
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
      "updated_at": "2016-11-16T17:23:18.445Z",
      "shortname": "fu-course-97",
      "topic_id": 113,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 97",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 302,
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-98",
      "html_url": "https://goskive.com/course/fu-course-98",
      "slug": "fu-course-98",
      "university_id": 105,
      "additional_university_ids": [

      ],
      "discipline_id": 115,
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
      "chapters_updated_at": "2016-11-16T17:23:18.297Z",
      "updated_at": "2016-11-16T17:23:18.766Z",
      "shortname": "fu-course-98",
      "topic_id": 114,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a59931207ddb5542d96d14a8eda296042dc53132c3bfaafb67bc7202bb736ad"
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
      "creator_id": 290,
      "id": 99,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-85",
      "html_url": "https://goskive.com/course/fu-course-85",
      "slug": "fu-course-85",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "discipline_id": 102,
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
      "updated_at": "2016-11-16T17:23:17.308Z",
      "shortname": "fu-course-85",
      "topic_id": 101,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 85",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 290,
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-86",
      "html_url": "https://goskive.com/course/fu-course-86",
      "slug": "fu-course-86",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "discipline_id": 103,
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
      "updated_at": "2016-11-16T17:23:17.348Z",
      "shortname": "fu-course-86",
      "topic_id": 102,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 86",
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
Authorization: Bearer 257e8979a05c617959a2e699183ebd688596fa88fee8c88b54c1f607896c2020
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
      "creator_id": 309,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-101",
      "html_url": "https://goskive.com/course/fu-course-101",
      "slug": "fu-course-101",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "discipline_id": 118,
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
      "updated_at": "2016-11-16T17:23:19.034Z",
      "shortname": "fu-course-101",
      "topic_id": 117,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 101",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 309,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-102",
      "html_url": "https://goskive.com/course/fu-course-102",
      "slug": "fu-course-102",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "discipline_id": 119,
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
      "updated_at": "2016-11-16T17:23:19.073Z",
      "shortname": "fu-course-102",
      "topic_id": 118,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 102",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 257e8979a05c617959a2e699183ebd688596fa88fee8c88b54c1f607896c2020"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer b2d71a25d06cf1964e12ee3fb14d9f42afc4f7886398ef516d4c53aa0af5ee2e
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
  "id": 329,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-16T17:23:21.134Z",
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
	-H "Authorization: Bearer b2d71a25d06cf1964e12ee3fb14d9f42afc4f7886398ef516d4c53aa0af5ee2e"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/533
Content-Type: application/json
Authorization: Bearer a4e4ebe4dda7325efadd3a5137f3230dfaa92a0cb807f7000839d684cda271ef
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
    "id": 533,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 176,
    "fields_of_study": [
      199,
      200
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-16T17:23:37.742Z",
    "updated_at": "2016-11-16T17:23:37.742Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/533" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4e4ebe4dda7325efadd3a5137f3230dfaa92a0cb807f7000839d684cda271ef"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/531
Content-Type: application/json
Authorization: Bearer 26e2d81b7cf2892bc9a1fad5b3b627c63aee7247fc5aa306cc1fb381a3d15140
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
    "id": 531,
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
    "created_at": "2016-11-16T17:23:37.592Z",
    "updated_at": "2016-11-16T17:23:37.592Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/531" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26e2d81b7cf2892bc9a1fad5b3b627c63aee7247fc5aa306cc1fb381a3d15140"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/20
Content-Type: application/json
Authorization: Bearer 249abce3fba5335b33440e2b37484d6885e79cfdfe3744f91ac023f046f20fa6
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 249abce3fba5335b33440e2b37484d6885e79cfdfe3744f91ac023f046f20fa6"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/19
Content-Type: application/json
Authorization: Bearer 46f83cd6ebe69eab06b057a6f0f8d7acfcc2c8b841304ebcdec09c5f8062c679
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
    "id": 19,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 129,
    "user_id": 877
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46f83cd6ebe69eab06b057a6f0f8d7acfcc2c8b841304ebcdec09c5f8062c679"
```
