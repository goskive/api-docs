---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Authentication

## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic Y2YzOWEzNTZkYTAyMzE0NTNmMjA1YWRmY2JhMWM5OTAyNGVjNDI0YjNlZGQ5
ZjlhYWE0Zjk0NDQ2ZmY2OWMwNDpjNjU4ZDQwYThlOTY3MDE1OTYxZTRmMDNi
MTQwZTFkMzU1Y2RlYWY3MDMwM2UzYjA3MDU2OWIwOWJkOGMxY2Nl

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
	-u cf39a356da0231453f205adfcba1c99024ec424b3edd9f9aaa4f94446ff69c04:c658d40a8e967015961e4f03b140e1d355cdeaf70303e3b070569b09bd8c1cce
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0929ccc681df40fbd3411410cf977e0af3ee2fa369e996a7f28a8b311aacb00b","client_secret":"827f00f3c4736fe713f96bf4fbd964cf169c84db300e670c937086229d826712"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0929ccc681df40fbd3411410cf977e0af3ee2fa369e996a7f28a8b311aacb00b","client_secret":"827f00f3c4736fe713f96bf4fbd964cf169c84db300e670c937086229d826712"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ODQzZDVlYjRkNGVlZTQxZWI5ZjE4MzQ4ZmNjMDFiYTljODU1OWE1ODMzMWUy
NjU1OGRmNGVlNTIyYjJmYmVkMzoyNDVkYzY1NTRkZjk5ZDk0M2YxMWRjMjM2
N2E2YzMzNTE4NDU3NDQ5MTY4Y2JmMTA2NGZkMWI4MGExZjE4ZmM4

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
  "access_token": "f81c748ee3fa4065ecc72196594eef25eeef2eb01bf9c4c8e17f2732811f78c6",
  "token_type": "bearer",
  "created_at": 1481803056
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 843d5eb4d4eee41eb9f18348fcc01ba9c8559a58331e26558df4ee522b2fbed3:245dc6554df99d943f11dc2367a6c33518457449168cbf1064fd1b80a1f18fc8
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e407a9e78b4ba3bdd0b5c8f216e86ca2f8572b26626aa1569c8f6525cbf31412","client_secret":"8b0d418561e40406a68b1ee7f6db7822eafec99637cebc5691303bd3eb005f55"}
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
  "access_token": "8540f1f48fa88f6c3ba83162bfe00d7754482af7691422c8631b77d24dc8a13d",
  "token_type": "bearer",
  "created_at": 1481803056
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e407a9e78b4ba3bdd0b5c8f216e86ca2f8572b26626aa1569c8f6525cbf31412","client_secret":"8b0d418561e40406a68b1ee7f6db7822eafec99637cebc5691303bd3eb005f55"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"72874023fd7812b05455ed6a7d4340fb0bb148a4eac7748431d3892819b5f653","client_secret":"55cafc533edcdfc3755903bfd737d4e722b5db7c1517a6818443e3484d1d4cb2"}
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
  "access_token": "64d32d48ec1259f971bfb5ba26a7af5c257c9235c953f15252fc9bda2fa2cf8e",
  "token_type": "bearer",
  "created_at": 1481803056
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"72874023fd7812b05455ed6a7d4340fb0bb148a4eac7748431d3892819b5f653","client_secret":"55cafc533edcdfc3755903bfd737d4e722b5db7c1517a6818443e3484d1d4cb2"}' -X POST \
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
Authorization: Bearer 0a9f57b6749e501d71925f973838ba1c63b528591ba047b5549ed2acb7da379a
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
    "company_id": 4,
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
	-H "Authorization: Bearer 0a9f57b6749e501d71925f973838ba1c63b528591ba047b5549ed2acb7da379a"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/47/flashcards
Content-Type: application/json
Authorization: Bearer da898e7c86babe1364d246311e1f8c8766b343a07bfe2173e494e7d0f3091b90
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":47,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 219,
    "chapter_id": 47,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:56:42.681Z",
    "created_at": "2016-12-15T11:56:42.681Z",
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
curl "api.goskive.com/v2/chapters/47/flashcards" -d '{"flashcard":{"chapter_id":47,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da898e7c86babe1364d246311e1f8c8766b343a07bfe2173e494e7d0f3091b90"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/49/flashcards
Content-Type: application/json
Authorization: Bearer e41de635448badc9aa610d9a2747b6207a094991d699fea08735815309d5f1b8
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 223,
      "chapter_id": 49,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:43.199Z",
      "created_at": "2016-12-15T11:56:43.199Z",
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
      "author_id": 223,
      "chapter_id": 49,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:43.242Z",
      "created_at": "2016-12-15T11:56:43.242Z",
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 223,
      "chapter_id": 49,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:43.285Z",
      "created_at": "2016-12-15T11:56:43.285Z",
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
	-H "Authorization: Bearer e41de635448badc9aa610d9a2747b6207a094991d699fea08735815309d5f1b8"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/193/questions
Content-Type: application/json
Authorization: Bearer b713d666f58e850b98e08a6a996afcf32beb7a17302191591496139acd26cf62
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":193,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 128,
    "obfuscated_id": "Q4ODZIcqv0E",
    "author_id": 833,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:39.492Z",
    "created_at": "2016-12-15T11:57:39.492Z",
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
        "id": 257,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 258,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 259,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 260,
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
curl "api.goskive.com/v2/chapters/193/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":193,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b713d666f58e850b98e08a6a996afcf32beb7a17302191591496139acd26cf62"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/190/questions
Content-Type: application/json
Authorization: Bearer 891a5c0fd2ee16cea815364602ece40252c7715567305904141329bf13f09850
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":190,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 125,
    "obfuscated_id": "K6zw0Yc6Me8",
    "author_id": 824,
    "chapter_id": 190,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:37.884Z",
    "created_at": "2016-12-15T11:57:37.884Z",
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
        "id": 250,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 251,
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
curl "api.goskive.com/v2/chapters/190/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":190,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 891a5c0fd2ee16cea815364602ece40252c7715567305904141329bf13f09850"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/192/questions
Content-Type: application/json
Authorization: Bearer ccb44775568e5325a824679f5621c524895a5ee824e3c41300568dbb2db6966a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":192,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 127,
    "obfuscated_id": "E3yfRgAzssw",
    "author_id": 830,
    "chapter_id": 192,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:38.921Z",
    "created_at": "2016-12-15T11:57:38.921Z",
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
        "id": 255,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 256,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/192/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":192,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccb44775568e5325a824679f5621c524895a5ee824e3c41300568dbb2db6966a"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/191/questions
Content-Type: application/json
Authorization: Bearer 823c9428157570baee5ef049365910b4e2bba8303cfc35574bd2001a68a1ebd6
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":191,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 126,
    "obfuscated_id": "fKTMLttUR-w",
    "author_id": 827,
    "chapter_id": 191,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:38.434Z",
    "created_at": "2016-12-15T11:57:38.434Z",
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
        "id": 252,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 253,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 254,
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
curl "api.goskive.com/v2/chapters/191/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":191,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 823c9428157570baee5ef049365910b4e2bba8303cfc35574bd2001a68a1ebd6"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/189/questions
Content-Type: application/json
Authorization: Bearer 6157ed96ba78abc290a9dfa5657ed15fa3d53cbf5baabbf857b2a310ecba0a77
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
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 818,
      "chapter_id": 189,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:37.274Z",
      "created_at": "2016-12-15T11:57:37.189Z",
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
          "id": 244,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 245,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 819,
      "chapter_id": 189,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:37.427Z",
      "created_at": "2016-12-15T11:57:37.342Z",
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
          "id": 246,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 247,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 820,
      "chapter_id": 189,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:37.579Z",
      "created_at": "2016-12-15T11:57:37.493Z",
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
          "id": 248,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 249,
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
curl "api.goskive.com/v2/chapters/189/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6157ed96ba78abc290a9dfa5657ed15fa3d53cbf5baabbf857b2a310ecba0a77"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/164
Content-Type: application/json
Authorization: Bearer e7e164b6850827b26898ce189d517156dc8bd071dac5ed978a85f8a2d369f296
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
curl "api.goskive.com/v2/chapters/164" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7e164b6850827b26898ce189d517156dc8bd071dac5ed978a85f8a2d369f296"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/167
Content-Type: application/json
Authorization: Bearer ff67acfa5c3f6e6e6b46e37f3743a1898b874ee06381bfc7d6ba480b818382bb
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
curl "api.goskive.com/v2/chapters/167" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff67acfa5c3f6e6e6b46e37f3743a1898b874ee06381bfc7d6ba480b818382bb"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/159
Content-Type: application/json
Authorization: Bearer 8bc1235b81790e6244fdb2d0f5e46a2c6db3a53ebdeebdefca3cf1279206f960
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
curl "api.goskive.com/v2/chapters/159" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8bc1235b81790e6244fdb2d0f5e46a2c6db3a53ebdeebdefca3cf1279206f960"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/165
Content-Type: application/json
Authorization: Bearer 22fd0afc9e77480b13c56122cd401610e41dac48018be55f08c69bbac345f385
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/165" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22fd0afc9e77480b13c56122cd401610e41dac48018be55f08c69bbac345f385"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/163
Content-Type: application/json
Authorization: Bearer ec17f3e613dcbf818d026ea19dbe27035a4890254f5be5e7a192fcb437908c84
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
    "id": 163,
    "updated_at": "2016-12-15T11:57:23.892Z",
    "course_id": 216,
    "author_id": 699,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T11:57:23.386Z",
    "questions_updated_at": "2016-12-15T11:57:23.386Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 703,
        "chapter_id": 163,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.874Z",
        "created_at": "2016-12-15T11:57:23.874Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 701,
        "chapter_id": 163,
        "position": 76,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.765Z",
        "created_at": "2016-12-15T11:57:23.680Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/163" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec17f3e613dcbf818d026ea19dbe27035a4890254f5be5e7a192fcb437908c84"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/160
Content-Type: application/json
Authorization: Bearer 8378e6237400b9e80414f2e788711fa4f68261057bd9c914142e15debc47c4a9
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
    "id": 160,
    "updated_at": "2016-12-15T11:57:22.449Z",
    "course_id": 213,
    "author_id": 687,
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
curl "api.goskive.com/v2/chapters/160" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8378e6237400b9e80414f2e788711fa4f68261057bd9c914142e15debc47c4a9"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/5/replies
Content-Type: application/json
Authorization: Bearer af82600779ec5ff3687ab0382b721bcdbad7509612e59fa165781379cd69c493
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
    "id": 6,
    "author_id": 150,
    "reply_to_id": 5,
    "created_at": "2016-12-15T11:56:34.454Z",
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
curl "api.goskive.com/v2/comments/5/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af82600779ec5ff3687ab0382b721bcdbad7509612e59fa165781379cd69c493"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/7/replies
Content-Type: application/json
Authorization: Bearer 1daf42d472ae9d8116128a48c2c3adbe7bc535a4706a0fd6378866e0842daa13
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
curl "api.goskive.com/v2/comments/7/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1daf42d472ae9d8116128a48c2c3adbe7bc535a4706a0fd6378866e0842daa13"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/59
Content-Type: application/json
Authorization: Bearer 72bcb3fc2588285ee2e048f00d56b2fd77b5628013184e8d8ecbabe04f5beb26
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
curl "api.goskive.com/v2/comments/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72bcb3fc2588285ee2e048f00d56b2fd77b5628013184e8d8ecbabe04f5beb26"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/20/republish
Content-Type: application/json
Authorization: Bearer 2088b2cf86db548175af96521be79277f90b944c032b30c0c693fc1345ae2702
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
	-H "Authorization: Bearer 2088b2cf86db548175af96521be79277f90b944c032b30c0c693fc1345ae2702"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/58
Content-Type: application/json
Authorization: Bearer b3c08d8efd42a7bca7dd3743176766386c59306574f5323a9e17486694534cdc
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3c08d8efd42a7bca7dd3743176766386c59306574f5323a9e17486694534cdc"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 5ffb8922f983c9730bdd9a15e15db93a1c171c9fc4f24f0aed8153fdd55096e6
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ffb8922f983c9730bdd9a15e15db93a1c171c9fc4f24f0aed8153fdd55096e6"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/19
Content-Type: application/json
Authorization: Bearer 35089418ceaf148ff1fe18f0e46da12f1d5cfc53f217afa9df8050e79edea945
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
    "id": 19,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T11:56:45.386Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35089418ceaf148ff1fe18f0e46da12f1d5cfc53f217afa9df8050e79edea945"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer bb76727846192c4ea4278f1cc6289676f62cc440118bbce4d4c5f8d7056a68e3
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
      "id": 16,
      "name": "Fake Company Name 12",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T11:56:45.320Z"
    },
    {
      "id": 17,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T11:56:45.324Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T11:56:45.328Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb76727846192c4ea4278f1cc6289676f62cc440118bbce4d4c5f8d7056a68e3"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/3/company_profiles
Content-Type: application/json
Authorization: Bearer 843dfabc8de9466a3fbc7c9f43eb55a199bf13689b38738a28797774e1559365
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
	-H "Authorization: Bearer 843dfabc8de9466a3fbc7c9f43eb55a199bf13689b38738a28797774e1559365"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/1/company_profiles
Content-Type: application/json
Authorization: Bearer c640db4d474308a79ebc847d7fde58e7f075865e9c039eedb48c747fce28eaa5
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
	-H "Authorization: Bearer c640db4d474308a79ebc847d7fde58e7f075865e9c039eedb48c747fce28eaa5"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 38aae6b93da37d896877c740f3902240170e864625849b49ad99f650c9087339
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
      "company_id": 20,
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
      "company_id": 23,
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
	-H "Authorization: Bearer 38aae6b93da37d896877c740f3902240170e864625849b49ad99f650c9087339"
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
Authorization: Bearer add5724915980b0e3f6cedabfed073c310c0a56b1cee78d8982a57ee43280fa5
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
	-H "Authorization: Bearer add5724915980b0e3f6cedabfed073c310c0a56b1cee78d8982a57ee43280fa5"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4f8518d8bcb1e407fc824234372befa49e2c7e9156852209b695f49893bca4c3
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
    "id": 105,
    "updated_at": "2016-12-15T11:56:59.901Z",
    "course_id": 138,
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

    ],
    "title": "Preparing the oven",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f8518d8bcb1e407fc824234372befa49e2c7e9156852209b695f49893bca4c3"
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
      "id": 93,
      "updated_at": "2016-12-15T11:56:58.208Z",
      "course_id": 132,
      "author_id": 416,
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
      "id": 94,
      "updated_at": "2016-12-15T11:56:58.233Z",
      "course_id": 132,
      "author_id": 417,
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
      "id": 95,
      "updated_at": "2016-12-15T11:56:58.446Z",
      "course_id": 132,
      "author_id": 418,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T11:56:58.086Z",
      "questions_updated_at": "2016-12-15T11:56:58.086Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 89",
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
Authorization: Bearer a88115ee1e477e768ac59315922e18fe8311d2f8fdd29e2c91b4c08589a5de2a
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
      "updated_at": "2016-12-15T11:56:59.005Z",
      "course_id": 135,
      "author_id": 427,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 93",
      "position": 1
    },
    {
      "id": 100,
      "updated_at": "2016-12-15T11:56:59.029Z",
      "course_id": 135,
      "author_id": 428,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 94",
      "position": 2
    },
    {
      "id": 101,
      "updated_at": "2016-12-15T11:56:59.239Z",
      "course_id": 135,
      "author_id": 429,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T11:56:58.859Z",
      "questions_updated_at": "2016-12-15T11:56:58.859Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 95",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a88115ee1e477e768ac59315922e18fe8311d2f8fdd29e2c91b4c08589a5de2a"
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
      "id": 96,
      "updated_at": "2016-12-15T11:56:58.757Z",
      "course_id": 134,
      "author_id": 423,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 90",
      "position": 1
    },
    {
      "id": 97,
      "updated_at": "2016-12-15T11:56:58.782Z",
      "course_id": 134,
      "author_id": 424,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 91",
      "position": 2
    },
    {
      "id": 98,
      "updated_at": "2016-12-15T11:56:58.807Z",
      "course_id": 134,
      "author_id": 425,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 92",
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
Authorization: Bearer 20abf00bdda2d3343725d66261ef37ad14e90510a9ddedf9fbfe4985b3bf1e3b
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
      "updated_at": "2016-12-15T11:56:59.452Z",
      "course_id": 136,
      "author_id": 434,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 96",
      "position": 1
    },
    {
      "id": 103,
      "updated_at": "2016-12-15T11:56:59.478Z",
      "course_id": 136,
      "author_id": 435,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 97",
      "position": 2
    },
    {
      "id": 104,
      "updated_at": "2016-12-15T11:56:59.505Z",
      "course_id": 136,
      "author_id": 436,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 98",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20abf00bdda2d3343725d66261ef37ad14e90510a9ddedf9fbfe4985b3bf1e3b"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 91d26249de79b1e163afd1dfcefe5beeb653e77d94958fd509a56c6934780e5a
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
    "course_id": 311,
    "user_id": 974,
    "updated_at": "2016-12-15T11:57:50.594Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91d26249de79b1e163afd1dfcefe5beeb653e77d94958fd509a56c6934780e5a"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f937dea9af07a4185dd4d0e7a2be864b87fd6c8955569bf657782e46cc055968
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
      "id": 6,
      "course_id": 315,
      "user_id": 984,
      "updated_at": "2016-12-15T11:57:51.423Z"
    },
    {
      "id": 7,
      "course_id": 315,
      "user_id": 985,
      "updated_at": "2016-12-15T11:57:51.439Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f937dea9af07a4185dd4d0e7a2be864b87fd6c8955569bf657782e46cc055968"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/194/files
Content-Type: application/json
Authorization: Bearer f633c097e74f93e155c91ecb4012e3b32cce38a3e0b4ac12c614579f4de36372
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
        "created_at": "2016-12-15T11:57:17.738Z",
        "updated_at": "2016-12-15T11:57:17.738Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T11:57:17.748Z",
      "updated_at": "2016-12-15T11:57:17.748Z",
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
        "created_at": "2016-12-15T11:57:17.758Z",
        "updated_at": "2016-12-15T11:57:17.758Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T11:57:17.767Z",
      "updated_at": "2016-12-15T11:57:17.767Z",
      "course_id": 194,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 8,
      "uploader": {
        "id": 624,
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
        "created_at": "2016-12-15T11:57:17.777Z",
        "updated_at": "2016-12-15T11:57:17.777Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T11:57:17.787Z",
      "updated_at": "2016-12-15T11:57:17.787Z",
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
	-H "Authorization: Bearer f633c097e74f93e155c91ecb4012e3b32cce38a3e0b4ac12c614579f4de36372"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/197/files
Content-Type: application/json
Authorization: Bearer a7c8fa0ecc92e838ba4434a79e4836d4f57201ff6e7e246ab6068bcc81b7c829
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
    "id": 9,
    "uploader": {
      "id": 631,
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
      "created_at": "2016-12-15T11:57:18.261Z",
      "updated_at": "2016-12-15T11:57:18.261Z"
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
    "created_at": "2016-12-15T11:57:18.292Z",
    "updated_at": "2016-12-15T11:57:18.292Z",
    "course_id": 197,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/197/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7c8fa0ecc92e838ba4434a79e4836d4f57201ff6e7e246ab6068bcc81b7c829"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/196/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer af4fff3b1c80d338fe144078944cbfb501bb86ff53b238516e25d1c2fba9bef3
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
    "key": "cache/5a767dd163c0f13d637ae30da5a3b2b7.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxMjo1NzoxOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzVhNzY3ZGQxNjNjMGYxM2Q2MzdhZTMwZGE1YTNiMmI3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDExNTcxOFoifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T115718Z",
    "x-amz-signature": "415d1914770d7705854d2a0a10d7a9987b61d0c86c26a13e9240dd371905f820"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/196/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af4fff3b1c80d338fe144078944cbfb501bb86ff53b238516e25d1c2fba9bef3"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 9538f1adef47923b9c2c86230944898885a2ba982694a31b4cf4a30b124d7b74
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
	-H "Authorization: Bearer 9538f1adef47923b9c2c86230944898885a2ba982694a31b4cf4a30b124d7b74"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0dace1ead050922d4970f09fef1cce8d9c428ebdfe017ac153d3114edf4753b6
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
	-H "Authorization: Bearer 0dace1ead050922d4970f09fef1cce8d9c428ebdfe017ac153d3114edf4753b6"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3ab1d76f2194b37db05767f982d64a34c32eb012e843072d8cc4a238c19fcd8d
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
	-H "Authorization: Bearer 3ab1d76f2194b37db05767f982d64a34c32eb012e843072d8cc4a238c19fcd8d"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f976060a20d6237a6b165678806d1ce77f7ba06d066d5e626254919ed3f11ec2
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
	-H "Authorization: Bearer f976060a20d6237a6b165678806d1ce77f7ba06d066d5e626254919ed3f11ec2"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer eabd5f478ddded6b049fef11132e1e0588ab6f7570b6300de9f57daa4b83aeb6
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
	-H "Authorization: Bearer eabd5f478ddded6b049fef11132e1e0588ab6f7570b6300de9f57daa4b83aeb6"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 928b714dfecb2183435a74b1a5ef7ff7a57934b20902dd1753e2e51a098e37be
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
    "creator_id": 717,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 206,
    "additional_university_ids": [

    ],
    "discipline_id": 231,
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
    "chapters_updated_at": "2016-12-15T11:57:25.000Z",
    "updated_at": "2016-12-15T11:57:26.258Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 718,
        "chapter_id": 168,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:26.037Z",
        "created_at": "2016-12-15T11:57:26.037Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 718,
        "chapter_id": 169,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:26.113Z",
        "created_at": "2016-12-15T11:57:26.113Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 718,
        "chapter_id": 168,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:26.079Z",
        "created_at": "2016-12-15T11:57:26.079Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 718,
        "chapter_id": 169,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:26.155Z",
        "created_at": "2016-12-15T11:57:26.155Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 718,
        "chapter_id": 168,
        "position": 79,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:25.232Z",
        "created_at": "2016-12-15T11:57:25.151Z",
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
        "author_id": 718,
        "chapter_id": 168,
        "position": 80,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:25.366Z",
        "created_at": "2016-12-15T11:57:25.290Z",
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
        "author_id": 718,
        "chapter_id": 169,
        "position": 81,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:25.538Z",
        "created_at": "2016-12-15T11:57:25.447Z",
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
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 718,
        "chapter_id": 169,
        "position": 82,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:25.679Z",
        "created_at": "2016-12-15T11:57:25.600Z",
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
      }
    ],
    "chapters": [
      {
        "id": 168,
        "updated_at": "2016-12-15T11:57:26.206Z",
        "course_id": 221,
        "author_id": 717,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T11:57:25.000Z",
        "questions_updated_at": "2016-12-15T11:57:25.000Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 150",
        "position": 1
      },
      {
        "id": 169,
        "updated_at": "2016-12-15T11:57:26.248Z",
        "course_id": 221,
        "author_id": 717,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T11:57:25.000Z",
        "questions_updated_at": "2016-12-15T11:57:25.000Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 151",
        "position": 2
      }
    ],
    "topic_id": 231,
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
	-H "Authorization: Bearer 928b714dfecb2183435a74b1a5ef7ff7a57934b20902dd1753e2e51a098e37be"
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
    "creator_id": 729,
    "id": 223,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 208,
    "additional_university_ids": [

    ],
    "discipline_id": 233,
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
    "chapters_updated_at": "2016-12-15T11:57:27.791Z",
    "updated_at": "2016-12-15T11:57:29.007Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 100,
        "obfuscated_id": "erXmBhoMZFI",
        "author_id": 729,
        "chapter_id": 172,
        "position": 91,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:28.011Z",
        "created_at": "2016-12-15T11:57:27.930Z",
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
      },
      {
        "id": 102,
        "obfuscated_id": "jFy90P7ldB4",
        "author_id": 729,
        "chapter_id": 173,
        "position": 93,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:28.298Z",
        "created_at": "2016-12-15T11:57:28.214Z",
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
            "id": 204,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 205,
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
        "id": 172,
        "updated_at": "2016-12-15T11:57:28.957Z",
        "course_id": 223,
        "author_id": 729,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T11:57:27.791Z",
        "questions_updated_at": "2016-12-15T11:57:27.791Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 154",
        "position": 1
      },
      {
        "id": 173,
        "updated_at": "2016-12-15T11:57:28.997Z",
        "course_id": 223,
        "author_id": 729,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T11:57:27.791Z",
        "questions_updated_at": "2016-12-15T11:57:27.791Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 155",
        "position": 2
      }
    ],
    "topic_id": 233,
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
PUT /v2/courses/239/pin
Content-Type: application/json
Authorization: Bearer 153bf75934fda9a55bc06e94e106cc86c74507bc0b63f04cf3752516b614f6c3
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/239/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 153bf75934fda9a55bc06e94e106cc86c74507bc0b63f04cf3752516b614f6c3"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/238/pin
Content-Type: application/json
Authorization: Bearer 35ba184e06355916f027bb9c1781e2f20ed7cad278e30785289b8a28484daca8
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/238/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35ba184e06355916f027bb9c1781e2f20ed7cad278e30785289b8a28484daca8"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0e52a2b2e359f5c9999dc877234a6e0dd2b3bea73e6f512a62009df28cebceb0
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
    "creator_id": 762,
    "id": 235,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 220,
    "additional_university_ids": [

    ],
    "discipline_id": 245,
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
    "updated_at": "2016-12-15T11:57:32.861Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 245,
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
	-H "Authorization: Bearer 0e52a2b2e359f5c9999dc877234a6e0dd2b3bea73e6f512a62009df28cebceb0"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 7552f9ec44c04908d3661573e490eadaff7f4a2329ff918bee6c164fd2ec2b04
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
    "id": 51,
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
    "created_at": "2016-12-15T11:56:25.420Z",
    "updated_at": "2016-12-15T11:56:25.420Z",
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
	-H "Authorization: Bearer 7552f9ec44c04908d3661573e490eadaff7f4a2329ff918bee6c164fd2ec2b04"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer e44dc6b6c5aceec70470eb7b8d6c4cc9af17e02656c66e3f43fe72e36d3e0dfe
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[42]}
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
    "id": 47,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      42
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T11:56:25.128Z",
    "updated_at": "2016-12-15T11:56:25.169Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[42]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e44dc6b6c5aceec70470eb7b8d6c4cc9af17e02656c66e3f43fe72e36d3e0dfe"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a6fef8862f5bca76aae1ec7ae9c34fd3e15a51231e6ba49c5b5186f96f1d4a2b
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
    "id": 49,
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
    "created_at": "2016-12-15T11:56:25.270Z",
    "updated_at": "2016-12-15T11:56:25.270Z",
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
	-H "Authorization: Bearer a6fef8862f5bca76aae1ec7ae9c34fd3e15a51231e6ba49c5b5186f96f1d4a2b"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b16d62ac597fd9411134a74db3ba094229bf78638e9843ef1769b5123b9cf3cc
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[43]}
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
    "id": 48,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      43
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T11:56:25.210Z",
    "updated_at": "2016-12-15T11:56:25.210Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[43]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b16d62ac597fd9411134a74db3ba094229bf78638e9843ef1769b5123b9cf3cc"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer db16c61af7d13d9ba5cc3fe1755af00e9b1fd030c279836bc23dfd2582d84f99
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

41
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
    "id": 46,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9ad36e6e905d60ab732686f35eab126183cb4524.jpg",
    "university_id": null,
    "fields_of_study": [
      41
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T11:56:24.781Z",
    "updated_at": "2016-12-15T11:56:25.074Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/aa484629e42cda6f9b956e5ab892c2a455f2c760.jpg",
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

41
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer db16c61af7d13d9ba5cc3fe1755af00e9b1fd030c279836bc23dfd2582d84f99"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer a20f8ac8aeb0be742e388505028697ef76c494771af03434c280d83a0032c01d
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
      "bookmarkable_id": 19,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 20,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 21,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a20f8ac8aeb0be742e388505028697ef76c494771af03434c280d83a0032c01d"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 6741a2c747f94fe56b52619de854c7cd004017e46f5f81928719079878bf775f
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
      "creator_id": 191,
      "id": 82,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-78",
      "html_url": "https://goskive.com/course/mit-course-78",
      "slug": "mit-course-78",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "discipline_id": 90,
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
      "updated_at": "2016-12-15T11:56:38.945Z",
      "shortname": "mit-course-78",
      "topic_id": 90,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 78",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 192,
      "id": 83,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-79",
      "html_url": "https://goskive.com/course/mit-course-79",
      "slug": "mit-course-79",
      "university_id": 61,
      "additional_university_ids": [

      ],
      "discipline_id": 91,
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
      "updated_at": "2016-12-15T11:56:39.071Z",
      "shortname": "mit-course-79",
      "topic_id": 91,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 79",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6741a2c747f94fe56b52619de854c7cd004017e46f5f81928719079878bf775f"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer c2bfd5932017bc7bca55ce4a5c7e3743b8f87e3a15f1e359e44427a1078e9785
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
        "created_at": "2016-12-15T11:56:36.850Z",
        "updated_at": "2016-12-15T11:56:36.850Z",
        "file_url": "memory://13ee7b96536b07a909be90e3d5aa6092.pdf",
        "course_id": 76,
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
        "created_at": "2016-12-15T11:56:36.976Z",
        "updated_at": "2016-12-15T11:56:36.976Z",
        "file_url": "memory://7d1a3404392422800ad94c076229e2bd.pdf",
        "course_id": 77,
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
        "created_at": "2016-12-15T11:56:37.210Z",
        "updated_at": "2016-12-15T11:56:37.210Z",
        "file_url": "memory://c6a749b4c960b3dba0eda5ab7a1b551b.pdf",
        "course_id": 78,
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
	-H "Authorization: Bearer c2bfd5932017bc7bca55ce4a5c7e3743b8f87e3a15f1e359e44427a1078e9785"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 857844f2041d2d6a454049b0cfe6123c771a34f2c5875b2628d2e9247c91e1a0
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
        "updated_at": "2016-12-15T11:57:19.647Z"
      },
      "created_at": "2016-12-15T11:57:19.651Z",
      "updated_at": "2016-12-15T11:57:19.651Z",
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
        "updated_at": "2016-12-15T11:57:19.659Z"
      },
      "created_at": "2016-12-15T11:57:19.662Z",
      "updated_at": "2016-12-15T11:57:19.662Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 857844f2041d2d6a454049b0cfe6123c771a34f2c5875b2628d2e9247c91e1a0"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer fdf6c73ddf04caeecb6badddeb6b9dc064a9f7c2136185210a5f553bace98598
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
      "id": 9,
      "created_at": "2016-12-15T11:57:04.935Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 9,
      "updated_at": "2016-12-15T11:57:05.087Z",
      "author_id": "494",
      "thread_subject_id": "155",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 10,
      "created_at": "2016-12-15T11:57:05.075Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 10,
      "updated_at": "2016-12-15T11:57:05.090Z",
      "author_id": "497",
      "thread_subject_id": "156",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 11,
      "created_at": "2016-12-15T11:57:05.464Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-12-15T11:57:05.464Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 12,
      "created_at": "2016-12-15T11:57:05.841Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-12-15T11:57:05.841Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 13,
      "created_at": "2016-12-15T11:57:06.220Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 20,
      "updated_at": "2016-12-15T11:57:06.220Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 14,
      "created_at": "2016-12-15T11:57:06.514Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 54,
      "updated_at": "2016-12-15T11:57:06.514Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 15,
      "created_at": "2016-12-15T11:57:06.816Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 55,
      "updated_at": "2016-12-15T11:57:06.816Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 16,
      "created_at": "2016-12-15T11:57:07.125Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 56,
      "updated_at": "2016-12-15T11:57:07.125Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdf6c73ddf04caeecb6badddeb6b9dc064a9f7c2136185210a5f553bace98598"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/17
Content-Type: application/json
Authorization: Bearer 99049f36066ebb0543ebff501dd67b8eb7deb1d967a514e957b5fd0b96b0467a
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T11:47:07.000Z"}}
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
    "created_at": "2016-12-15T11:57:07.309Z",
    "read_at": "2016-12-15T11:47:07.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 11,
    "updated_at": "2016-12-15T11:57:07.350Z",
    "author_id": "522",
    "thread_subject_id": "163",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/17" -d '{"notification":{"read_at":"2016-12-15T11:47:07.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99049f36066ebb0543ebff501dd67b8eb7deb1d967a514e957b5fd0b96b0467a"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer be56198a3903b88ac76882d949ef69c32557c42d2149e88af48dca5fb67a25f1
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
      "id": 4,
      "course_id": 199,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T11:57:18.715Z",
      "course_published": true,
      "updated_at": "2016-12-15T11:57:18.710Z"
    },
    {
      "id": 5,
      "course_id": 200,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T11:57:18.879Z",
      "course_published": true,
      "updated_at": "2016-12-15T11:57:18.874Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be56198a3903b88ac76882d949ef69c32557c42d2149e88af48dca5fb67a25f1"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 530175dc8bedec22b57fe9d03bfe98a207f24117434943f09a879183c68ef420
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
    "id": 3,
    "course_id": 198,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T11:57:18.489Z",
    "course_published": true,
    "updated_at": "2016-12-15T11:57:18.484Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 530175dc8bedec22b57fe9d03bfe98a207f24117434943f09a879183c68ef420"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 7948cc1a78a367b016aaa4741dd4963baca595344f1c9f5298f36137f710a8ab
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
    "course_id": 201,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T11:57:19.099Z",
    "course_published": true,
    "updated_at": "2016-12-15T11:57:19.091Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7948cc1a78a367b016aaa4741dd4963baca595344f1c9f5298f36137f710a8ab"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 5a27ee760590557bf43ae6595138f1c93eaabf5e815e5618fb34719782b5f0e2
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
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 12,
      "user_id": 157
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 13,
      "user_id": 157
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 14,
      "user_id": 157
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 15,
      "user_id": 157
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a27ee760590557bf43ae6595138f1c93eaabf5e815e5618fb34719782b5f0e2"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/266
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
    "id": 266,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 266,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 266
      },
      {
        "id": 267,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 266
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/266" -X GET \
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
      "id": 267,
      "name": "Universal radical attitude",
      "name_translations": {
        "en": "Universal radical attitude"
      }
    },
    {
      "id": 268,
      "name": "Sharable system-worthy data-warehouse",
      "name_translations": {
        "en": "Sharable system-worthy data-warehouse"
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
PATCH /v2/feedbacks/28/close
Content-Type: application/json
Authorization: Bearer ddcc00a6977cb95ded938c22e16b9c3304733f98856ddbe6b12abb23dbb583b1
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
    "id": 28,
    "user_id": 367,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T11:56:54.340Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/28/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddcc00a6977cb95ded938c22e16b9c3304733f98856ddbe6b12abb23dbb583b1"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/22/fix
Content-Type: application/json
Authorization: Bearer 16eb2eab370b51f917198cf878b2dc7ba41e5415334c58ac1bfbfb9526fa164d
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
    "id": 22,
    "user_id": 335,
    "feedbackable_id": 35,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T11:56:52.363Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/22/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16eb2eab370b51f917198cf878b2dc7ba41e5415334c58ac1bfbfb9526fa164d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/25
Content-Type: application/json
Authorization: Bearer 1caa620d02ef8e77bcf4c2e72d0f097f4ae8704f9881a978cf760697c83f19c2
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
    "id": 25,
    "user_id": 350,
    "feedbackable_id": 38,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T11:56:53.332Z",
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
curl "api.goskive.com/v2/feedbacks/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1caa620d02ef8e77bcf4c2e72d0f097f4ae8704f9881a978cf760697c83f19c2"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer e1b93494bc4ccc7a1a9ae800d930095464dd55b67c6a56ec9b08eea000126728
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
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1b93494bc4ccc7a1a9ae800d930095464dd55b67c6a56ec9b08eea000126728"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer 183d639644cd7ac7b5850287f67a06519ae12a000f7304cd7f149fc393311d87
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
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 183d639644cd7ac7b5850287f67a06519ae12a000f7304cd7f149fc393311d87"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/29/close
Content-Type: application/json
Authorization: Bearer 5f0272b946b922b66ab3b339c2304f106d7d9d0efb9cf30bbd46d7ef73eef43d
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
curl "api.goskive.com/v2/feedbacks/29/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f0272b946b922b66ab3b339c2304f106d7d9d0efb9cf30bbd46d7ef73eef43d"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/26
Content-Type: application/json
Authorization: Bearer 12219fec77e40430c7716d11d9bf2af27be69dca2d139ba906e420cf232c3d36
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
    "id": 26,
    "user_id": 355,
    "feedbackable_id": 39,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T11:56:53.710Z",
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
curl "api.goskive.com/v2/feedbacks/26" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12219fec77e40430c7716d11d9bf2af27be69dca2d139ba906e420cf232c3d36"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer cc73423dbaf9a28647dd87a9f7fbf20f9df7481c8abe2df94d69ee90bde1f505
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
	-H "Authorization: Bearer cc73423dbaf9a28647dd87a9f7fbf20f9df7481c8abe2df94d69ee90bde1f505"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer 32db0e295890a522e8bb5183ce5866c506a9f33a20c1174ffd5be145e6bd189f
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
	-H "Authorization: Bearer 32db0e295890a522e8bb5183ce5866c506a9f33a20c1174ffd5be145e6bd189f"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer f7f49078d866b023ed9c610049297ec88dec7e46f734efe4d88f51ff7c88daf2
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7f49078d866b023ed9c610049297ec88dec7e46f734efe4d88f51ff7c88daf2"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer e98ce14995cb90ae64ff14fadf3a43dd05f8986f29babaea4ee7d608c9cb67c2
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/003ed927390f912154493d224dd9d4f1.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T115747Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=eb2954aa39a85ad789c568ebd17dbcf4426581f08788ff41c4e7c73830678095",
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
	-H "Authorization: Bearer e98ce14995cb90ae64ff14fadf3a43dd05f8986f29babaea4ee7d608c9cb67c2"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/22/preview
Content-Type: application/json
Authorization: Bearer cf17768503a6a902fcb1a36250421e08e437532d46f19d65f307f377d9c7c5af
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/90931da71a78c0702e66b879531b8f5c.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T115750Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=d21015104e8a522a480369fc97dda77117aadddc0865ae7d153a73fc20546ba6",
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
	-H "Authorization: Bearer cf17768503a6a902fcb1a36250421e08e437532d46f19d65f307f377d9c7c5af"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 0792dffd004fd1b591bfe8f82ba4a96ad591dd95ab2e4cf557e9c9562f127e32
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
      "id": 945,
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
      "created_at": "2016-12-15T11:57:47.877Z",
      "updated_at": "2016-12-15T11:57:47.877Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T11:57:48.015Z",
    "updated_at": "2016-12-15T11:57:48.015Z",
    "course_id": 301,
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
	-H "Authorization: Bearer 0792dffd004fd1b591bfe8f82ba4a96ad591dd95ab2e4cf557e9c9562f127e32"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/5/matched_courses?required_cu_count=2
Authorization: Bearer f081cf4337d0c02c7fccf44fd1aac536ba806402a2ecd5793b3adc0879c65811
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
      "creator_id": 466,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 134,
      "additional_university_ids": [

      ],
      "discipline_id": 159,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 2,
      "questions_count": 1,
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
      "chapters_updated_at": "2016-12-15T11:57:01.566Z",
      "updated_at": "2016-12-15T11:57:02.765Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 159,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 471,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-e23067c3-1133-4e65-b58f-7d814e35ecaf",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-e23067c3-1133-4e65-b58f-7d814e35ecaf",
      "slug": "mit-the-great-british-bake-off-e23067c3-1133-4e65-b58f-7d814e35ecaf",
      "university_id": 135,
      "additional_university_ids": [

      ],
      "discipline_id": 160,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 2,
      "questions_count": 1,
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
      "chapters_updated_at": "2016-12-15T11:57:01.566Z",
      "updated_at": "2016-12-15T11:57:03.193Z",
      "shortname": "mit-the-great-british-bake-off-e23067c3-1133-4e65-b58f-7d814e35ecaf",
      "topic_id": 160,
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
curl "api.goskive.com/v2/files/5/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer f081cf4337d0c02c7fccf44fd1aac536ba806402a2ecd5793b3adc0879c65811"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/21/download
Content-Type: application/json
Authorization: Bearer f4ef2b95b17c265dd85533e2d3817f6cf1903d23ee95a46856996f0cfbc72aba
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4ef2b95b17c265dd85533e2d3817f6cf1903d23ee95a46856996f0cfbc72aba"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/20/report
Content-Type: application/json
Authorization: Bearer c4e5b52ef27d664a300dc149d865b753598e49b688fd74572d49cf371daebcb0
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
	-H "Authorization: Bearer c4e5b52ef27d664a300dc149d865b753598e49b688fd74572d49cf371daebcb0"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/15/bookmark
Content-Type: application/json
Authorization: Bearer 3845128c91c5a920901695ac90c6229a4f2b5f19c8c3f585988968699e1e92a5
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
	-H "Authorization: Bearer 3845128c91c5a920901695ac90c6229a4f2b5f19c8c3f585988968699e1e92a5"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/16/upvote
Content-Type: application/json
Authorization: Bearer a962c7b257f09ea2880c1d8e670b48e6634e1c68549323657e08cc5f4b674b02
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a962c7b257f09ea2880c1d8e670b48e6634e1c68549323657e08cc5f4b674b02"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/61/comments
Content-Type: application/json
Authorization: Bearer e6856a0ed7001f1d789e3b0bb1a631a737675d75a33795a4b77f4c78e6deab9c
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
    "id": 15,
    "author_id": 538,
    "reply_to_id": null,
    "created_at": "2016-12-15T11:57:08.766Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/61/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6856a0ed7001f1d789e3b0bb1a631a737675d75a33795a4b77f4c78e6deab9c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/59/comments
Content-Type: application/json
Authorization: Bearer 6dbbfe99d007136917413c2c36454552801aab069aa353cf3f2604cb99db9c53
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
    "id": 14,
    "author_id": 532,
    "reply_to_id": null,
    "created_at": "2016-12-15T11:57:08.121Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 30,
      "user_id": 532,
      "feedbackable_id": 59,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:08.119Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/59/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dbbfe99d007136917413c2c36454552801aab069aa353cf3f2604cb99db9c53"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/57/comments
Content-Type: application/json
Authorization: Bearer bba6ddbb2ab8177191a3b8a2f148954a72288a320cd9467b74341083d52ec3ca
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
      "id": 13,
      "author_id": 528,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:07.593Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 527,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:07.575Z",
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
curl "api.goskive.com/v2/flashcards/57/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bba6ddbb2ab8177191a3b8a2f148954a72288a320cd9467b74341083d52ec3ca"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/60/comments
Content-Type: application/json
Authorization: Bearer 300f57fc3805b13424083a140106fcf28a888ec137d901dafdf6a96263a4c018
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/flashcards/60/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 300f57fc3805b13424083a140106fcf28a888ec137d901dafdf6a96263a4c018"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/62/feedbacks
Content-Type: application/json
Authorization: Bearer 1147c609c4be5cec55e69cc922adffcad9323b9eb27d56cd87aa096694d1189d
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
    "id": 31,
    "user_id": 647,
    "feedbackable_id": 62,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T11:57:20.034Z",
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
curl "api.goskive.com/v2/flashcards/62/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1147c609c4be5cec55e69cc922adffcad9323b9eb27d56cd87aa096694d1189d"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer c6a94ebb0c877a5b2014d6a636fc018c97e6c67671bcdd0bae7d35c0bffda118
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
      "id": 36,
      "user_id": 665,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:21.248Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 664,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:21.235Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/66/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6a94ebb0c877a5b2014d6a636fc018c97e6c67671bcdd0bae7d35c0bffda118"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/45/votes
Content-Type: application/json
Authorization: Bearer ec138f94aa41d0c2051febc934f1bff70c50ecc40b430cb0955fdc3bf093f114
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
      "votable_id": 45,
      "user_id": 393
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 45,
      "user_id": 392
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 45,
      "user_id": 391
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/45/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec138f94aa41d0c2051febc934f1bff70c50ecc40b430cb0955fdc3bf093f114"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/27/republish
Content-Type: application/json
Authorization: Bearer 31189b84b841ef27e7e1f14178261c77823268d26e0c1eb0b21f0e248b95d8bc
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
curl "api.goskive.com/v2/flashcards/27/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31189b84b841ef27e7e1f14178261c77823268d26e0c1eb0b21f0e248b95d8bc"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/8/bookmark
Content-Type: application/json
Authorization: Bearer c28a2e03914eec5143c5ed3a4b9ce5288f65ff4e16644cdf8f61fe2d416928f0
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/8/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c28a2e03914eec5143c5ed3a4b9ce5288f65ff4e16644cdf8f61fe2d416928f0"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/7
Content-Type: application/json
Authorization: Bearer 4fc6e22faaf647713cab7c43b062602eba5808b160d038978e239b4443df9d8f
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fc6e22faaf647713cab7c43b062602eba5808b160d038978e239b4443df9d8f"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/9/downvote
Content-Type: application/json
Authorization: Bearer ff711ff9d1966b6ab9f5db6c14f92c0f3b3802b8ca8937ae511834e1ccce4c1d
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/9/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff711ff9d1966b6ab9f5db6c14f92c0f3b3802b8ca8937ae511834e1ccce4c1d"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/5
Content-Type: application/json
Authorization: Bearer 80717563ab00176b3f53ec734e8dc365c298b512991b3740a0daef6c70cca8bc
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
    "id": 5,
    "obfuscated_id": "iw-7peoPwEU",
    "author_id": 69,
    "chapter_id": 13,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:56:28.572Z",
    "created_at": "2016-12-15T11:56:28.572Z",
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
curl "api.goskive.com/v2/flashcards/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80717563ab00176b3f53ec734e8dc365c298b512991b3740a0daef6c70cca8bc"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/25/report
Content-Type: application/json
Authorization: Bearer ddaf08f37a0191b92f719c2c84aa35a8715532f95f7fa5c7e3b54170bca5aecf
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/25/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddaf08f37a0191b92f719c2c84aa35a8715532f95f7fa5c7e3b54170bca5aecf"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/6/bookmark
Content-Type: application/json
Authorization: Bearer 092611e99de3be23d970b58ebfebcc5efaa9659dfb115e7f95e0e3d29f8d348a
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/6/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 092611e99de3be23d970b58ebfebcc5efaa9659dfb115e7f95e0e3d29f8d348a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/28/upvote
Content-Type: application/json
Authorization: Bearer 938cd55eacf0498e2d9792a80fdf5f2b8b3ab345ddb46a312841ec067ef8cf76
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 938cd55eacf0498e2d9792a80fdf5f2b8b3ab345ddb46a312841ec067ef8cf76"
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
    "key": "cache/9821b6f1e69cffc09c4ef65016e0012b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxMjo1NjozNVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzk4MjFiNmYxZTY5Y2ZmYzA5YzRlZjY1MDE2ZTAwMTJiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTE1NjM1WiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T115635Z",
    "x-amz-signature": "29f00ec8096bb787e60cf8d32e167a747b561357c5f57ff3d5a299b6904bba67"
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
Authorization: Bearer cfdef84a2a80a89a4c5062d59608689ecaad34f310b2244df594311537a9dbff
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
	-H "Authorization: Bearer cfdef84a2a80a89a4c5062d59608689ecaad34f310b2244df594311537a9dbff"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer d70424a7bfcb87f41e07f34e6a6f9922e7c7600c1d988d644cf006368593332e
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
	-H "Authorization: Bearer d70424a7bfcb87f41e07f34e6a6f9922e7c7600c1d988d644cf006368593332e"
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
{"password":{"reset_password_token":"9jcdSY21Ns6nyaeUdT3L","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 211,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T11:56:41.356Z",
  "updated_at": "2016-12-15T11:56:41.524Z",
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
  "audit_id": 7520
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"9jcdSY21Ns6nyaeUdT3L","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/6/comments
Content-Type: application/json
Authorization: Bearer 99c5cb95868e717081bf6b41aeb4a5cb1bbcacd87126a8b67b788a28b2fcded7
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
    "id": 2,
    "author_id": 55,
    "reply_to_id": null,
    "created_at": "2016-12-15T11:56:26.504Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/6/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99c5cb95868e717081bf6b41aeb4a5cb1bbcacd87126a8b67b788a28b2fcded7"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/5/comments
Content-Type: application/json
Authorization: Bearer 7f0843bd00a44134451c2c6ebcfe329ada24a2cdf3b66fb33d8d7622f7586817
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
    "id": 1,
    "author_id": 52,
    "reply_to_id": null,
    "created_at": "2016-12-15T11:56:25.839Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 52,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:56:25.835Z",
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/5/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f0843bd00a44134451c2c6ebcfe329ada24a2cdf3b66fb33d8d7622f7586817"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/9/comments
Content-Type: application/json
Authorization: Bearer 6c6a1a89ce74bf04ea26929ac592bbf2c693ad546e1c9b5e7967b01f9f6b751e
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
      "author_id": 68,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:56:27.624Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 67,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:56:27.607Z",
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
curl "api.goskive.com/v2/questions/9/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c6a1a89ce74bf04ea26929ac592bbf2c693ad546e1c9b5e7967b01f9f6b751e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/7/comments
Content-Type: application/json
Authorization: Bearer 840934d17333728c7278d86b5595c9af2acbd95d0b4651ae93ceeee23368b387
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
| comment[feedback][id] | Feedback ID |
| comment[feedback][user_id] | Creator ID |
| comment[feedback][feedbackable_id] | Feedbackable ID |
| comment[feedback][feedbackable_type] | Feedbackable Type |
| comment[feedback][workflow_state] | Workflow State |
| comment[feedback][flags] | Flags |
| comment[feedback][updated_at] | Updated at |


```shell
curl "api.goskive.com/v2/questions/7/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 840934d17333728c7278d86b5595c9af2acbd95d0b4651ae93ceeee23368b387"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/120/feedbacks
Content-Type: application/json
Authorization: Bearer 59b649dda34033264b96587c2fd90a6d18e0f50b30b4f99bc36c4def09e681b5
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
    "id": 45,
    "user_id": 801,
    "feedbackable_id": 120,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T11:57:35.954Z",
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
curl "api.goskive.com/v2/questions/120/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59b649dda34033264b96587c2fd90a6d18e0f50b30b4f99bc36c4def09e681b5"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/119/feedbacks
Content-Type: application/json
Authorization: Bearer 4b46ee72f2bd14fdb1a11624173907274a842bbc4bb6cd95697521201634b9c3
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
      "user_id": 800,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:35.596Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 799,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:35.585Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/119/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b46ee72f2bd14fdb1a11624173907274a842bbc4bb6cd95697521201634b9c3"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/49/votes
Content-Type: application/json
Authorization: Bearer 4657c69a2ab30cda896be5871a1ed2bda093f143cda7e661d81451ee3e7f39cb
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
      "votable_id": 49,
      "user_id": 487
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 486
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 485
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4657c69a2ab30cda896be5871a1ed2bda093f143cda7e661d81451ee3e7f39cb"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/62/republish
Content-Type: application/json
Authorization: Bearer f5dcc22a65dfe450f024d2825015a2d86cacde14ef7848f79cb514bc82f1d729
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
curl "api.goskive.com/v2/questions/62/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5dcc22a65dfe450f024d2825015a2d86cacde14ef7848f79cb514bc82f1d729"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/81/bookmark
Content-Type: application/json
Authorization: Bearer b895c486b8d316f8ce0c416d3068adc3e2903b92014f201e0b2dc6aa880cfca6
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/81/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b895c486b8d316f8ce0c416d3068adc3e2903b92014f201e0b2dc6aa880cfca6"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/80
Content-Type: application/json
Authorization: Bearer 41670108c45bbe9c56e5f3974e29107106614d85d22140d6886fb652c4d169e1
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/80" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41670108c45bbe9c56e5f3974e29107106614d85d22140d6886fb652c4d169e1"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/59/downvote
Content-Type: application/json
Authorization: Bearer cf69db2469363b679ad260109d7195e445a337b6328f4b8a849ed3bb8de391b4
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/59/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf69db2469363b679ad260109d7195e445a337b6328f4b8a849ed3bb8de391b4"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/79
Content-Type: application/json
Authorization: Bearer 2c85a51f2236d10d522c39074df51d133f35786ec41b0119cc858e3624ed6a07
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 612,
    "chapter_id": 148,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:16.763Z",
    "created_at": "2016-12-15T11:57:16.680Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/79" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c85a51f2236d10d522c39074df51d133f35786ec41b0119cc858e3624ed6a07"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/57/report
Content-Type: application/json
Authorization: Bearer 4ceff23d955102057f69dd6d08c21d6d9fbab294b18d40f866ff82499e8410d8
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/57/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ceff23d955102057f69dd6d08c21d6d9fbab294b18d40f866ff82499e8410d8"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/60/bookmark
Content-Type: application/json
Authorization: Bearer e9205c7b9cb9b1eced82983423b1c56a32f9f8cfb82af5c7d4465fa1b642a9c6
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
	-H "Authorization: Bearer e9205c7b9cb9b1eced82983423b1c56a32f9f8cfb82af5c7d4465fa1b642a9c6"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/63
Content-Type: application/json
Authorization: Bearer c11abfcd493b904c405befa23b2756e4eaae6753aee131cf7b4251ad9202a32b
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":63,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T11:57:11.399Z","updated_at":"2016-12-15T11:57:11.479Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":132,"author_id":559,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 63,
    "obfuscated_id": "k3ebr8XrqxE",
    "author_id": 559,
    "chapter_id": 132,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T11:57:11.566Z",
    "created_at": "2016-12-15T11:57:11.399Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x00000013091628>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 127,
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
curl "api.goskive.com/v2/questions/63" -d '{"question":{"question":{"id":63,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T11:57:11.399Z","updated_at":"2016-12-15T11:57:11.479Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":132,"author_id":559,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c11abfcd493b904c405befa23b2756e4eaae6753aee131cf7b4251ad9202a32b"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/58/upvote
Content-Type: application/json
Authorization: Bearer 97c29df139316625d68139c1d63a133bb7a39ec8e0194963875d63b8fb323b23
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/58/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97c29df139316625d68139c1d63a133bb7a39ec8e0194963875d63b8fb323b23"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 7b9d7ed9f8355d210707d351f4b9127138b9b622546077bb953291be83026da6
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
      "creator_id": 451,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "discipline_id": 153,
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
      "updated_at": "2016-12-15T11:57:01.110Z",
      "shortname": "mit-pizza-201",
      "topic_id": 153,
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
	-H "Authorization: Bearer 7b9d7ed9f8355d210707d351f4b9127138b9b622546077bb953291be83026da6"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer e834a42b49c2bf364d5f0c6ef3f7fbb8ac77f861eae2b990c7d57f4a97f2a89a
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
      "id": 127,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-107",
      "html_url": "https://goskive.com/university/uni-107",
      "slug": "uni-107",
      "name": "National School of Pizza",
      "short_name": "Uni 107",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/626eb8c285543ccd5422ddc0dff200a7.jpg",
      "image_url_small": "memory://universities/aa3d3583806acf359a880751f88e60d8.jpg",
      "image_thumb_url": "memory://universities/3ec6f8d13ae08768c06c74529b49a05f.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T11:57:00.756Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 126,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-106",
      "html_url": "https://goskive.com/university/uni-106",
      "slug": "uni-106",
      "name": "National School of Pastry",
      "short_name": "Uni 106",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/b23454e135a000dbb210854f4c28fc04.jpg",
      "image_url_small": "memory://universities/e22668930861d996b5a05ac7102d2bcd.jpg",
      "image_thumb_url": "memory://universities/be31697dcf7384883d39c9a652ce7d73.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T11:57:00.545Z",
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
	-H "Authorization: Bearer e834a42b49c2bf364d5f0c6ef3f7fbb8ac77f861eae2b990c7d57f4a97f2a89a"
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
      "id": 76,
      "name": "Fundamental transitional conglomeration",
      "name_translations": {
        "en": "Fundamental transitional conglomeration"
      },
      "discipline_id": 76
    },
    {
      "id": 77,
      "name": "Enhanced clear-thinking circuit",
      "name_translations": {
        "en": "Enhanced clear-thinking circuit"
      },
      "discipline_id": 77
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
GET /v2/topics/75
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
    "id": 75,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 75
  }
}
```



```shell
curl "api.goskive.com/v2/topics/75" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 38f914581dc0cf899562c5141596b185a9a29b71bb126dd9c3f85f4858256024
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
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-46",
      "html_url": "https://goskive.com/university/uni-46",
      "slug": "uni-46",
      "name": "University 46",
      "short_name": "Uni 46",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/426201b7f519e121a4691422b62be629.jpg",
      "image_url_small": "memory://universities/6f8f2a14a90cf9326ae9f1e31f7d27b1.jpg",
      "image_thumb_url": "memory://universities/6d8f9a7a16788f90a69f5e5b9d930dc6.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T11:56:40.351Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 65,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-47",
      "html_url": "https://goskive.com/university/uni-47",
      "slug": "uni-47",
      "name": "University 47",
      "short_name": "Uni 47",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/9105ddea2c33aa6c3252af79f27978c1.jpg",
      "image_url_small": "memory://universities/07ccf10215a5e5bf927f315e265e6c0e.jpg",
      "image_thumb_url": "memory://universities/d634c155a5258bc023bf92fb495bfc9f.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T11:56:40.418Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 66,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-48",
      "html_url": "https://goskive.com/university/uni-48",
      "slug": "uni-48",
      "name": "University 48",
      "short_name": "Uni 48",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/e1f5614637f981083d2efa8e5fb0568a.jpg",
      "image_url_small": "memory://universities/da664d6c7f0b0bccf6fa4f610c85b523.jpg",
      "image_thumb_url": "memory://universities/0e0b02864bf51c914bcfb7b6f54c2b8d.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T11:56:40.486Z",
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
	-H "Authorization: Bearer 38f914581dc0cf899562c5141596b185a9a29b71bb126dd9c3f85f4858256024"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 77db0c743c65221b5b5ba6a1b5da1cf20a01e8c7780807d527b8170cfbec25cd
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
    "id": 67,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/6a041787659c69475b20efbf1bb3e5d2.jpg",
    "image_url_small": "memory://universities/d99ef760a538589cbc65928ba6317622.jpg",
    "image_thumb_url": "memory://universities/b80729ce9b2229ba151a0964d2594b1a.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T11:56:40.648Z",
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
	-H "Authorization: Bearer 77db0c743c65221b5b5ba6a1b5da1cf20a01e8c7780807d527b8170cfbec25cd"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4346a76f545b4187cc698f27f7d629240a49dfdf8c42a92f2ce08e0c15089e66
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":39,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 44,
    "id": 39,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 17,
    "additional_university_ids": [

    ],
    "discipline_id": 39,
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
    "chapters_updated_at": "2016-12-15T11:56:24.290Z",
    "updated_at": "2016-12-15T11:56:24.442Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 5,
        "updated_at": "2016-12-15T11:56:24.430Z",
        "course_id": 39,
        "author_id": 44,
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
        "id": 6,
        "updated_at": "2016-12-15T11:56:24.445Z",
        "course_id": 39,
        "author_id": 44,
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
        "id": 7,
        "updated_at": "2016-12-15T11:56:24.457Z",
        "course_id": 39,
        "author_id": 44,
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
    "topic_id": 39,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":39,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4346a76f545b4187cc698f27f7d629240a49dfdf8c42a92f2ce08e0c15089e66"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer dc4ddb8c9b60ddf988c635ca275fa9fede28094f0e364deecdf077f1201cf0f4
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}
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
    "creator_id": 45,
    "id": 40,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 18,
    "additional_university_ids": [

    ],
    "discipline_id": 40,
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
    "updated_at": "2016-12-15T11:56:24.689Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 40,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":40,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc4ddb8c9b60ddf988c635ca275fa9fede28094f0e364deecdf077f1201cf0f4"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a117f7861961433e991b64bb752be6608719c4b992500285ef2c3a87e9face58
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
      "creator_id": 12,
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "discipline_id": 11,
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
      "updated_at": "2016-12-15T11:56:20.935Z",
      "shortname": "fu-course-11",
      "topic_id": 11,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 12,
      "id": 12,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 4,
      "additional_university_ids": [

      ],
      "discipline_id": 12,
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
      "chapters_updated_at": "2016-12-15T11:56:20.743Z",
      "updated_at": "2016-12-15T11:56:21.183Z",
      "shortname": "fu-course-12",
      "topic_id": 12,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a117f7861961433e991b64bb752be6608719c4b992500285ef2c3a87e9face58"
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
      "creator_id": 22,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "discipline_id": 19,
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
      "updated_at": "2016-12-15T11:56:21.883Z",
      "shortname": "fu-course-19",
      "topic_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 22,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "discipline_id": 20,
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
      "chapters_updated_at": "2016-12-15T11:56:21.717Z",
      "updated_at": "2016-12-15T11:56:22.132Z",
      "shortname": "fu-course-20",
      "topic_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
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
Authorization: Bearer 4caa934fc3c0a6589544c8a23d281ea3b9077354315884ae0a0d38fae5c5ec98
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
      "creator_id": 19,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 6,
      "additional_university_ids": [

      ],
      "discipline_id": 15,
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
      "updated_at": "2016-12-15T11:56:21.597Z",
      "shortname": "fu-course-15",
      "topic_id": 15,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 19,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 6,
      "additional_university_ids": [

      ],
      "discipline_id": 16,
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
      "updated_at": "2016-12-15T11:56:21.631Z",
      "shortname": "fu-course-16",
      "topic_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4caa934fc3c0a6589544c8a23d281ea3b9077354315884ae0a0d38fae5c5ec98"
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
      "creator_id": 27,
      "id": 23,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 9,
      "additional_university_ids": [

      ],
      "discipline_id": 23,
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
      "updated_at": "2016-12-15T11:56:22.421Z",
      "shortname": "fu-course-23",
      "topic_id": 23,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 27,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 9,
      "additional_university_ids": [

      ],
      "discipline_id": 24,
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
      "updated_at": "2016-12-15T11:56:22.456Z",
      "shortname": "fu-course-24",
      "topic_id": 24,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
Authorization: Bearer 6d7bac73265b366d82b75bf44f316e0a7c44ee0cdf07316abe72c45c19c3f007
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
  "id": 196,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T11:56:39.414Z",
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
	-H "Authorization: Bearer 6d7bac73265b366d82b75bf44f316e0a7c44ee0cdf07316abe72c45c19c3f007"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/200
Content-Type: application/json
Authorization: Bearer 11319f721394fc5e41aa1edaaf9c4d4090c80b4ccd0119f1d67956d184dba78f
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
    "id": 200,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 63,
    "fields_of_study": [
      93,
      94
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T11:56:40.114Z",
    "updated_at": "2016-12-15T11:56:40.114Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/200" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11319f721394fc5e41aa1edaaf9c4d4090c80b4ccd0119f1d67956d184dba78f"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/202
Content-Type: application/json
Authorization: Bearer 004bfc9ab31cbd482bc736c36ec11f4853ededdf43973c504a1693c1885f35a7
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
    "id": 202,
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
    "created_at": "2016-12-15T11:56:40.223Z",
    "updated_at": "2016-12-15T11:56:40.223Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/202" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 004bfc9ab31cbd482bc736c36ec11f4853ededdf43973c504a1693c1885f35a7"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/7
Content-Type: application/json
Authorization: Bearer 5c7415f1e975b1ae918f8ae4f1a0839111d19c81c2c2dbe90d337939cc8bb6e4
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c7415f1e975b1ae918f8ae4f1a0839111d19c81c2c2dbe90d337939cc8bb6e4"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/9
Content-Type: application/json
Authorization: Bearer 3552cb6f9c29a05f2f5a18d95b0d4a65e43856ad81be7f62d071d95c7bd8fe96
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
    "id": 9,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 18,
    "user_id": 185
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3552cb6f9c29a05f2f5a18d95b0d4a65e43856ad81be7f62d071d95c7bd8fe96"
```
