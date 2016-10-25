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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c1284fd2e35f3b0a2ea697de7151777afbe18e8f7dcdbc4df656d82f3e20dc4b","client_secret":"61f6073dd57918943a6e8362957819370ef0717b095e7c5f734aacb7d9d6e5db"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"c1284fd2e35f3b0a2ea697de7151777afbe18e8f7dcdbc4df656d82f3e20dc4b","client_secret":"61f6073dd57918943a6e8362957819370ef0717b095e7c5f734aacb7d9d6e5db"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZjkyNTlhNGE0NGM0MmFhNmRjMDBiN2M2NzU2OGI2ODc1MTdmODBlMjYyZDk5
NTlmODc2YTBhMjczNzE1ZWE3YzowOGYzN2YwNDQzNTIyZWQzMDcwYjRhNjli
NDNjMTVkNmY5MDc0ZWQ5YTcwMmRkMzhhMGIzZWI5ZWM3ZTcxYTJl

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
	-u f9259a4a44c42aa6dc00b7c67568b687517f80e262d9959f876a0a273715ea7c:08f37f0443522ed3070b4a69b43c15d6f9074ed9a702dd38a0b3eb9ec7e71a2e
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e80c53d4efc9f7ea0f26ce436632873a4f7641cf5395d6f15866361156723997","client_secret":"8eba619d6f594317315f87bb63860d05b6deb79d90e23573aca6f76aac7e524f"}
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
  "access_token": "8fee15a3893871d660f6443e43d59bea2e2a85cdb8507670ac888975e0b0dbbe",
  "token_type": "bearer",
  "created_at": 1477387711
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"e80c53d4efc9f7ea0f26ce436632873a4f7641cf5395d6f15866361156723997","client_secret":"8eba619d6f594317315f87bb63860d05b6deb79d90e23573aca6f76aac7e524f"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTE2NDBjNzNhYmQzZDUxZGI5ZjU2ODIyOGE1MWExOWU4YmVkNjEyYmI5NDVm
MTk0MWM3YjliNzA0YTZhYzIzMzozOWE4YThjODVjNzQyMzAxNDA2ODUxODI2
NGZhMmM1ODQxMzQ3N2JkNDhiYTI0MzU5YWU5ZTM0YmM2N2Y3OTA2

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
  "access_token": "ccfa35e2f6faf5df0abf7d89530cf96279f4509899c500be0e07157a4ed32cea",
  "token_type": "bearer",
  "created_at": 1477387711
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u a1640c73abd3d51db9f568228a51a19e8bed612bb945f1941c7b9b704a6ac233:39a8a8c85c7423014068518264fa2c58413477bd48ba24359ae9e34bc67f7906
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
{"grant_type":"client_credentials","client_id":"3ab109e7028c71f9ddcf046076788631af1e490bbae8365891759bd3ece2b699","client_secret":"d849f92bc14ab98906e69b4983301a74984c3f5c5c76db3d44c6d9c39ee4bfb5"}
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
  "access_token": "2a99d2324790a0d53f3786ecc17f9eca8a7d750c10c443807ab3cc217eb1fb24",
  "token_type": "bearer",
  "created_at": 1477387711
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"3ab109e7028c71f9ddcf046076788631af1e490bbae8365891759bd3ece2b699","client_secret":"d849f92bc14ab98906e69b4983301a74984c3f5c5c76db3d44c6d9c39ee4bfb5"}' -X POST \
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
Authorization: Bearer bc1b77085e23ccd5278155cda867259b5faa39ab8b581268fd8d0fb6ee7fa315
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
	-H "Authorization: Bearer bc1b77085e23ccd5278155cda867259b5faa39ab8b581268fd8d0fb6ee7fa315"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/3/flashcards
Content-Type: application/json
Authorization: Bearer 02da3e515064057ad3a6881240a00260e1ac070e92656e64d35fc902480d976c
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":3,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 4,
    "obfuscated_id": "SaV_gL1ycAY",
    "author_id": 9,
    "chapter_id": 3,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:27:51.057Z",
    "created_at": "2016-10-25T09:27:51.057Z",
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
curl "api.goskive.com/v2/chapters/3/flashcards" -d '{"flashcard":{"chapter_id":3,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02da3e515064057ad3a6881240a00260e1ac070e92656e64d35fc902480d976c"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/2/flashcards
Content-Type: application/json
Authorization: Bearer c66a5eae02fdf28ae36d9a0fc0e6b1d510ee5ada22017da2945066dce4f06388
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
      "id": 1,
      "obfuscated_id": "vnOJWgI0jGc",
      "author_id": 4,
      "chapter_id": 2,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:27:50.767Z",
      "created_at": "2016-10-25T09:27:50.767Z",
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
      "id": 2,
      "obfuscated_id": "yHhUU9c1C7Y",
      "author_id": 4,
      "chapter_id": 2,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:27:50.808Z",
      "created_at": "2016-10-25T09:27:50.808Z",
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
      "id": 3,
      "obfuscated_id": "bco7bNtr_d4",
      "author_id": 4,
      "chapter_id": 2,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:27:50.844Z",
      "created_at": "2016-10-25T09:27:50.844Z",
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
curl "api.goskive.com/v2/chapters/2/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c66a5eae02fdf28ae36d9a0fc0e6b1d510ee5ada22017da2945066dce4f06388"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/108/questions
Content-Type: application/json
Authorization: Bearer e18483eeb76cd0f38373f556317353856a77d14510dd0d2abf6c83d5ff731b7d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":108,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 73,
    "obfuscated_id": "LJvjpBojvP0",
    "author_id": 515,
    "chapter_id": 108,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:34.915Z",
    "created_at": "2016-10-25T09:28:34.915Z",
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
        "id": 146,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 147,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 148,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 149,
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
curl "api.goskive.com/v2/chapters/108/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":108,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e18483eeb76cd0f38373f556317353856a77d14510dd0d2abf6c83d5ff731b7d"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/109/questions
Content-Type: application/json
Authorization: Bearer 55e6ed4a8e0aceff8385cea236e6690eb6178c5604da46d04e966bdcb2273fd8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":109,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 74,
    "obfuscated_id": "fL3buOIYvUI",
    "author_id": 518,
    "chapter_id": 109,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:35.459Z",
    "created_at": "2016-10-25T09:28:35.459Z",
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
        "id": 150,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 151,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/109/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":109,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55e6ed4a8e0aceff8385cea236e6690eb6178c5604da46d04e966bdcb2273fd8"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/110/questions
Content-Type: application/json
Authorization: Bearer b19587b8ff65e359dfb0f2580348ad75746329a326f1909136b1cd2fd91d1157
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":110,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 75,
    "obfuscated_id": "rRYuZazyhgg",
    "author_id": 521,
    "chapter_id": 110,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:35.781Z",
    "created_at": "2016-10-25T09:28:35.781Z",
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
        "id": 152,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 153,
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
curl "api.goskive.com/v2/chapters/110/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":110,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b19587b8ff65e359dfb0f2580348ad75746329a326f1909136b1cd2fd91d1157"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/107/questions
Content-Type: application/json
Authorization: Bearer 3d0b343d02a8572bca23603e706d4148c3573df5c8bb7c30c69c0aace3147002
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":107,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 512,
    "chapter_id": 107,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:34.343Z",
    "created_at": "2016-10-25T09:28:34.343Z",
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
curl "api.goskive.com/v2/chapters/107/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":107,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d0b343d02a8572bca23603e706d4148c3573df5c8bb7c30c69c0aace3147002"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/111/questions
Content-Type: application/json
Authorization: Bearer 7ec99ef045228d057eadfdcdeca0504f75bbd93462251a1116754667a075e5f2
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 524,
      "chapter_id": 111,
      "position": 72,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:36.215Z",
      "created_at": "2016-10-25T09:28:36.101Z",
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 525,
      "chapter_id": 111,
      "position": 73,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:36.402Z",
      "created_at": "2016-10-25T09:28:36.286Z",
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 526,
      "chapter_id": 111,
      "position": 74,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T09:28:36.592Z",
      "created_at": "2016-10-25T09:28:36.473Z",
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
curl "api.goskive.com/v2/chapters/111/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ec99ef045228d057eadfdcdeca0504f75bbd93462251a1116754667a075e5f2"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/119
Content-Type: application/json
Authorization: Bearer 1f1b8270fdfa72f6262c416fdc8eb3eefce7d9283e24c660efa6b8e245ad3738
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
curl "api.goskive.com/v2/chapters/119" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f1b8270fdfa72f6262c416fdc8eb3eefce7d9283e24c660efa6b8e245ad3738"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/121
Content-Type: application/json
Authorization: Bearer cd73dceb9033cc4e3c5bcf0da1a7041e74dfa782e823fc0b545af09616076cd8
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
curl "api.goskive.com/v2/chapters/121" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd73dceb9033cc4e3c5bcf0da1a7041e74dfa782e823fc0b545af09616076cd8"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/117
Content-Type: application/json
Authorization: Bearer cdd0b6fb83a750237c6b453b911cbb4abd6106cef7ee246f2f02f729ae64b7f7
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
curl "api.goskive.com/v2/chapters/117" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdd0b6fb83a750237c6b453b911cbb4abd6106cef7ee246f2f02f729ae64b7f7"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/118
Content-Type: application/json
Authorization: Bearer ae5fe11533d23fe83312d3f6d77b34edb6064891eedfb8cf4e59dcbf72b23782
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/118" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ae5fe11533d23fe83312d3f6d77b34edb6064891eedfb8cf4e59dcbf72b23782"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/113
Content-Type: application/json
Authorization: Bearer 6c3dc52b0e2a17137561c0940724e62c5665ab06f69b5233b9b9834fdc68723b
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
    "id": 113,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T09:28:38.231Z",
    "course_id": 147,
    "author_id": 542,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-25T09:28:37.713Z",
    "questions_updated_at": "2016-10-25T09:28:37.713Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 546,
        "chapter_id": 113,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.214Z",
        "created_at": "2016-10-25T09:28:38.214Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 544,
        "chapter_id": 113,
        "position": 76,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:38.109Z",
        "created_at": "2016-10-25T09:28:37.993Z",
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
            "id": 162,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 163,
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
curl "api.goskive.com/v2/chapters/113" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c3dc52b0e2a17137561c0940724e62c5665ab06f69b5233b9b9834fdc68723b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/116
Content-Type: application/json
Authorization: Bearer b848b84c735956675ee8a050eb74c3f8f2a82580473670cf8f79eb4c411301fd
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
    "id": 116,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T09:28:39.221Z",
    "course_id": 150,
    "author_id": 559,
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
curl "api.goskive.com/v2/chapters/116" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b848b84c735956675ee8a050eb74c3f8f2a82580473670cf8f79eb4c411301fd"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/13/replies
Content-Type: application/json
Authorization: Bearer 6661ced112fe165e27ee07272d04d126fa216f89d369a2b6222e38a30fc952e0
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
    "id": 14,
    "author_id": 399,
    "reply_to_id": 13,
    "created_at": "2016-10-25T09:28:26.350Z",
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
curl "api.goskive.com/v2/comments/13/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6661ced112fe165e27ee07272d04d126fa216f89d369a2b6222e38a30fc952e0"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/12/replies
Content-Type: application/json
Authorization: Bearer 856e0e7f7a5f793fa5fee559010d8de3ab41eab6d514df7daef8e8e540363bf2
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
curl "api.goskive.com/v2/comments/12/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 856e0e7f7a5f793fa5fee559010d8de3ab41eab6d514df7daef8e8e540363bf2"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/52
Content-Type: application/json
Authorization: Bearer bba010772b37d69864bbf2a2f4bc88557f10a224007c297d6ad1b89c0bbdaa13
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
curl "api.goskive.com/v2/comments/52" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bba010772b37d69864bbf2a2f4bc88557f10a224007c297d6ad1b89c0bbdaa13"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/54/republish
Content-Type: application/json
Authorization: Bearer 76312100aa21813270045c7eb99121debfdd63b9b6eacd7ae5946da9aa0ff21c
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
curl "api.goskive.com/v2/comments/54/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76312100aa21813270045c7eb99121debfdd63b9b6eacd7ae5946da9aa0ff21c"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/51
Content-Type: application/json
Authorization: Bearer d399a42c0aabd63443b863b763afb6667ef7e4fc6ce5d2d12db352ffabc368bc
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d399a42c0aabd63443b863b763afb6667ef7e4fc6ce5d2d12db352ffabc368bc"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/15/report
Content-Type: application/json
Authorization: Bearer d12be9234336f4847e3f9f817dafcf741038fb6c806fb777c9ccb2b988f1f7d6
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
	-H "Authorization: Bearer d12be9234336f4847e3f9f817dafcf741038fb6c806fb777c9ccb2b988f1f7d6"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/13
Content-Type: application/json
Authorization: Bearer e35f591d6580b8455927e37471c0f29616eb45cfd72ad28e7a6babe0e49b8471
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
    "id": 13,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-25T09:28:23.777Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e35f591d6580b8455927e37471c0f29616eb45cfd72ad28e7a6babe0e49b8471"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer c43e3b398d063fe330d58a42e6d7d1017ecff1b760fa71db0317b75253f028c3
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
      "id": 10,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T09:28:23.660Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T09:28:23.665Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T09:28:23.668Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c43e3b398d063fe330d58a42e6d7d1017ecff1b760fa71db0317b75253f028c3"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/16/company_profiles
Content-Type: application/json
Authorization: Bearer 8f6ad8aa21a95b97fae391aad597495f3507caba90389b40b192f3a91d1a2c13
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
curl "api.goskive.com/v2/companies/16/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f6ad8aa21a95b97fae391aad597495f3507caba90389b40b192f3a91d1a2c13"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/14/company_profiles
Content-Type: application/json
Authorization: Bearer f81ed7465c9b9dedf769cd854a54eb0c1dbe53d4aa2aa853be465cae292f98db
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
curl "api.goskive.com/v2/companies/14/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f81ed7465c9b9dedf769cd854a54eb0c1dbe53d4aa2aa853be465cae292f98db"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 6abe5bf8cd034cabfb13e1947444a87435ed28df7c6fd965a6fb37f713487a82
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
	-H "Authorization: Bearer 6abe5bf8cd034cabfb13e1947444a87435ed28df7c6fd965a6fb37f713487a82"
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
Authorization: Bearer 0db39953471ee6b1ab91194cd28181d28cff7e12b92c889fecbab6d17d8fbcd1
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
	-H "Authorization: Bearer 0db39953471ee6b1ab91194cd28181d28cff7e12b92c889fecbab6d17d8fbcd1"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c180af11f3691595870a90dd92a916c5dbde79d01243e6741bb9938c7530fe47
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
    "id": 191,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T09:29:07.857Z",
    "course_id": 305,
    "author_id": 955,
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
	-H "Authorization: Bearer c180af11f3691595870a90dd92a916c5dbde79d01243e6741bb9938c7530fe47"
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
      "id": 169,
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-25T09:29:05.276Z",
      "course_id": 292,
      "author_id": 905,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 170,
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-25T09:29:05.299Z",
      "course_id": 292,
      "author_id": 906,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 171,
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-25T09:29:05.544Z",
      "course_id": 292,
      "author_id": 907,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T09:29:05.202Z",
      "questions_updated_at": "2016-10-25T09:29:05.202Z",
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
Authorization: Bearer 96a1eebee896730788eded759828a7dbb43282f148d2732f269dd0100ba8cbe3
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
      "title": "Clever Chapter Title 160",
      "position": 1,
      "updated_at": "2016-10-25T09:29:06.584Z",
      "course_id": 298,
      "author_id": 930,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 182,
      "title": "Clever Chapter Title 161",
      "position": 2,
      "updated_at": "2016-10-25T09:29:06.608Z",
      "course_id": 298,
      "author_id": 931,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 183,
      "title": "Clever Chapter Title 162",
      "position": 3,
      "updated_at": "2016-10-25T09:29:06.880Z",
      "course_id": 298,
      "author_id": 932,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T09:29:06.511Z",
      "questions_updated_at": "2016-10-25T09:29:06.511Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96a1eebee896730788eded759828a7dbb43282f148d2732f269dd0100ba8cbe3"
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
      "id": 172,
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-25T09:29:05.661Z",
      "course_id": 293,
      "author_id": 911,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 173,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-25T09:29:05.684Z",
      "course_id": 293,
      "author_id": 912,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 174,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-25T09:29:05.708Z",
      "course_id": 293,
      "author_id": 913,
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
Authorization: Bearer b7755abcd5f7e7b032dab0855ccd0f8027c4a294757356e2f25aa81d4cf17c90
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
      "title": "Clever Chapter Title 163",
      "position": 1,
      "updated_at": "2016-10-25T09:29:07.129Z",
      "course_id": 300,
      "author_id": 939,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 185,
      "title": "Clever Chapter Title 164",
      "position": 2,
      "updated_at": "2016-10-25T09:29:07.152Z",
      "course_id": 300,
      "author_id": 940,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 186,
      "title": "Clever Chapter Title 165",
      "position": 3,
      "updated_at": "2016-10-25T09:29:07.175Z",
      "course_id": 300,
      "author_id": 941,
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
	-H "Authorization: Bearer b7755abcd5f7e7b032dab0855ccd0f8027c4a294757356e2f25aa81d4cf17c90"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 355b9ef053282bd90291315f7172444e7a77e6150b5a911a2915a28ac9353fdb
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
    "course_id": 256,
    "user_id": 783,
    "updated_at": "2016-10-25T09:28:53.855Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 355b9ef053282bd90291315f7172444e7a77e6150b5a911a2915a28ac9353fdb"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer b1b930580777de6707c11d803d752106322e36fdb744a89405cdbfdca3f65ca8
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
      "course_id": 251,
      "user_id": 769,
      "updated_at": "2016-10-25T09:28:53.164Z"
    },
    {
      "id": 3,
      "course_id": 251,
      "user_id": 770,
      "updated_at": "2016-10-25T09:28:53.178Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1b930580777de6707c11d803d752106322e36fdb744a89405cdbfdca3f65ca8"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/248/files
Content-Type: application/json
Authorization: Bearer c7fa4607b6096993c939961a887e15ebca2b39c89834e9ae1017ccdcf966019e
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
      "id": 12,
      "uploader": {
        "id": 760,
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
        "created_at": "2016-10-25T09:28:52.717Z",
        "updated_at": "2016-10-25T09:28:52.717Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T09:28:52.727Z",
      "updated_at": "2016-10-25T09:28:52.727Z",
      "course_id": 248,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 13,
      "uploader": {
        "id": 761,
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
        "created_at": "2016-10-25T09:28:52.735Z",
        "updated_at": "2016-10-25T09:28:52.735Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T09:28:52.743Z",
      "updated_at": "2016-10-25T09:28:52.743Z",
      "course_id": 248,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 762,
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
        "created_at": "2016-10-25T09:28:52.750Z",
        "updated_at": "2016-10-25T09:28:52.750Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T09:28:52.759Z",
      "updated_at": "2016-10-25T09:28:52.759Z",
      "course_id": 248,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/248/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7fa4607b6096993c939961a887e15ebca2b39c89834e9ae1017ccdcf966019e"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/250/files
Content-Type: application/json
Authorization: Bearer d978395e318cfc9e9b11e4b9ac085f47eb5115769fffd6fcaff586f30957fddc
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
    "id": 15,
    "uploader": {
      "id": 767,
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
      "created_at": "2016-10-25T09:28:53.012Z",
      "updated_at": "2016-10-25T09:28:53.012Z"
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
    "created_at": "2016-10-25T09:28:53.040Z",
    "updated_at": "2016-10-25T09:28:53.040Z",
    "course_id": 250,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/250/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d978395e318cfc9e9b11e4b9ac085f47eb5115769fffd6fcaff586f30957fddc"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/247/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 23a5f5f46c806b1f48ad9b7f23e22b116c4799981a96dc05540eab70764e0ced
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
    "key": "cache/5e2dc8fe3c57f5111dd219c7b6e12d7d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxMDoyODo1MloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzVlMmRjOGZlM2M1N2Y1MTExZGQyMTljN2I2ZTEyZDdkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI1VDA5Mjg1MloifV19",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T092852Z",
    "x-amz-signature": "64623df77e45660b2d60feddeabbb85da668871099a342b2d3fb361c7181bafa"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/247/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23a5f5f46c806b1f48ad9b7f23e22b116c4799981a96dc05540eab70764e0ced"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 30556d2ec9dba7860b9a08f350326a102260a885e9e8615364b9564848600826
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
	-H "Authorization: Bearer 30556d2ec9dba7860b9a08f350326a102260a885e9e8615364b9564848600826"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 10e7d60957c406262158149b3007efd9d6843cbc8c55d9b67757588de30bf74d
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
	-H "Authorization: Bearer 10e7d60957c406262158149b3007efd9d6843cbc8c55d9b67757588de30bf74d"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 07b8e510e671e6b2259f156d6f4afd19d5803d1e41ec26e3882909f71292b053
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
	-H "Authorization: Bearer 07b8e510e671e6b2259f156d6f4afd19d5803d1e41ec26e3882909f71292b053"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0e48277319686c1e90b8a79e6ad891867e2010bbe814c37310b93104f09d5469
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
	-H "Authorization: Bearer 0e48277319686c1e90b8a79e6ad891867e2010bbe814c37310b93104f09d5469"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 475708d10d22c62325cacbb0d6eb7402d348475aa7575686757dfad3cc6c1c2b
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
	-H "Authorization: Bearer 475708d10d22c62325cacbb0d6eb7402d348475aa7575686757dfad3cc6c1c2b"
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
    "creator_id": 210,
    "id": 51,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 52,
    "additional_university_ids": [

    ],
    "topic_id": 53,
    "discipline_id": 53,
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
    "chapters_updated_at": "2016-10-25T09:28:08.751Z",
    "updated_at": "2016-10-25T09:28:10.453Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 44,
        "title": "Clever Chapter Title 41",
        "position": 1,
        "updated_at": "2016-10-25T09:28:10.403Z",
        "course_id": 51,
        "author_id": 210,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T09:28:08.751Z",
        "questions_updated_at": "2016-10-25T09:28:08.751Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 45,
        "title": "Clever Chapter Title 42",
        "position": 2,
        "updated_at": "2016-10-25T09:28:10.444Z",
        "course_id": 51,
        "author_id": 210,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T09:28:08.751Z",
        "questions_updated_at": "2016-10-25T09:28:08.751Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 210,
        "chapter_id": 44,
        "position": 43,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:08.982Z",
        "created_at": "2016-10-25T09:28:08.841Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 210,
        "chapter_id": 45,
        "position": 45,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:09.429Z",
        "created_at": "2016-10-25T09:28:09.281Z",
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
Authorization: Bearer 22ddc00fa38289b9960e6bdd0f7d55acdc373ef926da343df5a6625dc9b16f8a
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
    "creator_id": 215,
    "id": 52,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 53,
    "additional_university_ids": [

    ],
    "topic_id": 54,
    "discipline_id": 54,
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
    "chapters_updated_at": "2016-10-25T09:28:10.516Z",
    "updated_at": "2016-10-25T09:28:12.263Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 46,
        "title": "Clever Chapter Title 43",
        "position": 1,
        "updated_at": "2016-10-25T09:28:12.210Z",
        "course_id": 52,
        "author_id": 215,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T09:28:10.516Z",
        "questions_updated_at": "2016-10-25T09:28:10.516Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 47,
        "title": "Clever Chapter Title 44",
        "position": 2,
        "updated_at": "2016-10-25T09:28:12.253Z",
        "course_id": 52,
        "author_id": 215,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T09:28:10.516Z",
        "questions_updated_at": "2016-10-25T09:28:10.516Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 216,
        "chapter_id": 46,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:12.028Z",
        "created_at": "2016-10-25T09:28:12.028Z",
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
        "author_id": 216,
        "chapter_id": 47,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:12.109Z",
        "created_at": "2016-10-25T09:28:12.109Z",
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
        "author_id": 216,
        "chapter_id": 46,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:12.074Z",
        "created_at": "2016-10-25T09:28:12.074Z",
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
        "author_id": 216,
        "chapter_id": 47,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:12.156Z",
        "created_at": "2016-10-25T09:28:12.156Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 216,
        "chapter_id": 46,
        "position": 49,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:10.775Z",
        "created_at": "2016-10-25T09:28:10.625Z",
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
            "id": 97,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 98,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 216,
        "chapter_id": 46,
        "position": 50,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:10.991Z",
        "created_at": "2016-10-25T09:28:10.850Z",
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
            "id": 99,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 100,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 216,
        "chapter_id": 47,
        "position": 51,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:11.242Z",
        "created_at": "2016-10-25T09:28:11.089Z",
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
            "id": 101,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 102,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 52,
        "obfuscated_id": "_rmh4zxMC_8",
        "author_id": 216,
        "chapter_id": 47,
        "position": 52,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T09:28:11.469Z",
        "created_at": "2016-10-25T09:28:11.322Z",
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
            "id": 103,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 104,
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
	-H "Authorization: Bearer 22ddc00fa38289b9960e6bdd0f7d55acdc373ef926da343df5a6625dc9b16f8a"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/48/pin
Content-Type: application/json
Authorization: Bearer 656226974a419792790d0ede336f8360abdf4b4d13d78a68777f3bc7f8cf276b
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/48/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 656226974a419792790d0ede336f8360abdf4b4d13d78a68777f3bc7f8cf276b"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/43/pin
Content-Type: application/json
Authorization: Bearer 9f35eea9d9d82394ff4232ec37651bd992787c10fcf6e7fa71f35877a387efa0
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/43/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f35eea9d9d82394ff4232ec37651bd992787c10fcf6e7fa71f35877a387efa0"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 1df09fa45d9bb9f90fd02ee70d5b719f336276ed4a23a8c41080eae356178e0b
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
    "creator_id": 193,
    "id": 46,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 47,
    "additional_university_ids": [

    ],
    "topic_id": 48,
    "discipline_id": 48,
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
    "updated_at": "2016-10-25T09:28:05.069Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1df09fa45d9bb9f90fd02ee70d5b719f336276ed4a23a8c41080eae356178e0b"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 7c29afe67d19c41b3fa9838e0fd863f59cb9b5d073b8655085d71159a386fe40
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
    "id": 490,
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
    "created_at": "2016-10-25T09:28:31.681Z",
    "updated_at": "2016-10-25T09:28:31.681Z",
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
	-H "Authorization: Bearer 7c29afe67d19c41b3fa9838e0fd863f59cb9b5d073b8655085d71159a386fe40"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer ac6a403b0adfffb909c6cf894c0647550040707b6abbaf65f38cec7bd2dbfded
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[140]}
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
    "id": 492,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      140
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T09:28:32.065Z",
    "updated_at": "2016-10-25T09:28:32.098Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[140]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac6a403b0adfffb909c6cf894c0647550040707b6abbaf65f38cec7bd2dbfded"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer da242e8b3d909d4505077a044d029aecc55805e3b60edabf4d694c483a834a60
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
    "created_at": "2016-10-25T09:28:32.191Z",
    "updated_at": "2016-10-25T09:28:32.191Z",
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
	-H "Authorization: Bearer da242e8b3d909d4505077a044d029aecc55805e3b60edabf4d694c483a834a60"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7db5cf43e055b70f06546a34904e1899c78c6619ac680d8bc333977b50ef8fda
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[143]}
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
      143
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T09:28:32.279Z",
    "updated_at": "2016-10-25T09:28:32.279Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[143]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7db5cf43e055b70f06546a34904e1899c78c6619ac680d8bc333977b50ef8fda"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 49ae64a90cde4fbea97104393b9b97aaf1f9a340075cfe592c54a8390c39de5b
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

139
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
    "id": 491,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/237cefb22966cfd82ab9902b63caca8dfdc35966.jpg",
    "university_id": null,
    "fields_of_study": [
      139
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T09:28:31.763Z",
    "updated_at": "2016-10-25T09:28:32.015Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/2273288400e9637cbabd2d58e542087737e93905.jpg",
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

139
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 49ae64a90cde4fbea97104393b9b97aaf1f9a340075cfe592c54a8390c39de5b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 84eb9145cb1cc6a3cdf3e83c0c2ea9e7710c68740a4e5f88e464fef2f75dd201
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
      "bookmarkable_id": 62,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 63,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 64,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84eb9145cb1cc6a3cdf3e83c0c2ea9e7710c68740a4e5f88e464fef2f75dd201"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 8ee2cf4dd4c15bf47b70c228e677d84f784001f612a42e20ccada68cc798cd11
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
      "company_id": 21,
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
      "id": 4,
      "title": "Campaign 3",
      "company_id": 22,
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
	-H "Authorization: Bearer 8ee2cf4dd4c15bf47b70c228e677d84f784001f612a42e20ccada68cc798cd11"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 0f67e3e11a9f3aa22645f2fa3a6ad157f603714da8adc090b5c43a2449854e5b
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
      "company_id": 17,
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
	-H "Authorization: Bearer 0f67e3e11a9f3aa22645f2fa3a6ad157f603714da8adc090b5c43a2449854e5b"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 44828ea38cb3a3d7aad4b9dda321065060d375944d04d9d72c73ebb9d13d0258
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
      "creator_id": 785,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-200",
      "html_url": "https://goskive.com/course/mit-course-200",
      "slug": "mit-course-200",
      "university_id": 242,
      "additional_university_ids": [

      ],
      "topic_id": 269,
      "discipline_id": 270,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 200",
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
      "updated_at": "2016-10-25T09:28:53.947Z",
      "shortname": "mit-course-200"
    },
    {
      "creator_id": 786,
      "id": 258,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-201",
      "html_url": "https://goskive.com/course/mit-course-201",
      "slug": "mit-course-201",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 270,
      "discipline_id": 271,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 201",
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
      "updated_at": "2016-10-25T09:28:54.026Z",
      "shortname": "mit-course-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44828ea38cb3a3d7aad4b9dda321065060d375944d04d9d72c73ebb9d13d0258"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 16a5c3f350c0debbe5714af5033bbf174eeb7ec5af77eb50ffaecc6cd173f61b
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
      "company_id": 7,
      "company": {
        "id": 7,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T09:28:04.484Z"
      },
      "created_at": "2016-10-25T09:28:04.487Z",
      "updated_at": "2016-10-25T09:28:04.487Z",
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
      "company_id": 8,
      "company": {
        "id": 8,
        "name": "Fake Company Name 7",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T09:28:04.495Z"
      },
      "created_at": "2016-10-25T09:28:04.498Z",
      "updated_at": "2016-10-25T09:28:04.498Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16a5c3f350c0debbe5714af5033bbf174eeb7ec5af77eb50ffaecc6cd173f61b"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 5049bcd6a8383f2bb0612dfb875782872fa32b2817265e87ea03c164e865d23f
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
      "company_id": 3,
      "company": {
        "id": 3,
        "name": "Fake Company Name 2",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/d9c7e5c9c3995932103d150e3b5a086080efc0e7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T09:28:04.278Z"
      },
      "created_at": "2016-10-25T09:28:04.283Z",
      "updated_at": "2016-10-25T09:28:04.283Z",
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
      "company_id": 4,
      "company": {
        "id": 4,
        "name": "Fake Company Name 3",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/24e720f3555e8498c9bf6c7c8a02d8273d9f80fb.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T09:28:04.296Z"
      },
      "created_at": "2016-10-25T09:28:04.299Z",
      "updated_at": "2016-10-25T09:28:04.299Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5049bcd6a8383f2bb0612dfb875782872fa32b2817265e87ea03c164e865d23f"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 4b275c586bd63f48424b2e5c2947a49d8bd22c1408c624009691ac2e1ddd66dc
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
      "id": 13,
      "created_at": "2016-10-25T09:28:50.261Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-10-25T09:28:50.365Z",
      "author_id": "726",
      "thread_subject_id": "238",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 14,
      "created_at": "2016-10-25T09:28:50.353Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-10-25T09:28:50.368Z",
      "author_id": "729",
      "thread_subject_id": "239",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 15,
      "created_at": "2016-10-25T09:28:50.722Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 15,
      "updated_at": "2016-10-25T09:28:50.722Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 16,
      "created_at": "2016-10-25T09:28:51.082Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-25T09:28:51.082Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 17,
      "created_at": "2016-10-25T09:28:51.447Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-25T09:28:51.447Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 18,
      "created_at": "2016-10-25T09:28:51.734Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 93,
      "updated_at": "2016-10-25T09:28:51.734Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 19,
      "created_at": "2016-10-25T09:28:52.029Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 94,
      "updated_at": "2016-10-25T09:28:52.029Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 20,
      "created_at": "2016-10-25T09:28:52.320Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 95,
      "updated_at": "2016-10-25T09:28:52.320Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b275c586bd63f48424b2e5c2947a49d8bd22c1408c624009691ac2e1ddd66dc"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/21
Content-Type: application/json
Authorization: Bearer 0a58148d92057daf807ad5fee503a2de5ce67e4850b38a6f06653aa12a5d796a
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-25T09:18:52.000Z"}}
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
    "id": 21,
    "created_at": "2016-10-25T09:28:52.507Z",
    "read_at": "2016-10-25T09:18:52.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 58,
    "updated_at": "2016-10-25T09:28:52.545Z",
    "author_id": "755",
    "thread_subject_id": "246",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/21" -d '{"notification":{"read_at":"2016-10-25T09:18:52.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a58148d92057daf807ad5fee503a2de5ce67e4850b38a6f06653aa12a5d796a"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 86c1534d6d4e2830b75fae6cdd7cb286a6fcc05fe398d83ddeddd26f8ba7a0fe
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
      "course_id": 93,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T09:28:22.080Z",
      "course_published": true,
      "updated_at": "2016-10-25T09:28:22.071Z"
    },
    {
      "id": 4,
      "course_id": 94,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T09:28:22.162Z",
      "course_published": true,
      "updated_at": "2016-10-25T09:28:22.153Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86c1534d6d4e2830b75fae6cdd7cb286a6fcc05fe398d83ddeddd26f8ba7a0fe"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 30311d2eac4ed5d4e8fc7572e61a01fd2e935bd658b2b3b6960703627fe717ce
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
    "id": 6,
    "course_id": 97,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T09:28:22.517Z",
    "course_published": true,
    "updated_at": "2016-10-25T09:28:22.509Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 30311d2eac4ed5d4e8fc7572e61a01fd2e935bd658b2b3b6960703627fe717ce"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 5b1204889587df854c91a014d29db790a909f22b26f8d185864efe29981fe29a
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
    "course_id": 92,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-25T09:28:21.940Z",
    "course_published": true,
    "updated_at": "2016-10-25T09:28:21.928Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b1204889587df854c91a014d29db790a909f22b26f8d185864efe29981fe29a"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 5940b73ba2c9a45393769f7016bc5f3db85be3d982d0c32225cd75c81338515d
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
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 68,
      "user_id": 496
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 69,
      "user_id": 496
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 70,
      "user_id": 496
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 71,
      "user_id": 496
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5940b73ba2c9a45393769f7016bc5f3db85be3d982d0c32225cd75c81338515d"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/110
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
    "id": 110,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 110,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 110
      },
      {
        "id": 111,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 110
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/110" -X GET \
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
      "id": 111,
      "name": "Vision-oriented local attitude",
      "name_translations": {
        "en": "Vision-oriented local attitude"
      }
    },
    {
      "id": 112,
      "name": "Balanced high-level hierarchy",
      "name_translations": {
        "en": "Balanced high-level hierarchy"
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
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer b15707dc0e96e2c982e2aabac88d637dbd1cb1aebfb2a3f37a34d485d044bc94
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
    "id": 3,
    "user_id": 52,
    "feedbackable_id": 11,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-25T09:27:54.417Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/3/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b15707dc0e96e2c982e2aabac88d637dbd1cb1aebfb2a3f37a34d485d044bc94"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer 206046921ac4bbdd91fc6d3e526982cb01ccfa4894b959b66f02e859f06024b8
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
    "id": 26,
    "user_id": 153,
    "feedbackable_id": 15,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-25T09:28:01.687Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/26/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 206046921ac4bbdd91fc6d3e526982cb01ccfa4894b959b66f02e859f06024b8"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/1
Content-Type: application/json
Authorization: Bearer df1fdd51d08bde599429d9eb362610a591414db5330068c072e05af23a582983
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
    "user_id": 40,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T09:27:53.880Z",
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
	-H "Authorization: Bearer df1fdd51d08bde599429d9eb362610a591414db5330068c072e05af23a582983"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/5/close
Content-Type: application/json
Authorization: Bearer dd6c7423b06af4eeb4b06d7139153c72756502e8c0f26ee6abcc63320dfeab7c
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
curl "api.goskive.com/v2/feedbacks/5/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd6c7423b06af4eeb4b06d7139153c72756502e8c0f26ee6abcc63320dfeab7c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 9a5279f7e9c3dd1b7273467d9142ae221c3976260dcc885212ddfa59bbc9a13b
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
	-H "Authorization: Bearer 9a5279f7e9c3dd1b7273467d9142ae221c3976260dcc885212ddfa59bbc9a13b"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer c05a175f0f475b69b217ee8d9ed203751ebf3f38442b32be5ec6b3d0c101ee31
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
	-H "Authorization: Bearer c05a175f0f475b69b217ee8d9ed203751ebf3f38442b32be5ec6b3d0c101ee31"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/2
Content-Type: application/json
Authorization: Bearer 3a6765858b899c0c19bccb3775e74449b836c3d23738b7749ec489f6064f5a66
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
    "user_id": 45,
    "feedbackable_id": 10,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T09:27:54.204Z",
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
	-H "Authorization: Bearer 3a6765858b899c0c19bccb3775e74449b836c3d23738b7749ec489f6064f5a66"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 7b5a3b69de25f6c8ff9e33758c138577ec889b539914ffc2fd8308145d663225
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
	-H "Authorization: Bearer 7b5a3b69de25f6c8ff9e33758c138577ec889b539914ffc2fd8308145d663225"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer da08234a5dfc9371b2a06f5109084babf06c94bee94ac8ac80a28aa30546164e
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
	-H "Authorization: Bearer da08234a5dfc9371b2a06f5109084babf06c94bee94ac8ac80a28aa30546164e"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/8
Content-Type: application/json
Authorization: Bearer cf29705ece041cd8796b314826e3e7036234eaa36c213045acff9ef44635bcbc
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/0fb4c833bb591d5a62c01cee1286a18e.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T092821Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=78db09f437f29987f168488e62e4db4514cad43127a06d7a80ec5bc49a326d5a"
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
	-H "Authorization: Bearer cf29705ece041cd8796b314826e3e7036234eaa36c213045acff9ef44635bcbc"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/3/preview
Content-Type: application/json
Authorization: Bearer 518604fd5a5d035ae2ec849ffc97c0af856e6a2526961dfcbc2d051d4972151f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/34a7ee8a6b77b4707f17fe59209303f5.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T092820Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=3b2964e87bfe74180ef2e4c674d0566ab92c0c4a7fd4e33f72b57e0e874d52b5"
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
	-H "Authorization: Bearer 518604fd5a5d035ae2ec849ffc97c0af856e6a2526961dfcbc2d051d4972151f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Content-Type: application/json
Authorization: Bearer b255e51dacb95f2fd7e2e88ba93a87d28a6a5fb17cfe482faf1e88641c929feb
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
      "id": 328,
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
      "created_at": "2016-10-25T09:28:20.713Z",
      "updated_at": "2016-10-25T09:28:20.713Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T09:28:20.786Z",
    "updated_at": "2016-10-25T09:28:20.786Z",
    "course_id": 85,
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
	-H "Authorization: Bearer b255e51dacb95f2fd7e2e88ba93a87d28a6a5fb17cfe482faf1e88641c929feb"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/2/matched_courses?required_cu_count=2
Authorization: Bearer c2c8d4e1fe73a7a994ec578cc0789acb1d923ce41613738a789668c3d44c1dda
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
      "creator_id": 23,
      "id": 7,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "topic_id": 7,
      "discipline_id": 7,
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
      "chapters_updated_at": "2016-10-25T09:27:51.318Z",
      "updated_at": "2016-10-25T09:27:52.892Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 28,
      "id": 8,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-30860cc0-bc1a-4676-84fa-13617ddac60f",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-30860cc0-bc1a-4676-84fa-13617ddac60f",
      "slug": "mit-the-great-british-bake-off-30860cc0-bc1a-4676-84fa-13617ddac60f",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "topic_id": 8,
      "discipline_id": 8,
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
      "chapters_updated_at": "2016-10-25T09:27:51.318Z",
      "updated_at": "2016-10-25T09:27:53.426Z",
      "shortname": "mit-the-great-british-bake-off-30860cc0-bc1a-4676-84fa-13617ddac60f"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/2/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer c2c8d4e1fe73a7a994ec578cc0789acb1d923ce41613738a789668c3d44c1dda"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/7/report
Content-Type: application/json
Authorization: Bearer d7a95a33d59f69cb8a8814506eb5aff3ad00beba2ccedc2a32f6cebb3206444d
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7a95a33d59f69cb8a8814506eb5aff3ad00beba2ccedc2a32f6cebb3206444d"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/58/comments
Content-Type: application/json
Authorization: Bearer 1602bc96114f2cd1adc0ed9fed97ac63535144813b856b677b29733a39b70a01
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
    "author_id": 295,
    "reply_to_id": null,
    "created_at": "2016-10-25T09:28:17.753Z",
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
curl "api.goskive.com/v2/flashcards/58/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1602bc96114f2cd1adc0ed9fed97ac63535144813b856b677b29733a39b70a01"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/57/comments
Content-Type: application/json
Authorization: Bearer 2e7590b6d8eda1b3ab685956b3fe5d9d5c47caf08f1ba842c9ec0eb66e810523
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
    "author_id": 292,
    "reply_to_id": null,
    "created_at": "2016-10-25T09:28:17.407Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 292,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:17.404Z",
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
curl "api.goskive.com/v2/flashcards/57/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e7590b6d8eda1b3ab685956b3fe5d9d5c47caf08f1ba842c9ec0eb66e810523"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/60/comments
Content-Type: application/json
Authorization: Bearer 8c151f4dbf9b701f09c713eb243dbb4a2e16d61380ce7b06145761170694cce4
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
      "id": 6,
      "author_id": 304,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:18.229Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 305,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:18.244Z",
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
curl "api.goskive.com/v2/flashcards/60/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c151f4dbf9b701f09c713eb243dbb4a2e16d61380ce7b06145761170694cce4"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/56/comments
Content-Type: application/json
Authorization: Bearer eca39815a030d4dfbf6b3bdd35f2b053c4390a0c53399a57982ed38b57020da1
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
curl "api.goskive.com/v2/flashcards/56/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eca39815a030d4dfbf6b3bdd35f2b053c4390a0c53399a57982ed38b57020da1"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/54/feedbacks
Content-Type: application/json
Authorization: Bearer df92b5f5fd57f82c9a0d4318cde837f1b42b8ba3cb2aae18c05a80498580fb03
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
    "id": 35,
    "user_id": 283,
    "feedbackable_id": 54,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T09:28:16.545Z",
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
curl "api.goskive.com/v2/flashcards/54/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df92b5f5fd57f82c9a0d4318cde837f1b42b8ba3cb2aae18c05a80498580fb03"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/53/feedbacks
Content-Type: application/json
Authorization: Bearer f1a7220b9d7a9427047d4d1b69cb77b505b91e9c8bc7284e1b2256597755dbbe
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
      "id": 34,
      "user_id": 282,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:16.338Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 281,
      "feedbackable_id": 53,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:16.328Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1a7220b9d7a9427047d4d1b69cb77b505b91e9c8bc7284e1b2256597755dbbe"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/47/votes
Content-Type: application/json
Authorization: Bearer 1ce12d84e57dc39fd3ba53ac76e42ca2a002c56c867ec330724d62aaa4ad2b53
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
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 252
    },
    {
      "id": 7,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 251
    },
    {
      "id": 6,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 47,
      "user_id": 250
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/47/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ce12d84e57dc39fd3ba53ac76e42ca2a002c56c867ec330724d62aaa4ad2b53"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/82/republish
Content-Type: application/json
Authorization: Bearer 2209ca98a869fa2d29439f122a785556cc2991f411d1bc9ea745d9ea5cc7c93b
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
curl "api.goskive.com/v2/flashcards/82/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2209ca98a869fa2d29439f122a785556cc2991f411d1bc9ea745d9ea5cc7c93b"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/61/bookmark
Content-Type: application/json
Authorization: Bearer 301deb3801e24f0b6487d46d233c89cd98c3b3aba99946fadf4bb8581ceeccbc
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/61/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 301deb3801e24f0b6487d46d233c89cd98c3b3aba99946fadf4bb8581ceeccbc"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/63
Content-Type: application/json
Authorization: Bearer 99063a9bf3e1bb83f0a3fc4b27f72317160cf150571f72d9c3c07ebe44d64ab0
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99063a9bf3e1bb83f0a3fc4b27f72317160cf150571f72d9c3c07ebe44d64ab0"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/62/downvote
Content-Type: application/json
Authorization: Bearer 76ac910f0aa95a1948e7c04748e0efaa26268427466cd9e5455482c635c314fc
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/62/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76ac910f0aa95a1948e7c04748e0efaa26268427466cd9e5455482c635c314fc"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/84
Content-Type: application/json
Authorization: Bearer c7200d89040cdb72ad9999bed532c34ac4f2776546930537f7f345719127f1bb
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
    "id": 84,
    "obfuscated_id": "Hu6DTUHzhWo",
    "author_id": 477,
    "chapter_id": 101,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:31.059Z",
    "created_at": "2016-10-25T09:28:31.059Z",
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
curl "api.goskive.com/v2/flashcards/84" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7200d89040cdb72ad9999bed532c34ac4f2776546930537f7f345719127f1bb"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/79/report
Content-Type: application/json
Authorization: Bearer b45d95758ece8fbaadeda4f4b5191d1fec8d766d76e924d9dbf0df9af2bf3e44
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/79/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b45d95758ece8fbaadeda4f4b5191d1fec8d766d76e924d9dbf0df9af2bf3e44"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/83/bookmark
Content-Type: application/json
Authorization: Bearer 8b39e50e651b94d501ce88dd03398ca7858c2647df97fce50254526060f8ec22
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/83/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b39e50e651b94d501ce88dd03398ca7858c2647df97fce50254526060f8ec22"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/80/upvote
Content-Type: application/json
Authorization: Bearer 6be87531a6230762a873ac36c3bc1812e7319c069c8147e193311259797c557c
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/80/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6be87531a6230762a873ac36c3bc1812e7319c069c8147e193311259797c557c"
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
    "key": "cache/d32d2bd25dc62ddc2714538df8632a3a.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxMDoyODoxNFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2QzMmQyYmQyNWRjNjJkZGMyNzE0NTM4ZGY4NjMyYTNhLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjVUMDkyODE0WiJ9XX0=",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T092814Z",
    "x-amz-signature": "3629e97e13dc3e377663f9b816521b2de18a25db5201dc2143fd773afe2b7f9c"
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
Authorization: Bearer 08de92a0351d2404715e237c80ddb7885698dcb01b68758680b4caa570cffd8e
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
curl "api.goskive.com/v2/me/jobs/8/sign_ups" -d '{"sign_up":{"email_address":"joe@megacorp.com"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08de92a0351d2404715e237c80ddb7885698dcb01b68758680b4caa570cffd8e"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 51c882d5e3ddebc0597a15df7cb2e48506d04a67d06d6ac377ffb961f55c7844
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
curl "api.goskive.com/v2/me/jobs/7/sign_ups" -d '{"sign_up":{"email_address":""}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51c882d5e3ddebc0597a15df7cb2e48506d04a67d06d6ac377ffb961f55c7844"
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
{"password":{"reset_password_token":"A4n1EFDP77meCMyehFA8","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 622,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-25T09:28:44.716Z",
  "updated_at": "2016-10-25T09:28:44.894Z",
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
  "audit_id": 4162
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"A4n1EFDP77meCMyehFA8","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/59/comments
Content-Type: application/json
Authorization: Bearer 935f64713cbf4d794b6bb0314a388d3efa49c1e9e2172695ed1e14585f6829c4
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
    "id": 9,
    "author_id": 312,
    "reply_to_id": null,
    "created_at": "2016-10-25T09:28:19.519Z",
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
curl "api.goskive.com/v2/questions/59/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 935f64713cbf4d794b6bb0314a388d3efa49c1e9e2172695ed1e14585f6829c4"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/57/comments
Content-Type: application/json
Authorization: Bearer 27e086ab767548a90ec38b31290f435d1decd57f66825318b871c4c82c7e3dca
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
    "id": 8,
    "author_id": 306,
    "reply_to_id": null,
    "created_at": "2016-10-25T09:28:18.650Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 306,
      "feedbackable_id": 57,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:18.648Z",
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
curl "api.goskive.com/v2/questions/57/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27e086ab767548a90ec38b31290f435d1decd57f66825318b871c4c82c7e3dca"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/61/comments
Content-Type: application/json
Authorization: Bearer 18d10c952a1740364e2285bad8598a30942c5b0b6ed5c129170ab8d625cd4676
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
      "id": 11,
      "author_id": 322,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:20.405Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 321,
      "reply_to_id": null,
      "created_at": "2016-10-25T09:28:20.389Z",
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
curl "api.goskive.com/v2/questions/61/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18d10c952a1740364e2285bad8598a30942c5b0b6ed5c129170ab8d625cd4676"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/58/comments
Content-Type: application/json
Authorization: Bearer 3395624d4948c88919b4d250374039f023701b9451db02a6301ef6cdc555102f
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
curl "api.goskive.com/v2/questions/58/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3395624d4948c88919b4d250374039f023701b9451db02a6301ef6cdc555102f"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/102/feedbacks
Content-Type: application/json
Authorization: Bearer fab97d77b4c156c5facbba8efd7d1e2073135e3fc5f21d0f262ce52575edee84
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
    "user_id": 818,
    "feedbackable_id": 102,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-25T09:28:56.417Z",
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
	-H "Authorization: Bearer fab97d77b4c156c5facbba8efd7d1e2073135e3fc5f21d0f262ce52575edee84"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/99/feedbacks
Content-Type: application/json
Authorization: Bearer 40e70d8375bc6f6d14784c7b12a11afb8f18e6438c786efdee3a8edff329df91
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
      "id": 42,
      "user_id": 803,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:55.341Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 802,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T09:28:55.330Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/99/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40e70d8375bc6f6d14784c7b12a11afb8f18e6438c786efdee3a8edff329df91"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/30/votes
Content-Type: application/json
Authorization: Bearer 053b345741487f87ba9f384c0587e9c57f513b763a819d62cfafc3958051c05e
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
      "votable_id": 30,
      "user_id": 176
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 30,
      "user_id": 175
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 30,
      "user_id": 174
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/30/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 053b345741487f87ba9f384c0587e9c57f513b763a819d62cfafc3958051c05e"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/106/republish
Content-Type: application/json
Authorization: Bearer 3ba95c3d40f32ae97520988f17ead11159222cc00e00d95540199581d6a2adc7
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
curl "api.goskive.com/v2/questions/106/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ba95c3d40f32ae97520988f17ead11159222cc00e00d95540199581d6a2adc7"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/107/bookmark
Content-Type: application/json
Authorization: Bearer 0bbc42bbc307614ad012475fef5b023c904482354f10023003b7924e04ae7b54
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/107/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bbc42bbc307614ad012475fef5b023c904482354f10023003b7924e04ae7b54"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/109
Content-Type: application/json
Authorization: Bearer 9b93a3870140eea9d92196f1c35e6de71152d063551fc40111c875cd4f3eeafe
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b93a3870140eea9d92196f1c35e6de71152d063551fc40111c875cd4f3eeafe"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/104/downvote
Content-Type: application/json
Authorization: Bearer 79e63671ece0fc9668ce6a1d947fdde141430c908e00040bed4b20dc8b6081c5
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/104/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 79e63671ece0fc9668ce6a1d947fdde141430c908e00040bed4b20dc8b6081c5"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/110
Content-Type: application/json
Authorization: Bearer 2af6735bf2e524f301d6ee4a8a08c06da045f5e459345113d05041151695ebae
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
    "id": 110,
    "obfuscated_id": "55JK4PuG2Hk",
    "author_id": 842,
    "chapter_id": 150,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:59.581Z",
    "created_at": "2016-10-25T09:28:59.468Z",
    "tags": [
      {
        "id": 12,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 11,
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
}
```



```shell
curl "api.goskive.com/v2/questions/110" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2af6735bf2e524f301d6ee4a8a08c06da045f5e459345113d05041151695ebae"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/127/report
Content-Type: application/json
Authorization: Bearer 5bbb5306ef79bd6650b444e476c066de1119bf9e44f1973f3bc910c45510cb2a
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/127/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5bbb5306ef79bd6650b444e476c066de1119bf9e44f1973f3bc910c45510cb2a"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/128/bookmark
Content-Type: application/json
Authorization: Bearer 997d00f97a78dfcca9fc228b43ecf68945aeebc76671228d2cc19a7f8d0c0f22
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/128/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 997d00f97a78dfcca9fc228b43ecf68945aeebc76671228d2cc19a7f8d0c0f22"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/108
Content-Type: application/json
Authorization: Bearer 82355e9d63097e04bd88bdb3d1f90ee726d61384e397c7af08b730ad0002df91
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":108,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T09:28:58.438Z","updated_at":"2016-10-25T09:28:58.552Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":148,"author_id":836,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 836,
    "chapter_id": 148,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T09:28:58.656Z",
    "created_at": "2016-10-25T09:28:58.438Z",
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
    "question": "{\"id\"=>108, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-25T09:28:58.438Z\", \"updated_at\"=>\"2016-10-25T09:28:58.552Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>148, \"author_id\"=>836, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 218,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 219,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 220,
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
curl "api.goskive.com/v2/questions/108" -d '{"question":{"question":{"id":108,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T09:28:58.438Z","updated_at":"2016-10-25T09:28:58.552Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":148,"author_id":836,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 82355e9d63097e04bd88bdb3d1f90ee726d61384e397c7af08b730ad0002df91"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/111/upvote
Content-Type: application/json
Authorization: Bearer e27e556242ac29b3fc5e4748aae0d7407df80e65f84efb6b4c8018420c95dbef
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
	-H "Authorization: Bearer e27e556242ac29b3fc5e4748aae0d7407df80e65f84efb6b4c8018420c95dbef"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer b857144654e6569415ad7292ac9f75933d3a2faf33840b607d4b2f99d1587f66
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
      "creator_id": 386,
      "id": 102,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 110,
      "additional_university_ids": [

      ],
      "topic_id": 107,
      "discipline_id": 107,
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
      "updated_at": "2016-10-25T09:28:24.983Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b857144654e6569415ad7292ac9f75933d3a2faf33840b607d4b2f99d1587f66"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 490dac213324ff125c0a53d89a233a26b427998efdbcc003c434e649a0585e9f
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
      "id": 108,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-106",
      "html_url": "https://goskive.com/university/uni-106",
      "slug": "uni-106",
      "name": "National School of Pizza",
      "short_name": "Uni 106",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6a9fa24a498e1c0325fb6c3481402b3b7b1edc26.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a95ae5e7e91665458aaf1066d893915854be5394.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T09:28:24.770Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 107,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-105",
      "html_url": "https://goskive.com/university/uni-105",
      "slug": "uni-105",
      "name": "National School of Pastry",
      "short_name": "Uni 105",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/47501c30005ace1e8cf5ce8d311d35f8e8031d1e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8701d988977fa68699c888ee61dc7050e74864f5.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T09:28:24.754Z",
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
	-H "Authorization: Bearer 490dac213324ff125c0a53d89a233a26b427998efdbcc003c434e649a0585e9f"
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
      "id": 64,
      "name": "Extended zero administration adapter",
      "name_translations": {
        "en": "Extended zero administration adapter"
      },
      "discipline_id": 64
    },
    {
      "id": 65,
      "name": "Realigned object-oriented model",
      "name_translations": {
        "en": "Realigned object-oriented model"
      },
      "discipline_id": 65
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
GET /v2/topics/66
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
    "id": 66,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 66
  }
}
```



```shell
curl "api.goskive.com/v2/topics/66" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 90201c9f4bba6201fbf3676d7d26ec3d69b871e98dc0ac813d15c0001c598f45
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
      "id": 106,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-104",
      "html_url": "https://goskive.com/university/uni-104",
      "slug": "uni-104",
      "name": "University 86",
      "short_name": "Uni 104",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8c3cfcc640b501142346d45d9c1216352db5b701.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/4beabc23e777fea45d5060d45c732f5a1d3ea5c3.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T09:28:24.285Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-102",
      "html_url": "https://goskive.com/university/uni-102",
      "slug": "uni-102",
      "name": "University 84",
      "short_name": "Uni 102",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/aa1ef98de1331ac39c7fcc94b9f4fe40534f67bb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/70d55274ddb3bf695b89ec0eabb79d2ece2a3652.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T09:28:24.254Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 105,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-103",
      "html_url": "https://goskive.com/university/uni-103",
      "slug": "uni-103",
      "name": "University 85",
      "short_name": "Uni 103",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/dc0e5d2206bfaa01cce6e261648c4dd86452febf.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f0b90cd6dc32511d16885857290a60c22dd539ef.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T09:28:24.269Z",
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
	-H "Authorization: Bearer 90201c9f4bba6201fbf3676d7d26ec3d69b871e98dc0ac813d15c0001c598f45"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 2a5b009c443b26d9acc670dda4309ad4108e35f4e863787c03fa2a0497588840
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
    "id": 102,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f4e3e0b6d63443adce6302be96668ddd729603db.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/0654e5221ee212e3d57aeb0560b86c3682155511.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-25T09:28:24.122Z",
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
	-H "Authorization: Bearer 2a5b009c443b26d9acc670dda4309ad4108e35f4e863787c03fa2a0497588840"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 122f6552433279be1ea4ef486068cd2f53d61fef61cba640b71376993e6dc87d
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":170,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 577,
    "id": 158,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "topic_id": 170,
    "discipline_id": 171,
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
    "chapters_updated_at": "2016-10-25T09:28:40.473Z",
    "updated_at": "2016-10-25T09:28:40.600Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 122,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-25T09:28:40.559Z",
        "course_id": 158,
        "author_id": 577,
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
        "updated_at": "2016-10-25T09:28:40.576Z",
        "course_id": 158,
        "author_id": 577,
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
        "updated_at": "2016-10-25T09:28:40.591Z",
        "course_id": 158,
        "author_id": 577,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":170,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 122f6552433279be1ea4ef486068cd2f53d61fef61cba640b71376993e6dc87d"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e4f324eaaf3812054d1dffbb751f69fc482cff68e03efd5bcf579be75ea831ad
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":169,"published":false}}
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
    "creator_id": 576,
    "id": 157,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "topic_id": 169,
    "discipline_id": 170,
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
    "updated_at": "2016-10-25T09:28:40.440Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":169,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4f324eaaf3812054d1dffbb751f69fc482cff68e03efd5bcf579be75ea831ad"
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
      "creator_id": 604,
      "id": 182,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "topic_id": 194,
      "discipline_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
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
      "updated_at": "2016-10-25T09:28:42.867Z",
      "shortname": "fu-course-131"
    },
    {
      "creator_id": 604,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "topic_id": 195,
      "discipline_id": 196,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "chapters_updated_at": "2016-10-25T09:28:43.140Z",
      "updated_at": "2016-10-25T09:28:43.147Z",
      "shortname": "fu-course-132"
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
Authorization: Bearer 4c497847aee45c1f35764816275325e0bfe407835cb081aa4a6b60e09b55ad7d
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
      "creator_id": 611,
      "id": 190,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "topic_id": 202,
      "discipline_id": 203,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
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
      "updated_at": "2016-10-25T09:28:43.556Z",
      "shortname": "fu-course-139"
    },
    {
      "creator_id": 611,
      "id": 191,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-140",
      "html_url": "https://goskive.com/course/fu-course-140",
      "slug": "fu-course-140",
      "university_id": 178,
      "additional_university_ids": [

      ],
      "topic_id": 203,
      "discipline_id": 204,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 140",
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
      "chapters_updated_at": "2016-10-25T09:28:43.830Z",
      "updated_at": "2016-10-25T09:28:43.836Z",
      "shortname": "fu-course-140"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c497847aee45c1f35764816275325e0bfe407835cb081aa4a6b60e09b55ad7d"
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
      "creator_id": 609,
      "id": 186,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 176,
      "additional_university_ids": [

      ],
      "topic_id": 198,
      "discipline_id": 199,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "updated_at": "2016-10-25T09:28:43.318Z",
      "shortname": "fu-course-135"
    },
    {
      "creator_id": 609,
      "id": 187,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 176,
      "additional_university_ids": [

      ],
      "topic_id": 199,
      "discipline_id": 200,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
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
      "updated_at": "2016-10-25T09:28:43.356Z",
      "shortname": "fu-course-136"
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
Authorization: Bearer e8d62bcaa4a71809354aaf00ddc8f18b38fbaf743c3b2d2695a6aab33a7a3728
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
      "creator_id": 617,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-143",
      "html_url": "https://goskive.com/course/fu-course-143",
      "slug": "fu-course-143",
      "university_id": 179,
      "additional_university_ids": [

      ],
      "topic_id": 206,
      "discipline_id": 207,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
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
      "updated_at": "2016-10-25T09:28:44.075Z",
      "shortname": "fu-course-143"
    },
    {
      "creator_id": 617,
      "id": 195,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-144",
      "html_url": "https://goskive.com/course/fu-course-144",
      "slug": "fu-course-144",
      "university_id": 179,
      "additional_university_ids": [

      ],
      "topic_id": 207,
      "discipline_id": 208,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 144",
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
      "updated_at": "2016-10-25T09:28:44.112Z",
      "shortname": "fu-course-144"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8d62bcaa4a71809354aaf00ddc8f18b38fbaf743c3b2d2695a6aab33a7a3728"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 763e8dc77ebb5b676c2730be9d0db5eecf2530dcb674945442f7ec348f979cea
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
  "id": 389,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-25T09:28:25.223Z",
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
	-H "Authorization: Bearer 763e8dc77ebb5b676c2730be9d0db5eecf2530dcb674945442f7ec348f979cea"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/179
Content-Type: application/json
Authorization: Bearer a62c310c4ea3fdb4e0cc297cb35e81ea84b64d8fc97dba9e7a251a4617206b89
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
    "id": 179,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 42,
    "fields_of_study": [
      42,
      43
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-25T09:28:03.960Z",
    "updated_at": "2016-10-25T09:28:03.960Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/179" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a62c310c4ea3fdb4e0cc297cb35e81ea84b64d8fc97dba9e7a251a4617206b89"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/177
Content-Type: application/json
Authorization: Bearer f894375325d2f5a4c53cfd78f78855d9908e9cd1630d3104566daae0d72284a2
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
    "id": 177,
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
    "created_at": "2016-10-25T09:28:03.805Z",
    "updated_at": "2016-10-25T09:28:03.805Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/177" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f894375325d2f5a4c53cfd78f78855d9908e9cd1630d3104566daae0d72284a2"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer 4e1ae9d4a5c8ee3cf0571a3ee2d38abc25e53a45cc5847a0e2fc84dd5d53f6c3
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
	-H "Authorization: Bearer 4e1ae9d4a5c8ee3cf0571a3ee2d38abc25e53a45cc5847a0e2fc84dd5d53f6c3"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/22
Content-Type: application/json
Authorization: Bearer a30c652d1c237db32abec2813e859575e5bf62d60d5c1f92520f49860d0697b4
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
    "votable_id": 134,
    "user_id": 966
  }
}
```



```shell
curl "api.goskive.com/v2/votes/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a30c652d1c237db32abec2813e859575e5bf62d60d5c1f92520f49860d0697b4"
```
