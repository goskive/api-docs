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
Authorization: Basic ZTc5Y2FjYjQwZGRhNDk5YWE2Y2E4YWU5OGE0ZmNmZjk0NjRhYzljNDcwZjRl
YjBhODQwNGRiMjVjYmU0M2NmYjpjM2JhMTdlODg1OTY5MTUzNjE4NzA2ZDE3
NDM2ZWFmMWM3NWMzNDFkMjYzOTg4YzE4YzUxMDU3Zjc3YjhhYWEw

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
	-u e79cacb40dda499aa6ca8ae98a4fcff9464ac9c470f4eb0a8404db25cbe43cfb:c3ba17e885969153618706d17436eaf1c75c341d263988c18c51057f77b8aaa0
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"252e993b6f66ac74c17c08f679fb9e3062bd19ec43b311276e89d7f535216e61","client_secret":"b2de30e8ea59f72cadbac27eddc3e55ff6499e3918f0067e896d9be4e562f9fa"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"252e993b6f66ac74c17c08f679fb9e3062bd19ec43b311276e89d7f535216e61","client_secret":"b2de30e8ea59f72cadbac27eddc3e55ff6499e3918f0067e896d9be4e562f9fa"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTMyMDlhZWY2M2M1ZmQ1OGFiYTUzNjFiMWMyOGRjOWQ4NGI4ZWVjMTExZjAy
MWJkMzg2ODE1NmI3MjU1NGFmMjoxMWQzMWUyNDg0NTczNjg0YzI1N2M3NDhk
MjYyM2IxMTk0MGY0MzU0OTZkN2Y3N2YwZDVkYzkzNzRkY2ZiYjlj

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
  "access_token": "bce090fff87bef332a2aca919ad59ae86095220bedab13e65d6f9f9c5f091438",
  "token_type": "bearer",
  "created_at": 1476444924
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u a3209aef63c5fd58aba5361b1c28dc9d84b8eec111f021bd3868156b72554af2:11d31e2484573684c257c748d2623b11940f435496d7f77f0d5dc9374dcfbb9c
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"32e584e36883863e06ef4bad6f9535ee79e428dd818f6cd60262367af1d3d1d3","client_secret":"878fb5e069e50a59b86d5ca49d13f8a6121162211872cf7f96c24318255dac1f"}
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
  "access_token": "c68fdb47039bb48d4e7f84694fa66a45a4318126a0d23ec4fa45262f35031d9b",
  "token_type": "bearer",
  "created_at": 1476444924
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"32e584e36883863e06ef4bad6f9535ee79e428dd818f6cd60262367af1d3d1d3","client_secret":"878fb5e069e50a59b86d5ca49d13f8a6121162211872cf7f96c24318255dac1f"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"5bf87deed0ef1e90c9c5294cd928ba0fb9346d6798020852dbfdedc54a7bbad8","client_secret":"7f90cdb4bff788cfbb5eadd6d304ee4cdbb952af62226f46e9b67b0be833539b"}
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
  "access_token": "bd1c6583a67503a3c93a130194a00bc0803c39e9141ac8d5a83add60eea09eaf",
  "token_type": "bearer",
  "created_at": 1476444925
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5bf87deed0ef1e90c9c5294cd928ba0fb9346d6798020852dbfdedc54a7bbad8","client_secret":"7f90cdb4bff788cfbb5eadd6d304ee4cdbb952af62226f46e9b67b0be833539b"}' -X POST \
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
Authorization: Bearer 6a0d4daf574d79a70788df86595006baa15e5debacd5ed1629da3cb6f5fbd79d
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
curl "api.goskive.com/v2/campaigns/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a0d4daf574d79a70788df86595006baa15e5debacd5ed1629da3cb6f5fbd79d"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/35/flashcards
Content-Type: application/json
Authorization: Bearer e71ae2a29cfb1aa4354d4df235fa20bb21f4e3d19ebc8d0c6a15023d25b85690
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":35,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 224,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:35:30.089Z",
    "created_at": "2016-10-14T11:35:30.089Z",
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
curl "api.goskive.com/v2/chapters/35/flashcards" -d '{"flashcard":{"chapter_id":35,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e71ae2a29cfb1aa4354d4df235fa20bb21f4e3d19ebc8d0c6a15023d25b85690"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/36/flashcards
Content-Type: application/json
Authorization: Bearer fbe6d3fc10d497374cba693c9d66484b965f3c0bf5ba66c747a3530b73518348
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 225,
      "chapter_id": 36,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:30.250Z",
      "created_at": "2016-10-14T11:35:30.250Z",
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
      "author_id": 225,
      "chapter_id": 36,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:30.287Z",
      "created_at": "2016-10-14T11:35:30.287Z",
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
      "author_id": 225,
      "chapter_id": 36,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:30.323Z",
      "created_at": "2016-10-14T11:35:30.323Z",
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
curl "api.goskive.com/v2/chapters/36/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbe6d3fc10d497374cba693c9d66484b965f3c0bf5ba66c747a3530b73518348"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/116/questions
Content-Type: application/json
Authorization: Bearer 0b7abec65b142a5c45314396ed3ebfbd100c7a208cd22aecec0d71e837892f55
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 79,
    "obfuscated_id": "BFjsqYG0c2I",
    "author_id": 674,
    "chapter_id": 116,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:01.404Z",
    "created_at": "2016-10-14T11:36:01.404Z",
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
        "id": 157,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 158,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 159,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 160,
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
curl "api.goskive.com/v2/chapters/116/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":116,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b7abec65b142a5c45314396ed3ebfbd100c7a208cd22aecec0d71e837892f55"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/115/questions
Content-Type: application/json
Authorization: Bearer aebd56e3174b7b9b30572626029ad45d62080e6240837bd431d81c84698b4b93
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":115,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 78,
    "obfuscated_id": "-wsYNe2w7uo",
    "author_id": 671,
    "chapter_id": 115,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:01.042Z",
    "created_at": "2016-10-14T11:36:01.042Z",
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
        "id": 155,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 156,
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
curl "api.goskive.com/v2/chapters/115/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":115,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aebd56e3174b7b9b30572626029ad45d62080e6240837bd431d81c84698b4b93"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/118/questions
Content-Type: application/json
Authorization: Bearer 7e5012256bd6fb964dae27c3c6ed146bfda1498ba418d96b5052bc801c5c3525
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 680,
    "chapter_id": 118,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:02.362Z",
    "created_at": "2016-10-14T11:36:02.362Z",
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
        "id": 164,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 165,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/118/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":118,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e5012256bd6fb964dae27c3c6ed146bfda1498ba418d96b5052bc801c5c3525"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/117/questions
Content-Type: application/json
Authorization: Bearer 16b0f0445bd8c3604ea6d3f3f9571a2b39f70ebc7b66366e748ff5de77b0773a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":117,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 677,
    "chapter_id": 117,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:01.928Z",
    "created_at": "2016-10-14T11:36:01.928Z",
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
        "id": 161,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 162,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 163,
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
curl "api.goskive.com/v2/chapters/117/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":117,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16b0f0445bd8c3604ea6d3f3f9571a2b39f70ebc7b66366e748ff5de77b0773a"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/114/questions
Content-Type: application/json
Authorization: Bearer 2b689f96aa05bfba74e48b937ea875e18b4466552334addb540624aa790fe57a
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
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 665,
      "chapter_id": 114,
      "position": 75,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:00.379Z",
      "created_at": "2016-10-14T11:36:00.259Z",
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 666,
      "chapter_id": 114,
      "position": 76,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:00.577Z",
      "created_at": "2016-10-14T11:36:00.455Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 667,
      "chapter_id": 114,
      "position": 77,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:00.781Z",
      "created_at": "2016-10-14T11:36:00.656Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/chapters/114/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b689f96aa05bfba74e48b937ea875e18b4466552334addb540624aa790fe57a"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/154
Content-Type: application/json
Authorization: Bearer 00f7cf05d59ed7a0d9796692dd0b78755ad6c7d5941e3beeb9e138329379d264
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
curl "api.goskive.com/v2/chapters/154" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00f7cf05d59ed7a0d9796692dd0b78755ad6c7d5941e3beeb9e138329379d264"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/155
Content-Type: application/json
Authorization: Bearer 01b4216a7fcd45a190f4deb03bf5d05932dc43bd1e7a4553f57dbd077a184e91
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
curl "api.goskive.com/v2/chapters/155" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01b4216a7fcd45a190f4deb03bf5d05932dc43bd1e7a4553f57dbd077a184e91"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/150
Content-Type: application/json
Authorization: Bearer ec51bcb25bb3a26004ea8491ec6e473c4d6ab83a034a31c628e3095daaf8b8e5
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
curl "api.goskive.com/v2/chapters/150" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec51bcb25bb3a26004ea8491ec6e473c4d6ab83a034a31c628e3095daaf8b8e5"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/156
Content-Type: application/json
Authorization: Bearer 1aefc56136d5947a401b513e0429b551d141a994d75522df3fb9a86f3f8f0a84
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/156" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1aefc56136d5947a401b513e0429b551d141a994d75522df3fb9a86f3f8f0a84"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/158
Content-Type: application/json
Authorization: Bearer 52ef5add278832993fa215e00f2d8b73ec63e2fe07338f1797f9d622b3e21d48
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
    "id": 158,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T11:36:17.020Z",
    "course_id": 272,
    "author_id": 826,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-14T11:36:16.458Z",
    "questions_updated_at": "2016-10-14T11:36:16.458Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 830,
        "chapter_id": 158,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:17.002Z",
        "created_at": "2016-10-14T11:36:17.002Z",
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
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 828,
        "chapter_id": 158,
        "position": 105,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:16.889Z",
        "created_at": "2016-10-14T11:36:16.765Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/158" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52ef5add278832993fa215e00f2d8b73ec63e2fe07338f1797f9d622b3e21d48"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/151
Content-Type: application/json
Authorization: Bearer c99ca5310ed2f243dc383003ddd8f8d64f9bd48576726af4824ea648049bce07
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
    "id": 151,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T11:36:14.634Z",
    "course_id": 265,
    "author_id": 802,
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
curl "api.goskive.com/v2/chapters/151" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c99ca5310ed2f243dc383003ddd8f8d64f9bd48576726af4824ea648049bce07"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/57/replies
Content-Type: application/json
Authorization: Bearer 233c419a77dd04bec65be3b426db5a4d4577d89b5bad153e83099bfb4e9801e4
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
    "id": 58,
    "author_id": 842,
    "reply_to_id": 57,
    "created_at": "2016-10-14T11:36:18.075Z",
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
curl "api.goskive.com/v2/comments/57/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 233c419a77dd04bec65be3b426db5a4d4577d89b5bad153e83099bfb4e9801e4"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer 8564ba0780a332a897e51cca1f2e269939ce122c40e7b0dba198a33123a57eab
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
curl "api.goskive.com/v2/comments/56/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8564ba0780a332a897e51cca1f2e269939ce122c40e7b0dba198a33123a57eab"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer d4d4c09ef63a8d5a19c773842999b412b6519e6635d0819d33ac17ee51ab5d38
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
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4d4c09ef63a8d5a19c773842999b412b6519e6635d0819d33ac17ee51ab5d38"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/49/republish
Content-Type: application/json
Authorization: Bearer 2b0a8a78c3c343d743b7f5c8cffcfd6abb070af3c1ef50e752222631eb6d8654
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
curl "api.goskive.com/v2/comments/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b0a8a78c3c343d743b7f5c8cffcfd6abb070af3c1ef50e752222631eb6d8654"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer 53048dd2a3d0b882d85de95add3d029a828a574092425fda4025517f3ce467cd
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53048dd2a3d0b882d85de95add3d029a828a574092425fda4025517f3ce467cd"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/51/report
Content-Type: application/json
Authorization: Bearer 32519fb422a4f2bae6e20b559dc85405d59c1312fe17a2e969e10f6a3607b6f4
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/51/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32519fb422a4f2bae6e20b559dc85405d59c1312fe17a2e969e10f6a3607b6f4"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer 4a659db64ffa7f5efb61ff8408504660ffd8148d3e2dba07e79f21c97bfcbdb8
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
    "updated_at": "2016-10-14T11:35:54.678Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a659db64ffa7f5efb61ff8408504660ffd8148d3e2dba07e79f21c97bfcbdb8"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer a8ebc67a7e6d863ea7c5ae9cfe6c6762c393c72ba1399571b27dc6fa604078ef
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
      "updated_at": "2016-10-14T11:35:54.757Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T11:35:54.762Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-14T11:35:54.766Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8ebc67a7e6d863ea7c5ae9cfe6c6762c393c72ba1399571b27dc6fa604078ef"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/23/company_profiles
Content-Type: application/json
Authorization: Bearer 724d7d3a6bd5c2e0b08efebc184cc2f48f6cf405902bfb32b2b9b781072442c6
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
curl "api.goskive.com/v2/companies/23/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 724d7d3a6bd5c2e0b08efebc184cc2f48f6cf405902bfb32b2b9b781072442c6"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/21/company_profiles
Content-Type: application/json
Authorization: Bearer 9c595004627c9ca0bb023e52cb330e3cc527bfa37dd2f9381ea3dda06aa42896
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
curl "api.goskive.com/v2/companies/21/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9c595004627c9ca0bb023e52cb330e3cc527bfa37dd2f9381ea3dda06aa42896"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer f01bfa0cc84a5a2da3f48a41e670105a5c2f4a6ce180db6edce9ab67a1a16ab4
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
	-H "Authorization: Bearer f01bfa0cc84a5a2da3f48a41e670105a5c2f4a6ce180db6edce9ab67a1a16ab4"
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
Authorization: Bearer 1a5765f638a676af2567e75dde570bf82dd1d2879f42170676a5cf940803dcb0
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
	-H "Authorization: Bearer 1a5765f638a676af2567e75dde570bf82dd1d2879f42170676a5cf940803dcb0"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 07c9ad71da8b2945c539dc3bd753ea5759511b2c286e5a55af40b4e597b766bb
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
    "id": 169,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T11:36:22.411Z",
    "course_id": 290,
    "author_id": 900,
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
	-H "Authorization: Bearer 07c9ad71da8b2945c539dc3bd753ea5759511b2c286e5a55af40b4e597b766bb"
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
      "title": "Clever Chapter Title 157",
      "position": 1,
      "updated_at": "2016-10-14T11:36:24.015Z",
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
      "id": 182,
      "title": "Clever Chapter Title 158",
      "position": 2,
      "updated_at": "2016-10-14T11:36:24.043Z",
      "course_id": 299,
      "author_id": 930,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 183,
      "title": "Clever Chapter Title 159",
      "position": 3,
      "updated_at": "2016-10-14T11:36:24.331Z",
      "course_id": 299,
      "author_id": 931,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T11:36:23.933Z",
      "questions_updated_at": "2016-10-14T11:36:23.933Z",
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
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f847531820805757c28de33b4166280eb71a7791c7c88da3613600da62d26e66
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
      "title": "Clever Chapter Title 163",
      "position": 1,
      "updated_at": "2016-10-14T11:36:24.767Z",
      "course_id": 302,
      "author_id": 940,
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
      "position": 2,
      "updated_at": "2016-10-14T11:36:24.793Z",
      "course_id": 302,
      "author_id": 941,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 189,
      "title": "Clever Chapter Title 165",
      "position": 3,
      "updated_at": "2016-10-14T11:36:25.069Z",
      "course_id": 302,
      "author_id": 942,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-14T11:36:24.686Z",
      "questions_updated_at": "2016-10-14T11:36:24.686Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f847531820805757c28de33b4166280eb71a7791c7c88da3613600da62d26e66"
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
      "title": "Clever Chapter Title 160",
      "position": 1,
      "updated_at": "2016-10-14T11:36:24.586Z",
      "course_id": 301,
      "author_id": 936,
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
      "position": 2,
      "updated_at": "2016-10-14T11:36:24.615Z",
      "course_id": 301,
      "author_id": 937,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 186,
      "title": "Clever Chapter Title 162",
      "position": 3,
      "updated_at": "2016-10-14T11:36:24.642Z",
      "course_id": 301,
      "author_id": 938,
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
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 49ce64cfc13203ab0c85db212cd7fb851d5aeac813e90c5c88099fe215775133
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
      "title": "Clever Chapter Title 166",
      "position": 1,
      "updated_at": "2016-10-14T11:36:25.246Z",
      "course_id": 303,
      "author_id": 947,
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
      "position": 2,
      "updated_at": "2016-10-14T11:36:25.272Z",
      "course_id": 303,
      "author_id": 948,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 192,
      "title": "Clever Chapter Title 168",
      "position": 3,
      "updated_at": "2016-10-14T11:36:25.297Z",
      "course_id": 303,
      "author_id": 949,
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
	-H "Authorization: Bearer 49ce64cfc13203ab0c85db212cd7fb851d5aeac813e90c5c88099fe215775133"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 09572ab77cb9817d1dfeb1d6e97f2dfba94d8a066b79489a0dde7b1eb35eaac7
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
    "course_id": 212,
    "user_id": 619,
    "updated_at": "2016-10-14T11:35:56.755Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09572ab77cb9817d1dfeb1d6e97f2dfba94d8a066b79489a0dde7b1eb35eaac7"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 36ca5548493d4fbd54ffc1533a9d629dd73ac6983743544c66cf9ce3c0855ad9
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
      "course_id": 217,
      "user_id": 631,
      "updated_at": "2016-10-14T11:35:57.397Z"
    },
    {
      "id": 7,
      "course_id": 217,
      "user_id": 632,
      "updated_at": "2016-10-14T11:35:57.413Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36ca5548493d4fbd54ffc1533a9d629dd73ac6983743544c66cf9ce3c0855ad9"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/40/files
Content-Type: application/json
Authorization: Bearer 6788330b6dc31d5e039b9a4ef5eaf07853cd9607ab3bc74d67d2f7735c37e5ea
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
        "id": 142,
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
        "created_at": "2016-10-14T11:35:23.178Z",
        "updated_at": "2016-10-14T11:35:23.178Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T11:35:23.193Z",
      "updated_at": "2016-10-14T11:35:23.193Z",
      "course_id": 40,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 143,
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
        "created_at": "2016-10-14T11:35:23.202Z",
        "updated_at": "2016-10-14T11:35:23.202Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T11:35:23.210Z",
      "updated_at": "2016-10-14T11:35:23.210Z",
      "course_id": 40,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 144,
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
        "created_at": "2016-10-14T11:35:23.217Z",
        "updated_at": "2016-10-14T11:35:23.217Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-14T11:35:23.225Z",
      "updated_at": "2016-10-14T11:35:23.225Z",
      "course_id": 40,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/40/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6788330b6dc31d5e039b9a4ef5eaf07853cd9607ab3bc74d67d2f7735c37e5ea"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/43/files
Content-Type: application/json
Authorization: Bearer e65b7262b0ace8358e639d578d1f93897538fd5c5e8e279fc8cbef9e1797e7cb
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
    "id": 4,
    "uploader": {
      "id": 151,
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
      "created_at": "2016-10-14T11:35:23.594Z",
      "updated_at": "2016-10-14T11:35:23.594Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-14T11:35:23.629Z",
    "updated_at": "2016-10-14T11:35:23.629Z",
    "course_id": 43,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/43/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e65b7262b0ace8358e639d578d1f93897538fd5c5e8e279fc8cbef9e1797e7cb"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/42/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer fa6e53689b5d786efaaf68bb960b30c385b95e95d790f7efae3293ea46ee4e90
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
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/6b42e05c652005d6d65c882ee772d3b2.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMjozNToyM1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS82YjQyZTA1YzY1MjAwNWQ2ZDY1Yzg4MmVlNzcyZDNiMi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTEzNTIzWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T113523Z",
    "x-amz-signature": "756a0f7e34210d666c10f35a64a89fcc53045155feac0085f4959cf92b061281"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/42/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa6e53689b5d786efaaf68bb960b30c385b95e95d790f7efae3293ea46ee4e90"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer acd67f2f711fc16b70895e8bc40e8450c8ba8e0314895cda4790b360499055b5
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
	-H "Authorization: Bearer acd67f2f711fc16b70895e8bc40e8450c8ba8e0314895cda4790b360499055b5"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8af5fa4f1d30e64ab6ab9e5861c5e1dd110519fc96891fa8643ac98f2db23317
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
	-H "Authorization: Bearer 8af5fa4f1d30e64ab6ab9e5861c5e1dd110519fc96891fa8643ac98f2db23317"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3c0b91cff2d688d73f2c118f2fed700da71bbb8b71f180c5ec64557d06877f2a
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
	-H "Authorization: Bearer 3c0b91cff2d688d73f2c118f2fed700da71bbb8b71f180c5ec64557d06877f2a"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 47b7a12e491cff44f97053983e2bfe6433d9d499d21384efdb4b5e2056d92e17
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
	-H "Authorization: Bearer 47b7a12e491cff44f97053983e2bfe6433d9d499d21384efdb4b5e2056d92e17"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ac4423d74d7220bdfe5a606ddb0fdab97b55b4b58c37d3e6ea20be68c7bee6eb
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
	-H "Authorization: Bearer ac4423d74d7220bdfe5a606ddb0fdab97b55b4b58c37d3e6ea20be68c7bee6eb"
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
    "creator_id": 116,
    "id": 35,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 36,
    "additional_university_ids": [

    ],
    "topic_id": 45,
    "discipline_id": 45,
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
    "chapters_updated_at": "2016-10-14T11:35:16.031Z",
    "updated_at": "2016-10-14T11:35:17.612Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 20,
        "title": "Clever Chapter Title 20",
        "position": 1,
        "updated_at": "2016-10-14T11:35:17.560Z",
        "course_id": 35,
        "author_id": 116,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T11:35:16.031Z",
        "questions_updated_at": "2016-10-14T11:35:16.031Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 21,
        "title": "Clever Chapter Title 21",
        "position": 2,
        "updated_at": "2016-10-14T11:35:17.604Z",
        "course_id": 35,
        "author_id": 116,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T11:35:16.031Z",
        "questions_updated_at": "2016-10-14T11:35:16.031Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 116,
        "chapter_id": 20,
        "position": 10,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:16.262Z",
        "created_at": "2016-10-14T11:35:16.131Z",
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
        "id": 12,
        "obfuscated_id": "4vzz6KHlMwo",
        "author_id": 116,
        "chapter_id": 21,
        "position": 12,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:16.679Z",
        "created_at": "2016-10-14T11:35:16.545Z",
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
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer d2f6fd93b3cc25aebdf5191f33e74d6acb46e2ce8d75056a682e1f7f34946683
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
    "creator_id": 121,
    "id": 36,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 37,
    "additional_university_ids": [

    ],
    "topic_id": 46,
    "discipline_id": 46,
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
    "chapters_updated_at": "2016-10-14T11:35:17.683Z",
    "updated_at": "2016-10-14T11:35:19.318Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 22,
        "title": "Clever Chapter Title 22",
        "position": 1,
        "updated_at": "2016-10-14T11:35:19.265Z",
        "course_id": 36,
        "author_id": 121,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T11:35:17.683Z",
        "questions_updated_at": "2016-10-14T11:35:17.683Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 23,
        "title": "Clever Chapter Title 23",
        "position": 2,
        "updated_at": "2016-10-14T11:35:19.310Z",
        "course_id": 36,
        "author_id": 121,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-14T11:35:17.683Z",
        "questions_updated_at": "2016-10-14T11:35:17.683Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 122,
        "chapter_id": 22,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:19.085Z",
        "created_at": "2016-10-14T11:35:19.085Z",
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
        "author_id": 122,
        "chapter_id": 23,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:19.165Z",
        "created_at": "2016-10-14T11:35:19.165Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 122,
        "chapter_id": 22,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:19.130Z",
        "created_at": "2016-10-14T11:35:19.130Z",
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
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 122,
        "chapter_id": 23,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:19.210Z",
        "created_at": "2016-10-14T11:35:19.210Z",
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
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 122,
        "chapter_id": 22,
        "position": 16,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:17.927Z",
        "created_at": "2016-10-14T11:35:17.794Z",
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
            "id": 31,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 32,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 122,
        "chapter_id": 22,
        "position": 17,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:18.124Z",
        "created_at": "2016-10-14T11:35:17.997Z",
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
            "id": 33,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 34,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 122,
        "chapter_id": 23,
        "position": 18,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:18.357Z",
        "created_at": "2016-10-14T11:35:18.218Z",
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
            "id": 35,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 36,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 122,
        "chapter_id": 23,
        "position": 19,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:18.566Z",
        "created_at": "2016-10-14T11:35:18.433Z",
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
            "id": 37,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 38,
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
	-H "Authorization: Bearer d2f6fd93b3cc25aebdf5191f33e74d6acb46e2ce8d75056a682e1f7f34946683"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/21/pin
Content-Type: application/json
Authorization: Bearer 3744c13830d6ffcebed92bd1e6b470bb54500ceedb17bf3798b3f959f638a29e
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/21/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3744c13830d6ffcebed92bd1e6b470bb54500ceedb17bf3798b3f959f638a29e"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/39/pin
Content-Type: application/json
Authorization: Bearer 2b4f4dbecc905452874f41a5809dfa5012c9b7dd9c9bb34f9acd32a9c3e8493f
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/39/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b4f4dbecc905452874f41a5809dfa5012c9b7dd9c9bb34f9acd32a9c3e8493f"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9f3f9ba93606ca92121b30f2ac0394e9a8ce3ab9c9e36e9276cc0874f7540639
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
    "creator_id": 91,
    "id": 23,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 24,
    "additional_university_ids": [

    ],
    "topic_id": 33,
    "discipline_id": 33,
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
    "updated_at": "2016-10-14T11:35:14.057Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f3f9ba93606ca92121b30f2ac0394e9a8ce3ab9c9e36e9276cc0874f7540639"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer bde6a6602c6fed6b7aee2ea9f99513d5c92e1d51f20460c620aaf727f4e2cbdc
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
    "id": 47,
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
    "created_at": "2016-10-14T11:35:10.840Z",
    "updated_at": "2016-10-14T11:35:10.840Z",
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
	-H "Authorization: Bearer bde6a6602c6fed6b7aee2ea9f99513d5c92e1d51f20460c620aaf727f4e2cbdc"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer eaffabaeb18ac42101a032a1ab22fa2b187cd6f2b93bd12f64c52c5e54ca2724
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[18]}
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
    "id": 42,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      18
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T11:35:10.151Z",
    "updated_at": "2016-10-14T11:35:10.202Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[18]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaffabaeb18ac42101a032a1ab22fa2b187cd6f2b93bd12f64c52c5e54ca2724"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0bda89465a96610ed9e1402f975f816e5d566f517f53e89965dbe98489a1f7c8
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
    "id": 43,
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
    "created_at": "2016-10-14T11:35:10.238Z",
    "updated_at": "2016-10-14T11:35:10.238Z",
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
	-H "Authorization: Bearer 0bda89465a96610ed9e1402f975f816e5d566f517f53e89965dbe98489a1f7c8"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 3eba9af23bf11d56e53aa76d0853705bb0f9e4db96ba772a0d3d24a8c6304b87
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[20]}
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
    "id": 44,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      20
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T11:35:10.337Z",
    "updated_at": "2016-10-14T11:35:10.337Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[20]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eba9af23bf11d56e53aa76d0853705bb0f9e4db96ba772a0d3d24a8c6304b87"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 04042a26e9ba1c23bcf9177ef25ec533263d7054623c12e7df99baa38f9745ac
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

22
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
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/fade0e36667af11c97c376776156d8013608c6cd.jpg",
    "university_id": null,
    "fields_of_study": [
      22
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-14T11:35:10.491Z",
    "updated_at": "2016-10-14T11:35:10.809Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/6826705c9baa635e267a92cf4ab94a5f8101fff6.jpg",
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

22
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 04042a26e9ba1c23bcf9177ef25ec533263d7054623c12e7df99baa38f9745ac"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer dd026845d175f95b4b600fd698e3e2bc6e315b6afb894a0f149b459f9a0381f3
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
      "id": 2,
      "bookmarkable_id": 5,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 6,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 7,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd026845d175f95b4b600fd698e3e2bc6e315b6afb894a0f149b459f9a0381f3"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 71593e8c7e837b854f2d87098e1af53976224200d255e9d17529a92e10bc3ad0
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
      "company_id": 32,
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
      "id": 12,
      "title": "Campaign 11",
      "company_id": 33,
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
	-H "Authorization: Bearer 71593e8c7e837b854f2d87098e1af53976224200d255e9d17529a92e10bc3ad0"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer e2e0b9494dfb7b6ceca4690a0e787a198cfec5a05e30f73830297f651bfbb577
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
      "company_id": 28,
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
	-H "Authorization: Bearer e2e0b9494dfb7b6ceca4690a0e787a198cfec5a05e30f73830297f651bfbb577"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 88909b987d53ad1ea12cb2689e5b0b3f29ced7c6ba989f75121a9223915ae560
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
      "creator_id": 378,
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-108",
      "html_url": "https://goskive.com/course/mit-course-108",
      "slug": "mit-course-108",
      "university_id": 118,
      "additional_university_ids": [

      ],
      "topic_id": 148,
      "discipline_id": 148,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
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
      "updated_at": "2016-10-14T11:35:41.154Z",
      "shortname": "mit-course-108"
    },
    {
      "creator_id": 379,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-109",
      "html_url": "https://goskive.com/course/mit-course-109",
      "slug": "mit-course-109",
      "university_id": 119,
      "additional_university_ids": [

      ],
      "topic_id": 149,
      "discipline_id": 149,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
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
      "updated_at": "2016-10-14T11:35:41.235Z",
      "shortname": "mit-course-109"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88909b987d53ad1ea12cb2689e5b0b3f29ced7c6ba989f75121a9223915ae560"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8764caf9a4ff2382ff8aa7b4b974387826dbc50585a71c93af007e837fc61d49
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
        "updated_at": "2016-10-14T11:35:13.528Z"
      },
      "created_at": "2016-10-14T11:35:13.532Z",
      "updated_at": "2016-10-14T11:35:13.532Z",
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
        "updated_at": "2016-10-14T11:35:13.541Z"
      },
      "created_at": "2016-10-14T11:35:13.544Z",
      "updated_at": "2016-10-14T11:35:13.544Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8764caf9a4ff2382ff8aa7b4b974387826dbc50585a71c93af007e837fc61d49"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer b90520eeccbe951ffc933e7c92ff089740f62fbba4adfeb62245fcb9fe758381
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
        "updated_at": "2016-10-14T11:35:13.264Z"
      },
      "created_at": "2016-10-14T11:35:13.269Z",
      "updated_at": "2016-10-14T11:35:13.269Z",
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
        "updated_at": "2016-10-14T11:35:13.284Z"
      },
      "created_at": "2016-10-14T11:35:13.288Z",
      "updated_at": "2016-10-14T11:35:13.288Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b90520eeccbe951ffc933e7c92ff089740f62fbba4adfeb62245fcb9fe758381"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 75abb225a0aaae985d0437810787711f5b8a1d26db4a688f497d9b1f7e04edbf
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
      "id": 11,
      "created_at": "2016-10-14T11:36:03.022Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 53,
      "updated_at": "2016-10-14T11:36:03.138Z",
      "author_id": "688",
      "thread_subject_id": "230",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 12,
      "created_at": "2016-10-14T11:36:03.126Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 54,
      "updated_at": "2016-10-14T11:36:03.143Z",
      "author_id": "691",
      "thread_subject_id": "231",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-10-14T11:36:03.530Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 14,
      "updated_at": "2016-10-14T11:36:03.530Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-10-14T11:36:03.920Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-10-14T11:36:03.920Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 15,
      "created_at": "2016-10-14T11:36:04.303Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-14T11:36:04.303Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 16,
      "created_at": "2016-10-14T11:36:04.602Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 85,
      "updated_at": "2016-10-14T11:36:04.602Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-10-14T11:36:04.908Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 86,
      "updated_at": "2016-10-14T11:36:04.908Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-10-14T11:36:05.236Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 87,
      "updated_at": "2016-10-14T11:36:05.236Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75abb225a0aaae985d0437810787711f5b8a1d26db4a688f497d9b1f7e04edbf"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/19
Content-Type: application/json
Authorization: Bearer 3741a50310b1d56f5d5166854efc6c6dcd5dae4a9fd0f702f135f60d774bf797
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-14T11:26:05.000Z"}}
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
    "id": 19,
    "created_at": "2016-10-14T11:36:05.379Z",
    "read_at": "2016-10-14T11:26:05.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 55,
    "updated_at": "2016-10-14T11:36:05.420Z",
    "author_id": "716",
    "thread_subject_id": "238",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/19" -d '{"notification":{"read_at":"2016-10-14T11:26:05.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3741a50310b1d56f5d5166854efc6c6dcd5dae4a9fd0f702f135f60d774bf797"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer c95b26dc54736cf927cd3c469c15f8e8051ef015bcc82fed302691c0c0486dc3
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
      "course_id": 48,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T11:35:24.656Z",
      "course_published": true,
      "updated_at": "2016-10-14T11:35:24.648Z"
    },
    {
      "id": 6,
      "course_id": 49,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-14T11:35:24.739Z",
      "course_published": true,
      "updated_at": "2016-10-14T11:35:24.732Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c95b26dc54736cf927cd3c469c15f8e8051ef015bcc82fed302691c0c0486dc3"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer d5d27d04d108fed32ea888cdae92c90fb62392ac5b5a71b4753d9f77cc0b9f3d
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
    "course_id": 44,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-14T11:35:24.053Z",
    "course_published": true,
    "updated_at": "2016-10-14T11:35:24.044Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5d27d04d108fed32ea888cdae92c90fb62392ac5b5a71b4753d9f77cc0b9f3d"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/3
Content-Type: application/json
Authorization: Bearer 1125762713fb5fcec6d7af1bb9ba0ada787ee49b6c14c33c0f2f3f6e0e78362b
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
    "course_id": 45,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-14T11:35:24.264Z",
    "course_published": true,
    "updated_at": "2016-10-14T11:35:24.251Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/3" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1125762713fb5fcec6d7af1bb9ba0ada787ee49b6c14c33c0f2f3f6e0e78362b"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer abb6cf1eecb2aad609d45f0a2694aa47ffbfd7b295071c817cf70397c0430ce8
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
      "votable_id": 38,
      "user_id": 231
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 39,
      "user_id": 231
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 40,
      "user_id": 231
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 41,
      "user_id": 231
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abb6cf1eecb2aad609d45f0a2694aa47ffbfd7b295071c817cf70397c0430ce8"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/224
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
    "id": 224,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 222,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 224
      },
      {
        "id": 223,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 224
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/224" -X GET \
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
      "id": 222,
      "name": "Versatile homogeneous process improvement",
      "name_translations": {
        "en": "Versatile homogeneous process improvement"
      }
    },
    {
      "id": 223,
      "name": "Exclusive eco-centric focus group",
      "name_translations": {
        "en": "Exclusive eco-centric focus group"
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
PATCH /v2/feedbacks/11/close
Content-Type: application/json
Authorization: Bearer 5bdb542d95daa730d35cf73e2fb3917e8de5b07d5726a657645c2e5d8dfa6120
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
    "id": 11,
    "user_id": 479,
    "feedbackable_id": 75,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-14T11:35:45.913Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/11/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bdb542d95daa730d35cf73e2fb3917e8de5b07d5726a657645c2e5d8dfa6120"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/33/fix
Content-Type: application/json
Authorization: Bearer 65b2a67f8e3b81d1b3600e7a3ab7f1b466140ca4977cc64d19f009da75324fee
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
    "id": 33,
    "user_id": 575,
    "feedbackable_id": 78,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-14T11:35:52.959Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/33/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65b2a67f8e3b81d1b3600e7a3ab7f1b466140ca4977cc64d19f009da75324fee"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/37
Content-Type: application/json
Authorization: Bearer e2f687ad8a6672cfe7555d2093d68aeca2757d7962bf6b93dc9a8b6bc7271b1e
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
    "id": 37,
    "user_id": 595,
    "feedbackable_id": 82,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T11:35:54.150Z",
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
curl "api.goskive.com/v2/feedbacks/37" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2f687ad8a6672cfe7555d2093d68aeca2757d7962bf6b93dc9a8b6bc7271b1e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/close
Content-Type: application/json
Authorization: Bearer 44eb53c8079295208e7f60ef4f59d9e0aa4ddd29df826e17bd74ebc41ef0feb6
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
curl "api.goskive.com/v2/feedbacks/13/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44eb53c8079295208e7f60ef4f59d9e0aa4ddd29df826e17bd74ebc41ef0feb6"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/fix
Content-Type: application/json
Authorization: Bearer e1a1a84660d818e3da795170238248d232ab87d4e85c08ce85ebbc989b438892
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
curl "api.goskive.com/v2/feedbacks/35/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1a1a84660d818e3da795170238248d232ab87d4e85c08ce85ebbc989b438892"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/36/fix
Content-Type: application/json
Authorization: Bearer 2120198e5b593eb272721e23d5802add46e3445369b2ebbd229375f54f77359e
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
curl "api.goskive.com/v2/feedbacks/36/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2120198e5b593eb272721e23d5802add46e3445369b2ebbd229375f54f77359e"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/38
Content-Type: application/json
Authorization: Bearer 98f8fc5d079675010bd3542fe0074cabfe89ca4e0fbbd07939e0a788507c3037
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
    "id": 38,
    "user_id": 600,
    "feedbackable_id": 83,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T11:35:54.446Z",
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
curl "api.goskive.com/v2/feedbacks/38" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98f8fc5d079675010bd3542fe0074cabfe89ca4e0fbbd07939e0a788507c3037"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Authorization: Bearer 86945ae908a492b236a42b5a7db36e0a0cfeb96952ebdf5bea7b76d65f936b8a
Content-Type: application/x-www-form-urlencoded
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
	-H "Authorization: Bearer 86945ae908a492b236a42b5a7db36e0a0cfeb96952ebdf5bea7b76d65f936b8a" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Authorization: Bearer 1c39b9b33aa2d6cc95fd7c964b4bac37e042e47f6d031319d8b592ff03ffec4b
Content-Type: application/x-www-form-urlencoded
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Authorization: Bearer 1c39b9b33aa2d6cc95fd7c964b4bac37e042e47f6d031319d8b592ff03ffec4b" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/8
Authorization: Bearer 39f3655d4a4b873beced62c6709b20df235d7879d48ce042c68db7ad7d004a76
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/65500ab19465040098f8b14d67db597e.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T113621Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=1fb7b9442144787e4c754b69a2550bd5da76ce6ac50466c223762f24108cca1c"
  }
}
```



```shell
curl "api.goskive.com/v2/files/8" -X GET \
	-H "Authorization: Bearer 39f3655d4a4b873beced62c6709b20df235d7879d48ce042c68db7ad7d004a76"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Authorization: Bearer 23359f33937749bd78b5f48ae5db2f0472516c727503461513b2b46b4397d0ee
Content-Type: application/json
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
      "id": 885,
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
      "created_at": "2016-10-14T11:36:21.696Z",
      "updated_at": "2016-10-14T11:36:21.696Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-14T11:36:21.771Z",
    "updated_at": "2016-10-14T11:36:21.771Z",
    "course_id": 285,
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
curl "api.goskive.com/v2/files/9/metadata" -X GET \
	-H "Authorization: Bearer 23359f33937749bd78b5f48ae5db2f0472516c727503461513b2b46b4397d0ee" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/5/matched_courses?required_cu_count=2
Authorization: Bearer daf5583682af57be137ba44edf4c10c1762490bdd281d9cecd4b159429a36056
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
      "creator_id": 644,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 232,
      "discipline_id": 233,
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
      "chapters_updated_at": "2016-10-14T11:35:57.476Z",
      "updated_at": "2016-10-14T11:35:59.111Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 649,
      "id": 221,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-d9ee4766-b474-474b-9995-1364c16f59c5",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-d9ee4766-b474-474b-9995-1364c16f59c5",
      "slug": "mit-the-great-british-bake-off-d9ee4766-b474-474b-9995-1364c16f59c5",
      "university_id": 201,
      "additional_university_ids": [

      ],
      "topic_id": 233,
      "discipline_id": 234,
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
      "chapters_updated_at": "2016-10-14T11:35:57.476Z",
      "updated_at": "2016-10-14T11:35:59.660Z",
      "shortname": "mit-the-great-british-bake-off-d9ee4766-b474-474b-9995-1364c16f59c5"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/5/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer daf5583682af57be137ba44edf4c10c1762490bdd281d9cecd4b159429a36056"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/7/preview
Authorization: Bearer 46b89d81e24ff7a528ef4d8cac4386d86eb5eca1c427973eda6e629b91f108cd
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/4129271e6d5259e6431fc87d76c278ed.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161014%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161014T113621Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=81b2d6db27782b2bbd99ccffa2cc63f03437add5769c82b593063003b3cc9874"
  }
}
```



```shell
curl "api.goskive.com/v2/files/7/preview" -X GET \
	-H "Authorization: Bearer 46b89d81e24ff7a528ef4d8cac4386d86eb5eca1c427973eda6e629b91f108cd"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/13/report
Authorization: Bearer 99f692bc8eee7b0d64c5ace3a175351c703ef63c19de9d973c7bd971dd1b0ac2
Content-Type: application/x-www-form-urlencoded
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
	-H "Authorization: Bearer 99f692bc8eee7b0d64c5ace3a175351c703ef63c19de9d973c7bd971dd1b0ac2" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/72/comments
Content-Type: application/json
Authorization: Bearer 723a4ee556ac77c96071ebca4236de15cf47bee4093168f6bf0b2b4718b3b669
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
    "id": 9,
    "author_id": 362,
    "reply_to_id": null,
    "created_at": "2016-10-14T11:35:39.914Z",
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
curl "api.goskive.com/v2/flashcards/72/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 723a4ee556ac77c96071ebca4236de15cf47bee4093168f6bf0b2b4718b3b669"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/73/comments
Content-Type: application/json
Authorization: Bearer d19949e60206348d00cab09cac6a9fcbdfc454b04866d796d77053801527d998
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
    "id": 10,
    "author_id": 365,
    "reply_to_id": null,
    "created_at": "2016-10-14T11:35:40.227Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 10,
      "user_id": 365,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:40.225Z",
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
curl "api.goskive.com/v2/flashcards/73/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d19949e60206348d00cab09cac6a9fcbdfc454b04866d796d77053801527d998"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/70/comments
Content-Type: application/json
Authorization: Bearer 6ce82c7b3cda812625237c7d0d118e5a9efd5189b5250efdef3dbecd0ae9e603
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
      "id": 8,
      "author_id": 358,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:39.545Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 357,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:39.529Z",
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
curl "api.goskive.com/v2/flashcards/70/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6ce82c7b3cda812625237c7d0d118e5a9efd5189b5250efdef3dbecd0ae9e603"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/74/comments
Content-Type: application/json
Authorization: Bearer 9bcfadc6817320876e7fefb09059daa5835d900fb77c1463c9136f3cc58e2cc8
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
curl "api.goskive.com/v2/flashcards/74/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bcfadc6817320876e7fefb09059daa5835d900fb77c1463c9136f3cc58e2cc8"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/7/feedbacks
Content-Type: application/json
Authorization: Bearer 300d01d12ff73c16af3fd383f127e0499075e98aaa89d9e57e399dc17ef48402
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
    "id": 7,
    "user_id": 78,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-14T11:35:12.392Z",
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
	-H "Authorization: Bearer 300d01d12ff73c16af3fd383f127e0499075e98aaa89d9e57e399dc17ef48402"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/5/feedbacks
Content-Type: application/json
Authorization: Bearer 862b62b13dc325b444fa1d7822cc29bb8582f75f5c10b6594053703aebb25728
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
      "id": 6,
      "user_id": 74,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:11.929Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 73,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:11.917Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 862b62b13dc325b444fa1d7822cc29bb8582f75f5c10b6594053703aebb25728"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/43/votes
Content-Type: application/json
Authorization: Bearer 1b81f342baee6074ca5bd6c0b36d3b145971e9dfbb8ed6dbad6285482cbfba32
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
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 43,
      "user_id": 250
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 43,
      "user_id": 249
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 43,
      "user_id": 248
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b81f342baee6074ca5bd6c0b36d3b145971e9dfbb8ed6dbad6285482cbfba32"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/51/republish
Content-Type: application/json
Authorization: Bearer a245df1db6c369bad6ff5837974bc3dd575658bcc86d76835051ffdadbfb8951
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
curl "api.goskive.com/v2/flashcards/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a245df1db6c369bad6ff5837974bc3dd575658bcc86d76835051ffdadbfb8951"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/46/bookmark
Content-Type: application/json
Authorization: Bearer 8e4d3a901e7a7cc6ce95a40b0bdcbe8bb9aed0c9bd61a99eec9872aa3b687036
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/46/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e4d3a901e7a7cc6ce95a40b0bdcbe8bb9aed0c9bd61a99eec9872aa3b687036"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50
Content-Type: application/json
Authorization: Bearer 485b1e3dc7448ca3ecaaae64bb34182b6a7477b034147173d6ee709d0ca2e0ed
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/50" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 485b1e3dc7448ca3ecaaae64bb34182b6a7477b034147173d6ee709d0ca2e0ed"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/68/downvote
Content-Type: application/json
Authorization: Bearer c154e24d921a9cc22908b5c876f27187293fd2c6ee3c9f64c4ba13b0308f3865
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/68/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c154e24d921a9cc22908b5c876f27187293fd2c6ee3c9f64c4ba13b0308f3865"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/47
Content-Type: application/json
Authorization: Bearer 50b63e1155ef35e23f54802ed9b59f35e7ce33b96646197720310ca5e188ca9a
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
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 280,
    "chapter_id": 51,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:35:35.527Z",
    "created_at": "2016-10-14T11:35:35.527Z",
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
curl "api.goskive.com/v2/flashcards/47" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50b63e1155ef35e23f54802ed9b59f35e7ce33b96646197720310ca5e188ca9a"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/48/report
Content-Type: application/json
Authorization: Bearer aabd59c27446006b4e3161087e8fa9e27e6f71d995867c4d0f3ed81b06bb0539
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/48/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aabd59c27446006b4e3161087e8fa9e27e6f71d995867c4d0f3ed81b06bb0539"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/49/bookmark
Content-Type: application/json
Authorization: Bearer 1b632f71092cd0a42788581c90d402ec28789806ed15bc2be45b069b456addad
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b632f71092cd0a42788581c90d402ec28789806ed15bc2be45b069b456addad"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/upvote
Content-Type: application/json
Authorization: Bearer a1bf40a2309caf4bc6ed8ff68dfbad5d626d4e4749e2567153ef1a7c53c077c2
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1bf40a2309caf4bc6ed8ff68dfbad5d626d4e4749e2567153ef1a7c53c077c2"
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
  "url": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de",
  "fields": {
    "key": "cache/3d65fbc1669b867fb39d8beb7c591652.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xNFQxMjozNTowNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8zZDY1ZmJjMTY2OWI4NjdmYjM5ZDhiZWI3YzU5MTY1Mi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxNC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTRUMTEzNTA0WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161014/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161014T113504Z",
    "x-amz-signature": "491720f0c2d90d7f881fb779af9eec918110e7c9bafa321c5a02a4fa7e114dba"
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
Authorization: Bearer b581742363e39a24fe11ea7b141433868711d24691a34a815aab63893377668e
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
	-H "Authorization: Bearer b581742363e39a24fe11ea7b141433868711d24691a34a815aab63893377668e"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 475b6051e20e3606319fb7921dfee1fc7fc9735979888ef9d4e8838e908f8668
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
	-H "Authorization: Bearer 475b6051e20e3606319fb7921dfee1fc7fc9735979888ef9d4e8838e908f8668"
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
{"password":{"reset_password_token":"RwwNSMyyoZtRqH7eH1e2","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 612,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-14T11:35:55.482Z",
  "updated_at": "2016-10-14T11:35:55.697Z",
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
  "audit_id": 4400
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"RwwNSMyyoZtRqH7eH1e2","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/42/comments
Content-Type: application/json
Authorization: Bearer f98ab4153deec7fc71914208e18356ae60f385d0922e468e794511532db8f01f
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
    "id": 3,
    "author_id": 257,
    "reply_to_id": null,
    "created_at": "2016-10-14T11:35:33.208Z",
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
curl "api.goskive.com/v2/questions/42/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f98ab4153deec7fc71914208e18356ae60f385d0922e468e794511532db8f01f"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/44/comments
Content-Type: application/json
Authorization: Bearer 0cdc51db0280b26decba7a5381de8f0e60e69eb47ce7d25fe687dfe693d38362
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
    "id": 4,
    "author_id": 263,
    "reply_to_id": null,
    "created_at": "2016-10-14T11:35:34.007Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 263,
      "feedbackable_id": 44,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:34.003Z",
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
curl "api.goskive.com/v2/questions/44/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cdc51db0280b26decba7a5381de8f0e60e69eb47ce7d25fe687dfe693d38362"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/45/comments
Content-Type: application/json
Authorization: Bearer c481d26a9ae3daea7c0a2e780c83827f152a2781a46dcd7cf2a944c704928c44
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
      "id": 5,
      "author_id": 269,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:34.454Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 270,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:34.471Z",
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
curl "api.goskive.com/v2/questions/45/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c481d26a9ae3daea7c0a2e780c83827f152a2781a46dcd7cf2a944c704928c44"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/43/comments
Content-Type: application/json
Authorization: Bearer 85bf4a5bfe47523c4cb823152baada55e306a93e8ec3cc63f183536c2f08a8fe
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
curl "api.goskive.com/v2/questions/43/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85bf4a5bfe47523c4cb823152baada55e306a93e8ec3cc63f183536c2f08a8fe"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/122/feedbacks
Content-Type: application/json
Authorization: Bearer 2f12034c49e493a1797b4d4b828b2c66c08fb8cb8b68a08d1a500b7b9721b318
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
    "id": 40,
    "user_id": 846,
    "feedbackable_id": 122,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-14T11:36:19.086Z",
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
curl "api.goskive.com/v2/questions/122/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f12034c49e493a1797b4d4b828b2c66c08fb8cb8b68a08d1a500b7b9721b318"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/128/feedbacks
Content-Type: application/json
Authorization: Bearer 2b54487b292e858bd59861273034d3395d99f54d39f444ef0145338afc6deb6c
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
      "id": 46,
      "user_id": 878,
      "feedbackable_id": 128,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:36:21.313Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 877,
      "feedbackable_id": 128,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:36:21.302Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/128/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b54487b292e858bd59861273034d3395d99f54d39f444ef0145338afc6deb6c"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/133/votes
Content-Type: application/json
Authorization: Bearer 7fa3ee73f4236c31800f93d2ebf97d16c6010d35c074095d6711837e81c00f59
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
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 961
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 960
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 959
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/133/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7fa3ee73f4236c31800f93d2ebf97d16c6010d35c074095d6711837e81c00f59"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/104/republish
Content-Type: application/json
Authorization: Bearer c02a9a462ba6e59b05ae4c1ca4ec64549a8f3baf272dabea3641fa26d5f8b59e
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
curl "api.goskive.com/v2/questions/104/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c02a9a462ba6e59b05ae4c1ca4ec64549a8f3baf272dabea3641fa26d5f8b59e"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/112/bookmark
Content-Type: application/json
Authorization: Bearer 2f80bc3a7cf7ffa7267198d197da807c2a7ff91224f31055cd2812c06f2f71ab
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
	-H "Authorization: Bearer 2f80bc3a7cf7ffa7267198d197da807c2a7ff91224f31055cd2812c06f2f71ab"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/106
Content-Type: application/json
Authorization: Bearer 46b71e1421cbefe8635f4afce5a341d5fabda3bb52e58209dc5c6036fd772896
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/106" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46b71e1421cbefe8635f4afce5a341d5fabda3bb52e58209dc5c6036fd772896"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/88/downvote
Content-Type: application/json
Authorization: Bearer 6a7e83a105e38fec5fef67100fac3173a3a07165bb03c12e997e119745da741e
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/88/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a7e83a105e38fec5fef67100fac3173a3a07165bb03c12e997e119745da741e"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/108
Content-Type: application/json
Authorization: Bearer f8905ad795278e8ba0ead564cdc4b5b404bea3f83f0410b1d305efbf65f1642b
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 783,
    "chapter_id": 145,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:12.595Z",
    "created_at": "2016-10-14T11:36:12.471Z",
    "tags": [
      {
        "id": 10,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 9,
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/108" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8905ad795278e8ba0ead564cdc4b5b404bea3f83f0410b1d305efbf65f1642b"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/111/report
Content-Type: application/json
Authorization: Bearer aff96fe0c7cb04d9ee5ad92f5b0f6b90a073e2d3d05ca45f2e1fa0ca9145dfeb
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aff96fe0c7cb04d9ee5ad92f5b0f6b90a073e2d3d05ca45f2e1fa0ca9145dfeb"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/110/bookmark
Content-Type: application/json
Authorization: Bearer 87e6a20113d9106c3aa4b77fe91b0b536bc26397deaee6ad70f5b2c3914fe2fb
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87e6a20113d9106c3aa4b77fe91b0b536bc26397deaee6ad70f5b2c3914fe2fb"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/107
Content-Type: application/json
Authorization: Bearer 6da30cea2c7c4657210a92396ca9966d6cf179abcbd54933b17475d43a440e56
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":107,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T11:36:11.956Z","updated_at":"2016-10-14T11:36:12.082Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":144,"author_id":780,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 107,
    "obfuscated_id": "_2rgp7tgq8o",
    "author_id": 780,
    "chapter_id": 144,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-14T11:36:12.196Z",
    "created_at": "2016-10-14T11:36:11.956Z",
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
    "question": "{\"id\"=>107, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-14T11:36:11.956Z\", \"updated_at\"=>\"2016-10-14T11:36:12.082Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>144, \"author_id\"=>780, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 216,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 217,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 218,
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
curl "api.goskive.com/v2/questions/107" -d '{"question":{"question":{"id":107,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-14T11:36:11.956Z","updated_at":"2016-10-14T11:36:12.082Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":144,"author_id":780,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6da30cea2c7c4657210a92396ca9966d6cf179abcbd54933b17475d43a440e56"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/109/upvote
Content-Type: application/json
Authorization: Bearer ca25960c7b88c09fba33546d68d0df096b1f3ceb981984533f5ccad7e0d2c833
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca25960c7b88c09fba33546d68d0df096b1f3ceb981984533f5ccad7e0d2c833"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 8f13b5df1f236d39d8222bd93d63059867c77fd90bffcfe827419979f7df74d6
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
      "creator_id": 374,
      "id": 135,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 116,
      "additional_university_ids": [

      ],
      "topic_id": 145,
      "discipline_id": 145,
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
      "updated_at": "2016-10-14T11:35:40.863Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f13b5df1f236d39d8222bd93d63059867c77fd90bffcfe827419979f7df74d6"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b522d241ee91416db0e2a211accffaadb62331909f7548699647f78f65ce9cae
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
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-96",
      "html_url": "https://goskive.com/university/uni-96",
      "slug": "uni-96",
      "name": "National School of Pizza",
      "short_name": "Uni 96",
      "acronym": "NSPI",
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
      "updated_at": "2016-10-14T11:35:40.642Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 113,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-95",
      "html_url": "https://goskive.com/university/uni-95",
      "slug": "uni-95",
      "name": "National School of Pastry",
      "short_name": "Uni 95",
      "acronym": "NSPA",
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
      "updated_at": "2016-10-14T11:35:40.626Z",
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
	-H "Authorization: Bearer b522d241ee91416db0e2a211accffaadb62331909f7548699647f78f65ce9cae"
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
      "id": 2,
      "name": "Up-sized grid-enabled database",
      "name_translations": {
        "en": "Up-sized grid-enabled database"
      },
      "discipline_id": 2
    },
    {
      "id": 3,
      "name": "Cross-group heuristic product",
      "name_translations": {
        "en": "Cross-group heuristic product"
      },
      "discipline_id": 3
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
GET /v2/topics/1
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
    "id": 1,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 1
  }
}
```



```shell
curl "api.goskive.com/v2/topics/1" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 89ffc3caab4b711a88b205c771657c220e185ac3b7e1549c6a73432d402d8275
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
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-194",
      "html_url": "https://goskive.com/university/uni-194",
      "slug": "uni-194",
      "name": "University 155",
      "short_name": "Uni 194",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/00a31358daafcf5bb69c7f7fe9a4f7834d0b34e1.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2cad3d6b785347184fb4aaf7589f7acdba85adc7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T11:36:02.621Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-193",
      "html_url": "https://goskive.com/university/uni-193",
      "slug": "uni-193",
      "name": "University 154",
      "short_name": "Uni 193",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d1110a973573c8974a39e5f6375fbdb606ee1c84.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ff09bc3bf3d009bff704e63ea3ef6b24839d4267.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T11:36:02.603Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-192",
      "html_url": "https://goskive.com/university/uni-192",
      "slug": "uni-192",
      "name": "University 153",
      "short_name": "Uni 192",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/80d702cfb8e72a69d8d05f8e08a870b3bc13ea2d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/bfff9977589a73d0f8ea06b648e77142051d97bd.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-14T11:36:02.585Z",
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
	-H "Authorization: Bearer 89ffc3caab4b711a88b205c771657c220e185ac3b7e1549c6a73432d402d8275"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 48da1d28d227db197aef61d27c8d5d655f683cdec53e2d97b3f72982b177e73c
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
    "id": 214,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8efdb8264c7f4a28df19e2f795afb7290e8efd49.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ad9fd4421755460f2afe46727848c3fa475fafa0.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-14T11:36:02.809Z",
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
	-H "Authorization: Bearer 48da1d28d227db197aef61d27c8d5d655f683cdec53e2d97b3f72982b177e73c"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3d7c891764582ccef4a767dc57f784355c7118e526f3b262f99b897b70d942f3
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":98,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 217,
    "id": 88,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 67,
    "additional_university_ids": [

    ],
    "topic_id": 98,
    "discipline_id": 98,
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
    "chapters_updated_at": "2016-10-14T11:35:29.149Z",
    "updated_at": "2016-10-14T11:35:29.293Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 32,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-14T11:35:29.247Z",
        "course_id": 88,
        "author_id": 217,
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
        "id": 33,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-14T11:35:29.266Z",
        "course_id": 88,
        "author_id": 217,
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
        "id": 34,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-14T11:35:29.283Z",
        "course_id": 88,
        "author_id": 217,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":98,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d7c891764582ccef4a767dc57f784355c7118e526f3b262f99b897b70d942f3"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 25feaeb3bebdb052f92b7946126071e79d7673283af280cd5045eb71befcb61d
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":99,"published":false}}
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
    "creator_id": 218,
    "id": 89,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 68,
    "additional_university_ids": [

    ],
    "topic_id": 99,
    "discipline_id": 99,
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
    "updated_at": "2016-10-14T11:35:29.444Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":99,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25feaeb3bebdb052f92b7946126071e79d7673283af280cd5045eb71befcb61d"
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
      "creator_id": 179,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-37",
      "html_url": "https://goskive.com/course/fu-course-37",
      "slug": "fu-course-37",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "topic_id": 66,
      "discipline_id": 66,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 37",
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
      "updated_at": "2016-10-14T11:35:25.514Z",
      "shortname": "fu-course-37"
    },
    {
      "creator_id": 179,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-38",
      "html_url": "https://goskive.com/course/fu-course-38",
      "slug": "fu-course-38",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "topic_id": 67,
      "discipline_id": 67,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 38",
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
      "chapters_updated_at": "2016-10-14T11:35:25.853Z",
      "updated_at": "2016-10-14T11:35:25.860Z",
      "shortname": "fu-course-38"
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
Authorization: Bearer d51a8ed987e12b24826a83cda0e911c9bb9b0a5db93c1505475bcca12fbad383
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
      "creator_id": 186,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 74,
      "discipline_id": 74,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 45",
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
      "updated_at": "2016-10-14T11:35:26.320Z",
      "shortname": "fu-course-45"
    },
    {
      "creator_id": 186,
      "id": 65,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 75,
      "discipline_id": 75,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 46",
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
      "chapters_updated_at": "2016-10-14T11:35:26.623Z",
      "updated_at": "2016-10-14T11:35:26.630Z",
      "shortname": "fu-course-46"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d51a8ed987e12b24826a83cda0e911c9bb9b0a5db93c1505475bcca12fbad383"
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
      "creator_id": 184,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-41",
      "html_url": "https://goskive.com/course/fu-course-41",
      "slug": "fu-course-41",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 70,
      "discipline_id": 70,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 41",
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
      "updated_at": "2016-10-14T11:35:26.084Z",
      "shortname": "fu-course-41"
    },
    {
      "creator_id": 184,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 71,
      "discipline_id": 71,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
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
      "updated_at": "2016-10-14T11:35:26.130Z",
      "shortname": "fu-course-42"
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
Authorization: Bearer f0709135da752cd2bf71b8d9d1b8bce12688fa6ec50e590eb21fe5d7853912c3
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
      "creator_id": 193,
      "id": 68,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-49",
      "html_url": "https://goskive.com/course/fu-course-49",
      "slug": "fu-course-49",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 78,
      "discipline_id": 78,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 49",
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
      "updated_at": "2016-10-14T11:35:26.929Z",
      "shortname": "fu-course-49"
    },
    {
      "creator_id": 193,
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-50",
      "html_url": "https://goskive.com/course/fu-course-50",
      "slug": "fu-course-50",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 79,
      "discipline_id": 79,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 50",
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
      "updated_at": "2016-10-14T11:35:26.973Z",
      "shortname": "fu-course-50"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0709135da752cd2bf71b8d9d1b8bce12688fa6ec50e590eb21fe5d7853912c3"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 33fa7dad68396684a6cb68c5f6aa4d18eb765e8d33b1c7223c1299e4eb768b3c
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
  "id": 832,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-14T11:36:17.152Z",
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
	-H "Authorization: Bearer 33fa7dad68396684a6cb68c5f6aa4d18eb765e8d33b1c7223c1299e4eb768b3c"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/25
Content-Type: application/json
Authorization: Bearer 240ef1992671a7c221b7cbbffc94862aa91dabc0b772b6b14bc8a806790b0280
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
    "id": 25,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 9,
    "fields_of_study": [
      12,
      13
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-14T11:35:08.778Z",
    "updated_at": "2016-10-14T11:35:08.778Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/25" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 240ef1992671a7c221b7cbbffc94862aa91dabc0b772b6b14bc8a806790b0280"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/27
Content-Type: application/json
Authorization: Bearer 5c812b88d4438a0651eaad8af193ec5b2ff18106d05e99222ca4036c2d6ae69e
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
    "id": 27,
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
    "created_at": "2016-10-14T11:35:08.868Z",
    "updated_at": "2016-10-14T11:35:08.868Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c812b88d4438a0651eaad8af193ec5b2ff18106d05e99222ca4036c2d6ae69e"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/1
Content-Type: application/json
Authorization: Bearer c32723597c47eec31b5bf02e5966aad13dec03ce8172bdd2851c00eb5ac9cb40
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
	-H "Authorization: Bearer c32723597c47eec31b5bf02e5966aad13dec03ce8172bdd2851c00eb5ac9cb40"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/2
Content-Type: application/json
Authorization: Bearer 7f8d1ecdf6a163e68e155aa8949879e40812db970728e671e1d4d02b81f39dfb
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
    "votable_id": 3,
    "user_id": 9
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f8d1ecdf6a163e68e155aa8949879e40812db970728e671e1d4d02b81f39dfb"
```
