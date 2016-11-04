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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"af6f5a03d8d788bb9d5cdb5525b539aecbb4583fa92e246ad54396d7285e1f08","client_secret":"5b0db46f37f0287f4d457b57ef611739575c542dae058801873c3557b3a516b0"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"af6f5a03d8d788bb9d5cdb5525b539aecbb4583fa92e246ad54396d7285e1f08","client_secret":"5b0db46f37f0287f4d457b57ef611739575c542dae058801873c3557b3a516b0"}' -X POST \
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
Authorization: Basic YTI5YTFiODUyZjA1MWNjZTNjNzE2MDRjOGMwMWY4MGEzODQ4ZTBhZjViODQ2
MDQ0YTIyMWNiMWVmOTljNzg2NDo0MTMwZjQ3OWVmYTI5YTczMDJlMzRhZjZh
ZWVhNWNjYWU3YzJlN2VmYjZhMzUwODZmMTMwNThhMjY1Zjg1MmVj

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
	-u a29a1b852f051cce3c71604c8c01f80a3848e0af5b846044a221cb1ef99c7864:4130f479efa29a7302e34af6aeea5ccae7c2e7efb6a35086f13058a265f852ec
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"df94e5edaec8dd10faa464831a65c8e213a245e3df17825efa0302532ad1490d","client_secret":"0c7c3e39061b5cd853787f6981e1e71a65668cb525c3550196c54f0c371f509a"}
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
  "access_token": "0ba2d93cbe814ac8c830f1eadc96daaadc5afc5c19f6d2caae7fb4e53337ea8a",
  "token_type": "bearer",
  "created_at": 1478275214
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"df94e5edaec8dd10faa464831a65c8e213a245e3df17825efa0302532ad1490d","client_secret":"0c7c3e39061b5cd853787f6981e1e71a65668cb525c3550196c54f0c371f509a"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZjUxMDA1NzM4YzIzOGU0ZTY4NmVhNDJjYjUwNmU1NTQ0YTE0Y2FiOGE5YTE0
YWQ4MTE4ZmNmYzgxNDhmYTA3ZDpmMGZlYWQyMTNkZGE4MmU3NDU3Yjg1ODc1
OWRhNWFlYzI5NjliNDhjODQ0NTg3NWY0MmFkYWI3NmU1NjFlNWRj

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
  "access_token": "fff5a3c0cf8fd5cb854ee7a9ea69833bc81878dea877e75013f6dcddec06be82",
  "token_type": "bearer",
  "created_at": 1478275214
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u f51005738c238e4e686ea42cb506e5544a14cab8a9a14ad8118fcfc8148fa07d:f0fead213dda82e7457b858759da5aec2969b48c8445875f42adab76e561e5dc
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
{"grant_type":"client_credentials","client_id":"17a4d69bfe93821436110e8e65a4d3de7ae4acb7c3eaac78e9a1c623d0fc3a1f","client_secret":"3bb4e9e70fa55ff7c04c4e6eb8ba79b49590a80896d139362c4f771c39045710"}
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
  "access_token": "0bb26ced170b904d859e6092810a63f5164e4435493c5f2ea8cc93963a05ce8a",
  "token_type": "bearer",
  "created_at": 1478275214
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"17a4d69bfe93821436110e8e65a4d3de7ae4acb7c3eaac78e9a1c623d0fc3a1f","client_secret":"3bb4e9e70fa55ff7c04c4e6eb8ba79b49590a80896d139362c4f771c39045710"}' -X POST \
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
Authorization: Bearer a575f40dd6c7184f078cb6d37e92f33505732bad225e72f2b6c2a9fd87acdf94
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
	-H "Authorization: Bearer a575f40dd6c7184f078cb6d37e92f33505732bad225e72f2b6c2a9fd87acdf94"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/74/flashcards
Content-Type: application/json
Authorization: Bearer 22248bfc7b7cfab611e1d68972eb8b5d8c0b730fbb1e7dd471b8526fb4434843
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":74,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 313,
    "chapter_id": 74,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:30.473Z",
    "created_at": "2016-11-04T16:00:30.473Z",
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
curl "api.goskive.com/v2/chapters/74/flashcards" -d '{"flashcard":{"chapter_id":74,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22248bfc7b7cfab611e1d68972eb8b5d8c0b730fbb1e7dd471b8526fb4434843"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/76/flashcards
Content-Type: application/json
Authorization: Bearer 8f798be4e43ebe3b8ede992446cfa90ed372f4da2a5bf49e0fd5898e70ddb403
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 317,
      "chapter_id": 76,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:30.898Z",
      "created_at": "2016-11-04T16:00:30.898Z",
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
      "author_id": 317,
      "chapter_id": 76,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:30.942Z",
      "created_at": "2016-11-04T16:00:30.942Z",
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
      "author_id": 317,
      "chapter_id": 76,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:30.987Z",
      "created_at": "2016-11-04T16:00:30.987Z",
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
curl "api.goskive.com/v2/chapters/76/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f798be4e43ebe3b8ede992446cfa90ed372f4da2a5bf49e0fd5898e70ddb403"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/112/questions
Content-Type: application/json
Authorization: Bearer b7717c7f27e3fb751e47907e7d18eab1aaedd95e56712b323832c7e0fb6f42f2
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":112,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 69,
    "obfuscated_id": "1EDi_PBgOnI",
    "author_id": 533,
    "chapter_id": 112,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:46.557Z",
    "created_at": "2016-11-04T16:00:46.557Z",
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
        "id": 137,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 138,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 139,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 140,
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
curl "api.goskive.com/v2/chapters/112/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":112,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7717c7f27e3fb751e47907e7d18eab1aaedd95e56712b323832c7e0fb6f42f2"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/113/questions
Content-Type: application/json
Authorization: Bearer 263769fc05126fa621d8aac00f11dfb50cf9852c9e27cc1b13a61f67cd71383c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":113,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 70,
    "obfuscated_id": "EDEz1xzotLc",
    "author_id": 536,
    "chapter_id": 113,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:47.316Z",
    "created_at": "2016-11-04T16:00:47.316Z",
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
        "id": 141,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 142,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/113/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":113,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 263769fc05126fa621d8aac00f11dfb50cf9852c9e27cc1b13a61f67cd71383c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/115/questions
Content-Type: application/json
Authorization: Bearer 1f19af790add02362d7603f1da2a954dbc12bdf376e735d9224189f308acbdc5
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
    "id": 72,
    "obfuscated_id": "oqzxOzwzIgw",
    "author_id": 542,
    "chapter_id": 115,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:48.385Z",
    "created_at": "2016-11-04T16:00:48.385Z",
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
        "id": 146,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 147,
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
	-H "Authorization: Bearer 1f19af790add02362d7603f1da2a954dbc12bdf376e735d9224189f308acbdc5"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/114/questions
Content-Type: application/json
Authorization: Bearer b216de41f2cbfeb3a4e192881494aff25c4e49fa4bd48c5c21deb1511a57743a
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":114,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 71,
    "obfuscated_id": "--JhLc6KEBw",
    "author_id": 539,
    "chapter_id": 114,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:47.855Z",
    "created_at": "2016-11-04T16:00:47.855Z",
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
        "id": 143,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 144,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 145,
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
curl "api.goskive.com/v2/chapters/114/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":114,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b216de41f2cbfeb3a4e192881494aff25c4e49fa4bd48c5c21deb1511a57743a"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/116/questions
Content-Type: application/json
Authorization: Bearer 4897808ae944eff8e5e4975973d5d362c81330d3b30c6177f2ecba03036bab10
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 545,
      "chapter_id": 116,
      "position": 69,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:49.013Z",
      "created_at": "2016-11-04T16:00:48.894Z",
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
          "id": 148,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 149,
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
      "author_id": 546,
      "chapter_id": 116,
      "position": 70,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:49.206Z",
      "created_at": "2016-11-04T16:00:49.084Z",
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
          "id": 150,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 151,
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
      "author_id": 547,
      "chapter_id": 116,
      "position": 71,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:49.398Z",
      "created_at": "2016-11-04T16:00:49.278Z",
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
          "id": 152,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 153,
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
curl "api.goskive.com/v2/chapters/116/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4897808ae944eff8e5e4975973d5d362c81330d3b30c6177f2ecba03036bab10"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/143
Content-Type: application/json
Authorization: Bearer 31ec835fe9de69e05a1aeabf73dbd1e1eec901cbd1bcbee4749cb9b152117add
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
curl "api.goskive.com/v2/chapters/143" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31ec835fe9de69e05a1aeabf73dbd1e1eec901cbd1bcbee4749cb9b152117add"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/144
Content-Type: application/json
Authorization: Bearer 41d256da63b10cc3df29aaf9dfdec847f477c0fc159b8682e81e2144d118d20b
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
curl "api.goskive.com/v2/chapters/144" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41d256da63b10cc3df29aaf9dfdec847f477c0fc159b8682e81e2144d118d20b"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/140
Content-Type: application/json
Authorization: Bearer 4eec7c629dbc3590675d7ffe282e532cc573bc481f49be484a5008241ea082c6
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
curl "api.goskive.com/v2/chapters/140" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eec7c629dbc3590675d7ffe282e532cc573bc481f49be484a5008241ea082c6"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/142
Content-Type: application/json
Authorization: Bearer c2af56d1811fb03c5ee94a82c74f23e820aaecfed5af7204c58a6f43449cfbfb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/142" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2af56d1811fb03c5ee94a82c74f23e820aaecfed5af7204c58a6f43449cfbfb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/147
Content-Type: application/json
Authorization: Bearer 84c757d78041a98435d093ec34eef510a9bcf984b83ca1ab847245982d61d265
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
    "id": 147,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-04T16:01:07.326Z",
    "course_id": 268,
    "author_id": 799,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-04T16:01:06.790Z",
    "questions_updated_at": "2016-11-04T16:01:06.790Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 803,
        "chapter_id": 147,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:07.308Z",
        "created_at": "2016-11-04T16:01:07.308Z",
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
        "id": 99,
        "obfuscated_id": "5fPQ9k37GTc",
        "author_id": 801,
        "chapter_id": 147,
        "position": 95,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:07.203Z",
        "created_at": "2016-11-04T16:01:07.082Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/147" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84c757d78041a98435d093ec34eef510a9bcf984b83ca1ab847245982d61d265"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/141
Content-Type: application/json
Authorization: Bearer 699203d6c459e7c677a6b4a619022e9fba2cf3dd1cf91e257042c072445f767b
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
    "id": 141,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-04T16:01:05.165Z",
    "course_id": 262,
    "author_id": 778,
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
curl "api.goskive.com/v2/chapters/141" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 699203d6c459e7c677a6b4a619022e9fba2cf3dd1cf91e257042c072445f767b"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/57/replies
Content-Type: application/json
Authorization: Bearer 2633d77e4893768c4e02041328f549b857b41d5788c97c044f7054cd2a9d95f8
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
    "author_id": 868,
    "reply_to_id": 57,
    "created_at": "2016-11-04T16:01:14.052Z",
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
	-H "Authorization: Bearer 2633d77e4893768c4e02041328f549b857b41d5788c97c044f7054cd2a9d95f8"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/56/replies
Content-Type: application/json
Authorization: Bearer e5af220f3c5b76ea81c4a76814ef6b36c81680e27d6ea2fa726bf34948a78c30
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
	-H "Authorization: Bearer e5af220f3c5b76ea81c4a76814ef6b36c81680e27d6ea2fa726bf34948a78c30"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/7
Content-Type: application/json
Authorization: Bearer 4bda77ccdeb8c7d0bb20827f29c8c9e8521cf5ab44596f9c83df396dbe03f093
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
	-H "Authorization: Bearer 4bda77ccdeb8c7d0bb20827f29c8c9e8521cf5ab44596f9c83df396dbe03f093"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/11/republish
Content-Type: application/json
Authorization: Bearer ca8bacc701ecbd076ffc44723804d5e0fad81a3bd85b0ee516fb4be70d3c4837
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
curl "api.goskive.com/v2/comments/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca8bacc701ecbd076ffc44723804d5e0fad81a3bd85b0ee516fb4be70d3c4837"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 44a7446d2d1b8def23bfa2b90975af40637570c102132ea05d9a881cf03bc0f2
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44a7446d2d1b8def23bfa2b90975af40637570c102132ea05d9a881cf03bc0f2"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/9/report
Content-Type: application/json
Authorization: Bearer 786086bac2e7db9626fca7536ea19e4b73a6223c8f76b9e2d3eebc1a7536d9f9
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/9/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 786086bac2e7db9626fca7536ea19e4b73a6223c8f76b9e2d3eebc1a7536d9f9"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/28
Content-Type: application/json
Authorization: Bearer fdbeecb1f7a08f6a0d1a802f89fe4981001b6728746f87ae9bffe2eb4afba83d
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
    "id": 28,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/30c5a74ecbb9237f9b94758b5bdae7ab7ea1f7b4.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-04T16:00:45.588Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdbeecb1f7a08f6a0d1a802f89fe4981001b6728746f87ae9bffe2eb4afba83d"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer d7588024f9a3fa99b4e92afb086a384c4b326dae42f343021d4dfea84451895c
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
      "id": 25,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-04T16:00:45.527Z"
    },
    {
      "id": 26,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-04T16:00:45.531Z"
    },
    {
      "id": 27,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-04T16:00:45.535Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7588024f9a3fa99b4e92afb086a384c4b326dae42f343021d4dfea84451895c"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/38/company_profiles
Content-Type: application/json
Authorization: Bearer fae00255f103d273383b13331d5de61429a07f1bcc1fd0d4f2673c4da387821d
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
curl "api.goskive.com/v2/companies/38/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fae00255f103d273383b13331d5de61429a07f1bcc1fd0d4f2673c4da387821d"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 180b7f7ace7798f351a5382560d78f13d1c44965b87c316e71502fa7a00c7c05
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
	-H "Authorization: Bearer 180b7f7ace7798f351a5382560d78f13d1c44965b87c316e71502fa7a00c7c05"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 5cbc8a7a1481634f4358107f34e31221a8d291a039fa9c223709f56b87b63651
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
      "id": 2,
      "title": "Campaign 1",
      "company_id": 5,
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
      "id": 5,
      "title": "Campaign 4",
      "company_id": 8,
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
	-H "Authorization: Bearer 5cbc8a7a1481634f4358107f34e31221a8d291a039fa9c223709f56b87b63651"
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
Authorization: Bearer 7706aeb69b3e1a093816f27cb2d7f8fdd9b52150bbf2f42d12b8ac970e2b234b
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
	-H "Authorization: Bearer 7706aeb69b3e1a093816f27cb2d7f8fdd9b52150bbf2f42d12b8ac970e2b234b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 68c6551559c666cdca630e999a948e460d79dfefb66e860c51d1ee09a9bac3ca
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
    "id": 22,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-04T16:00:04.810Z",
    "course_id": 13,
    "author_id": 50,
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
	-H "Authorization: Bearer 68c6551559c666cdca630e999a948e460d79dfefb66e860c51d1ee09a9bac3ca"
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
      "id": 7,
      "title": "Clever Chapter Title 7",
      "position": 1,
      "updated_at": "2016-11-04T16:00:03.005Z",
      "course_id": 4,
      "author_id": 16,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 8,
      "title": "Clever Chapter Title 8",
      "position": 2,
      "updated_at": "2016-11-04T16:00:03.029Z",
      "course_id": 4,
      "author_id": 17,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 9,
      "title": "Clever Chapter Title 9",
      "position": 3,
      "updated_at": "2016-11-04T16:00:03.279Z",
      "course_id": 4,
      "author_id": 18,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-04T16:00:02.932Z",
      "questions_updated_at": "2016-11-04T16:00:02.932Z",
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
Authorization: Bearer 78525fae2cdb988d13ebde788969c47491abce355bc4ba1929d2d26b4e9a62b5
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
      "id": 13,
      "title": "Clever Chapter Title 13",
      "position": 1,
      "updated_at": "2016-11-04T16:00:03.622Z",
      "course_id": 7,
      "author_id": 27,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 14,
      "title": "Clever Chapter Title 14",
      "position": 2,
      "updated_at": "2016-11-04T16:00:03.645Z",
      "course_id": 7,
      "author_id": 28,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 15,
      "title": "Clever Chapter Title 15",
      "position": 3,
      "updated_at": "2016-11-04T16:00:03.895Z",
      "course_id": 7,
      "author_id": 29,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-04T16:00:03.551Z",
      "questions_updated_at": "2016-11-04T16:00:03.551Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78525fae2cdb988d13ebde788969c47491abce355bc4ba1929d2d26b4e9a62b5"
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
      "id": 10,
      "title": "Clever Chapter Title 10",
      "position": 1,
      "updated_at": "2016-11-04T16:00:03.467Z",
      "course_id": 6,
      "author_id": 23,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 11,
      "title": "Clever Chapter Title 11",
      "position": 2,
      "updated_at": "2016-11-04T16:00:03.490Z",
      "course_id": 6,
      "author_id": 24,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 12,
      "title": "Clever Chapter Title 12",
      "position": 3,
      "updated_at": "2016-11-04T16:00:03.512Z",
      "course_id": 6,
      "author_id": 25,
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
Authorization: Bearer cce31e7dd39021074f1ca88790e091a25a52c517e28cb2f65a5023e7fd64b833
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
      "id": 16,
      "title": "Clever Chapter Title 16",
      "position": 1,
      "updated_at": "2016-11-04T16:00:04.056Z",
      "course_id": 8,
      "author_id": 34,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 17,
      "title": "Clever Chapter Title 17",
      "position": 2,
      "updated_at": "2016-11-04T16:00:04.079Z",
      "course_id": 8,
      "author_id": 35,
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
      "position": 3,
      "updated_at": "2016-11-04T16:00:04.102Z",
      "course_id": 8,
      "author_id": 36,
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
	-H "Authorization: Bearer cce31e7dd39021074f1ca88790e091a25a52c517e28cb2f65a5023e7fd64b833"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 3e074f91485e560dc5813b3e8608a8f1088a746133ce94eb0d8b9c421a1e5790
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
    "course_id": 49,
    "user_id": 196,
    "updated_at": "2016-11-04T16:00:14.603Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e074f91485e560dc5813b3e8608a8f1088a746133ce94eb0d8b9c421a1e5790"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer c6faf873f1f954db4d8d1093f9793ba4c29920488a992ae205f2236e7eff1193
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
      "course_id": 47,
      "user_id": 190,
      "updated_at": "2016-11-04T16:00:14.305Z"
    },
    {
      "id": 4,
      "course_id": 47,
      "user_id": 191,
      "updated_at": "2016-11-04T16:00:14.320Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6faf873f1f954db4d8d1093f9793ba4c29920488a992ae205f2236e7eff1193"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/119/files
Content-Type: application/json
Authorization: Bearer cf2bd9fa1330db77348619b8ff080f3abdcc882efc966e1da932a755345ec271
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
      "id": 20,
      "uploader": {
        "id": 416,
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
        "created_at": "2016-11-04T16:00:38.966Z",
        "updated_at": "2016-11-04T16:00:38.966Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-04T16:00:38.977Z",
      "updated_at": "2016-11-04T16:00:38.977Z",
      "course_id": 119,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 21,
      "uploader": {
        "id": 417,
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
        "created_at": "2016-11-04T16:00:38.984Z",
        "updated_at": "2016-11-04T16:00:38.984Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-04T16:00:38.994Z",
      "updated_at": "2016-11-04T16:00:38.994Z",
      "course_id": 119,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 22,
      "uploader": {
        "id": 418,
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
        "created_at": "2016-11-04T16:00:39.001Z",
        "updated_at": "2016-11-04T16:00:39.001Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-04T16:00:39.011Z",
      "updated_at": "2016-11-04T16:00:39.011Z",
      "course_id": 119,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/119/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf2bd9fa1330db77348619b8ff080f3abdcc882efc966e1da932a755345ec271"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/118/files
Content-Type: application/json
Authorization: Bearer b8b1a24b378ab0ddc9d152bca0b416e68cbff6993fb68bee949f2cdbc606aeb1
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
    "id": 19,
    "uploader": {
      "id": 414,
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
      "created_at": "2016-11-04T16:00:38.801Z",
      "updated_at": "2016-11-04T16:00:38.801Z"
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
    "created_at": "2016-11-04T16:00:38.835Z",
    "updated_at": "2016-11-04T16:00:38.835Z",
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
	-H "Authorization: Bearer b8b1a24b378ab0ddc9d152bca0b416e68cbff6993fb68bee949f2cdbc606aeb1"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/117/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer b22bc93e3eba1672c2ee0c0813fd88f9db3af2b8c3c3602fead25aa65a4e9ae4
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
    "key": "cache/b43e08eb43de81cf2ec0a63db4da3f51.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wNFQxNzowMDozOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2I0M2UwOGViNDNkZTgxY2YyZWMwYTYzZGI0ZGEzZjUxLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDQvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTA0VDE2MDAzOFoifV19",
    "x-amz-credential": "FAKE/20161104/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161104T160038Z",
    "x-amz-signature": "25c69b8e85a4a728e288e5d55a8d8968e31a72198b7dc05c38efbae4c5c8c905"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/117/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b22bc93e3eba1672c2ee0c0813fd88f9db3af2b8c3c3602fead25aa65a4e9ae4"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer bf16df2229fd546a7b5952c320237f9397b122b20ef498393ca55f106497506a
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
	-H "Authorization: Bearer bf16df2229fd546a7b5952c320237f9397b122b20ef498393ca55f106497506a"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d969898ab2d51a9262f198c133efd9c28d466490656a1b0081d751c046b2a6a0
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
	-H "Authorization: Bearer d969898ab2d51a9262f198c133efd9c28d466490656a1b0081d751c046b2a6a0"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8c5e1ed3520da154198070e49ac7519dee9fb0f12ef8bd1ed8338379af958ab4
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
	-H "Authorization: Bearer 8c5e1ed3520da154198070e49ac7519dee9fb0f12ef8bd1ed8338379af958ab4"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b8fd81b12a71b95d553f91ce40c29afd94abe8fcb350dd076c3143c08c4bb96e
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
	-H "Authorization: Bearer b8fd81b12a71b95d553f91ce40c29afd94abe8fcb350dd076c3143c08c4bb96e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6f6c74f98385ab9036966668953326e0619736c9dd806dadd898a017f35ffc25
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
	-H "Authorization: Bearer 6f6c74f98385ab9036966668953326e0619736c9dd806dadd898a017f35ffc25"
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
    "creator_id": 277,
    "id": 73,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 73,
    "additional_university_ids": [

    ],
    "topic_id": 73,
    "discipline_id": 73,
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
    "chapters_updated_at": "2016-11-04T16:00:22.241Z",
    "updated_at": "2016-11-04T16:00:23.925Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 66,
        "title": "Clever Chapter Title 63",
        "position": 1,
        "updated_at": "2016-11-04T16:00:23.874Z",
        "course_id": 73,
        "author_id": 277,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-04T16:00:22.241Z",
        "questions_updated_at": "2016-11-04T16:00:22.241Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 67,
        "title": "Clever Chapter Title 64",
        "position": 2,
        "updated_at": "2016-11-04T16:00:23.916Z",
        "course_id": 73,
        "author_id": 277,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-04T16:00:22.241Z",
        "questions_updated_at": "2016-11-04T16:00:22.241Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 277,
        "chapter_id": 66,
        "position": 37,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:22.474Z",
        "created_at": "2016-11-04T16:00:22.331Z",
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
            "id": 73,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 74,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 277,
        "chapter_id": 67,
        "position": 39,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:22.934Z",
        "created_at": "2016-11-04T16:00:22.784Z",
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
            "id": 77,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 78,
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
Authorization: Bearer 45039d457f47ce1bb6555a1cde947da0c1b65eb5428fa600b979e0c591640436
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
    "creator_id": 282,
    "id": 74,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 74,
    "additional_university_ids": [

    ],
    "topic_id": 74,
    "discipline_id": 74,
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
    "chapters_updated_at": "2016-11-04T16:00:23.988Z",
    "updated_at": "2016-11-04T16:00:25.733Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 68,
        "title": "Clever Chapter Title 65",
        "position": 1,
        "updated_at": "2016-11-04T16:00:25.681Z",
        "course_id": 74,
        "author_id": 282,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-04T16:00:23.988Z",
        "questions_updated_at": "2016-11-04T16:00:23.988Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 69,
        "title": "Clever Chapter Title 66",
        "position": 2,
        "updated_at": "2016-11-04T16:00:25.724Z",
        "course_id": 74,
        "author_id": 282,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-04T16:00:23.988Z",
        "questions_updated_at": "2016-11-04T16:00:23.988Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 283,
        "chapter_id": 68,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:25.497Z",
        "created_at": "2016-11-04T16:00:25.497Z",
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
        "author_id": 283,
        "chapter_id": 69,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:25.579Z",
        "created_at": "2016-11-04T16:00:25.579Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 283,
        "chapter_id": 68,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:25.545Z",
        "created_at": "2016-11-04T16:00:25.545Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 283,
        "chapter_id": 69,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:25.626Z",
        "created_at": "2016-11-04T16:00:25.626Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 283,
        "chapter_id": 68,
        "position": 43,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:24.241Z",
        "created_at": "2016-11-04T16:00:24.093Z",
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
            "id": 85,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 86,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 283,
        "chapter_id": 68,
        "position": 44,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:24.458Z",
        "created_at": "2016-11-04T16:00:24.318Z",
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
            "id": 87,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 88,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 283,
        "chapter_id": 69,
        "position": 45,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:24.711Z",
        "created_at": "2016-11-04T16:00:24.556Z",
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
            "id": 89,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 90,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 283,
        "chapter_id": 69,
        "position": 46,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:24.936Z",
        "created_at": "2016-11-04T16:00:24.791Z",
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
            "id": 91,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 92,
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
	-H "Authorization: Bearer 45039d457f47ce1bb6555a1cde947da0c1b65eb5428fa600b979e0c591640436"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/82/pin
Content-Type: application/json
Authorization: Bearer 53b3c460d0d578d71bcc2c09db0f945373d01ce1bf55b0593bcb0840d522ee00
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/82/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53b3c460d0d578d71bcc2c09db0f945373d01ce1bf55b0593bcb0840d522ee00"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/81/pin
Content-Type: application/json
Authorization: Bearer dcb5d4d7162344955b5320eb2af608fb01d43abcf3ae3fa21e85127761aa9a0e
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/81/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcb5d4d7162344955b5320eb2af608fb01d43abcf3ae3fa21e85127761aa9a0e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d7a110b0d7b37ec818e75400ebaaee2772349926902ce8e9d04c239a599cfee3
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
    "creator_id": 302,
    "id": 78,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 78,
    "additional_university_ids": [

    ],
    "topic_id": 78,
    "discipline_id": 78,
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
    "updated_at": "2016-11-04T16:00:29.832Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7a110b0d7b37ec818e75400ebaaee2772349926902ce8e9d04c239a599cfee3"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer be3c148bf17f5b42317e7047648ac8c8ec20084ff610b84a8c37aa4c4a247b4b
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
    "id": 683,
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
    "created_at": "2016-11-04T16:00:56.809Z",
    "updated_at": "2016-11-04T16:00:56.809Z",
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
	-H "Authorization: Bearer be3c148bf17f5b42317e7047648ac8c8ec20084ff610b84a8c37aa4c4a247b4b"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9822d4747f31d6e2ba9bb7b47b9d70c1513b1c927ef03fb40e471fb8c17385b5
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[217]}
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
    "id": 678,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      217
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-04T16:00:56.183Z",
    "updated_at": "2016-11-04T16:00:56.235Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[217]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9822d4747f31d6e2ba9bb7b47b9d70c1513b1c927ef03fb40e471fb8c17385b5"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 828cbfa1da147b346f54b563adbfccb9630793eb58a396cd0e0485335ceb7e18
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
    "id": 680,
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
    "created_at": "2016-11-04T16:00:56.346Z",
    "updated_at": "2016-11-04T16:00:56.346Z",
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
	-H "Authorization: Bearer 828cbfa1da147b346f54b563adbfccb9630793eb58a396cd0e0485335ceb7e18"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8d1dc371aead924ad835e7ab1f7ccc47407ef85fcf33422a2abf9e67f2561118
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[220]}
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
    "id": 681,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      220
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-04T16:00:56.445Z",
    "updated_at": "2016-11-04T16:00:56.445Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[220]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d1dc371aead924ad835e7ab1f7ccc47407ef85fcf33422a2abf9e67f2561118"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer a60f07811d4a8c422680b35380fd2c087895c233b764665a879b6a24ecfee1eb
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

221
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
    "id": 682,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/aa7e7214dfb51481c8cb3045abfcd503c92d5ff1.jpg",
    "university_id": null,
    "fields_of_study": [
      221
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-04T16:00:56.524Z",
    "updated_at": "2016-11-04T16:00:56.778Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/d078a39f38522bb3119ce76236fb2de06dc73a14.jpg",
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

221
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer a60f07811d4a8c422680b35380fd2c087895c233b764665a879b6a24ecfee1eb"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 1ee49ff02acd2a2ea35656f2aa3340f7b2d846eab60b4184075c875a857c61e4
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
      "bookmarkable_id": 104,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 105,
      "bookmarkable_type": "Question"
    },
    {
      "id": 8,
      "bookmarkable_id": 106,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee49ff02acd2a2ea35656f2aa3340f7b2d846eab60b4184075c875a857c61e4"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer f569419001c6f22f9e464e7adcbd51182a12275b707cbea0e7bfe58372782ceb
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
      "company_id": 21,
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
      "company_id": 22,
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
	-H "Authorization: Bearer f569419001c6f22f9e464e7adcbd51182a12275b707cbea0e7bfe58372782ceb"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 2147b9c5d1e5e106f142cc20d437fb6e96f205f6e5eb8f8c70d2c01d3a92b4f8
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
      "company_id": 17,
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
	-H "Authorization: Bearer 2147b9c5d1e5e106f142cc20d437fb6e96f205f6e5eb8f8c70d2c01d3a92b4f8"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d81aedf1b087ba46811285db7b8df022d29885dabfe4e7198d55e0cdc95936d2
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
      "creator_id": 235,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-30",
      "html_url": "https://goskive.com/course/mit-course-30",
      "slug": "mit-course-30",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 57,
      "discipline_id": 57,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 30",
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
      "updated_at": "2016-11-04T16:00:18.276Z",
      "shortname": "mit-course-30"
    },
    {
      "creator_id": 236,
      "id": 58,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-31",
      "html_url": "https://goskive.com/course/mit-course-31",
      "slug": "mit-course-31",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 58,
      "discipline_id": 58,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 31",
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
      "updated_at": "2016-11-04T16:00:18.354Z",
      "shortname": "mit-course-31"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d81aedf1b087ba46811285db7b8df022d29885dabfe4e7198d55e0cdc95936d2"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 2c1a907ba6419e519db8539e1bee9409895c2b2c3e11cc2cf67bf31999e3cd01
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
        "id": 16,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-11-04T16:00:35.264Z",
        "updated_at": "2016-11-04T16:00:35.264Z",
        "file_url": "memory://b5ef2c1c5585b32c79f982e29b8d8859.pdf",
        "course_id": 103,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 17,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-04T16:00:35.344Z",
        "updated_at": "2016-11-04T16:00:35.344Z",
        "file_url": "memory://4d8919735513525955011029a1d33658.pdf",
        "course_id": 104,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 18,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-11-04T16:00:35.425Z",
        "updated_at": "2016-11-04T16:00:35.425Z",
        "file_url": "memory://fab3474bec38998f471dc414d7a499a7.pdf",
        "course_id": 105,
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
	-H "Authorization: Bearer 2c1a907ba6419e519db8539e1bee9409895c2b2c3e11cc2cf67bf31999e3cd01"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer b6650a36f6cb87d45fac3fb33b4f6e244e205f1fc70b620b29f1410767a6b1f6
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
      "company_id": 34,
      "company": {
        "id": 34,
        "name": "Fake Company Name 32",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-04T16:00:57.031Z"
      },
      "created_at": "2016-11-04T16:00:57.034Z",
      "updated_at": "2016-11-04T16:00:57.034Z",
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
      "company_id": 35,
      "company": {
        "id": 35,
        "name": "Fake Company Name 33",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1608ebf234004cae8ed6c8e58a82be15d51242a1.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-04T16:00:57.041Z"
      },
      "created_at": "2016-11-04T16:00:57.044Z",
      "updated_at": "2016-11-04T16:00:57.044Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6650a36f6cb87d45fac3fb33b4f6e244e205f1fc70b620b29f1410767a6b1f6"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer df7fe9c6ecaf8600ad3d4e7ea074bceca0b0bf14df77c9d92ac23dd56f5bd975
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
      "company_id": 30,
      "company": {
        "id": 30,
        "name": "Fake Company Name 28",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a07e019e4ade49e0df967a2132297276f32d30ed.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-04T16:00:56.867Z"
      },
      "created_at": "2016-11-04T16:00:56.870Z",
      "updated_at": "2016-11-04T16:00:56.870Z",
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
      "company_id": 31,
      "company": {
        "id": 31,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/0df235007210ab1331461f6a10296cd43f327e64.png",
        "brand_color": "#000000",
        "updated_at": "2016-11-04T16:00:56.885Z"
      },
      "created_at": "2016-11-04T16:00:56.888Z",
      "updated_at": "2016-11-04T16:00:56.888Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df7fe9c6ecaf8600ad3d4e7ea074bceca0b0bf14df77c9d92ac23dd56f5bd975"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 23b0f32a75d91b4d1721a3674026bbede724f8668671ee34eefff3272606e7a0
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
      "id": 10,
      "created_at": "2016-11-04T16:00:54.017Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 48,
      "updated_at": "2016-11-04T16:00:54.123Z",
      "author_id": "652",
      "thread_subject_id": "204",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 11,
      "created_at": "2016-11-04T16:00:54.112Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 49,
      "updated_at": "2016-11-04T16:00:54.126Z",
      "author_id": "655",
      "thread_subject_id": "205",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 12,
      "created_at": "2016-11-04T16:00:54.488Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-11-04T16:00:54.488Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 13,
      "created_at": "2016-11-04T16:00:54.861Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-11-04T16:00:54.861Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 14,
      "created_at": "2016-11-04T16:00:55.237Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-04T16:00:55.237Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 15,
      "created_at": "2016-11-04T16:00:55.530Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 79,
      "updated_at": "2016-11-04T16:00:55.530Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 16,
      "created_at": "2016-11-04T16:00:55.824Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 80,
      "updated_at": "2016-11-04T16:00:55.824Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 17,
      "created_at": "2016-11-04T16:00:56.115Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 81,
      "updated_at": "2016-11-04T16:00:56.115Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23b0f32a75d91b4d1721a3674026bbede724f8668671ee34eefff3272606e7a0"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/9
Content-Type: application/json
Authorization: Bearer 3a8283f356eb1360188c6121389c22d41d8505bc85204eafce850acdfad20358
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-04T15:50:53.000Z"}}
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
    "id": 9,
    "created_at": "2016-11-04T16:00:53.814Z",
    "read_at": "2016-11-04T15:50:53.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 47,
    "updated_at": "2016-11-04T16:00:53.870Z",
    "author_id": "647",
    "thread_subject_id": "203",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/9" -d '{"notification":{"read_at":"2016-11-04T15:50:53.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a8283f356eb1360188c6121389c22d41d8505bc85204eafce850acdfad20358"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 6c493b2a0bf9d9f3878ebd34827596a14eadac211a9ecef6d9f1b2c2ada410b5
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
      "id": 6,
      "course_id": 153,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-04T16:00:46.135Z",
      "course_published": true,
      "updated_at": "2016-11-04T16:00:46.128Z"
    },
    {
      "id": 7,
      "course_id": 154,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-04T16:00:46.217Z",
      "course_published": true,
      "updated_at": "2016-11-04T16:00:46.209Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c493b2a0bf9d9f3878ebd34827596a14eadac211a9ecef6d9f1b2c2ada410b5"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer b3285d435da8f056596deaea91bd37c6f4d904914eeb288264b957c7c7e8ec07
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
    "course_id": 150,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-04T16:00:45.726Z",
    "course_published": true,
    "updated_at": "2016-11-04T16:00:45.717Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3285d435da8f056596deaea91bd37c6f4d904914eeb288264b957c7c7e8ec07"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer 2d6fa8f395283e7ecd9ec86284cd300a4e9e84157b8210a55a7b47f9c2aa2eb5
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
    "id": 8,
    "course_id": 155,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-04T16:00:46.377Z",
    "course_published": true,
    "updated_at": "2016-11-04T16:00:46.366Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d6fa8f395283e7ecd9ec86284cd300a4e9e84157b8210a55a7b47f9c2aa2eb5"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer f7740304f43f1c61d0f75104cc7b6aacebb075ac92f0a4d1c7a1ad22a7607359
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
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 100,
      "user_id": 827
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 101,
      "user_id": 827
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 102,
      "user_id": 827
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 827
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7740304f43f1c61d0f75104cc7b6aacebb075ac92f0a4d1c7a1ad22a7607359"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/293
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
    "id": 293,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 291,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 293
      },
      {
        "id": 292,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 293
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/293" -X GET \
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
      "id": 291,
      "name": "Multi-channelled coherent contingency",
      "name_translations": {
        "en": "Multi-channelled coherent contingency"
      }
    },
    {
      "id": 292,
      "name": "Extended client-driven software",
      "name_translations": {
        "en": "Extended client-driven software"
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
PATCH /v2/feedbacks/26/close
Content-Type: application/json
Authorization: Bearer a95ec9203a12a1d703efc568ba1d0815750b2fb4a536fa7c4c55b74cfb328935
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
    "id": 26,
    "user_id": 171,
    "feedbackable_id": 10,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-04T16:00:13.262Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a95ec9203a12a1d703efc568ba1d0815750b2fb4a536fa7c4c55b74cfb328935"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer b8752d105d8bf60e24aa58bced50344174dcbed457ea1930c53f8ad24d39066d
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
    "id": 4,
    "user_id": 73,
    "feedbackable_id": 7,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-04T16:00:06.496Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/4/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8752d105d8bf60e24aa58bced50344174dcbed457ea1930c53f8ad24d39066d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer 44a394917d2f799ebecba007bfd8885f35655ac54501118d17b36bcefc9c567c
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
    "user_id": 78,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-04T16:00:06.834Z",
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
curl "api.goskive.com/v2/feedbacks/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44a394917d2f799ebecba007bfd8885f35655ac54501118d17b36bcefc9c567c"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/fix
Content-Type: application/json
Authorization: Bearer 63beb6e811e6dada8315f18d796f5c115e90e1bfb41600d64a467874e72c4bf4
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
curl "api.goskive.com/v2/feedbacks/1/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63beb6e811e6dada8315f18d796f5c115e90e1bfb41600d64a467874e72c4bf4"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/2/fix
Content-Type: application/json
Authorization: Bearer d52a026e78c6fc62f60cac48c0e7fee43e649471800b12d28a3cb7241f73f5ad
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
curl "api.goskive.com/v2/feedbacks/2/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d52a026e78c6fc62f60cac48c0e7fee43e649471800b12d28a3cb7241f73f5ad"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/close
Content-Type: application/json
Authorization: Bearer a9f33ae48d21a270971c8347ffaa2975df36da634239afe6d64c4610a1a4c25d
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
curl "api.goskive.com/v2/feedbacks/28/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9f33ae48d21a270971c8347ffaa2975df36da634239afe6d64c4610a1a4c25d"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/6
Content-Type: application/json
Authorization: Bearer cf4ac44875ad08155d8654b201ff2057408b0552e4d04a68b7b567c992d3a240
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
    "id": 6,
    "user_id": 83,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-04T16:00:07.144Z",
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
curl "api.goskive.com/v2/feedbacks/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf4ac44875ad08155d8654b201ff2057408b0552e4d04a68b7b567c992d3a240"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 505230c2704cca64513884efca9590266af1f4fe7a3d9f984795f946ad3df36e
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 505230c2704cca64513884efca9590266af1f4fe7a3d9f984795f946ad3df36e"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/7/bookmark
Content-Type: application/json
Authorization: Bearer 390cfd1c1432f286e85825f7a862f15d5bf0c099f855946bef008709d121aced
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 390cfd1c1432f286e85825f7a862f15d5bf0c099f855946bef008709d121aced"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer ca98d35d01b463cfbfbda249f331f21691f5c850d513cc3e2fe9533f2f96401b
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
	-H "Authorization: Bearer ca98d35d01b463cfbfbda249f331f21691f5c850d513cc3e2fe9533f2f96401b"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/5
Content-Type: application/json
Authorization: Bearer 9c9cf57b6c38c9a9955f1ace1bf9dfbe455649ba57b4d6f91e2e83abeb6092ee
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/233f307e07ccae6b576f660a914cac94.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161104%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161104T160033Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=8b74886d54939caee6f9dea90c3131fcd53ede9d25024b0e70c657e01be864df",
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
	-H "Authorization: Bearer 9c9cf57b6c38c9a9955f1ace1bf9dfbe455649ba57b4d6f91e2e83abeb6092ee"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/4/preview
Content-Type: application/json
Authorization: Bearer fc740539f21885ecdb1ba17f7b3688f11dca788f584221e6f8aceeb7190abab6
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/cebfd663ed171789fdd632a4077c079c.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161104%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161104T160033Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=2da6875e624264622c3b06abd8db1e2fcb30f4844474504ad07184a9fb7fe6ad",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/4/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc740539f21885ecdb1ba17f7b3688f11dca788f584221e6f8aceeb7190abab6"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer fcb500f3035770ae569344ab6d6f54d607fba8c9737456cdfa6c4ab87fec11d4
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
    "id": 13,
    "uploader": {
      "id": 366,
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
      "created_at": "2016-11-04T16:00:34.804Z",
      "updated_at": "2016-11-04T16:00:34.804Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-04T16:00:34.880Z",
    "updated_at": "2016-11-04T16:00:34.880Z",
    "course_id": 100,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcb500f3035770ae569344ab6d6f54d607fba8c9737456cdfa6c4ab87fec11d4"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer 77a39d8f91f379ef961adc74e6dd87271d1d5873eed0e1972f35f8e7da9fae9d
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
      "creator_id": 218,
      "id": 54,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 54,
      "discipline_id": 54,
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
      "chapters_updated_at": "2016-11-04T16:00:15.133Z",
      "updated_at": "2016-11-04T16:00:16.850Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 223,
      "id": 55,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-86ab8c4a-89d6-4ada-9bdd-06f6df51403d",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-86ab8c4a-89d6-4ada-9bdd-06f6df51403d",
      "slug": "mit-the-great-british-bake-off-86ab8c4a-89d6-4ada-9bdd-06f6df51403d",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 55,
      "discipline_id": 55,
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
      "chapters_updated_at": "2016-11-04T16:00:15.133Z",
      "updated_at": "2016-11-04T16:00:17.457Z",
      "shortname": "mit-the-great-british-bake-off-86ab8c4a-89d6-4ada-9bdd-06f6df51403d"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 77a39d8f91f379ef961adc74e6dd87271d1d5873eed0e1972f35f8e7da9fae9d"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/11/download
Content-Type: application/json
Authorization: Bearer 5d39992d4c8520f46de3a4923637878797d73cd932032301b6852a719d57204b
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d39992d4c8520f46de3a4923637878797d73cd932032301b6852a719d57204b"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/3/report
Content-Type: application/json
Authorization: Bearer 5fd70c36b6f23bf39d1e57e2b347990644210a21fc3959618ad8ad0ec6a4eb21
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/3/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fd70c36b6f23bf39d1e57e2b347990644210a21fc3959618ad8ad0ec6a4eb21"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/15/bookmark
Content-Type: application/json
Authorization: Bearer 5ecbfddee37345bf0fb97e22458d69e7c0ac298d6bd17ddd3102cd2cbb08cdba
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
	-H "Authorization: Bearer 5ecbfddee37345bf0fb97e22458d69e7c0ac298d6bd17ddd3102cd2cbb08cdba"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/6/upvote
Content-Type: application/json
Authorization: Bearer ff3c53acdea5a6aaab63bbd3f945d2a1b8efd68d83d84bc1a8f59b33d79e5ae4
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff3c53acdea5a6aaab63bbd3f945d2a1b8efd68d83d84bc1a8f59b33d79e5ae4"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/87/comments
Content-Type: application/json
Authorization: Bearer 154fd3b6c9121af04c87715d95f5fb5f20b169d0af52c2e96a392049f4095275
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
    "author_id": 823,
    "reply_to_id": null,
    "created_at": "2016-11-04T16:01:08.783Z",
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
curl "api.goskive.com/v2/flashcards/87/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 154fd3b6c9121af04c87715d95f5fb5f20b169d0af52c2e96a392049f4095275"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/comments
Content-Type: application/json
Authorization: Bearer 6a3f6604b8d9df09b3499a948dd090c11d3eb5e7a791ce9dd807686970a6f549
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
    "author_id": 817,
    "reply_to_id": null,
    "created_at": "2016-11-04T16:01:08.213Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 817,
      "feedbackable_id": 85,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:01:08.210Z",
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
curl "api.goskive.com/v2/flashcards/85/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a3f6604b8d9df09b3499a948dd090c11d3eb5e7a791ce9dd807686970a6f549"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/84/comments
Content-Type: application/json
Authorization: Bearer a88f0a257f6914984544429d1b99cde42eaf1fc06244c103eab7a709f743ce74
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
      "author_id": 816,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:01:08.000Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 52,
      "author_id": 815,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:01:07.983Z",
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
curl "api.goskive.com/v2/flashcards/84/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a88f0a257f6914984544429d1b99cde42eaf1fc06244c103eab7a709f743ce74"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/86/comments
Content-Type: application/json
Authorization: Bearer a0d5d252e95ca75e9458a08216d0ae14c663b95e3c62e4ad4116bdde672a9374
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
curl "api.goskive.com/v2/flashcards/86/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0d5d252e95ca75e9458a08216d0ae14c663b95e3c62e4ad4116bdde672a9374"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/89/feedbacks
Content-Type: application/json
Authorization: Bearer 4a05f6a77ca5fe30033d55e80d66572a44f7282689366497952938de0f46e0c5
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
    "user_id": 952,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-04T16:01:23.331Z",
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
curl "api.goskive.com/v2/flashcards/89/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a05f6a77ca5fe30033d55e80d66572a44f7282689366497952938de0f46e0c5"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/94/feedbacks
Content-Type: application/json
Authorization: Bearer 996b6e08cb9d8c9f60857fb97b0faf9496e66d48586977f23606f1e5a800727c
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
      "id": 46,
      "user_id": 981,
      "feedbackable_id": 94,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:01:24.448Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 980,
      "feedbackable_id": 94,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:01:24.437Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/94/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 996b6e08cb9d8c9f60857fb97b0faf9496e66d48586977f23606f1e5a800727c"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/50/votes
Content-Type: application/json
Authorization: Bearer bfbc88c69f61c6d0ec9beb383840ea65d29cb56cce2553e7fa78d3fd763bfd42
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
      "id": 12,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 50,
      "user_id": 407
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 50,
      "user_id": 406
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 50,
      "user_id": 405
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfbc88c69f61c6d0ec9beb383840ea65d29cb56cce2553e7fa78d3fd763bfd42"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/57/republish
Content-Type: application/json
Authorization: Bearer 4f6c968cb2ada7ea19fe74f2a09e6684ae6fef47e86c03aaed2801ef01ba98b2
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
curl "api.goskive.com/v2/flashcards/57/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f6c968cb2ada7ea19fe74f2a09e6684ae6fef47e86c03aaed2801ef01ba98b2"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/54/bookmark
Content-Type: application/json
Authorization: Bearer 6a449b099de7876a9dcae216d69de0df7b39a7f58e03bd7356c9acbb4b2de502
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/54/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a449b099de7876a9dcae216d69de0df7b39a7f58e03bd7356c9acbb4b2de502"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/58
Content-Type: application/json
Authorization: Bearer 7773e6b95dba9db4229efd58b8b83b3220e27f2d2fc85a70729deaec00252e91
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7773e6b95dba9db4229efd58b8b83b3220e27f2d2fc85a70729deaec00252e91"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/52/downvote
Content-Type: application/json
Authorization: Bearer 71207107015db6db8231f5240dde44a30d3beb0cb5e2d54933c36453c71eef04
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/52/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71207107015db6db8231f5240dde44a30d3beb0cb5e2d54933c36453c71eef04"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/74
Content-Type: application/json
Authorization: Bearer 1ae162604decd0993b77392e655a076c24a5a810c305eea83897c7b1d11ee51b
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 496,
    "chapter_id": 106,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:00:43.316Z",
    "created_at": "2016-11-04T16:00:43.316Z",
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
curl "api.goskive.com/v2/flashcards/74" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ae162604decd0993b77392e655a076c24a5a810c305eea83897c7b1d11ee51b"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/55/report
Content-Type: application/json
Authorization: Bearer 7602f2080c6df51a3c993ccab6f0068d114c1ab51f556404dc98488602901ccb
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
	-H "Authorization: Bearer 7602f2080c6df51a3c993ccab6f0068d114c1ab51f556404dc98488602901ccb"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/51/bookmark
Content-Type: application/json
Authorization: Bearer 4405716cac1c4756411d09f17dd08732395c7de28d99486441c635947f12d1c6
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/51/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4405716cac1c4756411d09f17dd08732395c7de28d99486441c635947f12d1c6"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/53/upvote
Content-Type: application/json
Authorization: Bearer 2d864d414923f8b85e0fe491532bfb2ce2a5a8dbf46f99876137881b1bd7b864
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
	-H "Authorization: Bearer 2d864d414923f8b85e0fe491532bfb2ce2a5a8dbf46f99876137881b1bd7b864"
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
    "key": "cache/98be56e961e819d8950264ca36527b96.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wNFQxNzowMDo0NloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzk4YmU1NmU5NjFlODE5ZDg5NTAyNjRjYTM2NTI3Yjk2LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwNC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDRUMTYwMDQ2WiJ9XX0=",
    "x-amz-credential": "FAKE/20161104/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161104T160046Z",
    "x-amz-signature": "3dfc5a3c9e19448ad63b2d62d3c80c9ce3e0b942c599e34f5c6354e60f12a639"
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
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 30717993ae53e13bf4acbc66dbd1f1a96c65855501d8a37fc44d11aa6d409bd9
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
curl "api.goskive.com/v2/me/jobs/3/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30717993ae53e13bf4acbc66dbd1f1a96c65855501d8a37fc44d11aa6d409bd9"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 6e9bd0fcc94cc3791fffaf6c43c32bb5406e92afa20a914a6524273c8e15b69e
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
	-H "Authorization: Bearer 6e9bd0fcc94cc3791fffaf6c43c32bb5406e92afa20a914a6524273c8e15b69e"
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
{"password":{"reset_password_token":"a6Qr-6GXZnNhydU_Tddr","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 846,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-04T16:01:12.067Z",
  "updated_at": "2016-11-04T16:01:12.213Z",
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
  "audit_id": 5430
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"a6Qr-6GXZnNhydU_Tddr","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/65/comments
Content-Type: application/json
Authorization: Bearer 6477c958cc6a7c3ae8a1f212a6ec683372e47c6b77d2a5afbe9df4ba2bba8faf
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
    "author_id": 502,
    "reply_to_id": null,
    "created_at": "2016-11-04T16:00:44.078Z",
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
curl "api.goskive.com/v2/questions/65/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6477c958cc6a7c3ae8a1f212a6ec683372e47c6b77d2a5afbe9df4ba2bba8faf"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/66/comments
Content-Type: application/json
Authorization: Bearer 501303c245befaaf1e5a9daefa22210f08c93b0eb1933f103158cce97921b489
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
    "id": 3,
    "author_id": 505,
    "reply_to_id": null,
    "created_at": "2016-11-04T16:00:44.617Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 29,
      "user_id": 505,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:44.612Z",
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
curl "api.goskive.com/v2/questions/66/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 501303c245befaaf1e5a9daefa22210f08c93b0eb1933f103158cce97921b489"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/67/comments
Content-Type: application/json
Authorization: Bearer 7e367661a2dca74e9790535846246f6dc8c4bea4333927c020e7b9b73e28de7f
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
      "author_id": 511,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:45.075Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 512,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:45.091Z",
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
curl "api.goskive.com/v2/questions/67/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e367661a2dca74e9790535846246f6dc8c4bea4333927c020e7b9b73e28de7f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/64/comments
Content-Type: application/json
Authorization: Bearer 05caa87912f09202e10af88297cef228519522618ebc3b1fa7e2ab00603061eb
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
curl "api.goskive.com/v2/questions/64/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05caa87912f09202e10af88297cef228519522618ebc3b1fa7e2ab00603061eb"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/88/feedbacks
Content-Type: application/json
Authorization: Bearer 5f89627a05a0aabbaee2b4b4d29a631ebb1378bbb786b64ead922274b81d4d97
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
    "id": 36,
    "user_id": 717,
    "feedbackable_id": 88,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-04T16:00:59.557Z",
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
curl "api.goskive.com/v2/questions/88/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5f89627a05a0aabbaee2b4b4d29a631ebb1378bbb786b64ead922274b81d4d97"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/83/feedbacks
Content-Type: application/json
Authorization: Bearer 851ba9adc4d6ee40a0020c2211e60aac05c00e8e56e173c6c281a3956924a434
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
      "id": 31,
      "user_id": 694,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:57.824Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 693,
      "feedbackable_id": 83,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:57.813Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/83/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 851ba9adc4d6ee40a0020c2211e60aac05c00e8e56e173c6c281a3956924a434"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/32/votes
Content-Type: application/json
Authorization: Bearer 5fad9d12bdd895e36d1fc15aedf6eff8f951c80449e2941dccb50b597cfc1876
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
      "id": 4,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 246
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 245
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 32,
      "user_id": 244
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/32/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fad9d12bdd895e36d1fc15aedf6eff8f951c80449e2941dccb50b597cfc1876"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/111/republish
Content-Type: application/json
Authorization: Bearer 263693615c34ee64eeb69169e877c117a53765842fce892513feadc494837859
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
curl "api.goskive.com/v2/questions/111/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 263693615c34ee64eeb69169e877c117a53765842fce892513feadc494837859"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/132/bookmark
Content-Type: application/json
Authorization: Bearer 1c25c9abf56d205c44736ba1ce9753207633cd0e147c124c719fd10195718552
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/132/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c25c9abf56d205c44736ba1ce9753207633cd0e147c124c719fd10195718552"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/130
Content-Type: application/json
Authorization: Bearer cccd944540a1a1e02ca275cb7ee430bd0ab6a47bfe30b59396c71681599beb3a
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/130" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cccd944540a1a1e02ca275cb7ee430bd0ab6a47bfe30b59396c71681599beb3a"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/131/downvote
Content-Type: application/json
Authorization: Bearer 2390fa9f75a83a67f786ae4788f3e0ea16f53590ecccf8b9252e966353003138
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/131/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2390fa9f75a83a67f786ae4788f3e0ea16f53590ecccf8b9252e966353003138"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/112
Content-Type: application/json
Authorization: Bearer 00d5606d8f62ee0b65f8f8cab756856153b21856ff34588b35ac24fc43950f57
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
    "id": 112,
    "obfuscated_id": "7Qwj1ZvbWUI",
    "author_id": 878,
    "chapter_id": 165,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:01:15.636Z",
    "created_at": "2016-11-04T16:01:15.515Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 226,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 227,
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
curl "api.goskive.com/v2/questions/112" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00d5606d8f62ee0b65f8f8cab756856153b21856ff34588b35ac24fc43950f57"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/109/report
Content-Type: application/json
Authorization: Bearer 1bbe12cfbbcc7594fe0a83a134c47137e8bf1aee2782f7ba6ddfcf08f5627a53
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bbe12cfbbcc7594fe0a83a134c47137e8bf1aee2782f7ba6ddfcf08f5627a53"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/113/bookmark
Content-Type: application/json
Authorization: Bearer a79640e7fbb87ae60bb0793962b19c78957b26ed47f3c33ae40577b9ca305918
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/113/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a79640e7fbb87ae60bb0793962b19c78957b26ed47f3c33ae40577b9ca305918"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/133
Content-Type: application/json
Authorization: Bearer 9675a0122459ca35640bbcd7a7beb54ee7f649f4650e538e73cdef0f79026019
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":133,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-04T16:01:22.326Z","updated_at":"2016-11-04T16:01:22.448Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":186,"author_id":946,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 133,
    "obfuscated_id": "iZjW2yXbK_s",
    "author_id": 946,
    "chapter_id": 186,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-04T16:01:22.561Z",
    "created_at": "2016-11-04T16:01:22.326Z",
    "tags": [
      {
        "id": 18,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 17,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>133, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-04T16:01:22.326Z\", \"updated_at\"=>\"2016-11-04T16:01:22.448Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>186, \"author_id\"=>946, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 268,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 269,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 270,
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
curl "api.goskive.com/v2/questions/133" -d '{"question":{"question":{"id":133,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-04T16:01:22.326Z","updated_at":"2016-11-04T16:01:22.448Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":186,"author_id":946,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9675a0122459ca35640bbcd7a7beb54ee7f649f4650e538e73cdef0f79026019"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/114/upvote
Content-Type: application/json
Authorization: Bearer 1bf9980658f8ac77ad9701aaa2bc8c6a01fd5422a8c8588a467881a8578f9439
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/114/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bf9980658f8ac77ad9701aaa2bc8c6a01fd5422a8c8588a467881a8578f9439"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 426fd1886af6998a44d2654d5ec2b8569749f9c3fe1b2adc02fab58338129e4a
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
      "creator_id": 383,
      "id": 107,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 107,
      "additional_university_ids": [

      ],
      "topic_id": 109,
      "discipline_id": 109,
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
      "updated_at": "2016-11-04T16:00:35.723Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 426fd1886af6998a44d2654d5ec2b8569749f9c3fe1b2adc02fab58338129e4a"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 104e1d9b6d6f28052f7841deef8d02134566189d99276c6c6c0be66706b6eb04
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
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-110",
      "html_url": "https://goskive.com/university/uni-110",
      "slug": "uni-110",
      "name": "National School of Pizza",
      "short_name": "Uni 110",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/82018de485d26c9bc27540446774b49169a40672.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/185a914e401fa48a03ae327e11f997764d72b2a1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-04T16:00:35.976Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 109,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-109",
      "html_url": "https://goskive.com/university/uni-109",
      "slug": "uni-109",
      "name": "National School of Pastry",
      "short_name": "Uni 109",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/4bb8ec2c77619620225b3baa5e95c92743b5375d.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2d8a95d4c289fcc26bc01926bad682d4733c5159.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-04T16:00:35.959Z",
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
	-H "Authorization: Bearer 104e1d9b6d6f28052f7841deef8d02134566189d99276c6c6c0be66706b6eb04"
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
      "id": 113,
      "name": "Seamless systemic superstructure",
      "name_translations": {
        "en": "Seamless systemic superstructure"
      },
      "discipline_id": 113
    },
    {
      "id": 114,
      "name": "Total methodical complexity",
      "name_translations": {
        "en": "Total methodical complexity"
      },
      "discipline_id": 114
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
GET /v2/topics/112
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
    "id": 112,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 112
  }
}
```



```shell
curl "api.goskive.com/v2/topics/112" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer bea6b0d90446377a43d2dcb8132405f26de6966d9d4ed3400e5f2f528631c5fb
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
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-231",
      "html_url": "https://goskive.com/university/uni-231",
      "slug": "uni-231",
      "name": "University 168",
      "short_name": "Uni 231",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/aee0e8778cebe8ef22ecd763ce669c45c411ac08.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/87edf157c124817113d9d83db19282c9de6c6882.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-04T16:01:07.600Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-232",
      "html_url": "https://goskive.com/university/uni-232",
      "slug": "uni-232",
      "name": "University 169",
      "short_name": "Uni 232",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5452440103d47f459860a7f29f11e6182638afd3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/06389f81ddf2855e2ca107caf3d25de393066871.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-04T16:01:07.616Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-233",
      "html_url": "https://goskive.com/university/uni-233",
      "slug": "uni-233",
      "name": "University 170",
      "short_name": "Uni 233",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6190885c79a9290a49e008b96248f3e1bb3a995c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/07a9325f04475d8c3eff2cba8569141090ba847d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-04T16:01:07.633Z",
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
	-H "Authorization: Bearer bea6b0d90446377a43d2dcb8132405f26de6966d9d4ed3400e5f2f528631c5fb"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 3857d7211ce36a8e7b708ed77b36f35c94214649626a7f3e17f4616fcc907773
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
    "id": 249,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e64064e496406e3a9b1490f3767d064cb75ccc04.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/954dc48a8dbf886056be89bcb3474002f8db527d.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-04T16:01:07.427Z",
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
	-H "Authorization: Bearer 3857d7211ce36a8e7b708ed77b36f35c94214649626a7f3e17f4616fcc907773"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a9abb85d8c3c2e53659ce8a29ca4d909d64411599569913d654d155c48d40271
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":232,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 728,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 224,
    "additional_university_ids": [

    ],
    "topic_id": 232,
    "discipline_id": 232,
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
    "chapters_updated_at": "2016-11-04T16:01:00.746Z",
    "updated_at": "2016-11-04T16:01:00.883Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 132,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-11-04T16:01:00.840Z",
        "course_id": 222,
        "author_id": 728,
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
        "id": 133,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-11-04T16:01:00.857Z",
        "course_id": 222,
        "author_id": 728,
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
        "id": 134,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-11-04T16:01:00.874Z",
        "course_id": 222,
        "author_id": 728,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":232,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9abb85d8c3c2e53659ce8a29ca4d909d64411599569913d654d155c48d40271"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c421568cf4d91e224b0c1c4981caa8a4b1864f74c4814f79533eb16af7f2c381
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":231,"published":false}}
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
    "creator_id": 727,
    "id": 221,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 223,
    "additional_university_ids": [

    ],
    "topic_id": 231,
    "discipline_id": 231,
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
    "updated_at": "2016-11-04T16:01:00.710Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":231,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c421568cf4d91e224b0c1c4981caa8a4b1864f74c4814f79533eb16af7f2c381"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b95519d8ea938a58e492861e6a3649f339cf0f6bcdc5e0114dfe5b599127ef2e
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
      "creator_id": 735,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 240,
      "discipline_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
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
      "updated_at": "2016-11-04T16:01:01.528Z",
      "shortname": "fu-course-167"
    },
    {
      "creator_id": 735,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "topic_id": 241,
      "discipline_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
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
      "chapters_updated_at": "2016-11-04T16:01:01.829Z",
      "updated_at": "2016-11-04T16:01:01.836Z",
      "shortname": "fu-course-168"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b95519d8ea938a58e492861e6a3649f339cf0f6bcdc5e0114dfe5b599127ef2e"
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
      "creator_id": 765,
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 237,
      "additional_university_ids": [

      ],
      "topic_id": 264,
      "discipline_id": 264,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 191",
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
      "updated_at": "2016-11-04T16:01:04.166Z",
      "shortname": "fu-course-191"
    },
    {
      "creator_id": 765,
      "id": 255,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 237,
      "additional_university_ids": [

      ],
      "topic_id": 265,
      "discipline_id": 265,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
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
      "chapters_updated_at": "2016-11-04T16:01:04.469Z",
      "updated_at": "2016-11-04T16:01:04.476Z",
      "shortname": "fu-course-192"
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
Authorization: Bearer 47aac91887840b73fe748d60bbaf0568d5f96327e9f291cbc784a6f102279fe9
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
      "creator_id": 741,
      "id": 234,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-171",
      "html_url": "https://goskive.com/course/fu-course-171",
      "slug": "fu-course-171",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 244,
      "discipline_id": 244,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 171",
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
      "updated_at": "2016-11-04T16:01:02.064Z",
      "shortname": "fu-course-171"
    },
    {
      "creator_id": 741,
      "id": 235,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 245,
      "discipline_id": 245,
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
      "updated_at": "2016-11-04T16:01:02.104Z",
      "shortname": "fu-course-172"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47aac91887840b73fe748d60bbaf0568d5f96327e9f291cbc784a6f102279fe9"
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
      "creator_id": 770,
      "id": 258,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 238,
      "additional_university_ids": [

      ],
      "topic_id": 268,
      "discipline_id": 268,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
      "updated_at": "2016-11-04T16:01:04.657Z",
      "shortname": "fu-course-195"
    },
    {
      "creator_id": 770,
      "id": 259,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-196",
      "html_url": "https://goskive.com/course/fu-course-196",
      "slug": "fu-course-196",
      "university_id": 238,
      "additional_university_ids": [

      ],
      "topic_id": 269,
      "discipline_id": 269,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 196",
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
      "updated_at": "2016-11-04T16:01:04.697Z",
      "shortname": "fu-course-196"
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
Authorization: Bearer d066c3952d920250253a4d16b6d2b80ab37c0133a22b7e38fa8f8316b5a46c35
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
  "id": 387,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-04T16:00:36.085Z",
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
	-H "Authorization: Bearer d066c3952d920250253a4d16b6d2b80ab37c0133a22b7e38fa8f8316b5a46c35"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/334
Content-Type: application/json
Authorization: Bearer 259998327278f4f1f7afb2e2d30af5d39f4a6f516f155aa4867b51ff1a981a8b
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
    "id": 334,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 90,
    "fields_of_study": [
      90,
      91
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-04T16:00:33.012Z",
    "updated_at": "2016-11-04T16:00:33.012Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/334" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 259998327278f4f1f7afb2e2d30af5d39f4a6f516f155aa4867b51ff1a981a8b"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/336
Content-Type: application/json
Authorization: Bearer 32321553a95dd5ffda81953e3f5a8a84f2a31b14199095f3c0b910f052e001c0
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
    "id": 336,
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
    "created_at": "2016-11-04T16:00:33.108Z",
    "updated_at": "2016-11-04T16:00:33.108Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/336" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32321553a95dd5ffda81953e3f5a8a84f2a31b14199095f3c0b910f052e001c0"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/5
Content-Type: application/json
Authorization: Bearer 7bf94edba3822a70934a4e6d9289ed7af23c23e8f6231ab9c59182dcbec0aa41
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7bf94edba3822a70934a4e6d9289ed7af23c23e8f6231ab9c59182dcbec0aa41"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/7
Content-Type: application/json
Authorization: Bearer ef2ee7e7ad1153c94629cd8745483d40675061016ce5892f4379a098ce9fad5c
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
    "votable_id": 63,
    "user_id": 328
  }
}
```



```shell
curl "api.goskive.com/v2/votes/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef2ee7e7ad1153c94629cd8745483d40675061016ce5892f4379a098ce9fad5c"
```
