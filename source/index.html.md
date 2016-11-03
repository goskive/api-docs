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
Authorization: Basic MWY1YWQ4NTAyZWQ2OTNmYzdlNTZjODU3NDk1OTU2YWJhNzkyNmZhMGFlODBl
Yzk0ZjJlYTFhYjY1YzVkNmIxNDphYzU4OGE2OWMxZjgyMTMwYWVhODdmOGI1
YWExMTFkOWFmZWQ2MjE0YmUyMzEwYTRjYjllZGU3Y2M0NmI0MWQ0

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
	-u 1f5ad8502ed693fc7e56c857495956aba7926fa0ae80ec94f2ea1ab65c5d6b14:ac588a69c1f82130aea87f8b5aa111d9afed6214be2310a4cb9ede7cc46b41d4
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c83cbd45cb760648e0f20a94f72f28220f6a22eed492aa64254353b47d065495","client_secret":"5a7c74aa35da02ef109f69762e4a3b9bb82638dcee34c967328678f2c720db21"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c83cbd45cb760648e0f20a94f72f28220f6a22eed492aa64254353b47d065495","client_secret":"5a7c74aa35da02ef109f69762e4a3b9bb82638dcee34c967328678f2c720db21"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YmVkZmEwOTNhYjJlYTRmODViM2E3OThiYjIzOWMxNzY2MDY2Mjg3ZDM2M2Y0
MmFjNGJjMzc5ZTY1ZDliMWJkOToyYjEwMTEyYjZjNmE2ZWE2YjYwNjA3Zjhj
NWQxYTU2YTljMTRlYTExYjkyY2U5NmNiOWJhMWE0MzFkZGJjZWRl

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
  "access_token": "3547d53b29bd588214eab74d5d8f8ca73a0b04f2fc9829649aa752ecd4bdd733",
  "token_type": "bearer",
  "created_at": 1478172446
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u bedfa093ab2ea4f85b3a798bb239c1766066287d363f42ac4bc379e65d9b1bd9:2b10112b6c6a6ea6b60607f8c5d1a56a9c14ea11b92ce96cb9ba1a431ddbcede
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"357d83c888529b55159fc6f0f79c73c177a90f14bdd60386dc0e3e983f85453e","client_secret":"03e45a8b231499d82ebe1593206465b9d425a9cc4be7dd50545c9c6681f93335"}
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
  "access_token": "936d15613945a70313284952644d482b782ef4a2bc62a8b0633a2eb9bbded9c3",
  "token_type": "bearer",
  "created_at": 1478172446
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"357d83c888529b55159fc6f0f79c73c177a90f14bdd60386dc0e3e983f85453e","client_secret":"03e45a8b231499d82ebe1593206465b9d425a9cc4be7dd50545c9c6681f93335"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"b276f3649e40964e5298ce7170ff0799c3aa1eac9c4b8d67007a50b434185c98","client_secret":"8a49b96586df83bdb24848bca1a1fa63797c17581aa017e7bbc07a912632ab6b"}
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
  "access_token": "1983de1fb1f92898bfcc3ea4119115cb1dea609a3658f388c195230c8293c7f1",
  "token_type": "bearer",
  "created_at": 1478172446
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"b276f3649e40964e5298ce7170ff0799c3aa1eac9c4b8d67007a50b434185c98","client_secret":"8a49b96586df83bdb24848bca1a1fa63797c17581aa017e7bbc07a912632ab6b"}' -X POST \
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
GET /v2/campaigns/4
Content-Type: application/json
Authorization: Bearer 930dfa07d6e8ae787298b63b06909ea3429e364c57a06b28b9329165b13e2b85
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
    "id": 4,
    "title": "Recruiting pastry chefs",
    "company_id": 20,
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
curl "api.goskive.com/v2/campaigns/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 930dfa07d6e8ae787298b63b06909ea3429e364c57a06b28b9329165b13e2b85"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/80/flashcards
Content-Type: application/json
Authorization: Bearer 2c5fec9d29af2dd76e37cfd1d063de89475b5dca8aae1a5f1c7fbb29bd3538a0
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":80,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 26,
    "obfuscated_id": "cWAsrz6MOVI",
    "author_id": 339,
    "chapter_id": 80,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:24.029Z",
    "created_at": "2016-11-03T11:27:24.029Z",
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
curl "api.goskive.com/v2/chapters/80/flashcards" -d '{"flashcard":{"chapter_id":80,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c5fec9d29af2dd76e37cfd1d063de89475b5dca8aae1a5f1c7fbb29bd3538a0"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/81/flashcards
Content-Type: application/json
Authorization: Bearer 29519f4a3e4900554cd396e7068944044d9c76040250f6eecf4ca596ecb0523e
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 340,
      "chapter_id": 81,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:24.192Z",
      "created_at": "2016-11-03T11:27:24.192Z",
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
      "author_id": 340,
      "chapter_id": 81,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:24.237Z",
      "created_at": "2016-11-03T11:27:24.237Z",
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
      "author_id": 340,
      "chapter_id": 81,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:24.279Z",
      "created_at": "2016-11-03T11:27:24.279Z",
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
curl "api.goskive.com/v2/chapters/81/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29519f4a3e4900554cd396e7068944044d9c76040250f6eecf4ca596ecb0523e"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/76/questions
Content-Type: application/json
Authorization: Bearer 074027aad0bcf1865e6bdc6531f856333c689ede27e0d168e51b94ef3bb6a967
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":76,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 34,
    "obfuscated_id": "LRSQf_NrQzE",
    "author_id": 320,
    "chapter_id": 76,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:21.748Z",
    "created_at": "2016-11-03T11:27:21.748Z",
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
        "id": 68,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 69,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 70,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 71,
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
curl "api.goskive.com/v2/chapters/76/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":76,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 074027aad0bcf1865e6bdc6531f856333c689ede27e0d168e51b94ef3bb6a967"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/75/questions
Content-Type: application/json
Authorization: Bearer 72efcf3e3d817f5ce70b842015dc6515c85d22a59545dd4cdfe9d66a3a85138c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":75,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 317,
    "chapter_id": 75,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:21.404Z",
    "created_at": "2016-11-03T11:27:21.404Z",
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
        "id": 66,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 67,
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
curl "api.goskive.com/v2/chapters/75/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":75,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 72efcf3e3d817f5ce70b842015dc6515c85d22a59545dd4cdfe9d66a3a85138c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/77/questions
Content-Type: application/json
Authorization: Bearer 45d74e40f01cb8036237b7c48e8834ad0ee3c5ac8d586e358884dbc45ce3041b
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":77,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 35,
    "obfuscated_id": "soCS52BooV0",
    "author_id": 323,
    "chapter_id": 77,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:22.284Z",
    "created_at": "2016-11-03T11:27:22.284Z",
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
        "id": 72,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 73,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/77/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":77,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45d74e40f01cb8036237b7c48e8834ad0ee3c5ac8d586e358884dbc45ce3041b"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/74/questions
Content-Type: application/json
Authorization: Bearer 6c405762a1dbbe56066387aeec07a4e5b85c08884e82ec3bc9d2a2a53a9c17d3
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":74,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 314,
    "chapter_id": 74,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:20.965Z",
    "created_at": "2016-11-03T11:27:20.965Z",
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
curl "api.goskive.com/v2/chapters/74/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":74,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c405762a1dbbe56066387aeec07a4e5b85c08884e82ec3bc9d2a2a53a9c17d3"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/73/questions
Content-Type: application/json
Authorization: Bearer 4d0e0844a0fcc6bed5dc7dd1968e239003163b9ad4ea7f40b7bf7ff238f6363c
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
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 308,
      "chapter_id": 73,
      "position": 29,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:20.286Z",
      "created_at": "2016-11-03T11:27:20.158Z",
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
    },
    {
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 309,
      "chapter_id": 73,
      "position": 30,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:20.493Z",
      "created_at": "2016-11-03T11:27:20.361Z",
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
          "id": 59,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 60,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 310,
      "chapter_id": 73,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:20.703Z",
      "created_at": "2016-11-03T11:27:20.569Z",
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
        }
      ]
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/73/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d0e0844a0fcc6bed5dc7dd1968e239003163b9ad4ea7f40b7bf7ff238f6363c"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/101
Content-Type: application/json
Authorization: Bearer ce8e917f60472f4f78fd90927cc1cc542792c5239376b1b6089c82c18e7237c4
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
curl "api.goskive.com/v2/chapters/101" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce8e917f60472f4f78fd90927cc1cc542792c5239376b1b6089c82c18e7237c4"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/103
Content-Type: application/json
Authorization: Bearer d84a869daa8273595e922d9416cd18dbe2c0d5bf284dad50fb64eb96d8b01a9e
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
curl "api.goskive.com/v2/chapters/103" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d84a869daa8273595e922d9416cd18dbe2c0d5bf284dad50fb64eb96d8b01a9e"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/106
Content-Type: application/json
Authorization: Bearer a94a0385c00072342a6f84484463a7bf354a5333b354f5ee06d60de856660cbf
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
curl "api.goskive.com/v2/chapters/106" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a94a0385c00072342a6f84484463a7bf354a5333b354f5ee06d60de856660cbf"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/100
Content-Type: application/json
Authorization: Bearer 1c2d273dba110ae543f74f0e377a58dc7f1a469ad5469f161f794a4aff70a6dd
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/100" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c2d273dba110ae543f74f0e377a58dc7f1a469ad5469f161f794a4aff70a6dd"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/104
Content-Type: application/json
Authorization: Bearer d099659dbaeb0145874bd47767860d65f48564357b7f669e37c45095389e58b8
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
    "id": 104,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T11:27:41.148Z",
    "course_id": 163,
    "author_id": 548,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-03T11:27:40.648Z",
    "questions_updated_at": "2016-11-03T11:27:40.648Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 552,
        "chapter_id": 104,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.131Z",
        "created_at": "2016-11-03T11:27:41.131Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 550,
        "chapter_id": 104,
        "position": 72,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.030Z",
        "created_at": "2016-11-03T11:27:40.918Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/104" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d099659dbaeb0145874bd47767860d65f48564357b7f669e37c45095389e58b8"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/108
Content-Type: application/json
Authorization: Bearer a061bb652d5d5a01b82803a983adb69c778b87f4a9fa03bb6f9832c60dd2c7f8
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
    "id": 108,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T11:27:42.178Z",
    "course_id": 167,
    "author_id": 568,
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

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/108" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a061bb652d5d5a01b82803a983adb69c778b87f4a9fa03bb6f9832c60dd2c7f8"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/12/replies
Content-Type: application/json
Authorization: Bearer 47f609259ac86bb615d7e35e7621b9e8fa85ec85f3bdb56b55205a7f18b8545e
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
    "author_id": 331,
    "reply_to_id": 12,
    "created_at": "2016-11-03T11:27:23.377Z",
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
	-H "Authorization: Bearer 47f609259ac86bb615d7e35e7621b9e8fa85ec85f3bdb56b55205a7f18b8545e"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/14/replies
Content-Type: application/json
Authorization: Bearer 3005a74e11328500c8452d6f732f7dd220440da74b1f6b5a9fe3534b536a3a18
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
curl "api.goskive.com/v2/comments/14/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3005a74e11328500c8452d6f732f7dd220440da74b1f6b5a9fe3534b536a3a18"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/19
Content-Type: application/json
Authorization: Bearer 65443a9effabc06e24116dfe88ce8eecffcdbdafb54a53e681b69a7c86997141
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
curl "api.goskive.com/v2/comments/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65443a9effabc06e24116dfe88ce8eecffcdbdafb54a53e681b69a7c86997141"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/16/republish
Content-Type: application/json
Authorization: Bearer 87d2eceb4faeffac87283a6131d4d111390215c216ae7a2b4bffc65b9879c27c
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
curl "api.goskive.com/v2/comments/16/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87d2eceb4faeffac87283a6131d4d111390215c216ae7a2b4bffc65b9879c27c"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/20
Content-Type: application/json
Authorization: Bearer 674acb4e1b66c20e2081d2bc5e8c5ca2f681e3f24d81e439f17c4fa22b0c2626
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 674acb4e1b66c20e2081d2bc5e8c5ca2f681e3f24d81e439f17c4fa22b0c2626"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/15/report
Content-Type: application/json
Authorization: Bearer 0755d84e8f662cebd78a2e6376f79203c8ff47d802174a580aa08642e28e54bf
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/15/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0755d84e8f662cebd78a2e6376f79203c8ff47d802174a580aa08642e28e54bf"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/24
Content-Type: application/json
Authorization: Bearer d5902ad6b897bf6250c67258f59b599d5b577b335ebeae193ae30c04b9057967
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
    "id": 24,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-03T11:27:54.243Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5902ad6b897bf6250c67258f59b599d5b577b335ebeae193ae30c04b9057967"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 731cd2bbadd53e66f73ccdccca0395fc9a05e6e61b6fb9ea9f0bc27382cce096
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
      "id": 21,
      "name": "Fake Company Name 20",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T11:27:54.128Z"
    },
    {
      "id": 22,
      "name": "Fake Company Name 21",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T11:27:54.132Z"
    },
    {
      "id": 23,
      "name": "Fake Company Name 22",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/410e5dc805425b1d1ef49b9628e4f1141ae13d80.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T11:27:54.135Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 731cd2bbadd53e66f73ccdccca0395fc9a05e6e61b6fb9ea9f0bc27382cce096"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer e435779262a60a58e5629ccc298d6de489b458799de555aa5d79c4c1a4807210
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
	-H "Authorization: Bearer e435779262a60a58e5629ccc298d6de489b458799de555aa5d79c4c1a4807210"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer bde2cab83d372f3ae04a4044a692002c61241859ea2c6c5951d1704ac0f05ea0
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
	-H "Authorization: Bearer bde2cab83d372f3ae04a4044a692002c61241859ea2c6c5951d1704ac0f05ea0"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer ef44b4624f330dcab5d738771a9926a9c7798134125b3a35a85829a4c6896774
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
	-H "Authorization: Bearer ef44b4624f330dcab5d738771a9926a9c7798134125b3a35a85829a4c6896774"
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
Authorization: Bearer e976d142c97d56788f7d456fa4368995189117e75d61d29d88a1ed437e14fc2e
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
	-H "Authorization: Bearer e976d142c97d56788f7d456fa4368995189117e75d61d29d88a1ed437e14fc2e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b4847dd3f12fab3f575c1751f5a27322b7706a69b0e787d43452736882b069ac
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
    "id": 36,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T11:27:08.213Z",
    "course_id": 34,
    "author_id": 130,
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

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4847dd3f12fab3f575c1751f5a27322b7706a69b0e787d43452736882b069ac"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4c6b01a205d12e78a5971ebf41db4ad3ce3da73ed7dd51de9de8c06325cd73c7
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
      "id": 17,
      "title": "Clever Chapter Title 17",
      "position": 1,
      "updated_at": "2016-11-03T11:27:05.957Z",
      "course_id": 23,
      "author_id": 87,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 18,
      "title": "Clever Chapter Title 18",
      "position": 2,
      "updated_at": "2016-11-03T11:27:05.978Z",
      "course_id": 23,
      "author_id": 88,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 19,
      "title": "Clever Chapter Title 19",
      "position": 3,
      "updated_at": "2016-11-03T11:27:06.241Z",
      "course_id": 23,
      "author_id": 89,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T11:27:05.891Z",
      "questions_updated_at": "2016-11-03T11:27:05.891Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c6b01a205d12e78a5971ebf41db4ad3ce3da73ed7dd51de9de8c06325cd73c7"
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
      "id": 29,
      "title": "Clever Chapter Title 29",
      "position": 1,
      "updated_at": "2016-11-03T11:27:07.361Z",
      "course_id": 29,
      "author_id": 115,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 30,
      "title": "Clever Chapter Title 30",
      "position": 2,
      "updated_at": "2016-11-03T11:27:07.384Z",
      "course_id": 29,
      "author_id": 116,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 31,
      "title": "Clever Chapter Title 31",
      "position": 3,
      "updated_at": "2016-11-03T11:27:07.625Z",
      "course_id": 29,
      "author_id": 117,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T11:27:07.293Z",
      "questions_updated_at": "2016-11-03T11:27:07.293Z",
      "flashcards_count": 0,
      "questions_count": 1
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
Authorization: Bearer 26e1bba8cb25cf8acc3186fa886eb2f8bf454b142e329a547ceb3afa1842fdf1
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
      "id": 20,
      "title": "Clever Chapter Title 20",
      "position": 1,
      "updated_at": "2016-11-03T11:27:06.504Z",
      "course_id": 25,
      "author_id": 96,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 21,
      "title": "Clever Chapter Title 21",
      "position": 2,
      "updated_at": "2016-11-03T11:27:06.526Z",
      "course_id": 25,
      "author_id": 97,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 22,
      "title": "Clever Chapter Title 22",
      "position": 3,
      "updated_at": "2016-11-03T11:27:06.548Z",
      "course_id": 25,
      "author_id": 98,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26e1bba8cb25cf8acc3186fa886eb2f8bf454b142e329a547ceb3afa1842fdf1"
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
      "id": 32,
      "title": "Clever Chapter Title 32",
      "position": 1,
      "updated_at": "2016-11-03T11:27:07.733Z",
      "course_id": 30,
      "author_id": 121,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 33,
      "title": "Clever Chapter Title 33",
      "position": 2,
      "updated_at": "2016-11-03T11:27:07.756Z",
      "course_id": 30,
      "author_id": 122,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 34,
      "title": "Clever Chapter Title 34",
      "position": 3,
      "updated_at": "2016-11-03T11:27:07.780Z",
      "course_id": 30,
      "author_id": 123,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
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
Authorization: Bearer 688ea036d3e1d751ea5a8fadc240573be6367e2d909bf4c138b6f54064b01061
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
    "id": 3,
    "course_id": 76,
    "user_id": 290,
    "updated_at": "2016-11-03T11:27:19.400Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 688ea036d3e1d751ea5a8fadc240573be6367e2d909bf4c138b6f54064b01061"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 3a838320784e7d5dddae83d76ea49ab155270e9a16907ef06ebd1494dfff5cbe
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
      "course_id": 80,
      "user_id": 300,
      "updated_at": "2016-11-03T11:27:19.846Z"
    },
    {
      "id": 7,
      "course_id": 80,
      "user_id": 301,
      "updated_at": "2016-11-03T11:27:19.860Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a838320784e7d5dddae83d76ea49ab155270e9a16907ef06ebd1494dfff5cbe"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/18/files
Content-Type: application/json
Authorization: Bearer a10865006f38de0a47a59fa1c13ee4474f9e782ee1891197fa3e6ea9687e1b2a
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
        "id": 71,
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
        "created_at": "2016-11-03T11:27:05.138Z",
        "updated_at": "2016-11-03T11:27:05.138Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T11:27:05.151Z",
      "updated_at": "2016-11-03T11:27:05.151Z",
      "course_id": 18,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 72,
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
        "created_at": "2016-11-03T11:27:05.159Z",
        "updated_at": "2016-11-03T11:27:05.159Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T11:27:05.168Z",
      "updated_at": "2016-11-03T11:27:05.168Z",
      "course_id": 18,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 4,
      "uploader": {
        "id": 73,
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
        "created_at": "2016-11-03T11:27:05.175Z",
        "updated_at": "2016-11-03T11:27:05.175Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T11:27:05.184Z",
      "updated_at": "2016-11-03T11:27:05.184Z",
      "course_id": 18,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/18/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a10865006f38de0a47a59fa1c13ee4474f9e782ee1891197fa3e6ea9687e1b2a"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/16/files
Content-Type: application/json
Authorization: Bearer e25341888c724708b83265211d3f106710a8e55b0a9e2c8cc934ea475e940838
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
      "id": 67,
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
      "created_at": "2016-11-03T11:27:04.791Z",
      "updated_at": "2016-11-03T11:27:04.791Z"
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
    "created_at": "2016-11-03T11:27:04.848Z",
    "updated_at": "2016-11-03T11:27:04.848Z",
    "course_id": 16,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/16/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e25341888c724708b83265211d3f106710a8e55b0a9e2c8cc934ea475e940838"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/15/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer e287408163501eef18312bae31d5540443140f7bdee57ae64af3fa643a8ce60a
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
    "key": "cache/29a2acece208fbfebe4336800c46b2aa.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxMjoyNzowNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzI5YTJhY2VjZTIwOGZiZmViZTQzMzY4MDBjNDZiMmFhLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDMvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTAzVDExMjcwNFoifV19",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T112704Z",
    "x-amz-signature": "657e581c4583e6d62d11c34ed31deeecb1e7f4a5376b8f8722bbff0af23af8bc"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/15/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e287408163501eef18312bae31d5540443140f7bdee57ae64af3fa643a8ce60a"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 239c3c3d3305f535620441b416f06c585b912d09d5629fc9376bdfce183c8258
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
	-H "Authorization: Bearer 239c3c3d3305f535620441b416f06c585b912d09d5629fc9376bdfce183c8258"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 38abba016252f1e6e5b169791fdea35d64ede573b4574b6e6cf044623172d626
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
	-H "Authorization: Bearer 38abba016252f1e6e5b169791fdea35d64ede573b4574b6e6cf044623172d626"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ab3be78091d5b5d8fb2ae3de6d9702656963a4feb76139bb5989b29adf2d1201
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
	-H "Authorization: Bearer ab3be78091d5b5d8fb2ae3de6d9702656963a4feb76139bb5989b29adf2d1201"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bd931253e02186384f59ab52dcb1babcb54a549b520d40f19e58bb0f840b8fcc
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
	-H "Authorization: Bearer bd931253e02186384f59ab52dcb1babcb54a549b520d40f19e58bb0f840b8fcc"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7d56744478d014c0e54544af059f490fd65c9cafdcedcb2e8a6dfe205c716b1c
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
	-H "Authorization: Bearer 7d56744478d014c0e54544af059f490fd65c9cafdcedcb2e8a6dfe205c716b1c"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 598a98cf0d14bcbe7c260ad2ecf0e1c3c2b4ac021a25a8b68bc285b943ee4dcd
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
    "creator_id": 473,
    "id": 140,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 141,
    "additional_university_ids": [

    ],
    "topic_id": 145,
    "discipline_id": 146,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
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
    "chapters_updated_at": "2016-11-03T11:27:30.894Z",
    "updated_at": "2016-11-03T11:27:32.258Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 87,
        "title": "Clever Chapter Title 75",
        "position": 1,
        "updated_at": "2016-11-03T11:27:32.215Z",
        "course_id": 140,
        "author_id": 473,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T11:27:30.894Z",
        "questions_updated_at": "2016-11-03T11:27:30.894Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 88,
        "title": "Clever Chapter Title 76",
        "position": 2,
        "updated_at": "2016-11-03T11:27:32.251Z",
        "course_id": 140,
        "author_id": 473,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T11:27:30.894Z",
        "questions_updated_at": "2016-11-03T11:27:30.894Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 474,
        "chapter_id": 87,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:32.060Z",
        "created_at": "2016-11-03T11:27:32.060Z",
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
        "author_id": 474,
        "chapter_id": 88,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:32.132Z",
        "created_at": "2016-11-03T11:27:32.132Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 474,
        "chapter_id": 87,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:32.098Z",
        "created_at": "2016-11-03T11:27:32.098Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 474,
        "chapter_id": 88,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:32.169Z",
        "created_at": "2016-11-03T11:27:32.169Z",
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
        "author_id": 474,
        "chapter_id": 87,
        "position": 42,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:31.098Z",
        "created_at": "2016-11-03T11:27:30.988Z",
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
        "author_id": 474,
        "chapter_id": 87,
        "position": 43,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:31.264Z",
        "created_at": "2016-11-03T11:27:31.158Z",
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
        "author_id": 474,
        "chapter_id": 88,
        "position": 44,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:31.455Z",
        "created_at": "2016-11-03T11:27:31.341Z",
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
        "author_id": 474,
        "chapter_id": 88,
        "position": 45,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:31.627Z",
        "created_at": "2016-11-03T11:27:31.518Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 598a98cf0d14bcbe7c260ad2ecf0e1c3c2b4ac021a25a8b68bc285b943ee4dcd"
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
    "creator_id": 485,
    "id": 142,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 143,
    "additional_university_ids": [

    ],
    "topic_id": 147,
    "discipline_id": 148,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
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
    "chapters_updated_at": "2016-11-03T11:27:33.866Z",
    "updated_at": "2016-11-03T11:27:35.215Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 91,
        "title": "Clever Chapter Title 79",
        "position": 1,
        "updated_at": "2016-11-03T11:27:35.172Z",
        "course_id": 142,
        "author_id": 485,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T11:27:33.866Z",
        "questions_updated_at": "2016-11-03T11:27:33.866Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 92,
        "title": "Clever Chapter Title 80",
        "position": 2,
        "updated_at": "2016-11-03T11:27:35.208Z",
        "course_id": 142,
        "author_id": 485,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T11:27:33.866Z",
        "questions_updated_at": "2016-11-03T11:27:33.866Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 485,
        "chapter_id": 91,
        "position": 54,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:34.060Z",
        "created_at": "2016-11-03T11:27:33.951Z",
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
            "id": 118,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 119,
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
        "author_id": 485,
        "chapter_id": 92,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:34.416Z",
        "created_at": "2016-11-03T11:27:34.301Z",
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
            "id": 122,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 123,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ]
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
PUT /v2/courses/139/pin
Content-Type: application/json
Authorization: Bearer f9a06c6a32fd8a24e3b9711b302e22e292375154ea938fecdd36bc5918e7d94d
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/139/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9a06c6a32fd8a24e3b9711b302e22e292375154ea938fecdd36bc5918e7d94d"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/144/pin
Content-Type: application/json
Authorization: Bearer 488767f1c5e5599115372e1def9877cd67d8ee4f135fdefeb525f9ee69242205
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/144/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 488767f1c5e5599115372e1def9877cd67d8ee4f135fdefeb525f9ee69242205"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 42577e34a850100e6a551c4daaea5f99031a04ccbbbfbab525416fec38ebda5c
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
    "creator_id": 522,
    "id": 156,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 157,
    "additional_university_ids": [

    ],
    "topic_id": 161,
    "discipline_id": 162,
    "language_code": "fr",
    "exam_months": [

    ],
    "title": "Choux pastry 102",
    "organizational_identifier": null,
    "instructor_name": "",
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
    "updated_at": "2016-11-03T11:27:38.655Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42577e34a850100e6a551c4daaea5f99031a04ccbbbfbab525416fec38ebda5c"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 006ef47d4536049f431a3ae0ff457984732c63abd30a40fb5702836543231dc9
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
    "id": 716,
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
    "created_at": "2016-11-03T11:27:50.872Z",
    "updated_at": "2016-11-03T11:27:50.872Z",
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
	-H "Authorization: Bearer 006ef47d4536049f431a3ae0ff457984732c63abd30a40fb5702836543231dc9"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 66ca22452c19f5a25185d67fde7c2678dc5ce8b6ff2a6b1607bcc99125ba1de4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[221]}
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
    "id": 717,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      221
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T11:27:50.953Z",
    "updated_at": "2016-11-03T11:27:50.991Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[221]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66ca22452c19f5a25185d67fde7c2678dc5ce8b6ff2a6b1607bcc99125ba1de4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ca428b7d54375f4c66877df20393f2e1881cf96cb98e86e65ed219be89849d4f
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
    "id": 719,
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
    "created_at": "2016-11-03T11:27:51.081Z",
    "updated_at": "2016-11-03T11:27:51.081Z",
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
	-H "Authorization: Bearer ca428b7d54375f4c66877df20393f2e1881cf96cb98e86e65ed219be89849d4f"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 2410706287dcf0e1b64ee649933cab87a18bd79011fb583c44338dee846c752d
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[224]}
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
    "id": 720,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      224
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T11:27:51.171Z",
    "updated_at": "2016-11-03T11:27:51.171Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[224]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2410706287dcf0e1b64ee649933cab87a18bd79011fb583c44338dee846c752d"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 5cfb67d1ceed32bd583eeba8ba8defe4208db0f7f2c92818f0a838c61707559c
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

225
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
    "id": 721,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/29a4bc685ff95c7a662410dec5beef37fdca879d.jpg",
    "university_id": null,
    "fields_of_study": [
      225
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T11:27:51.238Z",
    "updated_at": "2016-11-03T11:27:51.494Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/66fcc3177554204d4358d5075fb49b49c23d5aba.jpg",
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

225
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 5cfb67d1ceed32bd583eeba8ba8defe4208db0f7f2c92818f0a838c61707559c"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 12c58e594d57a4fe8c14fb7bff06c11263272ade5f4a1de914287bf9964fdec3
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
      "bookmarkable_id": 95,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 96,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 97,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12c58e594d57a4fe8c14fb7bff06c11263272ade5f4a1de914287bf9964fdec3"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 407c62e8934bb11db51dbfe2566e45ae53f2d5b489e6e63a585bfd34e2ac93ef
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
      "company_id": 13,
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
      "company_id": 14,
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
	-H "Authorization: Bearer 407c62e8934bb11db51dbfe2566e45ae53f2d5b489e6e63a585bfd34e2ac93ef"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 3192ae5983114dade9e54528b66059b59ab862891e4c4da8a1567fb1a5d21dc7
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
      "company_id": 9,
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
	-H "Authorization: Bearer 3192ae5983114dade9e54528b66059b59ab862891e4c4da8a1567fb1a5d21dc7"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 089d3d93c21821d09985659f6b0ef74be0e8fb37910eaf3c88505ea19a019d28
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
      "creator_id": 76,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-19",
      "html_url": "https://goskive.com/course/mit-course-19",
      "slug": "mit-course-19",
      "university_id": 19,
      "additional_university_ids": [

      ],
      "topic_id": 19,
      "discipline_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 19",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:27:05.370Z",
      "shortname": "mit-course-19"
    },
    {
      "creator_id": 77,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-20",
      "html_url": "https://goskive.com/course/mit-course-20",
      "slug": "mit-course-20",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:27:05.452Z",
      "shortname": "mit-course-20"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 089d3d93c21821d09985659f6b0ef74be0e8fb37910eaf3c88505ea19a019d28"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 48b1f0de43cc61e069e9ceb14582b86480efc228e4978242046f25c168f225f8
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
        "id": 7,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-11-03T11:27:44.286Z",
        "updated_at": "2016-11-03T11:27:44.286Z",
        "file_url": "memory://fd163beecae71a7245e4ff2d9ad4023e.pdf",
        "course_id": 171,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 8,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-03T11:27:44.364Z",
        "updated_at": "2016-11-03T11:27:44.364Z",
        "file_url": "memory://8d89fbbe187095c1c04f36e43383a12c.pdf",
        "course_id": 172,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 9,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-03T11:27:44.439Z",
        "updated_at": "2016-11-03T11:27:44.439Z",
        "file_url": "memory://bf8c757c13ca6c51e474af2713aed647.pdf",
        "course_id": 173,
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
	-H "Authorization: Bearer 48b1f0de43cc61e069e9ceb14582b86480efc228e4978242046f25c168f225f8"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 4f3214aa105cb99cb116fb0a0177c74459c1446220c6c922fe1a59ded7602a22
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T11:27:22.918Z"
      },
      "created_at": "2016-11-03T11:27:22.921Z",
      "updated_at": "2016-11-03T11:27:22.921Z",
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 7",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T11:27:22.928Z"
      },
      "created_at": "2016-11-03T11:27:22.931Z",
      "updated_at": "2016-11-03T11:27:22.931Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f3214aa105cb99cb116fb0a0177c74459c1446220c6c922fe1a59ded7602a22"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 59181b47cd231d15f444082459f5ddd6c1b3d69e123c5af0344472d7a8e5254c
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
      "company_id": 2,
      "company": {
        "id": 2,
        "name": "Fake Company Name 2",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T11:27:22.682Z"
      },
      "created_at": "2016-11-03T11:27:22.687Z",
      "updated_at": "2016-11-03T11:27:22.687Z",
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
      "company_id": 3,
      "company": {
        "id": 3,
        "name": "Fake Company Name 3",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-03T11:27:22.701Z"
      },
      "created_at": "2016-11-03T11:27:22.705Z",
      "updated_at": "2016-11-03T11:27:22.705Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59181b47cd231d15f444082459f5ddd6c1b3d69e123c5af0344472d7a8e5254c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer d964493c368a41179db178622378714358a1834563e77e57bb01c37545501d9d
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
      "id": 14,
      "created_at": "2016-11-03T11:27:54.596Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-11-03T11:27:54.698Z",
      "author_id": "758",
      "thread_subject_id": "224",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 15,
      "created_at": "2016-11-03T11:27:54.687Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-11-03T11:27:54.701Z",
      "author_id": "761",
      "thread_subject_id": "225",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-11-03T11:27:55.051Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-11-03T11:27:55.051Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-11-03T11:27:55.404Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-11-03T11:27:55.404Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 18,
      "created_at": "2016-11-03T11:27:55.767Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-03T11:27:55.767Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 19,
      "created_at": "2016-11-03T11:27:56.051Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 92,
      "updated_at": "2016-11-03T11:27:56.051Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-11-03T11:27:56.339Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 93,
      "updated_at": "2016-11-03T11:27:56.339Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-11-03T11:27:56.625Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 94,
      "updated_at": "2016-11-03T11:27:56.625Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d964493c368a41179db178622378714358a1834563e77e57bb01c37545501d9d"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/13
Content-Type: application/json
Authorization: Bearer e13008ae73e3c23a2f3ce678368e980b8ff297594105a1e5532d76d06c5a88e6
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-03T11:17:54.000Z"}}
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
    "id": 13,
    "created_at": "2016-11-03T11:27:54.403Z",
    "read_at": "2016-11-03T11:17:54.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 56,
    "updated_at": "2016-11-03T11:27:54.456Z",
    "author_id": "753",
    "thread_subject_id": "223",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/13" -d '{"notification":{"read_at":"2016-11-03T11:17:54.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e13008ae73e3c23a2f3ce678368e980b8ff297594105a1e5532d76d06c5a88e6"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 13c6c7876e7447de4d5401176d5f5545aed14c4b092744dd41f5c0e2849d8ae4
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
      "course_id": 210,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T11:27:50.302Z",
      "course_published": true,
      "updated_at": "2016-11-03T11:27:50.295Z"
    },
    {
      "id": 5,
      "course_id": 211,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T11:27:50.377Z",
      "course_published": true,
      "updated_at": "2016-11-03T11:27:50.370Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13c6c7876e7447de4d5401176d5f5545aed14c4b092744dd41f5c0e2849d8ae4"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 271ee88888359f7d6767a4c5f6ac025f17056c8614776846d7d6082b55327572
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
    "id": 8,
    "course_id": 215,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T11:27:50.827Z",
    "course_published": true,
    "updated_at": "2016-11-03T11:27:50.820Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 271ee88888359f7d6767a4c5f6ac025f17056c8614776846d7d6082b55327572"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer e7f200a20b7717d3e85ecaa144e572e47881e7b12446c7411a2ab673a10b0a18
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
    "course_id": 214,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-03T11:27:50.737Z",
    "course_published": true,
    "updated_at": "2016-11-03T11:27:50.727Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7f200a20b7717d3e85ecaa144e572e47881e7b12446c7411a2ab673a10b0a18"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f4c65db9b22ead15c30a7ec46e2f5603bfc4b784fff49f478c62c280404f1a23
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
      "id": 7,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 82,
      "user_id": 722
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 83,
      "user_id": 722
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 84,
      "user_id": 722
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 85,
      "user_id": 722
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4c65db9b22ead15c30a7ec46e2f5603bfc4b784fff49f478c62c280404f1a23"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/42
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
    "id": 42,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 40,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 42
      },
      {
        "id": 41,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 42
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/42" -X GET \
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
      "id": 40,
      "name": "Profit-focused contextually-based knowledge base",
      "name_translations": {
        "en": "Profit-focused contextually-based knowledge base"
      }
    },
    {
      "id": 41,
      "name": "Enhanced optimal flexibility",
      "name_translations": {
        "en": "Enhanced optimal flexibility"
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
Authorization: Bearer 4654fa5130dbc719879c1d13ed376068058132934f1d613cced7b3944ae4989f
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
    "user_id": 259,
    "feedbackable_id": 24,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-03T11:27:16.493Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/36/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4654fa5130dbc719879c1d13ed376068058132934f1d613cced7b3944ae4989f"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/32/fix
Content-Type: application/json
Authorization: Bearer 4e40d2fa74f361825db8e3e17beab6a3f230c5796b32e42a1cc9203307612587
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
    "id": 32,
    "user_id": 237,
    "feedbackable_id": 20,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-03T11:27:15.541Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/32/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e40d2fa74f361825db8e3e17beab6a3f230c5796b32e42a1cc9203307612587"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/33
Content-Type: application/json
Authorization: Bearer 2692761c59371388a911f01328f6382830eb4c055c15f6db77fffdb6a1104689
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
    "id": 33,
    "user_id": 242,
    "feedbackable_id": 21,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T11:27:15.875Z",
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
curl "api.goskive.com/v2/feedbacks/33" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2692761c59371388a911f01328f6382830eb4c055c15f6db77fffdb6a1104689"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/29/fix
Content-Type: application/json
Authorization: Bearer bdd9cfafc75bf57009713db3c3d02b3003ebecade74ad44942ccb4bab8f20c89
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
curl "api.goskive.com/v2/feedbacks/29/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdd9cfafc75bf57009713db3c3d02b3003ebecade74ad44942ccb4bab8f20c89"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/30/fix
Content-Type: application/json
Authorization: Bearer 683e5c8d8826a7dc3ddae4b39ce02259a8dbbc7389b87e08e2c2a5432fc500c1
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
curl "api.goskive.com/v2/feedbacks/30/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 683e5c8d8826a7dc3ddae4b39ce02259a8dbbc7389b87e08e2c2a5432fc500c1"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/close
Content-Type: application/json
Authorization: Bearer 516f9956a94e6ec03c36fbb2845395877137c4f6c8bd844f343851ab03250912
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
curl "api.goskive.com/v2/feedbacks/35/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 516f9956a94e6ec03c36fbb2845395877137c4f6c8bd844f343851ab03250912"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/34
Content-Type: application/json
Authorization: Bearer 76cf1c0288d9034b062b6f66ca3759e3b66f9bbbbabaa9f22f2f92246e198670
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
    "id": 34,
    "user_id": 247,
    "feedbackable_id": 22,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T11:27:16.143Z",
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
curl "api.goskive.com/v2/feedbacks/34" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76cf1c0288d9034b062b6f66ca3759e3b66f9bbbbabaa9f22f2f92246e198670"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/20
Content-Type: application/json
Authorization: Bearer 91fbac3a7dc8b33ac6d6a33b644325fbd07cf4b8bd65b87401f727a896b0753c
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
	-H "Authorization: Bearer 91fbac3a7dc8b33ac6d6a33b644325fbd07cf4b8bd65b87401f727a896b0753c"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/10/bookmark
Content-Type: application/json
Authorization: Bearer 6763c1d30f996617aaf08744895e49102c2a85c8221afd3c00c125c59f454972
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6763c1d30f996617aaf08744895e49102c2a85c8221afd3c00c125c59f454972"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/21
Content-Type: application/json
Authorization: Bearer 054e54ea8bb7f14a7e37bc1d10e578c17eff2e744de6d06759440274ad517dd8
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/21" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 054e54ea8bb7f14a7e37bc1d10e578c17eff2e744de6d06759440274ad517dd8"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/12
Content-Type: application/json
Authorization: Bearer 9bbd16e35f3d11f946e6c67b600d5d1e38560790300b6d52b66738f95830f332
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/dc9926e1fccb4e515626101d5b434cf2.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T112749Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=9db6a1a4b29abacdd42f192f730db20bd38494662ac8fb0e81d7ed241c6bb546",
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
	-H "Authorization: Bearer 9bbd16e35f3d11f946e6c67b600d5d1e38560790300b6d52b66738f95830f332"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/13/preview
Content-Type: application/json
Authorization: Bearer 9fd21375e5a651bd92651a0decb51518f56e46cba73f921a4f406d2bef3c73f1
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/a03d39cc2b07e354f27e6383d2acc862.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T112749Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=ac1a92f515b055944fa5b23b6cfcff547bc82f67ded2bfc960a88e60dcf75594",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/13/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9fd21375e5a651bd92651a0decb51518f56e46cba73f921a4f406d2bef3c73f1"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 2917e24870f038d0938eef663e72367efaee67b6c0bbeb7ce60b6623fb815af0
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
      "id": 682,
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
      "created_at": "2016-11-03T11:27:49.198Z",
      "updated_at": "2016-11-03T11:27:49.198Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-03T11:27:49.269Z",
    "updated_at": "2016-11-03T11:27:49.269Z",
    "course_id": 202,
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
	-H "Authorization: Bearer 2917e24870f038d0938eef663e72367efaee67b6c0bbeb7ce60b6623fb815af0"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/6/matched_courses?required_cu_count=2
Authorization: Bearer 1f2d4b17592dd8492b02fa5682ed0b79e478752528128daecc4cc7375f1fb71b
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
      "creator_id": 359,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "topic_id": 100,
      "discipline_id": 101,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "chapters_updated_at": "2016-11-03T11:27:24.632Z",
      "updated_at": "2016-11-03T11:27:26.131Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 364,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-e4e4ea07-c50d-4eac-8dee-f659a35cb3e4",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-e4e4ea07-c50d-4eac-8dee-f659a35cb3e4",
      "slug": "mit-the-great-british-bake-off-e4e4ea07-c50d-4eac-8dee-f659a35cb3e4",
      "university_id": 97,
      "additional_university_ids": [

      ],
      "topic_id": 101,
      "discipline_id": 102,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "chapters_updated_at": "2016-11-03T11:27:24.632Z",
      "updated_at": "2016-11-03T11:27:26.681Z",
      "shortname": "mit-the-great-british-bake-off-e4e4ea07-c50d-4eac-8dee-f659a35cb3e4"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/6/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 1f2d4b17592dd8492b02fa5682ed0b79e478752528128daecc4cc7375f1fb71b"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/11/report
Content-Type: application/json
Authorization: Bearer 96b6bde7a51e59393ba51bbeb3cda3d1e9f1ce8d507e5dad0a9f0cd57b201f6a
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
	-H "Authorization: Bearer 96b6bde7a51e59393ba51bbeb3cda3d1e9f1ce8d507e5dad0a9f0cd57b201f6a"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/17/bookmark
Content-Type: application/json
Authorization: Bearer 8aa6d7f1751fb2cee4b3caaae1c7dee3691b070725e24adf3f98f05178383bfd
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8aa6d7f1751fb2cee4b3caaae1c7dee3691b070725e24adf3f98f05178383bfd"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/18/upvote
Content-Type: application/json
Authorization: Bearer f94295a330ad12900b624b396d8942cfd2b3334f5549950a5217b7e3bf590397
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f94295a330ad12900b624b396d8942cfd2b3334f5549950a5217b7e3bf590397"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/2/comments
Content-Type: application/json
Authorization: Bearer 8d64e7716c1658cc551bdcf89f423e846114c8670c4c7e0beb326ff59d193279
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
    "author_id": 6,
    "reply_to_id": null,
    "created_at": "2016-11-03T11:27:00.429Z",
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
	-H "Authorization: Bearer 8d64e7716c1658cc551bdcf89f423e846114c8670c4c7e0beb326ff59d193279"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/comments
Content-Type: application/json
Authorization: Bearer 39814057adf2d2f541081968922ead9144a02b821ffe88e18b4f71e78e75133c
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
    "author_id": 3,
    "reply_to_id": null,
    "created_at": "2016-11-03T11:26:59.886Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 3,
      "feedbackable_id": 1,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:26:59.881Z",
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
	-H "Authorization: Bearer 39814057adf2d2f541081968922ead9144a02b821ffe88e18b4f71e78e75133c"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/5/comments
Content-Type: application/json
Authorization: Bearer 41b278cc15e894b3d8845e827aa1752690c443e158a10c044d589c881e933b0b
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
      "author_id": 19,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:01.075Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 18,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:01.059Z",
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
	-H "Authorization: Bearer 41b278cc15e894b3d8845e827aa1752690c443e158a10c044d589c881e933b0b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/3/comments
Content-Type: application/json
Authorization: Bearer 776cedc6bb5d49520b9707eca8035d17824f4df68f422702b56484877a42f778
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
	-H "Authorization: Bearer 776cedc6bb5d49520b9707eca8035d17824f4df68f422702b56484877a42f778"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/12/feedbacks
Content-Type: application/json
Authorization: Bearer 58ee047cca7d7a8ff57efbfbab4419d68617527913191c3919fcd094156693e5
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
    "id": 8,
    "user_id": 50,
    "feedbackable_id": 12,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T11:27:02.497Z",
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
curl "api.goskive.com/v2/flashcards/12/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58ee047cca7d7a8ff57efbfbab4419d68617527913191c3919fcd094156693e5"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/9/feedbacks
Content-Type: application/json
Authorization: Bearer 6ddf299733f8de6a58cefb5a2256780df958633d21a4dc344c075a4131a06714
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
      "user_id": 41,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:01.929Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 40,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:01.917Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/9/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ddf299733f8de6a58cefb5a2256780df958633d21a4dc344c075a4131a06714"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/93/votes
Content-Type: application/json
Authorization: Bearer c2c8e18cb25d9d73a99bc9bf82727c4288c0c0e4f13375a91b881764c2c6aab8
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
      "id": 22,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 93,
      "user_id": 979
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 93,
      "user_id": 978
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 93,
      "user_id": 977
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/93/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2c8e18cb25d9d73a99bc9bf82727c4288c0c0e4f13375a91b881764c2c6aab8"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/64/republish
Content-Type: application/json
Authorization: Bearer ae65aaa0ee4a54eb4a3f08b6f3f591e074e3bd4f7665f856692630ae144120e9
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
curl "api.goskive.com/v2/flashcards/64/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae65aaa0ee4a54eb4a3f08b6f3f591e074e3bd4f7665f856692630ae144120e9"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/86/bookmark
Content-Type: application/json
Authorization: Bearer d748c5049c0c48ff884e457e463e401b1a2bc0b73231f4b19311c27de21a7c18
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/86/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d748c5049c0c48ff884e457e463e401b1a2bc0b73231f4b19311c27de21a7c18"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/67
Content-Type: application/json
Authorization: Bearer 82c27ba9bf037fd1485862363287d326ecfe53452c31e78321c55acaacbdd23a
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/67" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82c27ba9bf037fd1485862363287d326ecfe53452c31e78321c55acaacbdd23a"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/84/downvote
Content-Type: application/json
Authorization: Bearer 40ba4983f21cad8f7a0697ea56ea5ed2141f0b556f9a8a0163c8954772f08ae9
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/84/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40ba4983f21cad8f7a0697ea56ea5ed2141f0b556f9a8a0163c8954772f08ae9"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/87
Content-Type: application/json
Authorization: Bearer d5061b5064bd82e4f3de0ad14aa826e371695738487ac6dbeff0c2f36af661d4
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
    "id": 87,
    "obfuscated_id": "Jisk1d9Nmeo",
    "author_id": 667,
    "chapter_id": 135,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:27:48.378Z",
    "created_at": "2016-11-03T11:27:48.378Z",
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
curl "api.goskive.com/v2/flashcards/87" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5061b5064bd82e4f3de0ad14aa826e371695738487ac6dbeff0c2f36af661d4"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/85/report
Content-Type: application/json
Authorization: Bearer f62d3534a4803d9957e5a4803016e1fab4a35bc8d839f1110cdd7dfffd495ada
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/85/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f62d3534a4803d9957e5a4803016e1fab4a35bc8d839f1110cdd7dfffd495ada"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/66/bookmark
Content-Type: application/json
Authorization: Bearer fda50bdfdcd3f99fc32d5103a9b025b494139f40fc98b594c5404b23522d9ad7
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fda50bdfdcd3f99fc32d5103a9b025b494139f40fc98b594c5404b23522d9ad7"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/83/upvote
Content-Type: application/json
Authorization: Bearer 5059ff63fd36a09dc813a78dffb76bdb0578ac77f132c7e10954ddad19348b3b
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/83/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5059ff63fd36a09dc813a78dffb76bdb0578ac77f132c7e10954ddad19348b3b"
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
    "key": "cache/50c30f2d6b044d4ffdb2caf8542cb5fe.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxMjoyNzoyNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzUwYzMwZjJkNmIwNDRkNGZmZGIyY2FmODU0MmNiNWZlLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwMy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDNUMTEyNzI2WiJ9XX0=",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T112726Z",
    "x-amz-signature": "153dd4ecdcdd62798ba5694ae8dba08c770c3cfc5b66e1d6b2c6413b9589a8fc"
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
Authorization: Bearer 20f993f80f1f89dbcfccb7874c2534a161bdbd376de4d13824917611b69c20b0
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
	-H "Authorization: Bearer 20f993f80f1f89dbcfccb7874c2534a161bdbd376de4d13824917611b69c20b0"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer ea9543d7edd2bf804633a1aa6000110b9b6ad67fa6a926cb459bac77163c0479
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
	-H "Authorization: Bearer ea9543d7edd2bf804633a1aa6000110b9b6ad67fa6a926cb459bac77163c0479"
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
{"password":{"reset_password_token":"dmyGpWKqU3bYsQHAY8C2","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 58,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-03T11:27:03.469Z",
  "updated_at": "2016-11-03T11:27:03.665Z",
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
  "audit_id": 3358
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"dmyGpWKqU3bYsQHAY8C2","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/26/comments
Content-Type: application/json
Authorization: Bearer 3e8714fced5c400ab0ff54fe26808ee3237166622d1d186c0581847729e876dc
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
    "id": 10,
    "author_id": 278,
    "reply_to_id": null,
    "created_at": "2016-11-03T11:27:18.244Z",
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
curl "api.goskive.com/v2/questions/26/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e8714fced5c400ab0ff54fe26808ee3237166622d1d186c0581847729e876dc"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer 916659a71bc7e6e271126c7364dc3ad339b89789b6b8e01925e4183ed73bdfae
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
    "author_id": 281,
    "reply_to_id": null,
    "created_at": "2016-11-03T11:27:18.715Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 281,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:18.713Z",
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
curl "api.goskive.com/v2/questions/27/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 916659a71bc7e6e271126c7364dc3ad339b89789b6b8e01925e4183ed73bdfae"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/24/comments
Content-Type: application/json
Authorization: Bearer bdc1d8b1a4ecbc06b2b48471fb5dfcd2f9be5f16e58b00085858d66d0d35895b
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
      "author_id": 273,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:17.579Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 274,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:17.593Z",
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
curl "api.goskive.com/v2/questions/24/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bdc1d8b1a4ecbc06b2b48471fb5dfcd2f9be5f16e58b00085858d66d0d35895b"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/28/comments
Content-Type: application/json
Authorization: Bearer ea0e2cbd855ba9774a5deb0516c75702b3bddffb77c601284bb9f9c993c3cd93
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
curl "api.goskive.com/v2/questions/28/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea0e2cbd855ba9774a5deb0516c75702b3bddffb77c601284bb9f9c993c3cd93"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/102/feedbacks
Content-Type: application/json
Authorization: Bearer 5510ef92f9791c7abf8ba2c9e05fba6551a9a07e00b508eeab9292acad1ac01e
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
    "user_id": 858,
    "feedbackable_id": 102,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-03T11:28:03.336Z",
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
curl "api.goskive.com/v2/questions/102/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5510ef92f9791c7abf8ba2c9e05fba6551a9a07e00b508eeab9292acad1ac01e"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/106/feedbacks
Content-Type: application/json
Authorization: Bearer 514d52e21f0e0cddd4cc9e503e4f3ee69721df3c0e968c80d5ec0602ffca6e4f
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
      "user_id": 876,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:28:04.862Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 875,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:28:04.852Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/106/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 514d52e21f0e0cddd4cc9e503e4f3ee69721df3c0e968c80d5ec0602ffca6e4f"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/87/votes
Content-Type: application/json
Authorization: Bearer d3c053cd33a2fc32da4f805020ba9eb9e9126d87ce0dcc1f538aea4e7755ae7d
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
      "votable_id": 87,
      "user_id": 744
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 87,
      "user_id": 743
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 87,
      "user_id": 742
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/87/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3c053cd33a2fc32da4f805020ba9eb9e9126d87ce0dcc1f538aea4e7755ae7d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/112/republish
Content-Type: application/json
Authorization: Bearer 4546877fcf3f65b48ca6e1351f4f759a567692e902c184fa2568bdd678e5fe41
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
curl "api.goskive.com/v2/questions/112/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4546877fcf3f65b48ca6e1351f4f759a567692e902c184fa2568bdd678e5fe41"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/133/bookmark
Content-Type: application/json
Authorization: Bearer f6050ca5ace54b844864c774e2e6ff4f1536166cf34140d0eee923f9e3e942ac
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/133/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6050ca5ace54b844864c774e2e6ff4f1536166cf34140d0eee923f9e3e942ac"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/115
Content-Type: application/json
Authorization: Bearer 1ee3aef3f25214de112e94478dd3fbf59f5953d4cd3c72b4196d9a5448df4bbd
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee3aef3f25214de112e94478dd3fbf59f5953d4cd3c72b4196d9a5448df4bbd"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/114/downvote
Content-Type: application/json
Authorization: Bearer 8137bce0d748318723a6f332f4aeae10a52f7c5b15d78a1a9a6397514c62ecee
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8137bce0d748318723a6f332f4aeae10a52f7c5b15d78a1a9a6397514c62ecee"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/117
Content-Type: application/json
Authorization: Bearer e144748958bf47c98b49912283290f6b8a0369562e1a8e5ae52b63aebc03df28
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
    "id": 117,
    "obfuscated_id": "BsA8mEPn8aM",
    "author_id": 915,
    "chapter_id": 175,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:28:08.887Z",
    "created_at": "2016-11-03T11:28:08.774Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/117" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e144748958bf47c98b49912283290f6b8a0369562e1a8e5ae52b63aebc03df28"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/116/report
Content-Type: application/json
Authorization: Bearer 07ec36a29b404787bd62085429f5a64f7aefc0fa4cb71ca4eb6d139bdfe3aa6d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/116/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07ec36a29b404787bd62085429f5a64f7aefc0fa4cb71ca4eb6d139bdfe3aa6d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/134/bookmark
Content-Type: application/json
Authorization: Bearer e6c2cab71ad376a65e0e819896208adf33c2acf9de0c59eb5032a9790df747fc
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/134/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6c2cab71ad376a65e0e819896208adf33c2acf9de0c59eb5032a9790df747fc"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/113
Content-Type: application/json
Authorization: Bearer a579b5f9ff8c21fb838ceffa3268c7d76dedce1b3c374f483ff4d99b7996db65
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":113,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T11:28:06.920Z","updated_at":"2016-11-03T11:28:07.033Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":171,"author_id":903,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 113,
    "obfuscated_id": "pcyz_ZHBlMU",
    "author_id": 903,
    "chapter_id": 171,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T11:28:07.143Z",
    "created_at": "2016-11-03T11:28:06.920Z",
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
    "question": "{\"id\"=>113, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-03T11:28:06.920Z\", \"updated_at\"=>\"2016-11-03T11:28:07.033Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>171, \"author_id\"=>903, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 228,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 229,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 230,
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
curl "api.goskive.com/v2/questions/113" -d '{"question":{"question":{"id":113,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T11:28:06.920Z","updated_at":"2016-11-03T11:28:07.033Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":171,"author_id":903,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a579b5f9ff8c21fb838ceffa3268c7d76dedce1b3c374f483ff4d99b7996db65"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/110/upvote
Content-Type: application/json
Authorization: Bearer d9d668e7a486d43caf365a0953d25403042b67ce63aad214d0a2a94b8ee23e15
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9d668e7a486d43caf365a0953d25403042b67ce63aad214d0a2a94b8ee23e15"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 1c795f224344159bd44de805bab7e7d258da3eea0525ecc112139965b16da58c
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
      "creator_id": 133,
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 36,
      "additional_university_ids": [

      ],
      "topic_id": 37,
      "discipline_id": 37,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Pizza 201",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:27:08.460Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c795f224344159bd44de805bab7e7d258da3eea0525ecc112139965b16da58c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer e016e1bc13b2ded48f390c145b8ecd59857641d8995ac91b9ebe60236c9a9164
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
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-39",
      "html_url": "https://goskive.com/university/uni-39",
      "slug": "uni-39",
      "name": "National School of Pizza",
      "short_name": "Uni 39",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a7f77c43dfd5ecc00660cdc5a443484d3d65c8a5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/5e2c981db254fae9a6b35d65b5209d2ad371995f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T11:27:08.752Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-38",
      "html_url": "https://goskive.com/university/uni-38",
      "slug": "uni-38",
      "name": "National School of Pastry",
      "short_name": "Uni 38",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/787c71b072d0ce40e1e2bb9802f2149b627b3e66.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f463301a186d609139a3c7768efe3fd07dafa7cd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T11:27:08.736Z",
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
	-H "Authorization: Bearer e016e1bc13b2ded48f390c145b8ecd59857641d8995ac91b9ebe60236c9a9164"
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
      "id": 90,
      "name": "Cloned context-sensitive architecture",
      "name_translations": {
        "en": "Cloned context-sensitive architecture"
      },
      "discipline_id": 91
    },
    {
      "id": 91,
      "name": "Virtual zero administration complexity",
      "name_translations": {
        "en": "Virtual zero administration complexity"
      },
      "discipline_id": 92
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
GET /v2/topics/89
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
    "id": 89,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 90
  }
}
```



```shell
curl "api.goskive.com/v2/topics/89" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer afd6239436bf09f8fc1d64f41be95513c636b0eff374860749926460804b4fbc
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
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-160",
      "html_url": "https://goskive.com/university/uni-160",
      "slug": "uni-160",
      "name": "University 110",
      "short_name": "Uni 160",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/9bfbdefd8ed83d51115d2b1697b6e10e94110cf9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/fe99079d3b4162005ec2237e10e5d82eefde8b15.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T11:27:39.533Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-161",
      "html_url": "https://goskive.com/university/uni-161",
      "slug": "uni-161",
      "name": "University 111",
      "short_name": "Uni 161",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4d4d3eda1827ac32038178d61d500b5c212dc135.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9a8c9fc0d6f24bf66e3d8b1d28b9bda4573bd644.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T11:27:39.548Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-162",
      "html_url": "https://goskive.com/university/uni-162",
      "slug": "uni-162",
      "name": "University 112",
      "short_name": "Uni 162",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fa194e05180078f35d9e11db8e90c4d45115e850.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1030b35556686e77f817c84b8278173c8cc1fd5d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T11:27:39.563Z",
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
	-H "Authorization: Bearer afd6239436bf09f8fc1d64f41be95513c636b0eff374860749926460804b4fbc"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 77690db88f8f9b3e9046936e349000e91bd81cdef602725a827aa8560f3f5559
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
    "id": 163,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ae8d6816a352d2aa8601d46d67d4daeda031537c.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/7aa1893c4afe2a4ac5b9bfc07801ef554100f08f.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-03T11:27:39.675Z",
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
	-H "Authorization: Bearer 77690db88f8f9b3e9046936e349000e91bd81cdef602725a827aa8560f3f5559"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 11d8c1be08f4d5b28bcb2d2c4856cc26cb8fed4a79d72ec496fde685846b4bc3
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":252,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 813,
    "id": 240,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 247,
    "additional_university_ids": [

    ],
    "topic_id": 252,
    "discipline_id": 253,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
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
    "chapters_updated_at": "2016-11-03T11:27:58.983Z",
    "updated_at": "2016-11-03T11:27:59.116Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 153,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-11-03T11:27:59.075Z",
        "course_id": 240,
        "author_id": 813,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 154,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-11-03T11:27:59.091Z",
        "course_id": 240,
        "author_id": 813,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      },
      {
        "id": 155,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-11-03T11:27:59.107Z",
        "course_id": 240,
        "author_id": 813,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":252,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11d8c1be08f4d5b28bcb2d2c4856cc26cb8fed4a79d72ec496fde685846b4bc3"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fa69ecfe98c445b1b85d52961945757d1d249fcc3a2aedf0ef3e36de6aab3c56
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":253,"published":false}}
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
    "creator_id": 814,
    "id": 241,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 248,
    "additional_university_ids": [

    ],
    "topic_id": 253,
    "discipline_id": 254,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": "",
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
    "updated_at": "2016-11-03T11:27:59.258Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":253,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa69ecfe98c445b1b85d52961945757d1d249fcc3a2aedf0ef3e36de6aab3c56"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9017e2d0e4af80fb87d2106f8b0c154715de0e567815977f50c631ab90b1654f
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
      "creator_id": 842,
      "id": 266,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-194",
      "html_url": "https://goskive.com/course/fu-course-194",
      "slug": "fu-course-194",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "topic_id": 278,
      "discipline_id": 279,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 194",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:01.652Z",
      "shortname": "fu-course-194"
    },
    {
      "creator_id": 842,
      "id": 267,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 259,
      "additional_university_ids": [

      ],
      "topic_id": 279,
      "discipline_id": 280,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "chapters_updated_at": "2016-11-03T11:28:01.932Z",
      "updated_at": "2016-11-03T11:28:01.938Z",
      "shortname": "fu-course-195"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9017e2d0e4af80fb87d2106f8b0c154715de0e567815977f50c631ab90b1654f"
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
      "creator_id": 852,
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-202",
      "html_url": "https://goskive.com/course/fu-course-202",
      "slug": "fu-course-202",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 286,
      "discipline_id": 287,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 202",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:02.483Z",
      "shortname": "fu-course-202"
    },
    {
      "creator_id": 852,
      "id": 275,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 262,
      "additional_university_ids": [

      ],
      "topic_id": 287,
      "discipline_id": 288,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "chapters_updated_at": "2016-11-03T11:28:02.764Z",
      "updated_at": "2016-11-03T11:28:02.770Z",
      "shortname": "fu-course-203"
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
Authorization: Bearer c0b9b8229fa2225a3f5e27811d264ba7a3ad35b593f5ba3b1f40056a99ece94b
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
      "creator_id": 848,
      "id": 270,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-198",
      "html_url": "https://goskive.com/course/fu-course-198",
      "slug": "fu-course-198",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 282,
      "discipline_id": 283,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 198",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:02.152Z",
      "shortname": "fu-course-198"
    },
    {
      "creator_id": 848,
      "id": 271,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 260,
      "additional_university_ids": [

      ],
      "topic_id": 283,
      "discipline_id": 284,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:02.190Z",
      "shortname": "fu-course-199"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c0b9b8229fa2225a3f5e27811d264ba7a3ad35b593f5ba3b1f40056a99ece94b"
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
      "creator_id": 857,
      "id": 278,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-206",
      "html_url": "https://goskive.com/course/fu-course-206",
      "slug": "fu-course-206",
      "university_id": 264,
      "additional_university_ids": [

      ],
      "topic_id": 290,
      "discipline_id": 291,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 206",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:02.972Z",
      "shortname": "fu-course-206"
    },
    {
      "creator_id": 857,
      "id": 279,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-207",
      "html_url": "https://goskive.com/course/fu-course-207",
      "slug": "fu-course-207",
      "university_id": 264,
      "additional_university_ids": [

      ],
      "topic_id": 291,
      "discipline_id": 292,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 207",
      "organizational_identifier": null,
      "instructor_name": "",
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
      "updated_at": "2016-11-03T11:28:03.010Z",
      "shortname": "fu-course-207"
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
Authorization: Bearer 87b22e6119b64867af0db183323139b5f3b6f0b847474da86c221ef8aaa1f371
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
  "id": 581,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-03T11:27:43.592Z",
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
	-H "Authorization: Bearer 87b22e6119b64867af0db183323139b5f3b6f0b847474da86c221ef8aaa1f371"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/809
Content-Type: application/json
Authorization: Bearer 307709822c0e2f624cfa0eb5cd5fa1e3d3cded60932cf253e790621b17a6abf0
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
    "id": 809,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 246,
    "fields_of_study": [
      250,
      251
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-03T11:27:58.854Z",
    "updated_at": "2016-11-03T11:27:58.854Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/809" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 307709822c0e2f624cfa0eb5cd5fa1e3d3cded60932cf253e790621b17a6abf0"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/811
Content-Type: application/json
Authorization: Bearer 67a31533ed1f1df0cde697cebb6695375482405aceb22179dd7ed7448567e792
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
    "id": 811,
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
    "created_at": "2016-11-03T11:27:58.936Z",
    "updated_at": "2016-11-03T11:27:58.936Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/811" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67a31533ed1f1df0cde697cebb6695375482405aceb22179dd7ed7448567e792"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/1
Content-Type: application/json
Authorization: Bearer d3508fc184ff9f8df2da5a0a866ec8a95fc677f096be7c6cb6e5b9477a8f34c8
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3508fc184ff9f8df2da5a0a866ec8a95fc677f096be7c6cb6e5b9477a8f34c8"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/3
Content-Type: application/json
Authorization: Bearer a3485071c84a6477ad6aecce2baecb6e894f4b20491d12b114f88fbe4df7acc2
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
    "id": 3,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 81,
    "user_id": 577
  }
}
```



```shell
curl "api.goskive.com/v2/votes/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3485071c84a6477ad6aecce2baecb6e894f4b20491d12b114f88fbe4df7acc2"
```
