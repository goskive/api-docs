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
Authorization: Basic NWI2M2QxZWJhZTQ1MTg1YmZjYzI5MTljNTRiYmI4ZWU2MWUwM2IzNTg5NDg3
OThiODVhMDA5NjRmYTNkMzhkZTo5NzVjMDc3NGM4ZTAxMmQzYzZjOTE3MDYz
Y2M0OTQ2ZDI3OWMxYjdlODJjNzZmODA5OWIyYjNhZDk2NDkxYzUy

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
	-u 5b63d1ebae45185bfcc2919c54bbb8ee61e03b358948798b85a00964fa3d38de:975c0774c8e012d3c6c917063cc4946d279c1b7e82c76f8099b2b3ad96491c52
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2699da97ac5021f211c6793ec1dd3418bf6ab37beadda193c72b273ac8c6f34b","client_secret":"55a266d3d5147c6a8920077c04ed8ed5bff95dfd5a10adaceb2b1285d82141f4"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2699da97ac5021f211c6793ec1dd3418bf6ab37beadda193c72b273ac8c6f34b","client_secret":"55a266d3d5147c6a8920077c04ed8ed5bff95dfd5a10adaceb2b1285d82141f4"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZTE1NjhiNDkxYTQxNmFmMDJkZDA0ZTk5NTZkOTA2OGJjNDE1ZDQ3YmExMGNh
M2ViZmNlMDA2Y2UxYzczM2RkZjpiZTFlMDNmZTAzMmEzOTQ4OGVlNTQ2NDk4
MTcwNTJkYjYyMWNmZTE2YTBkZGMzMWI1YTQzNGJlN2IxNDczYTk5

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
  "access_token": "b43396fa4310cd900a1e6bdeda9170e66d8fa64cf2f5296c5c55b6942c485d79",
  "token_type": "bearer",
  "created_at": 1481820602
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u e1568b491a416af02dd04e9956d9068bc415d47ba10ca3ebfce006ce1c733ddf:be1e03fe032a39488ee54649817052db621cfe16a0ddc31b5a434be7b1473a99
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1fbcd95fcf9843d428ff09c20354e1249265ccbb5baa007489809fc535224862","client_secret":"454cdd695ba2cfad8ea0a776da01360d0073602b2cbad0a865b91fc0229d0809"}
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
  "access_token": "b47d7680bd8a8b03f821ab331ab725022bd93eaa8a314a83766ae8bc5a1df3f5",
  "token_type": "bearer",
  "created_at": 1481820602
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1fbcd95fcf9843d428ff09c20354e1249265ccbb5baa007489809fc535224862","client_secret":"454cdd695ba2cfad8ea0a776da01360d0073602b2cbad0a865b91fc0229d0809"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"b5ab4cca690208c9e37f1efa4d2fb64a4352ac9b040a838a972d6b865658d3af","client_secret":"b501c917f5ef3a981a66022148fbdf0482e6562e78e84c69eb711ed8c9c3d849"}
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
  "access_token": "cd56e21c79d568deca0f533dd226b22c30c05b7ef9a1dd067b27037f7c340818",
  "token_type": "bearer",
  "created_at": 1481820602
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"b5ab4cca690208c9e37f1efa4d2fb64a4352ac9b040a838a972d6b865658d3af","client_secret":"b501c917f5ef3a981a66022148fbdf0482e6562e78e84c69eb711ed8c9c3d849"}' -X POST \
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
Authorization: Bearer d3a00d529a757e67752f9c1b5ec53fc85f05e3fa813ed042ec48a64bfc1b1c01
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
    "company_id": 24,
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
	-H "Authorization: Bearer d3a00d529a757e67752f9c1b5ec53fc85f05e3fa813ed042ec48a64bfc1b1c01"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/193/flashcards
Content-Type: application/json
Authorization: Bearer d3ed50e06876e6b25293b42a7e5879fd24ee8d21f17855eb34f9cf073aae09df
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
    "id": 96,
    "obfuscated_id": "SEtQvXxfwHo",
    "author_id": 982,
    "chapter_id": 193,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:50:18.105Z",
    "created_at": "2016-12-15T16:50:18.105Z",
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
	-H "Authorization: Bearer d3ed50e06876e6b25293b42a7e5879fd24ee8d21f17855eb34f9cf073aae09df"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/195/flashcards
Content-Type: application/json
Authorization: Bearer c25cea3e6eea1e9ffbd6244e9f191a56fd0c7012e319ef19d720575d749060bf
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
      "id": 97,
      "obfuscated_id": "qdTHUgSdSV8",
      "author_id": 986,
      "chapter_id": 195,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:50:18.611Z",
      "created_at": "2016-12-15T16:50:18.611Z",
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
      "id": 98,
      "obfuscated_id": "icApzX10lRE",
      "author_id": 986,
      "chapter_id": 195,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:50:18.652Z",
      "created_at": "2016-12-15T16:50:18.652Z",
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
      "id": 99,
      "obfuscated_id": "5fPQ9k37GTc",
      "author_id": 986,
      "chapter_id": 195,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:50:18.693Z",
      "created_at": "2016-12-15T16:50:18.693Z",
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
curl "api.goskive.com/v2/chapters/195/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c25cea3e6eea1e9ffbd6244e9f191a56fd0c7012e319ef19d720575d749060bf"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/5/questions
Content-Type: application/json
Authorization: Bearer adee79116bd68a4ab7d2949af24d5f971f26fe7654fc714d76e75c8b4f699e83
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 25,
    "chapter_id": 5,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:48:50.475Z",
    "created_at": "2016-12-15T16:48:50.475Z",
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
        "id": 12,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 13,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 14,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 15,
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
curl "api.goskive.com/v2/chapters/5/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":5,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer adee79116bd68a4ab7d2949af24d5f971f26fe7654fc714d76e75c8b4f699e83"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/4/questions
Content-Type: application/json
Authorization: Bearer 721e884529f0bb2a65ec819c0dde4bbb055f27b772f2f754c343ced3021de0c3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 22,
    "chapter_id": 4,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:48:49.922Z",
    "created_at": "2016-12-15T16:48:49.922Z",
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
        "id": 10,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 11,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/4/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":4,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 721e884529f0bb2a65ec819c0dde4bbb055f27b772f2f754c343ced3021de0c3"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/6/questions
Content-Type: application/json
Authorization: Bearer 3f0e519499bdf0f06c09843bdc81b6b989401e78b372738b885209d3f0974396
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 28,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:48:51.122Z",
    "created_at": "2016-12-15T16:48:51.122Z",
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
        "id": 16,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 17,
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
curl "api.goskive.com/v2/chapters/6/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":6,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f0e519499bdf0f06c09843bdc81b6b989401e78b372738b885209d3f0974396"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/3/questions
Content-Type: application/json
Authorization: Bearer 49bb9b121f4f670308ba08106234b33670501f8aaeb1a5c7bbee7c6d9fd0232f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":3,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 19,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:48:49.425Z",
    "created_at": "2016-12-15T16:48:49.425Z",
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
        "id": 7,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 8,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 9,
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
curl "api.goskive.com/v2/chapters/3/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":3,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49bb9b121f4f670308ba08106234b33670501f8aaeb1a5c7bbee7c6d9fd0232f"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/1/questions
Content-Type: application/json
Authorization: Bearer 7945d7c2d18078c949fed50fadbe7337c865125691a560332b4dc9de7198e2fb
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
      "author_id": 10,
      "chapter_id": 1,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:48:48.513Z",
      "created_at": "2016-12-15T16:48:48.419Z",
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
      "author_id": 11,
      "chapter_id": 1,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:48:48.677Z",
      "created_at": "2016-12-15T16:48:48.585Z",
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
      "author_id": 12,
      "chapter_id": 1,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T16:48:48.865Z",
      "created_at": "2016-12-15T16:48:48.776Z",
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
curl "api.goskive.com/v2/chapters/1/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7945d7c2d18078c949fed50fadbe7337c865125691a560332b4dc9de7198e2fb"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/127
Content-Type: application/json
Authorization: Bearer 6963a35bbbfbeb4f121ee21a51d769d6f389ff840a9df78a40c18a28c9ea9a95
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
curl "api.goskive.com/v2/chapters/127" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6963a35bbbfbeb4f121ee21a51d769d6f389ff840a9df78a40c18a28c9ea9a95"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/128
Content-Type: application/json
Authorization: Bearer 84cf38ad39317abc1451fd046b620a75661f2843b28a3717351ade76c009e377
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
curl "api.goskive.com/v2/chapters/128" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84cf38ad39317abc1451fd046b620a75661f2843b28a3717351ade76c009e377"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/131
Content-Type: application/json
Authorization: Bearer 4f3e6e0f14650379d7cffb86166cceb66c1ff59c485c1c0ea57955144725b2a4
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
curl "api.goskive.com/v2/chapters/131" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f3e6e0f14650379d7cffb86166cceb66c1ff59c485c1c0ea57955144725b2a4"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/129
Content-Type: application/json
Authorization: Bearer bd1f6ccce430ff467d7d6649d2d99e71f1169de677020c5126620897463dc701
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/129" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd1f6ccce430ff467d7d6649d2d99e71f1169de677020c5126620897463dc701"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/133
Content-Type: application/json
Authorization: Bearer aa1a89bd80e135f4bf101633403f114d32907e614ee5ea1d32f2c8bda1a7eb5f
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
    "id": 133,
    "updated_at": "2016-12-15T16:49:39.361Z",
    "course_id": 148,
    "author_id": 531,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-15T16:49:38.853Z",
    "questions_updated_at": "2016-12-15T16:49:38.853Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 535,
        "chapter_id": 133,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:39.343Z",
        "created_at": "2016-12-15T16:49:39.343Z",
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
        "author_id": 533,
        "chapter_id": 133,
        "position": 81,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:39.239Z",
        "created_at": "2016-12-15T16:49:39.152Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/133" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa1a89bd80e135f4bf101633403f114d32907e614ee5ea1d32f2c8bda1a7eb5f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/132
Content-Type: application/json
Authorization: Bearer c25ba32b38056822f553156da44838e465ce7cf50c03ee32741c35a4f8191f91
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
    "id": 132,
    "updated_at": "2016-12-15T16:49:38.811Z",
    "course_id": 147,
    "author_id": 529,
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
curl "api.goskive.com/v2/chapters/132" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c25ba32b38056822f553156da44838e465ce7cf50c03ee32741c35a4f8191f91"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/7/replies
Content-Type: application/json
Authorization: Bearer e6a72c4d0921bd93019630e7d3c0f00b407b84c03e3e7c1be6130f3347dbe098
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
    "id": 8,
    "author_id": 215,
    "reply_to_id": 7,
    "created_at": "2016-12-15T16:49:07.452Z",
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
curl "api.goskive.com/v2/comments/7/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6a72c4d0921bd93019630e7d3c0f00b407b84c03e3e7c1be6130f3347dbe098"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/6/replies
Content-Type: application/json
Authorization: Bearer 1febf4c487f0128cd49c82737d44db882f518077eb1660df66355509a50ad190
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
curl "api.goskive.com/v2/comments/6/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1febf4c487f0128cd49c82737d44db882f518077eb1660df66355509a50ad190"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer 730404715d495dc04144d58b9b045e898131baad679687678cf70be35fbd53d3
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
curl "api.goskive.com/v2/comments/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 730404715d495dc04144d58b9b045e898131baad679687678cf70be35fbd53d3"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/24/republish
Content-Type: application/json
Authorization: Bearer e181f792c2dadb8120513af0023dd14c2186b67af5a00fc523272e527858baa4
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
curl "api.goskive.com/v2/comments/24/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e181f792c2dadb8120513af0023dd14c2186b67af5a00fc523272e527858baa4"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/21
Content-Type: application/json
Authorization: Bearer 5faa7b87ccb5489a65146625d8f216223b3432ada370fc9f467737ee2eeeb819
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5faa7b87ccb5489a65146625d8f216223b3432ada370fc9f467737ee2eeeb819"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/25/report
Content-Type: application/json
Authorization: Bearer 596897ed53a1cd8ea6ab0e30bc5d36e25fb7a34d29ab657698d9a318516d97e8
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/25/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 596897ed53a1cd8ea6ab0e30bc5d36e25fb7a34d29ab657698d9a318516d97e8"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/25
Content-Type: application/json
Authorization: Bearer ec302ecb292dce5ca934270a4ca9b6aa119b5c9c4e3934c9b5f8836b2a196cf7
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
    "id": 25,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-15T16:50:01.179Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec302ecb292dce5ca934270a4ca9b6aa119b5c9c4e3934c9b5f8836b2a196cf7"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 54124585e657cf0092f3b9e476a3f40cf024796ed8c94b64a6b6463ccd52cd57
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
      "id": 26,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T16:50:01.312Z"
    },
    {
      "id": 27,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T16:50:01.316Z"
    },
    {
      "id": 28,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-15T16:50:01.321Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54124585e657cf0092f3b9e476a3f40cf024796ed8c94b64a6b6463ccd52cd57"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/30/company_profiles
Content-Type: application/json
Authorization: Bearer 814f5fb99d740d08f6b6180c433635507b10362adcdf6e073e197279d125d47e
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
curl "api.goskive.com/v2/companies/30/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 814f5fb99d740d08f6b6180c433635507b10362adcdf6e073e197279d125d47e"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/29/company_profiles
Content-Type: application/json
Authorization: Bearer a743b7dc763d0fdc2842e6fe76f05e0f9bf988d0fbe9ae460e1c27282b90143d
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
curl "api.goskive.com/v2/companies/29/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a743b7dc763d0fdc2842e6fe76f05e0f9bf988d0fbe9ae460e1c27282b90143d"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 46635b71415df53e84a5a5f5c15166ef9e52188144288b3804d446e767347b60
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
	-H "Authorization: Bearer 46635b71415df53e84a5a5f5c15166ef9e52188144288b3804d446e767347b60"
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
Authorization: Bearer e7692981d508e72f258c0f4bcc2f79fd6beb2d0f877cbc90ca15ad0230128532
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
	-H "Authorization: Bearer e7692981d508e72f258c0f4bcc2f79fd6beb2d0f877cbc90ca15ad0230128532"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9c2952ce627798c1f81995d2cfc594d3286183dc0c3573c1923c39407f356c74
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
    "id": 96,
    "updated_at": "2016-12-15T16:49:28.476Z",
    "course_id": 119,
    "author_id": 423,
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
	-H "Authorization: Bearer 9c2952ce627798c1f81995d2cfc594d3286183dc0c3573c1923c39407f356c74"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0ef76ffbd9e4f178e1e73b693adf119465d762a98a83d3d1967b3e2edfa03294
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
      "id": 105,
      "updated_at": "2016-12-15T16:49:30.084Z",
      "course_id": 126,
      "author_id": 445,
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
      "id": 106,
      "updated_at": "2016-12-15T16:49:30.111Z",
      "course_id": 126,
      "author_id": 446,
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
      "id": 107,
      "updated_at": "2016-12-15T16:49:30.342Z",
      "course_id": 126,
      "author_id": 447,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T16:49:29.959Z",
      "questions_updated_at": "2016-12-15T16:49:29.959Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 98",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ef76ffbd9e4f178e1e73b693adf119465d762a98a83d3d1967b3e2edfa03294"
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
      "id": 111,
      "updated_at": "2016-12-15T16:49:31.001Z",
      "course_id": 129,
      "author_id": 459,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 102",
      "position": 1
    },
    {
      "id": 112,
      "updated_at": "2016-12-15T16:49:31.027Z",
      "course_id": 129,
      "author_id": 460,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 103",
      "position": 2
    },
    {
      "id": 113,
      "updated_at": "2016-12-15T16:49:31.255Z",
      "course_id": 129,
      "author_id": 461,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-15T16:49:30.874Z",
      "questions_updated_at": "2016-12-15T16:49:30.874Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 104",
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
Authorization: Bearer 273965d880981245013bb30da6dc04f0bb8eeaf22e7c8c025bf74a041ba3624f
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
      "id": 108,
      "updated_at": "2016-12-15T16:49:30.560Z",
      "course_id": 127,
      "author_id": 452,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 99",
      "position": 1
    },
    {
      "id": 109,
      "updated_at": "2016-12-15T16:49:30.586Z",
      "course_id": 127,
      "author_id": 453,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 100",
      "position": 2
    },
    {
      "id": 110,
      "updated_at": "2016-12-15T16:49:30.610Z",
      "course_id": 127,
      "author_id": 454,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 101",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 273965d880981245013bb30da6dc04f0bb8eeaf22e7c8c025bf74a041ba3624f"
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
      "id": 114,
      "updated_at": "2016-12-15T16:49:31.598Z",
      "course_id": 131,
      "author_id": 466,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 105",
      "position": 1
    },
    {
      "id": 115,
      "updated_at": "2016-12-15T16:49:31.624Z",
      "course_id": 131,
      "author_id": 467,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 106",
      "position": 2
    },
    {
      "id": 116,
      "updated_at": "2016-12-15T16:49:31.650Z",
      "course_id": 131,
      "author_id": 468,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 107",
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
Authorization: Bearer 51cb7cba02b2ef355825b0015fbfa639cfe97e092237643ae9fb415cb209078a
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
    "course_id": 155,
    "user_id": 559,
    "updated_at": "2016-12-15T16:49:41.212Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51cb7cba02b2ef355825b0015fbfa639cfe97e092237643ae9fb415cb209078a"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 4210432497407928de12c49a1a001f7337d52f26e19c0ad7a2bca3c96eeca251
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
      "course_id": 151,
      "user_id": 547,
      "updated_at": "2016-12-15T16:49:40.386Z"
    },
    {
      "id": 3,
      "course_id": 151,
      "user_id": 548,
      "updated_at": "2016-12-15T16:49:40.401Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4210432497407928de12c49a1a001f7337d52f26e19c0ad7a2bca3c96eeca251"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/190/files
Content-Type: application/json
Authorization: Bearer bf921fbaa7ef0bd4befa3aab59d54269967555a083dbb83fe5e937bf5ca40487
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
        "id": 689,
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
        "created_at": "2016-12-15T16:49:53.751Z",
        "updated_at": "2016-12-15T16:49:53.751Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T16:49:53.761Z",
      "updated_at": "2016-12-15T16:49:53.761Z",
      "course_id": 190,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 7,
      "uploader": {
        "id": 690,
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
        "created_at": "2016-12-15T16:49:53.772Z",
        "updated_at": "2016-12-15T16:49:53.772Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T16:49:53.782Z",
      "updated_at": "2016-12-15T16:49:53.782Z",
      "course_id": 190,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 8,
      "uploader": {
        "id": 691,
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
        "created_at": "2016-12-15T16:49:53.792Z",
        "updated_at": "2016-12-15T16:49:53.792Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-15T16:49:53.802Z",
      "updated_at": "2016-12-15T16:49:53.802Z",
      "course_id": 190,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/190/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf921fbaa7ef0bd4befa3aab59d54269967555a083dbb83fe5e937bf5ca40487"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/192/files
Content-Type: application/json
Authorization: Bearer fac50d1fcae102ea0e3a3c748713b330a98536bd7deefcda0faf3373b80b7b04
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
      "id": 696,
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
      "created_at": "2016-12-15T16:49:54.158Z",
      "updated_at": "2016-12-15T16:49:54.158Z"
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
    "created_at": "2016-12-15T16:49:54.190Z",
    "updated_at": "2016-12-15T16:49:54.190Z",
    "course_id": 192,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/192/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fac50d1fcae102ea0e3a3c748713b330a98536bd7deefcda0faf3373b80b7b04"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/193/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer b14977ea31fcdc989fae8c9b9ebe79110b4e612b20d09f01b6fc100ee557b6eb
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
    "key": "cache/e72de47d698679d19140f146508101b1.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNzo0OTo1NFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2U3MmRlNDdkNjk4Njc5ZDE5MTQwZjE0NjUwODEwMWIxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMTUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjE1VDE2NDk1NFoifV19",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T164954Z",
    "x-amz-signature": "c1413dfb649423677ed4201e0456dfd329db64e6bd88e04c0310c9307e2ab3b5"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/193/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b14977ea31fcdc989fae8c9b9ebe79110b4e612b20d09f01b6fc100ee557b6eb"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 8b29db386bfc5adc8debc6f0fd3f052df6a2bd552f5274d01e3db8597d5ebe1d
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
	-H "Authorization: Bearer 8b29db386bfc5adc8debc6f0fd3f052df6a2bd552f5274d01e3db8597d5ebe1d"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer af4fbacdafb85525468ff418af56a187d54f951427e4de08ac6a6c858d9af7af
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
	-H "Authorization: Bearer af4fbacdafb85525468ff418af56a187d54f951427e4de08ac6a6c858d9af7af"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 303f28165a9762bd0296d43f307355e03b1e4dd0a83ce71bfbaa7497110d9108
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
	-H "Authorization: Bearer 303f28165a9762bd0296d43f307355e03b1e4dd0a83ce71bfbaa7497110d9108"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer eb1e8a85e52969840dce3eaa43afdccdd9e88bb05d9db8ba5f596ce388d798c4
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
	-H "Authorization: Bearer eb1e8a85e52969840dce3eaa43afdccdd9e88bb05d9db8ba5f596ce388d798c4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c33438ffc4d101d72fcebde94bec54bc7f8399cdc334914dec1a534ee7e974ab
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
	-H "Authorization: Bearer c33438ffc4d101d72fcebde94bec54bc7f8399cdc334914dec1a534ee7e974ab"
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
    "creator_id": 331,
    "id": 92,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 92,
    "additional_university_ids": [

    ],
    "discipline_id": 98,
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
    "chapters_updated_at": "2016-12-15T16:49:16.358Z",
    "updated_at": "2016-12-15T16:49:17.600Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 331,
        "chapter_id": 77,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:16.578Z",
        "created_at": "2016-12-15T16:49:16.496Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 331,
        "chapter_id": 78,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:16.879Z",
        "created_at": "2016-12-15T16:49:16.791Z",
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
    "chapters": [
      {
        "id": 77,
        "updated_at": "2016-12-15T16:49:17.549Z",
        "course_id": 92,
        "author_id": 331,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T16:49:16.358Z",
        "questions_updated_at": "2016-12-15T16:49:16.358Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 71",
        "position": 1
      },
      {
        "id": 78,
        "updated_at": "2016-12-15T16:49:17.590Z",
        "course_id": 92,
        "author_id": 331,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T16:49:16.358Z",
        "questions_updated_at": "2016-12-15T16:49:16.358Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 72",
        "position": 2
      }
    ],
    "topic_id": 97,
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
Authorization: Bearer 97e153582c3354d5493d707fa370d506682bdcfd581851df91f4a48bfba63534
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
    "creator_id": 336,
    "id": 93,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 93,
    "additional_university_ids": [

    ],
    "discipline_id": 99,
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
    "chapters_updated_at": "2016-12-15T16:49:17.672Z",
    "updated_at": "2016-12-15T16:49:18.939Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 337,
        "chapter_id": 79,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.716Z",
        "created_at": "2016-12-15T16:49:18.716Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 337,
        "chapter_id": 80,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.791Z",
        "created_at": "2016-12-15T16:49:18.791Z",
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
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 337,
        "chapter_id": 79,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.758Z",
        "created_at": "2016-12-15T16:49:18.758Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 337,
        "chapter_id": 80,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.834Z",
        "created_at": "2016-12-15T16:49:18.834Z",
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
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 337,
        "chapter_id": 79,
        "position": 42,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:17.905Z",
        "created_at": "2016-12-15T16:49:17.820Z",
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
            "id": 94,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 95,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 337,
        "chapter_id": 79,
        "position": 43,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.041Z",
        "created_at": "2016-12-15T16:49:17.964Z",
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
            "id": 96,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 97,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 337,
        "chapter_id": 80,
        "position": 44,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.213Z",
        "created_at": "2016-12-15T16:49:18.123Z",
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
            "id": 98,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 99,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 337,
        "chapter_id": 80,
        "position": 45,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T16:49:18.355Z",
        "created_at": "2016-12-15T16:49:18.276Z",
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
            "id": 100,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 101,
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
        "id": 79,
        "updated_at": "2016-12-15T16:49:18.888Z",
        "course_id": 93,
        "author_id": 336,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T16:49:17.672Z",
        "questions_updated_at": "2016-12-15T16:49:17.672Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 73",
        "position": 1
      },
      {
        "id": 80,
        "updated_at": "2016-12-15T16:49:18.929Z",
        "course_id": 93,
        "author_id": 336,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-15T16:49:17.672Z",
        "questions_updated_at": "2016-12-15T16:49:17.672Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 74",
        "position": 2
      }
    ],
    "topic_id": 98,
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
	-H "Authorization: Bearer 97e153582c3354d5493d707fa370d506682bdcfd581851df91f4a48bfba63534"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/91/pin
Content-Type: application/json
Authorization: Bearer 6d40bc851961b5edb39652f34b13c50afd3fc4074ab2cc71ce920bea555b33eb
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/91/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d40bc851961b5edb39652f34b13c50afd3fc4074ab2cc71ce920bea555b33eb"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/96/pin
Content-Type: application/json
Authorization: Bearer bca3cd34bd75af4ea3f9b3fe574aa08aa66a588d4a760659ee04990a9f382c41
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/96/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bca3cd34bd75af4ea3f9b3fe574aa08aa66a588d4a760659ee04990a9f382c41"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4d6e1ad3308f9fb226a000de1ad063041b3777a9d64773e0607c2af0699ff3b4
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
    "creator_id": 380,
    "id": 108,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 108,
    "additional_university_ids": [

    ],
    "discipline_id": 114,
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
    "updated_at": "2016-12-15T16:49:24.489Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 113,
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
	-H "Authorization: Bearer 4d6e1ad3308f9fb226a000de1ad063041b3777a9d64773e0607c2af0699ff3b4"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 13cad43c08af0add46d93fff1a84949fed3e0d59310c1640e44668e2abdaab44
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
    "id": 602,
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
    "created_at": "2016-12-15T16:49:44.192Z",
    "updated_at": "2016-12-15T16:49:44.192Z",
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
	-H "Authorization: Bearer 13cad43c08af0add46d93fff1a84949fed3e0d59310c1640e44668e2abdaab44"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a70dde2f6191a84ddb96958a8bb0b5fed62c02e98bf688d2e2c6b95d959d83da
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[171]}
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
    "id": 604,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      171
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T16:49:44.635Z",
    "updated_at": "2016-12-15T16:49:44.676Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[171]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a70dde2f6191a84ddb96958a8bb0b5fed62c02e98bf688d2e2c6b95d959d83da"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a4f28c467a36dd314ceda4231e147c7e8c84b31a392427e0f2d0bc6b120c70dc
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
    "id": 607,
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
    "created_at": "2016-12-15T16:49:44.857Z",
    "updated_at": "2016-12-15T16:49:44.857Z",
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
	-H "Authorization: Bearer a4f28c467a36dd314ceda4231e147c7e8c84b31a392427e0f2d0bc6b120c70dc"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 84801225e73a9358486395e813cd221b3faa8dc5cf307698c8b5c4d2bce991d3
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[173]}
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
    "id": 606,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      173
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T16:49:44.796Z",
    "updated_at": "2016-12-15T16:49:44.796Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[173]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84801225e73a9358486395e813cd221b3faa8dc5cf307698c8b5c4d2bce991d3"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer f09c0e5ed0dcc8dab0c2bae29ddfb010dbd4c7a4200b9af0d9a6a6fcb537f5b4
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

170
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
    "id": 603,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/703985722db14b47efaafc34043890788523bd43.jpg",
    "university_id": null,
    "fields_of_study": [
      170
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-15T16:49:44.273Z",
    "updated_at": "2016-12-15T16:49:44.584Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/82685268bd2db7ca78867d25dc00dda5041f768b.jpg",
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

170
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer f09c0e5ed0dcc8dab0c2bae29ddfb010dbd4c7a4200b9af0d9a6a6fcb537f5b4"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 886d15f1b135aed6d84ab0decb86bcaeb9ff5059de677681d4dcbdeff18affb2
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
      "id": 8,
      "bookmarkable_id": 128,
      "bookmarkable_type": "Question"
    },
    {
      "id": 9,
      "bookmarkable_id": 129,
      "bookmarkable_type": "Question"
    },
    {
      "id": 10,
      "bookmarkable_id": 130,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 886d15f1b135aed6d84ab0decb86bcaeb9ff5059de677681d4dcbdeff18affb2"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer f82b2af666f2e3e9b28dd62cb0793251770a45a13e0f5778f1d28c1592abe84c
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
      "creator_id": 777,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-155",
      "html_url": "https://goskive.com/course/mit-course-155",
      "slug": "mit-course-155",
      "university_id": 221,
      "additional_university_ids": [

      ],
      "discipline_id": 231,
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
      "updated_at": "2016-12-15T16:50:00.987Z",
      "shortname": "mit-course-155",
      "topic_id": 230,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 155",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 778,
      "id": 221,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-156",
      "html_url": "https://goskive.com/course/mit-course-156",
      "slug": "mit-course-156",
      "university_id": 222,
      "additional_university_ids": [

      ],
      "discipline_id": 232,
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
      "updated_at": "2016-12-15T16:50:01.116Z",
      "shortname": "mit-course-156",
      "topic_id": 231,
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
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f82b2af666f2e3e9b28dd62cb0793251770a45a13e0f5778f1d28c1592abe84c"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 635bdfbf675e525cc975110ceace24dfcd81055a3ca74ee3f6ad640903664f3b
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
        "created_at": "2016-12-15T16:48:47.654Z",
        "updated_at": "2016-12-15T16:48:47.654Z",
        "file_url": "memory://907b9ff46f896c315c01bd5a2b56e648.pdf",
        "course_id": 1,
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
        "created_at": "2016-12-15T16:48:47.779Z",
        "updated_at": "2016-12-15T16:48:47.779Z",
        "file_url": "memory://1b04c1d4c98d910a85012f1edaf7d793.pdf",
        "course_id": 2,
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
        "created_at": "2016-12-15T16:48:47.900Z",
        "updated_at": "2016-12-15T16:48:47.900Z",
        "file_url": "memory://7acc41003dd5dcd3b587412b9ffdd0a4.pdf",
        "course_id": 3,
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
	-H "Authorization: Bearer 635bdfbf675e525cc975110ceace24dfcd81055a3ca74ee3f6ad640903664f3b"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 5afc0ca061658eaba590b0323a1e11ce6fb093faeab9de27ffde512c8743fe29
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
        "updated_at": "2016-12-15T16:50:14.856Z"
      },
      "created_at": "2016-12-15T16:50:14.860Z",
      "updated_at": "2016-12-15T16:50:14.860Z",
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
        "updated_at": "2016-12-15T16:50:14.868Z"
      },
      "created_at": "2016-12-15T16:50:14.871Z",
      "updated_at": "2016-12-15T16:50:14.871Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5afc0ca061658eaba590b0323a1e11ce6fb093faeab9de27ffde512c8743fe29"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer e2fcf5113a85ce682f9a732858ab0841faba9127819f2b6bcb25b0ac9dd09c57
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
      "created_at": "2016-12-15T16:49:58.148Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 17,
      "updated_at": "2016-12-15T16:49:58.304Z",
      "author_id": "743",
      "thread_subject_id": "211",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 19,
      "created_at": "2016-12-15T16:49:58.292Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 18,
      "updated_at": "2016-12-15T16:49:58.307Z",
      "author_id": "746",
      "thread_subject_id": "212",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-12-15T16:49:58.707Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-12-15T16:49:58.707Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 21,
      "created_at": "2016-12-15T16:49:59.166Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-12-15T16:49:59.166Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 22,
      "created_at": "2016-12-15T16:49:59.552Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-12-15T16:49:59.552Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 23,
      "created_at": "2016-12-15T16:49:59.850Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 117,
      "updated_at": "2016-12-15T16:49:59.850Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-12-15T16:50:00.157Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 118,
      "updated_at": "2016-12-15T16:50:00.157Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-12-15T16:50:00.461Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 119,
      "updated_at": "2016-12-15T16:50:00.461Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2fcf5113a85ce682f9a732858ab0841faba9127819f2b6bcb25b0ac9dd09c57"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/26
Content-Type: application/json
Authorization: Bearer 7c08b50534c8683158f10ea530635d4e21e7d8312611e19cba4c4ab00626b1e8
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-15T16:40:00.000Z"}}
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
    "id": 26,
    "created_at": "2016-12-15T16:50:00.699Z",
    "read_at": "2016-12-15T16:40:00.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 19,
    "updated_at": "2016-12-15T16:50:00.739Z",
    "author_id": "772",
    "thread_subject_id": "219",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/26" -d '{"notification":{"read_at":"2016-12-15T16:40:00.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c08b50534c8683158f10ea530635d4e21e7d8312611e19cba4c4ab00626b1e8"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer f72e05d16704934b33015c3945627552f47f052ff03f730eaa8acbeabccdba24
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
      "course_id": 54,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T16:49:06.296Z",
      "course_published": true,
      "updated_at": "2016-12-15T16:49:06.291Z"
    },
    {
      "id": 4,
      "course_id": 55,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-15T16:49:06.423Z",
      "course_published": true,
      "updated_at": "2016-12-15T16:49:06.418Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f72e05d16704934b33015c3945627552f47f052ff03f730eaa8acbeabccdba24"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer b170e66ce399ad33974ace4730542938d063d0cc32ffa5a58b46e71aba4f916f
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
    "course_id": 53,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-15T16:49:06.119Z",
    "course_published": true,
    "updated_at": "2016-12-15T16:49:06.114Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b170e66ce399ad33974ace4730542938d063d0cc32ffa5a58b46e71aba4f916f"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer a661a53034c3215d57b58899934d691b1a875cd6bcc2b1c399fa7b54579a5ac2
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
    "course_id": 56,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-15T16:49:06.688Z",
    "course_published": true,
    "updated_at": "2016-12-15T16:49:06.680Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a661a53034c3215d57b58899934d691b1a875cd6bcc2b1c399fa7b54579a5ac2"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 58fec6bc47d3b62968b8bf0c4eb5749faf02c1cd535f65541143baf8b1a6fdde
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
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 124,
      "user_id": 956
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 125,
      "user_id": 956
    },
    {
      "id": 22,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 126,
      "user_id": 956
    },
    {
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 127,
      "user_id": 956
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58fec6bc47d3b62968b8bf0c4eb5749faf02c1cd535f65541143baf8b1a6fdde"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/10
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
    "id": 10,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 10,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 10
      },
      {
        "id": 11,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 10
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/10" -X GET \
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
      "id": 11,
      "name": "Intuitive regional model",
      "name_translations": {
        "en": "Intuitive regional model"
      }
    },
    {
      "id": 12,
      "name": "Innovative bi-directional knowledge base",
      "name_translations": {
        "en": "Innovative bi-directional knowledge base"
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
PATCH /v2/feedbacks/2/close
Content-Type: application/json
Authorization: Bearer d92888b8cf17e3260217ac1193ad8dc2fe6342b0deee6251af1401a14e3735d6
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
    "id": 2,
    "user_id": 37,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-15T16:48:52.081Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d92888b8cf17e3260217ac1193ad8dc2fe6342b0deee6251af1401a14e3735d6"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/7/fix
Content-Type: application/json
Authorization: Bearer 54c1070a5e8a77d6da3fedd883a0f92986f1c146d5b24a6679144f36adfc6d8f
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
    "id": 7,
    "user_id": 64,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-15T16:48:53.991Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/7/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54c1070a5e8a77d6da3fedd883a0f92986f1c146d5b24a6679144f36adfc6d8f"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/4
Content-Type: application/json
Authorization: Bearer e2a847dfaf014c2c7b28264b512806a0bf70de14caf83984af2e1e16591138bf
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
    "id": 4,
    "user_id": 47,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T16:48:53.067Z",
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
curl "api.goskive.com/v2/feedbacks/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2a847dfaf014c2c7b28264b512806a0bf70de14caf83984af2e1e16591138bf"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/close
Content-Type: application/json
Authorization: Bearer d58badbb9a34b6e5f17178f503eb64b943d1ce7e7ef60ac59d8347ee06552535
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
	-H "Authorization: Bearer d58badbb9a34b6e5f17178f503eb64b943d1ce7e7ef60ac59d8347ee06552535"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/6/fix
Content-Type: application/json
Authorization: Bearer 59ea5db964770dec71292cf18514d4c1d0716f7ddccb7b016bf71515ed724155
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
curl "api.goskive.com/v2/feedbacks/6/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59ea5db964770dec71292cf18514d4c1d0716f7ddccb7b016bf71515ed724155"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/9/fix
Content-Type: application/json
Authorization: Bearer ad9dc194107919b78d87256525ac933162867532c98e2f3adeae78bce67379c4
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
	-H "Authorization: Bearer ad9dc194107919b78d87256525ac933162867532c98e2f3adeae78bce67379c4"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer e38b0854fc1d939e761ace12f82536479a8e899da95313d4db7ebb018785731e
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
    "id": 5,
    "user_id": 52,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T16:48:53.482Z",
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
curl "api.goskive.com/v2/feedbacks/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e38b0854fc1d939e761ace12f82536479a8e899da95313d4db7ebb018785731e"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/20
Content-Type: application/json
Authorization: Bearer eb5f272ea04b45a899ce0a227e96ee5f8cc382b9da50c602ff923f20f2110eca
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
	-H "Authorization: Bearer eb5f272ea04b45a899ce0a227e96ee5f8cc382b9da50c602ff923f20f2110eca"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/15/bookmark
Content-Type: application/json
Authorization: Bearer fd70080400ed0a7b1db8372b46073778db0d6aaeb0c458f0041e49c37c51c3d9
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd70080400ed0a7b1db8372b46073778db0d6aaeb0c458f0041e49c37c51c3d9"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer 0265cc65801f4c7a4876298902d22f61dd4e88a66b00805b283fe673c9192757
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
	-H "Authorization: Bearer 0265cc65801f4c7a4876298902d22f61dd4e88a66b00805b283fe673c9192757"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/21
Content-Type: application/json
Authorization: Bearer ebed04c13fbce94b173713c823c1d2382af932dde944ac1e4a5830fbb4ce0fca
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b6f8812074e81d933ef0a47ad5b43a98.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T164956Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=115b853e06e9ae01bda54925762382030c3f51127f028d02a839dd26bc35fd37",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebed04c13fbce94b173713c823c1d2382af932dde944ac1e4a5830fbb4ce0fca"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/10/preview
Content-Type: application/json
Authorization: Bearer 2677c90f528bd0aed8f20570c69cd0168e3c61eb0a9cd0c771c01b34847e1e60
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/682cb2d6c8033cf53f861f889c761cd4.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161215%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161215T164954Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=e6c548fae3cae26562db8244c3c718af06bf7914fa636dd939433bb07ef75ad9",
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
	-H "Authorization: Bearer 2677c90f528bd0aed8f20570c69cd0168e3c61eb0a9cd0c771c01b34847e1e60"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer f164079d4c29bc7872779bf5442a6a3c734cca3f5b142150f892b6ccb3cd8c02
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
    "id": 12,
    "uploader": {
      "id": 705,
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
      "created_at": "2016-12-15T16:49:54.793Z",
      "updated_at": "2016-12-15T16:49:54.793Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-15T16:49:54.921Z",
    "updated_at": "2016-12-15T16:49:54.921Z",
    "course_id": 196,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f164079d4c29bc7872779bf5442a6a3c734cca3f5b142150f892b6ccb3cd8c02"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/4/matched_courses?required_cu_count=2
Authorization: Bearer 9490acbab581fa7653a74d0c98fb783b97184979e779acd53916c4c93872cb79
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
      "creator_id": 406,
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 115,
      "additional_university_ids": [

      ],
      "discipline_id": 121,
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
      "chapters_updated_at": "2016-12-15T16:49:26.253Z",
      "updated_at": "2016-12-15T16:49:27.449Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 120,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 411,
      "id": 116,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-12440920-251c-4d00-9fb6-4311653429e8",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-12440920-251c-4d00-9fb6-4311653429e8",
      "slug": "mit-the-great-british-bake-off-12440920-251c-4d00-9fb6-4311653429e8",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "discipline_id": 122,
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
      "chapters_updated_at": "2016-12-15T16:49:26.253Z",
      "updated_at": "2016-12-15T16:49:27.861Z",
      "shortname": "mit-the-great-british-bake-off-12440920-251c-4d00-9fb6-4311653429e8",
      "topic_id": 121,
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
curl "api.goskive.com/v2/files/4/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 9490acbab581fa7653a74d0c98fb783b97184979e779acd53916c4c93872cb79"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/17/download
Content-Type: application/json
Authorization: Bearer 26a6b5e4623bcc60c47d4d628ae695046fce6195afb907941a9a7bf361b27596
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26a6b5e4623bcc60c47d4d628ae695046fce6195afb907941a9a7bf361b27596"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/22/report
Content-Type: application/json
Authorization: Bearer 63765bcad09aab5f59c2499bd83ca34d88306209d76f87546db3ef5f3fd3cd96
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63765bcad09aab5f59c2499bd83ca34d88306209d76f87546db3ef5f3fd3cd96"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/11/bookmark
Content-Type: application/json
Authorization: Bearer d5f064f0399776f2b37c974ec0e69f5cbc9f383ac6ab5e7feef43abb962811a6
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
	-H "Authorization: Bearer d5f064f0399776f2b37c974ec0e69f5cbc9f383ac6ab5e7feef43abb962811a6"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/16/upvote
Content-Type: application/json
Authorization: Bearer f3e48e608c81b48372b4469ff6f3ef4796436e697f46cfbf414f09b88f160bfb
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
	-H "Authorization: Bearer f3e48e608c81b48372b4469ff6f3ef4796436e697f46cfbf414f09b88f160bfb"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer fb2d87e42f706a9d15ac84c397a80e68975941e7d689d0ca3a136c20a8229453
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
    "id": 5,
    "author_id": 188,
    "reply_to_id": null,
    "created_at": "2016-12-15T16:49:05.063Z",
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
curl "api.goskive.com/v2/flashcards/13/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb2d87e42f706a9d15ac84c397a80e68975941e7d689d0ca3a136c20a8229453"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer 23bf01bcfdcc63b29047efd0c7a326f650b300614b016bbfc819ae804b65fa57
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
    "id": 4,
    "author_id": 185,
    "reply_to_id": null,
    "created_at": "2016-12-15T16:49:04.587Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 29,
      "user_id": 185,
      "feedbackable_id": 12,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:04.585Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23bf01bcfdcc63b29047efd0c7a326f650b300614b016bbfc819ae804b65fa57"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer 67803978ec2930c37fcabbe55d4ef00c4451677cb3e66ff173e444d0b9f3d816
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
      "id": 3,
      "author_id": 181,
      "reply_to_id": null,
      "created_at": "2016-12-15T16:49:04.051Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 180,
      "reply_to_id": null,
      "created_at": "2016-12-15T16:49:04.034Z",
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
curl "api.goskive.com/v2/flashcards/10/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67803978ec2930c37fcabbe55d4ef00c4451677cb3e66ff173e444d0b9f3d816"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/14/comments
Content-Type: application/json
Authorization: Bearer 040f76ec3cd4dfd527d536714cfd9c424e148f982a7690625467a9faa8f7c294
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
curl "api.goskive.com/v2/flashcards/14/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 040f76ec3cd4dfd527d536714cfd9c424e148f982a7690625467a9faa8f7c294"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/86/feedbacks
Content-Type: application/json
Authorization: Bearer 500d273d6889b97d5920204c6bd9746a202a80de596ef2f2309a6d366f670dd4
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
    "id": 45,
    "user_id": 596,
    "feedbackable_id": 86,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-15T16:49:43.594Z",
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
curl "api.goskive.com/v2/flashcards/86/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 500d273d6889b97d5920204c6bd9746a202a80de596ef2f2309a6d366f670dd4"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/84/feedbacks
Content-Type: application/json
Authorization: Bearer b8d53075df431a6ea1f256c277d272d9835f5e4b8ec503759b8c0c77e6cc06fe
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
      "id": 44,
      "user_id": 592,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:43.116Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 591,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:43.106Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8d53075df431a6ea1f256c277d272d9835f5e4b8ec503759b8c0c77e6cc06fe"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/89/votes
Content-Type: application/json
Authorization: Bearer 5aa63cb4529ce58ace3eb6fffce146805a0d06a6cd37a5819ae2463c316bdf57
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 89,
      "user_id": 790
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 89,
      "user_id": 789
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 89,
      "user_id": 788
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/89/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5aa63cb4529ce58ace3eb6fffce146805a0d06a6cd37a5819ae2463c316bdf57"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/19/republish
Content-Type: application/json
Authorization: Bearer 0ef8d783cb8c3c62667abe8c7c92ace59d12f94b0b6a951a0e1981e076bd76f0
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
curl "api.goskive.com/v2/flashcards/19/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ef8d783cb8c3c62667abe8c7c92ace59d12f94b0b6a951a0e1981e076bd76f0"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/38/bookmark
Content-Type: application/json
Authorization: Bearer 2be83448c1fc0a9511053e225f47112d9f09f777933e8e5a02fb186b8dc6c85c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2be83448c1fc0a9511053e225f47112d9f09f777933e8e5a02fb186b8dc6c85c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/16
Content-Type: application/json
Authorization: Bearer 531ebf9d7809a19d4eeb07dba7da102c3c109d954f041513eda1e9eef2ef0d26
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 531ebf9d7809a19d4eeb07dba7da102c3c109d954f041513eda1e9eef2ef0d26"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/downvote
Content-Type: application/json
Authorization: Bearer d83e5b5765a40c474fc31d1f6a7bd024ecf8fb78c554e2faf590bc5117127173
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d83e5b5765a40c474fc31d1f6a7bd024ecf8fb78c554e2faf590bc5117127173"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/37
Content-Type: application/json
Authorization: Bearer 45a8692e68f1df4096de3490d47729c3a80c342e2d2d127a82dff34a08a6c7a1
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
    "id": 37,
    "obfuscated_id": "95m_4XdR9PU",
    "author_id": 287,
    "chapter_id": 67,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:49:12.718Z",
    "created_at": "2016-12-15T16:49:12.718Z",
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
curl "api.goskive.com/v2/flashcards/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45a8692e68f1df4096de3490d47729c3a80c342e2d2d127a82dff34a08a6c7a1"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/17/report
Content-Type: application/json
Authorization: Bearer 051ef35808fdc17c03b3c497dece12a7ae5ecf4584234a9c2d0dfaeca4b11af5
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 051ef35808fdc17c03b3c497dece12a7ae5ecf4584234a9c2d0dfaeca4b11af5"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/15/bookmark
Content-Type: application/json
Authorization: Bearer f7b9d2bcc584fed96e5257dc08c99eb6d50148bc3fa29121043a9f7c43cde77a
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/15/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7b9d2bcc584fed96e5257dc08c99eb6d50148bc3fa29121043a9f7c43cde77a"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/36/upvote
Content-Type: application/json
Authorization: Bearer bb6bf847d1d05f0bbe7d423c77d35deb3f430e4c0fd2109635cd197c758c8d41
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/36/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb6bf847d1d05f0bbe7d423c77d35deb3f430e4c0fd2109635cd197c758c8d41"
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
    "key": "cache/7ad60ac256b35ef697b123418977f6cd.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0xNVQxNzo0ODo0NloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzdhZDYwYWMyNTZiMzVlZjY5N2IxMjM0MTg5NzdmNmNkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIxNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMTVUMTY0ODQ2WiJ9XX0=",
    "x-amz-credential": "FAKE/20161215/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161215T164846Z",
    "x-amz-signature": "2228ec748bfe4638587e8b22a748b956b6bf78edca7650153dd6c635934fb79d"
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
Authorization: Bearer 76d69427cbc9f55032135fd8abeefe0b0550b3f5adc465534dc8a3357e1458d2
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
	-H "Authorization: Bearer 76d69427cbc9f55032135fd8abeefe0b0550b3f5adc465534dc8a3357e1458d2"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 8a0eb5d4349ee332168d1b2b510b29e5906937eb9d3fb1b352f55a5a019fccb1
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
	-H "Authorization: Bearer 8a0eb5d4349ee332168d1b2b510b29e5906937eb9d3fb1b352f55a5a019fccb1"
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
{"password":{"reset_password_token":"89WSPhPSyxD9st4ZKBAh","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 499,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-15T16:49:34.775Z",
  "updated_at": "2016-12-15T16:49:35.397Z",
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
  "audit_id": 8099
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"89WSPhPSyxD9st4ZKBAh","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/77/comments
Content-Type: application/json
Authorization: Bearer 363e49f0cc65dfd8d420d617d0524e8030239fb0421ffe05afdef3e4eb6cf3ef
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
    "id": 12,
    "author_id": 479,
    "reply_to_id": null,
    "created_at": "2016-12-15T16:49:33.006Z",
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
curl "api.goskive.com/v2/questions/77/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 363e49f0cc65dfd8d420d617d0524e8030239fb0421ffe05afdef3e4eb6cf3ef"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/76/comments
Content-Type: application/json
Authorization: Bearer fb4b2aee3d059c4d639bb8e2d12bf3fec235878cfcb2b1f859dd61095e80bd96
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
    "id": 11,
    "author_id": 476,
    "reply_to_id": null,
    "created_at": "2016-12-15T16:49:32.474Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 476,
      "feedbackable_id": 76,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:32.471Z",
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
curl "api.goskive.com/v2/questions/76/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb4b2aee3d059c4d639bb8e2d12bf3fec235878cfcb2b1f859dd61095e80bd96"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/80/comments
Content-Type: application/json
Authorization: Bearer df8df587f2240b47d1973c2af41dff637c3c8d7a6f0d71102e37f78687e0eff9
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
      "id": 13,
      "author_id": 491,
      "reply_to_id": null,
      "created_at": "2016-12-15T16:49:34.142Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 492,
      "reply_to_id": null,
      "created_at": "2016-12-15T16:49:34.158Z",
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
curl "api.goskive.com/v2/questions/80/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df8df587f2240b47d1973c2af41dff637c3c8d7a6f0d71102e37f78687e0eff9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/78/comments
Content-Type: application/json
Authorization: Bearer 4e542535759153dd5cd1b999b986571a4356f5b77b3b20d68eefbae17267371b
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
curl "api.goskive.com/v2/questions/78/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e542535759153dd5cd1b999b986571a4356f5b77b3b20d68eefbae17267371b"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/32/feedbacks
Content-Type: application/json
Authorization: Bearer 28e05f5eaabf4f5fa5bf24a61324f2abf91a79cb7824338a650a7ea76234197c
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
    "id": 30,
    "user_id": 293,
    "feedbackable_id": 32,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-15T16:49:13.351Z",
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
curl "api.goskive.com/v2/questions/32/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28e05f5eaabf4f5fa5bf24a61324f2abf91a79cb7824338a650a7ea76234197c"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/38/feedbacks
Content-Type: application/json
Authorization: Bearer 16ec5cd4793251c995ba651c372e7dfe1e112d4254fb843736f6f62807f5cef7
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
      "id": 37,
      "user_id": 325,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:15.837Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 324,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T16:49:15.827Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/38/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16ec5cd4793251c995ba651c372e7dfe1e112d4254fb843736f6f62807f5cef7"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/67/votes
Content-Type: application/json
Authorization: Bearer 82f8e877d6e2339fd73368dc19f85a76e606f58ffcfd11388617f044c4e9b99c
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
      "id": 9,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 67,
      "user_id": 391
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 67,
      "user_id": 390
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 67,
      "user_id": 389
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/67/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82f8e877d6e2339fd73368dc19f85a76e606f58ffcfd11388617f044c4e9b99c"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/91/republish
Content-Type: application/json
Authorization: Bearer a9768714f8666c191f82c50dda38fcd3b2de428c6675c70ed8becfffc7dd2757
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
curl "api.goskive.com/v2/questions/91/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9768714f8666c191f82c50dda38fcd3b2de428c6675c70ed8becfffc7dd2757"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/112/bookmark
Content-Type: application/json
Authorization: Bearer 6954b72b9d9f8c46c734a4bd5f40336e81af9cc051b36733c776c1f1effc4268
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/112/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6954b72b9d9f8c46c734a4bd5f40336e81af9cc051b36733c776c1f1effc4268"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/113
Content-Type: application/json
Authorization: Bearer 0a7c33fc1ce3eb2f0ca4da599510cc39ecd908908fa3f72f5fdbb9dd018f45d1
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/113" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a7c33fc1ce3eb2f0ca4da599510cc39ecd908908fa3f72f5fdbb9dd018f45d1"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/89/downvote
Content-Type: application/json
Authorization: Bearer e8dd09655b9bc955d93a4882edcbf46c03ced3966e5fbc435c6fc8c32023080f
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/89/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8dd09655b9bc955d93a4882edcbf46c03ced3966e5fbc435c6fc8c32023080f"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/92
Content-Type: application/json
Authorization: Bearer 78f4f9acca2f412ed473da603bdbd368cb15d2a37090d4ec825cd7fcd5f66b0b
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
    "id": 92,
    "obfuscated_id": "__OphzZQiQY",
    "author_id": 617,
    "chapter_id": 147,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:49:46.158Z",
    "created_at": "2016-12-15T16:49:46.073Z",
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
        "id": 186,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 187,
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
curl "api.goskive.com/v2/questions/92" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78f4f9acca2f412ed473da603bdbd368cb15d2a37090d4ec825cd7fcd5f66b0b"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/95/report
Content-Type: application/json
Authorization: Bearer b4c4092b979e5b78f8a1ceeb72ac5ae438d4dc5dbc9000a1d911a2178cbf2daf
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/95/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4c4092b979e5b78f8a1ceeb72ac5ae438d4dc5dbc9000a1d911a2178cbf2daf"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/93/bookmark
Content-Type: application/json
Authorization: Bearer f8f8ebb69fc18b66a863671824c9161129e3f17378b40b5d31297a631a6fe08f
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/93/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8f8ebb69fc18b66a863671824c9161129e3f17378b40b5d31297a631a6fe08f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/94
Content-Type: application/json
Authorization: Bearer 76f6cdc0124e364d703dc2010941183f3a63d45657f7237393f6050686530638
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":94,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T16:49:46.722Z","updated_at":"2016-12-15T16:49:46.807Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":149,"author_id":623,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 94,
    "obfuscated_id": "CVi6VU_nV6k",
    "author_id": 623,
    "chapter_id": 149,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-15T16:49:46.896Z",
    "created_at": "2016-12-15T16:49:46.722Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x0000000f7ee550>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 192,
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
curl "api.goskive.com/v2/questions/94" -d '{"question":{"question":{"id":94,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-15T16:49:46.722Z","updated_at":"2016-12-15T16:49:46.807Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":149,"author_id":623,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76f6cdc0124e364d703dc2010941183f3a63d45657f7237393f6050686530638"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/111/upvote
Content-Type: application/json
Authorization: Bearer be0d568d17fd060065ef223bd9c68dbffb68bf1371c3a329bfa0479b7ea763e9
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be0d568d17fd060065ef223bd9c68dbffb68bf1371c3a329bfa0479b7ea763e9"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 3ad683fdd7963b683e62329a90d919102be24e240ad3aac494482d6044680a66
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
      "creator_id": 738,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 210,
      "additional_university_ids": [

      ],
      "discipline_id": 219,
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
      "updated_at": "2016-12-15T16:49:57.719Z",
      "shortname": "mit-pizza-201",
      "topic_id": 218,
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
	-H "Authorization: Bearer 3ad683fdd7963b683e62329a90d919102be24e240ad3aac494482d6044680a66"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer eb90108174402e4b22889ff81bf857e66400a2b525d1dc0fcb8b5da317353d39
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
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-208",
      "html_url": "https://goskive.com/university/uni-208",
      "slug": "uni-208",
      "name": "National School of Pizza",
      "short_name": "Uni 208",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/9205692782283b6f5094d9205875587a.jpg",
      "image_url_small": "memory://universities/24aecdd1898165ec7cd74c60c24fc469.jpg",
      "image_thumb_url": "memory://universities/11300b76001e7406c68a21cc9bc90501.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T16:49:57.438Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-207",
      "html_url": "https://goskive.com/university/uni-207",
      "slug": "uni-207",
      "name": "National School of Pastry",
      "short_name": "Uni 207",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/de3f373b430a883c410cf3061c4c23b5.jpg",
      "image_url_small": "memory://universities/9a6c6a1b985b4a1abbc82d767f10a7bd.jpg",
      "image_thumb_url": "memory://universities/5ee2d80971a722f62a253580746ef81c.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T16:49:57.366Z",
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
	-H "Authorization: Bearer eb90108174402e4b22889ff81bf857e66400a2b525d1dc0fcb8b5da317353d39"
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
      "name": "Secured bi-directional flexibility",
      "name_translations": {
        "en": "Secured bi-directional flexibility"
      },
      "discipline_id": 63
    },
    {
      "id": 63,
      "name": "Managed fresh-thinking forecast",
      "name_translations": {
        "en": "Managed fresh-thinking forecast"
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
GET /v2/topics/61
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
    "id": 61,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 62
  }
}
```



```shell
curl "api.goskive.com/v2/topics/61" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 4fa25bb2d5e70349d9c10dd18959a1e929592b88437b171f03421f79f8e7a8ee
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
      "id": 287,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-267",
      "html_url": "https://goskive.com/university/uni-267",
      "slug": "uni-267",
      "name": "University 207",
      "short_name": "Uni 267",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/4003a960443e34ca568a24bfd0cd1386.jpg",
      "image_url_small": "memory://universities/09a5cabecf88cb1715275a7ab241f255.jpg",
      "image_thumb_url": "memory://universities/c35508bcbe4b55d26acab3ce3e12f594.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T16:50:13.943Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 288,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-268",
      "html_url": "https://goskive.com/university/uni-268",
      "slug": "uni-268",
      "name": "University 208",
      "short_name": "Uni 268",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/f3cfa21747fb9079f85ea303cf9e2eed.jpg",
      "image_url_small": "memory://universities/c09cb65522224972c0c451ce82b3aa6e.jpg",
      "image_thumb_url": "memory://universities/af4d374f23cb58179ca71824101c566c.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T16:50:14.009Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 289,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-269",
      "html_url": "https://goskive.com/university/uni-269",
      "slug": "uni-269",
      "name": "University 209",
      "short_name": "Uni 269",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/2983f86eb4ebceaa7cebb1fcf5ab8641.jpg",
      "image_url_small": "memory://universities/8d2cff313ba9bcb8daa9a5eb9e229e90.jpg",
      "image_thumb_url": "memory://universities/fa15a3c712e9b8de5b209504998fae0a.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-15T16:50:14.075Z",
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
	-H "Authorization: Bearer 4fa25bb2d5e70349d9c10dd18959a1e929592b88437b171f03421f79f8e7a8ee"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1f7b29ab6f2af23d75970937f77069e67afcbfabfaa9cb1d10d8890b9c388354
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
    "id": 286,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/e9d554fb2a9c92a1b7cd49490a0926ab.jpg",
    "image_url_small": "memory://universities/5ece9e44c10aae96b4970d4a6b8ea128.jpg",
    "image_thumb_url": "memory://universities/0dd1b9444ac794ab16b7e8a89d6d764d.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-15T16:50:13.833Z",
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
	-H "Authorization: Bearer 1f7b29ab6f2af23d75970937f77069e67afcbfabfaa9cb1d10d8890b9c388354"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 89700c9c9558209a12d18db7469dc5c4889e55243aeecac583028466d4161a6a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":314,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 936,
    "id": 304,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 283,
    "additional_university_ids": [

    ],
    "discipline_id": 315,
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
    "chapters_updated_at": "2016-12-15T16:50:13.138Z",
    "updated_at": "2016-12-15T16:50:13.338Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 182,
        "updated_at": "2016-12-15T16:50:13.327Z",
        "course_id": 304,
        "author_id": 936,
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
        "id": 183,
        "updated_at": "2016-12-15T16:50:13.340Z",
        "course_id": 304,
        "author_id": 936,
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
        "id": 184,
        "updated_at": "2016-12-15T16:50:13.353Z",
        "course_id": 304,
        "author_id": 936,
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
    "topic_id": 314,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":314,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89700c9c9558209a12d18db7469dc5c4889e55243aeecac583028466d4161a6a"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f1bc229b8bec514743a1df7d2b5376d19326c172fad95eefec14fb36666ed723
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":315,"published":false}}
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
    "creator_id": 937,
    "id": 305,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 284,
    "additional_university_ids": [

    ],
    "discipline_id": 316,
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
    "updated_at": "2016-12-15T16:50:13.601Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 315,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":315,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1bc229b8bec514743a1df7d2b5376d19326c172fad95eefec14fb36666ed723"
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
      "creator_id": 894,
      "id": 268,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 267,
      "additional_university_ids": [

      ],
      "discipline_id": 279,
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
      "updated_at": "2016-12-15T16:50:08.817Z",
      "shortname": "fu-course-203",
      "topic_id": 278,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 894,
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-204",
      "html_url": "https://goskive.com/course/fu-course-204",
      "slug": "fu-course-204",
      "university_id": 267,
      "additional_university_ids": [

      ],
      "discipline_id": 280,
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
      "chapters_updated_at": "2016-12-15T16:50:08.640Z",
      "updated_at": "2016-12-15T16:50:09.074Z",
      "shortname": "fu-course-204",
      "topic_id": 279,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 204",
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
Authorization: Bearer d3960bda8116ade2215df77f302b2e2feff7fbf7081b992f5ca6b52dda019231
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
      "creator_id": 921,
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-227",
      "html_url": "https://goskive.com/course/fu-course-227",
      "slug": "fu-course-227",
      "university_id": 276,
      "additional_university_ids": [

      ],
      "discipline_id": 303,
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
      "updated_at": "2016-12-15T16:50:11.582Z",
      "shortname": "fu-course-227",
      "topic_id": 302,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 227",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 921,
      "id": 293,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-228",
      "html_url": "https://goskive.com/course/fu-course-228",
      "slug": "fu-course-228",
      "university_id": 276,
      "additional_university_ids": [

      ],
      "discipline_id": 304,
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
      "chapters_updated_at": "2016-12-15T16:50:11.402Z",
      "updated_at": "2016-12-15T16:50:11.837Z",
      "shortname": "fu-course-228",
      "topic_id": 303,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 228",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3960bda8116ade2215df77f302b2e2feff7fbf7081b992f5ca6b52dda019231"
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
      "creator_id": 899,
      "id": 272,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-207",
      "html_url": "https://goskive.com/course/fu-course-207",
      "slug": "fu-course-207",
      "university_id": 269,
      "additional_university_ids": [

      ],
      "discipline_id": 283,
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
      "updated_at": "2016-12-15T16:50:09.377Z",
      "shortname": "fu-course-207",
      "topic_id": 282,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 207",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 899,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-208",
      "html_url": "https://goskive.com/course/fu-course-208",
      "slug": "fu-course-208",
      "university_id": 269,
      "additional_university_ids": [

      ],
      "discipline_id": 284,
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
      "updated_at": "2016-12-15T16:50:09.411Z",
      "shortname": "fu-course-208",
      "topic_id": 283,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 208",
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
Authorization: Bearer fc1c2230ffaaf90fb43fa5f3b154ab2de171b3fb851467c81ba89d5abf0ef5e4
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
      "creator_id": 927,
      "id": 296,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-231",
      "html_url": "https://goskive.com/course/fu-course-231",
      "slug": "fu-course-231",
      "university_id": 277,
      "additional_university_ids": [

      ],
      "discipline_id": 307,
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
      "updated_at": "2016-12-15T16:50:12.139Z",
      "shortname": "fu-course-231",
      "topic_id": 306,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 231",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 927,
      "id": 297,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-232",
      "html_url": "https://goskive.com/course/fu-course-232",
      "slug": "fu-course-232",
      "university_id": 277,
      "additional_university_ids": [

      ],
      "discipline_id": 308,
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
      "updated_at": "2016-12-15T16:50:12.173Z",
      "shortname": "fu-course-232",
      "topic_id": 307,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 232",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc1c2230ffaaf90fb43fa5f3b154ab2de171b3fb851467c81ba89d5abf0ef5e4"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer d4c76a323b406a56080327cde07f087d82a5f16f03f3fac7a79b14f4478b07c6
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
  "id": 395,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-15T16:49:26.074Z",
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
	-H "Authorization: Bearer d4c76a323b406a56080327cde07f087d82a5f16f03f3fac7a79b14f4478b07c6"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/951
Content-Type: application/json
Authorization: Bearer 6ee988083bf26d940932a9d362a1351488ceea889c8da58edfb1736b44313f9d
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
    "id": 951,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 291,
    "fields_of_study": [
      317,
      318
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-15T16:50:15.157Z",
    "updated_at": "2016-12-15T16:50:15.157Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/951" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ee988083bf26d940932a9d362a1351488ceea889c8da58edfb1736b44313f9d"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/953
Content-Type: application/json
Authorization: Bearer 56f4e2c46c4dc2ff0db6bfd5e6d992d9354b507aec8419139d01d789b5fb5a9d
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
    "id": 953,
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
    "created_at": "2016-12-15T16:50:15.244Z",
    "updated_at": "2016-12-15T16:50:15.244Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/953" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56f4e2c46c4dc2ff0db6bfd5e6d992d9354b507aec8419139d01d789b5fb5a9d"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/3
Content-Type: application/json
Authorization: Bearer 1e3d9d8d505264dcb5f2f7c8ee0422a542598dee673c2dbdbbb4b3e10c61bb27
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
	-H "Authorization: Bearer 1e3d9d8d505264dcb5f2f7c8ee0422a542598dee673c2dbdbbb4b3e10c61bb27"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/2
Content-Type: application/json
Authorization: Bearer fe29b8e6a4bd7f4eb0032f2af5fed3c351cce6a41e567c25f2208a4466690b22
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
    "id": 2,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 28,
    "user_id": 169
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe29b8e6a4bd7f4eb0032f2af5fed3c351cce6a41e567c25f2208a4466690b22"
```
