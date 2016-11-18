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
Authorization: Basic YzMyMGNiNjQzZGJlZmE1NTQxNTY0NDYzMDA5OTlkNGFjZWNkYmZkMDhjNDI2
MjkyNTc4YjdjNjcyMWE2ZjAyMToyMGM5NDE5M2IxYzQ5MDIyOWVmMWNjMDIx
ZDFmOTI3OThmZTE3ODYzNWZhMTE1ZDc1ODljYjY5NDZlZTAyODdm

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
	-u c320cb643dbefa554156446300999d4acecdbfd08c426292578b7c6721a6f021:20c94193b1c490229ef1cc021d1f92798fe178635fa115d7589cb6946ee0287f
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c2046ec97a9d16cbe96c3c8558131d540d32d8677d29ea47a64a8051a04a0921","client_secret":"a6439919d9de465f61e477536ae26602cd6d732a12fd4230d46a9b09c56658ac"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c2046ec97a9d16cbe96c3c8558131d540d32d8677d29ea47a64a8051a04a0921","client_secret":"a6439919d9de465f61e477536ae26602cd6d732a12fd4230d46a9b09c56658ac"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic Y2JiZmE1ZTk3YzE3YzliYzRkZTc5MmI0MDM2YWI0NDg5OTYzZmVlZmZkY2Iy
MWQ1ODM0ZjY4ZWI1YzI4NjIyMTo5ZTA0MzVmYjNlYzVmMWI2N2M3YzJhMzlm
ZmFmYzIwOTg3NmM2NzZiYjc2ODc3NGFhYzcxODc2NjRhYzQ4MTEz

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
  "access_token": "f677879d8b70609343fc2c50202d53e9c14577ca39a7f613b2040422474dfe29",
  "token_type": "bearer",
  "created_at": 1479466608
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u cbbfa5e97c17c9bc4de792b4036ab4489963feeffdcb21d5834f68eb5c286221:9e0435fb3ec5f1b67c7c2a39ffafc209876c676bb768774aac7187664ac48113
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"4fe6cbd5c30457edb712bf7121259175c5121b86935b8f440ea41754574000cb","client_secret":"c6cb453a5fb48b87d9bb6f392c9b5ad67a9b0c0b5a79b9a73a341aac4caa9b66"}
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
  "access_token": "f6048c8f4d64a29e4530a2b746125c5b4a9ff0b4a9f84763daaf2d3b2fd04b7c",
  "token_type": "bearer",
  "created_at": 1479466608
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"4fe6cbd5c30457edb712bf7121259175c5121b86935b8f440ea41754574000cb","client_secret":"c6cb453a5fb48b87d9bb6f392c9b5ad67a9b0c0b5a79b9a73a341aac4caa9b66"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"5eba8a9a4dffb61580af86e9d17e008037b8d330e2d6eb54fb95571dd9638cd6","client_secret":"70e2084c376a0e77630205445a50d0c0ee2147d445c6e50770a45ecd63cdaaae"}
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
  "access_token": "92b344829208b9e8de66be48ac73b1f7521ab203965c2559814c9bb21bf0942d",
  "token_type": "bearer",
  "created_at": 1479466608
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5eba8a9a4dffb61580af86e9d17e008037b8d330e2d6eb54fb95571dd9638cd6","client_secret":"70e2084c376a0e77630205445a50d0c0ee2147d445c6e50770a45ecd63cdaaae"}' -X POST \
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
Authorization: Bearer 1c3a064e6df8f32aa4f2c26226e19d3de1d0e005942e2dc4ed76146ad5964d3d
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
	-H "Authorization: Bearer 1c3a064e6df8f32aa4f2c26226e19d3de1d0e005942e2dc4ed76146ad5964d3d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/131/flashcards
Content-Type: application/json
Authorization: Bearer 4387bf968421ed58bf8efd16adc2921852d68deefa4ece042667a665dd4ac324
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":131,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 71,
    "obfuscated_id": "--JhLc6KEBw",
    "author_id": 555,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:34.470Z",
    "created_at": "2016-11-18T10:56:34.470Z",
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
curl "api.goskive.com/v2/chapters/131/flashcards" -d '{"flashcard":{"chapter_id":131,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4387bf968421ed58bf8efd16adc2921852d68deefa4ece042667a665dd4ac324"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/133/flashcards
Content-Type: application/json
Authorization: Bearer 47ed6cab06f9d0e247e8a49c1a8430420927b0f6fd168ab3a17dafed916f654e
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 559,
      "chapter_id": 133,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:34.837Z",
      "created_at": "2016-11-18T10:56:34.837Z",
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 559,
      "chapter_id": 133,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:34.874Z",
      "created_at": "2016-11-18T10:56:34.874Z",
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
      "author_id": 559,
      "chapter_id": 133,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:34.912Z",
      "created_at": "2016-11-18T10:56:34.912Z",
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
curl "api.goskive.com/v2/chapters/133/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47ed6cab06f9d0e247e8a49c1a8430420927b0f6fd168ab3a17dafed916f654e"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/155/questions
Content-Type: application/json
Authorization: Bearer 3f9b9ef2e6c9d36fb6432af8579b660ec8f7a8b4a89875c5d0d6a68b47b503b2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":155,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 107,
    "obfuscated_id": "_2rgp7tgq8o",
    "author_id": 806,
    "chapter_id": 155,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:51.596Z",
    "created_at": "2016-11-18T10:56:51.596Z",
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
        "id": 214,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 215,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 216,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 217,
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
curl "api.goskive.com/v2/chapters/155/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":155,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f9b9ef2e6c9d36fb6432af8579b660ec8f7a8b4a89875c5d0d6a68b47b503b2"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/154/questions
Content-Type: application/json
Authorization: Bearer 7b359d1e3da2787b3416be0ccd9d0d7b4491ea1bd22e387b4921545aa6815c92
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":154,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 106,
    "obfuscated_id": "GEL902caNek",
    "author_id": 803,
    "chapter_id": 154,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:51.049Z",
    "created_at": "2016-11-18T10:56:51.049Z",
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
        "id": 212,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 213,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/154/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":154,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b359d1e3da2787b3416be0ccd9d0d7b4491ea1bd22e387b4921545aa6815c92"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/156/questions
Content-Type: application/json
Authorization: Bearer abd759e1681cf75f3d4a499bb3b6bb4c5bc8048ba73a186ee45bd85bb28a01c4
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":156,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 809,
    "chapter_id": 156,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:52.329Z",
    "created_at": "2016-11-18T10:56:52.329Z",
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
        "id": 218,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 219,
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
curl "api.goskive.com/v2/chapters/156/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":156,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abd759e1681cf75f3d4a499bb3b6bb4c5bc8048ba73a186ee45bd85bb28a01c4"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/157/questions
Content-Type: application/json
Authorization: Bearer 23dc86eb18cc5610add607c12969e00622b1cff341460914d3d5cd3a126ccc72
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":157,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 109,
    "obfuscated_id": "VSPyck5c2RY",
    "author_id": 812,
    "chapter_id": 157,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:52.866Z",
    "created_at": "2016-11-18T10:56:52.866Z",
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
        "id": 220,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 221,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 222,
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
curl "api.goskive.com/v2/chapters/157/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":157,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23dc86eb18cc5610add607c12969e00622b1cff341460914d3d5cd3a126ccc72"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/159/questions
Content-Type: application/json
Authorization: Bearer 575f644b08e81dc0c11cdfba3f626a63fe8181731bea6e5e6483f4b61a1a7619
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
      "id": 110,
      "obfuscated_id": "55JK4PuG2Hk",
      "author_id": 818,
      "chapter_id": 159,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:53.612Z",
      "created_at": "2016-11-18T10:56:53.494Z",
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
    },
    {
      "id": 111,
      "obfuscated_id": "G-D-sgMUtTw",
      "author_id": 819,
      "chapter_id": 159,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:53.805Z",
      "created_at": "2016-11-18T10:56:53.683Z",
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
          "id": 225,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 226,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 820,
      "chapter_id": 159,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:54.005Z",
      "created_at": "2016-11-18T10:56:53.880Z",
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
          "id": 227,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 228,
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
curl "api.goskive.com/v2/chapters/159/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 575f644b08e81dc0c11cdfba3f626a63fe8181731bea6e5e6483f4b61a1a7619"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/134
Content-Type: application/json
Authorization: Bearer 7d3aea8fd6d943682764cf149ec4204f9b5bb3c1d26b9cf2b3b50d49b47397a9
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
curl "api.goskive.com/v2/chapters/134" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d3aea8fd6d943682764cf149ec4204f9b5bb3c1d26b9cf2b3b50d49b47397a9"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/137
Content-Type: application/json
Authorization: Bearer 4ead356de3e50387032b917e6a0bd177cddd9e432993a56c05a028518e69092c
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
curl "api.goskive.com/v2/chapters/137" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ead356de3e50387032b917e6a0bd177cddd9e432993a56c05a028518e69092c"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/139
Content-Type: application/json
Authorization: Bearer ea5dcfa7760dcf902c915ff502a22f787820769477eda26a65b1b5ae949966c5
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
curl "api.goskive.com/v2/chapters/139" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea5dcfa7760dcf902c915ff502a22f787820769477eda26a65b1b5ae949966c5"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/135
Content-Type: application/json
Authorization: Bearer c4a068a2e23daac224baa490999bd2b3a2cf7943e4ab7310dcfb046551bc8c38
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/135" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4a068a2e23daac224baa490999bd2b3a2cf7943e4ab7310dcfb046551bc8c38"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/141
Content-Type: application/json
Authorization: Bearer 6a03fd296b3ce3c428a4fe1edac9bc7b738b710b2a96f0826403252981162471
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
    "id": 141,
    "updated_at": "2016-11-18T10:56:38.463Z",
    "course_id": 202,
    "author_id": 597,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-18T10:56:37.915Z",
    "questions_updated_at": "2016-11-18T10:56:37.915Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 601,
        "chapter_id": 141,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:38.445Z",
        "created_at": "2016-11-18T10:56:38.445Z",
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
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 599,
        "chapter_id": 141,
        "position": 86,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:38.337Z",
        "created_at": "2016-11-18T10:56:38.217Z",
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
            "id": 190,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 191,
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
curl "api.goskive.com/v2/chapters/141" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a03fd296b3ce3c428a4fe1edac9bc7b738b710b2a96f0826403252981162471"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/140
Content-Type: application/json
Authorization: Bearer 977c6f79d9f7b6ccee4d2aa5fa48e7947e38ced63f5a8777b63236fa38222eb2
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
    "id": 140,
    "updated_at": "2016-11-18T10:56:37.746Z",
    "course_id": 201,
    "author_id": 595,
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
curl "api.goskive.com/v2/chapters/140" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 977c6f79d9f7b6ccee4d2aa5fa48e7947e38ced63f5a8777b63236fa38222eb2"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/8/replies
Content-Type: application/json
Authorization: Bearer b1696ba144724e4b7934332f2a0dcc6e36dcfd4431504b393209cff798c90a4e
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
    "id": 9,
    "author_id": 616,
    "reply_to_id": 8,
    "created_at": "2016-11-18T10:56:39.707Z",
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
curl "api.goskive.com/v2/comments/8/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1696ba144724e4b7934332f2a0dcc6e36dcfd4431504b393209cff798c90a4e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/10/replies
Content-Type: application/json
Authorization: Bearer 4383c8a46fe628ebf9397434d4dcaf73a5b88a441a0a57eb217412767d59c947
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
curl "api.goskive.com/v2/comments/10/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4383c8a46fe628ebf9397434d4dcaf73a5b88a441a0a57eb217412767d59c947"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 7360f05f3324910a671a8cb3c12cf9faf6ccf32a4776194bb207a186f50ed6a7
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
curl "api.goskive.com/v2/comments/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7360f05f3324910a671a8cb3c12cf9faf6ccf32a4776194bb207a186f50ed6a7"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/51/republish
Content-Type: application/json
Authorization: Bearer e731c92f318a5554884234d0c1fb00405bb13bb73320f3fa3fa858179fca7396
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
curl "api.goskive.com/v2/comments/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e731c92f318a5554884234d0c1fb00405bb13bb73320f3fa3fa858179fca7396"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer 0c7d814bf7e3af09cc924c32a5432f5d15fd956831cde1ae3f64a84548ab0b32
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c7d814bf7e3af09cc924c32a5432f5d15fd956831cde1ae3f64a84548ab0b32"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/11/report
Content-Type: application/json
Authorization: Bearer 6d4f1658362eea1b0c8dd08f2f7d993839c257419a33e2c82798eea0814179ea
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d4f1658362eea1b0c8dd08f2f7d993839c257419a33e2c82798eea0814179ea"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/35
Content-Type: application/json
Authorization: Bearer a7e4c2bca3ef3b90a0faf32dc3bd4149539d4dab84ba371b0e6ee3199b65e402
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
    "id": 35,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-18T10:56:54.130Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/35" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7e4c2bca3ef3b90a0faf32dc3bd4149539d4dab84ba371b0e6ee3199b65e402"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 279855609d67149cb86f9e969f626a8287647c1c5320b400cc8d3c8a7d384784
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
      "id": 36,
      "name": "Fake Company Name 32",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a2f4b2b00a6e41aded703f9b480c1133be4aa18e.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T10:56:54.206Z"
    },
    {
      "id": 37,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T10:56:54.210Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-18T10:56:54.214Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 279855609d67149cb86f9e969f626a8287647c1c5320b400cc8d3c8a7d384784"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/3/company_profiles
Content-Type: application/json
Authorization: Bearer 75f404bcbc158dd6bf1971898ad698f944013d8732a263b9c82af9bb3965bcad
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
	-H "Authorization: Bearer 75f404bcbc158dd6bf1971898ad698f944013d8732a263b9c82af9bb3965bcad"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/1/company_profiles
Content-Type: application/json
Authorization: Bearer 26ce1edee6158014a01ab1caff7bd1c9c39d024c70b94bbbfbc3aa42560c508e
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
	-H "Authorization: Bearer 26ce1edee6158014a01ab1caff7bd1c9c39d024c70b94bbbfbc3aa42560c508e"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 3391f9299038c57ac7eabc9f309a6d09428473a55f3c27752bd7eb6ac1c7eb33
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
      "id": 7,
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
	-H "Authorization: Bearer 3391f9299038c57ac7eabc9f309a6d09428473a55f3c27752bd7eb6ac1c7eb33"
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
Authorization: Bearer c7c28ad134eb40a8593c3bd38aea7976d207d6af2d33130b3c912856fb087da9
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
	-H "Authorization: Bearer c7c28ad134eb40a8593c3bd38aea7976d207d6af2d33130b3c912856fb087da9"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8895e755175afdfbc646b21db849ee7bc2b0f9d8b03ce069f3dc744b65571017
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
    "id": 42,
    "updated_at": "2016-11-18T10:56:01.616Z",
    "course_id": 83,
    "author_id": 184,
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
	-H "Authorization: Bearer 8895e755175afdfbc646b21db849ee7bc2b0f9d8b03ce069f3dc744b65571017"
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
      "id": 48,
      "updated_at": "2016-11-18T10:56:02.645Z",
      "course_id": 89,
      "author_id": 199,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 42",
      "position": 1
    },
    {
      "id": 49,
      "updated_at": "2016-11-18T10:56:02.673Z",
      "course_id": 89,
      "author_id": 200,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 43",
      "position": 2
    },
    {
      "id": 50,
      "updated_at": "2016-11-18T10:56:02.977Z",
      "course_id": 89,
      "author_id": 201,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-18T10:56:02.559Z",
      "questions_updated_at": "2016-11-18T10:56:02.559Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 44",
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
Authorization: Bearer dddff2aa15726b1201d8b9ff4d938606d59d8e566453c87620af0710f0f60dc7
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
      "id": 54,
      "updated_at": "2016-11-18T10:56:03.381Z",
      "course_id": 92,
      "author_id": 210,
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
      "id": 55,
      "updated_at": "2016-11-18T10:56:03.408Z",
      "course_id": 92,
      "author_id": 211,
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
      "id": 56,
      "updated_at": "2016-11-18T10:56:03.701Z",
      "course_id": 92,
      "author_id": 212,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-18T10:56:03.299Z",
      "questions_updated_at": "2016-11-18T10:56:03.299Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 50",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dddff2aa15726b1201d8b9ff4d938606d59d8e566453c87620af0710f0f60dc7"
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
      "id": 51,
      "updated_at": "2016-11-18T10:56:03.194Z",
      "course_id": 91,
      "author_id": 206,
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
      "id": 52,
      "updated_at": "2016-11-18T10:56:03.220Z",
      "course_id": 91,
      "author_id": 207,
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
      "id": 53,
      "updated_at": "2016-11-18T10:56:03.247Z",
      "course_id": 91,
      "author_id": 208,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
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
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 91c37664c1de2b7620ec7a1f27d2390b85d5efd98673d29d06a8f3a67ae9fb36
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
      "id": 57,
      "updated_at": "2016-11-18T10:56:03.867Z",
      "course_id": 93,
      "author_id": 217,
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
      "id": 58,
      "updated_at": "2016-11-18T10:56:03.892Z",
      "course_id": 93,
      "author_id": 218,
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
      "id": 59,
      "updated_at": "2016-11-18T10:56:03.916Z",
      "course_id": 93,
      "author_id": 219,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 53",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91c37664c1de2b7620ec7a1f27d2390b85d5efd98673d29d06a8f3a67ae9fb36"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 252e1ff49414ea0937c3146c0e671431b460cf8074cbb20c12a83b93265b5de2
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
    "course_id": 182,
    "user_id": 537,
    "updated_at": "2016-11-18T10:56:31.932Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 252e1ff49414ea0937c3146c0e671431b460cf8074cbb20c12a83b93265b5de2"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer f35bc672d5994c584562080787300b19a4ed537400c2dab7d23733fab5fb185d
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
      "course_id": 178,
      "user_id": 525,
      "updated_at": "2016-11-18T10:56:31.318Z"
    },
    {
      "id": 2,
      "course_id": 178,
      "user_id": 526,
      "updated_at": "2016-11-18T10:56:31.334Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f35bc672d5994c584562080787300b19a4ed537400c2dab7d23733fab5fb185d"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/192/files
Content-Type: application/json
Authorization: Bearer 6d94ecda3edc40b7201c57c52b3b2d508511cbb01be53e2ebd1603db4ade0cc3
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
      "id": 7,
      "uploader": {
        "id": 568,
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
        "created_at": "2016-11-18T10:56:35.646Z",
        "updated_at": "2016-11-18T10:56:35.646Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T10:56:35.657Z",
      "updated_at": "2016-11-18T10:56:35.657Z",
      "course_id": 192,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 8,
      "uploader": {
        "id": 569,
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
        "created_at": "2016-11-18T10:56:35.665Z",
        "updated_at": "2016-11-18T10:56:35.665Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T10:56:35.676Z",
      "updated_at": "2016-11-18T10:56:35.676Z",
      "course_id": 192,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 570,
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
        "created_at": "2016-11-18T10:56:35.683Z",
        "updated_at": "2016-11-18T10:56:35.683Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-18T10:56:35.693Z",
      "updated_at": "2016-11-18T10:56:35.693Z",
      "course_id": 192,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/192/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d94ecda3edc40b7201c57c52b3b2d508511cbb01be53e2ebd1603db4ade0cc3"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/191/files
Content-Type: application/json
Authorization: Bearer 31073c0df642e6186d808dde602a1ae14194b16597384ba86b10c509c72f4e14
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
      "created_at": "2016-11-18T10:56:35.423Z",
      "updated_at": "2016-11-18T10:56:35.423Z"
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
    "created_at": "2016-11-18T10:56:35.500Z",
    "updated_at": "2016-11-18T10:56:35.500Z",
    "course_id": 191,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/191/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31073c0df642e6186d808dde602a1ae14194b16597384ba86b10c509c72f4e14"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/194/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer ac3253be018a90e48fd12d19019a5d8dcfe0bbdd3be55ca037354d12b7bac676
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
    "key": "cache/a76dd60afbc0767f94700ab3d58b8df4.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xOFQxMTo1NjozNVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2E3NmRkNjBhZmJjMDc2N2Y5NDcwMGFiM2Q1OGI4ZGY0LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMTgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTE4VDEwNTYzNVoifV19",
    "x-amz-credential": "FAKE/20161118/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161118T105635Z",
    "x-amz-signature": "ba839801353c0ae77ee6bd39a1faa80b2dfe3dcfbfc36bf934047003fa841dd9"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/194/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac3253be018a90e48fd12d19019a5d8dcfe0bbdd3be55ca037354d12b7bac676"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 6bf13779c77fd325fb3f614f3a104a3267ae4b1852ae7d25f4c2b4de4cb12993
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
	-H "Authorization: Bearer 6bf13779c77fd325fb3f614f3a104a3267ae4b1852ae7d25f4c2b4de4cb12993"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bf385a17ae272eb969e5525212d1fb8773888e43c513d8be26072df0b884dd79
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
	-H "Authorization: Bearer bf385a17ae272eb969e5525212d1fb8773888e43c513d8be26072df0b884dd79"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6d8f4bc6753fbcb8ad8c3d912018c8ccda5e2f569c83467dbc138a034ef4c318
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
	-H "Authorization: Bearer 6d8f4bc6753fbcb8ad8c3d912018c8ccda5e2f569c83467dbc138a034ef4c318"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 72c9893c2869c95f116b7047e1df96c8b060ffc0e70a352c9c2724781bbe5ac4
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
	-H "Authorization: Bearer 72c9893c2869c95f116b7047e1df96c8b060ffc0e70a352c9c2724781bbe5ac4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ea7b53489fefdcc3cfe4c63c0846c9db7dde9ba74780941052fa123d568f6978
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
	-H "Authorization: Bearer ea7b53489fefdcc3cfe4c63c0846c9db7dde9ba74780941052fa123d568f6978"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer a3cea7934be26f0f9e93d6a07d4d0cf3099c59204d4b79c9f52399fe69b411c8
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
    "creator_id": 432,
    "id": 152,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 135,
    "additional_university_ids": [

    ],
    "discipline_id": 158,
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
    "chapters_updated_at": "2016-11-18T10:56:20.841Z",
    "updated_at": "2016-11-18T10:56:22.266Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 433,
        "chapter_id": 111,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:22.063Z",
        "created_at": "2016-11-18T10:56:22.063Z",
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
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 433,
        "chapter_id": 112,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:22.133Z",
        "created_at": "2016-11-18T10:56:22.133Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 433,
        "chapter_id": 111,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:22.102Z",
        "created_at": "2016-11-18T10:56:22.102Z",
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
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 433,
        "chapter_id": 112,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:22.171Z",
        "created_at": "2016-11-18T10:56:22.171Z",
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
        "id": 66,
        "obfuscated_id": "H7dODBospvw",
        "author_id": 433,
        "chapter_id": 111,
        "position": 57,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:21.048Z",
        "created_at": "2016-11-18T10:56:20.934Z",
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
          }
        ]
      },
      {
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 433,
        "chapter_id": 111,
        "position": 58,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:21.222Z",
        "created_at": "2016-11-18T10:56:21.111Z",
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
            "id": 134,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 135,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 433,
        "chapter_id": 112,
        "position": 59,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:21.430Z",
        "created_at": "2016-11-18T10:56:21.309Z",
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
            "id": 136,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 137,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 433,
        "chapter_id": 112,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:21.610Z",
        "created_at": "2016-11-18T10:56:21.496Z",
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
            "id": 138,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 139,
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
        "id": 111,
        "updated_at": "2016-11-18T10:56:22.220Z",
        "course_id": 152,
        "author_id": 432,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T10:56:20.841Z",
        "questions_updated_at": "2016-11-18T10:56:20.841Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 105",
        "position": 1
      },
      {
        "id": 112,
        "updated_at": "2016-11-18T10:56:22.258Z",
        "course_id": 152,
        "author_id": 432,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T10:56:20.841Z",
        "questions_updated_at": "2016-11-18T10:56:20.841Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 106",
        "position": 2
      }
    ],
    "topic_id": 157,
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
	-H "Authorization: Bearer a3cea7934be26f0f9e93d6a07d4d0cf3099c59204d4b79c9f52399fe69b411c8"
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
    "creator_id": 444,
    "id": 154,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 137,
    "additional_university_ids": [

    ],
    "discipline_id": 160,
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
    "chapters_updated_at": "2016-11-18T10:56:23.942Z",
    "updated_at": "2016-11-18T10:56:25.396Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 444,
        "chapter_id": 115,
        "position": 69,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:24.151Z",
        "created_at": "2016-11-18T10:56:24.035Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 444,
        "chapter_id": 116,
        "position": 71,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:24.531Z",
        "created_at": "2016-11-18T10:56:24.407Z",
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
            "id": 160,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 161,
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
        "id": 115,
        "updated_at": "2016-11-18T10:56:25.348Z",
        "course_id": 154,
        "author_id": 444,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T10:56:23.942Z",
        "questions_updated_at": "2016-11-18T10:56:23.942Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 109",
        "position": 1
      },
      {
        "id": 116,
        "updated_at": "2016-11-18T10:56:25.388Z",
        "course_id": 154,
        "author_id": 444,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-18T10:56:23.942Z",
        "questions_updated_at": "2016-11-18T10:56:23.942Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 110",
        "position": 2
      }
    ],
    "topic_id": 159,
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
PUT /v2/courses/151/pin
Content-Type: application/json
Authorization: Bearer 85a220714cb5a2d096c00fab963885cc19bd7ac4799e0a99221ef016da046f58
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/151/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85a220714cb5a2d096c00fab963885cc19bd7ac4799e0a99221ef016da046f58"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/156/pin
Content-Type: application/json
Authorization: Bearer 607ade800d17e0d17b9fcabf7265c3cca08d0009f7b47a94fd235e385e0dedc0
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/156/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 607ade800d17e0d17b9fcabf7265c3cca08d0009f7b47a94fd235e385e0dedc0"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ceee28bdd344673130ce4dcf2637e30cd3d00a1afcd42cc5df26e8e4f58c85f8
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
    "creator_id": 461,
    "id": 159,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 142,
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
    "updated_at": "2016-11-18T10:56:27.498Z",
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
	-H "Authorization: Bearer ceee28bdd344673130ce4dcf2637e30cd3d00a1afcd42cc5df26e8e4f58c85f8"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 688d477e883c8d5a8f52277fc6aa5165378fa469e70aac37d7789d66077b1952
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
    "id": 970,
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
    "created_at": "2016-11-18T10:57:04.814Z",
    "updated_at": "2016-11-18T10:57:04.814Z",
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
	-H "Authorization: Bearer 688d477e883c8d5a8f52277fc6aa5165378fa469e70aac37d7789d66077b1952"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c6fbbdda9c532ec35de2608a50d878eda828288c2eec76991b97ef4e909566d8
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[319]}
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
    "id": 965,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      319
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T10:57:04.077Z",
    "updated_at": "2016-11-18T10:57:04.127Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[319]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6fbbdda9c532ec35de2608a50d878eda828288c2eec76991b97ef4e909566d8"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 218481dfb24cde778e31b35f38a8801ddaaee7232c0caff0299644fcc775d445
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
    "id": 966,
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
    "created_at": "2016-11-18T10:57:04.157Z",
    "updated_at": "2016-11-18T10:57:04.157Z",
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
	-H "Authorization: Bearer 218481dfb24cde778e31b35f38a8801ddaaee7232c0caff0299644fcc775d445"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 28d9d6a181ddb1fa73eb5477917142ae2e4c370e006590e518468003ce060a1b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[322]}
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
    "id": 968,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      322
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T10:57:04.328Z",
    "updated_at": "2016-11-18T10:57:04.328Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[322]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28d9d6a181ddb1fa73eb5477917142ae2e4c370e006590e518468003ce060a1b"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer d3f568c30570117b0337b9f5bb4e750db0dd9879f0ca2c31f97e72cf210e1f30
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

323
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
    "id": 969,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/ba33a9e11eed3f08e2dce3608fae47e39d895103.jpg",
    "university_id": null,
    "fields_of_study": [
      323
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-18T10:57:04.400Z",
    "updated_at": "2016-11-18T10:57:04.784Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/745ad642d5b151d52f5c9afbc1bf1dcb2b805b32.jpg",
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

323
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer d3f568c30570117b0337b9f5bb4e750db0dd9879f0ca2c31f97e72cf210e1f30"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 2b058f311aef5c0ddb6cd151777bad8ca047ddc33e1285173af085b97a16bbc5
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
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 65,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b058f311aef5c0ddb6cd151777bad8ca047ddc33e1285173af085b97a16bbc5"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer e696bf6d968a01f5bdd9b7a80c7e510f774e076791e7b1da5cd4c8eeb9321da5
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
      "company_id": 8,
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
      "id": 3,
      "title": "Campaign 3",
      "company_id": 9,
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
	-H "Authorization: Bearer e696bf6d968a01f5bdd9b7a80c7e510f774e076791e7b1da5cd4c8eeb9321da5"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 4b597ea8242f69065d2f48cd7467028227992673426213e3b8e0bb260370e40e
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
      "company_id": 4,
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
	-H "Authorization: Bearer 4b597ea8242f69065d2f48cd7467028227992673426213e3b8e0bb260370e40e"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 216dd57973e861581888ab630db3b58d68e8d80808f5780ece9de12da6e92aee
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
      "creator_id": 174,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-74",
      "html_url": "https://goskive.com/course/mit-course-74",
      "slug": "mit-course-74",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "discipline_id": 78,
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
      "updated_at": "2016-11-18T10:56:00.796Z",
      "shortname": "mit-course-74",
      "topic_id": 78,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 74",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 175,
      "id": 79,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-75",
      "html_url": "https://goskive.com/course/mit-course-75",
      "slug": "mit-course-75",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "discipline_id": 79,
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
      "updated_at": "2016-11-18T10:56:00.878Z",
      "shortname": "mit-course-75",
      "topic_id": 79,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 75",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 216dd57973e861581888ab630db3b58d68e8d80808f5780ece9de12da6e92aee"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer fa43dcd16ffacf7dc2c7234f2940c333597de98b90f4d270448bbb3405d76634
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
        "created_at": "2016-11-18T10:56:01.153Z",
        "updated_at": "2016-11-18T10:56:01.153Z",
        "file_url": "memory://a38a222e3c581c7166e3506f4ef88a04.pdf",
        "course_id": 80,
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
        "created_at": "2016-11-18T10:56:01.233Z",
        "updated_at": "2016-11-18T10:56:01.233Z",
        "file_url": "memory://2d448669ba4998e2f47ba3cf21c84d3d.pdf",
        "course_id": 81,
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
        "created_at": "2016-11-18T10:56:01.342Z",
        "updated_at": "2016-11-18T10:56:01.342Z",
        "file_url": "memory://30cda254410872d4da2eae9782c5eade.pdf",
        "course_id": 82,
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
	-H "Authorization: Bearer fa43dcd16ffacf7dc2c7234f2940c333597de98b90f4d270448bbb3405d76634"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 2b68001905440bc853ba2fe9d40cc8524db22b16443cc1719284dd82d288bb73
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
      "company_id": 17,
      "company": {
        "id": 17,
        "name": "Fake Company Name 14",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T10:56:35.247Z"
      },
      "created_at": "2016-11-18T10:56:35.250Z",
      "updated_at": "2016-11-18T10:56:35.250Z",
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
      "company_id": 18,
      "company": {
        "id": 18,
        "name": "Fake Company Name 15",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T10:56:35.259Z"
      },
      "created_at": "2016-11-18T10:56:35.262Z",
      "updated_at": "2016-11-18T10:56:35.262Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b68001905440bc853ba2fe9d40cc8524db22b16443cc1719284dd82d288bb73"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 71d0e8a7ef77e87201ce612af3e273e2fdffba75b2526972588f085a74eb440d
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
      "company_id": 13,
      "company": {
        "id": 13,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T10:56:35.037Z"
      },
      "created_at": "2016-11-18T10:56:35.042Z",
      "updated_at": "2016-11-18T10:56:35.042Z",
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 11",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-18T10:56:35.057Z"
      },
      "created_at": "2016-11-18T10:56:35.060Z",
      "updated_at": "2016-11-18T10:56:35.060Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71d0e8a7ef77e87201ce612af3e273e2fdffba75b2526972588f085a74eb440d"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 0f79c5e5e370b118fbb5272fe0998e8c10de933011d4af20ae3bdf1ca75d47e6
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
      "created_at": "2016-11-18T10:55:49.218Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 1,
      "updated_at": "2016-11-18T10:55:49.323Z",
      "author_id": "62",
      "thread_subject_id": "44",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 3,
      "created_at": "2016-11-18T10:55:49.312Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-11-18T10:55:49.328Z",
      "author_id": "65",
      "thread_subject_id": "45",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-11-18T10:55:49.714Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-11-18T10:55:49.714Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-11-18T10:55:50.091Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 6,
      "updated_at": "2016-11-18T10:55:50.091Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 6,
      "created_at": "2016-11-18T10:55:50.466Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-11-18T10:55:50.466Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 7,
      "created_at": "2016-11-18T10:55:50.757Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 11,
      "updated_at": "2016-11-18T10:55:50.757Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-11-18T10:55:51.061Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 12,
      "updated_at": "2016-11-18T10:55:51.061Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-11-18T10:55:51.353Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 13,
      "updated_at": "2016-11-18T10:55:51.353Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f79c5e5e370b118fbb5272fe0998e8c10de933011d4af20ae3bdf1ca75d47e6"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/10
Content-Type: application/json
Authorization: Bearer 881ee132c53f628a1e79faf2939ea0e3f407240e6e6384640141b8583300075f
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-18T10:45:51.000Z"}}
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
    "id": 10,
    "created_at": "2016-11-18T10:55:51.479Z",
    "read_at": "2016-11-18T10:45:51.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 3,
    "updated_at": "2016-11-18T10:55:51.516Z",
    "author_id": "90",
    "thread_subject_id": "52",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/10" -d '{"notification":{"read_at":"2016-11-18T10:45:51.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 881ee132c53f628a1e79faf2939ea0e3f407240e6e6384640141b8583300075f"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 01a56abe391fa47a7db7c457f875e9962cf583f5fd35c67129d4602336108d13
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
      "course_id": 136,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-18T10:56:14.851Z",
      "course_published": true,
      "updated_at": "2016-11-18T10:56:14.843Z"
    },
    {
      "id": 5,
      "course_id": 137,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-18T10:56:14.930Z",
      "course_published": true,
      "updated_at": "2016-11-18T10:56:14.922Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01a56abe391fa47a7db7c457f875e9962cf583f5fd35c67129d4602336108d13"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer dddaa88ef546bfc083e1d4cd95cf4f47fdfa9455cf3be6e298c458c65b69a2f5
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
    "id": 7,
    "course_id": 140,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-18T10:56:15.290Z",
    "course_published": true,
    "updated_at": "2016-11-18T10:56:15.282Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dddaa88ef546bfc083e1d4cd95cf4f47fdfa9455cf3be6e298c458c65b69a2f5"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 675303ce599820aff182d325c68aa97ad34dd252756dd9b923779bcb5314aad7
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
    "course_id": 135,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-18T10:56:14.706Z",
    "course_published": true,
    "updated_at": "2016-11-18T10:56:14.695Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 675303ce599820aff182d325c68aa97ad34dd252756dd9b923779bcb5314aad7"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer bd7855819af80f658a0613c7519e46ba0de7e912eb4cc177337ee2c38a2a9864
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
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 42,
      "user_id": 237
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 43,
      "user_id": 237
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 44,
      "user_id": 237
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 45,
      "user_id": 237
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd7855819af80f658a0613c7519e46ba0de7e912eb4cc177337ee2c38a2a9864"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/147
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
    "id": 147,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 145,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 147
      },
      {
        "id": 146,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 147
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/147" -X GET \
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
      "id": 145,
      "name": "Devolved eco-centric matrix",
      "name_translations": {
        "en": "Devolved eco-centric matrix"
      }
    },
    {
      "id": 146,
      "name": "User-friendly systemic open system",
      "name_translations": {
        "en": "User-friendly systemic open system"
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
PATCH /v2/feedbacks/18/close
Content-Type: application/json
Authorization: Bearer 21f8a0f867a32f10bafb8fed5689d3ec8b531a91c5072b743e89bf2c8b22bc8a
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
    "id": 18,
    "user_id": 828,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-18T10:56:54.452Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/18/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21f8a0f867a32f10bafb8fed5689d3ec8b531a91c5072b743e89bf2c8b22bc8a"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/fix
Content-Type: application/json
Authorization: Bearer 3c33c346edb6d6b05e5dba3bcce5788a0d3a3289c73ca17e42fbc373ad02ebc3
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
    "user_id": 843,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-18T10:56:55.314Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/21/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c33c346edb6d6b05e5dba3bcce5788a0d3a3289c73ca17e42fbc373ad02ebc3"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/25
Content-Type: application/json
Authorization: Bearer 530a3a65de11299dc260a8683a0078b020f4e4816e978708625cae06f0080a28
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
    "user_id": 863,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T10:56:56.419Z",
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
	-H "Authorization: Bearer 530a3a65de11299dc260a8683a0078b020f4e4816e978708625cae06f0080a28"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/close
Content-Type: application/json
Authorization: Bearer 4fde159e2b44262814a5b4d91c62b8a3e2906b949fa295d46e455c62fa7918df
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
curl "api.goskive.com/v2/feedbacks/20/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fde159e2b44262814a5b4d91c62b8a3e2906b949fa295d46e455c62fa7918df"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer e63185831a0c3ded2d7ad9f108d189c66c8893f61b9dbbbb22c9dc48b6082f9a
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
	-H "Authorization: Bearer e63185831a0c3ded2d7ad9f108d189c66c8893f61b9dbbbb22c9dc48b6082f9a"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer e5e993c0a1052a3b4ba18f3f85094a9d0690291f3603d6d10611a5abd750a336
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
	-H "Authorization: Bearer e5e993c0a1052a3b4ba18f3f85094a9d0690291f3603d6d10611a5abd750a336"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/26
Content-Type: application/json
Authorization: Bearer 6575b17b6ae1188182c3c1f44b26481f3dcc0c7be57b7865aea6cd2ed089843c
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
    "user_id": 868,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T10:56:56.690Z",
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
	-H "Authorization: Bearer 6575b17b6ae1188182c3c1f44b26481f3dcc0c7be57b7865aea6cd2ed089843c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer 33ea977b8de8d7c438403a0338ea7a08d45ad68ae239c63454014acd57f2e848
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
	-H "Authorization: Bearer 33ea977b8de8d7c438403a0338ea7a08d45ad68ae239c63454014acd57f2e848"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer c3f09b20f21af950a58e9566b8eefd3ce3cb990e16204c55f57c0076992e561e
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3f09b20f21af950a58e9566b8eefd3ce3cb990e16204c55f57c0076992e561e"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer 4970a897b799318896bbf3ebd3eb372c8ca667ec922b1873a8417f7adc585a22
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
	-H "Authorization: Bearer 4970a897b799318896bbf3ebd3eb372c8ca667ec922b1873a8417f7adc585a22"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer 8762581d8eff8e1101931a5770bb76ab6f43bd449a7cf3fb2d15461f3ee7cdc2
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/a85b5803534080ded7eb2c98112d6559.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161118%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161118T105646Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=33dd9f02cb1daef493da191c0310471c25706be825dcb5a330570ec13c0bb9bd",
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
	-H "Authorization: Bearer 8762581d8eff8e1101931a5770bb76ab6f43bd449a7cf3fb2d15461f3ee7cdc2"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer e84fd210d8910b0bc2a61f64a1957b017484d8845a4f3bfadc7b7bae670652c0
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/6dea50b4ed7a41fa71b8128ff563d7c0.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161118%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161118T105646Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=30cb937f7b8516df53469bf159fb239b0fcab5fa1aea42b72deba89dd8507c97",
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
	-H "Authorization: Bearer e84fd210d8910b0bc2a61f64a1957b017484d8845a4f3bfadc7b7bae670652c0"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/22/metadata
Content-Type: application/json
Authorization: Bearer 47840ef4089e740c467fc0abeedb1b1605ea040e6aa9861e3edb628fb070ff7e
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
    "id": 22,
    "uploader": {
      "id": 769,
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
      "created_at": "2016-11-18T10:56:47.832Z",
      "updated_at": "2016-11-18T10:56:47.832Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-18T10:56:47.906Z",
    "updated_at": "2016-11-18T10:56:47.906Z",
    "course_id": 267,
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
curl "api.goskive.com/v2/files/22/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47840ef4089e740c467fc0abeedb1b1605ea040e6aa9861e3edb628fb070ff7e"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/5/matched_courses?required_cu_count=2
Authorization: Bearer 77bc08718dcafcf13568fb822b300baebc71b255b120c3d3e9633a168c4ab63f
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
      "creator_id": 407,
      "id": 146,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 129,
      "additional_university_ids": [

      ],
      "discipline_id": 152,
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
      "chapters_updated_at": "2016-11-18T10:56:16.911Z",
      "updated_at": "2016-11-18T10:56:19.004Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 151,
      "language_code": "en",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 412,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-476cb8f6-5f60-48d5-bf53-95db816c5848",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-476cb8f6-5f60-48d5-bf53-95db816c5848",
      "slug": "mit-the-great-british-bake-off-476cb8f6-5f60-48d5-bf53-95db816c5848",
      "university_id": 130,
      "additional_university_ids": [

      ],
      "discipline_id": 153,
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
      "chapters_updated_at": "2016-11-18T10:56:16.911Z",
      "updated_at": "2016-11-18T10:56:19.559Z",
      "shortname": "mit-the-great-british-bake-off-476cb8f6-5f60-48d5-bf53-95db816c5848",
      "topic_id": 152,
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
curl "api.goskive.com/v2/files/5/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 77bc08718dcafcf13568fb822b300baebc71b255b120c3d3e9633a168c4ab63f"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/13/download
Content-Type: application/json
Authorization: Bearer 549dc19e47d7156af7a8a66cdfb45d67afe961fc76e8547e68e785317faf3ccf
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
	-H "Authorization: Bearer 549dc19e47d7156af7a8a66cdfb45d67afe961fc76e8547e68e785317faf3ccf"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/16/report
Content-Type: application/json
Authorization: Bearer 8abb1d93157710d6286a612879faf90f4b06f4e0f8087ca18da6d7b03f751db9
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8abb1d93157710d6286a612879faf90f4b06f4e0f8087ca18da6d7b03f751db9"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer 1a8243d92ccb02fba6182fa655766107fbf74fe80ae0968f8fb872185d7126f0
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a8243d92ccb02fba6182fa655766107fbf74fe80ae0968f8fb872185d7126f0"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/15/upvote
Content-Type: application/json
Authorization: Bearer 0f512f8c7dea61244bb90c5e25a0d587b05fc4a3076033e5e9db19522dff31b4
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
	-H "Authorization: Bearer 0f512f8c7dea61244bb90c5e25a0d587b05fc4a3076033e5e9db19522dff31b4"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/91/comments
Content-Type: application/json
Authorization: Bearer 9c64e0c24b6e0c9d88ea6f9d745888a6ff1516cd11b191a1f4c7767b02a719f9
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
    "author_id": 971,
    "reply_to_id": null,
    "created_at": "2016-11-18T10:57:05.018Z",
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
curl "api.goskive.com/v2/flashcards/91/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c64e0c24b6e0c9d88ea6f9d745888a6ff1516cd11b191a1f4c7767b02a719f9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/93/comments
Content-Type: application/json
Authorization: Bearer e7802fc0f3c0ec7462b53fa2c773be688957f876e1e40ec6aace3b1cc6461fce
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
    "id": 58,
    "author_id": 977,
    "reply_to_id": null,
    "created_at": "2016-11-18T10:57:05.483Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 977,
      "feedbackable_id": 93,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:57:05.481Z",
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
curl "api.goskive.com/v2/flashcards/93/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7802fc0f3c0ec7462b53fa2c773be688957f876e1e40ec6aace3b1cc6461fce"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/95/comments
Content-Type: application/json
Authorization: Bearer 0b2c23d0dfa9bd336bbf60576be1380e20e7118093379e3190f48eade56a53f1
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
      "id": 60,
      "author_id": 987,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:57:05.977Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 986,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:57:05.962Z",
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
curl "api.goskive.com/v2/flashcards/95/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b2c23d0dfa9bd336bbf60576be1380e20e7118093379e3190f48eade56a53f1"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/92/comments
Content-Type: application/json
Authorization: Bearer a1199236188a3361be98b01df6fd6068e1bb6dc4880e2d9603347fcc3ea3ea47
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
curl "api.goskive.com/v2/flashcards/92/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1199236188a3361be98b01df6fd6068e1bb6dc4880e2d9603347fcc3ea3ea47"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/63/feedbacks
Content-Type: application/json
Authorization: Bearer 9e79c65ec49988abda09ec508596f64a5237bc017e15a863e52b29d95984d36b
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
    "user_id": 484,
    "feedbackable_id": 63,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-18T10:56:29.442Z",
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
	-H "Authorization: Bearer 9e79c65ec49988abda09ec508596f64a5237bc017e15a863e52b29d95984d36b"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/69/feedbacks
Content-Type: application/json
Authorization: Bearer cbd02a4e5d82f65d2f6b9e538964eed4fc815a46efa15e9bf666ddd2776e5455
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
      "user_id": 516,
      "feedbackable_id": 69,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:30.820Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 515,
      "feedbackable_id": 69,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:30.809Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/69/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbd02a4e5d82f65d2f6b9e538964eed4fc815a46efa15e9bf666ddd2776e5455"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/80/votes
Content-Type: application/json
Authorization: Bearer e94ab5c1fae9cbcd3886f191e86a658695a67dc7af82b2a5d036818d7ecd0685
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
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 80,
      "user_id": 630
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 80,
      "user_id": 629
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 80,
      "user_id": 628
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/80/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e94ab5c1fae9cbcd3886f191e86a658695a67dc7af82b2a5d036818d7ecd0685"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/27/republish
Content-Type: application/json
Authorization: Bearer e9d9d20cee35af31d706e577c0837591a082a270b4d535856e120a37c2410349
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
	-H "Authorization: Bearer e9d9d20cee35af31d706e577c0837591a082a270b4d535856e120a37c2410349"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/29/bookmark
Content-Type: application/json
Authorization: Bearer b0c53a29d4338ce545ce9be405eab45ae5f688f051cfb0bed7b7a51056fdc818
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/29/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0c53a29d4338ce545ce9be405eab45ae5f688f051cfb0bed7b7a51056fdc818"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/10
Content-Type: application/json
Authorization: Bearer 6a684df9682d2f47343b46c767277a7f952610507c124e6a9cdda3d6ec661b1f
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a684df9682d2f47343b46c767277a7f952610507c124e6a9cdda3d6ec661b1f"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/9/downvote
Content-Type: application/json
Authorization: Bearer 49c8843ed9d823fa4d34d0f2a2434398767581c229834cb7aac70a9f5ae7a17f
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
	-H "Authorization: Bearer 49c8843ed9d823fa4d34d0f2a2434398767581c229834cb7aac70a9f5ae7a17f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/31
Content-Type: application/json
Authorization: Bearer 3b45d71b28967d437a64d4ffc1655e268c7026e11547e99177af70691f075d2f
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 368,
    "chapter_id": 101,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:56:14.328Z",
    "created_at": "2016-11-18T10:56:14.328Z",
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
curl "api.goskive.com/v2/flashcards/31" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b45d71b28967d437a64d4ffc1655e268c7026e11547e99177af70691f075d2f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/report
Content-Type: application/json
Authorization: Bearer a3a11f93d34f1eac6d6bffee150a647d3df148227b08c2bc6babccbbbd236050
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
	-H "Authorization: Bearer a3a11f93d34f1eac6d6bffee150a647d3df148227b08c2bc6babccbbbd236050"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/30/bookmark
Content-Type: application/json
Authorization: Bearer e142ef9f779385ad2214d1c9a1d64b6fa2331f860801486efb88edb9b818c22a
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/30/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e142ef9f779385ad2214d1c9a1d64b6fa2331f860801486efb88edb9b818c22a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/32/upvote
Content-Type: application/json
Authorization: Bearer 14a28cdc81f0738612b430a2a0e421f00c5b37b43d2c7475cab9026a3d962757
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/32/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14a28cdc81f0738612b430a2a0e421f00c5b37b43d2c7475cab9026a3d962757"
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
    "key": "cache/b4c43f0fa86d702bf3b4b9ca32ad9aff.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0xOFQxMTo1NjozNVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I0YzQzZjBmYTg2ZDcwMmJmM2I0YjljYTMyYWQ5YWZmLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTExOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMThUMTA1NjM1WiJ9XX0=",
    "x-amz-credential": "FAKE/20161118/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161118T105635Z",
    "x-amz-signature": "b8bf76f4003b8a00a91e0b6f580326086ac33a1e26f821efd5a416aa6530083d"
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
Authorization: Bearer b35597a9f43d0c0ebd7854baa7134a7f5bd049db993ece45ba0e5bbd1381fb2c
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
	-H "Authorization: Bearer b35597a9f43d0c0ebd7854baa7134a7f5bd049db993ece45ba0e5bbd1381fb2c"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer bcb1c51f592c14bad66d4112c8ae42e1cb94390fa72048959fb87371c4ad0568
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
	-H "Authorization: Bearer bcb1c51f592c14bad66d4112c8ae42e1cb94390fa72048959fb87371c4ad0568"
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
{"password":{"reset_password_token":"snxY1-yNGqcyXAQuTBJ7","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 544,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-18T10:56:33.699Z",
  "updated_at": "2016-11-18T10:56:33.833Z",
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
  "audit_id": 5135
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"snxY1-yNGqcyXAQuTBJ7","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/102/comments
Content-Type: application/json
Authorization: Bearer e2913945a155956a195c3ab9a3f74b97f4d8a7956871bbc1ac36ab110bd6fbf3
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
    "id": 53,
    "author_id": 787,
    "reply_to_id": null,
    "created_at": "2016-11-18T10:56:49.769Z",
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
curl "api.goskive.com/v2/questions/102/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2913945a155956a195c3ab9a3f74b97f4d8a7956871bbc1ac36ab110bd6fbf3"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/101/comments
Content-Type: application/json
Authorization: Bearer 9472ff14ca9b2532e2e008e65228d5b9e7510d5a126430c867810a79a412c773
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
    "author_id": 784,
    "reply_to_id": null,
    "created_at": "2016-11-18T10:56:49.293Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 17,
      "user_id": 784,
      "feedbackable_id": 101,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:49.289Z",
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
curl "api.goskive.com/v2/questions/101/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9472ff14ca9b2532e2e008e65228d5b9e7510d5a126430c867810a79a412c773"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/105/comments
Content-Type: application/json
Authorization: Bearer 46afa1ddf1c2e6c86f674b9a7e8a76e9110eaf4ef85fe0220fa6f49b0b7a5e3b
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
      "author_id": 799,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:50.858Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 800,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:50.874Z",
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
curl "api.goskive.com/v2/questions/105/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46afa1ddf1c2e6c86f674b9a7e8a76e9110eaf4ef85fe0220fa6f49b0b7a5e3b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/103/comments
Content-Type: application/json
Authorization: Bearer d1746cd5a2bf79fbf7a1c202b570fdb2cfdfe5b9386613754932147e86ee1525
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
curl "api.goskive.com/v2/questions/103/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1746cd5a2bf79fbf7a1c202b570fdb2cfdfe5b9386613754932147e86ee1525"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/46/feedbacks
Content-Type: application/json
Authorization: Bearer db6c81197a09208e124b41cd59eda1ee76acabb66c29596e61e3b7213a1aaf5b
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
    "id": 1,
    "user_id": 255,
    "feedbackable_id": 46,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-18T10:56:07.418Z",
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
curl "api.goskive.com/v2/questions/46/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db6c81197a09208e124b41cd59eda1ee76acabb66c29596e61e3b7213a1aaf5b"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/49/feedbacks
Content-Type: application/json
Authorization: Bearer fac314c318f9bdc7cb8ce50260d9622d508b3cf6f78454f2e07e093f37b1675d
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
      "id": 4,
      "user_id": 268,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:08.658Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 267,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:08.647Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fac314c318f9bdc7cb8ce50260d9622d508b3cf6f78454f2e07e093f37b1675d"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/5/votes
Content-Type: application/json
Authorization: Bearer a2a6ae5c4fdf3d12ebe802cb3d946b2bc57bc928b2a526d1b33fa8a9b8fb95a8
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 5,
      "user_id": 52
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 5,
      "user_id": 51
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 5,
      "user_id": 50
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/5/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2a6ae5c4fdf3d12ebe802cb3d946b2bc57bc928b2a526d1b33fa8a9b8fb95a8"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/37/republish
Content-Type: application/json
Authorization: Bearer 75a021442b03240640acf7d8a39a33ab531cc0b7d71b868ac00f6e35c958642b
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
curl "api.goskive.com/v2/questions/37/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75a021442b03240640acf7d8a39a33ab531cc0b7d71b868ac00f6e35c958642b"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/35/bookmark
Content-Type: application/json
Authorization: Bearer 8da471550c7b98691b25ea48e5ce756527e834313bdb2890a06b973b424efc0d
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/35/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8da471550c7b98691b25ea48e5ce756527e834313bdb2890a06b973b424efc0d"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/33
Content-Type: application/json
Authorization: Bearer 4fe90a28941b7d929814f8226d3d8af7eb1e36e5b20082e20aa5bb532cf830db
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/33" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fe90a28941b7d929814f8226d3d8af7eb1e36e5b20082e20aa5bb532cf830db"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/30/downvote
Content-Type: application/json
Authorization: Bearer 48106bb414103b212aa119b9ef5a24ade26a5f1428d6540edb329a386b666967
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/30/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48106bb414103b212aa119b9ef5a24ade26a5f1428d6540edb329a386b666967"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/29
Content-Type: application/json
Authorization: Bearer 48231445d8314619d23eefd1ff4f75fbb479a6ae6d6c5963c22d0f74d1bd053e
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
    "id": 29,
    "obfuscated_id": "rvs1sHrnKS4",
    "author_id": 142,
    "chapter_id": 32,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:55:56.450Z",
    "created_at": "2016-11-18T10:55:56.316Z",
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
        "id": 57,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 58,
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
curl "api.goskive.com/v2/questions/29" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48231445d8314619d23eefd1ff4f75fbb479a6ae6d6c5963c22d0f74d1bd053e"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/34/report
Content-Type: application/json
Authorization: Bearer 0a9516f726e628a84b59745b9e119982f220144b836a7f8399b5ed3bebcd89d1
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a9516f726e628a84b59745b9e119982f220144b836a7f8399b5ed3bebcd89d1"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/32/bookmark
Content-Type: application/json
Authorization: Bearer 30ef580b8c11c779f8a4537ea64615993beb78456203afce5d76e072795d0e41
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/32/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30ef580b8c11c779f8a4537ea64615993beb78456203afce5d76e072795d0e41"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/31
Content-Type: application/json
Authorization: Bearer 87c380ccf1a1ef8f1070532c2738600b3e6e32bd03c29ca59bade477b11d90e1
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":31,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-18T10:55:57.095Z","updated_at":"2016-11-18T10:55:57.226Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":34,"author_id":148,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 31,
    "obfuscated_id": "5rbCnI5XGHg",
    "author_id": 148,
    "chapter_id": 34,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-18T10:55:57.341Z",
    "created_at": "2016-11-18T10:55:57.095Z",
    "tags": [
      {
        "id": 6,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 5,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>31, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-18T10:55:57.095Z\", \"updated_at\"=>\"2016-11-18T10:55:57.226Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>34, \"author_id\"=>148, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 61,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 62,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 63,
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
curl "api.goskive.com/v2/questions/31" -d '{"question":{"question":{"id":31,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-18T10:55:57.095Z","updated_at":"2016-11-18T10:55:57.226Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":34,"author_id":148,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87c380ccf1a1ef8f1070532c2738600b3e6e32bd03c29ca59bade477b11d90e1"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/38/upvote
Content-Type: application/json
Authorization: Bearer c2aa5ff7808050966d85e80860f89a4edd055a2fcec6a13722c4e2350073be50
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
	-H "Authorization: Bearer c2aa5ff7808050966d85e80860f89a4edd055a2fcec6a13722c4e2350073be50"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6c21f238a50f2c864e5b1890f169213e2569030aa2a187c2a0ecf336c800a966
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
      "creator_id": 550,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 171,
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
      "updated_at": "2016-11-18T10:56:34.129Z",
      "shortname": "mit-pizza-201",
      "topic_id": 192,
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
	-H "Authorization: Bearer 6c21f238a50f2c864e5b1890f169213e2569030aa2a187c2a0ecf336c800a966"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 2bcead84a390db6532eeabb61d9e6851ca97182485d6dd4657d9e24aee246796
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
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-149",
      "html_url": "https://goskive.com/university/uni-149",
      "slug": "uni-149",
      "name": "National School of Pizza",
      "short_name": "Uni 149",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/7bc79840e61bacbd55aa93f5552ed498973da7e3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ef722df136740df4f3ec930d2c63e36ea0aab6cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T10:56:33.967Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-148",
      "html_url": "https://goskive.com/university/uni-148",
      "slug": "uni-148",
      "name": "National School of Pastry",
      "short_name": "Uni 148",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/04608c10e52ede3ea37be09b081d69e95b921be1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2de1e8a9f298593a399f64c7eacf215a79baee4a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T10:56:33.949Z",
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
	-H "Authorization: Bearer 2bcead84a390db6532eeabb61d9e6851ca97182485d6dd4657d9e24aee246796"
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
      "id": 81,
      "name": "Multi-tiered content-based productivity",
      "name_translations": {
        "en": "Multi-tiered content-based productivity"
      },
      "discipline_id": 81
    },
    {
      "id": 82,
      "name": "Open-architected asynchronous hierarchy",
      "name_translations": {
        "en": "Open-architected asynchronous hierarchy"
      },
      "discipline_id": 82
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
GET /v2/topics/80
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
    "id": 80,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 80
  }
}
```



```shell
curl "api.goskive.com/v2/topics/80" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 2e6844992d0d85addbea9ecca2721a658d6a5163770509aa0a5b91369cc97037
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
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-62",
      "html_url": "https://goskive.com/university/uni-62",
      "slug": "uni-62",
      "name": "University 47",
      "short_name": "Uni 62",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9939c76ba15dd234d59735df6dc666f7e74e91bc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/329c40401896c3249f00c3af10ad482972be9a53.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T10:56:06.813Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-63",
      "html_url": "https://goskive.com/university/uni-63",
      "slug": "uni-63",
      "name": "University 48",
      "short_name": "Uni 63",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/09729f1083d256271401c420f0ba16e452eb8033.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/6555adfa3dcc1f7c3ae4c87db69e3a789b6cf1f4.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T10:56:06.830Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 82,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-64",
      "html_url": "https://goskive.com/university/uni-64",
      "slug": "uni-64",
      "name": "University 49",
      "short_name": "Uni 64",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/55a93dfbea26e71abb477ed2ac5e96669bce8e00.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/0ab862876eec4175aff27ea2f4e2a3244a433f8b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-18T10:56:06.846Z",
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
	-H "Authorization: Bearer 2e6844992d0d85addbea9ecca2721a658d6a5163770509aa0a5b91369cc97037"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer af518bb4865c898fe71fa0f56f1964ae3c04eb425a75b3d3db6c8d24e3808699
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
    "id": 84,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/007ac229263210b73c1c1b94495f61eba41fa753.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/02bc84a61eeca0d671b84f4cda55974ecc3b4877.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-18T10:56:06.969Z",
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
	-H "Authorization: Bearer af518bb4865c898fe71fa0f56f1964ae3c04eb425a75b3d3db6c8d24e3808699"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9745a5fa8183dc272e9413751b9f52a5a5d975deb346f815c23e39c1c4574e02
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":3,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 4,
    "id": 3,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 3,
    "additional_university_ids": [

    ],
    "discipline_id": 3,
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
    "chapters_updated_at": "2016-11-18T10:55:43.546Z",
    "updated_at": "2016-11-18T10:55:43.694Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 1,
        "updated_at": "2016-11-18T10:55:43.647Z",
        "course_id": 3,
        "author_id": 4,
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
        "id": 2,
        "updated_at": "2016-11-18T10:55:43.668Z",
        "course_id": 3,
        "author_id": 4,
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
        "id": 3,
        "updated_at": "2016-11-18T10:55:43.684Z",
        "course_id": 3,
        "author_id": 4,
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
    "topic_id": 3,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":3,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9745a5fa8183dc272e9413751b9f52a5a5d975deb346f815c23e39c1c4574e02"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b21e9d6877139c226f95919966f5411e665efed9009e757aa5b1b1c17ab6b060
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":2,"published":false}}
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
    "creator_id": 3,
    "id": 2,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 2,
    "additional_university_ids": [

    ],
    "discipline_id": 2,
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
    "updated_at": "2016-11-18T10:55:43.474Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 2,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":2,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b21e9d6877139c226f95919966f5411e665efed9009e757aa5b1b1c17ab6b060"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fa5d1589bb9d0e1bd28cb018257630844280c48bf2d315b98fda08fd424ff9ae
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
      "creator_id": 21,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "discipline_id": 19,
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
      "updated_at": "2016-11-18T10:55:45.366Z",
      "shortname": "fu-course-15",
      "topic_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 21,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "discipline_id": 20,
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
      "chapters_updated_at": "2016-11-18T10:55:45.235Z",
      "updated_at": "2016-11-18T10:55:45.652Z",
      "shortname": "fu-course-16",
      "topic_id": 20,
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
	-H "Authorization: Bearer fa5d1589bb9d0e1bd28cb018257630844280c48bf2d315b98fda08fd424ff9ae"
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
      "creator_id": 31,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "discipline_id": 27,
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
      "updated_at": "2016-11-18T10:55:46.195Z",
      "shortname": "fu-course-23",
      "topic_id": 27,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 31,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "discipline_id": 28,
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
      "chapters_updated_at": "2016-11-18T10:55:46.031Z",
      "updated_at": "2016-11-18T10:55:46.513Z",
      "shortname": "fu-course-24",
      "topic_id": 28,
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
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 22dd1382db94e608406c103e34b51801992b82fb446112da6cea3075d33e2767
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
      "creator_id": 28,
      "id": 23,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 23,
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
      "updated_at": "2016-11-18T10:55:45.916Z",
      "shortname": "fu-course-19",
      "topic_id": 23,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 28,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 24,
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
      "updated_at": "2016-11-18T10:55:45.954Z",
      "shortname": "fu-course-20",
      "topic_id": 24,
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
	-H "Authorization: Bearer 22dd1382db94e608406c103e34b51801992b82fb446112da6cea3075d33e2767"
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
      "creator_id": 36,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 14,
      "additional_university_ids": [

      ],
      "discipline_id": 31,
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
      "updated_at": "2016-11-18T10:55:46.673Z",
      "shortname": "fu-course-27",
      "topic_id": 31,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 36,
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 14,
      "additional_university_ids": [

      ],
      "discipline_id": 32,
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
      "updated_at": "2016-11-18T10:55:46.708Z",
      "shortname": "fu-course-28",
      "topic_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
Authorization: Bearer ba38321e098d70615e8a58b10e13cfa27adff3056487817a8562907b9edc2a5a
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
  "id": 1,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-18T10:55:41.990Z",
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
	-H "Authorization: Bearer ba38321e098d70615e8a58b10e13cfa27adff3056487817a8562907b9edc2a5a"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/520
Content-Type: application/json
Authorization: Bearer dbd4e69a7ab949e4b186a524a32d100674eb2cd1f5234b0dbc9605e27dc4e415
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
    "id": 520,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 161,
    "fields_of_study": [
      183,
      184
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-18T10:56:31.097Z",
    "updated_at": "2016-11-18T10:56:31.097Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/520" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbd4e69a7ab949e4b186a524a32d100674eb2cd1f5234b0dbc9605e27dc4e415"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/522
Content-Type: application/json
Authorization: Bearer bea5bb1d9e941632fc46be05462386b3f1c46376d088bf1297336f795b51bf0c
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
    "id": 522,
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
    "created_at": "2016-11-18T10:56:31.187Z",
    "updated_at": "2016-11-18T10:56:31.187Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/522" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bea5bb1d9e941632fc46be05462386b3f1c46376d088bf1297336f795b51bf0c"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer 4e1d727970aac2fd1f25262bf047028583c79b143a8d716443424eb496a7ca5b
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
	-H "Authorization: Bearer 4e1d727970aac2fd1f25262bf047028583c79b143a8d716443424eb496a7ca5b"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/22
Content-Type: application/json
Authorization: Bearer d55498d805308fc90d3b280b2f045e5d4c8ce544f840f3803f69c18a84daf36d
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
    "id": 22,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 133,
    "user_id": 957
  }
}
```



```shell
curl "api.goskive.com/v2/votes/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d55498d805308fc90d3b280b2f045e5d4c8ce544f840f3803f69c18a84daf36d"
```
