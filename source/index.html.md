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
Authorization: Basic YjcxMmJjOGRkZThkZDA5NGYxOTBjZjNiN2I2YmZiOGUyZGY2ZTViOGU3OGY4
ZDYyOTZjM2M5M2NlMTk0ODMzMzo3YzFlODE2YjcwNDMxMTk4YWI0ODQ1Njlk
MWNlNDcxNzVhNDZlYThkZjU3ZWM2ODA3MTkwNzU0YTFmNjY1NmM3

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
	-u b712bc8dde8dd094f190cf3b7b6bfb8e2df6e5b8e78f8d6296c3c93ce1948333:7c1e816b70431198ab484569d1ce47175a46ea8df57ec6807190754a1f6656c7
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"05c009e1d107c530c757c49d5e495e32761a3f7083920775fe16db10d01629b6","client_secret":"1537e4e2eb7ac323a16217d66adf76cf3964f79d3cee6e8f93bc340586ec6311"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"05c009e1d107c530c757c49d5e495e32761a3f7083920775fe16db10d01629b6","client_secret":"1537e4e2eb7ac323a16217d66adf76cf3964f79d3cee6e8f93bc340586ec6311"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"b5ae37d1338c029c2acf7496a27aac32d39468b99b7c3abede6f0dde551c6417","client_secret":"84558503825583c9c49c1d29fc7f06423b194cda7727945d7892564a6621d8ab"}
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
  "access_token": "082fd982d6683422509f2da59530cc19eb88f95239a4f96afefda10397e8acb0",
  "token_type": "bearer",
  "created_at": 1478605193
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"b5ae37d1338c029c2acf7496a27aac32d39468b99b7c3abede6f0dde551c6417","client_secret":"84558503825583c9c49c1d29fc7f06423b194cda7727945d7892564a6621d8ab"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NDdiM2QxNTFhYzMyMzhhMzA3YjdmYmZjNWJmODlmMTExMDM1ODIzNzIyZjg1
YzNmZTUyNDZkYWUxNGJmY2QyNjoyYjNhYjEyYzkzZjY4YzViZDY5YmQ2NjEw
YTI3OTIxMWM5NzczM2U1ZWJjMTA0YWM2ZTZhNmVhMTQ3M2VlODIx

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
  "access_token": "77d921005e6915d510b9c96950ebc30405e290d30b336a1f63aaa4633df5ff67",
  "token_type": "bearer",
  "created_at": 1478605193
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 47b3d151ac3238a307b7fbfc5bf89f111035823722f85c3fe5246dae14bfcd26:2b3ab12c93f68c5bd69bd6610a279211c97733e5ebc104ac6e6a6ea1473ee821
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a49a86fd0e6ca7482134f7e4b5d88454f8963e32eafc014d89660e4bbefac68b","client_secret":"fe6809910ca3449d479d84ad2abc0520498306a847e400b0e43cbca0e6477423"}
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
  "access_token": "05de2dc77894e7e38cbe16cebc0da8a65792f8159fd31e463de1bb70d6d7358d",
  "token_type": "bearer",
  "created_at": 1478605193
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a49a86fd0e6ca7482134f7e4b5d88454f8963e32eafc014d89660e4bbefac68b","client_secret":"fe6809910ca3449d479d84ad2abc0520498306a847e400b0e43cbca0e6477423"}' -X POST \
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
GET /v2/campaigns/9
Content-Type: application/json
Authorization: Bearer 77fef2b13fac5995699176a112eec307f31d60567f9a3a1a7ebf1188e9c7a50c
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
    "id": 9,
    "title": "Recruiting pastry chefs",
    "company_id": 16,
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
curl "api.goskive.com/v2/campaigns/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77fef2b13fac5995699176a112eec307f31d60567f9a3a1a7ebf1188e9c7a50c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/154/flashcards
Content-Type: application/json
Authorization: Bearer b5fa6b036e65181a3b596da8c9dd64883d02ce6a861d697df581c5b8dd1ca21f
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":154,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 857,
    "chapter_id": 154,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:46.343Z",
    "created_at": "2016-11-08T11:40:46.343Z",
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
curl "api.goskive.com/v2/chapters/154/flashcards" -d '{"flashcard":{"chapter_id":154,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5fa6b036e65181a3b596da8c9dd64883d02ce6a861d697df581c5b8dd1ca21f"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/153/flashcards
Content-Type: application/json
Authorization: Bearer 707dc4a4b9d49f66946d2f3bbfafba86c99520d1054a9e01f81a0651e5b69904
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 852,
      "chapter_id": 153,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:46.069Z",
      "created_at": "2016-11-08T11:40:46.069Z",
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 852,
      "chapter_id": 153,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:46.106Z",
      "created_at": "2016-11-08T11:40:46.106Z",
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 852,
      "chapter_id": 153,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:46.141Z",
      "created_at": "2016-11-08T11:40:46.141Z",
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
	-H "Authorization: Bearer 707dc4a4b9d49f66946d2f3bbfafba86c99520d1054a9e01f81a0651e5b69904"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/105/questions
Content-Type: application/json
Authorization: Bearer b99554c19537d411c3bec46bf8964073895917878908ab67706fe07027e648e1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 83,
    "obfuscated_id": "FCSR-nKROLo",
    "author_id": 662,
    "chapter_id": 105,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:30.404Z",
    "created_at": "2016-11-08T11:40:30.404Z",
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
        "id": 167,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 168,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 169,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 170,
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
curl "api.goskive.com/v2/chapters/105/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":105,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b99554c19537d411c3bec46bf8964073895917878908ab67706fe07027e648e1"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/103/questions
Content-Type: application/json
Authorization: Bearer b2cd47d7c99fc5f34a92fa42f24eb1364664d42de13ee21f2499fe9ce995d31f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 81,
    "obfuscated_id": "jHF1owx40fU",
    "author_id": 656,
    "chapter_id": 103,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:29.317Z",
    "created_at": "2016-11-08T11:40:29.317Z",
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
        "id": 163,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 164,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/103/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":103,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2cd47d7c99fc5f34a92fa42f24eb1364664d42de13ee21f2499fe9ce995d31f"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/104/questions
Content-Type: application/json
Authorization: Bearer ac3566f38be4ddc887a91056fd1a77df8392a80d96faf2c27637bd9a144807f2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":104,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 82,
    "obfuscated_id": "D5TJ6kac5FE",
    "author_id": 659,
    "chapter_id": 104,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:29.865Z",
    "created_at": "2016-11-08T11:40:29.865Z",
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
        "id": 165,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 166,
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
curl "api.goskive.com/v2/chapters/104/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":104,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac3566f38be4ddc887a91056fd1a77df8392a80d96faf2c27637bd9a144807f2"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/102/questions
Content-Type: application/json
Authorization: Bearer 64dda857859d938b71a38782214af1fc1fca359e129352a00c4d426e0376b2a9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":102,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 80,
    "obfuscated_id": "94gVa2GR5x8",
    "author_id": 653,
    "chapter_id": 102,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:28.785Z",
    "created_at": "2016-11-08T11:40:28.785Z",
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
        "id": 160,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 161,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 162,
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
curl "api.goskive.com/v2/chapters/102/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":102,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64dda857859d938b71a38782214af1fc1fca359e129352a00c4d426e0376b2a9"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/100/questions
Content-Type: application/json
Authorization: Bearer 78e9ab0eea238ad25d98985054ff7c4b9d892873feac073f81f020a9db827e2e
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 644,
      "chapter_id": 100,
      "position": 68,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:27.982Z",
      "created_at": "2016-11-08T11:40:27.865Z",
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
      "author_id": 645,
      "chapter_id": 100,
      "position": 69,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:28.202Z",
      "created_at": "2016-11-08T11:40:28.053Z",
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
      "author_id": 646,
      "chapter_id": 100,
      "position": 70,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-08T11:40:28.397Z",
      "created_at": "2016-11-08T11:40:28.275Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/100/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78e9ab0eea238ad25d98985054ff7c4b9d892873feac073f81f020a9db827e2e"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/94
Content-Type: application/json
Authorization: Bearer 9ff328b61d52a3b3c6ec54d22a56fd64494ded5e19bfe90889dd8f8fd3f10e65
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
curl "api.goskive.com/v2/chapters/94" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ff328b61d52a3b3c6ec54d22a56fd64494ded5e19bfe90889dd8f8fd3f10e65"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/96
Content-Type: application/json
Authorization: Bearer bccd2cb2bce1ea0e02a1647792714e1814ba8f0cb782d4c5311d99c957f1a6b7
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
curl "api.goskive.com/v2/chapters/96" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bccd2cb2bce1ea0e02a1647792714e1814ba8f0cb782d4c5311d99c957f1a6b7"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/97
Content-Type: application/json
Authorization: Bearer 8d86c8b99802e1ce427240bdbf35a0c5b8edb62fec9a5cb20dd453b18fbec5ed
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
curl "api.goskive.com/v2/chapters/97" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d86c8b99802e1ce427240bdbf35a0c5b8edb62fec9a5cb20dd453b18fbec5ed"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/93
Content-Type: application/json
Authorization: Bearer 455cc4a2e719edcdc54caa1985298c7d53b717655cbd3d9ce94b89b58a07aaed
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/93" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 455cc4a2e719edcdc54caa1985298c7d53b717655cbd3d9ce94b89b58a07aaed"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/91
Content-Type: application/json
Authorization: Bearer aca2c1687f1291d7358a0d624c5dcaef279b85066a7e632db06371d927ec39cf
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
    "id": 91,
    "updated_at": "2016-11-08T11:40:23.496Z",
    "course_id": 196,
    "author_id": 572,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-08T11:40:22.954Z",
    "questions_updated_at": "2016-11-08T11:40:22.954Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 576,
        "chapter_id": 91,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:23.478Z",
        "created_at": "2016-11-08T11:40:23.478Z",
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
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 574,
        "chapter_id": 91,
        "position": 63,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:23.369Z",
        "created_at": "2016-11-08T11:40:23.248Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/91" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aca2c1687f1291d7358a0d624c5dcaef279b85066a7e632db06371d927ec39cf"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/99
Content-Type: application/json
Authorization: Bearer 478a80d1d4922705d00da0931fcac73726e7ffb84076e5a8b823b3e5a1f943de
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
    "id": 99,
    "updated_at": "2016-11-08T11:40:25.758Z",
    "course_id": 204,
    "author_id": 604,
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
curl "api.goskive.com/v2/chapters/99" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 478a80d1d4922705d00da0931fcac73726e7ffb84076e5a8b823b3e5a1f943de"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer e906187f78c7d5995532c2ceaea20915200592a622127348d0c5228856e1d40e
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
    "id": 4,
    "author_id": 112,
    "reply_to_id": 3,
    "created_at": "2016-11-08T11:39:48.264Z",
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
curl "api.goskive.com/v2/comments/3/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e906187f78c7d5995532c2ceaea20915200592a622127348d0c5228856e1d40e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/5/replies
Content-Type: application/json
Authorization: Bearer 4c10b5f9cc47db8db54ce85754537b1d1d888b659f6126553379268b3f10f18c
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
curl "api.goskive.com/v2/comments/5/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c10b5f9cc47db8db54ce85754537b1d1d888b659f6126553379268b3f10f18c"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 2ea390ed0eeb0c73460e35de835e3b45d28f86afaf8866f5d716064696325c78
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
	-H "Authorization: Bearer 2ea390ed0eeb0c73460e35de835e3b45d28f86afaf8866f5d716064696325c78"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/45/republish
Content-Type: application/json
Authorization: Bearer a78dd0d2c8e8eeada0b0787dd09a999548fdef1617a40f32d36b16a0bcfd3c20
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
curl "api.goskive.com/v2/comments/45/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a78dd0d2c8e8eeada0b0787dd09a999548fdef1617a40f32d36b16a0bcfd3c20"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer af87fc0566aef41f6597d610b79867967f4d9b8580dd242ef74d19e976d17ed7
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
	-H "Authorization: Bearer af87fc0566aef41f6597d610b79867967f4d9b8580dd242ef74d19e976d17ed7"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/44/report
Content-Type: application/json
Authorization: Bearer 18efb3547c217d605f81eca45d464330cf73c51b4e0087df3d0537870c35e918
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18efb3547c217d605f81eca45d464330cf73c51b4e0087df3d0537870c35e918"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 33a79a3010e3fb34a192a0283cc4ebc8f173e28028d234d8a2aa947d3d3f19e4
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
    "updated_at": "2016-11-08T11:40:57.330Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33a79a3010e3fb34a192a0283cc4ebc8f173e28028d234d8a2aa947d3d3f19e4"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 21096d3255ddc582ea65badb886f66e981256091975f9adbeeb62b9444c8904a
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
      "updated_at": "2016-11-08T11:40:57.447Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T11:40:57.451Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-08T11:40:57.455Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21096d3255ddc582ea65badb886f66e981256091975f9adbeeb62b9444c8904a"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/34/company_profiles
Content-Type: application/json
Authorization: Bearer e3af69cf73ab2fcfeeb1850fa10176f9d56548854d381b20fec071ee35df9d07
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
curl "api.goskive.com/v2/companies/34/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3af69cf73ab2fcfeeb1850fa10176f9d56548854d381b20fec071ee35df9d07"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/33/company_profiles
Content-Type: application/json
Authorization: Bearer 0d569d7482815913be29317804a2cb863845f92410ebd4e30e6097276b2158b8
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
curl "api.goskive.com/v2/companies/33/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d569d7482815913be29317804a2cb863845f92410ebd4e30e6097276b2158b8"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 1fc04455cd2c26e4906c9bbd890b1539ab53b07012da9c43b602b4720440d1bc
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
      "id": 1,
      "title": "Campaign 1",
      "company_id": 1,
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
      "id": 4,
      "title": "Campaign 4",
      "company_id": 4,
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
	-H "Authorization: Bearer 1fc04455cd2c26e4906c9bbd890b1539ab53b07012da9c43b602b4720440d1bc"
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
Authorization: Bearer b655cc1aa3f6c4e302863d3dc29722045ceb83a229b07745c1237916e2eeef7a
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
	-H "Authorization: Bearer b655cc1aa3f6c4e302863d3dc29722045ceb83a229b07745c1237916e2eeef7a"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c4ffc4795a2a6c1ed09d99edc8e7a110550d2e04eafc450c3fe796493a21d29d
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
    "id": 195,
    "updated_at": "2016-11-08T11:41:00.575Z",
    "course_id": 316,
    "author_id": 988,
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
	-H "Authorization: Bearer c4ffc4795a2a6c1ed09d99edc8e7a110550d2e04eafc450c3fe796493a21d29d"
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
      "id": 172,
      "updated_at": "2016-11-08T11:40:57.579Z",
      "course_id": 302,
      "author_id": 936,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 151",
      "position": 1
    },
    {
      "id": 173,
      "updated_at": "2016-11-08T11:40:57.603Z",
      "course_id": 302,
      "author_id": 937,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 152",
      "position": 2
    },
    {
      "id": 174,
      "updated_at": "2016-11-08T11:40:57.855Z",
      "course_id": 302,
      "author_id": 938,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T11:40:57.507Z",
      "questions_updated_at": "2016-11-08T11:40:57.507Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 153",
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
Authorization: Bearer b097b2606ab6a95b953bf1d91197e3c9cbbd9e966d8df04d7159eb83653eb099
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
      "updated_at": "2016-11-08T11:40:58.959Z",
      "course_id": 308,
      "author_id": 961,
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
      "updated_at": "2016-11-08T11:40:58.984Z",
      "course_id": 308,
      "author_id": 962,
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
      "updated_at": "2016-11-08T11:40:59.254Z",
      "course_id": 308,
      "author_id": 963,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-08T11:40:58.882Z",
      "questions_updated_at": "2016-11-08T11:40:58.882Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 165",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b097b2606ab6a95b953bf1d91197e3c9cbbd9e966d8df04d7159eb83653eb099"
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
      "id": 175,
      "updated_at": "2016-11-08T11:40:57.973Z",
      "course_id": 303,
      "author_id": 942,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 154",
      "position": 1
    },
    {
      "id": 176,
      "updated_at": "2016-11-08T11:40:57.997Z",
      "course_id": 303,
      "author_id": 943,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 155",
      "position": 2
    },
    {
      "id": 177,
      "updated_at": "2016-11-08T11:40:58.020Z",
      "course_id": 303,
      "author_id": 944,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 156",
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
Authorization: Bearer 23d81e12fbf11359258b88714d2f38c19ffb7ec6436fedeb916f3793afbae765
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
      "updated_at": "2016-11-08T11:40:59.572Z",
      "course_id": 310,
      "author_id": 970,
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
      "updated_at": "2016-11-08T11:40:59.597Z",
      "course_id": 310,
      "author_id": 971,
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
      "updated_at": "2016-11-08T11:40:59.621Z",
      "course_id": 310,
      "author_id": 972,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 168",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23d81e12fbf11359258b88714d2f38c19ffb7ec6436fedeb916f3793afbae765"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 03e53716e21653d27b1b5c708b72e73b17672dcf66289094f416bacf9a238a03
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
    "course_id": 189,
    "user_id": 552,
    "updated_at": "2016-11-08T11:40:21.687Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03e53716e21653d27b1b5c708b72e73b17672dcf66289094f416bacf9a238a03"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 99d2d07197421490a14fbfc7e644d8babdbeef13659aac544aebb23d733fd18f
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
      "course_id": 192,
      "user_id": 558,
      "updated_at": "2016-11-08T11:40:22.057Z"
    },
    {
      "id": 5,
      "course_id": 192,
      "user_id": 559,
      "updated_at": "2016-11-08T11:40:22.073Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99d2d07197421490a14fbfc7e644d8babdbeef13659aac544aebb23d733fd18f"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/117/files
Content-Type: application/json
Authorization: Bearer 06971b7476947237745a07898618bea33dad78c85db6492bd2da8c3d9fc53ef4
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
        "id": 401,
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
        "created_at": "2016-11-08T11:40:06.274Z",
        "updated_at": "2016-11-08T11:40:06.274Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T11:40:06.345Z",
      "updated_at": "2016-11-08T11:40:06.345Z",
      "course_id": 117,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
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
        "created_at": "2016-11-08T11:40:06.355Z",
        "updated_at": "2016-11-08T11:40:06.355Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T11:40:06.364Z",
      "updated_at": "2016-11-08T11:40:06.364Z",
      "course_id": 117,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 403,
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
        "created_at": "2016-11-08T11:40:06.372Z",
        "updated_at": "2016-11-08T11:40:06.372Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-08T11:40:06.381Z",
      "updated_at": "2016-11-08T11:40:06.381Z",
      "course_id": 117,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/117/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06971b7476947237745a07898618bea33dad78c85db6492bd2da8c3d9fc53ef4"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/118/files
Content-Type: application/json
Authorization: Bearer 2daf419af224eb9f529a4145454680b5c22b312ccfd065886e02383b9675c2b4
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
      "id": 406,
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
      "created_at": "2016-11-08T11:40:06.502Z",
      "updated_at": "2016-11-08T11:40:06.502Z"
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
    "created_at": "2016-11-08T11:40:06.534Z",
    "updated_at": "2016-11-08T11:40:06.534Z",
    "course_id": 118,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/118/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2daf419af224eb9f529a4145454680b5c22b312ccfd065886e02383b9675c2b4"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/119/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 35deedaf4a00decc54487489314967b8dcc0633cd4173ee179e02aa29cd84f8e
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
    "key": "cache/74b121993a12b836e5d6065016711756.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQxMjo0MDowNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzc0YjEyMTk5M2ExMmI4MzZlNWQ2MDY1MDE2NzExNzU2LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA4VDExNDAwNloifV19",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T114006Z",
    "x-amz-signature": "a2de4dbe814aafe9603f966a351dcc714369f1ef43090491c8d2319fe819de89"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/119/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35deedaf4a00decc54487489314967b8dcc0633cd4173ee179e02aa29cd84f8e"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 1525fc477e297171ff8d2cb08115b8e28aca85845770fc51e6bf3c8ae84c4bf4
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
	-H "Authorization: Bearer 1525fc477e297171ff8d2cb08115b8e28aca85845770fc51e6bf3c8ae84c4bf4"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a8e0e3448ac890f35fbe74fa6de0d2061dc536c1cbab44d8272daf19f44cbe67
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
	-H "Authorization: Bearer a8e0e3448ac890f35fbe74fa6de0d2061dc536c1cbab44d8272daf19f44cbe67"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f353ce108a4878102e99004e177177cf38008aa27e96c691fc53b63eab23581c
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
	-H "Authorization: Bearer f353ce108a4878102e99004e177177cf38008aa27e96c691fc53b63eab23581c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 609ef59bde601af0021bc4a7d5149aa38c07483f8ae08fefe3bbaab5387ed2e4
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
	-H "Authorization: Bearer 609ef59bde601af0021bc4a7d5149aa38c07483f8ae08fefe3bbaab5387ed2e4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 685b9d92a6b7f3011e7f0e1126b671e404ae5af128b31d8ae18e0e2831f30b10
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
	-H "Authorization: Bearer 685b9d92a6b7f3011e7f0e1126b671e404ae5af128b31d8ae18e0e2831f30b10"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 17cb3de925b64a45f3dddfd10406265b32e8e0a8b0ad9c3eb7cfd601d383cfa1
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
    "creator_id": 873,
    "id": 284,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 269,
    "additional_university_ids": [

    ],
    "discipline_id": 297,
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
    "chapters_updated_at": "2016-11-08T11:40:48.763Z",
    "updated_at": "2016-11-08T11:40:50.211Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 874,
        "chapter_id": 157,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.004Z",
        "created_at": "2016-11-08T11:40:50.004Z",
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
        "author_id": 874,
        "chapter_id": 158,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.076Z",
        "created_at": "2016-11-08T11:40:50.076Z",
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
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 874,
        "chapter_id": 157,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.045Z",
        "created_at": "2016-11-08T11:40:50.045Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 874,
        "chapter_id": 158,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.115Z",
        "created_at": "2016-11-08T11:40:50.115Z",
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
        "id": 107,
        "obfuscated_id": "_2rgp7tgq8o",
        "author_id": 874,
        "chapter_id": 157,
        "position": 94,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:48.987Z",
        "created_at": "2016-11-08T11:40:48.862Z",
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
            "id": 217,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 218,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 108,
        "obfuscated_id": "3MKez0MLRBM",
        "author_id": 874,
        "chapter_id": 157,
        "position": 95,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:49.162Z",
        "created_at": "2016-11-08T11:40:49.051Z",
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
            "id": 219,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 220,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 109,
        "obfuscated_id": "VSPyck5c2RY",
        "author_id": 874,
        "chapter_id": 158,
        "position": 96,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:49.364Z",
        "created_at": "2016-11-08T11:40:49.243Z",
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
            "id": 221,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 222,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 110,
        "obfuscated_id": "55JK4PuG2Hk",
        "author_id": 874,
        "chapter_id": 158,
        "position": 97,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:49.546Z",
        "created_at": "2016-11-08T11:40:49.430Z",
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
            "id": 223,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 224,
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
        "id": 157,
        "updated_at": "2016-11-08T11:40:50.164Z",
        "course_id": 284,
        "author_id": 873,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T11:40:48.763Z",
        "questions_updated_at": "2016-11-08T11:40:48.763Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 136",
        "position": 1
      },
      {
        "id": 158,
        "updated_at": "2016-11-08T11:40:50.204Z",
        "course_id": 284,
        "author_id": 873,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T11:40:48.763Z",
        "questions_updated_at": "2016-11-08T11:40:48.763Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 137",
        "position": 2
      }
    ],
    "topic_id": 296,
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
	-H "Authorization: Bearer 17cb3de925b64a45f3dddfd10406265b32e8e0a8b0ad9c3eb7cfd601d383cfa1"
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
    "creator_id": 879,
    "id": 285,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 270,
    "additional_university_ids": [

    ],
    "discipline_id": 298,
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
    "chapters_updated_at": "2016-11-08T11:40:50.338Z",
    "updated_at": "2016-11-08T11:40:51.821Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 879,
        "chapter_id": 159,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.546Z",
        "created_at": "2016-11-08T11:40:50.429Z",
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
      },
      {
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 879,
        "chapter_id": 160,
        "position": 102,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-08T11:40:50.929Z",
        "created_at": "2016-11-08T11:40:50.807Z",
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
      }
    ],
    "chapters": [
      {
        "id": 159,
        "updated_at": "2016-11-08T11:40:51.774Z",
        "course_id": 285,
        "author_id": 879,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T11:40:50.338Z",
        "questions_updated_at": "2016-11-08T11:40:50.338Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 138",
        "position": 1
      },
      {
        "id": 160,
        "updated_at": "2016-11-08T11:40:51.813Z",
        "course_id": 285,
        "author_id": 879,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-08T11:40:50.338Z",
        "questions_updated_at": "2016-11-08T11:40:50.338Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 139",
        "position": 2
      }
    ],
    "topic_id": 297,
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
PUT /v2/courses/282/pin
Content-Type: application/json
Authorization: Bearer 403c634a1c875b3673b5293259f0fc740841162ef842f30825d047ba312f1677
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/282/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 403c634a1c875b3673b5293259f0fc740841162ef842f30825d047ba312f1677"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/296/pin
Content-Type: application/json
Authorization: Bearer 6eda171ba30b19881543f8ebf8941b6c26aa154f46b142eb7638e2d7a7ebc6bb
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/296/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6eda171ba30b19881543f8ebf8941b6c26aa154f46b142eb7638e2d7a7ebc6bb"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b06a969e0ba22b8e3abf687ec5b72618d5f4fcb70b7689d2031ce267cc63fd7c
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
    "creator_id": 858,
    "id": 278,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 263,
    "additional_university_ids": [

    ],
    "discipline_id": 291,
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
    "updated_at": "2016-11-08T11:40:46.592Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 290,
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
	-H "Authorization: Bearer b06a969e0ba22b8e3abf687ec5b72618d5f4fcb70b7689d2031ce267cc63fd7c"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 58d65a0265c8f2ecb29f874e8cb7815e996bd3712a21efd61b1adb51c6433ac2
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
    "id": 498,
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
    "created_at": "2016-11-08T11:40:16.803Z",
    "updated_at": "2016-11-08T11:40:16.803Z",
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
	-H "Authorization: Bearer 58d65a0265c8f2ecb29f874e8cb7815e996bd3712a21efd61b1adb51c6433ac2"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8d6bd9d4086481ef24a7e6489178dcc3e5027612803b54108e3f5c53a03b4d67
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[150]}
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
    "id": 493,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      150
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T11:40:16.163Z",
    "updated_at": "2016-11-08T11:40:16.217Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[150]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d6bd9d4086481ef24a7e6489178dcc3e5027612803b54108e3f5c53a03b4d67"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer dd78a25fb92bf30e42949e11db446e0166d94104bb239111dbcb2c4298f1c156
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
    "id": 494,
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
    "created_at": "2016-11-08T11:40:16.248Z",
    "updated_at": "2016-11-08T11:40:16.248Z",
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
	-H "Authorization: Bearer dd78a25fb92bf30e42949e11db446e0166d94104bb239111dbcb2c4298f1c156"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c76d7b014d838c3d2093c9d66833172f3a27528d4f3c53dc0106921eba8ef200
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[152]}
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
    "id": 495,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      152
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T11:40:16.343Z",
    "updated_at": "2016-11-08T11:40:16.343Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[152]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c76d7b014d838c3d2093c9d66833172f3a27528d4f3c53dc0106921eba8ef200"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 99ce9ef8e651766107e2a33537c7d63c6f22c2e06fb021388df2510702cf09c8
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

154
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
    "id": 497,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/7ee09b6f96f11513be6f4082cbea3dd851cc37f1.jpg",
    "university_id": null,
    "fields_of_study": [
      154
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-08T11:40:16.489Z",
    "updated_at": "2016-11-08T11:40:16.773Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/512a4951e516904b116b22256897f9c2e3cc0774.jpg",
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

154
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 99ce9ef8e651766107e2a33537c7d63c6f22c2e06fb021388df2510702cf09c8"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 0b9cc2684e4aef3e243f0fd588e7c68f438a3f1dc3bdef69d4f5906b3b9d4df5
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
      "bookmarkable_id": 5,
      "bookmarkable_type": "Question"
    },
    {
      "id": 2,
      "bookmarkable_id": 6,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 7,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b9cc2684e4aef3e243f0fd588e7c68f438a3f1dc3bdef69d4f5906b3b9d4df5"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 22a12e6f04dca28968ac12500bd0b75520cee3caafc49f1449e26072b4d00a45
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
      "company_id": 29,
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
      "id": 12,
      "title": "Campaign 11",
      "company_id": 30,
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
	-H "Authorization: Bearer 22a12e6f04dca28968ac12500bd0b75520cee3caafc49f1449e26072b4d00a45"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer c76e81c7be7c021c262b44ceba519ce865014da589210f90726b91d02437fb6e
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
      "company_id": 25,
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
	-H "Authorization: Bearer c76e81c7be7c021c262b44ceba519ce865014da589210f90726b91d02437fb6e"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 780385c346dffc053179021789abe061c8d17f0e98b6ce8304edd57435f35653
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
      "creator_id": 212,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-69",
      "html_url": "https://goskive.com/course/mit-course-69",
      "slug": "mit-course-69",
      "university_id": 79,
      "additional_university_ids": [

      ],
      "discipline_id": 82,
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
      "updated_at": "2016-11-08T11:39:53.008Z",
      "shortname": "mit-course-69",
      "topic_id": 81,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 69",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 213,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-70",
      "html_url": "https://goskive.com/course/mit-course-70",
      "slug": "mit-course-70",
      "university_id": 80,
      "additional_university_ids": [

      ],
      "discipline_id": 83,
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
      "updated_at": "2016-11-08T11:39:53.091Z",
      "shortname": "mit-course-70",
      "topic_id": 82,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 70",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 780385c346dffc053179021789abe061c8d17f0e98b6ce8304edd57435f35653"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer f730b1cfe38c5decbfb866e04fb0b2c992822b533c8e66246ab04ba9315854d1
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
        "created_at": "2016-11-08T11:40:16.985Z",
        "updated_at": "2016-11-08T11:40:16.985Z",
        "file_url": "memory://b989f4e2932b03befc33a183e7032210.pdf",
        "course_id": 146,
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
        "created_at": "2016-11-08T11:40:17.065Z",
        "updated_at": "2016-11-08T11:40:17.065Z",
        "file_url": "memory://c369d7bb06556ce8cc5ccb0fcf529d4c.pdf",
        "course_id": 147,
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
        "created_at": "2016-11-08T11:40:17.139Z",
        "updated_at": "2016-11-08T11:40:17.139Z",
        "file_url": "memory://e627e3c5bbdf59bbf2b2459043337ad0.pdf",
        "course_id": 148,
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
	-H "Authorization: Bearer f730b1cfe38c5decbfb866e04fb0b2c992822b533c8e66246ab04ba9315854d1"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a81f5da5471f1a87587f04899e4127f15a8aa0e6813134651502695509e843b9
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T11:40:41.614Z"
      },
      "created_at": "2016-11-08T11:40:41.617Z",
      "updated_at": "2016-11-08T11:40:41.617Z",
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
      "company_id": 23,
      "company": {
        "id": 23,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T11:40:41.625Z"
      },
      "created_at": "2016-11-08T11:40:41.628Z",
      "updated_at": "2016-11-08T11:40:41.628Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a81f5da5471f1a87587f04899e4127f15a8aa0e6813134651502695509e843b9"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 1174c7da320a64fb4e8207030b8f564dee43b8d17af9d60f225236242d3bdc88
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
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T11:40:41.369Z"
      },
      "created_at": "2016-11-08T11:40:41.372Z",
      "updated_at": "2016-11-08T11:40:41.372Z",
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
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-08T11:40:41.386Z"
      },
      "created_at": "2016-11-08T11:40:41.389Z",
      "updated_at": "2016-11-08T11:40:41.389Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1174c7da320a64fb4e8207030b8f564dee43b8d17af9d60f225236242d3bdc88"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 07225fbaef9e7c457c932d00992c8c93930a83f2cab50fd3ac93087b21692041
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
      "created_at": "2016-11-08T11:40:43.244Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-11-08T11:40:43.353Z",
      "author_id": "819",
      "thread_subject_id": "267",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 19,
      "created_at": "2016-11-08T11:40:43.342Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-11-08T11:40:43.356Z",
      "author_id": "822",
      "thread_subject_id": "268",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-11-08T11:40:43.723Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-11-08T11:40:43.723Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 21,
      "created_at": "2016-11-08T11:40:44.089Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-11-08T11:40:44.089Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 22,
      "created_at": "2016-11-08T11:40:44.466Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 23,
      "updated_at": "2016-11-08T11:40:44.466Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 23,
      "created_at": "2016-11-08T11:40:44.759Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 98,
      "updated_at": "2016-11-08T11:40:44.759Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-11-08T11:40:45.056Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 99,
      "updated_at": "2016-11-08T11:40:45.056Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-11-08T11:40:45.348Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 100,
      "updated_at": "2016-11-08T11:40:45.348Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07225fbaef9e7c457c932d00992c8c93930a83f2cab50fd3ac93087b21692041"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/17
Content-Type: application/json
Authorization: Bearer 07236b08aadd4ade869d5fafc2a36a13492b8e2fc15270ed90a7ef4147a6b011
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-08T11:30:42.000Z"}}
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
    "created_at": "2016-11-08T11:40:43.078Z",
    "read_at": "2016-11-08T11:30:42.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 54,
    "updated_at": "2016-11-08T11:40:43.137Z",
    "author_id": "815",
    "thread_subject_id": "266",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/17" -d '{"notification":{"read_at":"2016-11-08T11:30:42.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07236b08aadd4ade869d5fafc2a36a13492b8e2fc15270ed90a7ef4147a6b011"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 43f5a9fbc2d47f6c56819572e836acf3267b463e387f26dee608fbf9bb75cd71
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
      "course_id": 8,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T11:39:39.506Z",
      "course_published": true,
      "updated_at": "2016-11-08T11:39:39.499Z"
    },
    {
      "id": 4,
      "course_id": 9,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-08T11:39:39.581Z",
      "course_published": true,
      "updated_at": "2016-11-08T11:39:39.574Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43f5a9fbc2d47f6c56819572e836acf3267b463e387f26dee608fbf9bb75cd71"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 2752ad71fde84f91941adb0982da87ee3344a77aea251b8c700444a04472a04b
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
    "course_id": 7,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-08T11:39:39.383Z",
    "course_published": true,
    "updated_at": "2016-11-08T11:39:39.375Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2752ad71fde84f91941adb0982da87ee3344a77aea251b8c700444a04472a04b"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 4cabaf81f6baa07a8a10b7b1b98f34ce904e6a033a74c82e19848f792c7697c3
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
    "course_id": 10,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-08T11:39:39.782Z",
    "course_published": true,
    "updated_at": "2016-11-08T11:39:39.771Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cabaf81f6baa07a8a10b7b1b98f34ce904e6a033a74c82e19848f792c7697c3"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 2fa777a0d2d85a33fb33b71890e4379b48d83290d33a3b57ebcf7488f08f20f7
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
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 1,
      "user_id": 1
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 1
    },
    {
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 3,
      "user_id": 1
    },
    {
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 4,
      "user_id": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2fa777a0d2d85a33fb33b71890e4379b48d83290d33a3b57ebcf7488f08f20f7"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/25
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
    "id": 25,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 23,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 25
      },
      {
        "id": 24,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 25
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/25" -X GET \
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
      "id": 23,
      "name": "Phased incremental analyzer",
      "name_translations": {
        "en": "Phased incremental analyzer"
      }
    },
    {
      "id": 24,
      "name": "Decentralized local capability",
      "name_translations": {
        "en": "Decentralized local capability"
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
PATCH /v2/feedbacks/33/close
Content-Type: application/json
Authorization: Bearer 3bc7a12a5f7796400b3b7b42399d3e90693025f470501d1c0f8b6f3b67ab1cca
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
    "id": 33,
    "user_id": 330,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-08T11:40:01.260Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/33/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3bc7a12a5f7796400b3b7b42399d3e90693025f470501d1c0f8b6f3b67ab1cca"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/10/fix
Content-Type: application/json
Authorization: Bearer 79504a8a556d47eadb4b634e6133cb1dc0400c37629c1a153f1504cef7c6720e
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
    "id": 10,
    "user_id": 229,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-08T11:39:53.748Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/10/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79504a8a556d47eadb4b634e6133cb1dc0400c37629c1a153f1504cef7c6720e"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/35
Content-Type: application/json
Authorization: Bearer 0f170590d0a493a04a19dd5ae9f6fc3faf5297bcef223bee1277a8619a54ff06
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
    "id": 35,
    "user_id": 340,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T11:40:01.739Z",
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
curl "api.goskive.com/v2/feedbacks/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f170590d0a493a04a19dd5ae9f6fc3faf5297bcef223bee1277a8619a54ff06"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/9/fix
Content-Type: application/json
Authorization: Bearer 4a2bc5b63fe673a98f2e7849c2c2da9d9ba25f7638fbeea78a47bdd20fa7d0e6
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
curl "api.goskive.com/v2/feedbacks/9/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a2bc5b63fe673a98f2e7849c2c2da9d9ba25f7638fbeea78a47bdd20fa7d0e6"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer 29a2b2b797f7ae995072955b31131dc71a3063734b915966f572f0723ea39e34
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
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29a2b2b797f7ae995072955b31131dc71a3063734b915966f572f0723ea39e34"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/34/close
Content-Type: application/json
Authorization: Bearer 078bc8fd753ac0b6ce059ab2316d5bc51db1e92d966cc6243660019b6926598d
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
curl "api.goskive.com/v2/feedbacks/34/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 078bc8fd753ac0b6ce059ab2316d5bc51db1e92d966cc6243660019b6926598d"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/36
Content-Type: application/json
Authorization: Bearer 1d9f4a6c64598afc8f4087adb538d11743b447e3cb0893aa1ed2fcec979eb104
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
    "id": 36,
    "user_id": 345,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T11:40:02.040Z",
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
curl "api.goskive.com/v2/feedbacks/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d9f4a6c64598afc8f4087adb538d11743b447e3cb0893aa1ed2fcec979eb104"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer a0413972f0d394efd4b85ca04f122fb8ba2a3cc24c9a044fe7c38216d13aac4e
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
curl "api.goskive.com/v2/files/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0413972f0d394efd4b85ca04f122fb8ba2a3cc24c9a044fe7c38216d13aac4e"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/20/bookmark
Content-Type: application/json
Authorization: Bearer 9936a3ebed89fbcf3d53477828ba4e2b33f926e768fc625d3d5b171bac59cd25
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/20/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9936a3ebed89fbcf3d53477828ba4e2b33f926e768fc625d3d5b171bac59cd25"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 192e27c01a638b0b32c82ae15783c58180dcaae6e774b76f0c1a65e5cb1ca97e
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
	-H "Authorization: Bearer 192e27c01a638b0b32c82ae15783c58180dcaae6e774b76f0c1a65e5cb1ca97e"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/12
Content-Type: application/json
Authorization: Bearer 56c1f96c8fcf45eeaa53903002a38f057dd3fea5b7ae4bf7c6bfcd92f83c47cd
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/0a697f7828fefca9584f100be1f9d53c.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T114026Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7621ba226ca82649b19a1caafa6587a71a05446e4bc8fb12b20005ed56f3d584",
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
	-H "Authorization: Bearer 56c1f96c8fcf45eeaa53903002a38f057dd3fea5b7ae4bf7c6bfcd92f83c47cd"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer 9323e363ae9cfceaf8db2a2ee7c6d5539611750db47fee7824f8786223475c74
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/8b4938344eff40f08448d90655674ad1.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161108%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161108T114026Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8507c2e8c9c6f7ebc5a83b801bd6796601bd1c5688d3cc3b875b87ca72a9be60",
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
	-H "Authorization: Bearer 9323e363ae9cfceaf8db2a2ee7c6d5539611750db47fee7824f8786223475c74"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer 076198e219556c50abb6e3e883a7f639c94fb2cac316a9206c0b2e4761f58846
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
    "id": 10,
    "uploader": {
      "id": 610,
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
      "created_at": "2016-11-08T11:40:26.098Z",
      "updated_at": "2016-11-08T11:40:26.098Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-08T11:40:26.174Z",
    "updated_at": "2016-11-08T11:40:26.174Z",
    "course_id": 207,
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
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 076198e219556c50abb6e3e883a7f639c94fb2cac316a9206c0b2e4761f58846"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/22/matched_courses?required_cu_count=2
Authorization: Bearer 12e8e862f45300afc018a535197e2511cc5f3961a3bea93833ba363b14c78243
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
      "creator_id": 791,
      "id": 262,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-3feff044-8ac0-4ba6-bc37-3683010afd12",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-3feff044-8ac0-4ba6-bc37-3683010afd12",
      "slug": "mit-the-great-british-bake-off-3feff044-8ac0-4ba6-bc37-3683010afd12",
      "university_id": 247,
      "additional_university_ids": [

      ],
      "discipline_id": 275,
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
      "chapters_updated_at": "2016-11-08T11:40:37.991Z",
      "updated_at": "2016-11-08T11:40:41.086Z",
      "shortname": "mit-the-great-british-bake-off-3feff044-8ac0-4ba6-bc37-3683010afd12",
      "topic_id": 274,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 786,
      "id": 261,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 246,
      "additional_university_ids": [

      ],
      "discipline_id": 274,
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
      "chapters_updated_at": "2016-11-08T11:40:37.991Z",
      "updated_at": "2016-11-08T11:40:40.530Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 273,
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
	-H "Authorization: Bearer 12e8e862f45300afc018a535197e2511cc5f3961a3bea93833ba363b14c78243"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/13/download
Content-Type: application/json
Authorization: Bearer 96dd0504c13d9abee65345ce24e917a30df3810059b5cf78e119a03c1c5bd02c
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
	-H "Authorization: Bearer 96dd0504c13d9abee65345ce24e917a30df3810059b5cf78e119a03c1c5bd02c"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 5778596cae512c591ffbd0d2392c30d9e1fdd0d9fb0cd9a313d435c5113f8d97
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
	-H "Authorization: Bearer 5778596cae512c591ffbd0d2392c30d9e1fdd0d9fb0cd9a313d435c5113f8d97"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/16/bookmark
Content-Type: application/json
Authorization: Bearer 27f92a1baaa0f9657fe11babbcc2fc8fa5fc590c01a307260f90d56d1727ffe7
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27f92a1baaa0f9657fe11babbcc2fc8fa5fc590c01a307260f90d56d1727ffe7"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/15/upvote
Content-Type: application/json
Authorization: Bearer 35743c590b03181ea64d20bc7cf17e180c290581ff631162ff4b080397a47d37
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
	-H "Authorization: Bearer 35743c590b03181ea64d20bc7cf17e180c290581ff631162ff4b080397a47d37"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/26/comments
Content-Type: application/json
Authorization: Bearer 46f50bf72bde2fcc340d1f771d553b28c7a0dea71df6710f276900a5f231e62a
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
    "id": 50,
    "author_id": 663,
    "reply_to_id": null,
    "created_at": "2016-11-08T11:40:31.158Z",
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
curl "api.goskive.com/v2/flashcards/26/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46f50bf72bde2fcc340d1f771d553b28c7a0dea71df6710f276900a5f231e62a"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/27/comments
Content-Type: application/json
Authorization: Bearer dae0d389267d7207cbd81d89c594f02f9d9012c1f9f221baa5fabf2d7aa3cd01
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
    "id": 51,
    "author_id": 666,
    "reply_to_id": null,
    "created_at": "2016-11-08T11:40:31.517Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 45,
      "user_id": 666,
      "feedbackable_id": 27,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:40:31.514Z",
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
curl "api.goskive.com/v2/flashcards/27/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dae0d389267d7207cbd81d89c594f02f9d9012c1f9f221baa5fabf2d7aa3cd01"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/30/comments
Content-Type: application/json
Authorization: Bearer 97772fa9b16c50d8ff302fc6c0a79e2d7ab0cfa89f9c7de3d50b40ee80bb03c2
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
      "id": 53,
      "author_id": 679,
      "reply_to_id": null,
      "created_at": "2016-11-08T11:40:32.262Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 678,
      "reply_to_id": null,
      "created_at": "2016-11-08T11:40:32.247Z",
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
curl "api.goskive.com/v2/flashcards/30/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97772fa9b16c50d8ff302fc6c0a79e2d7ab0cfa89f9c7de3d50b40ee80bb03c2"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/28/comments
Content-Type: application/json
Authorization: Bearer c7ade0ab4f31cb09bf80f7c14f259f8940751bcee53c80e187a954c9987110d4
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
curl "api.goskive.com/v2/flashcards/28/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7ade0ab4f31cb09bf80f7c14f259f8940751bcee53c80e187a954c9987110d4"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/16/feedbacks
Content-Type: application/json
Authorization: Bearer 8e034911c1d3173e02f6ffc4747c0b568bb43d4f0c2c78567d98343a242e0274
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
    "id": 43,
    "user_id": 391,
    "feedbackable_id": 16,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-08T11:40:05.516Z",
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
curl "api.goskive.com/v2/flashcards/16/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e034911c1d3173e02f6ffc4747c0b568bb43d4f0c2c78567d98343a242e0274"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/13/feedbacks
Content-Type: application/json
Authorization: Bearer 609a0e4f5995832f22a05f850771d1d6b8fbadd8ebd360a845cb624826f601ef
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
      "user_id": 381,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:40:04.947Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 382,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:40:04.958Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/13/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 609a0e4f5995832f22a05f850771d1d6b8fbadd8ebd360a845cb624826f601ef"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/56/votes
Content-Type: application/json
Authorization: Bearer 66bc5d6e522e1006bbb4be11bb5651443b1e5d46fd4660a073e465fe2c9496d6
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
      "id": 16,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 765
    },
    {
      "id": 15,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 764
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 56,
      "user_id": 763
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/56/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66bc5d6e522e1006bbb4be11bb5651443b1e5d46fd4660a073e465fe2c9496d6"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/46/republish
Content-Type: application/json
Authorization: Bearer f5b48b98efb4b743a4812cc8e3fcc3fa5fc292489b9d6c0c62cc3a4b3908e881
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
curl "api.goskive.com/v2/flashcards/46/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5b48b98efb4b743a4812cc8e3fcc3fa5fc292489b9d6c0c62cc3a4b3908e881"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/48/bookmark
Content-Type: application/json
Authorization: Bearer 00acea2e91b0e2f7d33e6e29503c00011de6833492102867dedd10e63c2a6e72
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/48/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00acea2e91b0e2f7d33e6e29503c00011de6833492102867dedd10e63c2a6e72"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/51
Content-Type: application/json
Authorization: Bearer 20095a6100eb529dae53c27882a3b48dbda07cea4ae872514c7b0b8db685720e
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20095a6100eb529dae53c27882a3b48dbda07cea4ae872514c7b0b8db685720e"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/54/downvote
Content-Type: application/json
Authorization: Bearer 780d253c243cb8e59af791260deb85f7cac750fbe6837e47bbadb18d05ddc611
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/54/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 780d253c243cb8e59af791260deb85f7cac750fbe6837e47bbadb18d05ddc611"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/52
Content-Type: application/json
Authorization: Bearer 1090a707efc724dc3ec3551c536fb85678cdf97ea69bcdd27ac07bdd04188f63
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
    "id": 52,
    "obfuscated_id": "_rmh4zxMC_8",
    "author_id": 748,
    "chapter_id": 132,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:35.917Z",
    "created_at": "2016-11-08T11:40:35.917Z",
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
curl "api.goskive.com/v2/flashcards/52" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1090a707efc724dc3ec3551c536fb85678cdf97ea69bcdd27ac07bdd04188f63"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/49/report
Content-Type: application/json
Authorization: Bearer 620c666feeb7625ea6cf76828d118dda1fef482bc44251d0b06c53cb600c7eb7
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 620c666feeb7625ea6cf76828d118dda1fef482bc44251d0b06c53cb600c7eb7"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50/bookmark
Content-Type: application/json
Authorization: Bearer 2565ccc7f012e4665b42befea2e27a13d8564ac8afa296a299988f87163f4db3
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2565ccc7f012e4665b42befea2e27a13d8564ac8afa296a299988f87163f4db3"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/53/upvote
Content-Type: application/json
Authorization: Bearer f882d5b1d957b58f4cf3c056bb82fcb8d6f71e446fb4429589c30ad5958ad3d4
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/53/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f882d5b1d957b58f4cf3c056bb82fcb8d6f71e446fb4429589c30ad5958ad3d4"
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
    "key": "cache/0ef79f9a41853354409ad9b07061cba7.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wOFQxMjo0MDo0NloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzBlZjc5ZjlhNDE4NTMzNTQ0MDlhZDliMDcwNjFjYmE3LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDhUMTE0MDQ2WiJ9XX0=",
    "x-amz-credential": "FAKE/20161108/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161108T114046Z",
    "x-amz-signature": "7e3e2ed9200d3590f72c64aea28a09d932bc388bd818c8847a20afc7c44f6a33"
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
Authorization: Bearer 335574cb9e25be4aa1199873c7e094c79d8cc6bab296b2b8a00eb8b72e6d5b16
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
	-H "Authorization: Bearer 335574cb9e25be4aa1199873c7e094c79d8cc6bab296b2b8a00eb8b72e6d5b16"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 6fe6c4f9fddbae81f9a9c3a096329ce30272b244e9863d878cf443bde0deffa2
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
	-H "Authorization: Bearer 6fe6c4f9fddbae81f9a9c3a096329ce30272b244e9863d878cf443bde0deffa2"
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
{"password":{"reset_password_token":"Hqc1kY3J2sPPbpy4YTxr","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 351,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-08T11:40:02.560Z",
  "updated_at": "2016-11-08T11:40:02.782Z",
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
  "audit_id": 4699
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"Hqc1kY3J2sPPbpy4YTxr","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/131/comments
Content-Type: application/json
Authorization: Bearer 8eb106d71084fe3fe7578575a484eafdacd59a63b7b90608ae4975f06b3fdf04
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
    "id": 60,
    "author_id": 926,
    "reply_to_id": null,
    "created_at": "2016-11-08T11:40:56.886Z",
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
curl "api.goskive.com/v2/questions/131/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8eb106d71084fe3fe7578575a484eafdacd59a63b7b90608ae4975f06b3fdf04"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/130/comments
Content-Type: application/json
Authorization: Bearer 7cf3d195aaa78144e74fe5eae97792c463f0fa7fb27c7dd5aaa4ae39947ecec4
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
    "id": 59,
    "author_id": 923,
    "reply_to_id": null,
    "created_at": "2016-11-08T11:40:56.440Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 923,
      "feedbackable_id": 130,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:40:56.437Z",
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
curl "api.goskive.com/v2/questions/130/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cf3d195aaa78144e74fe5eae97792c463f0fa7fb27c7dd5aaa4ae39947ecec4"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/127/comments
Content-Type: application/json
Authorization: Bearer 7f70cbc97f7ac36eced7c8ae7f9ea7018efce6dfe915e3f12be21401a1c13f2f
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
      "id": 58,
      "author_id": 916,
      "reply_to_id": null,
      "created_at": "2016-11-08T11:40:55.436Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 915,
      "reply_to_id": null,
      "created_at": "2016-11-08T11:40:55.420Z",
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
curl "api.goskive.com/v2/questions/127/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f70cbc97f7ac36eced7c8ae7f9ea7018efce6dfe915e3f12be21401a1c13f2f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/129/comments
Content-Type: application/json
Authorization: Bearer 32a31a7d7f5c27e915fc6924977c9160086fc59f7da690a8d526320dbce72ed4
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
curl "api.goskive.com/v2/questions/129/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32a31a7d7f5c27e915fc6924977c9160086fc59f7da690a8d526320dbce72ed4"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/12/feedbacks
Content-Type: application/json
Authorization: Bearer 2bd205df6c248ee0c05c9addd43582bc88f55ee53b2c43601328f16d50413356
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
    "user_id": 65,
    "feedbackable_id": 12,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-08T11:39:44.522Z",
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
curl "api.goskive.com/v2/questions/12/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bd205df6c248ee0c05c9addd43582bc88f55ee53b2c43601328f16d50413356"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/17/feedbacks
Content-Type: application/json
Authorization: Bearer 3f2f652f6b2b578d299963196e8c949c04ea7618eff7b5c6465f33e0c7911f5a
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
      "id": 8,
      "user_id": 94,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:39:46.385Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 93,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-08T11:39:46.374Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/17/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f2f652f6b2b578d299963196e8c949c04ea7618eff7b5c6465f33e0c7911f5a"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/92/votes
Content-Type: application/json
Authorization: Bearer 51e58a7849ccffe79bc614f0a20931c2d0e1c53a1e59ad0e5c229c2358727f3c
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 806
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 805
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 804
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/92/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51e58a7849ccffe79bc614f0a20931c2d0e1c53a1e59ad0e5c229c2358727f3c"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/62/republish
Content-Type: application/json
Authorization: Bearer 0617e8631b7374ea1938e3f45f2be1af0d013e63c6ecae2c0613ce11fd9c69b5
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
	-H "Authorization: Bearer 0617e8631b7374ea1938e3f45f2be1af0d013e63c6ecae2c0613ce11fd9c69b5"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/43/bookmark
Content-Type: application/json
Authorization: Bearer b0a0d7c5bedfb9d53cb94eae12c57d0e092c5672e5b8c0b59e2844cff392ceb5
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/43/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0a0d7c5bedfb9d53cb94eae12c57d0e092c5672e5b8c0b59e2844cff392ceb5"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/63
Content-Type: application/json
Authorization: Bearer 59616fa316d2f3fc7c537adaa8bc355c1772cb4dd4d139841842e61ae138b0af
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/63" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59616fa316d2f3fc7c537adaa8bc355c1772cb4dd4d139841842e61ae138b0af"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/42/downvote
Content-Type: application/json
Authorization: Bearer e00e6ef46d5f7d97e2d50d9e804687f0b2aca4ff29c0379743c6a054673e4fb3
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e00e6ef46d5f7d97e2d50d9e804687f0b2aca4ff29c0379743c6a054673e4fb3"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/64
Content-Type: application/json
Authorization: Bearer ef18063077c9a636f2e8e98aaee48cc4168355a9eb5fbd5ce0b5b3e165476cdc
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
    "id": 64,
    "obfuscated_id": "H-V851w7HZg",
    "author_id": 487,
    "chapter_id": 81,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:15.658Z",
    "created_at": "2016-11-08T11:40:15.537Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 128,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 129,
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
curl "api.goskive.com/v2/questions/64" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef18063077c9a636f2e8e98aaee48cc4168355a9eb5fbd5ce0b5b3e165476cdc"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/41/report
Content-Type: application/json
Authorization: Bearer d7056c4ea1e42508479b56348e4e0af1b143a8ba765ed9acd80d018a182a47ae
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/41/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7056c4ea1e42508479b56348e4e0af1b143a8ba765ed9acd80d018a182a47ae"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/65/bookmark
Content-Type: application/json
Authorization: Bearer 8a28cf361d762f22fe72853111702ba009c2908a311f6dc96b74d393f02231e2
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a28cf361d762f22fe72853111702ba009c2908a311f6dc96b74d393f02231e2"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/59
Content-Type: application/json
Authorization: Bearer efe8d0b58b5d4ea921859edbaeef49c5650a8fe73e00af483000864d4d48c232
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":59,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T11:40:13.227Z","updated_at":"2016-11-08T11:40:13.341Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":76,"author_id":472,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 59,
    "obfuscated_id": "fo0taK4dosk",
    "author_id": 472,
    "chapter_id": 76,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-08T11:40:13.449Z",
    "created_at": "2016-11-08T11:40:13.227Z",
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
    "question": "{\"id\"=>59, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-08T11:40:13.227Z\", \"updated_at\"=>\"2016-11-08T11:40:13.341Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>76, \"author_id\"=>472, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 117,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 118,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 119,
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
curl "api.goskive.com/v2/questions/59" -d '{"question":{"question":{"id":59,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-08T11:40:13.227Z","updated_at":"2016-11-08T11:40:13.341Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":76,"author_id":472,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer efe8d0b58b5d4ea921859edbaeef49c5650a8fe73e00af483000864d4d48c232"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/60/upvote
Content-Type: application/json
Authorization: Bearer 6b344505c9a787e33777570cff600a2b798bbeec560f1422fcf224de213e3332
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/60/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b344505c9a787e33777570cff600a2b798bbeec560f1422fcf224de213e3332"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 05dd48648769287cfbcd4fbeb1abccb339ea7747a571174cd533b10271339751
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
      "creator_id": 101,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 30,
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
      "updated_at": "2016-11-08T11:39:47.289Z",
      "shortname": "mit-pizza-201",
      "topic_id": 34,
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
	-H "Authorization: Bearer 05dd48648769287cfbcd4fbeb1abccb339ea7747a571174cd533b10271339751"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 5b78b3d70d4ea650ab781be68eee7718cc527a6f9e24131cbe25f1ce5d84e704
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
      "id": 33,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-33",
      "html_url": "https://goskive.com/university/uni-33",
      "slug": "uni-33",
      "name": "National School of Pizza",
      "short_name": "Uni 33",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/af4a59026331ce71aecbe5b7ff54137522b16fcc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/57d36010c7e6070facf87bca901b7198bfd678c1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T11:39:47.627Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-32",
      "html_url": "https://goskive.com/university/uni-32",
      "slug": "uni-32",
      "name": "National School of Pastry",
      "short_name": "Uni 32",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f3740963af3b785d81e56101e31332294478c35b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8b2eb16060f7c6a977153a523ce088cd8b6cb975.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T11:39:47.608Z",
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
	-H "Authorization: Bearer 5b78b3d70d4ea650ab781be68eee7718cc527a6f9e24131cbe25f1ce5d84e704"
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
      "id": 265,
      "name": "Proactive even-keeled internet solution",
      "name_translations": {
        "en": "Proactive even-keeled internet solution"
      },
      "discipline_id": 266
    },
    {
      "id": 266,
      "name": "Virtual zero tolerance emulation",
      "name_translations": {
        "en": "Virtual zero tolerance emulation"
      },
      "discipline_id": 267
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
GET /v2/topics/267
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
    "id": 267,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 268
  }
}
```



```shell
curl "api.goskive.com/v2/topics/267" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 7de9d199fd8711c448f845735e482c15edbe238c5ccce37aa86c208d97582651
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
      "id": 112,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-110",
      "html_url": "https://goskive.com/university/uni-110",
      "slug": "uni-110",
      "name": "University 101",
      "short_name": "Uni 110",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/226566b0e8f48a07eba2f7ffc319b71ab66e1e6f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b675d790d0cc028750a151165c1206d46cabb0bd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T11:40:04.154Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 113,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-111",
      "html_url": "https://goskive.com/university/uni-111",
      "slug": "uni-111",
      "name": "University 102",
      "short_name": "Uni 111",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0094eccb9bd9629a76a147d9a37af3a72de4f83e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/113ce34c1f4ce8c6241d9ab1a97426bd39d1712c.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T11:40:04.170Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-112",
      "html_url": "https://goskive.com/university/uni-112",
      "slug": "uni-112",
      "name": "University 103",
      "short_name": "Uni 112",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/226077c8a53a441f63f708cc445f0e8b8c0c0785.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2f9b3edea5422a0b21c56f310f6f46844af3f1b2.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-08T11:40:04.186Z",
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
	-H "Authorization: Bearer 7de9d199fd8711c448f845735e482c15edbe238c5ccce37aa86c208d97582651"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 346e6ae6ecb496bcb746f9a3c01aa190794400e8d76bf32e2d4cb286b8cbd681
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
    "id": 111,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/29fc8bca362837c836a5d6d8a1501019fb32da53.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/af2ae58961d5fa915fb5470017502a41936bf8a7.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-08T11:40:04.061Z",
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
	-H "Authorization: Bearer 346e6ae6ecb496bcb746f9a3c01aa190794400e8d76bf32e2d4cb286b8cbd681"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4c93c6a4a900d00735ccf20edcba29e6866685faabde1b34e45f8ff5fda440d8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":196,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 549,
    "id": 187,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 172,
    "additional_university_ids": [

    ],
    "discipline_id": 197,
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
    "chapters_updated_at": "2016-11-08T11:40:21.141Z",
    "updated_at": "2016-11-08T11:40:21.287Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 87,
        "updated_at": "2016-11-08T11:40:21.243Z",
        "course_id": 187,
        "author_id": 549,
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
        "id": 88,
        "updated_at": "2016-11-08T11:40:21.260Z",
        "course_id": 187,
        "author_id": 549,
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
        "id": 89,
        "updated_at": "2016-11-08T11:40:21.277Z",
        "course_id": 187,
        "author_id": 549,
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
    "topic_id": 196,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":196,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c93c6a4a900d00735ccf20edcba29e6866685faabde1b34e45f8ff5fda440d8"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 662a29d594a668a71f0b07d4ff39c286f961ee8a60be85cb4b0c92f5b0b1ce54
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":195,"published":false}}
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
    "creator_id": 548,
    "id": 186,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 171,
    "additional_university_ids": [

    ],
    "discipline_id": 196,
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
    "updated_at": "2016-11-08T11:40:21.068Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 195,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":195,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 662a29d594a668a71f0b07d4ff39c286f961ee8a60be85cb4b0c92f5b0b1ce54"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 47dfbd9add1049336ad10eaa53e925a42629d19d699fcc8dc2e0092524ccb71b
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
      "creator_id": 521,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-155",
      "html_url": "https://goskive.com/course/fu-course-155",
      "slug": "fu-course-155",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 173,
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
      "updated_at": "2016-11-08T11:40:18.516Z",
      "shortname": "fu-course-155",
      "topic_id": 172,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 521,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 174,
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
      "chapters_updated_at": "2016-11-08T11:40:18.375Z",
      "updated_at": "2016-11-08T11:40:18.809Z",
      "shortname": "fu-course-156",
      "topic_id": 173,
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
	-H "Authorization: Bearer 47dfbd9add1049336ad10eaa53e925a42629d19d699fcc8dc2e0092524ccb71b"
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
      "creator_id": 541,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-171",
      "html_url": "https://goskive.com/course/fu-course-171",
      "slug": "fu-course-171",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 189,
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
      "updated_at": "2016-11-08T11:40:20.247Z",
      "shortname": "fu-course-171",
      "topic_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 171",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 541,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 167,
      "additional_university_ids": [

      ],
      "discipline_id": 190,
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
      "chapters_updated_at": "2016-11-08T11:40:20.099Z",
      "updated_at": "2016-11-08T11:40:20.556Z",
      "shortname": "fu-course-172",
      "topic_id": 189,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 172",
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
Authorization: Bearer d5f1641d636075b18df3edb81e86038cd09c256f146f74dffd0a2478a73a3618
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
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-159",
      "html_url": "https://goskive.com/course/fu-course-159",
      "slug": "fu-course-159",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "discipline_id": 177,
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
      "updated_at": "2016-11-08T11:40:19.059Z",
      "shortname": "fu-course-159",
      "topic_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 159",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 527,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-160",
      "html_url": "https://goskive.com/course/fu-course-160",
      "slug": "fu-course-160",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "discipline_id": 178,
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
      "updated_at": "2016-11-08T11:40:19.101Z",
      "shortname": "fu-course-160",
      "topic_id": 177,
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
	-H "Authorization: Bearer d5f1641d636075b18df3edb81e86038cd09c256f146f74dffd0a2478a73a3618"
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
      "creator_id": 546,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-175",
      "html_url": "https://goskive.com/course/fu-course-175",
      "slug": "fu-course-175",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "discipline_id": 193,
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
      "updated_at": "2016-11-08T11:40:20.769Z",
      "shortname": "fu-course-175",
      "topic_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 546,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "discipline_id": 194,
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
      "updated_at": "2016-11-08T11:40:20.810Z",
      "shortname": "fu-course-176",
      "topic_id": 193,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
Authorization: Bearer ae338ec5802ff17af16a65c7a9289649ddbdfe6eca196aa35daa1f45a62c3c11
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
  "id": 567,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-08T11:40:22.455Z",
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
	-H "Authorization: Bearer ae338ec5802ff17af16a65c7a9289649ddbdfe6eca196aa35daa1f45a62c3c11"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/60
Content-Type: application/json
Authorization: Bearer cdc6f85a83e95ce18e7d2f656d8b72d20bd467c45b344e2c2985f07ae8950b8d
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
    "id": 60,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 21,
    "fields_of_study": [
      21,
      22
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-08T11:39:43.221Z",
    "updated_at": "2016-11-08T11:39:43.221Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/60" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdc6f85a83e95ce18e7d2f656d8b72d20bd467c45b344e2c2985f07ae8950b8d"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/58
Content-Type: application/json
Authorization: Bearer d9495e7ac5045199f60700b2d6c839626a42e16ce66ba80bdcf61117e77537f4
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
    "id": 58,
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
    "created_at": "2016-11-08T11:39:43.041Z",
    "updated_at": "2016-11-08T11:39:43.041Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/58" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9495e7ac5045199f60700b2d6c839626a42e16ce66ba80bdcf61117e77537f4"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/6
Content-Type: application/json
Authorization: Bearer aa4257a660d3d7a065c31008eac1caa1ae6fd24eaa9a801cd6a446dfe8b9dbb1
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa4257a660d3d7a065c31008eac1caa1ae6fd24eaa9a801cd6a446dfe8b9dbb1"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/7
Content-Type: application/json
Authorization: Bearer fd846f9b707c4af8db5d6583f3d30684c23e4b20083a58751d6c31b959f86037
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
    "id": 7,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 10,
    "user_id": 54
  }
}
```



```shell
curl "api.goskive.com/v2/votes/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd846f9b707c4af8db5d6583f3d30684c23e4b20083a58751d6c31b959f86037"
```
