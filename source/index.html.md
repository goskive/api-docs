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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1b1bbace40b964419a99e9e1a57a09a8f24c7cf8443400d8f0b4c9fce8263a43","client_secret":"6e7ab0d9eb714bec58f6210563424cc85899d7e30be2db826f68b565e560c2b3"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"1b1bbace40b964419a99e9e1a57a09a8f24c7cf8443400d8f0b4c9fce8263a43","client_secret":"6e7ab0d9eb714bec58f6210563424cc85899d7e30be2db826f68b565e560c2b3"}' -X POST \
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
Authorization: Basic MWM5MzcxMWY0NzQ1NzAzNTQxYmZlMDA1ZjY0YTA3ODE0N2RhNjIyZjViOTg3
NDA2ZjhhZThkMmZlZDM1NDVkMToxNDA5YWZmOWM0MjAyOGZhNWE5YWUyYWMw
ZWE1NzE0MWE4ZTdjMzM1MTY1MDg0ZWE1NTc2MGQ2NGU0NDA5YjVk

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
	-u 1c93711f4745703541bfe005f64a078147da622f5b987406f8ae8d2fed3545d1:1409aff9c42028fa5a9ae2ac0ea57141a8e7c335165084ea55760d64e4409b5d
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8501e1981cd2ad963d8b9a61ad4a8d22d99d521dda8ef50bea107dcd82b4f31a","client_secret":"d7abcf55dcb6685c7543ae2fb85d1c3e37418035c9169979502c73c8fc0d9331"}
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
  "access_token": "1254206286980650931d09c9e20e07f2f24d4502dd301fd9f44074aa71d47532",
  "token_type": "bearer",
  "created_at": 1476991878
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"8501e1981cd2ad963d8b9a61ad4a8d22d99d521dda8ef50bea107dcd82b4f31a","client_secret":"d7abcf55dcb6685c7543ae2fb85d1c3e37418035c9169979502c73c8fc0d9331"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MTQ3YWEzMjc1ZGIzMTY5Y2U4MGYzZmFjNDFlMmFjMjI4ZTUwYjdhMDZhNjBj
Nzc2NzUxYjVhZWU2ZTA5NGM5Nzo2OTJmMjdkYmMzZTMyMzNkNGMwM2JmY2E4
Y2FkNjEzNzI2ZTM0MDRjMDBjYTRiMDIyZTMwNmEwYWExMDhjZTgz

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
  "access_token": "0fffe1c76856ea2e2871804b0a6f51db56cb0c108d22fddb1b73c7c09ed9f206",
  "token_type": "bearer",
  "created_at": 1476991878
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 147aa3275db3169ce80f3fac41e2ac228e50b7a06a60c776751b5aee6e094c97:692f27dbc3e3233d4c03bfca8cad613726e3404c00ca4b022e306a0aa108ce83
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
{"grant_type":"client_credentials","client_id":"5b414646053e480f4b8b356204687d51947378869789d9320c6254bce96c20a0","client_secret":"a150da392a0090ac7a8cfc8dcbe76b42859a52ccd51744b36e7ab4c289c76eb6"}
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
  "access_token": "20d6edec180afd0f1b5bf16f451f73996cbff639627c7bcf540522f37fed11a5",
  "token_type": "bearer",
  "created_at": 1476991878
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5b414646053e480f4b8b356204687d51947378869789d9320c6254bce96c20a0","client_secret":"a150da392a0090ac7a8cfc8dcbe76b42859a52ccd51744b36e7ab4c289c76eb6"}' -X POST \
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
Authorization: Bearer 91f2e9477f7358d83e797b4b098bb46600812c7856e2c2e97e83041d527c740a
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
    "company_id": 36,
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
	-H "Authorization: Bearer 91f2e9477f7358d83e797b4b098bb46600812c7856e2c2e97e83041d527c740a"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/84/flashcards
Content-Type: application/json
Authorization: Bearer 1b7971e38579911ba6cf0f523903f895ad867a60a7a13af911a52707206e2201
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":84,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 42,
    "obfuscated_id": "6gppIIjkzlA",
    "author_id": 381,
    "chapter_id": 84,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:45.519Z",
    "created_at": "2016-10-20T19:31:45.519Z",
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
curl "api.goskive.com/v2/chapters/84/flashcards" -d '{"flashcard":{"chapter_id":84,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b7971e38579911ba6cf0f523903f895ad867a60a7a13af911a52707206e2201"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/82/flashcards
Content-Type: application/json
Authorization: Bearer 7a5540527f568338d58adecd02f89adf963096e8bc54f101f7a400280437ead3
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 373,
      "chapter_id": 82,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:45.111Z",
      "created_at": "2016-10-20T19:31:45.111Z",
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 373,
      "chapter_id": 82,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:45.151Z",
      "created_at": "2016-10-20T19:31:45.151Z",
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
      "author_id": 373,
      "chapter_id": 82,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:45.191Z",
      "created_at": "2016-10-20T19:31:45.191Z",
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
curl "api.goskive.com/v2/chapters/82/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a5540527f568338d58adecd02f89adf963096e8bc54f101f7a400280437ead3"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/74/questions
Content-Type: application/json
Authorization: Bearer 2a865c79052b224712be06909cfc3cb55a01ac276b8a6cc6cfd49c6cb7d22efb
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":74,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 41,
    "obfuscated_id": "11qbskrctUU",
    "author_id": 325,
    "chapter_id": 74,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:40.718Z",
    "created_at": "2016-10-20T19:31:40.718Z",
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
        "id": 82,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 83,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 84,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 85,
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
curl "api.goskive.com/v2/chapters/74/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":74,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a865c79052b224712be06909cfc3cb55a01ac276b8a6cc6cfd49c6cb7d22efb"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/71/questions
Content-Type: application/json
Authorization: Bearer fe612ea855d9dae823529a44aca6bcc4e6521a625e246e43f4433c6c2880be19
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":71,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 38,
    "obfuscated_id": "8_YCqPYFnsI",
    "author_id": 316,
    "chapter_id": 71,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:39.549Z",
    "created_at": "2016-10-20T19:31:39.549Z",
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
        "id": 75,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 76,
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
curl "api.goskive.com/v2/chapters/71/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":71,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe612ea855d9dae823529a44aca6bcc4e6521a625e246e43f4433c6c2880be19"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/73/questions
Content-Type: application/json
Authorization: Bearer ce88d3a4ca531e1a4f8110d0cff17fcb03c264d3bcb0db2820aedd39b6d683b7
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":73,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 40,
    "obfuscated_id": "lir5nwklJts",
    "author_id": 322,
    "chapter_id": 73,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:40.364Z",
    "created_at": "2016-10-20T19:31:40.364Z",
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
        "id": 80,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 81,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/73/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":73,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce88d3a4ca531e1a4f8110d0cff17fcb03c264d3bcb0db2820aedd39b6d683b7"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/72/questions
Content-Type: application/json
Authorization: Bearer f2385e2670fed2f82d60f1605734cc1ccd245977dd4fa0d2fbe154a7ce0e3110
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":72,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 319,
    "chapter_id": 72,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:39.924Z",
    "created_at": "2016-10-20T19:31:39.924Z",
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
        "id": 77,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 78,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 79,
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
curl "api.goskive.com/v2/chapters/72/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":72,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2385e2670fed2f82d60f1605734cc1ccd245977dd4fa0d2fbe154a7ce0e3110"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/75/questions
Content-Type: application/json
Authorization: Bearer 0c0f31540b64b49eeb6b495d8ecedb94a491dfa114dc6a5314d939f52fbe399c
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 328,
      "chapter_id": 75,
      "position": 38,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:41.372Z",
      "created_at": "2016-10-20T19:31:41.234Z",
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
    },
    {
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 329,
      "chapter_id": 75,
      "position": 39,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:41.593Z",
      "created_at": "2016-10-20T19:31:41.453Z",
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
          "id": 88,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 89,
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
      "author_id": 330,
      "chapter_id": 75,
      "position": 40,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T19:31:41.817Z",
      "created_at": "2016-10-20T19:31:41.675Z",
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
          "id": 90,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 91,
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
curl "api.goskive.com/v2/chapters/75/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c0f31540b64b49eeb6b495d8ecedb94a491dfa114dc6a5314d939f52fbe399c"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/94
Content-Type: application/json
Authorization: Bearer 42f4b5c474ad2a2845f9f486fa235f33aba627bd136709040bd9ea6bc0c58280
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
	-H "Authorization: Bearer 42f4b5c474ad2a2845f9f486fa235f33aba627bd136709040bd9ea6bc0c58280"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/97
Content-Type: application/json
Authorization: Bearer bad6de21428e826f6043d15fc345c66a56680488ba65539a56f1d4c6babea477
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
curl "api.goskive.com/v2/chapters/97" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bad6de21428e826f6043d15fc345c66a56680488ba65539a56f1d4c6babea477"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/93
Content-Type: application/json
Authorization: Bearer 23ee80425302d8b36914d731ee197349771efd16ea8364ec3a4f7239098c79e6
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
curl "api.goskive.com/v2/chapters/93" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23ee80425302d8b36914d731ee197349771efd16ea8364ec3a4f7239098c79e6"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/95
Content-Type: application/json
Authorization: Bearer 9d299265cc5ff93fe3fc7a345e8e6d60e1d8062d55105b21901a6c8d724d8984
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/95" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d299265cc5ff93fe3fc7a345e8e6d60e1d8062d55105b21901a6c8d724d8984"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/99
Content-Type: application/json
Authorization: Bearer 737b40ba5b493c0aeda03e28434e8cc7ccc0b0d29efe9c3765d93f754a9bbf20
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
    "id": 99,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-20T19:31:50.285Z",
    "course_id": 118,
    "author_id": 430,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-20T19:31:49.772Z",
    "questions_updated_at": "2016-10-20T19:31:49.772Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 434,
        "chapter_id": 99,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:50.269Z",
        "created_at": "2016-10-20T19:31:50.269Z",
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
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 432,
        "chapter_id": 99,
        "position": 51,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:31:50.163Z",
        "created_at": "2016-10-20T19:31:50.051Z",
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
            "id": 112,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 113,
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
curl "api.goskive.com/v2/chapters/99" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 737b40ba5b493c0aeda03e28434e8cc7ccc0b0d29efe9c3765d93f754a9bbf20"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/92
Content-Type: application/json
Authorization: Bearer d267c9015e437c355e92e26b52b8e7cf54adab6a1b38056d4740802bb941109f
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
    "id": 92,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-20T19:31:48.097Z",
    "course_id": 111,
    "author_id": 406,
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
curl "api.goskive.com/v2/chapters/92" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d267c9015e437c355e92e26b52b8e7cf54adab6a1b38056d4740802bb941109f"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/18/replies
Content-Type: application/json
Authorization: Bearer df9d594d38cb11fbf217aed54d9ab74b8a3085383626ce9d4478739a36e5e753
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
    "id": 19,
    "author_id": 876,
    "reply_to_id": 18,
    "created_at": "2016-10-20T19:32:31.730Z",
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
curl "api.goskive.com/v2/comments/18/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df9d594d38cb11fbf217aed54d9ab74b8a3085383626ce9d4478739a36e5e753"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/17/replies
Content-Type: application/json
Authorization: Bearer 1b3b0fa6826334e3813dc2c8eaa6e3a61b2dd4fcb88c4984e1299bf52f454681
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
curl "api.goskive.com/v2/comments/17/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b3b0fa6826334e3813dc2c8eaa6e3a61b2dd4fcb88c4984e1299bf52f454681"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/24
Content-Type: application/json
Authorization: Bearer ec6734d581fa4727239f29437bf01a98eba5c25d39fddefb9f11131d1e158516
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
curl "api.goskive.com/v2/comments/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ec6734d581fa4727239f29437bf01a98eba5c25d39fddefb9f11131d1e158516"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/21/republish
Content-Type: application/json
Authorization: Bearer 5ff750222b52ed26fb38fd95ea89e7f61f5528dfaa056fd5835077fac451dfe2
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
curl "api.goskive.com/v2/comments/21/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ff750222b52ed26fb38fd95ea89e7f61f5528dfaa056fd5835077fac451dfe2"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer c5fac66154465de2c551122db56e5d0e02501fd008eefc15744901e5849e9abb
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5fac66154465de2c551122db56e5d0e02501fd008eefc15744901e5849e9abb"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer b7ba979bdd38c0c370ac5d2f0d154773440390660f98a7f098c9a181dd6f8675
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7ba979bdd38c0c370ac5d2f0d154773440390660f98a7f098c9a181dd6f8675"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/27
Content-Type: application/json
Authorization: Bearer f0921c365611aa2ac3dfc572b721229a574999311585bead563d001165cc821c
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
    "id": 27,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/13980fe65fdd33968abf599dbc1d8a315727260c.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-20T19:31:44.965Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/27" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0921c365611aa2ac3dfc572b721229a574999311585bead563d001165cc821c"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 8038a755d0221c6205a5cd10811a8c4988b58dc08588129ed4e3f0d9e24e8737
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
      "id": 24,
      "name": "Fake Company Name 24",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-20T19:31:44.908Z"
    },
    {
      "id": 25,
      "name": "Fake Company Name 25",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-20T19:31:44.912Z"
    },
    {
      "id": 26,
      "name": "Fake Company Name 26",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/3e1bf9e2b3ffdd1384089f708b640bebc9514583.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-20T19:31:44.916Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8038a755d0221c6205a5cd10811a8c4988b58dc08588129ed4e3f0d9e24e8737"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/38/company_profiles
Content-Type: application/json
Authorization: Bearer ae4278b17241724961667f2d53d039222183ff022f945df9c6a7a889fedfd4a9
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
	-H "Authorization: Bearer ae4278b17241724961667f2d53d039222183ff022f945df9c6a7a889fedfd4a9"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer 3c58d6c7a3cdf4dd0e015587bdfbf537d0e1fdfd8a667913bdf17f1bb5ac03a8
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
	-H "Authorization: Bearer 3c58d6c7a3cdf4dd0e015587bdfbf537d0e1fdfd8a667913bdf17f1bb5ac03a8"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 96a8c6e1578035b7dd85bbef49e023a769eb4da2ed13eb1d7c988b608e8f0468
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
	-H "Authorization: Bearer 96a8c6e1578035b7dd85bbef49e023a769eb4da2ed13eb1d7c988b608e8f0468"
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
Authorization: Bearer 21776644d5198b422afb1beb8de51c65d10b24e0c5a346212979a7970a5fefab
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
	-H "Authorization: Bearer 21776644d5198b422afb1beb8de51c65d10b24e0c5a346212979a7970a5fefab"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2987115d375eb0bff8dc498abd94019c5f18becf293b141f5e63e25e98229e7b
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
    "id": 148,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T19:32:07.917Z",
    "course_id": 207,
    "author_id": 668,
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
	-H "Authorization: Bearer 2987115d375eb0bff8dc498abd94019c5f18becf293b141f5e63e25e98229e7b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 43f4872dcda9bac2bdd345b43d77758c560be0ce80592415e0a93b01a91f5bef
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
      "id": 128,
      "title": "Clever Chapter Title 107",
      "position": 1,
      "updated_at": "2016-10-20T19:32:05.524Z",
      "course_id": 196,
      "author_id": 625,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 129,
      "title": "Clever Chapter Title 108",
      "position": 2,
      "updated_at": "2016-10-20T19:32:05.548Z",
      "course_id": 196,
      "author_id": 626,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 130,
      "title": "Clever Chapter Title 109",
      "position": 3,
      "updated_at": "2016-10-20T19:32:05.800Z",
      "course_id": 196,
      "author_id": 627,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-20T19:32:05.451Z",
      "questions_updated_at": "2016-10-20T19:32:05.451Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43f4872dcda9bac2bdd345b43d77758c560be0ce80592415e0a93b01a91f5bef"
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
      "id": 140,
      "title": "Clever Chapter Title 119",
      "position": 1,
      "updated_at": "2016-10-20T19:32:06.982Z",
      "course_id": 202,
      "author_id": 653,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 141,
      "title": "Clever Chapter Title 120",
      "position": 2,
      "updated_at": "2016-10-20T19:32:07.007Z",
      "course_id": 202,
      "author_id": 654,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 142,
      "title": "Clever Chapter Title 121",
      "position": 3,
      "updated_at": "2016-10-20T19:32:07.267Z",
      "course_id": 202,
      "author_id": 655,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-20T19:32:06.909Z",
      "questions_updated_at": "2016-10-20T19:32:06.909Z",
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
Authorization: Bearer e56ef1c202ed638e7f37080de8b1769f788e63516fa83f5f8f312367bab40b49
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
      "id": 131,
      "title": "Clever Chapter Title 110",
      "position": 1,
      "updated_at": "2016-10-20T19:32:06.080Z",
      "course_id": 198,
      "author_id": 634,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 111",
      "position": 2,
      "updated_at": "2016-10-20T19:32:06.104Z",
      "course_id": 198,
      "author_id": 635,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 133,
      "title": "Clever Chapter Title 112",
      "position": 3,
      "updated_at": "2016-10-20T19:32:06.128Z",
      "course_id": 198,
      "author_id": 636,
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
	-H "Authorization: Bearer e56ef1c202ed638e7f37080de8b1769f788e63516fa83f5f8f312367bab40b49"
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
      "id": 143,
      "title": "Clever Chapter Title 122",
      "position": 1,
      "updated_at": "2016-10-20T19:32:07.457Z",
      "course_id": 204,
      "author_id": 660,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 144,
      "title": "Clever Chapter Title 123",
      "position": 2,
      "updated_at": "2016-10-20T19:32:07.481Z",
      "course_id": 204,
      "author_id": 661,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 145,
      "title": "Clever Chapter Title 124",
      "position": 3,
      "updated_at": "2016-10-20T19:32:07.504Z",
      "course_id": 204,
      "author_id": 662,
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
Authorization: Bearer 0ce9406a19762c114473960dca1d36c5fa3e11734bc474ab817aed1fac886bcb
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
    "id": 6,
    "course_id": 192,
    "user_id": 612,
    "updated_at": "2016-10-20T19:32:04.745Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ce9406a19762c114473960dca1d36c5fa3e11734bc474ab817aed1fac886bcb"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 83ddbdf974f910beb272e3aac5e2aacbb8a87c13031df7b6609388b56eca7402
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
      "course_id": 188,
      "user_id": 600,
      "updated_at": "2016-10-20T19:32:04.167Z"
    },
    {
      "id": 3,
      "course_id": 188,
      "user_id": 601,
      "updated_at": "2016-10-20T19:32:04.183Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83ddbdf974f910beb272e3aac5e2aacbb8a87c13031df7b6609388b56eca7402"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/3/files
Content-Type: application/json
Authorization: Bearer f9779c725149cfec18ba2912c801e52d4a458d13d98cb4d7c5f2ed015bb6c765
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
        "id": 6,
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
        "created_at": "2016-10-20T19:31:18.080Z",
        "updated_at": "2016-10-20T19:31:18.080Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T19:31:18.143Z",
      "updated_at": "2016-10-20T19:31:18.143Z",
      "course_id": 3,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 7,
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
        "created_at": "2016-10-20T19:31:18.150Z",
        "updated_at": "2016-10-20T19:31:18.150Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T19:31:18.159Z",
      "updated_at": "2016-10-20T19:31:18.159Z",
      "course_id": 3,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 8,
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
        "created_at": "2016-10-20T19:31:18.166Z",
        "updated_at": "2016-10-20T19:31:18.166Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-20T19:31:18.175Z",
      "updated_at": "2016-10-20T19:31:18.175Z",
      "course_id": 3,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/3/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9779c725149cfec18ba2912c801e52d4a458d13d98cb4d7c5f2ed015bb6c765"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/4/files
Content-Type: application/json
Authorization: Bearer eaf584d6783a1924257e48836f5e56f8e8085f5c1c37ce34f35454db99845154
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
      "id": 11,
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
      "created_at": "2016-10-20T19:31:18.301Z",
      "updated_at": "2016-10-20T19:31:18.301Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-20T19:31:18.329Z",
    "updated_at": "2016-10-20T19:31:18.329Z",
    "course_id": 4,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/4/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaf584d6783a1924257e48836f5e56f8e8085f5c1c37ce34f35454db99845154"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/1/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 16ece0eaba9d20bbf00ac9fceaf43b957b7d572fa62e16cd388f9b2994634ecb
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
    "key": "cache/6ebc2cf2459eb54a66bd0a957514712d.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMFQyMDozMToxN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzZlYmMyY2YyNDU5ZWI1NGE2NmJkMGE5NTc1MTQ3MTJkLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjAvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDIwVDE5MzExN1oifV19",
    "x-amz-credential": "FAKE/20161020/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161020T193117Z",
    "x-amz-signature": "4586366fb18effd62eabce09eca11f6cd216a97a359a47565264e5f133f2a2b7"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/1/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16ece0eaba9d20bbf00ac9fceaf43b957b7d572fa62e16cd388f9b2994634ecb"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 783d8c911103660f53ade34f38d3b21aa4b74016d576456a1211077e60a9ff03
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
	-H "Authorization: Bearer 783d8c911103660f53ade34f38d3b21aa4b74016d576456a1211077e60a9ff03"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ae75a1d3e958f9e1fd7d91525ff3f0f7451b7cef7437c9f2c417904a6e5bf0d9
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
	-H "Authorization: Bearer ae75a1d3e958f9e1fd7d91525ff3f0f7451b7cef7437c9f2c417904a6e5bf0d9"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0c2fae938b2aaa9e8a1cc7b4df9d43abee14919dbda1e3557e1325231fd0af19
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
	-H "Authorization: Bearer 0c2fae938b2aaa9e8a1cc7b4df9d43abee14919dbda1e3557e1325231fd0af19"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3cb4297498738e1af3f0015ce31de5279025f680c2419a0dbb657c072b930f7b
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
	-H "Authorization: Bearer 3cb4297498738e1af3f0015ce31de5279025f680c2419a0dbb657c072b930f7b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b4bdad5653eff265dc4750e0890f8e74fb6f026112515626987806e1e065c87c
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
	-H "Authorization: Bearer b4bdad5653eff265dc4750e0890f8e74fb6f026112515626987806e1e065c87c"
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
    "creator_id": 682,
    "id": 209,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 193,
    "additional_university_ids": [

    ],
    "topic_id": 214,
    "discipline_id": 214,
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
    "chapters_updated_at": "2016-10-20T19:32:10.073Z",
    "updated_at": "2016-10-20T19:32:11.519Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 149,
        "title": "Clever Chapter Title 125",
        "position": 1,
        "updated_at": "2016-10-20T19:32:11.473Z",
        "course_id": 209,
        "author_id": 682,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T19:32:10.073Z",
        "questions_updated_at": "2016-10-20T19:32:10.073Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 150,
        "title": "Clever Chapter Title 126",
        "position": 2,
        "updated_at": "2016-10-20T19:32:11.512Z",
        "course_id": 209,
        "author_id": 682,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T19:32:10.073Z",
        "questions_updated_at": "2016-10-20T19:32:10.073Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 682,
        "chapter_id": 149,
        "position": 78,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:10.283Z",
        "created_at": "2016-10-20T19:32:10.163Z",
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
            "id": 166,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 167,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 682,
        "chapter_id": 150,
        "position": 80,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:10.667Z",
        "created_at": "2016-10-20T19:32:10.543Z",
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
            "id": 170,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 171,
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
Authorization: Bearer 9132db4af1555ca7a71627a34e9f526c5596125ff93525411ff16d0e5da1f18c
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
    "creator_id": 687,
    "id": 210,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 194,
    "additional_university_ids": [

    ],
    "topic_id": 215,
    "discipline_id": 215,
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
    "chapters_updated_at": "2016-10-20T19:32:11.574Z",
    "updated_at": "2016-10-20T19:32:13.114Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 151,
        "title": "Clever Chapter Title 127",
        "position": 1,
        "updated_at": "2016-10-20T19:32:13.061Z",
        "course_id": 210,
        "author_id": 687,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T19:32:11.574Z",
        "questions_updated_at": "2016-10-20T19:32:11.574Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 152,
        "title": "Clever Chapter Title 128",
        "position": 2,
        "updated_at": "2016-10-20T19:32:13.105Z",
        "course_id": 210,
        "author_id": 687,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-20T19:32:11.574Z",
        "questions_updated_at": "2016-10-20T19:32:11.574Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 688,
        "chapter_id": 151,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:12.886Z",
        "created_at": "2016-10-20T19:32:12.886Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 688,
        "chapter_id": 152,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:12.964Z",
        "created_at": "2016-10-20T19:32:12.964Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 688,
        "chapter_id": 151,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:12.930Z",
        "created_at": "2016-10-20T19:32:12.930Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 688,
        "chapter_id": 152,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:13.008Z",
        "created_at": "2016-10-20T19:32:13.008Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 688,
        "chapter_id": 151,
        "position": 84,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:11.796Z",
        "created_at": "2016-10-20T19:32:11.673Z",
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
            "id": 178,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 179,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 688,
        "chapter_id": 151,
        "position": 85,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:11.978Z",
        "created_at": "2016-10-20T19:32:11.861Z",
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
            "id": 180,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 181,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 688,
        "chapter_id": 152,
        "position": 86,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:12.194Z",
        "created_at": "2016-10-20T19:32:12.065Z",
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
            "id": 182,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 183,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 91,
        "obfuscated_id": "EqPpyB0JN58",
        "author_id": 688,
        "chapter_id": 152,
        "position": 87,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T19:32:12.383Z",
        "created_at": "2016-10-20T19:32:12.262Z",
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
            "id": 184,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 185,
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
	-H "Authorization: Bearer 9132db4af1555ca7a71627a34e9f526c5596125ff93525411ff16d0e5da1f18c"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/217/pin
Content-Type: application/json
Authorization: Bearer bd4f4425f82ca82a24801d073f5130dd8ba8ec1fe204f43ec39dfa1023a411ed
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/217/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd4f4425f82ca82a24801d073f5130dd8ba8ec1fe204f43ec39dfa1023a411ed"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/227/pin
Content-Type: application/json
Authorization: Bearer 55637d36c2e97a358010a5e310bcfaeaff7d45d0da7a68acd185a217dac0c3ef
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/227/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55637d36c2e97a358010a5e310bcfaeaff7d45d0da7a68acd185a217dac0c3ef"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 62bb54711824935cc450f8b78669cdfa2dc2f18cdfac42d182fe343b269fc307
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
    "creator_id": 709,
    "id": 215,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 199,
    "additional_university_ids": [

    ],
    "topic_id": 220,
    "discipline_id": 220,
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
    "updated_at": "2016-10-20T19:32:16.811Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62bb54711824935cc450f8b78669cdfa2dc2f18cdfac42d182fe343b269fc307"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer cae123c11625260bbc8b1907ba63bf4625b71db2d560aab679263e670d3df86f
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
    "id": 736,
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
    "created_at": "2016-10-20T19:32:18.803Z",
    "updated_at": "2016-10-20T19:32:18.803Z",
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
	-H "Authorization: Bearer cae123c11625260bbc8b1907ba63bf4625b71db2d560aab679263e670d3df86f"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer e5793adbe2e25ad68c0c06b9c35e93b54f17d6f13deb491e945beef39937ccef
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[233]}
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
    "id": 737,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      233
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T19:32:18.885Z",
    "updated_at": "2016-10-20T19:32:18.921Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[233]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e5793adbe2e25ad68c0c06b9c35e93b54f17d6f13deb491e945beef39937ccef"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer fc66ce3d36b99dab2550a587d42a79476f66eefc196ac7b6a0c8c84aeae28562
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
    "id": 738,
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
    "created_at": "2016-10-20T19:32:18.944Z",
    "updated_at": "2016-10-20T19:32:18.944Z",
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
	-H "Authorization: Bearer fc66ce3d36b99dab2550a587d42a79476f66eefc196ac7b6a0c8c84aeae28562"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 1785ea223a770bf784215b39f91bce66f3b1cc8dec70319bcc29804c6eb38441
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[236]}
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
    "id": 740,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      236
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T19:32:19.124Z",
    "updated_at": "2016-10-20T19:32:19.124Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[236]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1785ea223a770bf784215b39f91bce66f3b1cc8dec70319bcc29804c6eb38441"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 07c328a77cc26b955d7cc55ba327aa46b09a09379c49a74ff5150ad1b803ceea
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

237
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
    "id": 741,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/8b743559e5de475584da03c489cc82de25f1a8de.jpg",
    "university_id": null,
    "fields_of_study": [
      237
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-20T19:32:19.199Z",
    "updated_at": "2016-10-20T19:32:19.462Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/9bd9cb86ca59485b3d39c2d4a5122bbc2348be10.jpg",
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

237
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 07c328a77cc26b955d7cc55ba327aa46b09a09379c49a74ff5150ad1b803ceea"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 6d64a3210392e571fe7c22dbf2ef065950a8f8f4e327a7ab50bcc3aaff065a26
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
	-H "Authorization: Bearer 6d64a3210392e571fe7c22dbf2ef065950a8f8f4e327a7ab50bcc3aaff065a26"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer b584ce23fdff86d5324f9b6574c00a0d7c86f632df40f6afa7fe87a09a1d5c5c
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
      "title": "Campaign 10",
      "company_id": 32,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 33,
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
	-H "Authorization: Bearer b584ce23fdff86d5324f9b6574c00a0d7c86f632df40f6afa7fe87a09a1d5c5c"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 76911c092c02ad68409bd14244eb71f9ffb350cc42485b25e548c7e04bcde1e8
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
      "id": 9,
      "title": "Campaign 9",
      "company_id": 28,
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
	-H "Authorization: Bearer 76911c092c02ad68409bd14244eb71f9ffb350cc42485b25e548c7e04bcde1e8"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer aff92378befd3a7b077503c608eca4753844d69e51f9797bca1742e59f18d7fd
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
      "creator_id": 748,
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-160",
      "html_url": "https://goskive.com/course/mit-course-160",
      "slug": "mit-course-160",
      "university_id": 217,
      "additional_university_ids": [

      ],
      "topic_id": 242,
      "discipline_id": 242,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 160",
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
      "updated_at": "2016-10-20T19:32:20.020Z",
      "shortname": "mit-course-160"
    },
    {
      "creator_id": 749,
      "id": 233,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-161",
      "html_url": "https://goskive.com/course/mit-course-161",
      "slug": "mit-course-161",
      "university_id": 218,
      "additional_university_ids": [

      ],
      "topic_id": 243,
      "discipline_id": 243,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 161",
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
      "updated_at": "2016-10-20T19:32:20.096Z",
      "shortname": "mit-course-161"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aff92378befd3a7b077503c608eca4753844d69e51f9797bca1742e59f18d7fd"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer e13240f907edd8683a6dccc0e3e8621b8ac9ca727cbb290e8f447c710020c750
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-20T19:31:42.777Z"
      },
      "created_at": "2016-10-20T19:31:42.780Z",
      "updated_at": "2016-10-20T19:31:42.780Z",
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
      "company_id": 22,
      "company": {
        "id": 22,
        "name": "Fake Company Name 22",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/c6596689a12a2cb3a167b18652a9485aec97373a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-20T19:31:42.788Z"
      },
      "created_at": "2016-10-20T19:31:42.791Z",
      "updated_at": "2016-10-20T19:31:42.791Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e13240f907edd8683a6dccc0e3e8621b8ac9ca727cbb290e8f447c710020c750"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8c41721eef47c178b3809d2fb53a10849b0d36ad985cc077a24488649c76da85
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
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-20T19:31:42.582Z"
      },
      "created_at": "2016-10-20T19:31:42.585Z",
      "updated_at": "2016-10-20T19:31:42.585Z",
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
        "name": "Fake Company Name 18",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-20T19:31:42.598Z"
      },
      "created_at": "2016-10-20T19:31:42.601Z",
      "updated_at": "2016-10-20T19:31:42.601Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8c41721eef47c178b3809d2fb53a10849b0d36ad985cc077a24488649c76da85"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 5b87fd9b80adb5c4191565acae60469ba33492929c5d9ccfaabf656cf0f9dc9a
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
      "id": 4,
      "created_at": "2016-10-20T19:31:32.181Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 6,
      "updated_at": "2016-10-20T19:31:32.283Z",
      "author_id": "199",
      "thread_subject_id": "47",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 5,
      "created_at": "2016-10-20T19:31:32.272Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-10-20T19:31:32.286Z",
      "author_id": "202",
      "thread_subject_id": "48",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 6,
      "created_at": "2016-10-20T19:31:32.670Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-10-20T19:31:32.670Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-10-20T19:31:33.053Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 6,
      "updated_at": "2016-10-20T19:31:33.053Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 8,
      "created_at": "2016-10-20T19:31:33.439Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 7,
      "updated_at": "2016-10-20T19:31:33.439Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 9,
      "created_at": "2016-10-20T19:31:33.742Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 35,
      "updated_at": "2016-10-20T19:31:33.742Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 10,
      "created_at": "2016-10-20T19:31:34.048Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 36,
      "updated_at": "2016-10-20T19:31:34.048Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-10-20T19:31:34.347Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 37,
      "updated_at": "2016-10-20T19:31:34.347Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b87fd9b80adb5c4191565acae60469ba33492929c5d9ccfaabf656cf0f9dc9a"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/12
Content-Type: application/json
Authorization: Bearer 389da36dd46dfb5c401ddbb3e8b68f678f40bed20f44d9f910508a0742298c96
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-20T19:21:34.000Z"}}
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
    "id": 12,
    "created_at": "2016-10-20T19:31:34.474Z",
    "read_at": "2016-10-20T19:21:34.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 8,
    "updated_at": "2016-10-20T19:31:34.512Z",
    "author_id": "227",
    "thread_subject_id": "55",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/12" -d '{"notification":{"read_at":"2016-10-20T19:21:34.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 389da36dd46dfb5c401ddbb3e8b68f678f40bed20f44d9f910508a0742298c96"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer b554b5f2bdeaa892ac5e7aa2ca891600ae8447c193e03e51f854e1dd07d496fb
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
      "id": 1,
      "course_id": 90,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-20T19:31:43.008Z",
      "course_published": true,
      "updated_at": "2016-10-20T19:31:42.998Z"
    },
    {
      "id": 2,
      "course_id": 91,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-20T19:31:43.087Z",
      "course_published": true,
      "updated_at": "2016-10-20T19:31:43.079Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b554b5f2bdeaa892ac5e7aa2ca891600ae8447c193e03e51f854e1dd07d496fb"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer de47caee90a549069b7828b991784d5d05c72dc384cfecfa058c4ca50073f315
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
    "course_id": 94,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-20T19:31:43.477Z",
    "course_published": true,
    "updated_at": "2016-10-20T19:31:43.469Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de47caee90a549069b7828b991784d5d05c72dc384cfecfa058c4ca50073f315"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer ed1048628fb66cdd264b629d990ae43025be7beaa264d03cbee839684edee13e
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
    "course_id": 95,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-20T19:31:43.640Z",
    "course_published": true,
    "updated_at": "2016-10-20T19:31:43.629Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed1048628fb66cdd264b629d990ae43025be7beaa264d03cbee839684edee13e"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer e6a104f7fa4a529c788a76b70b53d124a71947af0c042e09ffc5420098beba1c
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
      "votable_id": 46,
      "user_id": 389
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 47,
      "user_id": 389
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 48,
      "user_id": 389
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 389
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6a104f7fa4a529c788a76b70b53d124a71947af0c042e09ffc5420098beba1c"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/281
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
    "id": 281,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 279,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 281
      },
      {
        "id": 280,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 281
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/281" -X GET \
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
      "id": 279,
      "name": "Persistent explicit paradigm",
      "name_translations": {
        "en": "Persistent explicit paradigm"
      }
    },
    {
      "id": 280,
      "name": "Adaptive directional strategy",
      "name_translations": {
        "en": "Adaptive directional strategy"
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
PATCH /v2/feedbacks/5/close
Content-Type: application/json
Authorization: Bearer 0bff6cfd7bda6bbe1decbb261a8088755b93c5da6aa5be7f9007be4ccd1b2947
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
    "id": 5,
    "user_id": 76,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-20T19:31:23.065Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/5/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bff6cfd7bda6bbe1decbb261a8088755b93c5da6aa5be7f9007be4ccd1b2947"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 7a028f1e29ffa0df92195a68158d27fcf9c4ff775aa0a9bf65f11b6c198c1ff5
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
    "id": 28,
    "user_id": 177,
    "feedbackable_id": 9,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-20T19:31:29.797Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/28/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a028f1e29ffa0df92195a68158d27fcf9c4ff775aa0a9bf65f11b6c198c1ff5"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/1
Content-Type: application/json
Authorization: Bearer a9a305ecc85e22098254ca42fa9649bb136b498ad07f605b59a59086a22a23be
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
    "user_id": 54,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T19:31:21.662Z",
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
	-H "Authorization: Bearer a9a305ecc85e22098254ca42fa9649bb136b498ad07f605b59a59086a22a23be"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer 1ad6f3c9a300306c57492f17ecb77fc0f51e514db96ef54137875e76195e8115
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
	-H "Authorization: Bearer 1ad6f3c9a300306c57492f17ecb77fc0f51e514db96ef54137875e76195e8115"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 58b5378a2d88ddcbbfbe7e9e6346d9148c410361e832719cbf4b8652f74d2d27
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
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58b5378a2d88ddcbbfbe7e9e6346d9148c410361e832719cbf4b8652f74d2d27"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/fix
Content-Type: application/json
Authorization: Bearer dd0b2ed3965875adba73e09926893e7042cdfde556e7a7c5195948ef848692a2
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
curl "api.goskive.com/v2/feedbacks/26/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd0b2ed3965875adba73e09926893e7042cdfde556e7a7c5195948ef848692a2"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/2
Content-Type: application/json
Authorization: Bearer f2f51f34d7efec3513d7ab36ad89521e74e17352e950f58a06e7c400ee001175
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
    "user_id": 59,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T19:31:22.047Z",
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
	-H "Authorization: Bearer f2f51f34d7efec3513d7ab36ad89521e74e17352e950f58a06e7c400ee001175"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer f63e5b99e97a709cd8cfeee163d171bfd74fe55efabfcf23b9c40200ef31363f
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
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f63e5b99e97a709cd8cfeee163d171bfd74fe55efabfcf23b9c40200ef31363f"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer ffcc7d5fcaec3ef027e8e3b1212a7a68f3101b134f23c89423379f04c294e406
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffcc7d5fcaec3ef027e8e3b1212a7a68f3101b134f23c89423379f04c294e406"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/5
Content-Type: application/json
Authorization: Bearer 62de71bf00732344c8f7415d6eb7360075d23d39ebf6bed058cfcfac3f8c4700
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/61c35a4bc4894860ff0436eed7932cbc.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161020%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161020T193150Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=89cb32d0ba21b1a1951d84654a5869f5d8827ac69843f8c5e62744ba7cf7b799"
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
	-H "Authorization: Bearer 62de71bf00732344c8f7415d6eb7360075d23d39ebf6bed058cfcfac3f8c4700"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/7/preview
Content-Type: application/json
Authorization: Bearer c7ec6e0bf8188b4b2cb23f22c793da22f0d692bfce6309cab3e70f30fdd642ff
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/7f114c1a1b2fb40f0693e379e3706367.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161020%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161020T193150Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=a12664967c3bf89d4f4f48778e5f20b881642317b84bc06ca7ac0133017b1d36"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/7/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7ec6e0bf8188b4b2cb23f22c793da22f0d692bfce6309cab3e70f30fdd642ff"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer f8c13e160f62a70c1f3c1eb1f07737cad0e451f22046ec629c1282937ed68c0a
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
      "id": 450,
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
      "created_at": "2016-10-20T19:31:51.225Z",
      "updated_at": "2016-10-20T19:31:51.225Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-20T19:31:51.297Z",
    "updated_at": "2016-10-20T19:31:51.297Z",
    "course_id": 124,
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
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8c13e160f62a70c1f3c1eb1f07737cad0e451f22046ec629c1282937ed68c0a"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/14/matched_courses?required_cu_count=2
Authorization: Bearer 44418ce7a40b6ba88860bf8ea1fbbc40f312ce358ff6eb185dab3d28c6febd36
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
      "creator_id": 583,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 168,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 189,
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
      "chapters_updated_at": "2016-10-20T19:32:01.596Z",
      "updated_at": "2016-10-20T19:32:03.246Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 588,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-9dbde2dd-4e0a-483d-924f-10910903c528",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-9dbde2dd-4e0a-483d-924f-10910903c528",
      "slug": "mit-the-great-british-bake-off-9dbde2dd-4e0a-483d-924f-10910903c528",
      "university_id": 169,
      "additional_university_ids": [

      ],
      "topic_id": 190,
      "discipline_id": 190,
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
      "chapters_updated_at": "2016-10-20T19:32:01.596Z",
      "updated_at": "2016-10-20T19:32:03.791Z",
      "shortname": "mit-the-great-british-bake-off-9dbde2dd-4e0a-483d-924f-10910903c528"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/14/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 44418ce7a40b6ba88860bf8ea1fbbc40f312ce358ff6eb185dab3d28c6febd36"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/6/report
Content-Type: application/json
Authorization: Bearer 423ee6cd7a07ab6ad9ef3f11a0bca8bdcb3e199e0ec5a30848dc4c63131306a7
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 423ee6cd7a07ab6ad9ef3f11a0bca8bdcb3e199e0ec5a30848dc4c63131306a7"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/35/comments
Content-Type: application/json
Authorization: Bearer 254a2c6d6e546c24d8374184ea8869bdf5430f5a8427e6f4956cf74b2e1d62e9
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
    "author_id": 356,
    "reply_to_id": null,
    "created_at": "2016-10-20T19:31:43.992Z",
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
curl "api.goskive.com/v2/flashcards/35/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 254a2c6d6e546c24d8374184ea8869bdf5430f5a8427e6f4956cf74b2e1d62e9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/36/comments
Content-Type: application/json
Authorization: Bearer a374d4936bc371322ff4d4ca9463985ec6d19745ba4d210274df8d9d8877aece
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
    "author_id": 359,
    "reply_to_id": null,
    "created_at": "2016-10-20T19:31:44.299Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 30,
      "user_id": 359,
      "feedbackable_id": 36,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:44.296Z",
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
curl "api.goskive.com/v2/flashcards/36/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a374d4936bc371322ff4d4ca9463985ec6d19745ba4d210274df8d9d8877aece"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/37/comments
Content-Type: application/json
Authorization: Bearer 7642c0cce4197e12dce704edd878e4461c6336cd584a25525d0d811224bc5f04
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
      "id": 11,
      "author_id": 365,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:31:44.626Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 366,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:31:44.643Z",
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
curl "api.goskive.com/v2/flashcards/37/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7642c0cce4197e12dce704edd878e4461c6336cd584a25525d0d811224bc5f04"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/34/comments
Content-Type: application/json
Authorization: Bearer 13b49d0a40d3151af385120832077b99839be9df87cc02db24c703927a4aa764
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
curl "api.goskive.com/v2/flashcards/34/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13b49d0a40d3151af385120832077b99839be9df87cc02db24c703927a4aa764"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/89/feedbacks
Content-Type: application/json
Authorization: Bearer 1b7f9ba39412ab74305a448570864b7f53cfbb9f3e605d79a13aab66418f4faf
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
    "user_id": 754,
    "feedbackable_id": 89,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-20T19:32:20.657Z",
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
	-H "Authorization: Bearer 1b7f9ba39412ab74305a448570864b7f53cfbb9f3e605d79a13aab66418f4faf"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/91/feedbacks
Content-Type: application/json
Authorization: Bearer 86dc62aa575c2f24eaaa53c7464f3eed032f435103535e3e00c5c0fca8f6a66b
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
      "id": 42,
      "user_id": 764,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:32:21.115Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 763,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:32:21.104Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86dc62aa575c2f24eaaa53c7464f3eed032f435103535e3e00c5c0fca8f6a66b"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/49/votes
Content-Type: application/json
Authorization: Bearer 38e16f58fd5832f79467fbee799a50c5330a18ac754c21d74a5ecf17a35a66f0
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
      "id": 20,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 49,
      "user_id": 524
    },
    {
      "id": 19,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 49,
      "user_id": 523
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 49,
      "user_id": 522
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/49/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38e16f58fd5832f79467fbee799a50c5330a18ac754c21d74a5ecf17a35a66f0"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/32/republish
Content-Type: application/json
Authorization: Bearer df759ee05887288daf7926b880cfa205c0a63be12e80ed56a0807a1aad0d31e8
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
curl "api.goskive.com/v2/flashcards/32/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df759ee05887288daf7926b880cfa205c0a63be12e80ed56a0807a1aad0d31e8"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/12/bookmark
Content-Type: application/json
Authorization: Bearer 011ce058066baf558b3b5adc9b86c35187b0a359802219f12bab9f1b102c5228
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/12/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 011ce058066baf558b3b5adc9b86c35187b0a359802219f12bab9f1b102c5228"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/10
Content-Type: application/json
Authorization: Bearer 90fdf377404000f1172ff864b49cbafee6c86fd5d5776c86f79b42e87133cb0f
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
	-H "Authorization: Bearer 90fdf377404000f1172ff864b49cbafee6c86fd5d5776c86f79b42e87133cb0f"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/11/downvote
Content-Type: application/json
Authorization: Bearer d0f873cbfedf2ada3bc734f1b8cd6a0b4ec8baf935d1fd4ce089ec3686b2fc19
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/11/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0f873cbfedf2ada3bc734f1b8cd6a0b4ec8baf935d1fd4ce089ec3686b2fc19"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/13
Content-Type: application/json
Authorization: Bearer de80cff5f68617e85475799993b1530d68489b7521ec31d7d18b0320606de151
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
    "id": 13,
    "obfuscated_id": "6UMEHi0zidE",
    "author_id": 246,
    "chapter_id": 50,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:31:36.043Z",
    "created_at": "2016-10-20T19:31:36.043Z",
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
curl "api.goskive.com/v2/flashcards/13" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de80cff5f68617e85475799993b1530d68489b7521ec31d7d18b0320606de151"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/31/report
Content-Type: application/json
Authorization: Bearer d356e657a9534d37c50c9ce1d4d4fe2ce7be4d37c4f41b418fcc3f4ae83cb9f2
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/31/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d356e657a9534d37c50c9ce1d4d4fe2ce7be4d37c4f41b418fcc3f4ae83cb9f2"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/30/bookmark
Content-Type: application/json
Authorization: Bearer bcb68ecf1c2d468aad17e5967c9f72e87abb10e6d87d3eb207358068cf11e1a9
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
	-H "Authorization: Bearer bcb68ecf1c2d468aad17e5967c9f72e87abb10e6d87d3eb207358068cf11e1a9"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/14/upvote
Content-Type: application/json
Authorization: Bearer ab6695151fa2258f0c0a866cc19a816c03df9aeb47c2ad2c8c51e77dd1d3efb2
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/14/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab6695151fa2258f0c0a866cc19a816c03df9aeb47c2ad2c8c51e77dd1d3efb2"
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
    "key": "cache/d4323ade19044ae0140657bfc196afa0.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yMFQyMDozMToxNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Q0MzIzYWRlMTkwNDRhZTAxNDA2NTdiZmMxOTZhZmEwLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyMC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjBUMTkzMTE2WiJ9XX0=",
    "x-amz-credential": "FAKE/20161020/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161020T193116Z",
    "x-amz-signature": "66fe167782e111dd2f21f9d0746c8026d8d70e3e0b9a2ba7b4d33382aec77f33"
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
Authorization: Bearer f084d2eb73c8583f8e2ffa3e1209404c02734834920cc377dc3915a2cf2e9f40
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
	-H "Authorization: Bearer f084d2eb73c8583f8e2ffa3e1209404c02734834920cc377dc3915a2cf2e9f40"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer 8ed59e348b3a9e7dd4d90be989cc53613af3bfe71178243a5e660b893927cda9
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
	-H "Authorization: Bearer 8ed59e348b3a9e7dd4d90be989cc53613af3bfe71178243a5e660b893927cda9"
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
{"password":{"reset_password_token":"BPsDxVRtyCKgZswor79T","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 673,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-20T19:32:08.512Z",
  "updated_at": "2016-10-20T19:32:08.691Z",
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
  "audit_id": 4759
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"BPsDxVRtyCKgZswor79T","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/28/comments
Content-Type: application/json
Authorization: Bearer 7c5760eca567b383bca2ba866557c84e53c049de13d776c62c07adb26bfc4ea0
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
    "author_id": 182,
    "reply_to_id": null,
    "created_at": "2016-10-20T19:31:30.782Z",
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
curl "api.goskive.com/v2/questions/28/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c5760eca567b383bca2ba866557c84e53c049de13d776c62c07adb26bfc4ea0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/27/comments
Content-Type: application/json
Authorization: Bearer fb7ba2f5f2af456fe1e87dd415f2682639c3f41dd0138f4ebb11f3e6fd746003
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
    "id": 2,
    "author_id": 179,
    "reply_to_id": null,
    "created_at": "2016-10-20T19:31:30.320Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 29,
      "user_id": 179,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:30.318Z",
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
	-H "Authorization: Bearer fb7ba2f5f2af456fe1e87dd415f2682639c3f41dd0138f4ebb11f3e6fd746003"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/30/comments
Content-Type: application/json
Authorization: Bearer 4f23142269c4b621a1edf9b53d7011fff199b9c2eaa4942ff4f2bbc679bcc189
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
      "author_id": 191,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:31:31.551Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 192,
      "reply_to_id": null,
      "created_at": "2016-10-20T19:31:31.567Z",
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
curl "api.goskive.com/v2/questions/30/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f23142269c4b621a1edf9b53d7011fff199b9c2eaa4942ff4f2bbc679bcc189"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/29/comments
Content-Type: application/json
Authorization: Bearer 1633338cbd9913d3e6362bee193aef1d6184a89a45f521ac594ecaa8609aa8ef
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
curl "api.goskive.com/v2/questions/29/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1633338cbd9913d3e6362bee193aef1d6184a89a45f521ac594ecaa8609aa8ef"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/65/feedbacks
Content-Type: application/json
Authorization: Bearer f6e17ed6f9a33d0cbaf761d0108a91d702b5702cf5bec5c4913e026e960dd99d
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
    "id": 37,
    "user_id": 510,
    "feedbackable_id": 65,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-20T19:31:55.860Z",
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
curl "api.goskive.com/v2/questions/65/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6e17ed6f9a33d0cbaf761d0108a91d702b5702cf5bec5c4913e026e960dd99d"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/63/feedbacks
Content-Type: application/json
Authorization: Bearer cae4cbbe40632b573e753da6ff00997a179c7dbf81d89f23eb83f0b0c6ee75e2
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
      "user_id": 506,
      "feedbackable_id": 63,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:55.222Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 505,
      "feedbackable_id": 63,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T19:31:55.211Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/63/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cae4cbbe40632b573e753da6ff00997a179c7dbf81d89f23eb83f0b0c6ee75e2"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/2/votes
Content-Type: application/json
Authorization: Bearer 7aa67a924c0c47c1a2a40b99cc471a059e5298b5a5796de37e0eda02e279c4a3
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
      "votable_id": 2,
      "user_id": 26
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 25
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 2,
      "user_id": 24
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/2/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7aa67a924c0c47c1a2a40b99cc471a059e5298b5a5796de37e0eda02e279c4a3"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/127/republish
Content-Type: application/json
Authorization: Bearer 0c8b28a54ed641cdb425e49390d4282c050bc0d9bf85e271e7494cc0210fb929
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
curl "api.goskive.com/v2/questions/127/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c8b28a54ed641cdb425e49390d4282c050bc0d9bf85e271e7494cc0210fb929"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/111/bookmark
Content-Type: application/json
Authorization: Bearer ddf5b5a8aa32902c43fb9d3c621686723d5667b02d84121bca999521dbfed68c
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddf5b5a8aa32902c43fb9d3c621686723d5667b02d84121bca999521dbfed68c"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/109
Content-Type: application/json
Authorization: Bearer 1357c6c41ee4939ccd9250b0573cdf27c6fb3dbd971af0dbcc126e5b627f1bf5
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
	-H "Authorization: Bearer 1357c6c41ee4939ccd9250b0573cdf27c6fb3dbd971af0dbcc126e5b627f1bf5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/110/downvote
Content-Type: application/json
Authorization: Bearer b42f7b1459540b56230227c6bbecf73f39b6feaf1b2225ee975a2317a602ab0a
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b42f7b1459540b56230227c6bbecf73f39b6feaf1b2225ee975a2317a602ab0a"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/108
Content-Type: application/json
Authorization: Bearer 1f7361ee2fcff92065324f081864859d63d8dd8641103aecbda6535e52c36128
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
    "author_id": 787,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:32:22.152Z",
    "created_at": "2016-10-20T19:32:22.021Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/questions/108" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f7361ee2fcff92065324f081864859d63d8dd8641103aecbda6535e52c36128"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/130/report
Content-Type: application/json
Authorization: Bearer 99c95ed8bb1f8d340d98db7731665447e634ff9c731f810bc8514220188335b1
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/130/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99c95ed8bb1f8d340d98db7731665447e634ff9c731f810bc8514220188335b1"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/132/bookmark
Content-Type: application/json
Authorization: Bearer 4acd04e8e4ed4168f82b1888aff2b8d65b2c52605fc11040448f85c981a81f39
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/132/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4acd04e8e4ed4168f82b1888aff2b8d65b2c52605fc11040448f85c981a81f39"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/131
Content-Type: application/json
Authorization: Bearer fb74447f8a85d1c2bce2355a6478a8ead3c2acadb6aea2f15ea1039fdfd20cab
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":131,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-20T19:32:30.092Z","updated_at":"2016-10-20T19:32:30.232Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":192,"author_id":861,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 131,
    "obfuscated_id": "gCw8isdgMKE",
    "author_id": 861,
    "chapter_id": 192,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-20T19:32:30.368Z",
    "created_at": "2016-10-20T19:32:30.092Z",
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
    "question": "{\"id\"=>131, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-20T19:32:30.092Z\", \"updated_at\"=>\"2016-10-20T19:32:30.232Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>192, \"author_id\"=>861, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 264,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 265,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 266,
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
curl "api.goskive.com/v2/questions/131" -d '{"question":{"question":{"id":131,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-20T19:32:30.092Z","updated_at":"2016-10-20T19:32:30.232Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":192,"author_id":861,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb74447f8a85d1c2bce2355a6478a8ead3c2acadb6aea2f15ea1039fdfd20cab"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/129/upvote
Content-Type: application/json
Authorization: Bearer 6894b8068393e6ddf978ec6c05952fae697437b0c13c6973ceff7f3de1f5674d
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/129/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6894b8068393e6ddf978ec6c05952fae697437b0c13c6973ceff7f3de1f5674d"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 927b8e65c56e5ee63d8dc00d667e72f3dc06f1edd7831fb51ea967db4c5ae1f4
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
      "creator_id": 742,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 212,
      "additional_university_ids": [

      ],
      "topic_id": 239,
      "discipline_id": 239,
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
      "updated_at": "2016-10-20T19:32:19.576Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 927b8e65c56e5ee63d8dc00d667e72f3dc06f1edd7831fb51ea967db4c5ae1f4"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b405a8392ff75cf8d85afcca8f287a340e4ef31d1eb96ce824c7e9b98584fe67
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
      "id": 215,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-195",
      "html_url": "https://goskive.com/university/uni-195",
      "slug": "uni-195",
      "name": "National School of Pizza",
      "short_name": "Uni 195",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/01fa4d063f9dcdd8de74fbee940bd3d5be1e97eb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/899bdee5fe1909868aae15fc75d04a4125a1dead.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T19:32:19.828Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 214,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-194",
      "html_url": "https://goskive.com/university/uni-194",
      "slug": "uni-194",
      "name": "National School of Pastry",
      "short_name": "Uni 194",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8efdb8264c7f4a28df19e2f795afb7290e8efd49.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ad9fd4421755460f2afe46727848c3fa475fafa0.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T19:32:19.813Z",
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
	-H "Authorization: Bearer b405a8392ff75cf8d85afcca8f287a340e4ef31d1eb96ce824c7e9b98584fe67"
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
      "id": 48,
      "name": "Phased actuating infrastructure",
      "name_translations": {
        "en": "Phased actuating infrastructure"
      },
      "discipline_id": 48
    },
    {
      "id": 49,
      "name": "Exclusive 3rd generation productivity",
      "name_translations": {
        "en": "Exclusive 3rd generation productivity"
      },
      "discipline_id": 49
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
GET /v2/topics/47
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
    "id": 47,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 47
  }
}
```



```shell
curl "api.goskive.com/v2/topics/47" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 3a6b12ef54b5c31ab2e3a0c9c202840ce829637a5779dfee4edcec7a6d47a452
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
      "id": 10,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-10",
      "html_url": "https://goskive.com/university/uni-10",
      "slug": "uni-10",
      "name": "University 10",
      "short_name": "Uni 10",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/907b97acad454546ae110f7cad7c8a133f868482.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/590c7f8b9d9c518ab5b695e676ac1e98a5606cc2.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T19:31:20.376Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-11",
      "html_url": "https://goskive.com/university/uni-11",
      "slug": "uni-11",
      "name": "University 11",
      "short_name": "Uni 11",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/87ba84ab1107072a961e4e0676ef38b11ea6bc3e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b1af93f712353ded5aa14b0defbbe8f407c0d997.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T19:31:20.390Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 12,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-12",
      "html_url": "https://goskive.com/university/uni-12",
      "slug": "uni-12",
      "name": "University 12",
      "short_name": "Uni 12",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5bcbb5f32f57a2edaadd2dbcddd13bce2e6da770.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/35e26355049fa64a351bfa2fbc72aee98aac48f5.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-20T19:31:20.405Z",
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
	-H "Authorization: Bearer 3a6b12ef54b5c31ab2e3a0c9c202840ce829637a5779dfee4edcec7a6d47a452"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 4b33807535008339c04b44a8472cf3fe0d939d5102537430ea18fce1a0be81d3
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
    "id": 13,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0807ab42117f07e0ba6d1aca79325e2f65ec600d.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1203abbdb8e1c4445cac833cf83747bef4ae8006.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-20T19:31:20.517Z",
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
	-H "Authorization: Bearer 4b33807535008339c04b44a8472cf3fe0d939d5102537430ea18fce1a0be81d3"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 27c06f7d1d34e92148ac1a596cc3eb690ace133171da180884b9b2b4d8975875
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":186,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 572,
    "id": 181,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "topic_id": 186,
    "discipline_id": 186,
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
    "chapters_updated_at": "2016-10-20T19:32:01.398Z",
    "updated_at": "2016-10-20T19:32:01.531Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 118,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-20T19:32:01.487Z",
        "course_id": 181,
        "author_id": 572,
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
        "id": 119,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-20T19:32:01.504Z",
        "course_id": 181,
        "author_id": 572,
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
        "id": 120,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-20T19:32:01.521Z",
        "course_id": 181,
        "author_id": 572,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":186,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27c06f7d1d34e92148ac1a596cc3eb690ace133171da180884b9b2b4d8975875"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9e11efd5162bf146fe4bddc5df2116f32add9c39408b4520030c5a9cf3e5aebc
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":185,"published":false}}
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
    "creator_id": 571,
    "id": 180,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "topic_id": 185,
    "discipline_id": 185,
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
    "updated_at": "2016-10-20T19:32:01.365Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":185,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e11efd5162bf146fe4bddc5df2116f32add9c39408b4520030c5a9cf3e5aebc"
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
      "creator_id": 543,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 161,
      "discipline_id": 161,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
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
      "updated_at": "2016-10-20T19:31:58.815Z",
      "shortname": "fu-course-134"
    },
    {
      "creator_id": 543,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 162,
      "discipline_id": 162,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
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
      "chapters_updated_at": "2016-10-20T19:31:59.108Z",
      "updated_at": "2016-10-20T19:31:59.115Z",
      "shortname": "fu-course-135"
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
Authorization: Bearer edb359f1206dbd2869111636503bc9b69cedf8e25ffb19cb3e250ed71e97596c
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
      "creator_id": 550,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 169,
      "discipline_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "updated_at": "2016-10-20T19:31:59.559Z",
      "shortname": "fu-course-142"
    },
    {
      "creator_id": 550,
      "id": 165,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-143",
      "html_url": "https://goskive.com/course/fu-course-143",
      "slug": "fu-course-143",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 170,
      "discipline_id": 170,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
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
      "chapters_updated_at": "2016-10-20T19:31:59.839Z",
      "updated_at": "2016-10-20T19:31:59.845Z",
      "shortname": "fu-course-143"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edb359f1206dbd2869111636503bc9b69cedf8e25ffb19cb3e250ed71e97596c"
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
      "creator_id": 548,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "discipline_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
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
      "updated_at": "2016-10-20T19:31:59.348Z",
      "shortname": "fu-course-138"
    },
    {
      "creator_id": 548,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 155,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 166,
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
      "updated_at": "2016-10-20T19:31:59.385Z",
      "shortname": "fu-course-139"
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
Authorization: Bearer 2701d71d1aa86b3057d89ff9a91e93773fe5b4fe523a07d5db67eacb9016a1ae
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
      "creator_id": 557,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 158,
      "additional_university_ids": [

      ],
      "topic_id": 173,
      "discipline_id": 173,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
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
      "updated_at": "2016-10-20T19:32:00.113Z",
      "shortname": "fu-course-146"
    },
    {
      "creator_id": 557,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 158,
      "additional_university_ids": [

      ],
      "topic_id": 174,
      "discipline_id": 174,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
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
      "updated_at": "2016-10-20T19:32:00.152Z",
      "shortname": "fu-course-147"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2701d71d1aa86b3057d89ff9a91e93773fe5b4fe523a07d5db67eacb9016a1ae"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 74f1dfce84d60cfcd8818ae8be2dfd9eef8f92ef4160214212d8ba245f4d88cb
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
  "id": 616,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-20T19:32:04.970Z",
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
	-H "Authorization: Bearer 74f1dfce84d60cfcd8818ae8be2dfd9eef8f92ef4160214212d8ba245f4d88cb"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/461
Content-Type: application/json
Authorization: Bearer 54de0406cd40dffa246dfb00b45c5a46c5c29a8f13d722b8becfd1ce3b52921f
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
    "id": 461,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 133,
    "fields_of_study": [
      131,
      132
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-20T19:31:51.793Z",
    "updated_at": "2016-10-20T19:31:51.793Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/461" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54de0406cd40dffa246dfb00b45c5a46c5c29a8f13d722b8becfd1ce3b52921f"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/463
Content-Type: application/json
Authorization: Bearer 0104b735d9f3dd718050dfc4a3def2c14be2f244356a1251f91f675221d892bc
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
    "id": 463,
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
    "created_at": "2016-10-20T19:31:51.875Z",
    "updated_at": "2016-10-20T19:31:51.875Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/463" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0104b735d9f3dd718050dfc4a3def2c14be2f244356a1251f91f675221d892bc"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/14
Content-Type: application/json
Authorization: Bearer 2b344bfe66e90740aaf4bf7efab5fafa566acc5e7b6539f9c3cab8d323440af8
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b344bfe66e90740aaf4bf7efab5fafa566acc5e7b6539f9c3cab8d323440af8"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/15
Content-Type: application/json
Authorization: Bearer ea6b9df0420c13e376409b937a4ff95b06acedb0558dd26f0685edb3ee8437f2
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
    "votable_id": 57,
    "user_id": 469
  }
}
```



```shell
curl "api.goskive.com/v2/votes/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea6b9df0420c13e376409b937a4ff95b06acedb0558dd26f0685edb3ee8437f2"
```
