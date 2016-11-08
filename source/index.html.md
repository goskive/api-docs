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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"85aec37133a8079bb6c3cf3537c4a4e133b523d1751d30652917489150c29b1d","client_secret":"819b4a85e1a7a66e2e87762e75e6ea38f09a1571963a05590098f1b8de75133c"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"85aec37133a8079bb6c3cf3537c4a4e133b523d1751d30652917489150c29b1d","client_secret":"819b4a85e1a7a66e2e87762e75e6ea38f09a1571963a05590098f1b8de75133c"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZmRjZTVkMWVlOTdmYzY0NzNlMjNiZGEyNTAyOTkyYjYzZWU5OWViZjE2Njll
ZjY5NDIxYzdlZWJjODE4ZTJlNTpmZWYxZTE2MTQxMjg4NDJkNGI3MTVlOWVj
Mjc1MDliZmY0NWQ5MmZkYzc5YTI4NWVmOTUxNWJjMGY2ZDFjMjk3

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
	-u fdce5d1ee97fc6473e23bda2502992b63ee99ebf1669ef69421c7eebc818e2e5:fef1e1614128842d4b715e9ec27509bff45d92fdc79a285ef9515bc0f6d1c297
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
{"grant_type":"client_credentials","client_id":"951ea3d419e176452dac16656b241c872d09b1bbe5cfd49569876f05f3af477b","client_secret":"182ea6f5c5fcfd8b40b832176426d2e7aa9a77a8896ef58d86632dff544028e9"}
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
  "access_token": "96d7fa6d630e0bcbecf4126568e6ce5fd23ece7f6436ab720c11480d24024964",
  "token_type": "bearer",
  "created_at": 1478614863
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"951ea3d419e176452dac16656b241c872d09b1bbe5cfd49569876f05f3af477b","client_secret":"182ea6f5c5fcfd8b40b832176426d2e7aa9a77a8896ef58d86632dff544028e9"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2caba9262aea635628fcecc16685d561884deb03086671837dd4c2a5713e7005","client_secret":"1276f62efc9bd1308bf0889c03a2ff044769247cc36402bb7e89e83d9c431cc0"}
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
  "access_token": "723163f8e06d9cb969da34b8316956c22bb1564111456c2c7b65243aee1aff5b",
  "token_type": "bearer",
  "created_at": 1478614863
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2caba9262aea635628fcecc16685d561884deb03086671837dd4c2a5713e7005","client_secret":"1276f62efc9bd1308bf0889c03a2ff044769247cc36402bb7e89e83d9c431cc0"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NGQwZDgxZjBjMTUxMGQ4MDU5ZmRmNThkNGQyZDJhN2Y1ZmFiMmE0ZmU3ZTIz
ZjUwZGIwMjUyMTVjOTEwM2RkMTplZDkwM2UzMjZhN2ViYmE1ZGY0ZTkxZTM0
OTI3NWM2MjNjOWQ0Zjg3OTE0MGJiZTYzNDkzZGM2NWE3YzcwZjQ2

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
  "access_token": "a7e901c27dab85276c217b24a3ffd8006b6a477f1b6da88369d4d1a7cb4e2ad9",
  "token_type": "bearer",
  "created_at": 1478614863
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 4d0d81f0c1510d8059fdf58d4d2d2a7f5fab2a4fe7e23f50db025215c9103dd1:ed903e326a7ebba5df4e91e349275c623c9d4f879140bbe63493dc65a7c70f46
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
Authorization: Bearer 2bfc8a9c909b5bf4ea0a3bca1e768d724cb891d7166cac272f748fe52fea4641
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
    "company_id": 33,
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
	-H "Authorization: Bearer 2bfc8a9c909b5bf4ea0a3bca1e768d724cb891d7166cac272f748fe52fea4641"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/123/flashcards
Content-Type: application/json
Authorization: Bearer d00de980d80f3f94ccea23cb9fdfb46be0c92337348eca4ee066ed11e245fbc3
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":123,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 53,
    "obfuscated_id": "XffxqHkTsbc",
    "author_id": 593,
    "chapter_id": 123,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:41.894Z",
    "created_at": "2016-11-08T14:21:41.894Z",
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
curl "api.goskive.com/v2/chapters/123/flashcards" -d '{"flashcard":{"chapter_id":123,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d00de980d80f3f94ccea23cb9fdfb46be0c92337348eca4ee066ed11e245fbc3"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/125/flashcards
Content-Type: application/json
Authorization: Bearer 2ad08e591efec3cf43f0b197045ac25d6ac89cc641d612d73fe3dd09dd9fc3cb
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
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 597,
      "chapter_id": 125,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:42.256Z",
      "created_at": "2016-11-08T14:21:42.256Z",
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
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 597,
      "chapter_id": 125,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:42.291Z",
      "created_at": "2016-11-08T14:21:42.291Z",
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
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 597,
      "chapter_id": 125,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:42.326Z",
      "created_at": "2016-11-08T14:21:42.326Z",
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
curl "api.goskive.com/v2/chapters/125/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ad08e591efec3cf43f0b197045ac25d6ac89cc641d612d73fe3dd09dd9fc3cb"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/166/questions
Content-Type: application/json
Authorization: Bearer 97ef4a309494807dee61cd89a0ddf4237e260a288d71e8e7c6d1480d0fd24e0e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":166,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 94,
    "obfuscated_id": "CVi6VU_nV6k",
    "author_id": 785,
    "chapter_id": 166,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:56.120Z",
    "created_at": "2016-11-08T14:21:56.120Z",
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
        "id": 189,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 190,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 191,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 192,
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
curl "api.goskive.com/v2/chapters/166/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":166,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97ef4a309494807dee61cd89a0ddf4237e260a288d71e8e7c6d1480d0fd24e0e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/164/questions
Content-Type: application/json
Authorization: Bearer cfba75f13d438f8df32570015311f93a236322d1b945e547b17a3e03ec31cbdd
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":164,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 92,
    "obfuscated_id": "__OphzZQiQY",
    "author_id": 779,
    "chapter_id": 164,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:55.078Z",
    "created_at": "2016-11-08T14:21:55.078Z",
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
        "id": 185,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 186,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/164/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":164,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfba75f13d438f8df32570015311f93a236322d1b945e547b17a3e03ec31cbdd"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/165/questions
Content-Type: application/json
Authorization: Bearer ebdf5a04f0f66f7d1b8c2448b12ded6674aa308e1337a0902affd9ece0ba8ba1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":165,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 93,
    "obfuscated_id": "4z_mapEg68k",
    "author_id": 782,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:55.595Z",
    "created_at": "2016-11-08T14:21:55.595Z",
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
        "id": 187,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 188,
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
curl "api.goskive.com/v2/chapters/165/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":165,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebdf5a04f0f66f7d1b8c2448b12ded6674aa308e1337a0902affd9ece0ba8ba1"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/163/questions
Content-Type: application/json
Authorization: Bearer 03682b7244aff30fd7c2b52c48eea8bda3c80807cde345e6d125ed54ba7cedd0
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":163,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 91,
    "obfuscated_id": "EqPpyB0JN58",
    "author_id": 776,
    "chapter_id": 163,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:54.570Z",
    "created_at": "2016-11-08T14:21:54.570Z",
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
        "id": 182,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 183,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 184,
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
curl "api.goskive.com/v2/chapters/163/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":163,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03682b7244aff30fd7c2b52c48eea8bda3c80807cde345e6d125ed54ba7cedd0"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/162/questions
Content-Type: application/json
Authorization: Bearer d3db5a36ee1fc20a5fcb7439a55cf554fe2ef363265502108cfb4d30c758076d
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 770,
      "chapter_id": 162,
      "position": 79,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:53.950Z",
      "created_at": "2016-11-08T14:21:53.835Z",
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
          "id": 176,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 177,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 771,
      "chapter_id": 162,
      "position": 80,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:54.138Z",
      "created_at": "2016-11-08T14:21:54.020Z",
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
          "id": 178,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 179,
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
      "author_id": 772,
      "chapter_id": 162,
      "position": 81,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T14:21:54.328Z",
      "created_at": "2016-11-08T14:21:54.209Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/162/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3db5a36ee1fc20a5fcb7439a55cf554fe2ef363265502108cfb4d30c758076d"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/24
Content-Type: application/json
Authorization: Bearer 7736c5b5f9426c635cee2a5a56ead7480a62b2d469a559971a5d4ab42ae9b6ba
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
curl "api.goskive.com/v2/chapters/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7736c5b5f9426c635cee2a5a56ead7480a62b2d469a559971a5d4ab42ae9b6ba"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/25
Content-Type: application/json
Authorization: Bearer 5495bbc938db4031afa2275383a388251bd1cffb56d77680eaf725c05c37c62c
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
curl "api.goskive.com/v2/chapters/25" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5495bbc938db4031afa2275383a388251bd1cffb56d77680eaf725c05c37c62c"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/21
Content-Type: application/json
Authorization: Bearer 895b97e8f3377e495071e55fa129243da235599dcadf31f7e7a4442341a31dd5
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
curl "api.goskive.com/v2/chapters/21" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 895b97e8f3377e495071e55fa129243da235599dcadf31f7e7a4442341a31dd5"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/26
Content-Type: application/json
Authorization: Bearer 0e42a923d0e8ec771025b397cafdeccd7f5fc7249e9ea8f6494c1838f4617609
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/26" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e42a923d0e8ec771025b397cafdeccd7f5fc7249e9ea8f6494c1838f4617609"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/27
Content-Type: application/json
Authorization: Bearer d5b6eed2d23d434af3f5dcabe3cd3e8c3659a3b606f289243c7cd6f81128df9e
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
    "id": 27,
    "updated_at": "2016-11-08T14:21:07.135Z",
    "course_id": 41,
    "author_id": 139,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-08T14:21:06.619Z",
    "questions_updated_at": "2016-11-08T14:21:06.619Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 143,
        "chapter_id": 27,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.118Z",
        "created_at": "2016-11-08T14:21:07.118Z",
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
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 141,
        "chapter_id": 27,
        "position": 9,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:21:07.016Z",
        "created_at": "2016-11-08T14:21:06.897Z",
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
            "id": 17,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 18,
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
curl "api.goskive.com/v2/chapters/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5b6eed2d23d434af3f5dcabe3cd3e8c3659a3b606f289243c7cd6f81128df9e"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/22
Content-Type: application/json
Authorization: Bearer 2876e1f6ac7b3e256f6be3eed221ccd2deea5d39a0744ad4f87f9c2839ad5907
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
    "id": 22,
    "updated_at": "2016-11-08T14:21:05.549Z",
    "course_id": 36,
    "author_id": 125,
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
curl "api.goskive.com/v2/chapters/22" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2876e1f6ac7b3e256f6be3eed221ccd2deea5d39a0744ad4f87f9c2839ad5907"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/12/replies
Content-Type: application/json
Authorization: Bearer 68a9ea54df085b0f2cce6960d1078900d056b8665fcd0ee59b19789acfaf901e
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
    "id": 13,
    "author_id": 318,
    "reply_to_id": 12,
    "created_at": "2016-11-08T14:21:18.361Z",
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
curl "api.goskive.com/v2/comments/12/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68a9ea54df085b0f2cce6960d1078900d056b8665fcd0ee59b19789acfaf901e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/11/replies
Content-Type: application/json
Authorization: Bearer 837264978c57ef48c7686d52198b298a9e1382a21f9a5af1325298313bbf1dc2
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
curl "api.goskive.com/v2/comments/11/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 837264978c57ef48c7686d52198b298a9e1382a21f9a5af1325298313bbf1dc2"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer 46642c273ae1ebf61396347da334654be6d5dc542ca0ec145bdb05980a6048ef
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
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46642c273ae1ebf61396347da334654be6d5dc542ca0ec145bdb05980a6048ef"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/17/republish
Content-Type: application/json
Authorization: Bearer db9b58b66ab4a4026d41f9a93e62c075bbc14e35f0b164fcd0e2bd66031a7167
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
curl "api.goskive.com/v2/comments/17/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db9b58b66ab4a4026d41f9a93e62c075bbc14e35f0b164fcd0e2bd66031a7167"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer 7da3c79a0fce6e6bf190f4a0c146aa62c2ea135755c2ba29bef5ed35fd20add5
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7da3c79a0fce6e6bf190f4a0c146aa62c2ea135755c2ba29bef5ed35fd20add5"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/16/report
Content-Type: application/json
Authorization: Bearer 501b51afc7b088ae135f0799c2bfd409f4cf80ef01a13368e216da21562e655c
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 501b51afc7b088ae135f0799c2bfd409f4cf80ef01a13368e216da21562e655c"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/32
Content-Type: application/json
Authorization: Bearer 2da679dec2a1ae91644de17f19199ce1382abb090e65635e0bc86e9c952cf5d3
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
    "id": 32,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/4827d71e510ab6acd29eb9520c31ac72b53161f6.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-08T14:21:13.396Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/32" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2da679dec2a1ae91644de17f19199ce1382abb090e65635e0bc86e9c952cf5d3"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 6bdf3eaa23a0416aecfc50d5ec1e220bb4e8558a8d9208f7ecb2a2aaedc5b0d5
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
      "id": 30,
      "name": "Fake Company Name 30",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T14:21:13.277Z"
    },
    {
      "id": 31,
      "name": "Fake Company Name 31",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/0df235007210ab1331461f6a10296cd43f327e64.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T14:21:13.280Z"
    },
    {
      "id": 29,
      "name": "Fake Company Name 29",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/eb30fd9939333e805126ba26a8736769f7ca2ba6.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T14:21:13.273Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bdf3eaa23a0416aecfc50d5ec1e220bb4e8558a8d9208f7ecb2a2aaedc5b0d5"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/39/company_profiles
Content-Type: application/json
Authorization: Bearer b5bd2b7e1ae4c7f25375809d5ce883d8e10e73d04eb2fb2a8af26972756d8580
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
curl "api.goskive.com/v2/companies/39/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5bd2b7e1ae4c7f25375809d5ce883d8e10e73d04eb2fb2a8af26972756d8580"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 1ae64b0cc8ef95b91e020d235b33685ce8617e4b2c28fb2a65fa456bc4b32ba2
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
	-H "Authorization: Bearer 1ae64b0cc8ef95b91e020d235b33685ce8617e4b2c28fb2a65fa456bc4b32ba2"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 6ba64ad929c00642dbc20c2cbcd410647bdafdf8aa541e4b938b33c1582c69ba
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
	-H "Authorization: Bearer 6ba64ad929c00642dbc20c2cbcd410647bdafdf8aa541e4b938b33c1582c69ba"
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
Authorization: Bearer 37f721b60eabcecdb65ad84935df7c410e6c43af94295dabcee77b5b522cc775
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
	-H "Authorization: Bearer 37f721b60eabcecdb65ad84935df7c410e6c43af94295dabcee77b5b522cc775"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6f9e40f1eb14e8277d49828b26e4af0001bf33b20a5c11db8900d4ff7abf52d4
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
    "updated_at": "2016-11-08T14:21:10.851Z",
    "course_id": 57,
    "author_id": 205,
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
	-H "Authorization: Bearer 6f9e40f1eb14e8277d49828b26e4af0001bf33b20a5c11db8900d4ff7abf52d4"
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
      "id": 38,
      "updated_at": "2016-11-08T14:21:09.277Z",
      "course_id": 50,
      "author_id": 178,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 29",
      "position": 1
    },
    {
      "id": 39,
      "updated_at": "2016-11-08T14:21:09.300Z",
      "course_id": 50,
      "author_id": 179,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 30",
      "position": 2
    },
    {
      "id": 40,
      "updated_at": "2016-11-08T14:21:09.554Z",
      "course_id": 50,
      "author_id": 180,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T14:21:09.208Z",
      "questions_updated_at": "2016-11-08T14:21:09.208Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 31",
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
Authorization: Bearer 360e7d63ad4129f8afc011d76b25eb56ed2d664655a751507c50c807fe0d11db
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
      "id": 44,
      "updated_at": "2016-11-08T14:21:09.911Z",
      "course_id": 53,
      "author_id": 189,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 35",
      "position": 1
    },
    {
      "id": 45,
      "updated_at": "2016-11-08T14:21:09.934Z",
      "course_id": 53,
      "author_id": 190,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 36",
      "position": 2
    },
    {
      "id": 46,
      "updated_at": "2016-11-08T14:21:10.189Z",
      "course_id": 53,
      "author_id": 191,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T14:21:09.840Z",
      "questions_updated_at": "2016-11-08T14:21:09.840Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 37",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 360e7d63ad4129f8afc011d76b25eb56ed2d664655a751507c50c807fe0d11db"
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
      "id": 41,
      "updated_at": "2016-11-08T14:21:09.751Z",
      "course_id": 52,
      "author_id": 185,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 32",
      "position": 1
    },
    {
      "id": 42,
      "updated_at": "2016-11-08T14:21:09.774Z",
      "course_id": 52,
      "author_id": 186,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 33",
      "position": 2
    },
    {
      "id": 43,
      "updated_at": "2016-11-08T14:21:09.796Z",
      "course_id": 52,
      "author_id": 187,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 34",
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
Authorization: Bearer 48b5fee46d85f8428f58c1b8d328217318eb66285b6e89d4b57119e44b9953ad
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
      "id": 47,
      "updated_at": "2016-11-08T14:21:10.343Z",
      "course_id": 54,
      "author_id": 196,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 38",
      "position": 1
    },
    {
      "id": 48,
      "updated_at": "2016-11-08T14:21:10.367Z",
      "course_id": 54,
      "author_id": 197,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 39",
      "position": 2
    },
    {
      "id": 49,
      "updated_at": "2016-11-08T14:21:10.392Z",
      "course_id": 54,
      "author_id": 198,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 40",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48b5fee46d85f8428f58c1b8d328217318eb66285b6e89d4b57119e44b9953ad"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 2c531a37e8b96559a05d4f28a6cc0280b8ed79c09058f4320d895d0f35f3f05a
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
    "course_id": 11,
    "user_id": 32,
    "updated_at": "2016-11-08T14:20:59.792Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c531a37e8b96559a05d4f28a6cc0280b8ed79c09058f4320d895d0f35f3f05a"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 1da4994e6dbc1d707e9e322e4d5f865129aad60d48f3977ac5438954794f794d
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
      "course_id": 12,
      "user_id": 34,
      "updated_at": "2016-11-08T14:20:59.874Z"
    },
    {
      "id": 4,
      "course_id": 12,
      "user_id": 35,
      "updated_at": "2016-11-08T14:20:59.888Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1da4994e6dbc1d707e9e322e4d5f865129aad60d48f3977ac5438954794f794d"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/9/files
Content-Type: application/json
Authorization: Bearer e14890922778c514f63c5bcf697be458004c701f9131fb2ba968a14c011580f9
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
        "id": 25,
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
        "created_at": "2016-11-08T14:20:59.403Z",
        "updated_at": "2016-11-08T14:20:59.403Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T14:20:59.416Z",
      "updated_at": "2016-11-08T14:20:59.416Z",
      "course_id": 9,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 26,
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
        "created_at": "2016-11-08T14:20:59.425Z",
        "updated_at": "2016-11-08T14:20:59.425Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T14:20:59.434Z",
      "updated_at": "2016-11-08T14:20:59.434Z",
      "course_id": 9,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 27,
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
        "created_at": "2016-11-08T14:20:59.441Z",
        "updated_at": "2016-11-08T14:20:59.441Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T14:20:59.449Z",
      "updated_at": "2016-11-08T14:20:59.449Z",
      "course_id": 9,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/9/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e14890922778c514f63c5bcf697be458004c701f9131fb2ba968a14c011580f9"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/7/files
Content-Type: application/json
Authorization: Bearer 8f480e92290da0ec28f6a90a4620474012392523c0c8eef48f7da241309da48f
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
      "id": 21,
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
      "created_at": "2016-11-08T14:20:59.051Z",
      "updated_at": "2016-11-08T14:20:59.051Z"
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
    "created_at": "2016-11-08T14:20:59.111Z",
    "updated_at": "2016-11-08T14:20:59.111Z",
    "course_id": 7,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/7/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f480e92290da0ec28f6a90a4620474012392523c0c8eef48f7da241309da48f"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/6/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 182824955f2ca53fbcce429c523d4110739d1e6a07364f24654294bf65875356
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
    "key": "cache/776bc6eddfc8307b9c74d779d16b9c8a.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQxNToyMDo1OFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzc3NmJjNmVkZGZjODMwN2I5Yzc0ZDc3OWQxNmI5YzhhLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA4VDE0MjA1OFoifV19",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T142058Z",
    "x-amz-signature": "5518e4ad2ddf47581544bec4e549cdcaf9d0097a9e2194dc0b3da56dcf899900"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/6/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 182824955f2ca53fbcce429c523d4110739d1e6a07364f24654294bf65875356"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 72f97badddff56b8368492312a1ed6fa242c08363ac32df66b5c710521acc6da
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
	-H "Authorization: Bearer 72f97badddff56b8368492312a1ed6fa242c08363ac32df66b5c710521acc6da"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a002c217d8fed861de7420354ccf53969742eee47c20777cac7c7decc3a8dc09
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
	-H "Authorization: Bearer a002c217d8fed861de7420354ccf53969742eee47c20777cac7c7decc3a8dc09"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 505fa91acdf23169785015e8f50c09a5636a04eabfcb72a987f939fea3cb3301
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
	-H "Authorization: Bearer 505fa91acdf23169785015e8f50c09a5636a04eabfcb72a987f939fea3cb3301"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f91c1ed4175f0934e1b42cebcf2da5569e2991d738d712dc8bb12065cf4a266f
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
	-H "Authorization: Bearer f91c1ed4175f0934e1b42cebcf2da5569e2991d738d712dc8bb12065cf4a266f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b436fb3c4bcdc68d20b2a7f777dc3b943a4f907c1cf9db05cc430eed4111b201
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
	-H "Authorization: Bearer b436fb3c4bcdc68d20b2a7f777dc3b943a4f907c1cf9db05cc430eed4111b201"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 0dc384608b1a088d7e77c3387888ebe2135aa5e10a848eeb5303ed619ad7e040
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
    "creator_id": 963,
    "id": 313,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 297,
    "additional_university_ids": [

    ],
    "discipline_id": 324,
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
    "chapters_updated_at": "2016-11-08T14:22:12.969Z",
    "updated_at": "2016-11-08T14:22:14.362Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 964,
        "chapter_id": 190,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:14.168Z",
        "created_at": "2016-11-08T14:22:14.168Z",
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
        "author_id": 964,
        "chapter_id": 191,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:14.235Z",
        "created_at": "2016-11-08T14:22:14.235Z",
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
        "author_id": 964,
        "chapter_id": 190,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:14.206Z",
        "created_at": "2016-11-08T14:22:14.206Z",
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
        "author_id": 964,
        "chapter_id": 191,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:14.272Z",
        "created_at": "2016-11-08T14:22:14.272Z",
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
        "id": 117,
        "obfuscated_id": "BsA8mEPn8aM",
        "author_id": 964,
        "chapter_id": 190,
        "position": 104,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:13.176Z",
        "created_at": "2016-11-08T14:22:13.062Z",
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
        "author_id": 964,
        "chapter_id": 190,
        "position": 105,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:13.347Z",
        "created_at": "2016-11-08T14:22:13.236Z",
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
      },
      {
        "id": 119,
        "obfuscated_id": "JRh8sWka24Y",
        "author_id": 964,
        "chapter_id": 191,
        "position": 106,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:13.545Z",
        "created_at": "2016-11-08T14:22:13.426Z",
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
            "id": 241,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 242,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 120,
        "obfuscated_id": "vEr9LtFjURM",
        "author_id": 964,
        "chapter_id": 191,
        "position": 107,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:13.723Z",
        "created_at": "2016-11-08T14:22:13.609Z",
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
            "id": 243,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 244,
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
        "id": 190,
        "updated_at": "2016-11-08T14:22:14.318Z",
        "course_id": 313,
        "author_id": 963,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T14:22:12.969Z",
        "questions_updated_at": "2016-11-08T14:22:12.969Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 166",
        "position": 1
      },
      {
        "id": 191,
        "updated_at": "2016-11-08T14:22:14.355Z",
        "course_id": 313,
        "author_id": 963,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T14:22:12.969Z",
        "questions_updated_at": "2016-11-08T14:22:12.969Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 167",
        "position": 2
      }
    ],
    "topic_id": 323,
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
	-H "Authorization: Bearer 0dc384608b1a088d7e77c3387888ebe2135aa5e10a848eeb5303ed619ad7e040"
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
    "creator_id": 969,
    "id": 314,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 298,
    "additional_university_ids": [

    ],
    "discipline_id": 325,
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
    "chapters_updated_at": "2016-11-08T14:22:14.482Z",
    "updated_at": "2016-11-08T14:22:15.901Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 123,
        "obfuscated_id": "N9-wuAhut60",
        "author_id": 969,
        "chapter_id": 192,
        "position": 110,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:14.698Z",
        "created_at": "2016-11-08T14:22:14.579Z",
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
            "id": 249,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 250,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 125,
        "obfuscated_id": "K6zw0Yc6Me8",
        "author_id": 969,
        "chapter_id": 193,
        "position": 112,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T14:22:15.071Z",
        "created_at": "2016-11-08T14:22:14.953Z",
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
            "id": 253,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 254,
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
        "id": 192,
        "updated_at": "2016-11-08T14:22:15.856Z",
        "course_id": 314,
        "author_id": 969,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T14:22:14.482Z",
        "questions_updated_at": "2016-11-08T14:22:14.482Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 168",
        "position": 1
      },
      {
        "id": 193,
        "updated_at": "2016-11-08T14:22:15.893Z",
        "course_id": 314,
        "author_id": 969,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T14:22:14.482Z",
        "questions_updated_at": "2016-11-08T14:22:14.482Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 169",
        "position": 2
      }
    ],
    "topic_id": 324,
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
PUT /v2/courses/302/pin
Content-Type: application/json
Authorization: Bearer 70eb9884c66b50df39c9272d609da3c04f71eee14fcabfdd407cb78fe40126d7
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/302/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70eb9884c66b50df39c9272d609da3c04f71eee14fcabfdd407cb78fe40126d7"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/316/pin
Content-Type: application/json
Authorization: Bearer 02c9972d449e236e0fd15cb5b58ebd85e71abb983cb56d55bc490ddd35ead6b2
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/316/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02c9972d449e236e0fd15cb5b58ebd85e71abb983cb56d55bc490ddd35ead6b2"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c23260a0dc16828137bd23e1079a3c17402726083964512f25a62c58f53cb309
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
    "creator_id": 930,
    "id": 299,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 283,
    "additional_university_ids": [

    ],
    "discipline_id": 310,
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
    "updated_at": "2016-11-08T14:22:09.500Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 309,
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
	-H "Authorization: Bearer c23260a0dc16828137bd23e1079a3c17402726083964512f25a62c58f53cb309"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 6c7f7567cf5e86e4ed1fd6d74d665c0417b7fe4741997f18b66242a8ee2dbfab
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
    "id": 585,
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
    "created_at": "2016-11-08T14:21:41.088Z",
    "updated_at": "2016-11-08T14:21:41.088Z",
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
	-H "Authorization: Bearer 6c7f7567cf5e86e4ed1fd6d74d665c0417b7fe4741997f18b66242a8ee2dbfab"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ab5e5550745f937bbe6591f8a4e579b51d3e9d9d0969db2efcd70f5428a27922
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[186]}
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
    "id": 586,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      186
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T14:21:41.175Z",
    "updated_at": "2016-11-08T14:21:41.213Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[186]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab5e5550745f937bbe6591f8a4e579b51d3e9d9d0969db2efcd70f5428a27922"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 340244cfb1d53dab4e6015720053f0918e717a3e1d744fccaa0a8f09fc21f005
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
    "id": 589,
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
    "created_at": "2016-11-08T14:21:41.375Z",
    "updated_at": "2016-11-08T14:21:41.375Z",
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
	-H "Authorization: Bearer 340244cfb1d53dab4e6015720053f0918e717a3e1d744fccaa0a8f09fc21f005"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c16b0e9e92a8cb6b979640b479ff124ea2fe5cfbc8ce02e6d7ed97ad4a88c715
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[187]}
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
    "id": 587,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      187
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T14:21:41.254Z",
    "updated_at": "2016-11-08T14:21:41.254Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[187]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c16b0e9e92a8cb6b979640b479ff124ea2fe5cfbc8ce02e6d7ed97ad4a88c715"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 7356d3115b05df0e85180718d41ead579cef076c6ba0ab96b18d5a1f614dd61d
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

190
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
    "id": 590,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/04b1018bedcd06dba69ba04ad495473324183168.jpg",
    "university_id": null,
    "fields_of_study": [
      190
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T14:21:41.466Z",
    "updated_at": "2016-11-08T14:21:41.741Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/1c98e027b16b8694a49dc2f0f6c3bd45b3a57ba8.jpg",
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

190
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 7356d3115b05df0e85180718d41ead579cef076c6ba0ab96b18d5a1f614dd61d"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 27156ca31fbfc6e4cc153531ff0ad4f39026448a324b70b9cb42aa7a402e2f71
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
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27156ca31fbfc6e4cc153531ff0ad4f39026448a324b70b9cb42aa7a402e2f71"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer ddd8856dff7a99de39a450dfe2fb8fd38cb79bcf9a1063707b8121b39d92fd82
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
      "company_id": 25,
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
      "company_id": 26,
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
	-H "Authorization: Bearer ddd8856dff7a99de39a450dfe2fb8fd38cb79bcf9a1063707b8121b39d92fd82"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer a27941460713e149365b328658bbba19225ea64b4d5b6137fc37b57f4cdb7baf
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
      "company_id": 21,
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
	-H "Authorization: Bearer a27941460713e149365b328658bbba19225ea64b4d5b6137fc37b57f4cdb7baf"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d6884d84ae3ec59233fde9d1da7f56beb85711f294bd6c614c75d27a1dc8d16d
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
      "creator_id": 153,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-24",
      "html_url": "https://goskive.com/course/mit-course-24",
      "slug": "mit-course-24",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "discipline_id": 46,
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
      "updated_at": "2016-11-08T14:21:07.934Z",
      "shortname": "mit-course-24",
      "topic_id": 46,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 154,
      "id": 44,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-25",
      "html_url": "https://goskive.com/course/mit-course-25",
      "slug": "mit-course-25",
      "university_id": 44,
      "additional_university_ids": [

      ],
      "discipline_id": 47,
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
      "updated_at": "2016-11-08T14:21:08.008Z",
      "shortname": "mit-course-25",
      "topic_id": 47,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 25",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6884d84ae3ec59233fde9d1da7f56beb85711f294bd6c614c75d27a1dc8d16d"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer d8d2fc7b4c6b202a329006da64171ef494ff0dbcc72a1e8a50705fe59c5eef7c
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
        "created_at": "2016-11-08T14:21:29.227Z",
        "updated_at": "2016-11-08T14:21:29.227Z",
        "file_url": "memory://bceca9abce1a7a9fb7b1cdb8016d3f90.pdf",
        "course_id": 118,
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
        "created_at": "2016-11-08T14:21:29.310Z",
        "updated_at": "2016-11-08T14:21:29.310Z",
        "file_url": "memory://1fe93b5cdd77b04bef6f6d2cae0d7f19.pdf",
        "course_id": 119,
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
        "created_at": "2016-11-08T14:21:29.388Z",
        "updated_at": "2016-11-08T14:21:29.388Z",
        "file_url": "memory://7ba276304c82b3d0391a97a3172b6f62.pdf",
        "course_id": 120,
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
	-H "Authorization: Bearer d8d2fc7b4c6b202a329006da64171ef494ff0dbcc72a1e8a50705fe59c5eef7c"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 3144ea2d4f60769a3ab055a7db957f3a4d2a0300fa0ee267d40984f6bb728f8c
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T14:21:01.345Z"
      },
      "created_at": "2016-11-08T14:21:01.348Z",
      "updated_at": "2016-11-08T14:21:01.348Z",
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
      "company_id": 19,
      "company": {
        "id": 19,
        "name": "Fake Company Name 19",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T14:21:01.356Z"
      },
      "created_at": "2016-11-08T14:21:01.359Z",
      "updated_at": "2016-11-08T14:21:01.359Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3144ea2d4f60769a3ab055a7db957f3a4d2a0300fa0ee267d40984f6bb728f8c"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cf45b890094a3105fcf98596de158695bea1e33f562e5157a963170bdbc647bb
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T14:21:01.123Z"
      },
      "created_at": "2016-11-08T14:21:01.127Z",
      "updated_at": "2016-11-08T14:21:01.127Z",
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
      "company_id": 15,
      "company": {
        "id": 15,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T14:21:01.139Z"
      },
      "created_at": "2016-11-08T14:21:01.143Z",
      "updated_at": "2016-11-08T14:21:01.143Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf45b890094a3105fcf98596de158695bea1e33f562e5157a963170bdbc647bb"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer ace8f20ab54980b69a0e56611ab4bfb6b9017180480db932360c2ed7603d27b1
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
      "id": 18,
      "created_at": "2016-11-08T14:21:57.269Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-11-08T14:21:57.372Z",
      "author_id": "795",
      "thread_subject_id": "234",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 19,
      "created_at": "2016-11-08T14:21:57.361Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 60,
      "updated_at": "2016-11-08T14:21:57.375Z",
      "author_id": "798",
      "thread_subject_id": "235",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-11-08T14:21:57.727Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-11-08T14:21:57.727Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 21,
      "created_at": "2016-11-08T14:21:58.130Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-08T14:21:58.130Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 22,
      "created_at": "2016-11-08T14:21:58.492Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-11-08T14:21:58.492Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 23,
      "created_at": "2016-11-08T14:21:58.779Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 99,
      "updated_at": "2016-11-08T14:21:58.779Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-11-08T14:21:59.073Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 100,
      "updated_at": "2016-11-08T14:21:59.073Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-11-08T14:21:59.363Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 101,
      "updated_at": "2016-11-08T14:21:59.363Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ace8f20ab54980b69a0e56611ab4bfb6b9017180480db932360c2ed7603d27b1"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/17
Content-Type: application/json
Authorization: Bearer 4a95abd7ecea0442de8744130c8ca010a79bea3ec7a1b22886ee3cf98ff62050
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-08T14:11:57.000Z"}}
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
    "id": 17,
    "created_at": "2016-11-08T14:21:57.109Z",
    "read_at": "2016-11-08T14:11:57.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-11-08T14:21:57.163Z",
    "author_id": "791",
    "thread_subject_id": "233",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/17" -d '{"notification":{"read_at":"2016-11-08T14:11:57.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a95abd7ecea0442de8744130c8ca010a79bea3ec7a1b22886ee3cf98ff62050"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3c314a5d76194b05c0f377e3278e45cfaafcf2e4206e464f29b375b20a999e7f
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
      "course_id": 190,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T14:21:43.738Z",
      "course_published": true,
      "updated_at": "2016-11-08T14:21:43.731Z"
    },
    {
      "id": 6,
      "course_id": 191,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T14:21:43.817Z",
      "course_published": true,
      "updated_at": "2016-11-08T14:21:43.809Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c314a5d76194b05c0f377e3278e45cfaafcf2e4206e464f29b375b20a999e7f"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 5690fb3ba8f2d52ec29a6a760713d8598049d5ffa8e5b820de284a29cec1698c
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
    "course_id": 189,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T14:21:43.625Z",
    "course_published": true,
    "updated_at": "2016-11-08T14:21:43.618Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5690fb3ba8f2d52ec29a6a760713d8598049d5ffa8e5b820de284a29cec1698c"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer 6da927e6608f3e925512c3eef917deaa76c68448b7c7218c99bf41ab36393c2a
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
    "course_id": 192,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-08T14:21:44.073Z",
    "course_published": true,
    "updated_at": "2016-11-08T14:21:44.062Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6da927e6608f3e925512c3eef917deaa76c68448b7c7218c99bf41ab36393c2a"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3fb03eef7568168940ebf536671fade3c1bb76121ba97438b6bcc87cd776c730
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
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 84,
      "user_id": 752
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 85,
      "user_id": 752
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 86,
      "user_id": 752
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 87,
      "user_id": 752
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fb03eef7568168940ebf536671fade3c1bb76121ba97438b6bcc87cd776c730"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/50
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
    "id": 50,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 48,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 50
      },
      {
        "id": 49,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 50
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/50" -X GET \
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
      "id": 48,
      "name": "Cloned impactful utilisation",
      "name_translations": {
        "en": "Cloned impactful utilisation"
      }
    },
    {
      "id": 49,
      "name": "Phased didactic standardization",
      "name_translations": {
        "en": "Phased didactic standardization"
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
Authorization: Bearer e582bd68e68ec56120e816ae086d04d7fb4fc4b1a932e6b54cc7be71b9055bb4
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
    "user_id": 719,
    "feedbackable_id": 59,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-08T14:21:50.398Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/40/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e582bd68e68ec56120e816ae086d04d7fb4fc4b1a932e6b54cc7be71b9055bb4"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/45/fix
Content-Type: application/json
Authorization: Bearer 392f270f1063cbdb5ee58b930314d362c9cf34b8db4062a6bed9cc2b40156d81
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
    "id": 45,
    "user_id": 744,
    "feedbackable_id": 64,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-08T14:21:51.725Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/45/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 392f270f1063cbdb5ee58b930314d362c9cf34b8db4062a6bed9cc2b40156d81"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer 4bebe1de2665eab145ca4b5f1b5a3ee5450911545f18044342dea1f1b2ab7746
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
    "user_id": 626,
    "feedbackable_id": 57,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T14:21:44.224Z",
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
	-H "Authorization: Bearer 4bebe1de2665eab145ca4b5f1b5a3ee5450911545f18044342dea1f1b2ab7746"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/close
Content-Type: application/json
Authorization: Bearer e60b77675b10882c16f345ff96ed5fd008d1ead68afdcf7e42de509bc577b4ea
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
	-H "Authorization: Bearer e60b77675b10882c16f345ff96ed5fd008d1ead68afdcf7e42de509bc577b4ea"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 5c8140ea6ee110fbc937e86485a5ba306e2a3ee3e8bf079bd529fcee983f5552
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
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c8140ea6ee110fbc937e86485a5ba306e2a3ee3e8bf079bd529fcee983f5552"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/fix
Content-Type: application/json
Authorization: Bearer f723db8166e9ff3b018090c890c30ca273edea2eff88fb0ddb08a8f99347c8f7
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
	-H "Authorization: Bearer f723db8166e9ff3b018090c890c30ca273edea2eff88fb0ddb08a8f99347c8f7"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 89c735f5cd22938e2c20b31eb1a4741d8470a50a4465735e9e51e94277b0e878
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
    "user_id": 631,
    "feedbackable_id": 58,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T14:21:44.485Z",
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
	-H "Authorization: Bearer 89c735f5cd22938e2c20b31eb1a4741d8470a50a4465735e9e51e94277b0e878"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer 67f367f1aac94454727f302472e7a77889aedb6d0a9ad8019fb1a52e261154fa
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
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67f367f1aac94454727f302472e7a77889aedb6d0a9ad8019fb1a52e261154fa"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/21/bookmark
Content-Type: application/json
Authorization: Bearer 0917512bf5a4f3364630470bfd5823316ef6bc019cb03c57a37ca2fb3dd5ddd3
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
	-H "Authorization: Bearer 0917512bf5a4f3364630470bfd5823316ef6bc019cb03c57a37ca2fb3dd5ddd3"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer aac41af46dbba208176c15fb8e083725124fe40a18af40ced67430a86714fe83
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aac41af46dbba208176c15fb8e083725124fe40a18af40ced67430a86714fe83"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/16
Content-Type: application/json
Authorization: Bearer 950f0733876471fd0851793258fa267aaeebd6af614409efc4b61a44ef56b28b
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/c56e9e8750060e4a9ed32761e25833de.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T142208Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d3d6e59bd81d525167d68997fa8cf28138afb2d8b12f8b5c928c3e4af1c169aa",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 950f0733876471fd0851793258fa267aaeebd6af614409efc4b61a44ef56b28b"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer 5b8deab90344d0616ec1ed61da3929abfb150de7bcea580a59278017ab7e7c74
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b9e3b4f35d825cd633d305e58060de21.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T142208Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a19d2c82e6b440d621a19eb02951d5ad49a4b8f8ad2e57215a802881ea4dac04",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/14/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b8deab90344d0616ec1ed61da3929abfb150de7bcea580a59278017ab7e7c74"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/19/metadata
Content-Type: application/json
Authorization: Bearer 71936bca956eaf9d09eeb5893dfdc0f7ab24d4c2353bdb8506981f53c6dbdf59
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
    "id": 19,
    "uploader": {
      "id": 916,
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
      "created_at": "2016-11-08T14:22:08.730Z",
      "updated_at": "2016-11-08T14:22:08.730Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-08T14:22:08.800Z",
    "updated_at": "2016-11-08T14:22:08.800Z",
    "course_id": 294,
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
curl "api.goskive.com/v2/files/19/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71936bca956eaf9d09eeb5893dfdc0f7ab24d4c2353bdb8506981f53c6dbdf59"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/8/matched_courses?required_cu_count=2
Authorization: Bearer 986a3b6228dd85b3c0a0eee9cfd366da3a12eba97d7376bea63c0d0b201ae03e
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
      "creator_id": 433,
      "id": 124,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "discipline_id": 130,
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
      "chapters_updated_at": "2016-11-08T14:21:29.449Z",
      "updated_at": "2016-11-08T14:21:32.015Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 129,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 438,
      "id": 125,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-0fc7864f-0c97-4c9a-8bf0-91d65fdad445",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-0fc7864f-0c97-4c9a-8bf0-91d65fdad445",
      "slug": "mit-the-great-british-bake-off-0fc7864f-0c97-4c9a-8bf0-91d65fdad445",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "discipline_id": 131,
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
      "chapters_updated_at": "2016-11-08T14:21:29.449Z",
      "updated_at": "2016-11-08T14:21:32.649Z",
      "shortname": "mit-the-great-british-bake-off-0fc7864f-0c97-4c9a-8bf0-91d65fdad445",
      "topic_id": 130,
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
	-H "Authorization: Bearer 986a3b6228dd85b3c0a0eee9cfd366da3a12eba97d7376bea63c0d0b201ae03e"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/15/download
Content-Type: application/json
Authorization: Bearer 76f7aada4d3270d7e7f271e73adb8e4d392b3f6673159f7c483f480f74eac2bc
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
	-H "Authorization: Bearer 76f7aada4d3270d7e7f271e73adb8e4d392b3f6673159f7c483f480f74eac2bc"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/13/report
Content-Type: application/json
Authorization: Bearer d156c79f1ebe9524ee07d580e34a14808b492e88cafa8a7214ca71a6be171974
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d156c79f1ebe9524ee07d580e34a14808b492e88cafa8a7214ca71a6be171974"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/22/bookmark
Content-Type: application/json
Authorization: Bearer ac2ba549ef251a999966593554710c3ebfb291156dafdd4b7c8358cb3cc597fa
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/22/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac2ba549ef251a999966593554710c3ebfb291156dafdd4b7c8358cb3cc597fa"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/20/upvote
Content-Type: application/json
Authorization: Bearer fecd0e5ac6b5882f109608a631289677f186ea01aed17407bb150550b121ce1f
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fecd0e5ac6b5882f109608a631289677f186ea01aed17407bb150550b121ce1f"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer e8c8292e98d61f97de0b22715ef8ff4b27ea2ae4ae375800f59259a8b5fee7f4
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
    "author_id": 101,
    "reply_to_id": null,
    "created_at": "2016-11-08T14:21:04.107Z",
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
curl "api.goskive.com/v2/flashcards/10/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8c8292e98d61f97de0b22715ef8ff4b27ea2ae4ae375800f59259a8b5fee7f4"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer dabd79ec8e553d4af8e5995e76cbb01e81c85d0f0276860b29e99b1a5be5e392
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
    "id": 8,
    "author_id": 107,
    "reply_to_id": null,
    "created_at": "2016-11-08T14:21:04.544Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 107,
      "feedbackable_id": 12,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:04.542Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dabd79ec8e553d4af8e5995e76cbb01e81c85d0f0276860b29e99b1a5be5e392"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer a867f3415228897d56fb6e387e6eb4288cbe720a25b0e81d72c749380843d65c
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
      "id": 10,
      "author_id": 114,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:04.834Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 113,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:21:04.820Z",
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
curl "api.goskive.com/v2/flashcards/13/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a867f3415228897d56fb6e387e6eb4288cbe720a25b0e81d72c749380843d65c"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer acc19261aed51bc9da79273c297295eb01fc0b1b976e120570bf76496e865cb3
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
	-H "Authorization: Bearer acc19261aed51bc9da79273c297295eb01fc0b1b976e120570bf76496e865cb3"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/9/feedbacks
Content-Type: application/json
Authorization: Bearer d186503b3ad05074595418da210a03d903390b17d4e6fd3efc1ae12fa0b6d7d3
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
    "id": 9,
    "user_id": 92,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T14:21:03.422Z",
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
curl "api.goskive.com/v2/flashcards/9/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d186503b3ad05074595418da210a03d903390b17d4e6fd3efc1ae12fa0b6d7d3"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/4/feedbacks
Content-Type: application/json
Authorization: Bearer 4803b5a79c86a9c46694cb43eeea81b79dc461562c6e09613673955260bef0c5
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
      "id": 5,
      "user_id": 71,
      "feedbackable_id": 4,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:02.268Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 70,
      "feedbackable_id": 4,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:02.258Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/4/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4803b5a79c86a9c46694cb43eeea81b79dc461562c6e09613673955260bef0c5"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/46/votes
Content-Type: application/json
Authorization: Bearer 9649c6b380d93d4206a4242dc8f14a4f2c62b076b7263be73bcf479f442ea585
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
      "votable_id": 46,
      "user_id": 328
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 46,
      "user_id": 327
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 46,
      "user_id": 326
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/46/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9649c6b380d93d4206a4242dc8f14a4f2c62b076b7263be73bcf479f442ea585"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/23/republish
Content-Type: application/json
Authorization: Bearer 0ea357286be904d69eb91a1c8a2ac097d357b1698ed4f49b3e14bc0d8d7e5667
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
curl "api.goskive.com/v2/flashcards/23/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ea357286be904d69eb91a1c8a2ac097d357b1698ed4f49b3e14bc0d8d7e5667"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/43/bookmark
Content-Type: application/json
Authorization: Bearer 648cc81d7ac3e056ce3a938122324a009e90d8baf4fabd2ad2bcff1c176ea2d9
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 648cc81d7ac3e056ce3a938122324a009e90d8baf4fabd2ad2bcff1c176ea2d9"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/40
Content-Type: application/json
Authorization: Bearer e47bb8b5a23f7d9b29e50168dc442ca5c3b77acf4ea2f2dce05e56ca9fa583c2
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e47bb8b5a23f7d9b29e50168dc442ca5c3b77acf4ea2f2dce05e56ca9fa583c2"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/45/downvote
Content-Type: application/json
Authorization: Bearer a12b81d4656db5f6562666b664728755655d4a1beac033b0a2b5f0af667df397
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/45/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a12b81d4656db5f6562666b664728755655d4a1beac033b0a2b5f0af667df397"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/44
Content-Type: application/json
Authorization: Bearer 08144a18fda711f61df005ca9bd9fe1def5aeed2bc95d38d3750081f2d1e5ad9
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
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 303,
    "chapter_id": 79,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:17.308Z",
    "created_at": "2016-11-08T14:21:17.308Z",
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
curl "api.goskive.com/v2/flashcards/44" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08144a18fda711f61df005ca9bd9fe1def5aeed2bc95d38d3750081f2d1e5ad9"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/report
Content-Type: application/json
Authorization: Bearer afdab37ae3042059fe5a4e76d2a2b80a8554cae45c157aa9fae6704aba40bd2c
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afdab37ae3042059fe5a4e76d2a2b80a8554cae45c157aa9fae6704aba40bd2c"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/39/bookmark
Content-Type: application/json
Authorization: Bearer 1c3ab471a4e56ca95c9bc96602cc26b06c71050c64b45b7e54f72277168fbe49
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/39/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c3ab471a4e56ca95c9bc96602cc26b06c71050c64b45b7e54f72277168fbe49"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/41/upvote
Content-Type: application/json
Authorization: Bearer 570d94b593c03b54116031779c55f2f927b449a193266041130b39c90d99075e
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 570d94b593c03b54116031779c55f2f927b449a193266041130b39c90d99075e"
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
    "key": "cache/e9107ab8c35c53938b3e944815310b26.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQxNToyMToxMloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2U5MTA3YWI4YzM1YzUzOTM4YjNlOTQ0ODE1MzEwYjI2LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDhUMTQyMTEyWiJ9XX0=",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T142112Z",
    "x-amz-signature": "37c740bd1b89ccd8b8054059057a6a31660098b66b132b9690ecde142d0fafa4"
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
Authorization: Bearer 6e182a8b1afe4c827213b0f97f4e6a7d57a3542e7faab1cdbe6dec5e65bd0f16
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
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e182a8b1afe4c827213b0f97f4e6a7d57a3542e7faab1cdbe6dec5e65bd0f16"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 430202113d7f1a73be4e34fdd702fb3e6ae6eb323626fbdb6638a7c8858ece11
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
curl "api.goskive.com/v2/me/jobs/7/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 430202113d7f1a73be4e34fdd702fb3e6ae6eb323626fbdb6638a7c8858ece11"
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
{"password":{"reset_password_token":"hmK7C9yjwbwHTHxjDdet","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 883,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-08T14:22:05.685Z",
  "updated_at": "2016-11-08T14:22:06.282Z",
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
  "audit_id": 5628
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"hmK7C9yjwbwHTHxjDdet","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/2/comments
Content-Type: application/json
Authorization: Bearer 797c66f35a99d9533daec98c87b1b43408b12eac86c7c078ec5153a62b157f78
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
    "id": 1,
    "author_id": 4,
    "reply_to_id": null,
    "created_at": "2016-11-08T14:20:57.394Z",
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
curl "api.goskive.com/v2/questions/2/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 797c66f35a99d9533daec98c87b1b43408b12eac86c7c078ec5153a62b157f78"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/3/comments
Content-Type: application/json
Authorization: Bearer c486bad65f852d5572bfb8942974ba73540eb687d879f17ced998b1c0a2e5100
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
    "id": 2,
    "author_id": 7,
    "reply_to_id": null,
    "created_at": "2016-11-08T14:20:58.081Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 7,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:20:58.077Z",
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
curl "api.goskive.com/v2/questions/3/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c486bad65f852d5572bfb8942974ba73540eb687d879f17ced998b1c0a2e5100"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/5/comments
Content-Type: application/json
Authorization: Bearer 8dbfbbfff8f5c20e4a12c1b9926f75b6235add6717652c79a6b5a16d0c2dda5a
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
      "author_id": 17,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:20:58.843Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 16,
      "reply_to_id": null,
      "created_at": "2016-11-08T14:20:58.827Z",
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
curl "api.goskive.com/v2/questions/5/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8dbfbbfff8f5c20e4a12c1b9926f75b6235add6717652c79a6b5a16d0c2dda5a"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/1/comments
Content-Type: application/json
Authorization: Bearer f26c183bb4672929cb0f6d1262aa276afeb1b4733b1ebd1aaa270fd13397aaa0
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
curl "api.goskive.com/v2/questions/1/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f26c183bb4672929cb0f6d1262aa276afeb1b4733b1ebd1aaa270fd13397aaa0"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/55/feedbacks
Content-Type: application/json
Authorization: Bearer 0a6ec3d6d94f926cfa9c6d6c8012d4afe1e9d61751f4660abf8e9aefccc75f09
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
    "id": 12,
    "user_id": 457,
    "feedbackable_id": 55,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-08T14:21:34.833Z",
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
curl "api.goskive.com/v2/questions/55/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a6ec3d6d94f926cfa9c6d6c8012d4afe1e9d61751f4660abf8e9aefccc75f09"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/59/feedbacks
Content-Type: application/json
Authorization: Bearer 8e8342f6c4f522b409b2cb88f9f4dd565b6375f656ed162631e1bfa9748bf674
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
      "id": 16,
      "user_id": 481,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:36.346Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 480,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T14:21:36.336Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/59/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e8342f6c4f522b409b2cb88f9f4dd565b6375f656ed162631e1bfa9748bf674"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/103/votes
Content-Type: application/json
Authorization: Bearer 11eebfd31b1d231fb14995280ddad0f3b3a12c67557ac699ab89702ecef5543a
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 830
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 829
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 828
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/103/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11eebfd31b1d231fb14995280ddad0f3b3a12c67557ac699ab89702ecef5543a"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/30/republish
Content-Type: application/json
Authorization: Bearer a8ce71bb2a8776ecb191fc20d47d788e37cbf52c5a356d25043ec5c60f9c2543
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
curl "api.goskive.com/v2/questions/30/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8ce71bb2a8776ecb191fc20d47d788e37cbf52c5a356d25043ec5c60f9c2543"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/24/bookmark
Content-Type: application/json
Authorization: Bearer c315bd0d1a3a18bcd4232544da12ae79630071dbaf8390135ca9a4aa20aa681a
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
	-H "Authorization: Bearer c315bd0d1a3a18bcd4232544da12ae79630071dbaf8390135ca9a4aa20aa681a"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/23
Content-Type: application/json
Authorization: Bearer 3aecd76cce1a2946fec94bd66388a0e5cef1f7a18ca5d8503efbf68afb96086b
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/23" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aecd76cce1a2946fec94bd66388a0e5cef1f7a18ca5d8503efbf68afb96086b"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/27/downvote
Content-Type: application/json
Authorization: Bearer 24adf0d9a462854d613d5ba59d1fa3d1a7db140924a7394f66300661b20a24e6
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24adf0d9a462854d613d5ba59d1fa3d1a7db140924a7394f66300661b20a24e6"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/21
Content-Type: application/json
Authorization: Bearer 50a95da01cff0246cc338bb0385013f6956c713bd410d3fe28e4e58e0d151a74
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
    "id": 21,
    "obfuscated_id": "XIvx1qd7-fY",
    "author_id": 335,
    "chapter_id": 86,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:19.873Z",
    "created_at": "2016-11-08T14:21:19.737Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 41,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 42,
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
curl "api.goskive.com/v2/questions/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50a95da01cff0246cc338bb0385013f6956c713bd410d3fe28e4e58e0d151a74"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/22/report
Content-Type: application/json
Authorization: Bearer a9f6ee905a0182ce2b0b25c7ccf66a1f3638788594c820cf22c6017826615a27
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9f6ee905a0182ce2b0b25c7ccf66a1f3638788594c820cf22c6017826615a27"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/26/bookmark
Content-Type: application/json
Authorization: Bearer 8de45105df134d4df59291fc35c3698cb10659989fa7033bd590941ae87fadab
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/26/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8de45105df134d4df59291fc35c3698cb10659989fa7033bd590941ae87fadab"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/28
Content-Type: application/json
Authorization: Bearer 52d7d652a60a56c4ce7bb91cb311d54b11f96a398c0c331feb31e89d668aed11
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":28,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T14:21:22.799Z","updated_at":"2016-11-08T14:21:22.936Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":93,"author_id":356,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 28,
    "obfuscated_id": "hO6PHFgN8Aw",
    "author_id": 356,
    "chapter_id": 93,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T14:21:23.048Z",
    "created_at": "2016-11-08T14:21:22.799Z",
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
    "question": "{\"id\"=>28, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-08T14:21:22.799Z\", \"updated_at\"=>\"2016-11-08T14:21:22.936Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>93, \"author_id\"=>356, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 55,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 56,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 57,
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
curl "api.goskive.com/v2/questions/28" -d '{"question":{"question":{"id":28,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T14:21:22.799Z","updated_at":"2016-11-08T14:21:22.936Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":93,"author_id":356,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52d7d652a60a56c4ce7bb91cb311d54b11f96a398c0c331feb31e89d668aed11"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/25/upvote
Content-Type: application/json
Authorization: Bearer 10b0afc5f253f75e5326ac9a5c43015433428b47e13f80cbee4abe1523fb0470
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/25/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10b0afc5f253f75e5326ac9a5c43015433428b47e13f80cbee4abe1523fb0470"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 90f1fe0d058b554da63bb95cc4290feeb7f847feba069fb89606e0753657ca3b
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
      "creator_id": 449,
      "id": 128,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "discipline_id": 134,
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
      "updated_at": "2016-11-08T14:21:33.595Z",
      "shortname": "mit-pizza-201",
      "topic_id": 133,
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
	-H "Authorization: Bearer 90f1fe0d058b554da63bb95cc4290feeb7f847feba069fb89606e0753657ca3b"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 4c9448c347537a25cad8fa61f70a1927ea55a6095d8b0351f3e9c0ee7a10bea9
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
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-133",
      "html_url": "https://goskive.com/university/uni-133",
      "slug": "uni-133",
      "name": "National School of Pizza",
      "short_name": "Uni 133",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/549584df18bcc6166f3099c479cb15d1320c128e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/3cf492ea3fae834aba879881ee82734c5b7fbf38.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T14:21:33.888Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 134,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-132",
      "html_url": "https://goskive.com/university/uni-132",
      "slug": "uni-132",
      "name": "National School of Pastry",
      "short_name": "Uni 132",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/caa75247c2e91a7aec1b8a0bdabdfccb176270c0.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d5ada9c44b26f2c598bb20c18390244ba176ada1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T14:21:33.872Z",
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
	-H "Authorization: Bearer 4c9448c347537a25cad8fa61f70a1927ea55a6095d8b0351f3e9c0ee7a10bea9"
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
      "id": 30,
      "name": "Upgradable next generation utilisation",
      "name_translations": {
        "en": "Upgradable next generation utilisation"
      },
      "discipline_id": 30
    },
    {
      "id": 31,
      "name": "Devolved non-volatile customer loyalty",
      "name_translations": {
        "en": "Devolved non-volatile customer loyalty"
      },
      "discipline_id": 31
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
GET /v2/topics/29
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
    "id": 29,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 29
  }
}
```



```shell
curl "api.goskive.com/v2/topics/29" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 21273a40b53e7edf05f7c40bddb1a442459640268d5ffff52390809f53625ff0
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
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-90",
      "html_url": "https://goskive.com/university/uni-90",
      "slug": "uni-90",
      "name": "University 56",
      "short_name": "Uni 90",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/43b5fbbd11770049c4e0f41985099c3831c7f96f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/57b3014ced834e5e114cfe048366ffac65aacc51.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T14:21:18.577Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 91,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-91",
      "html_url": "https://goskive.com/university/uni-91",
      "slug": "uni-91",
      "name": "University 57",
      "short_name": "Uni 91",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0acbb8c8fa3ee80c22c483f268ba1d99f253aa4e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b2cf275a516a5fe6923a38239128ad7a28df233b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T14:21:18.593Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 92,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-92",
      "html_url": "https://goskive.com/university/uni-92",
      "slug": "uni-92",
      "name": "University 58",
      "short_name": "Uni 92",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b3ea3d00a2d8319ab945fe9e5e810ffa19a4d3bd.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e1569ad6c3d0aedaf265cb53f0e148deb76c43ab.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T14:21:18.610Z",
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
	-H "Authorization: Bearer 21273a40b53e7edf05f7c40bddb1a442459640268d5ffff52390809f53625ff0"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer a8911ff4d94416570745ebcc811e267cd8eeb77a8d92cf2c5c9307829205fa5b
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
    "id": 93,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/b4bec54a7f7cd323d36919c55d64b5b5c335955f.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c663f9415e0a293c066cadc042878bf2842ce887.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-08T14:21:18.669Z",
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
	-H "Authorization: Bearer a8911ff4d94416570745ebcc811e267cd8eeb77a8d92cf2c5c9307829205fa5b"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bc81aef8b123775c7987aeb3d88d76bbde43111f0dba9b6ff2df8a646e2b1fb9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":292,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 879,
    "id": 282,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 266,
    "additional_university_ids": [

    ],
    "discipline_id": 293,
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
    "chapters_updated_at": "2016-11-08T14:22:04.915Z",
    "updated_at": "2016-11-08T14:22:05.058Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 181,
        "updated_at": "2016-11-08T14:22:05.016Z",
        "course_id": 282,
        "author_id": 879,
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
        "id": 182,
        "updated_at": "2016-11-08T14:22:05.033Z",
        "course_id": 282,
        "author_id": 879,
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
        "id": 183,
        "updated_at": "2016-11-08T14:22:05.049Z",
        "course_id": 282,
        "author_id": 879,
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
    "topic_id": 292,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":292,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc81aef8b123775c7987aeb3d88d76bbde43111f0dba9b6ff2df8a646e2b1fb9"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 84b38083612f4cf1b8b836e7fe8f86eb06aece38f7b4b652d7b4be8f1da704fa
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":291,"published":false}}
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
    "creator_id": 878,
    "id": 281,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 265,
    "additional_university_ids": [

    ],
    "discipline_id": 292,
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
    "updated_at": "2016-11-08T14:22:04.836Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 291,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":291,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84b38083612f4cf1b8b836e7fe8f86eb06aece38f7b4b652d7b4be8f1da704fa"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 19cf64c8079c8c76201293de08b16761270c2e9f1b3d585248421a6c3abcb831
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
      "creator_id": 852,
      "id": 259,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-206",
      "html_url": "https://goskive.com/course/fu-course-206",
      "slug": "fu-course-206",
      "university_id": 256,
      "additional_university_ids": [

      ],
      "discipline_id": 270,
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
      "updated_at": "2016-11-08T14:22:02.495Z",
      "shortname": "fu-course-206",
      "topic_id": 269,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 206",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 852,
      "id": 260,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-207",
      "html_url": "https://goskive.com/course/fu-course-207",
      "slug": "fu-course-207",
      "university_id": 256,
      "additional_university_ids": [

      ],
      "discipline_id": 271,
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
      "chapters_updated_at": "2016-11-08T14:22:02.350Z",
      "updated_at": "2016-11-08T14:22:02.783Z",
      "shortname": "fu-course-207",
      "topic_id": 270,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 207",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19cf64c8079c8c76201293de08b16761270c2e9f1b3d585248421a6c3abcb831"
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
      "creator_id": 862,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "discipline_id": 278,
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
      "updated_at": "2016-11-08T14:22:03.314Z",
      "shortname": "fu-course-214",
      "topic_id": 277,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 862,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "discipline_id": 279,
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
      "chapters_updated_at": "2016-11-08T14:22:03.169Z",
      "updated_at": "2016-11-08T14:22:03.603Z",
      "shortname": "fu-course-215",
      "topic_id": 278,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
Authorization: Bearer 93ed6a76ae077eb5bf0ca11f78a31f985f19cda64601dbf8e50ac243c4c4ae9b
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
      "creator_id": 859,
      "id": 263,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-210",
      "html_url": "https://goskive.com/course/fu-course-210",
      "slug": "fu-course-210",
      "university_id": 258,
      "additional_university_ids": [

      ],
      "discipline_id": 274,
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
      "updated_at": "2016-11-08T14:22:03.055Z",
      "shortname": "fu-course-210",
      "topic_id": 273,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 210",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 859,
      "id": 264,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-211",
      "html_url": "https://goskive.com/course/fu-course-211",
      "slug": "fu-course-211",
      "university_id": 258,
      "additional_university_ids": [

      ],
      "discipline_id": 275,
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
      "updated_at": "2016-11-08T14:22:03.096Z",
      "shortname": "fu-course-211",
      "topic_id": 274,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 211",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93ed6a76ae077eb5bf0ca11f78a31f985f19cda64601dbf8e50ac243c4c4ae9b"
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
      "creator_id": 867,
      "id": 271,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-218",
      "html_url": "https://goskive.com/course/fu-course-218",
      "slug": "fu-course-218",
      "university_id": 261,
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
      "updated_at": "2016-11-08T14:22:03.814Z",
      "shortname": "fu-course-218",
      "topic_id": 281,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 218",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 867,
      "id": 272,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-219",
      "html_url": "https://goskive.com/course/fu-course-219",
      "slug": "fu-course-219",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "discipline_id": 283,
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
      "updated_at": "2016-11-08T14:22:03.853Z",
      "shortname": "fu-course-219",
      "topic_id": 282,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 219",
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
Authorization: Bearer b08a52ab5e76e1926e8b46eb2f31e3878b41bb98b6ecb4e1cb88a753f940bdbb
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
  "id": 882,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-08T14:22:05.499Z",
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
	-H "Authorization: Bearer b08a52ab5e76e1926e8b46eb2f31e3878b41bb98b6ecb4e1cb88a753f940bdbb"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/987
Content-Type: application/json
Authorization: Bearer 7a201aafe77cfdc85d7f984e7d786ec1b6b8427b89347fbb8cd7c0e134ee4229
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
    "id": 987,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 301,
    "fields_of_study": [
      327,
      328
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-08T14:22:18.047Z",
    "updated_at": "2016-11-08T14:22:18.047Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/987" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a201aafe77cfdc85d7f984e7d786ec1b6b8427b89347fbb8cd7c0e134ee4229"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/985
Content-Type: application/json
Authorization: Bearer 34b010e16ab8ec058b4b5673a96a2c130911a200988ebfb95fd57531b3cb2b2e
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
    "id": 985,
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
    "created_at": "2016-11-08T14:22:17.885Z",
    "updated_at": "2016-11-08T14:22:17.885Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/985" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34b010e16ab8ec058b4b5673a96a2c130911a200988ebfb95fd57531b3cb2b2e"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/3
Content-Type: application/json
Authorization: Bearer 4d0a21d14148347d31c35278bf52656fdb9bb7d4e3e582af7f6403a09192844c
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d0a21d14148347d31c35278bf52656fdb9bb7d4e3e582af7f6403a09192844c"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/1
Content-Type: application/json
Authorization: Bearer 42041f7988eb8eadf2d207bea7516e241573046eba8306181a4118f7c023ff32
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
    "id": 1,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 15,
    "user_id": 210
  }
}
```



```shell
curl "api.goskive.com/v2/votes/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42041f7988eb8eadf2d207bea7516e241573046eba8306181a4118f7c023ff32"
```
