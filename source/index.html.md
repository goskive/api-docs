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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"088c4056a30379a6d8b863e845a4d54c8c5660617c9b0a028b259464ebff7af6","client_secret":"85b32f1595ffe25bdba846943dfd77b28233e0c8b8258420adc4698bdc5e57b7"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"088c4056a30379a6d8b863e845a4d54c8c5660617c9b0a028b259464ebff7af6","client_secret":"85b32f1595ffe25bdba846943dfd77b28233e0c8b8258420adc4698bdc5e57b7"}' -X POST \
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
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YzhlNDllODI5MTNhZThlZWZiZmEzMjkzNTk2MWQzZTgzNTQ2MmFjNjg3MzRm
ZjM2Njg2Y2NjYmQ3MDdiOGJmODo2MGU2ZTcyNTBkNTJkMDcxODY4N2IyYjBk
ZWQ1Nzc0MjEyZDY3YjQxMzdmN2Y3OTk3NDRhN2JlMjU4N2UwMWZh

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
	-u c8e49e82913ae8eefbfa32935961d3e835462ac68734ff36686cccbd707b8bf8:60e6e7250d52d0718687b2b0ded5774212d67b4137f7f799744a7be2587e01fa
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9980a5cf5ae5fa9822ff3d21e03aa5002588b8e7699e7b9a09641e6f70c7ce4b","client_secret":"29403967de5a553fa479502486e3006e178e580fad3cb3f4931a4d4e107c2252"}
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
  "access_token": "f756016e0e540b2d78796d7a142dabb378e0b31fe8ea73bf6dadc12502827190",
  "token_type": "bearer",
  "created_at": 1481220627
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"9980a5cf5ae5fa9822ff3d21e03aa5002588b8e7699e7b9a09641e6f70c7ce4b","client_secret":"29403967de5a553fa479502486e3006e178e580fad3cb3f4931a4d4e107c2252"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic Njk1NTExYzc0MGU3OTBkN2MxZWY0NzRkYzA1YWY4YWMxNTIzMDQzMDUzNTcw
M2IzNTY1YzYwMzJjNzVkMjc4ZTpmZDk3YjYwZGNlYmJiMWI2YWE0YjZmNzg0
ZTQ3MDM3MTI2NGM1NTgxZDE1YzdiOTllODNmZjJkZWUwMGY3YWU3

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
  "access_token": "dc1fa021f2ef7bc1bc68d8b0b9064c5eca7811ffba86f724da09dd1a7fdb5f66",
  "token_type": "bearer",
  "created_at": 1481220627
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 695511c740e790d7c1ef474dc05af8ac15230430535703b3565c6032c75d278e:fd97b60dcebbb1b6aa4b6f784e470371264c5581d15c7b99e83ff2dee00f7ae7
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
{"grant_type":"client_credentials","client_id":"6377102cbd0e56777b57b8c5d3e4dd3f33f7f444f986341a30ae574d999efcb7","client_secret":"e5b59d195a1fdc5a20a24cf0275190657a65db680f289810f4f654a024f8d772"}
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
  "access_token": "292de0d6c76b839f4c423c8f8e4e94bf78f746f6151168f1b61890b61dc689a3",
  "token_type": "bearer",
  "created_at": 1481220627
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"6377102cbd0e56777b57b8c5d3e4dd3f33f7f444f986341a30ae574d999efcb7","client_secret":"e5b59d195a1fdc5a20a24cf0275190657a65db680f289810f4f654a024f8d772"}' -X POST \
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
Authorization: Bearer d272dbf446e080c0b2fe85ba4e6d722bb609d4faef3ff806a1735a44987914a7
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
	-H "Authorization: Bearer d272dbf446e080c0b2fe85ba4e6d722bb609d4faef3ff806a1735a44987914a7"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/146/flashcards
Content-Type: application/json
Authorization: Bearer 99491e332216f12d78897dd962ba0ed8e9131f43990b6bc4892d9497dd287f06
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":146,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 86,
    "obfuscated_id": "7q-2LHZR3Kk",
    "author_id": 766,
    "chapter_id": 146,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:10:24.267Z",
    "created_at": "2016-12-08T18:10:24.267Z",
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
curl "api.goskive.com/v2/chapters/146/flashcards" -d '{"flashcard":{"chapter_id":146,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99491e332216f12d78897dd962ba0ed8e9131f43990b6bc4892d9497dd287f06"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/147/flashcards
Content-Type: application/json
Authorization: Bearer 148da3e7442f844a494bd07c8f79657209d6c8295efa0e4f837ba862b5e0e6e7
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
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 767,
      "chapter_id": 147,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:24.557Z",
      "created_at": "2016-12-08T18:10:24.557Z",
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 767,
      "chapter_id": 147,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:24.597Z",
      "created_at": "2016-12-08T18:10:24.597Z",
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 767,
      "chapter_id": 147,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:10:24.637Z",
      "created_at": "2016-12-08T18:10:24.637Z",
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
curl "api.goskive.com/v2/chapters/147/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 148da3e7442f844a494bd07c8f79657209d6c8295efa0e4f837ba862b5e0e6e7"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/49/questions
Content-Type: application/json
Authorization: Bearer 6c7a5181bb525e5a1a5240b41a75ac1b5ca6e06a1807d29e891bda4338e998aa
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":49,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 265,
    "chapter_id": 49,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:40.582Z",
    "created_at": "2016-12-08T18:09:40.582Z",
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
curl "api.goskive.com/v2/chapters/49/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":49,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c7a5181bb525e5a1a5240b41a75ac1b5ca6e06a1807d29e891bda4338e998aa"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/46/questions
Content-Type: application/json
Authorization: Bearer 9efb517aeb816292cd267612fe213a06b5b4d180ef3738cd998629b7bc414b97
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":46,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 256,
    "chapter_id": 46,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:39.004Z",
    "created_at": "2016-12-08T18:09:39.004Z",
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
curl "api.goskive.com/v2/chapters/46/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":46,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9efb517aeb816292cd267612fe213a06b5b4d180ef3738cd998629b7bc414b97"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/48/questions
Content-Type: application/json
Authorization: Bearer e0b17090bdceed603bbeb3555dffe3d86899ac7a12c895cd989e2a2db6cb1dd4
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":48,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 262,
    "chapter_id": 48,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:40.047Z",
    "created_at": "2016-12-08T18:09:40.047Z",
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
        "id": 64,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 65,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/48/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":48,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0b17090bdceed603bbeb3555dffe3d86899ac7a12c895cd989e2a2db6cb1dd4"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/47/questions
Content-Type: application/json
Authorization: Bearer 34d19df2e1a6b4eaa639f4567344ea1f029fa69b8afc5893364c711de6d0c792
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":47,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 259,
    "chapter_id": 47,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:39.562Z",
    "created_at": "2016-12-08T18:09:39.562Z",
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
        "id": 61,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 62,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 63,
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
curl "api.goskive.com/v2/chapters/47/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":47,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34d19df2e1a6b4eaa639f4567344ea1f029fa69b8afc5893364c711de6d0c792"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/44/questions
Content-Type: application/json
Authorization: Bearer f18d72692b2bcff28236bf4558cde8af792496c089e0c6fffd7cfeb84e21e078
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 247,
      "chapter_id": 44,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:38.243Z",
      "created_at": "2016-12-08T18:09:38.160Z",
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
    },
    {
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 248,
      "chapter_id": 44,
      "position": 28,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:38.386Z",
      "created_at": "2016-12-08T18:09:38.306Z",
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
        }
      ]
    },
    {
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 249,
      "chapter_id": 44,
      "position": 29,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T18:09:38.533Z",
      "created_at": "2016-12-08T18:09:38.450Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/44/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f18d72692b2bcff28236bf4558cde8af792496c089e0c6fffd7cfeb84e21e078"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/104
Content-Type: application/json
Authorization: Bearer 1cfa670f85551d64dfd825bcd4bdc245dd3ab7bd6c502cbd6bab8ff6c507ec16
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
curl "api.goskive.com/v2/chapters/104" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cfa670f85551d64dfd825bcd4bdc245dd3ab7bd6c502cbd6bab8ff6c507ec16"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/105
Content-Type: application/json
Authorization: Bearer 7852b63fff569fe0e6cac9e0a671b492f64516c08083eba1aaa3cbd077db6ca5
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
curl "api.goskive.com/v2/chapters/105" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7852b63fff569fe0e6cac9e0a671b492f64516c08083eba1aaa3cbd077db6ca5"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/102
Content-Type: application/json
Authorization: Bearer 1d3a741468d2ca1bdf2e5246433a66934b86353afe82bb7719bb891ff6dea8fd
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
curl "api.goskive.com/v2/chapters/102" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d3a741468d2ca1bdf2e5246433a66934b86353afe82bb7719bb891ff6dea8fd"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/103
Content-Type: application/json
Authorization: Bearer 006718c84a0870dff46f76870e2a5b14b00ce04d3077130e314696ac7327d1f2
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/103" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 006718c84a0870dff46f76870e2a5b14b00ce04d3077130e314696ac7327d1f2"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/108
Content-Type: application/json
Authorization: Bearer 66478273f22b6854227c0bd6e61f9b626d02e73417d62be195a8f4f3127ee3f0
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
    "id": 108,
    "updated_at": "2016-12-08T18:10:14.181Z",
    "course_id": 213,
    "author_id": 613,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-08T18:10:13.674Z",
    "questions_updated_at": "2016-12-08T18:10:13.674Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 617,
        "chapter_id": 108,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:14.163Z",
        "created_at": "2016-12-08T18:10:14.163Z",
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
        "id": 103,
        "obfuscated_id": "AVhVflMAvL0",
        "author_id": 615,
        "chapter_id": 108,
        "position": 90,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:14.054Z",
        "created_at": "2016-12-08T18:10:13.968Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/108" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66478273f22b6854227c0bd6e61f9b626d02e73417d62be195a8f4f3127ee3f0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/101
Content-Type: application/json
Authorization: Bearer d85e596cb8d629890e623c77aeb0db50daf06761e491fb3f6b142b17ec7a5d16
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
    "id": 101,
    "updated_at": "2016-12-08T18:10:11.908Z",
    "course_id": 206,
    "author_id": 589,
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
curl "api.goskive.com/v2/chapters/101" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d85e596cb8d629890e623c77aeb0db50daf06761e491fb3f6b142b17ec7a5d16"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer 9820ca11d9f7c44b477ba338bc91f9076d037a908a59c6b90ea230034b83612f
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
    "id": 59,
    "author_id": 958,
    "reply_to_id": 58,
    "created_at": "2016-12-08T18:10:41.274Z",
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
curl "api.goskive.com/v2/comments/58/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9820ca11d9f7c44b477ba338bc91f9076d037a908a59c6b90ea230034b83612f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer fb74f1a3b5b422bf7cbdb7e08bb040e012889250221d1b661f118012dda8915f
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
curl "api.goskive.com/v2/comments/60/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb74f1a3b5b422bf7cbdb7e08bb040e012889250221d1b661f118012dda8915f"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/50
Content-Type: application/json
Authorization: Bearer d1e36e14b03ae61395d67e496e5f95b17cd5b4dd7e981a0406ebc07cc9f6ad23
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
curl "api.goskive.com/v2/comments/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1e36e14b03ae61395d67e496e5f95b17cd5b4dd7e981a0406ebc07cc9f6ad23"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/47/republish
Content-Type: application/json
Authorization: Bearer 967806ef8b52ed405fbafdd5836f38a8a492f2f843be16b385ceafb501565fae
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
	-H "Authorization: Bearer 967806ef8b52ed405fbafdd5836f38a8a492f2f843be16b385ceafb501565fae"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 9e2b030313178cb36549bd9a279be2343880eebe2d72d97d1f0ec6789c779a5a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e2b030313178cb36549bd9a279be2343880eebe2d72d97d1f0ec6789c779a5a"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/45/report
Content-Type: application/json
Authorization: Bearer bea79c3791b8b5b2a0e4be0019bd5a82faf9104f571ef8812c023f329c49fb05
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/45/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bea79c3791b8b5b2a0e4be0019bd5a82faf9104f571ef8812c023f329c49fb05"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/12
Content-Type: application/json
Authorization: Bearer be4def4445a1b84d8f5e72241632ec188a7bd4361bf57e442b66db8ab8c8e368
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
    "id": 12,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-08T18:10:23.939Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/12" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be4def4445a1b84d8f5e72241632ec188a7bd4361bf57e442b66db8ab8c8e368"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer b6bc26888b5c6e59ac3347d9e01731f0595bad630e76f510ff3292fdf0c2d528
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
      "id": 9,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:10:23.871Z"
    },
    {
      "id": 10,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:10:23.876Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T18:10:23.880Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6bc26888b5c6e59ac3347d9e01731f0595bad630e76f510ff3292fdf0c2d528"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/26/company_profiles
Content-Type: application/json
Authorization: Bearer 9ca0d5760447483367bfcb59308885217feaeec00b61cd31c33178cc2bf66f9e
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
curl "api.goskive.com/v2/companies/26/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ca0d5760447483367bfcb59308885217feaeec00b61cd31c33178cc2bf66f9e"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 04fab8703f22a0940f3c2b0c8b7f49535a1845f67eb886741a0902220208866c
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
curl "api.goskive.com/v2/companies/25/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04fab8703f22a0940f3c2b0c8b7f49535a1845f67eb886741a0902220208866c"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 3978d4dcba051dd8b21c699583deba676273653a8eb1ec2214af939315f6cad3
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
      "company_id": 19,
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
      "company_id": 22,
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
	-H "Authorization: Bearer 3978d4dcba051dd8b21c699583deba676273653a8eb1ec2214af939315f6cad3"
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
Authorization: Bearer 8f84faecc1c9a9c5efd7550ab01285bdea4678cf9916995d7a55efec80e23fac
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
	-H "Authorization: Bearer 8f84faecc1c9a9c5efd7550ab01285bdea4678cf9916995d7a55efec80e23fac"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 56429c4d0dc1218fd9afe148d4d4a83ef81c8444cf5821d6fc433cdbc5c62a3c
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
    "id": 184,
    "updated_at": "2016-12-08T18:10:38.675Z",
    "course_id": 301,
    "author_id": 929,
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
	-H "Authorization: Bearer 56429c4d0dc1218fd9afe148d4d4a83ef81c8444cf5821d6fc433cdbc5c62a3c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8636fc0f07742e6096b1351984b137326188366eb81cb2c839f12cf90eef0f07
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
      "id": 162,
      "updated_at": "2016-12-08T18:10:35.679Z",
      "course_id": 289,
      "author_id": 881,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 141",
      "position": 1
    },
    {
      "id": 163,
      "updated_at": "2016-12-08T18:10:35.707Z",
      "course_id": 289,
      "author_id": 882,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 142",
      "position": 2
    },
    {
      "id": 164,
      "updated_at": "2016-12-08T18:10:35.924Z",
      "course_id": 289,
      "author_id": 883,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T18:10:35.542Z",
      "questions_updated_at": "2016-12-08T18:10:35.542Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 143",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8636fc0f07742e6096b1351984b137326188366eb81cb2c839f12cf90eef0f07"
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
      "id": 168,
      "updated_at": "2016-12-08T18:10:36.519Z",
      "course_id": 292,
      "author_id": 895,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 147",
      "position": 1
    },
    {
      "id": 169,
      "updated_at": "2016-12-08T18:10:36.546Z",
      "course_id": 292,
      "author_id": 896,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 148",
      "position": 2
    },
    {
      "id": 170,
      "updated_at": "2016-12-08T18:10:36.763Z",
      "course_id": 292,
      "author_id": 897,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T18:10:36.414Z",
      "questions_updated_at": "2016-12-08T18:10:36.414Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 149",
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
Authorization: Bearer fc4bbef794e977366b3fa0b83b66a22fa838adb97adb476067d5deb71407ff52
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
      "id": 165,
      "updated_at": "2016-12-08T18:10:36.129Z",
      "course_id": 290,
      "author_id": 888,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 144",
      "position": 1
    },
    {
      "id": 166,
      "updated_at": "2016-12-08T18:10:36.155Z",
      "course_id": 290,
      "author_id": 889,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 145",
      "position": 2
    },
    {
      "id": 167,
      "updated_at": "2016-12-08T18:10:36.180Z",
      "course_id": 290,
      "author_id": 890,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 146",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc4bbef794e977366b3fa0b83b66a22fa838adb97adb476067d5deb71407ff52"
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
      "id": 171,
      "updated_at": "2016-12-08T18:10:36.922Z",
      "course_id": 293,
      "author_id": 901,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 150",
      "position": 1
    },
    {
      "id": 172,
      "updated_at": "2016-12-08T18:10:36.950Z",
      "course_id": 293,
      "author_id": 902,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 151",
      "position": 2
    },
    {
      "id": 173,
      "updated_at": "2016-12-08T18:10:36.978Z",
      "course_id": 293,
      "author_id": 903,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 152",
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
Authorization: Bearer 6f753dd0094994e9aa855037d5741d8cd1c750ce0d2ac144eb95f44604234a72
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
    "course_id": 287,
    "user_id": 877,
    "updated_at": "2016-12-08T18:10:35.242Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f753dd0094994e9aa855037d5741d8cd1c750ce0d2ac144eb95f44604234a72"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 7358a0fee737d0d35e20f3747abb019a9a4f8902fc81a2552b42cbb0106eca4c
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
      "course_id": 284,
      "user_id": 867,
      "updated_at": "2016-12-08T18:10:34.657Z"
    },
    {
      "id": 2,
      "course_id": 284,
      "user_id": 868,
      "updated_at": "2016-12-08T18:10:34.673Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7358a0fee737d0d35e20f3747abb019a9a4f8902fc81a2552b42cbb0106eca4c"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/134/files
Content-Type: application/json
Authorization: Bearer e52bf385fb50455a2f0850127931d48a5aa007aac0b89cd68f9d0bdc9306ccb2
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
      "id": 14,
      "uploader": {
        "id": 381,
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
        "created_at": "2016-12-08T18:09:52.461Z",
        "updated_at": "2016-12-08T18:09:52.461Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:09:52.472Z",
      "updated_at": "2016-12-08T18:09:52.472Z",
      "course_id": 134,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 15,
      "uploader": {
        "id": 382,
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
        "created_at": "2016-12-08T18:09:52.483Z",
        "updated_at": "2016-12-08T18:09:52.483Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:09:52.492Z",
      "updated_at": "2016-12-08T18:09:52.492Z",
      "course_id": 134,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 16,
      "uploader": {
        "id": 383,
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
        "created_at": "2016-12-08T18:09:52.503Z",
        "updated_at": "2016-12-08T18:09:52.503Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T18:09:52.513Z",
      "updated_at": "2016-12-08T18:09:52.513Z",
      "course_id": 134,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/134/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e52bf385fb50455a2f0850127931d48a5aa007aac0b89cd68f9d0bdc9306ccb2"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/135/files
Content-Type: application/json
Authorization: Bearer 0f1e65b83e4f0d51715664709b81d6315b94da3f3a2e5d6f4e943d5c4c0d7097
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
    "id": 17,
    "uploader": {
      "id": 386,
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
      "created_at": "2016-12-08T18:09:52.671Z",
      "updated_at": "2016-12-08T18:09:52.671Z"
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
    "created_at": "2016-12-08T18:09:52.701Z",
    "updated_at": "2016-12-08T18:09:52.701Z",
    "course_id": 135,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/135/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f1e65b83e4f0d51715664709b81d6315b94da3f3a2e5d6f4e943d5c4c0d7097"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/136/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 4d8bc65fe5439865f1b0dcc9fe45a5edcdbe20e31f0e6c770be6fa699741f62a
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
    "key": "cache/d00fb8524b905abf210be6ca08e1abbd.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxOTowOTo1MloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2QwMGZiODUyNGI5MDVhYmYyMTBiZTZjYTA4ZTFhYmJkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA4VDE4MDk1MloifV19",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T180952Z",
    "x-amz-signature": "757f999adaaef01664317932bfa46f9e63f5cce27921877062c63f5544704eb2"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/136/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d8bc65fe5439865f1b0dcc9fe45a5edcdbe20e31f0e6c770be6fa699741f62a"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 99da138d2f12c7f0e620a0659ed0370a485dd405a19a1f00ce6819d242cedbba
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
	-H "Authorization: Bearer 99da138d2f12c7f0e620a0659ed0370a485dd405a19a1f00ce6819d242cedbba"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 07a7f5115e37060457eb0325dc55c0ed7272cd24f3e993c0b6a2f74806a6f678
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
	-H "Authorization: Bearer 07a7f5115e37060457eb0325dc55c0ed7272cd24f3e993c0b6a2f74806a6f678"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d153aa09aeb5876dec820e8993388d815d15aa30eb90903e4fff5476ec56d3c7
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
	-H "Authorization: Bearer d153aa09aeb5876dec820e8993388d815d15aa30eb90903e4fff5476ec56d3c7"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1989c2a3e82ce53bd590eddda7b6e39ac79c1e0f8c2139e179f539f85895bd8f
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
	-H "Authorization: Bearer 1989c2a3e82ce53bd590eddda7b6e39ac79c1e0f8c2139e179f539f85895bd8f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer df5855962e949a5afdfacd6427a115c4333d9e5f71aa52ddce5013b11602b4d6
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
	-H "Authorization: Bearer df5855962e949a5afdfacd6427a115c4333d9e5f71aa52ddce5013b11602b4d6"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 828772d05cce2c6ca07eaa6173541d82194151657567867790a61c7640891940
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
    "creator_id": 568,
    "id": 202,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 181,
    "additional_university_ids": [

    ],
    "discipline_id": 209,
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
    "chapters_updated_at": "2016-12-08T18:10:07.554Z",
    "updated_at": "2016-12-08T18:10:08.764Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 569,
        "chapter_id": 94,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.540Z",
        "created_at": "2016-12-08T18:10:08.540Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 569,
        "chapter_id": 95,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.616Z",
        "created_at": "2016-12-08T18:10:08.616Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 569,
        "chapter_id": 94,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.583Z",
        "created_at": "2016-12-08T18:10:08.583Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 569,
        "chapter_id": 95,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.659Z",
        "created_at": "2016-12-08T18:10:08.659Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 569,
        "chapter_id": 94,
        "position": 67,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.760Z",
        "created_at": "2016-12-08T18:10:07.679Z",
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
            "id": 163,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 164,
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
        "author_id": 569,
        "chapter_id": 94,
        "position": 68,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:07.892Z",
        "created_at": "2016-12-08T18:10:07.817Z",
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
      },
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 569,
        "chapter_id": 95,
        "position": 69,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.054Z",
        "created_at": "2016-12-08T18:10:07.970Z",
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
            "id": 167,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 168,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 569,
        "chapter_id": 95,
        "position": 70,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:08.193Z",
        "created_at": "2016-12-08T18:10:08.114Z",
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
            "id": 169,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 170,
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
        "id": 94,
        "updated_at": "2016-12-08T18:10:08.712Z",
        "course_id": 202,
        "author_id": 568,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:10:07.554Z",
        "questions_updated_at": "2016-12-08T18:10:07.554Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 85",
        "position": 1
      },
      {
        "id": 95,
        "updated_at": "2016-12-08T18:10:08.753Z",
        "course_id": 202,
        "author_id": 568,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:10:07.554Z",
        "questions_updated_at": "2016-12-08T18:10:07.554Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 86",
        "position": 2
      }
    ],
    "topic_id": 209,
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
	-H "Authorization: Bearer 828772d05cce2c6ca07eaa6173541d82194151657567867790a61c7640891940"
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
    "creator_id": 574,
    "id": 203,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 182,
    "additional_university_ids": [

    ],
    "discipline_id": 210,
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
    "chapters_updated_at": "2016-12-08T18:10:08.916Z",
    "updated_at": "2016-12-08T18:10:10.134Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 574,
        "chapter_id": 96,
        "position": 73,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:09.124Z",
        "created_at": "2016-12-08T18:10:09.041Z",
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
            "id": 175,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 176,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 574,
        "chapter_id": 97,
        "position": 75,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T18:10:09.421Z",
        "created_at": "2016-12-08T18:10:09.336Z",
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
            "id": 179,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 180,
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
        "id": 96,
        "updated_at": "2016-12-08T18:10:10.082Z",
        "course_id": 203,
        "author_id": 574,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:10:08.916Z",
        "questions_updated_at": "2016-12-08T18:10:08.916Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 87",
        "position": 1
      },
      {
        "id": 97,
        "updated_at": "2016-12-08T18:10:10.124Z",
        "course_id": 203,
        "author_id": 574,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T18:10:08.916Z",
        "questions_updated_at": "2016-12-08T18:10:08.916Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 88",
        "position": 2
      }
    ],
    "topic_id": 210,
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
PUT /v2/courses/200/pin
Content-Type: application/json
Authorization: Bearer 8091d7e1da26b1efe51688a2b6589bef5a054e238d7ad96e5818fc7e124d2257
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/200/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8091d7e1da26b1efe51688a2b6589bef5a054e238d7ad96e5818fc7e124d2257"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/199/pin
Content-Type: application/json
Authorization: Bearer e38529ae3ff216e95c0261964df5d71d827b3ed914eefa68f34d0b3fa5097c54
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/199/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e38529ae3ff216e95c0261964df5d71d827b3ed914eefa68f34d0b3fa5097c54"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 66b97f61a8256d4f23f879e01590f62200e590201e3f531b3c1cd64c1e46e731
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
    "creator_id": 533,
    "id": 187,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 166,
    "additional_university_ids": [

    ],
    "discipline_id": 194,
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
    "updated_at": "2016-12-08T18:10:03.814Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 194,
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
	-H "Authorization: Bearer 66b97f61a8256d4f23f879e01590f62200e590201e3f531b3c1cd64c1e46e731"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer ab3c3fc87d5d8b9f2c063c224546fc15bb9f8f0115667d8021a2d4011b5eb99d
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
    "id": 17,
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
    "created_at": "2016-12-08T18:09:15.381Z",
    "updated_at": "2016-12-08T18:09:15.381Z",
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
	-H "Authorization: Bearer ab3c3fc87d5d8b9f2c063c224546fc15bb9f8f0115667d8021a2d4011b5eb99d"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9cfc400bf97338c5fe1a2d2a2979426af807c066e4a3c339846375f507b2381b
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[5]}
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
      5
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:09:15.078Z",
    "updated_at": "2016-12-08T18:09:15.120Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[5]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cfc400bf97338c5fe1a2d2a2979426af807c066e4a3c339846375f507b2381b"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1008e3b8e7f863d0ffd93c826c7141517ba6913d42d53cec2ceeca508e5746b9
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
    "id": 14,
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
    "created_at": "2016-12-08T18:09:15.146Z",
    "updated_at": "2016-12-08T18:09:15.146Z",
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
	-H "Authorization: Bearer 1008e3b8e7f863d0ffd93c826c7141517ba6913d42d53cec2ceeca508e5746b9"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9c8996b9a03c829af39117c378645e32e1c1ae7288fc9d4f2b78b5f8c8758644
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[7]}
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
    "id": 15,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      7
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:09:15.242Z",
    "updated_at": "2016-12-08T18:09:15.242Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[7]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c8996b9a03c829af39117c378645e32e1c1ae7288fc9d4f2b78b5f8c8758644"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer d31c1dcb8ab3af531cba0b206a5453b36df9ff5518a29262db6ced01382d3312
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

4
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
    "id": 12,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/81e4889a7d32467b24496c7d1f3cd6f307cb07e9.jpg",
    "university_id": null,
    "fields_of_study": [
      4
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T18:09:14.768Z",
    "updated_at": "2016-12-08T18:09:15.014Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/3be75877e70cfb7585807843284c76bfd6d85d16.jpg",
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

4
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer d31c1dcb8ab3af531cba0b206a5453b36df9ff5518a29262db6ced01382d3312"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 4fc3657143238e3da9fa10b9ea2fd6b5968ce77fb58d719c787f192208510c3b
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
	-H "Authorization: Bearer 4fc3657143238e3da9fa10b9ea2fd6b5968ce77fb58d719c787f192208510c3b"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer bb1d21ac4c3f18c6414dd547b4e488e8caba9d42e28ab4ad1bd5b67c8135035a
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
	-H "Authorization: Bearer bb1d21ac4c3f18c6414dd547b4e488e8caba9d42e28ab4ad1bd5b67c8135035a"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 30b2be04715801ab25189a1e8c26e4d4529c4afbbe3378b9fc8851af85e7bd1a
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
	-H "Authorization: Bearer 30b2be04715801ab25189a1e8c26e4d4529c4afbbe3378b9fc8851af85e7bd1a"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d9815158d7e88e449d43136535d05ccd51e2621b50ed5abedb534bd6bd07e3fa
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
      "creator_id": 978,
      "id": 312,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-240",
      "html_url": "https://goskive.com/course/mit-course-240",
      "slug": "mit-course-240",
      "university_id": 297,
      "additional_university_ids": [

      ],
      "discipline_id": 325,
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
      "updated_at": "2016-12-08T18:10:43.202Z",
      "shortname": "mit-course-240",
      "topic_id": 324,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 240",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 979,
      "id": 313,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-241",
      "html_url": "https://goskive.com/course/mit-course-241",
      "slug": "mit-course-241",
      "university_id": 298,
      "additional_university_ids": [

      ],
      "discipline_id": 326,
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
      "updated_at": "2016-12-08T18:10:43.310Z",
      "shortname": "mit-course-241",
      "topic_id": 325,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 241",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9815158d7e88e449d43136535d05ccd51e2621b50ed5abedb534bd6bd07e3fa"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer cbfbf01f68515484e06d4e1c0540caecf8420dd64a7b0b0d89e4cb34cbcfb63e
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
        "created_at": "2016-12-08T18:10:27.546Z",
        "updated_at": "2016-12-08T18:10:27.546Z",
        "file_url": "memory://abf822595d2885ee2a8056f4311a316c.pdf",
        "course_id": 263,
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
        "created_at": "2016-12-08T18:10:27.654Z",
        "updated_at": "2016-12-08T18:10:27.654Z",
        "file_url": "memory://14a8ec8f9998e9d3855a9ae11e4681f5.pdf",
        "course_id": 264,
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
        "created_at": "2016-12-08T18:10:27.761Z",
        "updated_at": "2016-12-08T18:10:27.761Z",
        "file_url": "memory://d369a9f6da7b971b6c46d8186765f580.pdf",
        "course_id": 265,
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
	-H "Authorization: Bearer cbfbf01f68515484e06d4e1c0540caecf8420dd64a7b0b0d89e4cb34cbcfb63e"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 75ebeecdda61d185200600e7265e599e313e1c0f2a9b937d2b00548f5e7c07d5
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
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:10:33.559Z"
      },
      "created_at": "2016-12-08T18:10:33.563Z",
      "updated_at": "2016-12-08T18:10:33.563Z",
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
        "name": "Fake Company Name 30",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:10:33.572Z"
      },
      "created_at": "2016-12-08T18:10:33.576Z",
      "updated_at": "2016-12-08T18:10:33.576Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75ebeecdda61d185200600e7265e599e313e1c0f2a9b937d2b00548f5e7c07d5"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cdef9e3b857712d5fb93473d13bc973b6b75333962b6c0060ee621d0ad685a98
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
      "company_id": 29,
      "company": {
        "id": 29,
        "name": "Fake Company Name 25",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/eb30fd9939333e805126ba26a8736769f7ca2ba6.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:10:33.387Z"
      },
      "created_at": "2016-12-08T18:10:33.392Z",
      "updated_at": "2016-12-08T18:10:33.392Z",
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
      "company_id": 30,
      "company": {
        "id": 30,
        "name": "Fake Company Name 26",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T18:10:33.410Z"
      },
      "created_at": "2016-12-08T18:10:33.414Z",
      "updated_at": "2016-12-08T18:10:33.414Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdef9e3b857712d5fb93473d13bc973b6b75333962b6c0060ee621d0ad685a98"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer bde07ff544445af2cc78fbf9c6d98bd7d6abbd9a548edba0ceb95c0452e2ca54
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
      "id": 16,
      "created_at": "2016-12-08T18:10:29.498Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-12-08T18:10:30.718Z",
      "author_id": "822",
      "thread_subject_id": "270",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-12-08T18:10:30.706Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-12-08T18:10:30.722Z",
      "author_id": "825",
      "thread_subject_id": "271",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-12-08T18:10:31.099Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-12-08T18:10:31.099Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-12-08T18:10:31.471Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-12-08T18:10:31.471Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-12-08T18:10:31.845Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-12-08T18:10:31.845Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-12-08T18:10:32.131Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 122,
      "updated_at": "2016-12-08T18:10:32.131Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-12-08T18:10:32.420Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 123,
      "updated_at": "2016-12-08T18:10:32.420Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-12-08T18:10:32.703Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 124,
      "updated_at": "2016-12-08T18:10:32.703Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bde07ff544445af2cc78fbf9c6d98bd7d6abbd9a548edba0ceb95c0452e2ca54"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/24
Content-Type: application/json
Authorization: Bearer f9510649eba3eb2404733b0bf195f2cb49089122cb182204d90c4a3dd936c857
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-08T18:00:32.000Z"}}
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
    "id": 24,
    "created_at": "2016-12-08T18:10:32.956Z",
    "read_at": "2016-12-08T18:00:32.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 57,
    "updated_at": "2016-12-08T18:10:32.997Z",
    "author_id": "851",
    "thread_subject_id": "278",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/24" -d '{"notification":{"read_at":"2016-12-08T18:00:32.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9510649eba3eb2404733b0bf195f2cb49089122cb182204d90c4a3dd936c857"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 3ee8f37cae25617a035ed6ba5670234e3eee8215a2875e2d18d419d3238ffb12
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
      "course_id": 100,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T18:09:41.604Z",
      "course_published": true,
      "updated_at": "2016-12-08T18:09:41.599Z"
    },
    {
      "id": 4,
      "course_id": 101,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T18:09:41.711Z",
      "course_published": true,
      "updated_at": "2016-12-08T18:09:41.707Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ee8f37cae25617a035ed6ba5670234e3eee8215a2875e2d18d419d3238ffb12"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 862bfbdaee0c7ecd2218c7bbcc57777f7bb53fa79f383d6883311b12a7d794a7
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
    "course_id": 102,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T18:09:41.901Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:09:41.897Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 862bfbdaee0c7ecd2218c7bbcc57777f7bb53fa79f383d6883311b12a7d794a7"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 63e35956e7b1dd4a0f442dc2353813b810b41e6d14fc643d662107452aa585b2
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
    "id": 2,
    "course_id": 99,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-08T18:09:41.478Z",
    "course_published": true,
    "updated_at": "2016-12-08T18:09:41.470Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63e35956e7b1dd4a0f442dc2353813b810b41e6d14fc643d662107452aa585b2"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer b075d2d30bbd0fcdb15f2eafe0916b7465e7968342a7e02bea286fad9ad38e3a
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
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 115,
      "user_id": 806
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 116,
      "user_id": 806
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 117,
      "user_id": 806
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 118,
      "user_id": 806
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b075d2d30bbd0fcdb15f2eafe0916b7465e7968342a7e02bea286fad9ad38e3a"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/299
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
    "id": 299,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 299,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 299
      },
      {
        "id": 300,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 299
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/299" -X GET \
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
      "id": 300,
      "name": "Self-enabling cohesive framework",
      "name_translations": {
        "en": "Self-enabling cohesive framework"
      }
    },
    {
      "id": 301,
      "name": "Profound explicit utilisation",
      "name_translations": {
        "en": "Profound explicit utilisation"
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
PATCH /v2/feedbacks/4/close
Content-Type: application/json
Authorization: Bearer da954b33b90e8b4d6700bcdf4caf95a7f6a86fdda3968361310e2535b0eafd90
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
    "id": 4,
    "user_id": 75,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-08T18:09:19.331Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/4/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da954b33b90e8b4d6700bcdf4caf95a7f6a86fdda3968361310e2535b0eafd90"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 8820004df663756872ade23f809e4013b6bd568461f2f1e9e8d0abf9a8891ed4
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
    "user_id": 176,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-08T18:09:26.876Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8820004df663756872ade23f809e4013b6bd568461f2f1e9e8d0abf9a8891ed4"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/1
Content-Type: application/json
Authorization: Bearer 29f1b8d744e995edf30d835851e56f558a5e3564abf77b1d9c9e5c1cb86862c3
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
    "id": 1,
    "user_id": 58,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:09:18.490Z",
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
curl "api.goskive.com/v2/feedbacks/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29f1b8d744e995edf30d835851e56f558a5e3564abf77b1d9c9e5c1cb86862c3"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer ac8aa82705a9e7da8bec8010114b3bcc5dbe134bf729fa1806b3abbc1346f25b
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
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac8aa82705a9e7da8bec8010114b3bcc5dbe134bf729fa1806b3abbc1346f25b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 0602bc42294db695ec382df20bf9c4b0a11c31315559d5f0b9d58a97a9eea4f1
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
	-H "Authorization: Bearer 0602bc42294db695ec382df20bf9c4b0a11c31315559d5f0b9d58a97a9eea4f1"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 6517423b6515ed61deba44f3481e4bc5861b260f7725eb19f53678c79ea1de50
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
	-H "Authorization: Bearer 6517423b6515ed61deba44f3481e4bc5861b260f7725eb19f53678c79ea1de50"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/2
Content-Type: application/json
Authorization: Bearer fbbbe00b7eb9494d82fc2188ebe47de0e970edaa4dcf8dc68e8ffe3af10d0da8
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
    "id": 2,
    "user_id": 63,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:09:18.887Z",
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
curl "api.goskive.com/v2/feedbacks/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbbbe00b7eb9494d82fc2188ebe47de0e970edaa4dcf8dc68e8ffe3af10d0da8"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 54d4d41c9d6add237773e686358a2b2b492d434cd64892fcacde3984663a6a88
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
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54d4d41c9d6add237773e686358a2b2b492d434cd64892fcacde3984663a6a88"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/13/bookmark
Content-Type: application/json
Authorization: Bearer 22086715ed3ef5603ebdb71148a3b2d6e04c4c5c3c4903f5b5edd2e7a29c5e5a
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
	-H "Authorization: Bearer 22086715ed3ef5603ebdb71148a3b2d6e04c4c5c3c4903f5b5edd2e7a29c5e5a"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer f646016ef0ebb5a53261b88cb34ab345b57cbf3997f59a0158cbf37d09955bbd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f646016ef0ebb5a53261b88cb34ab345b57cbf3997f59a0158cbf37d09955bbd"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/5
Content-Type: application/json
Authorization: Bearer 0feb2b9ad136e095080ac679bbc5b9a1a9b695159b4341bdf1b8c498fe9a50be
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/69241085c4c51db8f986fe915a3f1bd7.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T180916Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=a3d7b817918806fbe45b12e02fa8f4c7b6d91926a4b47281f0bf530e6827712b",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0feb2b9ad136e095080ac679bbc5b9a1a9b695159b4341bdf1b8c498fe9a50be"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/12/preview
Content-Type: application/json
Authorization: Bearer 3481d35eecccdd286d821a8c016208bb22d4cde61d5ca0e2b03628139a40b56f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5c9ad89242ebbc9d212cd3bf3fed5ab2.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T180918Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=7e87f532819c4379f59f0de0930524f17324eed68e45b3f0ea933c2aa8622dbf",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/12/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3481d35eecccdd286d821a8c016208bb22d4cde61d5ca0e2b03628139a40b56f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Content-Type: application/json
Authorization: Bearer e97dc3087255e0a93e3ec3adf472d2572c667b8cf9879f392371e81b4af3c2da
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
    "id": 9,
    "uploader": {
      "id": 41,
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
      "created_at": "2016-12-08T18:09:17.388Z",
      "updated_at": "2016-12-08T18:09:17.388Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-08T18:09:17.492Z",
    "updated_at": "2016-12-08T18:09:17.492Z",
    "course_id": 12,
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
curl "api.goskive.com/v2/files/9/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e97dc3087255e0a93e3ec3adf472d2572c667b8cf9879f392371e81b4af3c2da"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/18/matched_courses?required_cu_count=2
Authorization: Bearer 3ca831c38df8e91e3f57d5c90b137abbf5b410d95251a350d6d604e26cf9d229
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
      "creator_id": 629,
      "id": 216,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 195,
      "additional_university_ids": [

      ],
      "discipline_id": 223,
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
      "chapters_updated_at": "2016-12-08T18:10:14.276Z",
      "updated_at": "2016-12-08T18:10:15.706Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 223,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 634,
      "id": 217,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-bb246352-0cb1-45e7-8425-12d8a4e11749",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-bb246352-0cb1-45e7-8425-12d8a4e11749",
      "slug": "mit-the-great-british-bake-off-bb246352-0cb1-45e7-8425-12d8a4e11749",
      "university_id": 196,
      "additional_university_ids": [

      ],
      "discipline_id": 224,
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
      "chapters_updated_at": "2016-12-08T18:10:14.276Z",
      "updated_at": "2016-12-08T18:10:16.182Z",
      "shortname": "mit-the-great-british-bake-off-bb246352-0cb1-45e7-8425-12d8a4e11749",
      "topic_id": 224,
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
curl "api.goskive.com/v2/files/18/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 3ca831c38df8e91e3f57d5c90b137abbf5b410d95251a350d6d604e26cf9d229"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/3/download
Content-Type: application/json
Authorization: Bearer 5cfceb01dccd8769574158e4eb6e69832d7b685968781b413d30dab53370c6fc
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5cfceb01dccd8769574158e4eb6e69832d7b685968781b413d30dab53370c6fc"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/2/report
Content-Type: application/json
Authorization: Bearer b8de32ed5d122050303b64a2cb8a1bc9f6236b630c82cee275c32e9570951c20
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/2/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8de32ed5d122050303b64a2cb8a1bc9f6236b630c82cee275c32e9570951c20"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/1/bookmark
Content-Type: application/json
Authorization: Bearer c2efda4bf7d2c2daaedfc9eeed27086da487a7c717b39adc5a3932361fc06200
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
	-H "Authorization: Bearer c2efda4bf7d2c2daaedfc9eeed27086da487a7c717b39adc5a3932361fc06200"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/4/upvote
Content-Type: application/json
Authorization: Bearer f932662c429641ef99cc8c72ce4b70a5699d797f5d18c4137b53b82f6f5e4a0d
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f932662c429641ef99cc8c72ce4b70a5699d797f5d18c4137b53b82f6f5e4a0d"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/15/comments
Content-Type: application/json
Authorization: Bearer fb55ea673a4322ad8db446544af884f3c048e21c866e16a8fa93bbf828e738bc
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
    "author_id": 231,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:09:35.385Z",
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
curl "api.goskive.com/v2/flashcards/15/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb55ea673a4322ad8db446544af884f3c048e21c866e16a8fa93bbf828e738bc"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/16/comments
Content-Type: application/json
Authorization: Bearer 516cca1f753e7b6c08e7954c43ac9d04deb9ab53be6b38df423b99aa8848cd2a
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
    "id": 3,
    "author_id": 234,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:09:37.405Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 29,
      "user_id": 234,
      "feedbackable_id": 16,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:37.402Z",
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
curl "api.goskive.com/v2/flashcards/16/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 516cca1f753e7b6c08e7954c43ac9d04deb9ab53be6b38df423b99aa8848cd2a"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/17/comments
Content-Type: application/json
Authorization: Bearer ce1207e2bbb2c96e720b5f2250806dad97665992390dc3e04b0f6235f16b2064
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
      "author_id": 240,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:37.756Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 241,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:37.773Z",
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
curl "api.goskive.com/v2/flashcards/17/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce1207e2bbb2c96e720b5f2250806dad97665992390dc3e04b0f6235f16b2064"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/14/comments
Content-Type: application/json
Authorization: Bearer dc10abd4775ab783bb33260f4ff45a95196a683dac2e98067aa278fb90ea3591
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
curl "api.goskive.com/v2/flashcards/14/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc10abd4775ab783bb33260f4ff45a95196a683dac2e98067aa278fb90ea3591"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/79/feedbacks
Content-Type: application/json
Authorization: Bearer b9df60f152cded0235e719eed09ec024bf2f5f709ed8a4e9532e03e627b52b4a
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
    "id": 40,
    "user_id": 728,
    "feedbackable_id": 79,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:10:22.180Z",
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
curl "api.goskive.com/v2/flashcards/79/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9df60f152cded0235e719eed09ec024bf2f5f709ed8a4e9532e03e627b52b4a"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/83/feedbacks
Content-Type: application/json
Authorization: Bearer a50a4e3ea77d9ffcf7452d0f3cdb450508556c4b124cd2d628c526628e2ecd36
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
      "user_id": 746,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:23.241Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 745,
      "feedbackable_id": 83,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:23.229Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a50a4e3ea77d9ffcf7452d0f3cdb450508556c4b124cd2d628c526628e2ecd36"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/94/votes
Content-Type: application/json
Authorization: Bearer 51f44340eb28cd8021e80fc97dd48be558cc2742ea11ed21c7745e0aa0ac2543
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
      "votable_id": 94,
      "user_id": 946
    },
    {
      "id": 17,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 945
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 94,
      "user_id": 944
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/94/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51f44340eb28cd8021e80fc97dd48be558cc2742ea11ed21c7745e0aa0ac2543"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/54/republish
Content-Type: application/json
Authorization: Bearer 2cd33d2988215a69a314a772db261b09706ef27a41af90ec296fbcf33f8fa2e1
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
curl "api.goskive.com/v2/flashcards/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cd33d2988215a69a314a772db261b09706ef27a41af90ec296fbcf33f8fa2e1"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/bookmark
Content-Type: application/json
Authorization: Bearer 7c1b48e0df6c9d0ff2e6b1b4c1fbf35b369ad3b720262f2925c8d090313c9a77
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/56/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c1b48e0df6c9d0ff2e6b1b4c1fbf35b369ad3b720262f2925c8d090313c9a77"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/76
Content-Type: application/json
Authorization: Bearer 436f92cfbb094940598ef06b02a2151155a797937703731b88318e0d9e82143b
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 436f92cfbb094940598ef06b02a2151155a797937703731b88318e0d9e82143b"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/75/downvote
Content-Type: application/json
Authorization: Bearer d89d4ad9515e9569b34d148bf4efa92cdf438c0a8f78d6af4b265c969153c94f
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
	-H "Authorization: Bearer d89d4ad9515e9569b34d148bf4efa92cdf438c0a8f78d6af4b265c969153c94f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/59
Content-Type: application/json
Authorization: Bearer 4eacc8f3961cae7103d804b12dd6d95f53faf8d396f4245c2dec67c459b1d989
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
    "id": 59,
    "obfuscated_id": "fo0taK4dosk",
    "author_id": 663,
    "chapter_id": 119,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:10:18.095Z",
    "created_at": "2016-12-08T18:10:18.095Z",
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
curl "api.goskive.com/v2/flashcards/59" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eacc8f3961cae7103d804b12dd6d95f53faf8d396f4245c2dec67c459b1d989"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/55/report
Content-Type: application/json
Authorization: Bearer 1e3baa93b0c29404aea7985bf2d79aa4ead0496f2fa2058114db6a2c23cf40ef
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/55/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e3baa93b0c29404aea7985bf2d79aa4ead0496f2fa2058114db6a2c23cf40ef"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/58/bookmark
Content-Type: application/json
Authorization: Bearer f4e16ae74c01d621618c58c21fe436028770bf2fbc08a92252b1578dd89f0451
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4e16ae74c01d621618c58c21fe436028770bf2fbc08a92252b1578dd89f0451"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/57/upvote
Content-Type: application/json
Authorization: Bearer e4d67839f481ba3db8e714ebf7dc9d599f00b52d5cd48485c855c813e946fafd
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/57/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4d67839f481ba3db8e714ebf7dc9d599f00b52d5cd48485c855c813e946fafd"
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
    "key": "cache/c7178356a9b45b7f89666a23146392dc.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxOToxMDozM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2M3MTc4MzU2YTliNDViN2Y4OTY2NmEyMzE0NjM5MmRjLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDhUMTgxMDMzWiJ9XX0=",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T181033Z",
    "x-amz-signature": "33d000cdd20a7e9e60c3fabb81197a117e313661fec5ce4a965b2ea806e75ce4"
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
Authorization: Bearer d32388de2504bc2a297df827d2d5a529818ea6f486df682ff3acfbd015084429
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
	-H "Authorization: Bearer d32388de2504bc2a297df827d2d5a529818ea6f486df682ff3acfbd015084429"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer bea751a2d5bd31f8fd5180dde092fce2438077e5ee4f8a116d007fee077a2728
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
	-H "Authorization: Bearer bea751a2d5bd31f8fd5180dde092fce2438077e5ee4f8a116d007fee077a2728"
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
{"password":{"reset_password_token":"xNDaB6yJ7qs8yL8LoEyt","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 389,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-08T18:09:52.890Z",
  "updated_at": "2016-12-08T18:09:53.485Z",
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
  "audit_id": 7830
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"xNDaB6yJ7qs8yL8LoEyt","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/36/comments
Content-Type: application/json
Authorization: Bearer 9cddb848eaf5164a4213711cd1e307ccf06a8c1e484d7c87cba3de9a37ce9ccb
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
    "id": 8,
    "author_id": 286,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:09:42.868Z",
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
curl "api.goskive.com/v2/questions/36/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cddb848eaf5164a4213711cd1e307ccf06a8c1e484d7c87cba3de9a37ce9ccb"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/38/comments
Content-Type: application/json
Authorization: Bearer a2426c3e2eec332078ba486d95ee04a116c42a63fa12a1978e71f7b193d5ba51
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
    "id": 9,
    "author_id": 292,
    "reply_to_id": null,
    "created_at": "2016-12-08T18:09:43.658Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 30,
      "user_id": 292,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:09:43.655Z",
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
curl "api.goskive.com/v2/questions/38/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2426c3e2eec332078ba486d95ee04a116c42a63fa12a1978e71f7b193d5ba51"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/34/comments
Content-Type: application/json
Authorization: Bearer aa53e8877f02b586282878e368b9f19e684be8c22916121d552dac10cc77aa93
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
      "id": 6,
      "author_id": 281,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:42.218Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 282,
      "reply_to_id": null,
      "created_at": "2016-12-08T18:09:42.235Z",
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
curl "api.goskive.com/v2/questions/34/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa53e8877f02b586282878e368b9f19e684be8c22916121d552dac10cc77aa93"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/37/comments
Content-Type: application/json
Authorization: Bearer 52c941761fce1d04b68230eea8a28a5fa251a565e9d039ea8d7472edace44387
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
curl "api.goskive.com/v2/questions/37/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52c941761fce1d04b68230eea8a28a5fa251a565e9d039ea8d7472edace44387"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/71/feedbacks
Content-Type: application/json
Authorization: Bearer 9e1aeb97a3e7e0936c1d458a5400170030d28950bd2e80534bbeaa50367df3b5
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
    "id": 38,
    "user_id": 528,
    "feedbackable_id": 71,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-08T18:10:03.333Z",
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
curl "api.goskive.com/v2/questions/71/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e1aeb97a3e7e0936c1d458a5400170030d28950bd2e80534bbeaa50367df3b5"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/69/feedbacks
Content-Type: application/json
Authorization: Bearer 301dd7c837d9f5f1877d0706135c8014fe63b1c7ac2a748444ef0336aa009786
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
      "id": 36,
      "user_id": 524,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:02.463Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 523,
      "feedbackable_id": 69,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T18:10:02.448Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/69/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 301dd7c837d9f5f1877d0706135c8014fe63b1c7ac2a748444ef0336aa009786"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/130/votes
Content-Type: application/json
Authorization: Bearer 047e27c6024c0f4f88c821d8e5ebada50f3340053eab9e7d6797c00bfcc4e904
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
      "votable_id": 130,
      "user_id": 969
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 968
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 967
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/130/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 047e27c6024c0f4f88c821d8e5ebada50f3340053eab9e7d6797c00bfcc4e904"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/56/republish
Content-Type: application/json
Authorization: Bearer b352e849fa4b9107c9831aefc421082cd01835f3cbf8b8290b2ad632b61f7285
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
	-H "Authorization: Bearer b352e849fa4b9107c9831aefc421082cd01835f3cbf8b8290b2ad632b61f7285"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/58/bookmark
Content-Type: application/json
Authorization: Bearer 460fd5bcc65dac4b7b0c8ef858f8364f07e02d7fcf7bd0021021bbd4a7c55cc0
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
	-H "Authorization: Bearer 460fd5bcc65dac4b7b0c8ef858f8364f07e02d7fcf7bd0021021bbd4a7c55cc0"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/59
Content-Type: application/json
Authorization: Bearer ef79aaebe67572110d51554dfca62ccc8af17ea77e665a9dcc0005977575e9c5
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
	-H "Authorization: Bearer ef79aaebe67572110d51554dfca62ccc8af17ea77e665a9dcc0005977575e9c5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/62/downvote
Content-Type: application/json
Authorization: Bearer 97f237d2169a868a919bcdb65a9e499e7b0391335dd77784521a5fdae2360418
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/62/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97f237d2169a868a919bcdb65a9e499e7b0391335dd77784521a5fdae2360418"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/60
Content-Type: application/json
Authorization: Bearer de84c5084b976b5ebdbe31a6493b6dc708a4a98982065dc4bcae28f772bbf412
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
    "id": 60,
    "obfuscated_id": "XsZtONYAiuo",
    "author_id": 366,
    "chapter_id": 76,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:51.205Z",
    "created_at": "2016-12-08T18:09:51.125Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/60" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de84c5084b976b5ebdbe31a6493b6dc708a4a98982065dc4bcae28f772bbf412"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/55/report
Content-Type: application/json
Authorization: Bearer 2cc9b305511ce094fe85c696a51c60423df0fb07b509abb925b55a87fec4b669
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/55/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2cc9b305511ce094fe85c696a51c60423df0fb07b509abb925b55a87fec4b669"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/63/bookmark
Content-Type: application/json
Authorization: Bearer 84af9cb33173ecc544eaf32833631f8a7c52037469082027398f8905a8140b89
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/63/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84af9cb33173ecc544eaf32833631f8a7c52037469082027398f8905a8140b89"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/39
Content-Type: application/json
Authorization: Bearer 7a2bf7bcffd9cda8c7c7a5c718382e57197fe5643b07958da79691d2143524a5
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":39,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T18:09:44.511Z","updated_at":"2016-12-08T18:09:44.591Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":55,"author_id":298,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 298,
    "chapter_id": 55,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T18:09:44.676Z",
    "created_at": "2016-12-08T18:09:44.511Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x0000000f9c8100>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 80,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 81,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 82,
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
curl "api.goskive.com/v2/questions/39" -d '{"question":{"question":{"id":39,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T18:09:44.511Z","updated_at":"2016-12-08T18:09:44.591Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":55,"author_id":298,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a2bf7bcffd9cda8c7c7a5c718382e57197fe5643b07958da79691d2143524a5"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/61/upvote
Content-Type: application/json
Authorization: Bearer 4fb282c3e5fd3a84411271a7b450760b6a6187a2ea80a84072531c4bfa6dc1f5
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/61/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fb282c3e5fd3a84411271a7b450760b6a6187a2ea80a84072531c4bfa6dc1f5"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 86f8c3e01c28e7c7e7cf7a1c5388444dbd392bd91236ac8cd1c49da30586506a
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
      "creator_id": 862,
      "id": 280,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "discipline_id": 290,
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
      "updated_at": "2016-12-08T18:10:34.162Z",
      "shortname": "mit-pizza-201",
      "topic_id": 290,
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
	-H "Authorization: Bearer 86f8c3e01c28e7c7e7cf7a1c5388444dbd392bd91236ac8cd1c49da30586506a"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 12f763805e2a0fed908ce44e85fc1c772741cbccb5498eb2b69a9dcac532bc29
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
      "id": 259,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-241",
      "html_url": "https://goskive.com/university/uni-241",
      "slug": "uni-241",
      "name": "National School of Pizza",
      "short_name": "Uni 241",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/61c0ead21a56eb3dabcee297cbf79f67.jpg",
      "image_thumb_url": "memory://universities/5a8b93066a7a2589d6ff799147533e0e.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:10:33.892Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 258,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-240",
      "html_url": "https://goskive.com/university/uni-240",
      "slug": "uni-240",
      "name": "National School of Pastry",
      "short_name": "Uni 240",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/4e977e76e0a51a53c25f25abdea61a93.jpg",
      "image_thumb_url": "memory://universities/ac3bb4d0501acc70959818b21e1904bb.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:10:33.845Z",
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
	-H "Authorization: Bearer 12f763805e2a0fed908ce44e85fc1c772741cbccb5498eb2b69a9dcac532bc29"
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
      "id": 261,
      "name": "Monitored composite parallelism",
      "name_translations": {
        "en": "Monitored composite parallelism"
      },
      "discipline_id": 261
    },
    {
      "id": 262,
      "name": "Polarised next generation application",
      "name_translations": {
        "en": "Polarised next generation application"
      },
      "discipline_id": 262
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
GET /v2/topics/260
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
    "id": 260,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 260
  }
}
```



```shell
curl "api.goskive.com/v2/topics/260" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer ab64aba5c9dc122b0c78ddb5f2001a89f964ee0278c3cc9ab480e079ef54c012
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
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-271",
      "html_url": "https://goskive.com/university/uni-271",
      "slug": "uni-271",
      "name": "University 208",
      "short_name": "Uni 271",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/ac4835d53a3ceb94101e1c2011bb216f.jpg",
      "image_thumb_url": "memory://universities/19a98a41854b9c5369a5b39c07793ff9.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:10:40.851Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 290,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-270",
      "html_url": "https://goskive.com/university/uni-270",
      "slug": "uni-270",
      "name": "University 207",
      "short_name": "Uni 270",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/6b4ccf8fbb1107ade69dda5c19818974.jpg",
      "image_thumb_url": "memory://universities/8ca206fcf681e0af4341a83cf2a725ee.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:10:40.801Z",
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
      "name": "University 206",
      "short_name": "Uni 269",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "memory://universities/d86105a734f1484a84ba1509494f71fb.jpg",
      "image_thumb_url": "memory://universities/155c4b20480fac9679b6c88019a160af.jpg",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T18:10:40.752Z",
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
	-H "Authorization: Bearer ab64aba5c9dc122b0c78ddb5f2001a89f964ee0278c3cc9ab480e079ef54c012"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 236767d922bae77dce2236455df098e76c52d0fe693b8962b1572c000e6996e0
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
    "id": 287,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "memory://universities/74b9906a9abb8f97d873b69a3580172c.jpg",
    "image_thumb_url": "memory://universities/f3ff5ec0f6ef5120f28a7986ac8b98d6.jpg",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-08T18:10:40.556Z",
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
	-H "Authorization: Bearer 236767d922bae77dce2236455df098e76c52d0fe693b8962b1572c000e6996e0"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 86284d5cccc0f1cc150b3d243aedf5ddc990ba20e97e06590f18b8bcddbb1d3a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":51,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 183,
    "id": 46,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 46,
    "additional_university_ids": [

    ],
    "discipline_id": 51,
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
    "chapters_updated_at": "2016-12-08T18:09:27.305Z",
    "updated_at": "2016-12-08T18:09:27.455Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 32,
        "updated_at": "2016-12-08T18:09:27.443Z",
        "course_id": 46,
        "author_id": 183,
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
        "id": 33,
        "updated_at": "2016-12-08T18:09:27.458Z",
        "course_id": 46,
        "author_id": 183,
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
        "id": 34,
        "updated_at": "2016-12-08T18:09:27.472Z",
        "course_id": 46,
        "author_id": 183,
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
    "topic_id": 51,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":51,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86284d5cccc0f1cc150b3d243aedf5ddc990ba20e97e06590f18b8bcddbb1d3a"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c70bffd45114e9cbfe8b86df89146a7d1a0d9e210bd537658d41e6abca19ae42
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":52,"published":false}}
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
    "creator_id": 184,
    "id": 47,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 47,
    "additional_university_ids": [

    ],
    "discipline_id": 52,
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
    "updated_at": "2016-12-08T18:09:27.713Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 52,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":52,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c70bffd45114e9cbfe8b86df89146a7d1a0d9e210bd537658d41e6abca19ae42"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 10196c6e7baad9e0cbeada0f6016a630c904f1a7ed19af65e03a39fc429f320a
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
      "creator_id": 192,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-52",
      "html_url": "https://goskive.com/course/fu-course-52",
      "slug": "fu-course-52",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "discipline_id": 61,
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
      "updated_at": "2016-12-08T18:09:28.800Z",
      "shortname": "fu-course-52",
      "topic_id": 61,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 52",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 192,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-53",
      "html_url": "https://goskive.com/course/fu-course-53",
      "slug": "fu-course-53",
      "university_id": 52,
      "additional_university_ids": [

      ],
      "discipline_id": 62,
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
      "chapters_updated_at": "2016-12-08T18:09:28.472Z",
      "updated_at": "2016-12-08T18:09:29.054Z",
      "shortname": "fu-course-53",
      "topic_id": 62,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 53",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10196c6e7baad9e0cbeada0f6016a630c904f1a7ed19af65e03a39fc429f320a"
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
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-60",
      "html_url": "https://goskive.com/course/fu-course-60",
      "slug": "fu-course-60",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "discipline_id": 69,
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
      "updated_at": "2016-12-08T18:09:29.807Z",
      "shortname": "fu-course-60",
      "topic_id": 69,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 60",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 202,
      "id": 65,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-61",
      "html_url": "https://goskive.com/course/fu-course-61",
      "slug": "fu-course-61",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "discipline_id": 70,
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
      "chapters_updated_at": "2016-12-08T18:09:29.521Z",
      "updated_at": "2016-12-08T18:09:30.061Z",
      "shortname": "fu-course-61",
      "topic_id": 70,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 61",
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
Authorization: Bearer 0341c37aa143e961b72dd63226d4f37c4d0a159d7589a22d7bf4da2c6ef747f7
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
      "creator_id": 198,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-56",
      "html_url": "https://goskive.com/course/fu-course-56",
      "slug": "fu-course-56",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "discipline_id": 65,
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
      "updated_at": "2016-12-08T18:09:29.295Z",
      "shortname": "fu-course-56",
      "topic_id": 65,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 198,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "discipline_id": 66,
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
      "updated_at": "2016-12-08T18:09:29.334Z",
      "shortname": "fu-course-57",
      "topic_id": 66,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0341c37aa143e961b72dd63226d4f37c4d0a159d7589a22d7bf4da2c6ef747f7"
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
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-64",
      "html_url": "https://goskive.com/course/fu-course-64",
      "slug": "fu-course-64",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "discipline_id": 73,
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
      "updated_at": "2016-12-08T18:09:30.319Z",
      "shortname": "fu-course-64",
      "topic_id": 73,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 64",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 207,
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-65",
      "html_url": "https://goskive.com/course/fu-course-65",
      "slug": "fu-course-65",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "discipline_id": 74,
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
      "updated_at": "2016-12-08T18:09:30.353Z",
      "shortname": "fu-course-65",
      "topic_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 65",
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
Authorization: Bearer 426e58a8c4a6bd288ecac5bc8fbcc0f5203ebd3cc7f74c061af241badf82b312
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
  "id": 494,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-08T18:10:00.225Z",
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
	-H "Authorization: Bearer 426e58a8c4a6bd288ecac5bc8fbcc0f5203ebd3cc7f74c061af241badf82b312"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/399
Content-Type: application/json
Authorization: Bearer a45aaed92974f847a150481c249f4ef1af18768f9222b2fb7d5ede77cc4e569e
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
    "id": 399,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 115,
    "fields_of_study": [
      142,
      143
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-08T18:09:54.841Z",
    "updated_at": "2016-12-08T18:09:54.841Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/399" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a45aaed92974f847a150481c249f4ef1af18768f9222b2fb7d5ede77cc4e569e"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/397
Content-Type: application/json
Authorization: Bearer 6933fd996a723849120badd68f636ea0ff28b246ec52f592c6920982fbfa1689
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
    "id": 397,
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
    "created_at": "2016-12-08T18:09:54.668Z",
    "updated_at": "2016-12-08T18:09:54.668Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/397" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6933fd996a723849120badd68f636ea0ff28b246ec52f592c6920982fbfa1689"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/6
Content-Type: application/json
Authorization: Bearer 4209594063bde4c6019cb2e20b7854428f4525812cd36708b9747737cb60c451
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
	-H "Authorization: Bearer 4209594063bde4c6019cb2e20b7854428f4525812cd36708b9747737cb60c451"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/8
Content-Type: application/json
Authorization: Bearer 0698bbba57973f72777c933b78b6dfa365fb5ed03dc3a8fb58b4d9524da28ce7
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
    "id": 8,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 114,
    "user_id": 789
  }
}
```



```shell
curl "api.goskive.com/v2/votes/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0698bbba57973f72777c933b78b6dfa365fb5ed03dc3a8fb58b4d9524da28ce7"
```
