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
Authorization: Basic ZTE1ZGMwOTRiYzJkMDQ4NmEzYjc5YzRkYmFkYjY1YTM0ODViNTY2ZTRiYzY4
NWRlODI5YjA5YWFlODgyZWY3NzpkNjcxNzZlYWJhZWE1MmIxNDQ0ZDYxN2Fk
ZTA2YmFiMzNhNmEwMTM3Y2UzMzIyN2U5ODY0NTNhMDdjNDM5NzA0

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
	-u e15dc094bc2d0486a3b79c4dbadb65a3485b566e4bc685de829b09aae882ef77:d67176eabaea52b1444d617ade06bab33a6a0137ce33227e986453a07c439704
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"46a6c7b13c65938e94a50c6493262f311ec44b1bb6a3e2e454a77df50da72b68","client_secret":"5f605a64060385f48ef17ddaf4ff556195caeaa00a3c0a177c10b6b50ecdfa61"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"46a6c7b13c65938e94a50c6493262f311ec44b1bb6a3e2e454a77df50da72b68","client_secret":"5f605a64060385f48ef17ddaf4ff556195caeaa00a3c0a177c10b6b50ecdfa61"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"575f082ef8d836b36b987f17bcdba880d57b06fcda5ecabcc981d1c0a9f9b07f","client_secret":"3c2d070679ad8eb990752d36c06d78bdc2213054c72b59d8277936badbd8a35f"}
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
  "access_token": "c268a17efaf5b90043b089f10634c3ccb7b7826cef4b0a1a836926405114711d",
  "token_type": "bearer",
  "created_at": 1477484980
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"575f082ef8d836b36b987f17bcdba880d57b06fcda5ecabcc981d1c0a9f9b07f","client_secret":"3c2d070679ad8eb990752d36c06d78bdc2213054c72b59d8277936badbd8a35f"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTkxYzZiODU5NzE3MGRiNThmZTdmZmRkMzgzYmY0Y2RiMjBiMTBkNWZjZWQ0
YjdkNzMzYzk3MDVhNTFlMDkwNDpkMDBlYjRiMWI4OWQ5YWIwMzZhN2I5ZTQ0
NDIwZjU0MDU4YzM5M2UzN2UwM2MwZWIyZTBhNDJlMjE1MDE4YjBi

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
  "access_token": "9b240f866e3c2e14ab8edfad0554ddfb9ba7f0b95f899ff5cab8d5e5f45b0661",
  "token_type": "bearer",
  "created_at": 1477484980
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u a91c6b8597170db58fe7ffdd383bf4cdb20b10d5fced4b7d733c9705a51e0904:d00eb4b1b89d9ab036a7b9e44420f54058c393e37e03c0eb2e0a42e215018b0b
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"10f5595fe722c9a20d8244eb79e49b500ee60d4952db5020e95ead78019a5c8e","client_secret":"d281f9edd96a6ab4840df2a0d760e76405a338fe4c8b661cda03faf36c2456e1"}
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
  "access_token": "541de671c1aaa4edaa777512a6dedbfe1ed1039235e59f30a5072749ae3f6c9c",
  "token_type": "bearer",
  "created_at": 1477484980
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"10f5595fe722c9a20d8244eb79e49b500ee60d4952db5020e95ead78019a5c8e","client_secret":"d281f9edd96a6ab4840df2a0d760e76405a338fe4c8b661cda03faf36c2456e1"}' -X POST \
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
Authorization: Bearer 691a147b013a3507a30e681ff7562b9611f56efe56f97de2b75bc91faf3c1dd9
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
    "company_id": 1,
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
	-H "Authorization: Bearer 691a147b013a3507a30e681ff7562b9611f56efe56f97de2b75bc91faf3c1dd9"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/142/flashcards
Content-Type: application/json
Authorization: Bearer 7dfa16efdb5e9c580199c6c3946612d4b0c7dc9a6b9919e147380782c3aa9d0a
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":142,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 622,
    "chapter_id": 142,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:29:34.057Z",
    "created_at": "2016-10-26T12:29:34.057Z",
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
curl "api.goskive.com/v2/chapters/142/flashcards" -d '{"flashcard":{"chapter_id":142,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dfa16efdb5e9c580199c6c3946612d4b0c7dc9a6b9919e147380782c3aa9d0a"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/144/flashcards
Content-Type: application/json
Authorization: Bearer be7b3abae567a60422da0bad78e6d7d48cd1d49311090eb128d9be40b70148f1
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
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 626,
      "chapter_id": 144,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:34.316Z",
      "created_at": "2016-10-26T12:29:34.316Z",
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
      "author_id": 626,
      "chapter_id": 144,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:34.353Z",
      "created_at": "2016-10-26T12:29:34.353Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 626,
      "chapter_id": 144,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:29:34.389Z",
      "created_at": "2016-10-26T12:29:34.389Z",
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
curl "api.goskive.com/v2/chapters/144/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be7b3abae567a60422da0bad78e6d7d48cd1d49311090eb128d9be40b70148f1"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/38/questions
Content-Type: application/json
Authorization: Bearer d54bf1f994ce9e3065d17dce82ea8eaf90a31d89f35885087b772d27d5b65ae6
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 19,
    "obfuscated_id": "xt199h-LGto",
    "author_id": 155,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:51.774Z",
    "created_at": "2016-10-26T12:28:51.774Z",
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
        "id": 38,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 39,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 40,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 41,
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
curl "api.goskive.com/v2/chapters/38/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":38,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d54bf1f994ce9e3065d17dce82ea8eaf90a31d89f35885087b772d27d5b65ae6"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/35/questions
Content-Type: application/json
Authorization: Bearer 113ee3fb02d9358f5ad9bd06aefbd22d2a4e8e950c544e5968b1db85d696377c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":35,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 16,
    "obfuscated_id": "Drq0t9y67cE",
    "author_id": 146,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:50.667Z",
    "created_at": "2016-10-26T12:28:50.667Z",
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
        "id": 31,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 32,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/35/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":35,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 113ee3fb02d9358f5ad9bd06aefbd22d2a4e8e950c544e5968b1db85d696377c"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/36/questions
Content-Type: application/json
Authorization: Bearer c06d089ebe96b41cc3f9e99ac5a6b042076d34adc0263affd8520f816ceed44f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 17,
    "obfuscated_id": "s3oqsdqLejU",
    "author_id": 149,
    "chapter_id": 36,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:51.016Z",
    "created_at": "2016-10-26T12:28:51.016Z",
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
        "id": 33,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 34,
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
curl "api.goskive.com/v2/chapters/36/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":36,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c06d089ebe96b41cc3f9e99ac5a6b042076d34adc0263affd8520f816ceed44f"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/37/questions
Content-Type: application/json
Authorization: Bearer 75aea7cc212f421750c47963c92bd557992730cb62b4ecb09273b46723ed6dac
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":37,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 18,
    "obfuscated_id": "9KZ-wsvd6MY",
    "author_id": 152,
    "chapter_id": 37,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:51.353Z",
    "created_at": "2016-10-26T12:28:51.353Z",
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
        "id": 35,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 36,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 37,
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
curl "api.goskive.com/v2/chapters/37/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":37,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75aea7cc212f421750c47963c92bd557992730cb62b4ecb09273b46723ed6dac"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/33/questions
Content-Type: application/json
Authorization: Bearer 00db61ac20e7206457fde0caa1dd5c32d6cd667311b9da7de62b63ecd5803c56
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 137,
      "chapter_id": 33,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:49.877Z",
      "created_at": "2016-10-26T12:28:49.754Z",
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
          "id": 25,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 26,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 138,
      "chapter_id": 33,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:50.074Z",
      "created_at": "2016-10-26T12:28:49.948Z",
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
          "id": 27,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 28,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 139,
      "chapter_id": 33,
      "position": 15,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T12:28:50.277Z",
      "created_at": "2016-10-26T12:28:50.147Z",
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
          "id": 29,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 30,
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
curl "api.goskive.com/v2/chapters/33/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00db61ac20e7206457fde0caa1dd5c32d6cd667311b9da7de62b63ecd5803c56"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/188
Content-Type: application/json
Authorization: Bearer 7b2195ef6a6f6550d4274cacf956d1089e94185230e51cd82dc20d89edd4a3c0
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
curl "api.goskive.com/v2/chapters/188" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b2195ef6a6f6550d4274cacf956d1089e94185230e51cd82dc20d89edd4a3c0"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 32e492585920e45d39a09154013186725ff240d4a600640b3842c0c782149547
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
curl "api.goskive.com/v2/chapters/190" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32e492585920e45d39a09154013186725ff240d4a600640b3842c0c782149547"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/185
Content-Type: application/json
Authorization: Bearer 95c0fb7d3c77a9ce127238194c0b61285d620004eb16eef3515885419ca662e0
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
curl "api.goskive.com/v2/chapters/185" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95c0fb7d3c77a9ce127238194c0b61285d620004eb16eef3515885419ca662e0"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 7e6a32e4dbd21438eafd3a249c008b0437bf7384ffe62b24b4174ed3df2f3831
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/189" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e6a32e4dbd21438eafd3a249c008b0437bf7384ffe62b24b4174ed3df2f3831"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/182
Content-Type: application/json
Authorization: Bearer e1b32b772d7e724fc7e97f5f2f1107054923b8308aba82d0a510f077915edf12
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
    "id": 182,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T12:29:52.509Z",
    "course_id": 288,
    "author_id": 906,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-26T12:29:51.979Z",
    "questions_updated_at": "2016-10-26T12:29:51.979Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 910,
        "chapter_id": 182,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:52.491Z",
        "created_at": "2016-10-26T12:29:52.491Z",
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
        "id": 126,
        "obfuscated_id": "fKTMLttUR-w",
        "author_id": 908,
        "chapter_id": 182,
        "position": 113,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:52.385Z",
        "created_at": "2016-10-26T12:29:52.267Z",
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
            "id": 255,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 256,
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
curl "api.goskive.com/v2/chapters/182" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1b32b772d7e724fc7e97f5f2f1107054923b8308aba82d0a510f077915edf12"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/186
Content-Type: application/json
Authorization: Bearer 1c633ac74d7665ed957ac8dfb09a03e16faf056351a1ed36c922bb1d0f81a73f
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
    "id": 186,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T12:29:53.623Z",
    "course_id": 292,
    "author_id": 926,
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
curl "api.goskive.com/v2/chapters/186" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c633ac74d7665ed957ac8dfb09a03e16faf056351a1ed36c922bb1d0f81a73f"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer ec0bd1a93c32495ecc4b86326a8660a186af5f119afe1cbf889b15c63aaf53ed
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
    "author_id": 899,
    "reply_to_id": 58,
    "created_at": "2016-10-26T12:29:51.494Z",
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
	-H "Authorization: Bearer ec0bd1a93c32495ecc4b86326a8660a186af5f119afe1cbf889b15c63aaf53ed"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer d5ef531a471bcc951a3fccc9bb78e2d5b7257e3bb73c43c8a984580198b77de5
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
	-H "Authorization: Bearer d5ef531a471bcc951a3fccc9bb78e2d5b7257e3bb73c43c8a984580198b77de5"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer 52107291002a6942d459725f69fd96bc7eedeefbed7c9718435a9e0f18f7e113
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
curl "api.goskive.com/v2/comments/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52107291002a6942d459725f69fd96bc7eedeefbed7c9718435a9e0f18f7e113"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/42/republish
Content-Type: application/json
Authorization: Bearer 66a8fde64f45740474e5c6dfc985b19864fa2abcf025d1403f2974b592ea924d
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
curl "api.goskive.com/v2/comments/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66a8fde64f45740474e5c6dfc985b19864fa2abcf025d1403f2974b592ea924d"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer 144a361de4a9f60a0919fdd676bb092b34cf493bb5908594c4dd339271fec8b3
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 144a361de4a9f60a0919fdd676bb092b34cf493bb5908594c4dd339271fec8b3"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/40/report
Content-Type: application/json
Authorization: Bearer 7421838bea797a582dbb2f32a9417d5514dc9d32ec19f96d1de61e3f5ff43cd8
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/40/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7421838bea797a582dbb2f32a9417d5514dc9d32ec19f96d1de61e3f5ff43cd8"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/5
Content-Type: application/json
Authorization: Bearer 7825a9fdb00c900b58e3cb5dbdf708091a071a761a5c2f92ad1f6098cb341fe5
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
    "id": 5,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-26T12:28:57.964Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7825a9fdb00c900b58e3cb5dbdf708091a071a761a5c2f92ad1f6098cb341fe5"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 3af4eda200c87b05510a790dc4abf4e40129a159214cb98248b033ad4ab18b78
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
      "id": 2,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8391423c1d91938de942cf9859ae9a53d10a866a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T12:28:57.842Z"
    },
    {
      "id": 3,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T12:28:57.847Z"
    },
    {
      "id": 4,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-26T12:28:57.850Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3af4eda200c87b05510a790dc4abf4e40129a159214cb98248b033ad4ab18b78"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/18/company_profiles
Content-Type: application/json
Authorization: Bearer 91c70b31eb793a7972ba62c07accba36ba7d9a4f9a0425da4a4d91dbd92047f7
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
curl "api.goskive.com/v2/companies/18/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91c70b31eb793a7972ba62c07accba36ba7d9a4f9a0425da4a4d91dbd92047f7"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/17/company_profiles
Content-Type: application/json
Authorization: Bearer b7c9d06c06631f4077fcd159b5089a6c150fdb576b5653a426132742d89ed6b5
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
curl "api.goskive.com/v2/companies/17/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7c9d06c06631f4077fcd159b5089a6c150fdb576b5653a426132742d89ed6b5"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 4dd695d37d7234dbef0e15700cff341eca1cad20374f19593e36097732cc36b6
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
	-H "Authorization: Bearer 4dd695d37d7234dbef0e15700cff341eca1cad20374f19593e36097732cc36b6"
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
Authorization: Bearer 09baabdfa3d408e75b0440057dec94355f7cc824d8e6b213a3076f314e6b629e
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
	-H "Authorization: Bearer 09baabdfa3d408e75b0440057dec94355f7cc824d8e6b213a3076f314e6b629e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 57685d1c2d4096140f737b14e34b850400b55717ed3d7f02f6d96c0d600f61eb
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
    "id": 118,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T12:29:30.279Z",
    "course_id": 185,
    "author_id": 560,
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
	-H "Authorization: Bearer 57685d1c2d4096140f737b14e34b850400b55717ed3d7f02f6d96c0d600f61eb"
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
      "id": 124,
      "title": "Clever Chapter Title 112",
      "position": 1,
      "updated_at": "2016-10-26T12:29:30.948Z",
      "course_id": 190,
      "author_id": 573,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 125,
      "title": "Clever Chapter Title 113",
      "position": 2,
      "updated_at": "2016-10-26T12:29:30.971Z",
      "course_id": 190,
      "author_id": 574,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 126,
      "title": "Clever Chapter Title 114",
      "position": 3,
      "updated_at": "2016-10-26T12:29:31.249Z",
      "course_id": 190,
      "author_id": 575,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T12:29:30.874Z",
      "questions_updated_at": "2016-10-26T12:29:30.874Z",
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
Authorization: Bearer cf66888569ef274db85b72b2441ca8340b92700eb591d03bd8cc2c935f91d2ac
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
      "id": 130,
      "title": "Clever Chapter Title 118",
      "position": 1,
      "updated_at": "2016-10-26T12:29:31.601Z",
      "course_id": 193,
      "author_id": 584,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 131,
      "title": "Clever Chapter Title 119",
      "position": 2,
      "updated_at": "2016-10-26T12:29:31.624Z",
      "course_id": 193,
      "author_id": 585,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 120",
      "position": 3,
      "updated_at": "2016-10-26T12:29:31.872Z",
      "course_id": 193,
      "author_id": 586,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-26T12:29:31.527Z",
      "questions_updated_at": "2016-10-26T12:29:31.527Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf66888569ef274db85b72b2441ca8340b92700eb591d03bd8cc2c935f91d2ac"
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
      "id": 127,
      "title": "Clever Chapter Title 115",
      "position": 1,
      "updated_at": "2016-10-26T12:29:31.364Z",
      "course_id": 191,
      "author_id": 579,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 128,
      "title": "Clever Chapter Title 116",
      "position": 2,
      "updated_at": "2016-10-26T12:29:31.387Z",
      "course_id": 191,
      "author_id": 580,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 129,
      "title": "Clever Chapter Title 117",
      "position": 3,
      "updated_at": "2016-10-26T12:29:31.411Z",
      "course_id": 191,
      "author_id": 581,
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
Authorization: Bearer d231ad72c656b6b2d79fe3a8b251ee36c882f082d8d4101a18ac17b8d1512ae8
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
      "id": 133,
      "title": "Clever Chapter Title 121",
      "position": 1,
      "updated_at": "2016-10-26T12:29:32.128Z",
      "course_id": 195,
      "author_id": 593,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 134,
      "title": "Clever Chapter Title 122",
      "position": 2,
      "updated_at": "2016-10-26T12:29:32.155Z",
      "course_id": 195,
      "author_id": 594,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 135,
      "title": "Clever Chapter Title 123",
      "position": 3,
      "updated_at": "2016-10-26T12:29:32.178Z",
      "course_id": 195,
      "author_id": 595,
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
	-H "Authorization: Bearer d231ad72c656b6b2d79fe3a8b251ee36c882f082d8d4101a18ac17b8d1512ae8"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer a64a6079dc5fcb9df3d8731135bf0179e71ba25120c73b109aaf94a3ec5ba9d4
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
    "course_id": 33,
    "user_id": 105,
    "updated_at": "2016-10-26T12:28:46.846Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a64a6079dc5fcb9df3d8731135bf0179e71ba25120c73b109aaf94a3ec5ba9d4"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d02162595598c962b11702f83c9d4d095acca352b47c1c6ec224eeb03c57f875
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
      "course_id": 32,
      "user_id": 101,
      "updated_at": "2016-10-26T12:28:46.669Z"
    },
    {
      "id": 4,
      "course_id": 32,
      "user_id": 102,
      "updated_at": "2016-10-26T12:28:46.683Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d02162595598c962b11702f83c9d4d095acca352b47c1c6ec224eeb03c57f875"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/245/files
Content-Type: application/json
Authorization: Bearer 8ba0605ae7c6ad28c3cb1d8f7f448b6b990e6f34074021ac9aec9a3cf087533c
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
        "id": 727,
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
        "created_at": "2016-10-26T12:29:38.720Z",
        "updated_at": "2016-10-26T12:29:38.720Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T12:29:38.731Z",
      "updated_at": "2016-10-26T12:29:38.731Z",
      "course_id": 245,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 15,
      "uploader": {
        "id": 728,
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
        "created_at": "2016-10-26T12:29:38.738Z",
        "updated_at": "2016-10-26T12:29:38.738Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T12:29:38.747Z",
      "updated_at": "2016-10-26T12:29:38.747Z",
      "course_id": 245,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 16,
      "uploader": {
        "id": 729,
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
        "created_at": "2016-10-26T12:29:38.754Z",
        "updated_at": "2016-10-26T12:29:38.754Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-26T12:29:38.763Z",
      "updated_at": "2016-10-26T12:29:38.763Z",
      "course_id": 245,
      "filename": "example.pdf",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/245/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ba0605ae7c6ad28c3cb1d8f7f448b6b990e6f34074021ac9aec9a3cf087533c"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/246/files
Content-Type: application/json
Authorization: Bearer 8b10729a76323526e0ace332f57f8173136cba4f5f755232ea91d7f6419e679a
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
    "id": 17,
    "uploader": {
      "id": 732,
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
      "created_at": "2016-10-26T12:29:38.883Z",
      "updated_at": "2016-10-26T12:29:38.883Z"
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
    "created_at": "2016-10-26T12:29:38.911Z",
    "updated_at": "2016-10-26T12:29:38.911Z",
    "course_id": 246,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/246/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b10729a76323526e0ace332f57f8173136cba4f5f755232ea91d7f6419e679a"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/243/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 75224c04dbeb533bf4ddbdfdb4eec3b2efbd8892c0409a501b122deeb2fce9a1
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
    "key": "cache/ab5ee1e497ba468744297a6507f9454f.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxMzoyOTozOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2FiNWVlMWU0OTdiYTQ2ODc0NDI5N2E2NTA3Zjk0NTRmLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjYvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI2VDEyMjkzOFoifV19",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T122938Z",
    "x-amz-signature": "b9c4b1cf35c690d21a2e7bb9f00eed54826e90106b8901f3234e9f95198f736c"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/243/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75224c04dbeb533bf4ddbdfdb4eec3b2efbd8892c0409a501b122deeb2fce9a1"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer b8bf70c1112c6e91806e4b661b8cdad37a141c30cc4577110ab0b974b4d0dd25
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
	-H "Authorization: Bearer b8bf70c1112c6e91806e4b661b8cdad37a141c30cc4577110ab0b974b4d0dd25"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4b7bb93066acab692eb3eeabb68921bf5fd78eb79fad4d5292c0fd426ec6ea71
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
	-H "Authorization: Bearer 4b7bb93066acab692eb3eeabb68921bf5fd78eb79fad4d5292c0fd426ec6ea71"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 472a018453dcfc48ffc4feea293616e7f4f8d24c05c5c56b82fe16a6745ab85e
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
	-H "Authorization: Bearer 472a018453dcfc48ffc4feea293616e7f4f8d24c05c5c56b82fe16a6745ab85e"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 707252a9548fa1ab7c688d5f9e3497168405276852122fa1519ab7ed92817ef0
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
	-H "Authorization: Bearer 707252a9548fa1ab7c688d5f9e3497168405276852122fa1519ab7ed92817ef0"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cead6d000d03730ca29aaac90305ee2a021a37c6112a4ce53415937aed4a9075
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
	-H "Authorization: Bearer cead6d000d03730ca29aaac90305ee2a021a37c6112a4ce53415937aed4a9075"
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
    "creator_id": 352,
    "id": 128,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 112,
    "additional_university_ids": [

    ],
    "topic_id": 135,
    "discipline_id": 136,
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
    "chapters_updated_at": "2016-10-26T12:29:12.431Z",
    "updated_at": "2016-10-26T12:29:13.835Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 76,
        "title": "Clever Chapter Title 67",
        "position": 1,
        "updated_at": "2016-10-26T12:29:13.790Z",
        "course_id": 128,
        "author_id": 352,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T12:29:12.431Z",
        "questions_updated_at": "2016-10-26T12:29:12.431Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 77,
        "title": "Clever Chapter Title 68",
        "position": 2,
        "updated_at": "2016-10-26T12:29:13.827Z",
        "course_id": 128,
        "author_id": 352,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T12:29:12.431Z",
        "questions_updated_at": "2016-10-26T12:29:12.431Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 352,
        "chapter_id": 76,
        "position": 45,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:12.635Z",
        "created_at": "2016-10-26T12:29:12.520Z",
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
            "id": 119,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 120,
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
        "author_id": 352,
        "chapter_id": 77,
        "position": 47,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:13.007Z",
        "created_at": "2016-10-26T12:29:12.887Z",
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
Authorization: Bearer fcc510c8c7c6eb41c36d3ba01178f1fd977abcf592f0698c03c81a74ae0859c2
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
    "creator_id": 363,
    "id": 130,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 114,
    "additional_university_ids": [

    ],
    "topic_id": 137,
    "discipline_id": 138,
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
    "chapters_updated_at": "2016-10-26T12:29:15.396Z",
    "updated_at": "2016-10-26T12:29:16.817Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 80,
        "title": "Clever Chapter Title 71",
        "position": 1,
        "updated_at": "2016-10-26T12:29:16.770Z",
        "course_id": 130,
        "author_id": 363,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T12:29:15.396Z",
        "questions_updated_at": "2016-10-26T12:29:15.396Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 81,
        "title": "Clever Chapter Title 72",
        "position": 2,
        "updated_at": "2016-10-26T12:29:16.810Z",
        "course_id": 130,
        "author_id": 363,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-26T12:29:15.396Z",
        "questions_updated_at": "2016-10-26T12:29:15.396Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 364,
        "chapter_id": 80,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:16.614Z",
        "created_at": "2016-10-26T12:29:16.614Z",
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
        "id": 53,
        "obfuscated_id": "XffxqHkTsbc",
        "author_id": 364,
        "chapter_id": 81,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:16.684Z",
        "created_at": "2016-10-26T12:29:16.684Z",
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
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 364,
        "chapter_id": 80,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:16.653Z",
        "created_at": "2016-10-26T12:29:16.653Z",
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
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 364,
        "chapter_id": 81,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:16.722Z",
        "created_at": "2016-10-26T12:29:16.722Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 364,
        "chapter_id": 80,
        "position": 57,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.607Z",
        "created_at": "2016-10-26T12:29:15.493Z",
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
            "id": 143,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 144,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 364,
        "chapter_id": 80,
        "position": 58,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.778Z",
        "created_at": "2016-10-26T12:29:15.669Z",
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
            "id": 145,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 146,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 364,
        "chapter_id": 81,
        "position": 59,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:15.980Z",
        "created_at": "2016-10-26T12:29:15.859Z",
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
            "id": 147,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 148,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 364,
        "chapter_id": 81,
        "position": 60,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T12:29:16.160Z",
        "created_at": "2016-10-26T12:29:16.045Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcc510c8c7c6eb41c36d3ba01178f1fd977abcf592f0698c03c81a74ae0859c2"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/144/pin
Content-Type: application/json
Authorization: Bearer dea5627660f0c0f7c5401190fd46415180e9f7d5736ae428cade594e672f57eb
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/144/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dea5627660f0c0f7c5401190fd46415180e9f7d5736ae428cade594e672f57eb"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/126/pin
Content-Type: application/json
Authorization: Bearer 087a5b3720bd38489ce34c0300d9185625ad3b0bb54eecb5ef8871b5283bfed4
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/126/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 087a5b3720bd38489ce34c0300d9185625ad3b0bb54eecb5ef8871b5283bfed4"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9daaa55d31977e7d067d5b14b6b89e2225e679b6624658db96c5b5e62f04a47a
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
    "creator_id": 391,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 125,
    "additional_university_ids": [

    ],
    "topic_id": 148,
    "discipline_id": 149,
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
    "updated_at": "2016-10-26T12:29:18.693Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9daaa55d31977e7d067d5b14b6b89e2225e679b6624658db96c5b5e62f04a47a"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer f94ac0b758d1a7ce925eef6ca4fb13ea810b5e7f217306b2d2ca12c389d9a828
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
    "id": 611,
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
    "created_at": "2016-10-26T12:29:32.986Z",
    "updated_at": "2016-10-26T12:29:32.986Z",
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
	-H "Authorization: Bearer f94ac0b758d1a7ce925eef6ca4fb13ea810b5e7f217306b2d2ca12c389d9a828"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f5cbd6503a60813f81fc68f9fae18256db690ae08cdd55810b2ecf6ec09b37e4
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[207]}
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
    "id": 613,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      207
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T12:29:33.408Z",
    "updated_at": "2016-10-26T12:29:33.441Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[207]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5cbd6503a60813f81fc68f9fae18256db690ae08cdd55810b2ecf6ec09b37e4"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 8cf1465ce2ac91b4bc1928c874e2acf50a0d991f3b4f2c1ee68332380b5ffd9e
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
    "id": 614,
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
    "created_at": "2016-10-26T12:29:33.461Z",
    "updated_at": "2016-10-26T12:29:33.461Z",
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
	-H "Authorization: Bearer 8cf1465ce2ac91b4bc1928c874e2acf50a0d991f3b4f2c1ee68332380b5ffd9e"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d16583b6748d95b6eaa52ca4acf1a2732215f1e040295ab5481fb303ef18a969
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[210]}
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
    "id": 616,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      210
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T12:29:33.620Z",
    "updated_at": "2016-10-26T12:29:33.620Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[210]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d16583b6748d95b6eaa52ca4acf1a2732215f1e040295ab5481fb303ef18a969"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer b1d1cf7363036fc24f699f8deb9ee477e8d31147d42efeae3e99ac0c5281c133
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

206
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
    "id": 612,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/bb9f0277119685d1659a40d6ef04bbde0288b37b.jpg",
    "university_id": null,
    "fields_of_study": [
      206
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-26T12:29:33.079Z",
    "updated_at": "2016-10-26T12:29:33.357Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/76396fc19fc5795160f5175185c7da5eb4f04521.jpg",
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

206
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer b1d1cf7363036fc24f699f8deb9ee477e8d31147d42efeae3e99ac0c5281c133"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 37f7d92e340df56a700ec7a70d7e8d1e16b0bf2abf1b4e19a5532b6213b29f3f
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
      "bookmarkable_id": 1,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 2,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 3,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 37f7d92e340df56a700ec7a70d7e8d1e16b0bf2abf1b4e19a5532b6213b29f3f"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 1e84bc1fcfb9893ef21106f1db9c5f2db560e3962ec42feb10d858690c09c0eb
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
      "id": 3,
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
      "id": 4,
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
	-H "Authorization: Bearer 1e84bc1fcfb9893ef21106f1db9c5f2db560e3962ec42feb10d858690c09c0eb"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8089d7bc770ece033ac8085609795fb684152bf2610a4b18283b32f002addf72
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
	-H "Authorization: Bearer 8089d7bc770ece033ac8085609795fb684152bf2610a4b18283b32f002addf72"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer d5d6cd00c47afe8fd55cb3baea1afe72f0c411005999f42deff4ca67eb48c6c0
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
      "creator_id": 414,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-111",
      "html_url": "https://goskive.com/course/mit-course-111",
      "slug": "mit-course-111",
      "university_id": 132,
      "additional_university_ids": [

      ],
      "topic_id": 155,
      "discipline_id": 156,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
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
      "updated_at": "2016-10-26T12:29:20.473Z",
      "shortname": "mit-course-111"
    },
    {
      "creator_id": 415,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-112",
      "html_url": "https://goskive.com/course/mit-course-112",
      "slug": "mit-course-112",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 156,
      "discipline_id": 157,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 112",
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
      "updated_at": "2016-10-26T12:29:20.549Z",
      "shortname": "mit-course-112"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5d6cd00c47afe8fd55cb3baea1afe72f0c411005999f42deff4ca67eb48c6c0"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 7b1d80346ac86a1bf0687c92746c043473ae51ed0c6c3c29f7da91f201581efe
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
      "company_id": 25,
      "company": {
        "id": 25,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T12:29:45.570Z"
      },
      "created_at": "2016-10-26T12:29:45.574Z",
      "updated_at": "2016-10-26T12:29:45.574Z",
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
      "company_id": 26,
      "company": {
        "id": 26,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T12:29:45.581Z"
      },
      "created_at": "2016-10-26T12:29:45.584Z",
      "updated_at": "2016-10-26T12:29:45.584Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b1d80346ac86a1bf0687c92746c043473ae51ed0c6c3c29f7da91f201581efe"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 7b2ffbab2c628b2c9af9cc4d9505d8b809e99597cce04bc6cef14eee845fac52
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 16",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T12:29:45.411Z"
      },
      "created_at": "2016-10-26T12:29:45.414Z",
      "updated_at": "2016-10-26T12:29:45.414Z",
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-26T12:29:45.427Z"
      },
      "created_at": "2016-10-26T12:29:45.431Z",
      "updated_at": "2016-10-26T12:29:45.431Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b2ffbab2c628b2c9af9cc4d9505d8b809e99597cce04bc6cef14eee845fac52"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 13f03c7c6c48092ffa91c8c442888787780c90f97f5c8c2c1c0b076043cab233
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
      "id": 15,
      "created_at": "2016-10-26T12:29:47.100Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 53,
      "updated_at": "2016-10-26T12:29:47.205Z",
      "author_id": "828",
      "thread_subject_id": "269",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-26T12:29:47.194Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 54,
      "updated_at": "2016-10-26T12:29:47.209Z",
      "author_id": "831",
      "thread_subject_id": "270",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-26T12:29:47.565Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-26T12:29:47.565Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-26T12:29:47.929Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-26T12:29:47.929Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-26T12:29:48.296Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-26T12:29:48.296Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-26T12:29:48.587Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 120,
      "updated_at": "2016-10-26T12:29:48.587Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-26T12:29:48.884Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 121,
      "updated_at": "2016-10-26T12:29:48.884Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-26T12:29:49.178Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 122,
      "updated_at": "2016-10-26T12:29:49.178Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13f03c7c6c48092ffa91c8c442888787780c90f97f5c8c2c1c0b076043cab233"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/23
Content-Type: application/json
Authorization: Bearer 4e3cbc86e7cdc9d65e68b6a59252efe35032c15c8b6ce77a8e86de88410fc5dc
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-26T12:19:49.000Z"}}
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
    "id": 23,
    "created_at": "2016-10-26T12:29:49.365Z",
    "read_at": "2016-10-26T12:19:49.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 55,
    "updated_at": "2016-10-26T12:29:49.403Z",
    "author_id": "857",
    "thread_subject_id": "277",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/23" -d '{"notification":{"read_at":"2016-10-26T12:19:49.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e3cbc86e7cdc9d65e68b6a59252efe35032c15c8b6ce77a8e86de88410fc5dc"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 18647ebbe0654a6b09f08d4ebcd4b21da7150b99bff86b5c97ddf8c742ce9c5e
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
      "course_id": 297,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T12:29:54.705Z",
      "course_published": true,
      "updated_at": "2016-10-26T12:29:54.697Z"
    },
    {
      "id": 5,
      "course_id": 298,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-26T12:29:54.781Z",
      "course_published": true,
      "updated_at": "2016-10-26T12:29:54.774Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18647ebbe0654a6b09f08d4ebcd4b21da7150b99bff86b5c97ddf8c742ce9c5e"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer f1997343323ef3c8f45f610a8a810f03affd06a14625dcb016880f9afb3d322d
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
    "course_id": 300,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-26T12:29:55.032Z",
    "course_published": true,
    "updated_at": "2016-10-26T12:29:55.023Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1997343323ef3c8f45f610a8a810f03affd06a14625dcb016880f9afb3d322d"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 2f96c099505b498cd7e5eee790b2a5d153ffddf3dd8f3c12279c34005fb892dd
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
    "course_id": 299,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-26T12:29:54.938Z",
    "course_published": true,
    "updated_at": "2016-10-26T12:29:54.928Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f96c099505b498cd7e5eee790b2a5d153ffddf3dd8f3c12279c34005fb892dd"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer c2f51bbfeade61e96881850ea8f4057ce978187a166c953b6da38784d4725c1e
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
      "votable_id": 131,
      "user_id": 952
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 132,
      "user_id": 952
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 133,
      "user_id": 952
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 134,
      "user_id": 952
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2f51bbfeade61e96881850ea8f4057ce978187a166c953b6da38784d4725c1e"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/3
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
    "id": 3,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 1,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 3
      },
      {
        "id": 2,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 3
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/3" -X GET \
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
      "id": 1,
      "name": "Multi-tiered explicit function",
      "name_translations": {
        "en": "Multi-tiered explicit function"
      }
    },
    {
      "id": 2,
      "name": "Decentralized multi-tasking knowledge base",
      "name_translations": {
        "en": "Decentralized multi-tasking knowledge base"
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
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer 147969e073efd1e67704a597b96ef96240474cc180f2f0707f14db81c496deb1
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
    "id": 27,
    "user_id": 546,
    "feedbackable_id": 69,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-26T12:29:29.391Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 147969e073efd1e67704a597b96ef96240474cc180f2f0707f14db81c496deb1"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/4/fix
Content-Type: application/json
Authorization: Bearer bebbbecf3c7d90434917809ab97868f3a609c53baf412317ad47ce37ea31e3b1
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
    "user_id": 443,
    "feedbackable_id": 65,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-26T12:29:22.475Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/4/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bebbbecf3c7d90434917809ab97868f3a609c53baf412317ad47ce37ea31e3b1"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer 401eb8462f468ea5c2567b049793d31bfc0e788dae3df2a2ed5c40e2a75c47fe
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
    "user_id": 448,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T12:29:22.844Z",
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
	-H "Authorization: Bearer 401eb8462f468ea5c2567b049793d31bfc0e788dae3df2a2ed5c40e2a75c47fe"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/1/fix
Content-Type: application/json
Authorization: Bearer 1154f0c240bdc8ed99e3c514eca319e8eb1781239e7b867a7351e8079cb513c1
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
	-H "Authorization: Bearer 1154f0c240bdc8ed99e3c514eca319e8eb1781239e7b867a7351e8079cb513c1"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/2/fix
Content-Type: application/json
Authorization: Bearer 749bbe19de3c24b53d54f81218f5db9d59a61d69323ff2b6d20d055da796fd31
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
	-H "Authorization: Bearer 749bbe19de3c24b53d54f81218f5db9d59a61d69323ff2b6d20d055da796fd31"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/close
Content-Type: application/json
Authorization: Bearer 0afa8fecadfacf200f0e2cc8fe179fa4f19fb317f10f9d5c16e8ff4b7c9919de
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
	-H "Authorization: Bearer 0afa8fecadfacf200f0e2cc8fe179fa4f19fb317f10f9d5c16e8ff4b7c9919de"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/6
Content-Type: application/json
Authorization: Bearer e25ec44c626b2b41fa324ebf451605913bf12a4f82edad73d5b28b6db14340cb
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
    "user_id": 453,
    "feedbackable_id": 67,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T12:29:23.145Z",
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
	-H "Authorization: Bearer e25ec44c626b2b41fa324ebf451605913bf12a4f82edad73d5b28b6db14340cb"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 5292d59d07ddba28d3e9c251b120a83809cb928d829060be507248dd229f1662
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
	-H "Authorization: Bearer 5292d59d07ddba28d3e9c251b120a83809cb928d829060be507248dd229f1662"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/13/bookmark
Content-Type: application/json
Authorization: Bearer 418de99ec83ed388a6eb1b13f9e9c37cab7b62b3841681d39e5f3d69cbe29619
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
	-H "Authorization: Bearer 418de99ec83ed388a6eb1b13f9e9c37cab7b62b3841681d39e5f3d69cbe29619"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer 5c0bffa00a439d2921214f5dc43fd120a8e05c041029a27011212127f2feea67
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
	-H "Authorization: Bearer 5c0bffa00a439d2921214f5dc43fd120a8e05c041029a27011212127f2feea67"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/8
Content-Type: application/json
Authorization: Bearer e2472b8e3e6fd3107825e988c8bf05412ab511b49f0d0a4dd9258f18f7c0eabe
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/79edbe719d4f440e8e67506c9e938d2a.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T122909Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=6e55636984f583c4a15047b4e63ae9e9e96f5071d78fffb30d6e3ff72c8287c7",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2472b8e3e6fd3107825e988c8bf05412ab511b49f0d0a4dd9258f18f7c0eabe"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/3/preview
Content-Type: application/json
Authorization: Bearer 6d0bbadcd444f13e841e1a231cdff89b59f0fb1c82bb2e5c6ba4880236bf602a
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/c1fe06f25c87043dfbc923a532ad6203.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161026%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161026T122909Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=0b9138e3ccf626264b9bfc58a5a3515c974beac92e9892eb390b22fc8dd86f7b",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/3/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d0bbadcd444f13e841e1a231cdff89b59f0fb1c82bb2e5c6ba4880236bf602a"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Content-Type: application/json
Authorization: Bearer 9ae76836f673f4c6ce6f57c3d8fa2872894a9914c3a4e2921c60844112e6d4c3
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
    "id": 5,
    "uploader": {
      "id": 319,
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
      "created_at": "2016-10-26T12:29:09.467Z",
      "updated_at": "2016-10-26T12:29:09.467Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-26T12:29:09.539Z",
    "updated_at": "2016-10-26T12:29:09.539Z",
    "course_id": 117,
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
curl "api.goskive.com/v2/files/5/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ae76836f673f4c6ce6f57c3d8fa2872894a9914c3a4e2921c60844112e6d4c3"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer af973eaf8fe8a3860844924fcde28a9d6baa88069d865a69e011396668ccda15
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
      "creator_id": 121,
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 38,
      "additional_university_ids": [

      ],
      "topic_id": 43,
      "discipline_id": 44,
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
      "chapters_updated_at": "2016-10-26T12:28:47.232Z",
      "updated_at": "2016-10-26T12:28:48.794Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 126,
      "id": 39,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-b806fb7a-a2d9-45fc-882c-2ef286087183",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-b806fb7a-a2d9-45fc-882c-2ef286087183",
      "slug": "mit-the-great-british-bake-off-b806fb7a-a2d9-45fc-882c-2ef286087183",
      "university_id": 39,
      "additional_university_ids": [

      ],
      "topic_id": 44,
      "discipline_id": 45,
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
      "chapters_updated_at": "2016-10-26T12:28:47.232Z",
      "updated_at": "2016-10-26T12:28:49.334Z",
      "shortname": "mit-the-great-british-bake-off-b806fb7a-a2d9-45fc-882c-2ef286087183"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer af973eaf8fe8a3860844924fcde28a9d6baa88069d865a69e011396668ccda15"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/12/report
Content-Type: application/json
Authorization: Bearer e28248bd25a965877b672c526f1b9781e76f4ce52589fb7355e1f778181c1517
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e28248bd25a965877b672c526f1b9781e76f4ce52589fb7355e1f778181c1517"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/7/bookmark
Content-Type: application/json
Authorization: Bearer f69a98340fb18d8765af886955ed97f9cce07d3db4f909cbdd03fa327aa40cd0
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f69a98340fb18d8765af886955ed97f9cce07d3db4f909cbdd03fa327aa40cd0"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/81/comments
Content-Type: application/json
Authorization: Bearer 1ce2d14ae546555063512fbacef91192fd9826852bfcd4a5592f512644043ec3
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
    "id": 52,
    "author_id": 820,
    "reply_to_id": null,
    "created_at": "2016-10-26T12:29:46.665Z",
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
curl "api.goskive.com/v2/flashcards/81/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ce2d14ae546555063512fbacef91192fd9826852bfcd4a5592f512644043ec3"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/80/comments
Content-Type: application/json
Authorization: Bearer ed792230d5573753648aaf4e93bb1efe3193b94cfdfe6f8be09d30807e6af349
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
    "author_id": 817,
    "reply_to_id": null,
    "created_at": "2016-10-26T12:29:46.353Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 817,
      "feedbackable_id": 80,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:46.350Z",
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
curl "api.goskive.com/v2/flashcards/80/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed792230d5573753648aaf4e93bb1efe3193b94cfdfe6f8be09d30807e6af349"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/79/comments
Content-Type: application/json
Authorization: Bearer ee800449067f395da1cf5a2a38b4701d5fd0e679a4fad5ed4e98214672d2ff82
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
      "id": 49,
      "author_id": 815,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:46.135Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 816,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:46.151Z",
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
curl "api.goskive.com/v2/flashcards/79/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee800449067f395da1cf5a2a38b4701d5fd0e679a4fad5ed4e98214672d2ff82"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/82/comments
Content-Type: application/json
Authorization: Bearer f211afd0c0a839996842576e9eb51c29cfb1ebf703a56a01732f0c8a6440c16b
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
curl "api.goskive.com/v2/flashcards/82/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f211afd0c0a839996842576e9eb51c29cfb1ebf703a56a01732f0c8a6440c16b"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/90/feedbacks
Content-Type: application/json
Authorization: Bearer dd535cedb7bdfd81feace3577a4ac87c88dfb3bbb6c3e45a75686a521cda867b
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
    "id": 46,
    "user_id": 892,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-26T12:29:50.998Z",
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
curl "api.goskive.com/v2/flashcards/90/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd535cedb7bdfd81feace3577a4ac87c88dfb3bbb6c3e45a75686a521cda867b"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/87/feedbacks
Content-Type: application/json
Authorization: Bearer 0c8c33952a6aad8cd03762e38b0458e69d5631bd4384d37e36d3665cd7e0b0db
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
      "user_id": 885,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:50.305Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 884,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:50.294Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c8c33952a6aad8cd03762e38b0458e69d5631bd4384d37e36d3665cd7e0b0db"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/60/votes
Content-Type: application/json
Authorization: Bearer de45a3d7bf4a90b7233a348472de63c2bb2a7d3a9b531dd6639938ac4901344a
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
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 60,
      "user_id": 409
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 60,
      "user_id": 408
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 60,
      "user_id": 407
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/60/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de45a3d7bf4a90b7233a348472de63c2bb2a7d3a9b531dd6639938ac4901344a"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/4/republish
Content-Type: application/json
Authorization: Bearer 6f3c99e21b0cc2bb3fa3101ef6ae76de2304ab3879d9525da3663e21c17765d5
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
curl "api.goskive.com/v2/flashcards/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f3c99e21b0cc2bb3fa3101ef6ae76de2304ab3879d9525da3663e21c17765d5"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/2/bookmark
Content-Type: application/json
Authorization: Bearer 31c77a320e898aee6b3c11f631ef1cc4e5e8375239dadb395b75200ed69d2703
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/2/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31c77a320e898aee6b3c11f631ef1cc4e5e8375239dadb395b75200ed69d2703"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/1
Content-Type: application/json
Authorization: Bearer 9d2714626e2c996d1b0b9c77e410ced8b3ad3308371e59b6cd33c1fe31223e7a
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d2714626e2c996d1b0b9c77e410ced8b3ad3308371e59b6cd33c1fe31223e7a"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/24/downvote
Content-Type: application/json
Authorization: Bearer 5c85446a747d92011023526e308c43042057bdef7ad2c44714b188526399da25
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/24/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c85446a747d92011023526e308c43042057bdef7ad2c44714b188526399da25"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/6
Content-Type: application/json
Authorization: Bearer 7e6f1b6e39c48ca0336dac7389a7c56ca5b71554b8b7630da1652c3d45d5c99f
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
    "id": 6,
    "obfuscated_id": "eyxYPTvoIb8",
    "author_id": 16,
    "chapter_id": 6,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:41.561Z",
    "created_at": "2016-10-26T12:28:41.561Z",
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
curl "api.goskive.com/v2/flashcards/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7e6f1b6e39c48ca0336dac7389a7c56ca5b71554b8b7630da1652c3d45d5c99f"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/22/report
Content-Type: application/json
Authorization: Bearer 5ae459d665583843c7b7fcdb3429ada76889141dc6c46257f14ac6e2b1cce1b3
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/22/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ae459d665583843c7b7fcdb3429ada76889141dc6c46257f14ac6e2b1cce1b3"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/5/bookmark
Content-Type: application/json
Authorization: Bearer 7a62f42f145dd35a367450a49d0542d9b7ced9d0b12b5d09997839cd102208bc
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/5/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a62f42f145dd35a367450a49d0542d9b7ced9d0b12b5d09997839cd102208bc"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/23/upvote
Content-Type: application/json
Authorization: Bearer 56eb7fd98d2ff7b3ddd881ca51775795226beda61b4ae2a9feb0875890861049
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/23/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56eb7fd98d2ff7b3ddd881ca51775795226beda61b4ae2a9feb0875890861049"
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
    "key": "cache/f812cf97777be1d9d3ebea1a4b23fe8f.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNlQxMzoyODo0OVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Y4MTJjZjk3Nzc3YmUxZDlkM2ViZWExYTRiMjNmZThmLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNi9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjZUMTIyODQ5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161026/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161026T122849Z",
    "x-amz-signature": "882da74f26a2fb888cebe87669c77d9410eaef2820b842c15c9a677f5f9341b9"
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
Authorization: Bearer 6dbd2af2bf42ef3b0c75f4bfc4b4180179bae4b7fd3110af6f244186e59dc340
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
	-H "Authorization: Bearer 6dbd2af2bf42ef3b0c75f4bfc4b4180179bae4b7fd3110af6f244186e59dc340"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 3ae38ca776ab0c333f861ffddc8e3ecb1edb27e215093ee71cae5b0dbf056877
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
	-H "Authorization: Bearer 3ae38ca776ab0c333f861ffddc8e3ecb1edb27e215093ee71cae5b0dbf056877"
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
{"password":{"reset_password_token":"uuHnUuqpNtHFNSeE_YC6","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 226,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-26T12:28:59.384Z",
  "updated_at": "2016-10-26T12:28:59.526Z",
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
  "audit_id": 3704
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"uuHnUuqpNtHFNSeE_YC6","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/104/comments
Content-Type: application/json
Authorization: Bearer be768b75f60b2df78a84637f8b5d3e39e49bad651e471a1de1925062c789415c
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
    "id": 43,
    "author_id": 751,
    "reply_to_id": null,
    "created_at": "2016-10-26T12:29:40.837Z",
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
curl "api.goskive.com/v2/questions/104/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be768b75f60b2df78a84637f8b5d3e39e49bad651e471a1de1925062c789415c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/106/comments
Content-Type: application/json
Authorization: Bearer 188f9ac6a068e420a29eaea9acbd5066bfeb43b68f783ac23ae051ccc1e03b3c
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
    "id": 44,
    "author_id": 757,
    "reply_to_id": null,
    "created_at": "2016-10-26T12:29:41.631Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 29,
      "user_id": 757,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:41.628Z",
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
curl "api.goskive.com/v2/questions/106/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 188f9ac6a068e420a29eaea9acbd5066bfeb43b68f783ac23ae051ccc1e03b3c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/107/comments
Content-Type: application/json
Authorization: Bearer c101f6895df533e53d51a8b8eb2436005c48d9d988b2a45ebfb809a81f16bcdf
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
      "id": 46,
      "author_id": 764,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:42.093Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 763,
      "reply_to_id": null,
      "created_at": "2016-10-26T12:29:42.077Z",
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
curl "api.goskive.com/v2/questions/107/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c101f6895df533e53d51a8b8eb2436005c48d9d988b2a45ebfb809a81f16bcdf"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/105/comments
Content-Type: application/json
Authorization: Bearer 0379c6156a3d2ef107bc4bf29d02ed8281b1ff2a9f7b2b9bc31ed8bc36bddc0e
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
curl "api.goskive.com/v2/questions/105/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0379c6156a3d2ef107bc4bf29d02ed8281b1ff2a9f7b2b9bc31ed8bc36bddc0e"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/115/feedbacks
Content-Type: application/json
Authorization: Bearer 6bf866504b7ce01ca2fcad1b5b88dd45ae313b5eafd4d8c891bf400af84a76ea
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
    "user_id": 798,
    "feedbackable_id": 115,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-26T12:29:44.784Z",
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
curl "api.goskive.com/v2/questions/115/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bf866504b7ce01ca2fcad1b5b88dd45ae313b5eafd4d8c891bf400af84a76ea"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/109/feedbacks
Content-Type: application/json
Authorization: Bearer d354450872c1068f9ad22853ef83b414b162a4d73ab8db6ac47f8d46cf14a08d
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
      "user_id": 772,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:42.746Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 771,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T12:29:42.735Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/109/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d354450872c1068f9ad22853ef83b414b162a4d73ab8db6ac47f8d46cf14a08d"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/22/votes
Content-Type: application/json
Authorization: Bearer f9d3a7d6286a16a5eb2b0ae09ebaf70f5f0685d67c57e6ee86c320ce5232840b
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
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 22,
      "user_id": 171
    },
    {
      "id": 5,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 22,
      "user_id": 170
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 22,
      "user_id": 169
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/22/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9d3a7d6286a16a5eb2b0ae09ebaf70f5f0685d67c57e6ee86c320ce5232840b"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/48/republish
Content-Type: application/json
Authorization: Bearer 1331a7b06500fa2bbb0dc8ee63fc88d8ab8b262bd681b6d0c15069341acbd171
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
curl "api.goskive.com/v2/questions/48/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1331a7b06500fa2bbb0dc8ee63fc88d8ab8b262bd681b6d0c15069341acbd171"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/28/bookmark
Content-Type: application/json
Authorization: Bearer 1168e2368913cb171561dd2b2f44d6442a3688f06fafc2204054451f3b992c5c
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/28/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1168e2368913cb171561dd2b2f44d6442a3688f06fafc2204054451f3b992c5c"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/45
Content-Type: application/json
Authorization: Bearer ca4600fbcb3a668640af17dbe1c3ba7e33f5f91b3a0e5108cdd2e96b15a5f2d4
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca4600fbcb3a668640af17dbe1c3ba7e33f5f91b3a0e5108cdd2e96b15a5f2d4"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/50/downvote
Content-Type: application/json
Authorization: Bearer 6b77ec1a5a1ba9a79d082af94da0fce97fe777e409285137a77b20bc4791bfea
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b77ec1a5a1ba9a79d082af94da0fce97fe777e409285137a77b20bc4791bfea"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/51
Content-Type: application/json
Authorization: Bearer 89d0320f5e551f5bc040ca18f245e98afa492fc8335eb29278c8c3b826534a4d
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
    "id": 51,
    "obfuscated_id": "fXx2Zpse_KI",
    "author_id": 305,
    "chapter_id": 73,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:29:08.585Z",
    "created_at": "2016-10-26T12:29:08.472Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 105,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 106,
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
curl "api.goskive.com/v2/questions/51" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89d0320f5e551f5bc040ca18f245e98afa492fc8335eb29278c8c3b826534a4d"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/46/report
Content-Type: application/json
Authorization: Bearer 4306265156bff2418a5f4da12a0816e5507be9cf03540c090e3213318c9daac1
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4306265156bff2418a5f4da12a0816e5507be9cf03540c090e3213318c9daac1"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/49/bookmark
Content-Type: application/json
Authorization: Bearer 4f43e240bb8cd7f10691656e8a3add6e2c2abf07980a4c7ba86d36757433e1cb
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/49/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f43e240bb8cd7f10691656e8a3add6e2c2abf07980a4c7ba86d36757433e1cb"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/27
Content-Type: application/json
Authorization: Bearer 257ae91981bb52c4830282a114b3124f52fcdd3f160f4207d09625ff131b36a3
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":27,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T12:28:59.652Z","updated_at":"2016-10-26T12:28:59.791Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":49,"author_id":228,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 27,
    "obfuscated_id": "sJgVCs3QBfA",
    "author_id": 228,
    "chapter_id": 49,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-26T12:28:59.914Z",
    "created_at": "2016-10-26T12:28:59.652Z",
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
    "question": "{\"id\"=>27, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-26T12:28:59.652Z\", \"updated_at\"=>\"2016-10-26T12:28:59.791Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>49, \"author_id\"=>228, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 56,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 57,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 58,
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
curl "api.goskive.com/v2/questions/27" -d '{"question":{"question":{"id":27,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-26T12:28:59.652Z","updated_at":"2016-10-26T12:28:59.791Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":49,"author_id":228,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 257ae91981bb52c4830282a114b3124f52fcdd3f160f4207d09625ff131b36a3"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/44/upvote
Content-Type: application/json
Authorization: Bearer d0190d2fc18410888ea23d70d83fa27524ba87a2e4077e8e568113199131b517
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/44/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0190d2fc18410888ea23d70d83fa27524ba87a2e4077e8e568113199131b517"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer f655ea4658ddee81db8eff00471c07c126f6b3691e73d9d0c047f95325819ff7
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
      "creator_id": 420,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 137,
      "additional_university_ids": [

      ],
      "topic_id": 158,
      "discipline_id": 159,
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
      "updated_at": "2016-10-26T12:29:20.951Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f655ea4658ddee81db8eff00471c07c126f6b3691e73d9d0c047f95325819ff7"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer df72e69dd33144af49644b132436baa6b0fe55e4deb635c587d3b4bb5a75fc4c
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
      "self_url": "http://api.goskive.test/api/v2/universities/uni-115",
      "html_url": "https://goskive.com/university/uni-115",
      "slug": "uni-115",
      "name": "National School of Pizza",
      "short_name": "Uni 115",
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
      "updated_at": "2016-10-26T12:29:20.740Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 134,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-114",
      "html_url": "https://goskive.com/university/uni-114",
      "slug": "uni-114",
      "name": "National School of Pastry",
      "short_name": "Uni 114",
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
      "updated_at": "2016-10-26T12:29:20.724Z",
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
	-H "Authorization: Bearer df72e69dd33144af49644b132436baa6b0fe55e4deb635c587d3b4bb5a75fc4c"
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
      "id": 4,
      "name": "Quality-focused holistic firmware",
      "name_translations": {
        "en": "Quality-focused holistic firmware"
      },
      "discipline_id": 5
    },
    {
      "id": 5,
      "name": "Right-sized user-facing infrastructure",
      "name_translations": {
        "en": "Right-sized user-facing infrastructure"
      },
      "discipline_id": 6
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
GET /v2/topics/3
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
    "id": 3,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 4
  }
}
```



```shell
curl "api.goskive.com/v2/topics/3" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer ec92986e5c41ce02547b4ea04e5b445eb87d689e6f722a78c0da245f6096c18f
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
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-78",
      "html_url": "https://goskive.com/university/uni-78",
      "slug": "uni-78",
      "name": "University 66",
      "short_name": "Uni 78",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dd45b8e274d1d0e55b5afff67d218d948442eaca.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ed3aed27ec2abf05787537f4c8572fb9080bbebf.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T12:29:09.030Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-77",
      "html_url": "https://goskive.com/university/uni-77",
      "slug": "uni-77",
      "name": "University 65",
      "short_name": "Uni 77",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dc8f2469ecddd5af6505d9db2042b45f53ad683e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c9a133dca397548adb89a35bebfdaee19823cf8d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T12:29:09.014Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-76",
      "html_url": "https://goskive.com/university/uni-76",
      "slug": "uni-76",
      "name": "University 64",
      "short_name": "Uni 76",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3587f09ccbcc321f7f63c35b7e737171f83e68af.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a71c5926eacc7efc335b877c4910cd8c4e3565b7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-26T12:29:08.998Z",
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
	-H "Authorization: Bearer ec92986e5c41ce02547b4ea04e5b445eb87d689e6f722a78c0da245f6096c18f"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 1ef7263e49ed0f37eeac9569d74d36cc339ee0d698d001252a2d7b26c7f9aa24
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
    "id": 98,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/070d79cba40171651c2b94b5973daa5e481d8e8b.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/996ac5a0409fd87fb7916cf000c978b3cfba5a20.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-26T12:29:09.145Z",
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
	-H "Authorization: Bearer 1ef7263e49ed0f37eeac9569d74d36cc339ee0d698d001252a2d7b26c7f9aa24"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ceb46aaa2465ebcdc62e0a7ce76bf2ff86cba78d246422f40a64161c40f98d7a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":58,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 173,
    "id": 51,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 52,
    "additional_university_ids": [

    ],
    "topic_id": 58,
    "discipline_id": 59,
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
    "chapters_updated_at": "2016-10-26T12:28:53.847Z",
    "updated_at": "2016-10-26T12:28:53.977Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 42,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-26T12:28:53.934Z",
        "course_id": 51,
        "author_id": 173,
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
        "id": 43,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-26T12:28:53.951Z",
        "course_id": 51,
        "author_id": 173,
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
        "id": 44,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-26T12:28:53.967Z",
        "course_id": 51,
        "author_id": 173,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":58,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ceb46aaa2465ebcdc62e0a7ce76bf2ff86cba78d246422f40a64161c40f98d7a"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9e73a6592c7a597425f52628bee17ee268033e5f1a0246e76430ca31f75ba901
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":59,"published":false}}
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
    "creator_id": 174,
    "id": 52,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 53,
    "additional_university_ids": [

    ],
    "topic_id": 59,
    "discipline_id": 60,
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
    "updated_at": "2016-10-26T12:28:54.120Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":59,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e73a6592c7a597425f52628bee17ee268033e5f1a0246e76430ca31f75ba901"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9cad58c2bf7386e5f1ebbb2348902d15563e4e84ac853805e86d54dd886ff7d6
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
      "creator_id": 177,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-34",
      "html_url": "https://goskive.com/course/fu-course-34",
      "slug": "fu-course-34",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 63,
      "discipline_id": 64,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 34",
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
      "updated_at": "2016-10-26T12:28:54.437Z",
      "shortname": "fu-course-34"
    },
    {
      "creator_id": 177,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-35",
      "html_url": "https://goskive.com/course/fu-course-35",
      "slug": "fu-course-35",
      "university_id": 55,
      "additional_university_ids": [

      ],
      "topic_id": 64,
      "discipline_id": 65,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 35",
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
      "chapters_updated_at": "2016-10-26T12:28:54.742Z",
      "updated_at": "2016-10-26T12:28:54.749Z",
      "shortname": "fu-course-35"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cad58c2bf7386e5f1ebbb2348902d15563e4e84ac853805e86d54dd886ff7d6"
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
      "creator_id": 207,
      "id": 80,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 64,
      "additional_university_ids": [

      ],
      "topic_id": 87,
      "discipline_id": 88,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
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
      "updated_at": "2016-10-26T12:28:56.947Z",
      "shortname": "fu-course-58"
    },
    {
      "creator_id": 207,
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 64,
      "additional_university_ids": [

      ],
      "topic_id": 88,
      "discipline_id": 89,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 59",
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
      "chapters_updated_at": "2016-10-26T12:28:57.245Z",
      "updated_at": "2016-10-26T12:28:57.252Z",
      "shortname": "fu-course-59"
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
Authorization: Bearer fa38d23abfeac71c36fc8c4e7c717e996729175b7e83e25aa5ce6ec58ffe01a7
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
      "creator_id": 183,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-38",
      "html_url": "https://goskive.com/course/fu-course-38",
      "slug": "fu-course-38",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 67,
      "discipline_id": 68,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 38",
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
      "updated_at": "2016-10-26T12:28:54.967Z",
      "shortname": "fu-course-38"
    },
    {
      "creator_id": 183,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-39",
      "html_url": "https://goskive.com/course/fu-course-39",
      "slug": "fu-course-39",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 68,
      "discipline_id": 69,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 39",
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
      "updated_at": "2016-10-26T12:28:55.005Z",
      "shortname": "fu-course-39"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa38d23abfeac71c36fc8c4e7c717e996729175b7e83e25aa5ce6ec58ffe01a7"
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
      "creator_id": 212,
      "id": 84,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-62",
      "html_url": "https://goskive.com/course/fu-course-62",
      "slug": "fu-course-62",
      "university_id": 66,
      "additional_university_ids": [

      ],
      "topic_id": 91,
      "discipline_id": 92,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 62",
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
      "updated_at": "2016-10-26T12:28:57.443Z",
      "shortname": "fu-course-62"
    },
    {
      "creator_id": 212,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-63",
      "html_url": "https://goskive.com/course/fu-course-63",
      "slug": "fu-course-63",
      "university_id": 66,
      "additional_university_ids": [

      ],
      "topic_id": 92,
      "discipline_id": 93,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 63",
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
      "updated_at": "2016-10-26T12:28:57.478Z",
      "shortname": "fu-course-63"
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
Authorization: Bearer 5245932a6801df50a39a4c4bdee6e4efe00e6d199074aebd3acaeb2d327d3933
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
  "id": 308,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-26T12:29:08.755Z",
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
	-H "Authorization: Bearer 5245932a6801df50a39a4c4bdee6e4efe00e6d199074aebd3acaeb2d327d3933"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/156
Content-Type: application/json
Authorization: Bearer 52907b642ebb03064aa25f3048bac17f9385cd07e69997d2c9d6070941c8affc
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
    "id": 156,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 47,
    "fields_of_study": [
      52,
      53
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-26T12:28:52.239Z",
    "updated_at": "2016-10-26T12:28:52.239Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/156" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52907b642ebb03064aa25f3048bac17f9385cd07e69997d2c9d6070941c8affc"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/158
Content-Type: application/json
Authorization: Bearer 7f3697757f22b0cdd1e5776804bf31f4f6d34f40c73c369ae238944088ead368
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
    "id": 158,
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
    "created_at": "2016-10-26T12:28:52.321Z",
    "updated_at": "2016-10-26T12:28:52.321Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/158" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f3697757f22b0cdd1e5776804bf31f4f6d34f40c73c369ae238944088ead368"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/13
Content-Type: application/json
Authorization: Bearer 891f113d8a166a098e6a22cb76ca58d32e41163d531e504c55165d88b3fe8547
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 891f113d8a166a098e6a22cb76ca58d32e41163d531e504c55165d88b3fe8547"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/15
Content-Type: application/json
Authorization: Bearer 3c7a0ca430e7a40b0d652a18ed3d9d7823ac4e190c7946b05b1985c6c7548cc3
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
    "id": 15,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 103,
    "user_id": 741
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c7a0ca430e7a40b0d652a18ed3d9d7823ac4e190c7946b05b1985c6c7548cc3"
```
