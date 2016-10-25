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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"b48136a5196528daebdf5546a3319015d28760c87902df3026b2646aa2d85590","client_secret":"06c5b439d2ecd0b5aa56788c9fb3f9ebe440b3cbc16f6cc645aee51f3e3a6c46"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"b48136a5196528daebdf5546a3319015d28760c87902df3026b2646aa2d85590","client_secret":"06c5b439d2ecd0b5aa56788c9fb3f9ebe440b3cbc16f6cc645aee51f3e3a6c46"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NzNiOGY4YTgyNjIwNmZjODM0MWE0ODhhMzM1MGQ4NjJjMjdjNTNmMWNlOTY2
ZGUzYWJmMGRkN2YzMjJmOTA5MDplYzNhMjhlZDk1YTE0YjI0N2I3NDM1N2Rl
NGNlZmI5MTRhZDdlOGJhMThmNTg1ODNmN2YwZjQ3ODM2NzExMjc5

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
	-u 73b8f8a826206fc8341a488a3350d862c27c53f1ce966de3abf0dd7f322f9090:ec3a28ed95a14b247b74357de4cefb914ad7e8ba18f58583f7f0f47836711279
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
{"grant_type":"client_credentials","client_id":"f719c2bb314a565da77b66648f47147f7b82e3026b45e93461cf14bd4292f7e1","client_secret":"595af101d9c4cab292005211e6843da05a02511c230c3ad8fb6163d3036af2a7"}
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
  "access_token": "39fa1911f820a2d82036a73727163d0b763d27f8333384bc9d5e14e7c441c165",
  "token_type": "bearer",
  "created_at": 1477427521
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"f719c2bb314a565da77b66648f47147f7b82e3026b45e93461cf14bd4292f7e1","client_secret":"595af101d9c4cab292005211e6843da05a02511c230c3ad8fb6163d3036af2a7"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"70628c3380709a4e66033cf35acf061eaddfde80c0ce51b9dc446a0dc9594713","client_secret":"c6c167fd3f76d4c2990dbcad6d1be72d49c167def4e1f75862061ca250402f76"}
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
  "access_token": "5179ee52574a09f8cd1473420c0b20f37d91beef25d6cf03146e07cb859d36d6",
  "token_type": "bearer",
  "created_at": 1477427521
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"70628c3380709a4e66033cf35acf061eaddfde80c0ce51b9dc446a0dc9594713","client_secret":"c6c167fd3f76d4c2990dbcad6d1be72d49c167def4e1f75862061ca250402f76"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTIwZjdkMjEzOWVmN2JhMWFkNDBmM2RmYWJjNGRjNDNjMmQwNDIxZjMyYTlh
NWMzNjgxZjE5Mjg5Mjk3NWMyNDo3NTgzNDEzNjRkMzg4NGRlMWMzOWYwNGUy
MDVjYWZkZGNiNzlhOTFlNGYzMmEwZTU2ZjYwNzAyNjhhYmM3YmVm

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
  "access_token": "d9d130a60cf1ba0918fab4e5e0159c0f9c2d65b8f182c142db5488857412b931",
  "token_type": "bearer",
  "created_at": 1477427521
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 920f7d2139ef7ba1ad40f3dfabc4dc43c2d0421f32a9a5c3681f192892975c24:758341364d3884de1c39f04e205cafddcb79a91e4f32a0e56f6070268abc7bef
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
Authorization: Bearer 552ec5cfca2347ec35efe7fa24b1297c31d4777736ebef82067e53e3942e908d
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
curl "api.goskive.com/v2/campaigns/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 552ec5cfca2347ec35efe7fa24b1297c31d4777736ebef82067e53e3942e908d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/100/flashcards
Content-Type: application/json
Authorization: Bearer edec9e528436d01e7c31aa3a4e60518f380929ef8a8c89007a995e57a2abf8e5
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":100,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 52,
    "obfuscated_id": "_rmh4zxMC_8",
    "author_id": 516,
    "chapter_id": 100,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:32:13.028Z",
    "created_at": "2016-10-25T20:32:13.028Z",
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
curl "api.goskive.com/v2/chapters/100/flashcards" -d '{"flashcard":{"chapter_id":100,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edec9e528436d01e7c31aa3a4e60518f380929ef8a8c89007a995e57a2abf8e5"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/99/flashcards
Content-Type: application/json
Authorization: Bearer a10a13977f264ed89c31efce01dff8c9646ea95727860239ecb6f821fcffa4dc
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 511,
      "chapter_id": 99,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:12.711Z",
      "created_at": "2016-10-25T20:32:12.711Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 511,
      "chapter_id": 99,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:12.749Z",
      "created_at": "2016-10-25T20:32:12.749Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 511,
      "chapter_id": 99,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:12.787Z",
      "created_at": "2016-10-25T20:32:12.787Z",
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
curl "api.goskive.com/v2/chapters/99/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a10a13977f264ed89c31efce01dff8c9646ea95727860239ecb6f821fcffa4dc"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/30/questions
Content-Type: application/json
Authorization: Bearer d4e76630749e531ddb5a951f7441f48f28523c2e114ff87d455136520b43fd3e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":30,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 15,
    "obfuscated_id": "j5PwoYQzNCc",
    "author_id": 212,
    "chapter_id": 30,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:45.714Z",
    "created_at": "2016-10-25T20:31:45.714Z",
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
        "id": 30,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 31,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 32,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 33,
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
curl "api.goskive.com/v2/chapters/30/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":30,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4e76630749e531ddb5a951f7441f48f28523c2e114ff87d455136520b43fd3e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/27/questions
Content-Type: application/json
Authorization: Bearer e63e7304aa1da790c7932c08599baa2f9136a55753083fe140cd2f250ea8423d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":27,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 12,
    "obfuscated_id": "4vzz6KHlMwo",
    "author_id": 203,
    "chapter_id": 27,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:44.604Z",
    "created_at": "2016-10-25T20:31:44.604Z",
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
        "id": 23,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 24,
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
curl "api.goskive.com/v2/chapters/27/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":27,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e63e7304aa1da790c7932c08599baa2f9136a55753083fe140cd2f250ea8423d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/28/questions
Content-Type: application/json
Authorization: Bearer b70041c6ee8d7c839c76822a0c96f713bda61ed2b2d58ba5d7f00e8e4a44f468
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":28,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 206,
    "chapter_id": 28,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:44.960Z",
    "created_at": "2016-10-25T20:31:44.960Z",
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
        "id": 25,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 26,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/28/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":28,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b70041c6ee8d7c839c76822a0c96f713bda61ed2b2d58ba5d7f00e8e4a44f468"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/29/questions
Content-Type: application/json
Authorization: Bearer 46ffd46ab26a7206bb2013f595195c53f7cbb07a5aa8be8b1bbe6ba88ebbc574
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":29,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 14,
    "obfuscated_id": "gbKzjBR_8tw",
    "author_id": 209,
    "chapter_id": 29,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:45.300Z",
    "created_at": "2016-10-25T20:31:45.300Z",
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
        "id": 27,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 28,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 29,
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
curl "api.goskive.com/v2/chapters/29/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":29,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46ffd46ab26a7206bb2013f595195c53f7cbb07a5aa8be8b1bbe6ba88ebbc574"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/25/questions
Content-Type: application/json
Authorization: Bearer 386ed8815975d339e9c5775a7dc80663897db5924d7cc1544d18762252c1cefc
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
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 194,
      "chapter_id": 25,
      "position": 9,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:43.726Z",
      "created_at": "2016-10-25T20:31:43.599Z",
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
    },
    {
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 195,
      "chapter_id": 25,
      "position": 10,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:43.931Z",
      "created_at": "2016-10-25T20:31:43.805Z",
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
          "id": 19,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 20,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 196,
      "chapter_id": 25,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:44.143Z",
      "created_at": "2016-10-25T20:31:44.007Z",
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
          "id": 21,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 22,
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
curl "api.goskive.com/v2/chapters/25/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 386ed8815975d339e9c5775a7dc80663897db5924d7cc1544d18762252c1cefc"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 94ee8e8695bc6f61f4bc7c893117066755c4464e94ff85ad34164efb4eaff192
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
curl "api.goskive.com/v2/chapters/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94ee8e8695bc6f61f4bc7c893117066755c4464e94ff85ad34164efb4eaff192"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 38948b9029fbf66a3c9a7197e396d6755ddfe7b4403c59fb76d63edd057ab2b0
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
curl "api.goskive.com/v2/chapters/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38948b9029fbf66a3c9a7197e396d6755ddfe7b4403c59fb76d63edd057ab2b0"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/6
Content-Type: application/json
Authorization: Bearer 5669d6283c77dcc676f38b039bd6bcfddac88f1ae3c91fb7199d64a316b81885
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
curl "api.goskive.com/v2/chapters/6" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5669d6283c77dcc676f38b039bd6bcfddac88f1ae3c91fb7199d64a316b81885"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/10
Content-Type: application/json
Authorization: Bearer 238a01b583efc4c8c8362d7d75d0617c2e32c31bd0a22b3c73ff978ac8fae3b5
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 238a01b583efc4c8c8362d7d75d0617c2e32c31bd0a22b3c73ff978ac8fae3b5"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/2
Content-Type: application/json
Authorization: Bearer 4e6637874463b0a3f16a5e9beb9394744effd7b3c173527eaa0db9d1cba932d4
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
    "id": 2,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T20:31:37.183Z",
    "course_id": 43,
    "author_id": 99,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-25T20:31:36.566Z",
    "questions_updated_at": "2016-10-25T20:31:36.566Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 103,
        "chapter_id": 2,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.165Z",
        "created_at": "2016-10-25T20:31:37.165Z",
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
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 101,
        "chapter_id": 2,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.029Z",
        "created_at": "2016-10-25T20:31:36.900Z",
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
}
```



```shell
curl "api.goskive.com/v2/chapters/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e6637874463b0a3f16a5e9beb9394744effd7b3c173527eaa0db9d1cba932d4"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/4
Content-Type: application/json
Authorization: Bearer 4711518e285cfaf3718b6cb42f4bd9dec5d471f7760d7a091856c5a3b4d10884
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
    "id": 4,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T20:31:38.172Z",
    "course_id": 45,
    "author_id": 113,
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
curl "api.goskive.com/v2/chapters/4" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4711518e285cfaf3718b6cb42f4bd9dec5d471f7760d7a091856c5a3b4d10884"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/52/replies
Content-Type: application/json
Authorization: Bearer 4d827ed46d664e28cc8d6071496f29fd0afbf8eff0d9430aedbdad481694ddcc
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
    "author_id": 521,
    "reply_to_id": 52,
    "created_at": "2016-10-25T20:32:13.479Z",
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
	-H "Authorization: Bearer 4d827ed46d664e28cc8d6071496f29fd0afbf8eff0d9430aedbdad481694ddcc"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/54/replies
Content-Type: application/json
Authorization: Bearer b432a266b0f49bfa886a8671f2ead619db33b5ad633cae837bd9bb03aa0c419f
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
curl "api.goskive.com/v2/comments/54/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b432a266b0f49bfa886a8671f2ead619db33b5ad633cae837bd9bb03aa0c419f"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/41
Content-Type: application/json
Authorization: Bearer 182dfcbbf2bf687f99d85d5b2bc67dd0aef2ac4556a529409a435738e200a7ad
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
curl "api.goskive.com/v2/comments/41" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 182dfcbbf2bf687f99d85d5b2bc67dd0aef2ac4556a529409a435738e200a7ad"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/37/republish
Content-Type: application/json
Authorization: Bearer 7a8fe49b94e12a97cc072aec7e7a964625843aec2b40ed107da9d9164b24ed45
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
curl "api.goskive.com/v2/comments/37/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a8fe49b94e12a97cc072aec7e7a964625843aec2b40ed107da9d9164b24ed45"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/39
Content-Type: application/json
Authorization: Bearer fcdd978d16f68ef33e26aff869f445ef032ab22ebcb52ae6fb5b46ff8e69ed06
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/39" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcdd978d16f68ef33e26aff869f445ef032ab22ebcb52ae6fb5b46ff8e69ed06"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/38/report
Content-Type: application/json
Authorization: Bearer 5a79ed80975f7eba1c564fee0b7b38e45681f3bc351c7b33fe447be0ce9d7848
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/38/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a79ed80975f7eba1c564fee0b7b38e45681f3bc351c7b33fe447be0ce9d7848"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer 35e85e116d215ebde912fcce940709dfd8191fc9687122873772dcd028c638ea
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
    "id": 4,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-25T20:31:58.255Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 35e85e116d215ebde912fcce940709dfd8191fc9687122873772dcd028c638ea"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 94c8e5f2eaa5b9ac74e4409c4ba640d797d4ec784aab8a09d30535b8bd09bb97
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
      "id": 1,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3a0f39043c0ca2c128a5ff9758d4ae685c4b7f2d.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:31:58.188Z"
    },
    {
      "id": 2,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:31:58.194Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T20:31:58.198Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94c8e5f2eaa5b9ac74e4409c4ba640d797d4ec784aab8a09d30535b8bd09bb97"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/27/company_profiles
Content-Type: application/json
Authorization: Bearer 441bc127389912d5b875484828358fbbba2475d04229bb4eb9e907557f8014ae
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
	-H "Authorization: Bearer 441bc127389912d5b875484828358fbbba2475d04229bb4eb9e907557f8014ae"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/25/company_profiles
Content-Type: application/json
Authorization: Bearer 65d37b8cc7b351072259539b0be1bb81ce6596407edca2bca6a2b9b300e1341c
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
	-H "Authorization: Bearer 65d37b8cc7b351072259539b0be1bb81ce6596407edca2bca6a2b9b300e1341c"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 6a2255e97dda9d8ca424b4481fbb67d13f40881bca9a3a5b6aafa3808a564edd
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
      "id": 9,
      "title": "Campaign 8",
      "company_id": 34,
      "precluded_campaign_ids": [

      ],
      "company_profiles": [
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
      "id": 12,
      "title": "Campaign 11",
      "company_id": 37,
      "precluded_campaign_ids": [

      ],
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
	-H "Authorization: Bearer 6a2255e97dda9d8ca424b4481fbb67d13f40881bca9a3a5b6aafa3808a564edd"
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
Authorization: Bearer 506e75eceefd971723c151b843a88ec7ebc60eb16ffaf87e81b92454e43b5802
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
	-H "Authorization: Bearer 506e75eceefd971723c151b843a88ec7ebc60eb16ffaf87e81b92454e43b5802"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 26347d2efa163dab07c01999be7b5701f5f6cda9e82610d202a389f3ba1fe4fd
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
    "id": 172,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:32:47.069Z",
    "course_id": 287,
    "author_id": 882,
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
	-H "Authorization: Bearer 26347d2efa163dab07c01999be7b5701f5f6cda9e82610d202a389f3ba1fe4fd"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1bc2870acbbc5079dfe0c285812526ec9ef4640ba9e5b1fa4123cab63da99543
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
      "id": 183,
      "title": "Clever Chapter Title 159",
      "position": 1,
      "updated_at": "2016-10-25T20:32:48.315Z",
      "course_id": 294,
      "author_id": 907,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 184,
      "title": "Clever Chapter Title 160",
      "position": 2,
      "updated_at": "2016-10-25T20:32:48.339Z",
      "course_id": 294,
      "author_id": 908,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 185,
      "title": "Clever Chapter Title 161",
      "position": 3,
      "updated_at": "2016-10-25T20:32:48.599Z",
      "course_id": 294,
      "author_id": 909,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T20:32:48.243Z",
      "questions_updated_at": "2016-10-25T20:32:48.243Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bc2870acbbc5079dfe0c285812526ec9ef4640ba9e5b1fa4123cab63da99543"
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
      "id": 189,
      "title": "Clever Chapter Title 165",
      "position": 1,
      "updated_at": "2016-10-25T20:32:49.086Z",
      "course_id": 297,
      "author_id": 921,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 190,
      "title": "Clever Chapter Title 166",
      "position": 2,
      "updated_at": "2016-10-25T20:32:49.112Z",
      "course_id": 297,
      "author_id": 922,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 191,
      "title": "Clever Chapter Title 167",
      "position": 3,
      "updated_at": "2016-10-25T20:32:49.377Z",
      "course_id": 297,
      "author_id": 923,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T20:32:49.006Z",
      "questions_updated_at": "2016-10-25T20:32:49.006Z",
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
Authorization: Bearer 7bb493aeb4964bd202c16c24c990185190e2cf1cc596c3f16e7e55ba6143d5ad
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
      "id": 186,
      "title": "Clever Chapter Title 162",
      "position": 1,
      "updated_at": "2016-10-25T20:32:48.760Z",
      "course_id": 295,
      "author_id": 914,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 187,
      "title": "Clever Chapter Title 163",
      "position": 2,
      "updated_at": "2016-10-25T20:32:48.785Z",
      "course_id": 295,
      "author_id": 915,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 188,
      "title": "Clever Chapter Title 164",
      "position": 3,
      "updated_at": "2016-10-25T20:32:48.810Z",
      "course_id": 295,
      "author_id": 916,
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
	-H "Authorization: Bearer 7bb493aeb4964bd202c16c24c990185190e2cf1cc596c3f16e7e55ba6143d5ad"
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
      "id": 192,
      "title": "Clever Chapter Title 168",
      "position": 1,
      "updated_at": "2016-10-25T20:32:49.587Z",
      "course_id": 299,
      "author_id": 928,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 193,
      "title": "Clever Chapter Title 169",
      "position": 2,
      "updated_at": "2016-10-25T20:32:49.612Z",
      "course_id": 299,
      "author_id": 929,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 194,
      "title": "Clever Chapter Title 170",
      "position": 3,
      "updated_at": "2016-10-25T20:32:49.637Z",
      "course_id": 299,
      "author_id": 930,
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
Authorization: Bearer 3eae3cf029af0f80efb1e040ac7b339ca3f755ef72c3c797900a0a8655cefaf8
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
    "course_id": 304,
    "user_id": 950,
    "updated_at": "2016-10-25T20:32:51.312Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eae3cf029af0f80efb1e040ac7b339ca3f755ef72c3c797900a0a8655cefaf8"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 6b7b710191a0f5ee756786e4d8d9fccd12d87d7dcf587ae097c2188f0d5b14ac
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
      "course_id": 302,
      "user_id": 944,
      "updated_at": "2016-10-25T20:32:50.992Z"
    },
    {
      "id": 4,
      "course_id": 302,
      "user_id": 945,
      "updated_at": "2016-10-25T20:32:51.007Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b7b710191a0f5ee756786e4d8d9fccd12d87d7dcf587ae097c2188f0d5b14ac"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/134/files
Content-Type: application/json
Authorization: Bearer 4ef44ba18de9dee8031e83470e5b579e27899fd652d14c64742af828a453353a
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
        "id": 436,
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
        "created_at": "2016-10-25T20:32:06.748Z",
        "updated_at": "2016-10-25T20:32:06.748Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:32:06.759Z",
      "updated_at": "2016-10-25T20:32:06.759Z",
      "course_id": 134,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 5,
      "uploader": {
        "id": 437,
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
        "created_at": "2016-10-25T20:32:06.767Z",
        "updated_at": "2016-10-25T20:32:06.767Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:32:06.777Z",
      "updated_at": "2016-10-25T20:32:06.777Z",
      "course_id": 134,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 6,
      "uploader": {
        "id": 438,
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
        "created_at": "2016-10-25T20:32:06.784Z",
        "updated_at": "2016-10-25T20:32:06.784Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T20:32:06.794Z",
      "updated_at": "2016-10-25T20:32:06.794Z",
      "course_id": 134,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/134/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ef44ba18de9dee8031e83470e5b579e27899fd652d14c64742af828a453353a"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/132/files
Content-Type: application/json
Authorization: Bearer 46258b49e006ea0842a0e936baffc28fe697b4a725970c1bb2eda8ae48092d87
```

`POST /v2/courses/:course_id/files`

#### Parameters


```json
{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}
```


| Name | Description |
|:-----|:------------|
| file[category]  | Category: summary|assignment|exam|other |
| file[filename]  | Filename |
| file[file_url]  | URL to the file in cache on S3 |



### Response

```
Content-Type: application/json; charset=utf-8
201 Created
```


```json
{
  "file": {
    "id": 3,
    "uploader": {
      "id": 432,
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
      "created_at": "2016-10-25T20:32:06.438Z",
      "updated_at": "2016-10-25T20:32:06.438Z"
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
    "created_at": "2016-10-25T20:32:06.482Z",
    "updated_at": "2016-10-25T20:32:06.482Z",
    "course_id": 132,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/132/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46258b49e006ea0842a0e936baffc28fe697b4a725970c1bb2eda8ae48092d87"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/135/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 367e7b4912baf885ba707150fc675983c26fe59041f911a76f5611778323298e
```

`GET /v2/courses/:course_id/file_upload/cache/presign`

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
    "key": "cache/b8a81ae09305a09eaa6ee187693fe2b2.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQyMTozMjowNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I4YTgxYWUwOTMwNWEwOWVhYTZlZTE4NzY5M2ZlMmIyLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI1VDIwMzIwNloifV19",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T203206Z",
    "x-amz-signature": "1a6bae74d9739418274212821f278d189402f03c2087f24a275ef30871a656e5"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/135/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 367e7b4912baf885ba707150fc675983c26fe59041f911a76f5611778323298e"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 9f01db2283e28952e0fb8cc99c3fe2b70e37d693b67fb7856a733574885c5212
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
	-H "Authorization: Bearer 9f01db2283e28952e0fb8cc99c3fe2b70e37d693b67fb7856a733574885c5212"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 01eacfedfa31c858c5249c6a97b54c8b9191e11ee61971399da25bf767fb91ed
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
	-H "Authorization: Bearer 01eacfedfa31c858c5249c6a97b54c8b9191e11ee61971399da25bf767fb91ed"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 68da9d1ed3d0560eabff96f67619c621c966aa956a416a4a362a12c87f3c1368
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
	-H "Authorization: Bearer 68da9d1ed3d0560eabff96f67619c621c966aa956a416a4a362a12c87f3c1368"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ea8c5b7d52cfd54a27eca7e644477ae55b9f389ad9613beef09e674a89a8cbc3
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
	-H "Authorization: Bearer ea8c5b7d52cfd54a27eca7e644477ae55b9f389ad9613beef09e674a89a8cbc3"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a2f63a071b5d1ad339f9ea4590ecef783ac19f7af9976d1c0222c1d8a776998b
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
	-H "Authorization: Bearer a2f63a071b5d1ad339f9ea4590ecef783ac19f7af9976d1c0222c1d8a776998b"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 94b33aa8681a8b46366784f68e16256927e657681fc1c19ec0edabee42269412
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
    "creator_id": 572,
    "id": 177,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 184,
    "additional_university_ids": [

    ],
    "topic_id": 181,
    "discipline_id": 182,
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
    "chapters_updated_at": "2016-10-25T20:32:19.188Z",
    "updated_at": "2016-10-25T20:32:20.682Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 112,
        "title": "Clever Chapter Title 94",
        "position": 1,
        "updated_at": "2016-10-25T20:32:20.633Z",
        "course_id": 177,
        "author_id": 572,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:32:19.188Z",
        "questions_updated_at": "2016-10-25T20:32:19.188Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 113,
        "title": "Clever Chapter Title 95",
        "position": 2,
        "updated_at": "2016-10-25T20:32:20.674Z",
        "course_id": 177,
        "author_id": 572,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:32:19.188Z",
        "questions_updated_at": "2016-10-25T20:32:19.188Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 573,
        "chapter_id": 112,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:20.463Z",
        "created_at": "2016-10-25T20:32:20.463Z",
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
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 573,
        "chapter_id": 113,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:20.538Z",
        "created_at": "2016-10-25T20:32:20.538Z",
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
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 573,
        "chapter_id": 112,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:20.505Z",
        "created_at": "2016-10-25T20:32:20.505Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 573,
        "chapter_id": 113,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:20.580Z",
        "created_at": "2016-10-25T20:32:20.580Z",
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
        "author_id": 573,
        "chapter_id": 112,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:19.413Z",
        "created_at": "2016-10-25T20:32:19.293Z",
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
        "author_id": 573,
        "chapter_id": 112,
        "position": 61,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:19.592Z",
        "created_at": "2016-10-25T20:32:19.481Z",
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
        "author_id": 573,
        "chapter_id": 113,
        "position": 62,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:19.802Z",
        "created_at": "2016-10-25T20:32:19.675Z",
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
        "author_id": 573,
        "chapter_id": 113,
        "position": 63,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:19.989Z",
        "created_at": "2016-10-25T20:32:19.869Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94b33aa8681a8b46366784f68e16256927e657681fc1c19ec0edabee42269412"
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
    "creator_id": 584,
    "id": 179,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 186,
    "additional_university_ids": [

    ],
    "topic_id": 183,
    "discipline_id": 184,
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
    "chapters_updated_at": "2016-10-25T20:32:22.397Z",
    "updated_at": "2016-10-25T20:32:23.852Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 116,
        "title": "Clever Chapter Title 98",
        "position": 1,
        "updated_at": "2016-10-25T20:32:23.802Z",
        "course_id": 179,
        "author_id": 584,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:32:22.397Z",
        "questions_updated_at": "2016-10-25T20:32:22.397Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 117,
        "title": "Clever Chapter Title 99",
        "position": 2,
        "updated_at": "2016-10-25T20:32:23.844Z",
        "course_id": 179,
        "author_id": 584,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T20:32:22.397Z",
        "questions_updated_at": "2016-10-25T20:32:22.397Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 584,
        "chapter_id": 116,
        "position": 72,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.599Z",
        "created_at": "2016-10-25T20:32:22.486Z",
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
            "id": 173,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 174,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 584,
        "chapter_id": 117,
        "position": 74,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.994Z",
        "created_at": "2016-10-25T20:32:22.877Z",
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
            "id": 177,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 178,
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
PUT /v2/courses/184/pin
Content-Type: application/json
Authorization: Bearer 9c837bc8c3ab79a119ea7cdf3444d5e75cc13e892299fc8f3729d2d9dc1804a2
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/184/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c837bc8c3ab79a119ea7cdf3444d5e75cc13e892299fc8f3729d2d9dc1804a2"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/175/pin
Content-Type: application/json
Authorization: Bearer 7b1aa85c215eaf99d22c59ce79f5c7029d404a562b8656e633b4bec2290b2186
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/175/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b1aa85c215eaf99d22c59ce79f5c7029d404a562b8656e633b4bec2290b2186"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e788ba62211677dcd927cb0c3b73e3c42eb70d3c2ae0e721e530c1b41cf87a65
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
    "creator_id": 593,
    "id": 182,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 189,
    "additional_university_ids": [

    ],
    "topic_id": 186,
    "discipline_id": 187,
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
    "updated_at": "2016-10-25T20:32:24.269Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e788ba62211677dcd927cb0c3b73e3c42eb70d3c2ae0e721e530c1b41cf87a65"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer f99c50ff2dc17db9e3cd876539fdf5a1b1f235a2c44a3d526bbe7b4e3a307ac7
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
    "id": 936,
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
    "created_at": "2016-10-25T20:32:50.423Z",
    "updated_at": "2016-10-25T20:32:50.423Z",
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
	-H "Authorization: Bearer f99c50ff2dc17db9e3cd876539fdf5a1b1f235a2c44a3d526bbe7b4e3a307ac7"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8ea973047ce229519ce078907c31f8e53f71480fca00c476bf1e497014364b22
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[304]}
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
    "id": 931,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      304
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:32:49.711Z",
    "updated_at": "2016-10-25T20:32:49.769Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[304]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ea973047ce229519ce078907c31f8e53f71480fca00c476bf1e497014364b22"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer c128db005a9d475af6e818c1e3cb00d623178d0d0cced1d6aceea9e83702f7ac
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
    "id": 934,
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
    "created_at": "2016-10-25T20:32:49.994Z",
    "updated_at": "2016-10-25T20:32:49.994Z",
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
	-H "Authorization: Bearer c128db005a9d475af6e818c1e3cb00d623178d0d0cced1d6aceea9e83702f7ac"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8fae7029070f4dbaefc7e43c285d76a0fe2388e055769f03bc02205f1759b820
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[305]}
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
    "id": 932,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      305
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:32:49.828Z",
    "updated_at": "2016-10-25T20:32:49.828Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[305]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fae7029070f4dbaefc7e43c285d76a0fe2388e055769f03bc02205f1759b820"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer bd4bb652f9f5306c1453ba688040318ee958a1aacda3910d86bfd3d2709816db
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

308
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
    "id": 935,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/500d6d067e23ade2d6e3129f4c8a072c2feea42b.jpg",
    "university_id": null,
    "fields_of_study": [
      308
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T20:32:50.097Z",
    "updated_at": "2016-10-25T20:32:50.391Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/76c117df340c49148a9e8c675973dc185d3ae0cd.jpg",
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

308
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer bd4bb652f9f5306c1453ba688040318ee958a1aacda3910d86bfd3d2709816db"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 786b2ece445f23b277568f2b2d3032b0f943b83fe9b943532bcdf30ff1f00647
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
      "id": 5,
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 786b2ece445f23b277568f2b2d3032b0f943b83fe9b943532bcdf30ff1f00647"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b5cca727a197f45086a4d9c2e3138cf8a8e3421dd150a1a3ea0a9fdaa3a2b90c
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
      "company_id": 20,
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
      "company_id": 21,
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
	-H "Authorization: Bearer b5cca727a197f45086a4d9c2e3138cf8a8e3421dd150a1a3ea0a9fdaa3a2b90c"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 9a9804759a4fb1c4950c78fbb8d99d969a0d9d22add4d07be8226e9d6c4bfb1c
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
      "company_id": 16,
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
	-H "Authorization: Bearer 9a9804759a4fb1c4950c78fbb8d99d969a0d9d22add4d07be8226e9d6c4bfb1c"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer c3aad30c22e608f5a6a5e943d72200850fe8d18a43db76660a341644815afbcd
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
      "creator_id": 962,
      "id": 306,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-234",
      "html_url": "https://goskive.com/course/mit-course-234",
      "slug": "mit-course-234",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "topic_id": 318,
      "discipline_id": 319,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 234",
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
      "updated_at": "2016-10-25T20:32:53.728Z",
      "shortname": "mit-course-234"
    },
    {
      "creator_id": 963,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-235",
      "html_url": "https://goskive.com/course/mit-course-235",
      "slug": "mit-course-235",
      "university_id": 292,
      "additional_university_ids": [

      ],
      "topic_id": 319,
      "discipline_id": 320,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 235",
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
      "updated_at": "2016-10-25T20:32:53.813Z",
      "shortname": "mit-course-235"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3aad30c22e608f5a6a5e943d72200850fe8d18a43db76660a341644815afbcd"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer cd69d724e28f7345b02dd492ceeece14fa4cca8c457025d55ba3e5dcc9284705
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
      "company_id": 13,
      "company": {
        "id": 13,
        "name": "Fake Company Name 12",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T20:32:01.032Z"
      },
      "created_at": "2016-10-25T20:32:01.036Z",
      "updated_at": "2016-10-25T20:32:01.036Z",
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 13",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T20:32:01.045Z"
      },
      "created_at": "2016-10-25T20:32:01.049Z",
      "updated_at": "2016-10-25T20:32:01.049Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd69d724e28f7345b02dd492ceeece14fa4cca8c457025d55ba3e5dcc9284705"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 24380e022eed22da0f9d240bb1ffad27573a840c293f1c8fffe943324a1c3a5c
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
      "company_id": 9,
      "company": {
        "id": 9,
        "name": "Fake Company Name 8",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T20:32:00.801Z"
      },
      "created_at": "2016-10-25T20:32:00.805Z",
      "updated_at": "2016-10-25T20:32:00.805Z",
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T20:32:00.819Z"
      },
      "created_at": "2016-10-25T20:32:00.823Z",
      "updated_at": "2016-10-25T20:32:00.823Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24380e022eed22da0f9d240bb1ffad27573a840c293f1c8fffe943324a1c3a5c"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 73eb404be8683d43d7bdeed39ac077dbbe7064463fc1038cde1f261901b65947
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
      "created_at": "2016-10-25T20:32:29.069Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-10-25T20:32:29.183Z",
      "author_id": "646",
      "thread_subject_id": "225",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 17,
      "created_at": "2016-10-25T20:32:29.171Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-10-25T20:32:29.187Z",
      "author_id": "649",
      "thread_subject_id": "226",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-25T20:32:29.565Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-25T20:32:29.565Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-10-25T20:32:29.951Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-25T20:32:29.951Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 20,
      "created_at": "2016-10-25T20:32:30.365Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-25T20:32:30.365Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 21,
      "created_at": "2016-10-25T20:32:30.665Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 98,
      "updated_at": "2016-10-25T20:32:30.665Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-25T20:32:30.982Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 99,
      "updated_at": "2016-10-25T20:32:30.982Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-10-25T20:32:31.291Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 100,
      "updated_at": "2016-10-25T20:32:31.291Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73eb404be8683d43d7bdeed39ac077dbbe7064463fc1038cde1f261901b65947"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/24
Content-Type: application/json
Authorization: Bearer 7d39757afb26222ec4b5994d4ebdf6d6deb1bb8a1b246bf9e8834b116e85f23a
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-25T20:22:31.000Z"}}
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
    "created_at": "2016-10-25T20:32:31.429Z",
    "read_at": "2016-10-25T20:22:31.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 57,
    "updated_at": "2016-10-25T20:32:31.470Z",
    "author_id": "674",
    "thread_subject_id": "233",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/24" -d '{"notification":{"read_at":"2016-10-25T20:22:31.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d39757afb26222ec4b5994d4ebdf6d6deb1bb8a1b246bf9e8834b116e85f23a"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6e13c163d4cf24af6685355f06075abcb2bacbcb6449c327cbf9ea192cfcd9a7
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
      "course_id": 247,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T20:32:36.726Z",
      "course_published": true,
      "updated_at": "2016-10-25T20:32:36.718Z"
    },
    {
      "id": 4,
      "course_id": 248,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T20:32:36.803Z",
      "course_published": true,
      "updated_at": "2016-10-25T20:32:36.795Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e13c163d4cf24af6685355f06075abcb2bacbcb6449c327cbf9ea192cfcd9a7"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 8e707c62ba024f973298c02d128f9f32355d27681f4ae426e3bac3cc014afc7a
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
    "course_id": 249,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T20:32:36.923Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:32:36.914Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e707c62ba024f973298c02d128f9f32355d27681f4ae426e3bac3cc014afc7a"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer ceb275a84d08a8cc9082a7b48a60aef663e2fe687c97d498174576ac391bbf39
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
    "course_id": 246,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-25T20:32:36.591Z",
    "course_published": true,
    "updated_at": "2016-10-25T20:32:36.580Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceb275a84d08a8cc9082a7b48a60aef663e2fe687c97d498174576ac391bbf39"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 67567106522e0fc4189e1a69f87f4c5d94d6e4d716b88ca99a850c5e0b0778f1
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
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 109,
      "user_id": 715
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 110,
      "user_id": 715
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 111,
      "user_id": 715
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 112,
      "user_id": 715
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67567106522e0fc4189e1a69f87f4c5d94d6e4d716b88ca99a850c5e0b0778f1"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/136
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
    "id": 136,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 134,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 136
      },
      {
        "id": 135,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 136
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/136" -X GET \
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
      "id": 134,
      "name": "Exclusive transitional customer loyalty",
      "name_translations": {
        "en": "Exclusive transitional customer loyalty"
      }
    },
    {
      "id": 135,
      "name": "Optional demand-driven application",
      "name_translations": {
        "en": "Optional demand-driven application"
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
PATCH /v2/feedbacks/44/close
Content-Type: application/json
Authorization: Bearer a2af632f74ae6297f1aa5b8b3665d081f6524fcb47662449dc42e804223a670f
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
    "id": 44,
    "user_id": 855,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-25T20:32:45.267Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/44/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2af632f74ae6297f1aa5b8b3665d081f6524fcb47662449dc42e804223a670f"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/40/fix
Content-Type: application/json
Authorization: Bearer 0745d09b3e842d033b9a4a2b45c95041bdf3c870e74d99b0f62c0759828444f9
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
    "user_id": 835,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-25T20:32:44.097Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/40/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0745d09b3e842d033b9a4a2b45c95041bdf3c870e74d99b0f62c0759828444f9"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/45
Content-Type: application/json
Authorization: Bearer a18005f60ac050173bc7061f01df10b09fdf9a2db23c24fadaab6430325e6f50
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
    "id": 45,
    "user_id": 860,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:32:45.589Z",
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
curl "api.goskive.com/v2/feedbacks/45" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a18005f60ac050173bc7061f01df10b09fdf9a2db23c24fadaab6430325e6f50"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/38/fix
Content-Type: application/json
Authorization: Bearer 54819bd38ba519860a94aab4d1e4751c2e40521e627cb5239d4ecd47a8ca93cb
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
	-H "Authorization: Bearer 54819bd38ba519860a94aab4d1e4751c2e40521e627cb5239d4ecd47a8ca93cb"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/41/fix
Content-Type: application/json
Authorization: Bearer 3a11f171111042833903890290c98daaeaf7d78e5737022c71a8b1adddef26a8
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
curl "api.goskive.com/v2/feedbacks/41/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a11f171111042833903890290c98daaeaf7d78e5737022c71a8b1adddef26a8"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/42/close
Content-Type: application/json
Authorization: Bearer a7cd13e748c29152520cb30e0fdf89097e275a6ac1d148f77a9b30e33f60a41b
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
	-H "Authorization: Bearer a7cd13e748c29152520cb30e0fdf89097e275a6ac1d148f77a9b30e33f60a41b"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/46
Content-Type: application/json
Authorization: Bearer 04af5589697ecd1b3a0043f343514c27ea0275822ee89fedd84699511d3829ff
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
    "id": 46,
    "user_id": 865,
    "feedbackable_id": 91,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:32:45.882Z",
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
curl "api.goskive.com/v2/feedbacks/46" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04af5589697ecd1b3a0043f343514c27ea0275822ee89fedd84699511d3829ff"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 73dc28e73104971215a32cad1d7109dff1968f39d263953a93a7a8aa2a0a86e1
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
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 73dc28e73104971215a32cad1d7109dff1968f39d263953a93a7a8aa2a0a86e1"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer daffaf4208dc1f392333509c52d89872211d15ba34e801bad91d490c3f3df581
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daffaf4208dc1f392333509c52d89872211d15ba34e801bad91d490c3f3df581"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/15
Content-Type: application/json
Authorization: Bearer 5588096eb61c71b19902f3863936d82ab5d5cf3c653a2e98c80e25c00067d511
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5f2b9da75c18dad92c05152fcfeb9ded.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T203211Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8f74715502759af31d1b608cb9853e93cec7a8b927a465b885e0ac9c8e122f64",
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
	-H "Authorization: Bearer 5588096eb61c71b19902f3863936d82ab5d5cf3c653a2e98c80e25c00067d511"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/14/preview
Content-Type: application/json
Authorization: Bearer a80a872568a8776762635b56a9283a1974b9b5798273bc3fe244bb9cd2eb4a50
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/b7dd01c31db112080362a5cf3f1c62ec.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T203211Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=f4892f0eb844acb7a9900ee1e989a2e68d19814ddfbfe625d55029babd393fda",
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
	-H "Authorization: Bearer a80a872568a8776762635b56a9283a1974b9b5798273bc3fe244bb9cd2eb4a50"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer f3ad279599f426caf46acd4297be05d8dfe01a83d7d846a2e2eb08964e30afee
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
    "id": 7,
    "uploader": {
      "id": 471,
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
      "created_at": "2016-10-25T20:32:09.819Z",
      "updated_at": "2016-10-25T20:32:09.819Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T20:32:09.895Z",
    "updated_at": "2016-10-25T20:32:09.895Z",
    "course_id": 146,
    "filename": "Pastry Making Notes.pdf",
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
| file[status] | Status |
| file[download_count] | Download count |
| file[created_at] | Created at |
| file[updated_at] | Updated at |
| file[course_id] | Course ID |
| file[category] | Category |
| file[is_anonymous] | Anonymous |


```shell
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f3ad279599f426caf46acd4297be05d8dfe01a83d7d846a2e2eb08964e30afee"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer a89f7ac2a7427cad3053e3ba4b21bad197bf8881a3b81aa7f09a1325569174fb
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
      "creator_id": 303,
      "id": 99,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 100,
      "additional_university_ids": [

      ],
      "topic_id": 101,
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
      "chapters_updated_at": "2016-10-25T20:31:55.374Z",
      "updated_at": "2016-10-25T20:31:57.082Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 308,
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-e388d065-b33a-4a8c-879f-60fc95681bb2",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-e388d065-b33a-4a8c-879f-60fc95681bb2",
      "slug": "mit-the-great-british-bake-off-e388d065-b33a-4a8c-879f-60fc95681bb2",
      "university_id": 101,
      "additional_university_ids": [

      ],
      "topic_id": 102,
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
      "chapters_updated_at": "2016-10-25T20:31:55.374Z",
      "updated_at": "2016-10-25T20:31:57.668Z",
      "shortname": "mit-the-great-british-bake-off-e388d065-b33a-4a8c-879f-60fc95681bb2"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer a89f7ac2a7427cad3053e3ba4b21bad197bf8881a3b81aa7f09a1325569174fb"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/10/report
Content-Type: application/json
Authorization: Bearer aa01267bf11615eef5010756ce8cd8cb0583bfbe11eb18e682eac4e4ae01515a
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/10/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aa01267bf11615eef5010756ce8cd8cb0583bfbe11eb18e682eac4e4ae01515a"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/6/comments
Content-Type: application/json
Authorization: Bearer 51b751f94d8fbf3ee065a9fc91bff3709b3cb55b34d32c47649df010feee5d1f
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
    "id": 43,
    "author_id": 139,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:31:40.546Z",
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
curl "api.goskive.com/v2/flashcards/6/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51b751f94d8fbf3ee065a9fc91bff3709b3cb55b34d32c47649df010feee5d1f"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/5/comments
Content-Type: application/json
Authorization: Bearer 49e884247e6337c900f5ab980902e283b6dc6b6e3bd3be2b157292a3b38e475a
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
    "id": 42,
    "author_id": 136,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:31:39.902Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 1,
      "user_id": 136,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:39.897Z",
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
curl "api.goskive.com/v2/flashcards/5/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 49e884247e6337c900f5ab980902e283b6dc6b6e3bd3be2b157292a3b38e475a"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer 6cdf2bb90fd815debd7f3bc0399c4069d9186f6e9d52cf60bd98ce9aa0c05ae4
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
      "id": 44,
      "author_id": 151,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:41.235Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 152,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:41.252Z",
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
curl "api.goskive.com/v2/flashcards/9/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cdf2bb90fd815debd7f3bc0399c4069d9186f6e9d52cf60bd98ce9aa0c05ae4"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/7/comments
Content-Type: application/json
Authorization: Bearer 3782717f0e36272169fe8859d15d19c48425523cdb9b82b05fec1cdd2d32f93c
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
curl "api.goskive.com/v2/flashcards/7/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3782717f0e36272169fe8859d15d19c48425523cdb9b82b05fec1cdd2d32f93c"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/11/feedbacks
Content-Type: application/json
Authorization: Bearer be54420f1f55f763ee98a32c4a5e8bcdb16b21adcb6468762a428453ebd64684
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
    "id": 3,
    "user_id": 156,
    "feedbackable_id": 11,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:31:41.821Z",
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
	-H "Authorization: Bearer be54420f1f55f763ee98a32c4a5e8bcdb16b21adcb6468762a428453ebd64684"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/13/feedbacks
Content-Type: application/json
Authorization: Bearer 1ec7737783be821a41f0641cd2b7621524b82066de05d57239566ad0bf4cc58c
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
      "user_id": 166,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:42.296Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 165,
      "feedbackable_id": 13,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:42.284Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/13/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ec7737783be821a41f0641cd2b7621524b82066de05d57239566ad0bf4cc58c"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/47/votes
Content-Type: application/json
Authorization: Bearer eca1ada21daa498cc711b360a1663d93135682c4adfd483835c2b220dbed3926
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
      "id": 7,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 450
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 449
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 448
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/47/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eca1ada21daa498cc711b360a1663d93135682c4adfd483835c2b220dbed3926"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/23/republish
Content-Type: application/json
Authorization: Bearer 955b68188216383c81717accec5122bdafee04608be4730807365b81ca07a28a
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
	-H "Authorization: Bearer 955b68188216383c81717accec5122bdafee04608be4730807365b81ca07a28a"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/bookmark
Content-Type: application/json
Authorization: Bearer 02448eaca4fb4cc5ad9b60d146aebcb1c37d1c4468ef8dbc7f2efaa5721e79c8
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02448eaca4fb4cc5ad9b60d146aebcb1c37d1c4468ef8dbc7f2efaa5721e79c8"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/25
Content-Type: application/json
Authorization: Bearer 1f44ab69ff33ed1028dd89f8fea5bca42179cc7d20c0552ee1a45900fd0aaa05
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/25" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f44ab69ff33ed1028dd89f8fea5bca42179cc7d20c0552ee1a45900fd0aaa05"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/downvote
Content-Type: application/json
Authorization: Bearer a790cead9582425a5f6d1f5a10ac1bee3985e99ce55d177482e06fefde25d89e
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/26/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a790cead9582425a5f6d1f5a10ac1bee3985e99ce55d177482e06fefde25d89e"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/24
Content-Type: application/json
Authorization: Bearer 60f2de57c9c04580d0e903116ffb1f63581889e968a0580d2b7d0f62710220b6
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
    "id": 24,
    "obfuscated_id": "KHM5yo_z4Ds",
    "author_id": 360,
    "chapter_id": 67,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:32:02.399Z",
    "created_at": "2016-10-25T20:32:02.399Z",
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
curl "api.goskive.com/v2/flashcards/24" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60f2de57c9c04580d0e903116ffb1f63581889e968a0580d2b7d0f62710220b6"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/45/report
Content-Type: application/json
Authorization: Bearer dd763255a10419f96558435f826a4dcbfe3e8e0a6cf966acdfdd83c3942933f3
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/45/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd763255a10419f96558435f826a4dcbfe3e8e0a6cf966acdfdd83c3942933f3"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/42/bookmark
Content-Type: application/json
Authorization: Bearer 31cb5108f8c5ff29c198b88c1f385e3c40fd694e723552921317cf9542260245
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31cb5108f8c5ff29c198b88c1f385e3c40fd694e723552921317cf9542260245"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/43/upvote
Content-Type: application/json
Authorization: Bearer 623e9d7f20117b9975c48020a4cdb044017e76b370087976b2a61690c036a456
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/43/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 623e9d7f20117b9975c48020a4cdb044017e76b370087976b2a61690c036a456"
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
    "key": "cache/6062f78993b965149d2085fcff9bc2a3.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQyMTozMjoxM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzYwNjJmNzg5OTNiOTY1MTQ5ZDIwODVmY2ZmOWJjMmEzLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjVUMjAzMjEzWiJ9XX0=",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T203213Z",
    "x-amz-signature": "aabd59e548b3e3d25d67e0babbdcc7de309e87fe3ee9e9cb799a1acf202e3aa9"
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
Authorization: Bearer 81074671d8ea54c73e4c02c25915a643007e2325254ef5bfb250a99115fee89e
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
curl "api.goskive.com/v2/me/jobs/2/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81074671d8ea54c73e4c02c25915a643007e2325254ef5bfb250a99115fee89e"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 225ca039029d01adedd89036e53b0c9350a89da9857cdf6b35165a6330bebbb4
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
	-H "Authorization: Bearer 225ca039029d01adedd89036e53b0c9350a89da9857cdf6b35165a6330bebbb4"
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
{"password":{"reset_password_token":"vuKG5rx8EZEkF39mXXkE","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 957,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-25T20:32:53.411Z",
  "updated_at": "2016-10-25T20:32:53.592Z",
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
  "audit_id": 5458
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"vuKG5rx8EZEkF39mXXkE","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/49/comments
Content-Type: application/json
Authorization: Bearer dd15f024df3262b38250106cb8133b70f3ab12b28b06aacc07e3aa494281b4ac
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
    "id": 48,
    "author_id": 325,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:31:59.189Z",
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
curl "api.goskive.com/v2/questions/49/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd15f024df3262b38250106cb8133b70f3ab12b28b06aacc07e3aa494281b4ac"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/50/comments
Content-Type: application/json
Authorization: Bearer ac8c682c8d5e0f2d2394815fbd78b8029123350ad1d23076c568430ec8b66ee1
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
    "author_id": 328,
    "reply_to_id": null,
    "created_at": "2016-10-25T20:31:59.652Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 10,
      "user_id": 328,
      "feedbackable_id": 50,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:59.648Z",
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
curl "api.goskive.com/v2/questions/50/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac8c682c8d5e0f2d2394815fbd78b8029123350ad1d23076c568430ec8b66ee1"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/53/comments
Content-Type: application/json
Authorization: Bearer 17a3d65bb0348986f535f116dc8f93ac1406c4b1a7473c9afa3099e404323a19
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
      "id": 50,
      "author_id": 340,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:32:00.716Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 341,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:32:00.732Z",
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
curl "api.goskive.com/v2/questions/53/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17a3d65bb0348986f535f116dc8f93ac1406c4b1a7473c9afa3099e404323a19"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/51/comments
Content-Type: application/json
Authorization: Bearer 8f9aa6ec3646e10c18e0d2da0ac46f577cd6db6a9710fe88d33fc5aa91d40cf5
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
curl "api.goskive.com/v2/questions/51/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f9aa6ec3646e10c18e0d2da0ac46f577cd6db6a9710fe88d33fc5aa91d40cf5"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/102/feedbacks
Content-Type: application/json
Authorization: Bearer 02297f8f99c82ed43906953f868ea7c3b8138ed4f714dab0195cbcfef4b579a4
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
    "user_id": 679,
    "feedbackable_id": 102,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-25T20:32:32.277Z",
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
	-H "Authorization: Bearer 02297f8f99c82ed43906953f868ea7c3b8138ed4f714dab0195cbcfef4b579a4"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/108/feedbacks
Content-Type: application/json
Authorization: Bearer fff394ac6d65522754030d4b75a56d60e95aaad12042a8b7351f7e7ff6f4e29b
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
      "id": 18,
      "user_id": 711,
      "feedbackable_id": 108,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:34.609Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 710,
      "feedbackable_id": 108,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:34.599Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/108/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fff394ac6d65522754030d4b75a56d60e95aaad12042a8b7351f7e7ff6f4e29b"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/59/votes
Content-Type: application/json
Authorization: Bearer f0ae6cddce701cec110a46ea71e2cc9ab5b849220d35e171c82ed66044ad823f
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 507
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 506
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 59,
      "user_id": 505
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/59/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0ae6cddce701cec110a46ea71e2cc9ab5b849220d35e171c82ed66044ad823f"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/20/republish
Content-Type: application/json
Authorization: Bearer 7e736a47c89df981beeca71381beabbb0c72fedd0e060e054cd15eabe5385d43
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
curl "api.goskive.com/v2/questions/20/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e736a47c89df981beeca71381beabbb0c72fedd0e060e054cd15eabe5385d43"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/21/bookmark
Content-Type: application/json
Authorization: Bearer f35b9c223e89050fb61c7cf67be8ad1e7f0927388f1b1331e0c215081ede707f
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/21/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f35b9c223e89050fb61c7cf67be8ad1e7f0927388f1b1331e0c215081ede707f"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/40
Content-Type: application/json
Authorization: Bearer 40861c9c04ba14de47b1e4c10092c29c586cbebc8fee3c66903d348e5442d4d5
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40861c9c04ba14de47b1e4c10092c29c586cbebc8fee3c66903d348e5442d4d5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/22/downvote
Content-Type: application/json
Authorization: Bearer 7a2aa190fd231f602ac13504f39e25cb896afeee74a00eab3ea89816f91e0ced
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a2aa190fd231f602ac13504f39e25cb896afeee74a00eab3ea89816f91e0ced"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/23
Content-Type: application/json
Authorization: Bearer e28c4da8cd51897b788b22da1363ba3ea3d8acbee4e1ecbb43dfac92c8e5fe91
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 234,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:49.145Z",
    "created_at": "2016-10-25T20:31:49.017Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e28c4da8cd51897b788b22da1363ba3ea3d8acbee4e1ecbb43dfac92c8e5fe91"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/17/report
Content-Type: application/json
Authorization: Bearer b8fea390981eac70db382dca04077aa9c295d99af905eb0acd212294446b725a
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/17/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8fea390981eac70db382dca04077aa9c295d99af905eb0acd212294446b725a"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/39/bookmark
Content-Type: application/json
Authorization: Bearer ea94afeb65a15c55f9b57fc2c9a2ec9a39398a98aa51117df75651c085060d9f
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/39/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea94afeb65a15c55f9b57fc2c9a2ec9a39398a98aa51117df75651c085060d9f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/16
Content-Type: application/json
Authorization: Bearer c802115706aa4888c526181b415ddede2106b6019644bab2e74951a48b97d44c
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":16,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T20:31:46.198Z","updated_at":"2016-10-25T20:31:46.323Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":31,"author_id":213,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 16,
    "obfuscated_id": "Drq0t9y67cE",
    "author_id": 213,
    "chapter_id": 31,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T20:31:46.441Z",
    "created_at": "2016-10-25T20:31:46.198Z",
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
    "question": "{\"id\"=>16, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-25T20:31:46.198Z\", \"updated_at\"=>\"2016-10-25T20:31:46.323Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>31, \"author_id\"=>213, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 34,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 35,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 36,
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
curl "api.goskive.com/v2/questions/16" -d '{"question":{"question":{"id":16,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T20:31:46.198Z","updated_at":"2016-10-25T20:31:46.323Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":31,"author_id":213,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c802115706aa4888c526181b415ddede2106b6019644bab2e74951a48b97d44c"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/18/upvote
Content-Type: application/json
Authorization: Bearer 731375863f59cc260622e714fa0a648ddf400892c90e5bc2770f68c1d0093ba2
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/18/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 731375863f59cc260622e714fa0a648ddf400892c90e5bc2770f68c1d0093ba2"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 66597911bf7b209ecebe98934719d4e0fed60fbb25ae67489dac00e3ad687a5c
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
      "creator_id": 469,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 146,
      "additional_university_ids": [

      ],
      "topic_id": 147,
      "discipline_id": 148,
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
      "updated_at": "2016-10-25T20:32:09.618Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66597911bf7b209ecebe98934719d4e0fed60fbb25ae67489dac00e3ad687a5c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 18c75dcc44a5743e21de4dbed487b49752a41dc8955676be63abae2b2313af19
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
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-144",
      "html_url": "https://goskive.com/university/uni-144",
      "slug": "uni-144",
      "name": "National School of Pizza",
      "short_name": "Uni 144",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a5dfa351bbcaee6d732d80d377ee3c3c12237e84.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/dae6aada46711b55e68ea47c4f10053d1411123a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:32:09.321Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-143",
      "html_url": "https://goskive.com/university/uni-143",
      "slug": "uni-143",
      "name": "National School of Pastry",
      "short_name": "Uni 143",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/a58445f18da323c32d6a01ee13edfd8e910335cc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2fe7ca1fa741826191cad0989815045dbd19a0b6.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:32:09.303Z",
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
	-H "Authorization: Bearer 18c75dcc44a5743e21de4dbed487b49752a41dc8955676be63abae2b2313af19"
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
      "id": 309,
      "name": "Exclusive 24 hour functionalities",
      "name_translations": {
        "en": "Exclusive 24 hour functionalities"
      },
      "discipline_id": 310
    },
    {
      "id": 310,
      "name": "Public-key static firmware",
      "name_translations": {
        "en": "Public-key static firmware"
      },
      "discipline_id": 311
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
GET /v2/topics/311
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
    "id": 311,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 312
  }
}
```



```shell
curl "api.goskive.com/v2/topics/311" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 96b140c3c9260f21c2a4a8e2c47e3fca80ed64254b260f9ff89c5768484700b5
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
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-165",
      "html_url": "https://goskive.com/university/uni-165",
      "slug": "uni-165",
      "name": "University 142",
      "short_name": "Uni 165",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ea7eab85497e5dfbeb10e3fc1cd56f0ba8e3851b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a07cd0ff93d2a822365e0a2e08130bf99a02417d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T20:32:14.513Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-166",
      "html_url": "https://goskive.com/university/uni-166",
      "slug": "uni-166",
      "name": "University 143",
      "short_name": "Uni 166",
      "acronym": "MIT",
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
      "updated_at": "2016-10-25T20:32:14.532Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-167",
      "html_url": "https://goskive.com/university/uni-167",
      "slug": "uni-167",
      "name": "University 144",
      "short_name": "Uni 167",
      "acronym": "MIT",
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
      "updated_at": "2016-10-25T20:32:14.551Z",
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
	-H "Authorization: Bearer 96b140c3c9260f21c2a4a8e2c47e3fca80ed64254b260f9ff89c5768484700b5"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 2a23dc2670a848376b30daf86aab8d39e0826752aaa5f4a83de08824578ab99d
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
    "id": 165,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d42ffac50a87c2f5f95462aa80d7eef46b931fdc.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4b22ef9138b10be2b344bf80993382e2349656fe.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-25T20:32:14.345Z",
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
	-H "Authorization: Bearer 2a23dc2670a848376b30daf86aab8d39e0826752aaa5f4a83de08824578ab99d"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d84dde72edd7dfe9c00b23aa51fddc31139fa7ae1febb104b9de26eb1a691243
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":227,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 641,
    "id": 223,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 208,
    "additional_university_ids": [

    ],
    "topic_id": 227,
    "discipline_id": 228,
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
    "chapters_updated_at": "2016-10-25T20:32:28.587Z",
    "updated_at": "2016-10-25T20:32:28.725Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 122,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-25T20:32:28.682Z",
        "course_id": 223,
        "author_id": 641,
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
        "id": 123,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-25T20:32:28.699Z",
        "course_id": 223,
        "author_id": 641,
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
        "id": 124,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-25T20:32:28.716Z",
        "course_id": 223,
        "author_id": 641,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":227,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d84dde72edd7dfe9c00b23aa51fddc31139fa7ae1febb104b9de26eb1a691243"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7c3f0257f5101618c3c45a3e3bce1fbbc9d03fe5e4335d0974c4b1ec81417bd6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":226,"published":false}}
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
    "creator_id": 640,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "topic_id": 226,
    "discipline_id": 227,
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
    "updated_at": "2016-10-25T20:32:28.553Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":226,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c3f0257f5101618c3c45a3e3bce1fbbc9d03fe5e4335d0974c4b1ec81417bd6"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1740b8c2556bb088665bf1643ade8976e92cb1e6763051da992647cac304e240
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
      "creator_id": 603,
      "id": 191,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 194,
      "additional_university_ids": [

      ],
      "topic_id": 195,
      "discipline_id": 196,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
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
      "updated_at": "2016-10-25T20:32:25.085Z",
      "shortname": "fu-course-148"
    },
    {
      "creator_id": 603,
      "id": 192,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 194,
      "additional_university_ids": [

      ],
      "topic_id": 196,
      "discipline_id": 197,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
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
      "chapters_updated_at": "2016-10-25T20:32:25.394Z",
      "updated_at": "2016-10-25T20:32:25.401Z",
      "shortname": "fu-course-149"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1740b8c2556bb088665bf1643ade8976e92cb1e6763051da992647cac304e240"
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
      "creator_id": 633,
      "id": 215,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 203,
      "additional_university_ids": [

      ],
      "topic_id": 219,
      "discipline_id": 220,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 172",
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
      "updated_at": "2016-10-25T20:32:27.766Z",
      "shortname": "fu-course-172"
    },
    {
      "creator_id": 633,
      "id": 216,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-173",
      "html_url": "https://goskive.com/course/fu-course-173",
      "slug": "fu-course-173",
      "university_id": 203,
      "additional_university_ids": [

      ],
      "topic_id": 220,
      "discipline_id": 221,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
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
      "chapters_updated_at": "2016-10-25T20:32:28.053Z",
      "updated_at": "2016-10-25T20:32:28.059Z",
      "shortname": "fu-course-173"
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
Authorization: Bearer 93d46c2fa6e6064003d62b924f79c14dc6fe6a49cc824162a009a253f50b0610
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
      "creator_id": 609,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 195,
      "additional_university_ids": [

      ],
      "topic_id": 199,
      "discipline_id": 200,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
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
      "updated_at": "2016-10-25T20:32:25.642Z",
      "shortname": "fu-course-152"
    },
    {
      "creator_id": 609,
      "id": 196,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 195,
      "additional_university_ids": [

      ],
      "topic_id": 200,
      "discipline_id": 201,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 153",
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
      "updated_at": "2016-10-25T20:32:25.685Z",
      "shortname": "fu-course-153"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 93d46c2fa6e6064003d62b924f79c14dc6fe6a49cc824162a009a253f50b0610"
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
      "creator_id": 638,
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 204,
      "additional_university_ids": [

      ],
      "topic_id": 223,
      "discipline_id": 224,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "updated_at": "2016-10-25T20:32:28.242Z",
      "shortname": "fu-course-176"
    },
    {
      "creator_id": 638,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-177",
      "html_url": "https://goskive.com/course/fu-course-177",
      "slug": "fu-course-177",
      "university_id": 204,
      "additional_university_ids": [

      ],
      "topic_id": 224,
      "discipline_id": 225,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 177",
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
      "updated_at": "2016-10-25T20:32:28.283Z",
      "shortname": "fu-course-177"
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
Authorization: Bearer d86b62ab94c39ea040bfa22aafaec7ea9feefc6e665398dd8466089452eb2f9c
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
  "id": 527,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-25T20:32:14.080Z",
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
	-H "Authorization: Bearer d86b62ab94c39ea040bfa22aafaec7ea9feefc6e665398dd8466089452eb2f9c"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/132
Content-Type: application/json
Authorization: Bearer 915d7bd742a956a47308252f97f0990e6e793d3ce2e08f11afd262d4a0bf0400
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
    "id": 132,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 52,
    "fields_of_study": [
      52,
      53
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-25T20:31:39.566Z",
    "updated_at": "2016-10-25T20:31:39.566Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/132" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 915d7bd742a956a47308252f97f0990e6e793d3ce2e08f11afd262d4a0bf0400"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/134
Content-Type: application/json
Authorization: Bearer f868ac311d14111cffce3779571225f57c240714f52801597bda4ccfcfaab9d8
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
    "id": 134,
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
    "created_at": "2016-10-25T20:31:39.660Z",
    "updated_at": "2016-10-25T20:31:39.660Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/134" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f868ac311d14111cffce3779571225f57c240714f52801597bda4ccfcfaab9d8"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/10
Content-Type: application/json
Authorization: Bearer 0439503f98dd4b7000521ef9cb354d5a91a3a0e1d37fc18042457cb896511cf8
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/10" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0439503f98dd4b7000521ef9cb354d5a91a3a0e1d37fc18042457cb896511cf8"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/9
Content-Type: application/json
Authorization: Bearer 0c3cec7918321704a67b0f48f4cbb0565a464a540ee4338cd55ce6fa99e0b151
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
    "votable_id": 54,
    "user_id": 454
  }
}
```



```shell
curl "api.goskive.com/v2/votes/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c3cec7918321704a67b0f48f4cbb0565a464a540ee4338cd55ce6fa99e0b151"
```
