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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5cc35f3e129f92324456e79282f8389a0528022023240fe2109d4ca6041b3721","client_secret":"2d9eb80ad57ab8f3fabbc393ae738607957405a241b62436c061a2d0d526e965"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"5cc35f3e129f92324456e79282f8389a0528022023240fe2109d4ca6041b3721","client_secret":"2d9eb80ad57ab8f3fabbc393ae738607957405a241b62436c061a2d0d526e965"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OGUwNTA3ZGYzM2IyN2JhYTk2ZGM0YjIwY2U3ZDAwMWJkZGYyMWZjYTljY2Jm
YjY4MWNhZTQyOWFkYWNlMmM3MDo3NmNhZDQxNzYzYWU3MzU1Zjg1ZjZlOGRm
MjBiMjM0YTc5YTUxODFjYWJkYjk0ZjQ1NWQ5NTI2NDhjZjY1YWM5

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
	-u 8e0507df33b27baa96dc4b20ce7d001bddf21fca9ccbfb681cae429adace2c70:76cad41763ae7355f85f6e8df20b234a79a5181cabdb94f455d952648cf65ac9
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"bf2cc158b6e3b7c19ec9da78a7f980dc38750fe59e61e981477c9f9ab9c9a7a0","client_secret":"b2baa159a2da7389866edd970d4020a7bb1fd1e73f4f146836dba3d8b4e793f1"}
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
  "access_token": "1326617943da72abd7a03cc4b4a632dd1c60682d13d6f55253468c1f3e00357b",
  "token_type": "bearer",
  "created_at": 1481221683
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"bf2cc158b6e3b7c19ec9da78a7f980dc38750fe59e61e981477c9f9ab9c9a7a0","client_secret":"b2baa159a2da7389866edd970d4020a7bb1fd1e73f4f146836dba3d8b4e793f1"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZTA4M2UzZGQ1MWI3ZWU5N2Y2ODg5MjQyZjBhN2I5MjNkNmQ1NjYzNTIzYmY3
NmViZDIzMmYyYWUxZmRiNmZlYjo3YjdkZWJmOTY0ZWNiMDE0ZTRjOWI5NDY3
NjI4MmM5NDI0YjExNzg2MDY1NmZmZGU0NWExMzdmYzAyMzZkNzQx

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
  "access_token": "8bc8db401b440cf0301f9e018889355ae0921d484f8394345d45923908db9465",
  "token_type": "bearer",
  "created_at": 1481221683
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u e083e3dd51b7ee97f6889242f0a7b923d6d5663523bf76ebd232f2ae1fdb6feb:7b7debf964ecb014e4c9b94676282c9424b117860656ffde45a137fc0236d741
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
{"grant_type":"client_credentials","client_id":"94e0237fae7ef4b3d309aff53743a27d9fa86134c8cb08915a407633553176ae","client_secret":"2c61c14d4d0389a1100367710c6ab791aa64ddda8e380e10d339a4f58cc76e21"}
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
  "access_token": "6971b5b3925607072a9aaf6dbee68555fdb06de11418f558173c48e9afa80d5f",
  "token_type": "bearer",
  "created_at": 1481221683
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"94e0237fae7ef4b3d309aff53743a27d9fa86134c8cb08915a407633553176ae","client_secret":"2c61c14d4d0389a1100367710c6ab791aa64ddda8e380e10d339a4f58cc76e21"}' -X POST \
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
Authorization: Bearer 5a7cc22307bd881ac0796bc0211d9e04e2e8cf14ae4b38b3a7c71d05a7fa21c0
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
    "company_id": 39,
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
	-H "Authorization: Bearer 5a7cc22307bd881ac0796bc0211d9e04e2e8cf14ae4b38b3a7c71d05a7fa21c0"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/143/flashcards
Content-Type: application/json
Authorization: Bearer 256fe2c66f566a5e2968a575463dc687053ca00cb8ff1ef2ad7f811cb2065d6a
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":143,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "author_id": 823,
    "chapter_id": 143,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:27:49.289Z",
    "created_at": "2016-12-08T18:27:49.289Z",
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
curl "api.goskive.com/v2/chapters/143/flashcards" -d '{"flashcard":{"chapter_id":143,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 256fe2c66f566a5e2968a575463dc687053ca00cb8ff1ef2ad7f811cb2065d6a"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/141/flashcards
Content-Type: application/json
Authorization: Bearer bee0e561231c998117a0a6e5dbe8fc50e6f1656bc50fbbe8dd310803153cccec
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 815,
      "chapter_id": 141,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:48.822Z",
      "created_at": "2016-12-08T18:27:48.822Z",
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
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 815,
      "chapter_id": 141,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:48.861Z",
      "created_at": "2016-12-08T18:27:48.861Z",
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
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 815,
      "chapter_id": 141,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:27:48.900Z",
      "created_at": "2016-12-08T18:27:48.900Z",
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
curl "api.goskive.com/v2/chapters/141/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bee0e561231c998117a0a6e5dbe8fc50e6f1656bc50fbbe8dd310803153cccec"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/19/questions
Content-Type: application/json
Authorization: Bearer 5191fbf393b0b5b6860af4d6e18a6d1874ac7c05779752bb2f883e4286b363a1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":19,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 83,
    "chapter_id": 19,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:26:50.102Z",
    "created_at": "2016-12-08T18:26:50.102Z",
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
        "id": 66,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 67,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 68,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 69,
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
curl "api.goskive.com/v2/chapters/19/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":19,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5191fbf393b0b5b6860af4d6e18a6d1874ac7c05779752bb2f883e4286b363a1"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/16/questions
Content-Type: application/json
Authorization: Bearer 59617535928935c2e1ec473256d9b3ab5a72021a38395ac9fca3ba15093e8626
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":16,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 74,
    "chapter_id": 16,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:26:48.525Z",
    "created_at": "2016-12-08T18:26:48.525Z",
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
        "id": 59,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 60,
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
curl "api.goskive.com/v2/chapters/16/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":16,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59617535928935c2e1ec473256d9b3ab5a72021a38395ac9fca3ba15093e8626"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/17/questions
Content-Type: application/json
Authorization: Bearer cb3b3a546afc94343cdb9b7a175883c190cecd2c0a7e621495d2895dacf63398
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":17,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 77,
    "chapter_id": 17,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:26:49.083Z",
    "created_at": "2016-12-08T18:26:49.083Z",
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
        "id": 61,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 62,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/17/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":17,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb3b3a546afc94343cdb9b7a175883c190cecd2c0a7e621495d2895dacf63398"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/18/questions
Content-Type: application/json
Authorization: Bearer 98676628e9eaa1b218806deac9f2c59cf9ccea4872d3ee92235b91690066b6c8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":18,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 80,
    "chapter_id": 18,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:26:49.629Z",
    "created_at": "2016-12-08T18:26:49.629Z",
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
        "id": 63,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 64,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 65,
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
curl "api.goskive.com/v2/chapters/18/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":18,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98676628e9eaa1b218806deac9f2c59cf9ccea4872d3ee92235b91690066b6c8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/21/questions
Content-Type: application/json
Authorization: Bearer 059324a01db65fed465bf8396566df73e837f4f08346912c12063103cda06908
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 89,
      "chapter_id": 21,
      "position": 30,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:26:50.990Z",
      "created_at": "2016-12-08T18:26:50.896Z",
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
          "id": 70,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 71,
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
      "author_id": 90,
      "chapter_id": 21,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:26:51.156Z",
      "created_at": "2016-12-08T18:26:51.060Z",
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
    },
    {
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 91,
      "chapter_id": 21,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:26:51.322Z",
      "created_at": "2016-12-08T18:26:51.226Z",
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
          "id": 74,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 75,
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
curl "api.goskive.com/v2/chapters/21/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 059324a01db65fed465bf8396566df73e837f4f08346912c12063103cda06908"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/49
Content-Type: application/json
Authorization: Bearer 1b208ce75e9ce0b112613f3d5ccaa4ed37331d359c1526647190fbf3a0f2032c
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
curl "api.goskive.com/v2/chapters/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b208ce75e9ce0b112613f3d5ccaa4ed37331d359c1526647190fbf3a0f2032c"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/50
Content-Type: application/json
Authorization: Bearer 73d9c41cba429a648473192277d5dee0d79bab39aa12f6cc25c955866b1264e5
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
curl "api.goskive.com/v2/chapters/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73d9c41cba429a648473192277d5dee0d79bab39aa12f6cc25c955866b1264e5"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/45
Content-Type: application/json
Authorization: Bearer 3eb131ed5a61da90627ed74b13181a17eeb66aa913fc6ee13e3b0487ff67fc67
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
curl "api.goskive.com/v2/chapters/45" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eb131ed5a61da90627ed74b13181a17eeb66aa913fc6ee13e3b0487ff67fc67"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/48
Content-Type: application/json
Authorization: Bearer f366946127ff58fb7cf5dbb7824b7967faa847bbe90d78b900380735164fad74
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f366946127ff58fb7cf5dbb7824b7967faa847bbe90d78b900380735164fad74"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/52
Content-Type: application/json
Authorization: Bearer cc3b107556069d93f9cf14d576d396d1a71eede65a03b8c2b6beb3ee4fbc9bbc
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
    "id": 52,
    "updated_at": "2016-12-08T18:27:09.252Z",
    "course_id": 113,
    "author_id": 266,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-08T18:27:08.712Z",
    "questions_updated_at": "2016-12-08T18:27:08.712Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 270,
        "chapter_id": 52,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.230Z",
        "created_at": "2016-12-08T18:27:09.230Z",
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
        "author_id": 268,
        "chapter_id": 52,
        "position": 55,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:27:09.116Z",
        "created_at": "2016-12-08T18:27:09.013Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/52" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc3b107556069d93f9cf14d576d396d1a71eede65a03b8c2b6beb3ee4fbc9bbc"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/46
Content-Type: application/json
Authorization: Bearer dabd08e84f5c4e41dfb65f5ed61db2824396fd80efc04013d8dd500708969ec3
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
    "id": 46,
    "updated_at": "2016-12-08T18:27:07.477Z",
    "course_id": 107,
    "author_id": 249,
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
curl "api.goskive.com/v2/chapters/46" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dabd08e84f5c4e41dfb65f5ed61db2824396fd80efc04013d8dd500708969ec3"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/52/replies
Content-Type: application/json
Authorization: Bearer cbd1f1350afd36b9908117bb8876f8b3c3873c339de47ec9f1ffce5ad6b0504d
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
    "author_id": 544,
    "reply_to_id": 52,
    "created_at": "2016-12-08T18:27:29.539Z",
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
	-H "Authorization: Bearer cbd1f1350afd36b9908117bb8876f8b3c3873c339de47ec9f1ffce5ad6b0504d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer c6afc602bc06fbfde0a9d91d9250c6e2bd821ae96ed9aeb5a9d83c7b8e8977ef
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
	-H "Authorization: Bearer c6afc602bc06fbfde0a9d91d9250c6e2bd821ae96ed9aeb5a9d83c7b8e8977ef"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/10
Content-Type: application/json
Authorization: Bearer 92f407686ead4dc09ad8bc0b8a2a0227c19e9c681db747af375ac7a9aba504a3
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
	-H "Authorization: Bearer 92f407686ead4dc09ad8bc0b8a2a0227c19e9c681db747af375ac7a9aba504a3"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/47/republish
Content-Type: application/json
Authorization: Bearer c59a636d04a17f538182935b4484d2aae4e60799d561dea028943a232930a01a
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
	-H "Authorization: Bearer c59a636d04a17f538182935b4484d2aae4e60799d561dea028943a232930a01a"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/11
Content-Type: application/json
Authorization: Bearer deadb2ab0850f26ef1e40b289465141d71e28be448fd69b9a25fed0bada92b0b
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer deadb2ab0850f26ef1e40b289465141d71e28be448fd69b9a25fed0bada92b0b"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/8/report
Content-Type: application/json
Authorization: Bearer 09c4a5b1bfdef43a07126029a6b6d3d5a2657df399acd538589ae202480d5fd9
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09c4a5b1bfdef43a07126029a6b6d3d5a2657df399acd538589ae202480d5fd9"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/38
Content-Type: application/json
Authorization: Bearer 8faa8a709bfaab18ef8aed85272b8f1bc275edc6a74d7435a1f4aa8715bb96ff
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
    "id": 38,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-08T18:27:49.825Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8faa8a709bfaab18ef8aed85272b8f1bc275edc6a74d7435a1f4aa8715bb96ff"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 270311e66597e7cb87202f901dd7c7f25a7c642802fbee79b411d9a60a69a063
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
      "id": 35,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:27:49.699Z"
    },
    {
      "id": 36,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:27:49.704Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:27:49.708Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 270311e66597e7cb87202f901dd7c7f25a7c642802fbee79b411d9a60a69a063"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/14/company_profiles
Content-Type: application/json
Authorization: Bearer 15fe19a51cf8120a6b9f1fd42b6503089f8e7e82a3a9157faf8aabfc25d297eb
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
curl "api.goskive.com/v2/companies/14/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 15fe19a51cf8120a6b9f1fd42b6503089f8e7e82a3a9157faf8aabfc25d297eb"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer 5b4a8f6de45e3d59795726fbd974ce1663da8823073567020992fb9559cc117a
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b4a8f6de45e3d59795726fbd974ce1663da8823073567020992fb9559cc117a"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 2b8575a7c5a18317626837c2890ef8560db07425b21d74680a60435ea2d6ea73
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
      "company_id": 7,
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b8575a7c5a18317626837c2890ef8560db07425b21d74680a60435ea2d6ea73"
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
Authorization: Bearer 1c5e1162a5e3fdf16a1134123f8459af32fa1ef20b9f1af1f5a06398c75898d9
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
	-H "Authorization: Bearer 1c5e1162a5e3fdf16a1134123f8459af32fa1ef20b9f1af1f5a06398c75898d9"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer bdc702a093f810d50386c5271e43eb4c1c9bfa7adfb5f27d27b9093690b621a3
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
    "id": 193,
    "updated_at": "2016-12-08T18:28:02.646Z",
    "course_id": 313,
    "author_id": 976,
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
	-H "Authorization: Bearer bdc702a093f810d50386c5271e43eb4c1c9bfa7adfb5f27d27b9093690b621a3"
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
      "id": 181,
      "updated_at": "2016-12-08T18:28:01.090Z",
      "course_id": 307,
      "author_id": 951,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 160",
      "position": 1
    },
    {
      "id": 182,
      "updated_at": "2016-12-08T18:28:01.115Z",
      "course_id": 307,
      "author_id": 952,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 161",
      "position": 2
    },
    {
      "id": 183,
      "updated_at": "2016-12-08T18:28:01.332Z",
      "course_id": 307,
      "author_id": 953,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T18:28:00.950Z",
      "questions_updated_at": "2016-12-08T18:28:00.950Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 162",
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
Authorization: Bearer 12f0280c2d714d4303a3624587933c290b474b0e23c2578a5184ff2221c1a334
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
      "id": 187,
      "updated_at": "2016-12-08T18:28:01.803Z",
      "course_id": 310,
      "author_id": 962,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 166",
      "position": 1
    },
    {
      "id": 188,
      "updated_at": "2016-12-08T18:28:01.827Z",
      "course_id": 310,
      "author_id": 963,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 167",
      "position": 2
    },
    {
      "id": 189,
      "updated_at": "2016-12-08T18:28:02.041Z",
      "course_id": 310,
      "author_id": 964,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T18:28:01.701Z",
      "questions_updated_at": "2016-12-08T18:28:01.701Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 168",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12f0280c2d714d4303a3624587933c290b474b0e23c2578a5184ff2221c1a334"
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
      "id": 184,
      "updated_at": "2016-12-08T18:28:01.601Z",
      "course_id": 309,
      "author_id": 958,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 163",
      "position": 1
    },
    {
      "id": 185,
      "updated_at": "2016-12-08T18:28:01.625Z",
      "course_id": 309,
      "author_id": 959,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 164",
      "position": 2
    },
    {
      "id": 186,
      "updated_at": "2016-12-08T18:28:01.650Z",
      "course_id": 309,
      "author_id": 960,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 165",
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
Authorization: Bearer 9269adb0cb185a5febbb7333ff3e359750ce76c6965f1e4139b769060fee3bfe
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
      "id": 190,
      "updated_at": "2016-12-08T18:28:02.238Z",
      "course_id": 311,
      "author_id": 969,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 169",
      "position": 1
    },
    {
      "id": 191,
      "updated_at": "2016-12-08T18:28:02.263Z",
      "course_id": 311,
      "author_id": 970,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 170",
      "position": 2
    },
    {
      "id": 192,
      "updated_at": "2016-12-08T18:28:02.287Z",
      "course_id": 311,
      "author_id": 971,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 171",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9269adb0cb185a5febbb7333ff3e359750ce76c6965f1e4139b769060fee3bfe"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0f5e8260030dc1887a73965360b191f8c01cbe76aee4d9cc43c8b07df30eee6f
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
    "course_id": 195,
    "user_id": 512,
    "updated_at": "2016-12-08T18:27:25.687Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f5e8260030dc1887a73965360b191f8c01cbe76aee4d9cc43c8b07df30eee6f"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 85a94f8e98df497393af47cbf9aecef105057ca00d6224e5a79b6dd8abf83e71
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
      "course_id": 194,
      "user_id": 508,
      "updated_at": "2016-12-08T18:27:25.461Z"
    },
    {
      "id": 4,
      "course_id": 194,
      "user_id": 509,
      "updated_at": "2016-12-08T18:27:25.476Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85a94f8e98df497393af47cbf9aecef105057ca00d6224e5a79b6dd8abf83e71"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/43/files
Content-Type: application/json
Authorization: Bearer ceab8bd75301250ba8e2bc27983a3a2020687cf4668464bf523939f2a6dc5b19
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
        "id": 138,
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
        "created_at": "2016-12-08T18:26:55.558Z",
        "updated_at": "2016-12-08T18:26:55.558Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:26:55.633Z",
      "updated_at": "2016-12-08T18:26:55.633Z",
      "course_id": 43,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 139,
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
        "created_at": "2016-12-08T18:26:55.645Z",
        "updated_at": "2016-12-08T18:26:55.645Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:26:55.655Z",
      "updated_at": "2016-12-08T18:26:55.655Z",
      "course_id": 43,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 140,
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
        "created_at": "2016-12-08T18:26:55.664Z",
        "updated_at": "2016-12-08T18:26:55.664Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:26:55.673Z",
      "updated_at": "2016-12-08T18:26:55.673Z",
      "course_id": 43,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/43/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceab8bd75301250ba8e2bc27983a3a2020687cf4668464bf523939f2a6dc5b19"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/46/files
Content-Type: application/json
Authorization: Bearer 18be5b94f59bc2295da9589a2b8b23e63bedee5531ca87cda9f761e55507d3d6
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
      "id": 147,
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
      "created_at": "2016-12-08T18:26:56.096Z",
      "updated_at": "2016-12-08T18:26:56.096Z"
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
    "created_at": "2016-12-08T18:26:56.127Z",
    "updated_at": "2016-12-08T18:26:56.127Z",
    "course_id": 46,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/46/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18be5b94f59bc2295da9589a2b8b23e63bedee5531ca87cda9f761e55507d3d6"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/45/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 2c1a02553b06f5e1eb64a385c9a11a7e0870ad210ebc8081b6ca84db75efbbf3
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
    "key": "cache/d3bd7396d926b733baa02d627a769afc.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxOToyNjo1NVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2QzYmQ3Mzk2ZDkyNmI3MzNiYWEwMmQ2MjdhNzY5YWZjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA4VDE4MjY1NVoifV19",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T182655Z",
    "x-amz-signature": "c72c1cfdf688419071440483cab90445eadc199e0501df88af951f73ed02a78b"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/45/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c1a02553b06f5e1eb64a385c9a11a7e0870ad210ebc8081b6ca84db75efbbf3"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer a1dbe701e0a58434d731c63d8495df489c7f48005c210e0c986d7a30e4317b21
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
	-H "Authorization: Bearer a1dbe701e0a58434d731c63d8495df489c7f48005c210e0c986d7a30e4317b21"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer eda2b98c810209d53240532eccaa1a9d25486b078c56b2be9c59161fb93c6c8b
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
	-H "Authorization: Bearer eda2b98c810209d53240532eccaa1a9d25486b078c56b2be9c59161fb93c6c8b"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 466456d5c61bc508548e7dc477c00c2ef49ca200af9a8e49443ff1e9b257bb3c
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
	-H "Authorization: Bearer 466456d5c61bc508548e7dc477c00c2ef49ca200af9a8e49443ff1e9b257bb3c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d149de9ecd715e4ab61996517497607e494db653057dfd6bc3e071c6f3e02542
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
	-H "Authorization: Bearer d149de9ecd715e4ab61996517497607e494db653057dfd6bc3e071c6f3e02542"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a0341c68029672b04e42d67c2adf8f9831a3b9007892a97420e3d6917a8cf96f
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
	-H "Authorization: Bearer a0341c68029672b04e42d67c2adf8f9831a3b9007892a97420e3d6917a8cf96f"
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
    "creator_id": 46,
    "id": 15,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 15,
    "additional_university_ids": [

    ],
    "discipline_id": 20,
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
    "chapters_updated_at": "2016-12-08T18:26:43.477Z",
    "updated_at": "2016-12-08T18:26:44.696Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 46,
        "chapter_id": 10,
        "position": 12,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:43.680Z",
        "created_at": "2016-12-08T18:26:43.594Z",
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
            "id": 23,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 24,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 46,
        "chapter_id": 11,
        "position": 14,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:43.980Z",
        "created_at": "2016-12-08T18:26:43.892Z",
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
            "id": 27,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 28,
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
        "id": 10,
        "updated_at": "2016-12-08T18:26:44.646Z",
        "course_id": 15,
        "author_id": 46,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:26:43.477Z",
        "questions_updated_at": "2016-12-08T18:26:43.477Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 10",
        "position": 1
      },
      {
        "id": 11,
        "updated_at": "2016-12-08T18:26:44.685Z",
        "course_id": 15,
        "author_id": 46,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:26:43.477Z",
        "questions_updated_at": "2016-12-08T18:26:43.477Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 11",
        "position": 2
      }
    ],
    "topic_id": 20,
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
Authorization: Bearer f5235fbac860d0be9078a64eb625b1dfb2c355097871ed66c96d77711c420398
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
    "creator_id": 57,
    "id": 17,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 17,
    "additional_university_ids": [

    ],
    "discipline_id": 22,
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
    "chapters_updated_at": "2016-12-08T18:26:46.145Z",
    "updated_at": "2016-12-08T18:26:47.433Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 58,
        "chapter_id": 14,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:47.206Z",
        "created_at": "2016-12-08T18:26:47.206Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 58,
        "chapter_id": 15,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:47.285Z",
        "created_at": "2016-12-08T18:26:47.285Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 58,
        "chapter_id": 14,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:47.250Z",
        "created_at": "2016-12-08T18:26:47.250Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 58,
        "chapter_id": 15,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:47.329Z",
        "created_at": "2016-12-08T18:26:47.329Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 58,
        "chapter_id": 14,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:46.365Z",
        "created_at": "2016-12-08T18:26:46.275Z",
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
            "id": 47,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 48,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 58,
        "chapter_id": 14,
        "position": 25,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:46.509Z",
        "created_at": "2016-12-08T18:26:46.426Z",
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
            "id": 49,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 50,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 58,
        "chapter_id": 15,
        "position": 26,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:46.683Z",
        "created_at": "2016-12-08T18:26:46.590Z",
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
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 58,
        "chapter_id": 15,
        "position": 27,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:26:46.830Z",
        "created_at": "2016-12-08T18:26:46.745Z",
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
            "id": 53,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 54,
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
        "id": 14,
        "updated_at": "2016-12-08T18:26:47.380Z",
        "course_id": 17,
        "author_id": 57,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:26:46.145Z",
        "questions_updated_at": "2016-12-08T18:26:46.145Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 14",
        "position": 1
      },
      {
        "id": 15,
        "updated_at": "2016-12-08T18:26:47.422Z",
        "course_id": 17,
        "author_id": 57,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:26:46.145Z",
        "questions_updated_at": "2016-12-08T18:26:46.145Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 15",
        "position": 2
      }
    ],
    "topic_id": 22,
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
	-H "Authorization: Bearer f5235fbac860d0be9078a64eb625b1dfb2c355097871ed66c96d77711c420398"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/13/pin
Content-Type: application/json
Authorization: Bearer da106a5dfb71e0f3f1a32e512eed622b6fbbf6d49563d8e7cf3cf7ae8172793b
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/13/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da106a5dfb71e0f3f1a32e512eed622b6fbbf6d49563d8e7cf3cf7ae8172793b"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/22/pin
Content-Type: application/json
Authorization: Bearer ef21c5aaa431eac5a7951407326aa924077a7d919a0a9d3553ed2afbb43941b4
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/22/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef21c5aaa431eac5a7951407326aa924077a7d919a0a9d3553ed2afbb43941b4"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3b4b5d454d582ccd1a50d66255c2bbac7708465a6e49f81c03b3c39fb6792c1d
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
    "creator_id": 63,
    "id": 18,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 18,
    "additional_university_ids": [

    ],
    "discipline_id": 23,
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
    "updated_at": "2016-12-08T18:26:47.713Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 23,
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
	-H "Authorization: Bearer 3b4b5d454d582ccd1a50d66255c2bbac7708465a6e49f81c03b3c39fb6792c1d"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 0eba02871fb06c2daad6542189274eb7f91d35e85cc49f69076ebf15dd47fa8d
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
    "id": 12,
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
    "created_at": "2016-12-08T18:26:39.522Z",
    "updated_at": "2016-12-08T18:26:39.522Z",
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
	-H "Authorization: Bearer 0eba02871fb06c2daad6542189274eb7f91d35e85cc49f69076ebf15dd47fa8d"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ba65d0cf2c2c57ca49d6d1d09caaffa69f95f15a3844c18a1924972572e280ae
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[4]}
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
    "id": 13,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      4
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:26:39.621Z",
    "updated_at": "2016-12-08T18:26:39.681Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[4]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba65d0cf2c2c57ca49d6d1d09caaffa69f95f15a3844c18a1924972572e280ae"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 4b7074d61f57a3eda76e7c8f392066acc56453f05869ca18f465773746c1dabb
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
    "id": 16,
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
    "created_at": "2016-12-08T18:26:39.854Z",
    "updated_at": "2016-12-08T18:26:39.854Z",
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
	-H "Authorization: Bearer 4b7074d61f57a3eda76e7c8f392066acc56453f05869ca18f465773746c1dabb"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 86434a34864e38bb2aab42a8a72698bf9df5023cc2588898b703f23b3e8337a4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[5]}
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
    "id": 14,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      5
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:26:39.723Z",
    "updated_at": "2016-12-08T18:26:39.723Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[5]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86434a34864e38bb2aab42a8a72698bf9df5023cc2588898b703f23b3e8337a4"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 895a3875afcfa01cc9307a80869b3b53b0ce30301dde0aeccd95ee70f0e97f01
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

8
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
    "id": 17,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/3183f61c3605d413913ed7209959601a5ed87993.jpg",
    "university_id": null,
    "fields_of_study": [
      8
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:26:39.945Z",
    "updated_at": "2016-12-08T18:26:40.164Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/94b516c5c3c2c68a649d50fe1ebbbe111bc0e3cd.jpg",
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

8
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 895a3875afcfa01cc9307a80869b3b53b0ce30301dde0aeccd95ee70f0e97f01"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 3e8b2d9fbdf759708a7c602606b2ad1949d35ea0187105c2b39ada3d1135a71c
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
      "id": 1,
      "bookmarkable_id": 1,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 2,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 3,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e8b2d9fbdf759708a7c602606b2ad1949d35ea0187105c2b39ada3d1135a71c"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b222f9270e2051ea1322ef57ebaefde9af91853019d13599da6a809d6e7ce7ca
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
      "company_id": 31,
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
      "company_id": 32,
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
	-H "Authorization: Bearer b222f9270e2051ea1322ef57ebaefde9af91853019d13599da6a809d6e7ce7ca"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b9b6a6d88ed5852c310738882ec11439f8735c53f55a7e13c263b5a5fa51ef84
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
      "company_id": 27,
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
	-H "Authorization: Bearer b9b6a6d88ed5852c310738882ec11439f8735c53f55a7e13c263b5a5fa51ef84"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 4edef976083e6db3075b5a0051c368577fb27a871c61ee12c99ea156ffc870bb
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
      "creator_id": 830,
      "id": 272,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-215",
      "html_url": "https://goskive.com/course/mit-course-215",
      "slug": "mit-course-215",
      "university_id": 252,
      "additional_university_ids": [

      ],
      "discipline_id": 285,
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
      "updated_at": "2016-12-08T18:27:50.032Z",
      "shortname": "mit-course-215",
      "topic_id": 284,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 831,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-216",
      "html_url": "https://goskive.com/course/mit-course-216",
      "slug": "mit-course-216",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "discipline_id": 286,
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
      "updated_at": "2016-12-08T18:27:50.138Z",
      "shortname": "mit-course-216",
      "topic_id": 285,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 216",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4edef976083e6db3075b5a0051c368577fb27a871c61ee12c99ea156ffc870bb"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 5dfa95b0979b6c7237f80fac766fcd2a82c1e924666fab3c96fb304c844ea1d4
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
        "created_at": "2016-12-08T18:27:20.625Z",
        "updated_at": "2016-12-08T18:27:20.625Z",
        "file_url": "memory://15029e55747246474983d1383f008af9.pdf",
        "course_id": 180,
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
        "created_at": "2016-12-08T18:27:20.736Z",
        "updated_at": "2016-12-08T18:27:20.736Z",
        "file_url": "memory://7b96f791169a18774b00fb9b75fa1fd1.pdf",
        "course_id": 181,
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
        "created_at": "2016-12-08T18:27:20.849Z",
        "updated_at": "2016-12-08T18:27:20.849Z",
        "file_url": "memory://49efee4ec7f49e1b0d495701c9dcd92c.pdf",
        "course_id": 182,
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
	-H "Authorization: Bearer 5dfa95b0979b6c7237f80fac766fcd2a82c1e924666fab3c96fb304c844ea1d4"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 2e47a516afc05ff9d94cc1b599c05209a2866094974d684a229a0451e1855e43
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
      "company_id": 24,
      "company": {
        "id": 24,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:27:35.672Z"
      },
      "created_at": "2016-12-08T18:27:35.675Z",
      "updated_at": "2016-12-08T18:27:35.675Z",
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
      "company_id": 25,
      "company": {
        "id": 25,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:27:35.683Z"
      },
      "created_at": "2016-12-08T18:27:35.687Z",
      "updated_at": "2016-12-08T18:27:35.687Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e47a516afc05ff9d94cc1b599c05209a2866094974d684a229a0451e1855e43"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 72a733e0f51472f2b95e51a23ee6d7c7ec5f29bfcc4a2f622717b80c41d22cd9
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
      "company_id": 20,
      "company": {
        "id": 20,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:27:35.460Z"
      },
      "created_at": "2016-12-08T18:27:35.463Z",
      "updated_at": "2016-12-08T18:27:35.463Z",
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:27:35.479Z"
      },
      "created_at": "2016-12-08T18:27:35.482Z",
      "updated_at": "2016-12-08T18:27:35.482Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72a733e0f51472f2b95e51a23ee6d7c7ec5f29bfcc4a2f622717b80c41d22cd9"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 305edcda7736145e9eea1f894c09ea6f8ee1b4329bcd5d6cde1ebd88026f7150
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
      "id": 2,
      "created_at": "2016-12-08T18:26:53.150Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-12-08T18:26:53.281Z",
      "author_id": "110",
      "thread_subject_id": "35",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 3,
      "created_at": "2016-12-08T18:26:53.270Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-12-08T18:26:53.284Z",
      "author_id": "113",
      "thread_subject_id": "36",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-12-08T18:26:53.693Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-12-08T18:26:53.693Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-12-08T18:26:54.067Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-12-08T18:26:54.067Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 6,
      "created_at": "2016-12-08T18:26:54.463Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-12-08T18:26:54.463Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 7,
      "created_at": "2016-12-08T18:26:54.755Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 41,
      "updated_at": "2016-12-08T18:26:54.755Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-12-08T18:26:55.047Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 42,
      "updated_at": "2016-12-08T18:26:55.047Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-12-08T18:26:55.368Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 43,
      "updated_at": "2016-12-08T18:26:55.368Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 305edcda7736145e9eea1f894c09ea6f8ee1b4329bcd5d6cde1ebd88026f7150"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/1
Content-Type: application/json
Authorization: Bearer 85794a59cc12991becf8a83cf3506d0ad1c74590704cc44b969700ebc3449285
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-08T18:16:52.000Z"}}
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
    "id": 1,
    "created_at": "2016-12-08T18:26:52.968Z",
    "read_at": "2016-12-08T18:16:52.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-12-08T18:26:53.018Z",
    "author_id": "106",
    "thread_subject_id": "34",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/1" -d '{"notification":{"read_at":"2016-12-08T18:16:52.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85794a59cc12991becf8a83cf3506d0ad1c74590704cc44b969700ebc3449285"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 4e04accd1cdf7a07afeda743a3318233c8ee06f06fa75dc0c2b0aa88e50c8f35
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
      "course_id": 55,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T18:26:58.600Z",
      "course_published": true,
      "updated_at": "2016-12-08T18:26:58.595Z"
    },
    {
      "id": 3,
      "course_id": 56,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T18:26:58.707Z",
      "course_published": true,
      "updated_at": "2016-12-08T18:26:58.702Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e04accd1cdf7a07afeda743a3318233c8ee06f06fa75dc0c2b0aa88e50c8f35"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer f185c2afcd0c88de9141ffedba815f5ac60ef5b27eb65f1624e9099a6c15423f
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
    "course_id": 59,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T18:26:59.222Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:26:59.217Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f185c2afcd0c88de9141ffedba815f5ac60ef5b27eb65f1624e9099a6c15423f"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 00073a2b225ac8c10cc56f18009cff697d58e4477243ee436b9cd92fee5c67e8
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
    "course_id": 60,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-08T18:26:59.431Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:26:59.421Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00073a2b225ac8c10cc56f18009cff697d58e4477243ee436b9cd92fee5c67e8"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 1822ed9c63c042b7d235b66e85506fc060e49cde0e447deaf6f78056bdd76d8b
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
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 80,
      "user_id": 628
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 628
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 82,
      "user_id": 628
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 83,
      "user_id": 628
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1822ed9c63c042b7d235b66e85506fc060e49cde0e447deaf6f78056bdd76d8b"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/52
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
    "id": 52,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 52,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 52
      },
      {
        "id": 53,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 52
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/52" -X GET \
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
      "id": 53,
      "name": "Object-based secondary toolset",
      "name_translations": {
        "en": "Object-based secondary toolset"
      }
    },
    {
      "id": 54,
      "name": "Exclusive context-sensitive database",
      "name_translations": {
        "en": "Exclusive context-sensitive database"
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
PATCH /v2/feedbacks/45/close
Content-Type: application/json
Authorization: Bearer 31794e05769dfe336a071162eaed03168aa391c5f6ee15bcea3943025542aa36
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
    "id": 45,
    "user_id": 766,
    "feedbackable_id": 87,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-08T18:27:45.438Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/45/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31794e05769dfe336a071162eaed03168aa391c5f6ee15bcea3943025542aa36"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/40/fix
Content-Type: application/json
Authorization: Bearer d7862e1f44a97faeeae208a6b9c71aab010d1742b5117e10407c1d387b5a3fa9
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
    "user_id": 739,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-08T18:27:43.722Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/40/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7862e1f44a97faeeae208a6b9c71aab010d1742b5117e10407c1d387b5a3fa9"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/42
Content-Type: application/json
Authorization: Bearer bda368972cd6e16061f8a6ccd0fc45218f2abd5ccc523805aa28e7fe6bd4bc40
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
    "id": 42,
    "user_id": 749,
    "feedbackable_id": 84,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:27:44.521Z",
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
curl "api.goskive.com/v2/feedbacks/42" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bda368972cd6e16061f8a6ccd0fc45218f2abd5ccc523805aa28e7fe6bd4bc40"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/38/fix
Content-Type: application/json
Authorization: Bearer 96b6048efa2d205e9bed2731f2922251788328520b1bc32d38ff661de16d6126
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
curl "api.goskive.com/v2/feedbacks/38/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96b6048efa2d205e9bed2731f2922251788328520b1bc32d38ff661de16d6126"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/39/fix
Content-Type: application/json
Authorization: Bearer 8ffbfe7e7efccf8fb69e2adb2bda1feb7542a247893b9f5c45b0adc3259c51a5
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
curl "api.goskive.com/v2/feedbacks/39/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ffbfe7e7efccf8fb69e2adb2bda1feb7542a247893b9f5c45b0adc3259c51a5"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/close
Content-Type: application/json
Authorization: Bearer 2dab3b76c66626d876bce8ad10174997da7fac596cc8f0e3d087120b3a1d3672
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
curl "api.goskive.com/v2/feedbacks/46/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dab3b76c66626d876bce8ad10174997da7fac596cc8f0e3d087120b3a1d3672"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/43
Content-Type: application/json
Authorization: Bearer a7d7f69e26d3807c189bbf856d80e125c4b66f93a41f0ca1e368203260e2419c
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
    "id": 43,
    "user_id": 754,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:27:44.877Z",
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
curl "api.goskive.com/v2/feedbacks/43" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7d7f69e26d3807c189bbf856d80e125c4b66f93a41f0ca1e368203260e2419c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 0bfa49c82ae87e9f84f8235685364ac957bfd5def8e4b3147eeb840396b77d53
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
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bfa49c82ae87e9f84f8235685364ac957bfd5def8e4b3147eeb840396b77d53"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/13/bookmark
Content-Type: application/json
Authorization: Bearer b7176526cc7581313b8ad73652f9a3b5631a4fa18fedb2253ecfde833f6511ae
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7176526cc7581313b8ad73652f9a3b5631a4fa18fedb2253ecfde833f6511ae"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer a7286dec2e334e135b4bd0d894665d641c4354e6623c2a540b15fd5d4ac799a1
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
	-H "Authorization: Bearer a7286dec2e334e135b4bd0d894665d641c4354e6623c2a540b15fd5d4ac799a1"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/15
Content-Type: application/json
Authorization: Bearer e13106bc64802b774109537c2a7afa8f67e3cbae674ef949e71f9be370613614
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/a38e00d23ff63d8f93056dee95025e3d.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T182746Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=b626ca50a0dffe5dab9694fa9cfa75aea4ac8285cb32346b770ba18e25321462",
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
	-H "Authorization: Bearer e13106bc64802b774109537c2a7afa8f67e3cbae674ef949e71f9be370613614"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/22/preview
Content-Type: application/json
Authorization: Bearer 1e1750ee999c572b7958478e463c0420c9d5c7d811c39361eeb56dc8606b77f5
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/33e715a939c6c436b84d36583769eb36.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T182748Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d459970f7b3af90ed5a065cf58fca68f652d18c1431554b30b6a588fc54b9de2",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/22/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e1750ee999c572b7958478e463c0420c9d5c7d811c39361eeb56dc8606b77f5"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/17/metadata
Content-Type: application/json
Authorization: Bearer b55695e66de085676d052291d0f0318e981399b7d7ce75921eefdca63f432a79
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
    "id": 17,
    "uploader": {
      "id": 793,
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
      "created_at": "2016-12-08T18:27:46.922Z",
      "updated_at": "2016-12-08T18:27:46.922Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-08T18:27:47.021Z",
    "updated_at": "2016-12-08T18:27:47.021Z",
    "course_id": 262,
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
curl "api.goskive.com/v2/files/17/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b55695e66de085676d052291d0f0318e981399b7d7ce75921eefdca63f432a79"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer caf6fe0a73e96bb9d31b8b537633a0119792d907e3a1a2d800f7bffb9d97e451
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
      "creator_id": 608,
      "id": 217,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 197,
      "additional_university_ids": [

      ],
      "discipline_id": 230,
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
      "chapters_updated_at": "2016-12-08T18:27:33.195Z",
      "updated_at": "2016-12-08T18:27:34.613Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 229,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 613,
      "id": 218,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-c285ff8a-a87f-4938-9876-d1548eead6cd",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-c285ff8a-a87f-4938-9876-d1548eead6cd",
      "slug": "mit-the-great-british-bake-off-c285ff8a-a87f-4938-9876-d1548eead6cd",
      "university_id": 198,
      "additional_university_ids": [

      ],
      "discipline_id": 231,
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
      "chapters_updated_at": "2016-12-08T18:27:33.195Z",
      "updated_at": "2016-12-08T18:27:35.092Z",
      "shortname": "mit-the-great-british-bake-off-c285ff8a-a87f-4938-9876-d1548eead6cd",
      "topic_id": 230,
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
curl "api.goskive.com/v2/files/8/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer caf6fe0a73e96bb9d31b8b537633a0119792d907e3a1a2d800f7bffb9d97e451"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/19/download
Content-Type: application/json
Authorization: Bearer 5df56c00b335dd10df07dfbf53d35dc0e85eed611b950cd1f8f3f638c459a05d
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
	-H "Authorization: Bearer 5df56c00b335dd10df07dfbf53d35dc0e85eed611b950cd1f8f3f638c459a05d"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/20/report
Content-Type: application/json
Authorization: Bearer 2f7311bddeca9267ad6f63bf3043a244ae47c1d150dc3cac41cd18dd1f20800b
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f7311bddeca9267ad6f63bf3043a244ae47c1d150dc3cac41cd18dd1f20800b"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/14/bookmark
Content-Type: application/json
Authorization: Bearer 7d6394c321ff6e3e41f26cdf216c218cbb65fe9d820b5fe9bb00fd5df8baa714
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
	-H "Authorization: Bearer 7d6394c321ff6e3e41f26cdf216c218cbb65fe9d820b5fe9bb00fd5df8baa714"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/21/upvote
Content-Type: application/json
Authorization: Bearer ba4f1c7c86499592794d838c4c9bcc1934c1d05ec00c9a79a710c29e5c8e479a
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba4f1c7c86499592794d838c4c9bcc1934c1d05ec00c9a79a710c29e5c8e479a"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/65/comments
Content-Type: application/json
Authorization: Bearer 649b6f053fee06b0efaa8f866ef6b89dc286f8512ffed92aaa79da3393426597
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
    "author_id": 551,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:27:30.494Z",
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
curl "api.goskive.com/v2/flashcards/65/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 649b6f053fee06b0efaa8f866ef6b89dc286f8512ffed92aaa79da3393426597"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/63/comments
Content-Type: application/json
Authorization: Bearer 652cc574a7ebcff56d41f6c067d60a305260351847c87e2ef9271895072856cb
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
    "author_id": 545,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:27:29.900Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 545,
      "feedbackable_id": 63,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:29.898Z",
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
	-H "Authorization: Bearer 652cc574a7ebcff56d41f6c067d60a305260351847c87e2ef9271895072856cb"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/66/comments
Content-Type: application/json
Authorization: Bearer 38372d80659739c443885a7e3e3bcc88657d377e9c5c91ab1137de7ef12f46b0
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
      "id": 56,
      "author_id": 557,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:30.832Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 558,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:30.848Z",
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
curl "api.goskive.com/v2/flashcards/66/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38372d80659739c443885a7e3e3bcc88657d377e9c5c91ab1137de7ef12f46b0"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/64/comments
Content-Type: application/json
Authorization: Bearer 2e346d0535b920bf921aa75974130821cbeba1e8159cd45b2015c3fabfbc24a4
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
curl "api.goskive.com/v2/flashcards/64/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e346d0535b920bf921aa75974130821cbeba1e8159cd45b2015c3fabfbc24a4"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/74/feedbacks
Content-Type: application/json
Authorization: Bearer 7cd9efe6cb090e7148aeedcd5132c1989d466adbb2f16abe79b1dcaddd81239d
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
    "id": 17,
    "user_id": 592,
    "feedbackable_id": 74,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:27:32.588Z",
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
curl "api.goskive.com/v2/flashcards/74/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cd9efe6cb090e7148aeedcd5132c1989d466adbb2f16abe79b1dcaddd81239d"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/73/feedbacks
Content-Type: application/json
Authorization: Bearer 28aeba4570dcb284b7f0563467489476aaa93b7b42dabd0e793fe65193ee246a
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
      "user_id": 591,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:32.349Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 590,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:32.339Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/73/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28aeba4570dcb284b7f0563467489476aaa93b7b42dabd0e793fe65193ee246a"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/61/votes
Content-Type: application/json
Authorization: Bearer db1777513c3c675a253e86f04fe49dfdb21f7724ca135d30c95643bbdb046bb7
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
      "id": 13,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 61,
      "user_id": 523
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 61,
      "user_id": 522
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 61,
      "user_id": 521
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/61/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db1777513c3c675a253e86f04fe49dfdb21f7724ca135d30c95643bbdb046bb7"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/36/republish
Content-Type: application/json
Authorization: Bearer 5565dc5f1e4a6dce29b406e918e7eb74b07654b18c612d486dc41222b9c50f98
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
curl "api.goskive.com/v2/flashcards/36/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5565dc5f1e4a6dce29b406e918e7eb74b07654b18c612d486dc41222b9c50f98"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/39/bookmark
Content-Type: application/json
Authorization: Bearer 7a051e6e909f618fccdd23498ed60b112e4ce1cf2433962ea763841ef5934810
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a051e6e909f618fccdd23498ed60b112e4ce1cf2433962ea763841ef5934810"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/43
Content-Type: application/json
Authorization: Bearer b8a2061ea75767dd95dac12135381befe6a63b287284487446c75d1324e400dd
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8a2061ea75767dd95dac12135381befe6a63b287284487446c75d1324e400dd"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/downvote
Content-Type: application/json
Authorization: Bearer 432ab2de4a7efc48b204dcda61593bd9729435219cc2320fdc08d6cdc97efc8d
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 432ab2de4a7efc48b204dcda61593bd9729435219cc2320fdc08d6cdc97efc8d"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/42
Content-Type: application/json
Authorization: Bearer c45ea71de319b972d1e18b034053eb14b7b3f84a2b03a8aae6f409e86e605c31
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
    "id": 42,
    "obfuscated_id": "6gppIIjkzlA",
    "author_id": 394,
    "chapter_id": 60,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:27:17.006Z",
    "created_at": "2016-12-08T18:27:17.006Z",
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
curl "api.goskive.com/v2/flashcards/42" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c45ea71de319b972d1e18b034053eb14b7b3f84a2b03a8aae6f409e86e605c31"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/report
Content-Type: application/json
Authorization: Bearer 25cddd05ff267d2669e4e0a44d85d26186ecbe3edc6dfb6552232604a914c57d
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25cddd05ff267d2669e4e0a44d85d26186ecbe3edc6dfb6552232604a914c57d"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/38/bookmark
Content-Type: application/json
Authorization: Bearer d55cf8784cc3b9cff6ce23b45c6b7a00913e44cb19389b3d84757d588ffc8194
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d55cf8784cc3b9cff6ce23b45c6b7a00913e44cb19389b3d84757d588ffc8194"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/upvote
Content-Type: application/json
Authorization: Bearer abbfd4c51941bfd3d16930711b60c9301bc6df27d4290d4a9b482e35465ff9df
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abbfd4c51941bfd3d16930711b60c9301bc6df27d4290d4a9b482e35465ff9df"
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
    "key": "cache/16cdad2123b01c7ca48bcced466cf64e.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxOToyNzowN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzE2Y2RhZDIxMjNiMDFjN2NhNDhiY2NlZDQ2NmNmNjRlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDhUMTgyNzA3WiJ9XX0=",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T182707Z",
    "x-amz-signature": "145a8995922cdb9ca90e0d2bfcb55af55647119f9f9bd38255eb9fb40c2bfa59"
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
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 01190e5bb8ffd2c23480564b94ce341447624fc1502318e85bc0e2ccf447a110
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
curl "api.goskive.com/v2/me/jobs/1/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01190e5bb8ffd2c23480564b94ce341447624fc1502318e85bc0e2ccf447a110"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer c5664b4bc887339ff2f7e69ef071aad3e34351925e03598dc9126ccb5300207a
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
	-H "Authorization: Bearer c5664b4bc887339ff2f7e69ef071aad3e34351925e03598dc9126ccb5300207a"
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
{"password":{"reset_password_token":"FYkwYRxM1G_ssiSdiC1o","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 531,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-08T18:27:28.694Z",
  "updated_at": "2016-12-08T18:27:28.851Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "locale": "en",
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "audit_id": 8165
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"FYkwYRxM1G_ssiSdiC1o","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Content-Type: application/json
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
Content-Type: application/json
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
POST /v2/questions/50/comments
Content-Type: application/json
Authorization: Bearer 96d9e2a72112b3307c0c00375a3b422aea91a573864be3cc03f133935dee1159
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
    "author_id": 191,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:27:00.853Z",
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
curl "api.goskive.com/v2/questions/50/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96d9e2a72112b3307c0c00375a3b422aea91a573864be3cc03f133935dee1159"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/51/comments
Content-Type: application/json
Authorization: Bearer 6e658e4763ef1fdc1036702b60240e445c0f79ee212eb222d73251f25b06760c
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
    "id": 7,
    "author_id": 194,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:27:01.922Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 194,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:01.918Z",
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
curl "api.goskive.com/v2/questions/51/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e658e4763ef1fdc1036702b60240e445c0f79ee212eb222d73251f25b06760c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/48/comments
Content-Type: application/json
Authorization: Bearer e7c0a744e4b8e499dc5bb6bcc0ede875a73028c1a6be2ee404e4848d5d723c12
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
      "author_id": 186,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:00.116Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 187,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:27:00.133Z",
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
curl "api.goskive.com/v2/questions/48/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7c0a744e4b8e499dc5bb6bcc0ede875a73028c1a6be2ee404e4848d5d723c12"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/49/comments
Content-Type: application/json
Authorization: Bearer b6d613605a4ff29dc1018f2a923a82a6449229618368eecaffa6e579d007752a
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
curl "api.goskive.com/v2/questions/49/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6d613605a4ff29dc1018f2a923a82a6449229618368eecaffa6e579d007752a"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/69/feedbacks
Content-Type: application/json
Authorization: Bearer b80edc130f8d48ccc61cf61241a377ba870c9ae2b1cd9ae8cea03de7e5c1096f
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
    "id": 9,
    "user_id": 493,
    "feedbackable_id": 69,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:27:24.136Z",
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
curl "api.goskive.com/v2/questions/69/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b80edc130f8d48ccc61cf61241a377ba870c9ae2b1cd9ae8cea03de7e5c1096f"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/67/feedbacks
Content-Type: application/json
Authorization: Bearer 88126bd595847482f8fc1e633de735d350763da58e315ccd387699a851186189
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
      "user_id": 489,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:23.213Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 488,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:27:23.202Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/67/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88126bd595847482f8fc1e633de735d350763da58e315ccd387699a851186189"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/46/votes
Content-Type: application/json
Authorization: Bearer 4a7731a3b503dd7ccea49c4ad21b93a888c7eda1b134db0c1fe7c384a1069c4e
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
      "votable_id": 46,
      "user_id": 159
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 46,
      "user_id": 158
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 46,
      "user_id": 157
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/46/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a7731a3b503dd7ccea49c4ad21b93a888c7eda1b134db0c1fe7c384a1069c4e"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/109/republish
Content-Type: application/json
Authorization: Bearer 11b87e6f870a4f9304d5825436a3a5ab2a12c2b246188fc3e821e92d7490380a
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
curl "api.goskive.com/v2/questions/109/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11b87e6f870a4f9304d5825436a3a5ab2a12c2b246188fc3e821e92d7490380a"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/108/bookmark
Content-Type: application/json
Authorization: Bearer eaaa64c791218b04d5458d7098e7777705be29b68ed5e04d0471f289bdf99c97
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/108/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaaa64c791218b04d5458d7098e7777705be29b68ed5e04d0471f289bdf99c97"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/131
Content-Type: application/json
Authorization: Bearer c144ba21eb4f56715bf1f4366373029b0f93483245101541878a0a9897ef51f1
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/131" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c144ba21eb4f56715bf1f4366373029b0f93483245101541878a0a9897ef51f1"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/126/downvote
Content-Type: application/json
Authorization: Bearer ac19a1f62a59832fee86388ce35aadcae15130cec9366fef1ec1507d7ac4d374
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/126/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac19a1f62a59832fee86388ce35aadcae15130cec9366fef1ec1507d7ac4d374"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/127
Content-Type: application/json
Authorization: Bearer e6a69e6585537b896a027e070478b9d7cffb46cffb79937af3e337d2e935ab4a
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
    "id": 127,
    "obfuscated_id": "E3yfRgAzssw",
    "author_id": 909,
    "chapter_id": 167,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:27:57.658Z",
    "created_at": "2016-12-08T18:27:57.576Z",
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
        "id": 256,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 257,
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
curl "api.goskive.com/v2/questions/127" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6a69e6585537b896a027e070478b9d7cffb46cffb79937af3e337d2e935ab4a"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/107/report
Content-Type: application/json
Authorization: Bearer c2564de14ee6d9444c3ee70650571b7a80849bf3fecd96659c6bc29c51123060
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/107/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2564de14ee6d9444c3ee70650571b7a80849bf3fecd96659c6bc29c51123060"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/129/bookmark
Content-Type: application/json
Authorization: Bearer 7859455a7bf5eabed9b881557ff10908defa6400733bd6a33f5ce7ad558f7fd4
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
	-H "Authorization: Bearer 7859455a7bf5eabed9b881557ff10908defa6400733bd6a33f5ce7ad558f7fd4"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/128
Content-Type: application/json
Authorization: Bearer 73010bcfc82722db464ce8d4349e39c6c4bf3a37624a0e9f4eae8c6aba7ac6a1
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":128,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T18:27:57.879Z","updated_at":"2016-12-08T18:27:57.962Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":168,"author_id":912,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 128,
    "obfuscated_id": "Q4ODZIcqv0E",
    "author_id": 912,
    "chapter_id": 168,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:27:58.049Z",
    "created_at": "2016-12-08T18:27:57.879Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x000000127470b8>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 258,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 259,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 260,
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
curl "api.goskive.com/v2/questions/128" -d '{"question":{"question":{"id":128,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T18:27:57.879Z","updated_at":"2016-12-08T18:27:57.962Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":168,"author_id":912,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73010bcfc82722db464ce8d4349e39c6c4bf3a37624a0e9f4eae8c6aba7ac6a1"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/130/upvote
Content-Type: application/json
Authorization: Bearer 5899d61c2bb24354e320bf26ccf9e53522f6b12f3b48e222f8273702030c4bbd
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/130/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5899d61c2bb24354e320bf26ccf9e53522f6b12f3b48e222f8273702030c4bbd"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer b82c7da3b851d25362d952e7d9a4d80528d3155078d18137671036a17a98694c
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
      "creator_id": 163,
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "discipline_id": 59,
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
      "updated_at": "2016-12-08T18:26:58.106Z",
      "shortname": "mit-pizza-201",
      "topic_id": 58,
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
	-H "Authorization: Bearer b82c7da3b851d25362d952e7d9a4d80528d3155078d18137671036a17a98694c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer ccef26365c3dba8d1cb185f7bbc23136b8baa6c7ad9e5ece92a01d639765f970
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
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-51",
      "html_url": "https://goskive.com/university/uni-51",
      "slug": "uni-51",
      "name": "National School of Pizza",
      "short_name": "Uni 51",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/a250af885c6472f657eb43e02ccf9e4c.jpg",
      "image_thumb_url": "memory://universities/1903b78292692316bc16b745552261ab.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:26:57.843Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 50,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-50",
      "html_url": "https://goskive.com/university/uni-50",
      "slug": "uni-50",
      "name": "National School of Pastry",
      "short_name": "Uni 50",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/2740b97c2429ca1b0c82c25bed4a9263.jpg",
      "image_thumb_url": "memory://universities/c3af06a01b610ad7d562e6d2f59abe98.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:26:57.797Z",
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
	-H "Authorization: Bearer ccef26365c3dba8d1cb185f7bbc23136b8baa6c7ad9e5ece92a01d639765f970"
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
      "id": 114,
      "name": "Implemented directional forecast",
      "name_translations": {
        "en": "Implemented directional forecast"
      },
      "discipline_id": 115
    },
    {
      "id": 115,
      "name": "Ergonomic client-driven projection",
      "name_translations": {
        "en": "Ergonomic client-driven projection"
      },
      "discipline_id": 116
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
GET /v2/topics/113
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
    "id": 113,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 114
  }
}
```



```shell
curl "api.goskive.com/v2/topics/113" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer c2c3d3941dd87ddb3eebbb3a59227d5f4c93222c545bcd8e3dc8261060655c74
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
      "id": 284,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-264",
      "html_url": "https://goskive.com/university/uni-264",
      "slug": "uni-264",
      "name": "University 216",
      "short_name": "Uni 264",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/a980aa84971ab26965155bb49cb44cd5.jpg",
      "image_thumb_url": "memory://universities/8b71eab50b4828e391a8ef8948d97c79.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:27:59.551Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 285,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-265",
      "html_url": "https://goskive.com/university/uni-265",
      "slug": "uni-265",
      "name": "University 217",
      "short_name": "Uni 265",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/c0820a6425360b505588a9c32285eb10.jpg",
      "image_thumb_url": "memory://universities/699fc479ad2b1d63cb7f85cbdcf413c8.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:27:59.596Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 286,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-266",
      "html_url": "https://goskive.com/university/uni-266",
      "slug": "uni-266",
      "name": "University 218",
      "short_name": "Uni 266",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/7b04a5fc8b688a81a6c777b054f70d55.jpg",
      "image_thumb_url": "memory://universities/0b644d4e2e07331639d4dd3df157ca2f.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:27:59.641Z",
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
	-H "Authorization: Bearer c2c3d3941dd87ddb3eebbb3a59227d5f4c93222c545bcd8e3dc8261060655c74"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 7953107ee3674856f75b61c943a10c38f6115d7b3958c8b88e00a69d84e47d2b
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
    "id": 282,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/825cc23db1650bf646b45d5e09526664.jpg",
    "image_thumb_url": "memory://universities/a350243df112b2e6831d46f55acee78e.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-08T18:27:59.365Z",
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
	-H "Authorization: Bearer 7953107ee3674856f75b61c943a10c38f6115d7b3958c8b88e00a69d84e47d2b"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 19feab2238d27570e9bac5028b879919be91264048de91e6b82445ac6d1346c8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":75,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 199,
    "id": 68,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 69,
    "additional_university_ids": [

    ],
    "discipline_id": 76,
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
    "chapters_updated_at": "2016-12-08T18:27:02.424Z",
    "updated_at": "2016-12-08T18:27:02.571Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 38,
        "updated_at": "2016-12-08T18:27:02.558Z",
        "course_id": 68,
        "author_id": 199,
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
        "id": 39,
        "updated_at": "2016-12-08T18:27:02.573Z",
        "course_id": 68,
        "author_id": 199,
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
        "id": 40,
        "updated_at": "2016-12-08T18:27:02.588Z",
        "course_id": 68,
        "author_id": 199,
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
    "topic_id": 75,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":75,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19feab2238d27570e9bac5028b879919be91264048de91e6b82445ac6d1346c8"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer af81b61faacb89d9cf35211b1704d167c2bd493f46db9c2baa892fc9959ba4ef
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":74,"published":false}}
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
    "creator_id": 198,
    "id": 67,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 68,
    "additional_university_ids": [

    ],
    "discipline_id": 75,
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
    "updated_at": "2016-12-08T18:27:02.378Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 74,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":74,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af81b61faacb89d9cf35211b1704d167c2bd493f46db9c2baa892fc9959ba4ef"
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
      "creator_id": 202,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-39",
      "html_url": "https://goskive.com/course/fu-course-39",
      "slug": "fu-course-39",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "discipline_id": 80,
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
      "updated_at": "2016-12-08T18:27:03.000Z",
      "shortname": "fu-course-39",
      "topic_id": 79,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 39",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 202,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-40",
      "html_url": "https://goskive.com/course/fu-course-40",
      "slug": "fu-course-40",
      "university_id": 71,
      "additional_university_ids": [

      ],
      "discipline_id": 81,
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
      "chapters_updated_at": "2016-12-08T18:27:02.845Z",
      "updated_at": "2016-12-08T18:27:03.285Z",
      "shortname": "fu-course-40",
      "topic_id": 80,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 40",
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
Authorization: Bearer cefcad1839b90a35b1caeeaf1a9c8b6a9f939888c2df3754d6c3edbd90cbe891
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
      "creator_id": 209,
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "discipline_id": 88,
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
      "updated_at": "2016-12-08T18:27:03.765Z",
      "shortname": "fu-course-47",
      "topic_id": 87,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 209,
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-48",
      "html_url": "https://goskive.com/course/fu-course-48",
      "slug": "fu-course-48",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "discipline_id": 89,
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
      "chapters_updated_at": "2016-12-08T18:27:03.612Z",
      "updated_at": "2016-12-08T18:27:04.041Z",
      "shortname": "fu-course-48",
      "topic_id": 88,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 48",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cefcad1839b90a35b1caeeaf1a9c8b6a9f939888c2df3754d6c3edbd90cbe891"
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
      "creator_id": 207,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-43",
      "html_url": "https://goskive.com/course/fu-course-43",
      "slug": "fu-course-43",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "discipline_id": 84,
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
      "updated_at": "2016-12-08T18:27:03.479Z",
      "shortname": "fu-course-43",
      "topic_id": 83,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 43",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 207,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "discipline_id": 85,
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
      "updated_at": "2016-12-08T18:27:03.512Z",
      "shortname": "fu-course-44",
      "topic_id": 84,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 44",
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
Authorization: Bearer 78b81b1de1849dc0a40a2e6233717c4081647c249a984dca67b60423cb9a470a
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
      "creator_id": 216,
      "id": 84,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-51",
      "html_url": "https://goskive.com/course/fu-course-51",
      "slug": "fu-course-51",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "discipline_id": 92,
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
      "updated_at": "2016-12-08T18:27:04.377Z",
      "shortname": "fu-course-51",
      "topic_id": 91,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 51",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 216,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-52",
      "html_url": "https://goskive.com/course/fu-course-52",
      "slug": "fu-course-52",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "discipline_id": 93,
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
      "updated_at": "2016-12-08T18:27:04.409Z",
      "shortname": "fu-course-52",
      "topic_id": 92,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 52",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78b81b1de1849dc0a40a2e6233717c4081647c249a984dca67b60423cb9a470a"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 61fab3f7f1462716806ee5d020e82dfd1b082e364c5cf2532ff032e0a2a57f14
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
  "id": 824,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-08T18:27:49.509Z",
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
	-H "Authorization: Bearer 61fab3f7f1462716806ee5d020e82dfd1b082e364c5cf2532ff032e0a2a57f14"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/279
Content-Type: application/json
Authorization: Bearer 7d98c65dd5363b1c5f35b1b232db6df44fb1c3a93ddb49fab3e61cd7a8c13860
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
    "id": 279,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 94,
    "fields_of_study": [
      125,
      126
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-08T18:27:10.074Z",
    "updated_at": "2016-12-08T18:27:10.074Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/279" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d98c65dd5363b1c5f35b1b232db6df44fb1c3a93ddb49fab3e61cd7a8c13860"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/281
Content-Type: application/json
Authorization: Bearer 96ee141991476d94a6050ac0c740636ccb271d4c99eeb4dd75d11915394d36fa
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
    "id": 281,
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
    "created_at": "2016-12-08T18:27:10.160Z",
    "updated_at": "2016-12-08T18:27:10.160Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/281" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96ee141991476d94a6050ac0c740636ccb271d4c99eeb4dd75d11915394d36fa"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/20
Content-Type: application/json
Authorization: Bearer 1eccfde8f0537807d2ed4ef18953eee2a5a5d30069db7d72104700794d7f3fe9
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
	-H "Authorization: Bearer 1eccfde8f0537807d2ed4ef18953eee2a5a5d30069db7d72104700794d7f3fe9"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/19
Content-Type: application/json
Authorization: Bearer 117619f8e07917735710c14aebb7c70f8512f926a1b3ea48800f46342505194d
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
    "votable_id": 104,
    "user_id": 832
  }
}
```



```shell
curl "api.goskive.com/v2/votes/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 117619f8e07917735710c14aebb7c70f8512f926a1b3ea48800f46342505194d"
```
