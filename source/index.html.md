---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# Authentication

## Authentication error on create

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic YTkyYzg5NDlkMTMzYzgwNWJmOTBhZWY5OWE4NzhhODg1NmQ3OTg3NTI2ZTQ2
ODUxYjEwMjA1MGZhMTNmYWExZToyMjJkNWQ3YTlkYzQ2MDY0ZGRkZGQwZjgx
OGQ2MTk0M2RiYThlNjNkOGRlYjMzMTY4MWU3ODc5YTU3NjMyYTRm

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
401 Unauthorized
```


```json
{
  "error": "invalid_resource_owner",
  "error_description": "The provided resource owner credentials are not valid, or resource owner cannot be found"
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u a92c8949d133c805bf90aef99a878a8856d7987526e46851b102050fa13faa1e:222d5d7a9dc46064ddddd0f818d61943dba8e63d8deb331681e7879a57632a4f
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic N2U0M2EyNzQyNTFiOTI2ODA4YmYxYWEwNDMzNDNkYjc2YmIzOTMxNjE3Nzc4
ZDc5NjM5MTBiODljMTI5MTVkZTpiNTUyODNkZTg1MGJiNTc1ZWY1YjVhZDQ4
MWQyY2I2ZTlhODAzMWYyNjg4ZGYzZjU0NGFjYjVmY2E1YzM1YzJl

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
	-u 7e43a274251b926808bf1aa043343db76bb3931617778d7963910b89c12915de:b55283de850bb575ef5b5ad481d2cb6e9a8031f2688df3f544acb5fca5c35c2e
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

Credentials for another tenant gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ddcbbb491ee1ea8d34b6f9413f287cac25cc38294a6375304c0f6b2c9d9bf88f","client_secret":"b40d7d5d91aa61161dd104a553e9a39ccf6bf47a47f1643c8f196816175eeb64"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"ddcbbb491ee1ea8d34b6f9413f287cac25cc38294a6375304c0f6b2c9d9bf88f","client_secret":"b40d7d5d91aa61161dd104a553e9a39ccf6bf47a47f1643c8f196816175eeb64"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"9fb74dd0210ffb29d65a864a2191a03d1a3ce5aceac7b8fc878fb0576a005436","client_secret":"74fb755c6249442436bc35ededb908e372dd42b081d212e6b4a2d41049f81b02"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"9fb74dd0210ffb29d65a864a2191a03d1a3ce5aceac7b8fc878fb0576a005436","client_secret":"74fb755c6249442436bc35ededb908e372dd42b081d212e6b4a2d41049f81b02"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"426d5fe36684a0cbc158244bbc53829b62e69e0c4e298132e4a524a8750a1474","client_secret":"245dfcdd254bf80eb77dc48f089cc36e3b16bcf864121f99404c3434f8bd6663"}
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
  "access_token": "56015ddd30ae84d585c490a30d9db1930b1dcd226d8b7183f31a93b9053a4368",
  "token_type": "bearer",
  "created_at": 1475758671
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"426d5fe36684a0cbc158244bbc53829b62e69e0c4e298132e4a524a8750a1474","client_secret":"245dfcdd254bf80eb77dc48f089cc36e3b16bcf864121f99404c3434f8bd6663"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic N2QwYzk4MTM2NTVmODRkMDk5YjA5ZmZjNzFjMDRhOWYzOWNlNjJhMmNmNjY0
YzVjMDdhY2NkNmZlZWM0NjM3NDoyMzFjNzhhMGUzODQ5ZWY0ZTAzZDkwOTlk
ZjkzZjJkMTFlZjVkYTZhMzRhMzY5NDY3NDY2ZGNiZWNkZDRmNDc0

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
  "access_token": "4e79f50df2b18573c16f49cd39591a4e60955790451970b436c615cc87875a92",
  "token_type": "bearer",
  "created_at": 1475758678
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 7d0c9813655f84d099b09ffc71c04a9f39ce62a2cf664c5c07accd6feec46374:231c78a0e3849ef4e03d9099df93f2d11ef5da6a34a369467466dcbecdd4f474
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a0d60ce4635743f13423966b4e4ca13f3cb6e56102dc52aa0276dd242c5283cc","client_secret":"01ec4799821cb7b8aa032d6a7093c23db0a64b1dd942ed0c8d29ed3009381d47"}
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
  "access_token": "6c4ca96afaa37bca49dfa2cd20dfb3fc9752d67fbd41d79c318db353b3346639",
  "token_type": "bearer",
  "created_at": 1475758678
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"a0d60ce4635743f13423966b4e4ca13f3cb6e56102dc52aa0276dd242c5283cc","client_secret":"01ec4799821cb7b8aa032d6a7093c23db0a64b1dd942ed0c8d29ed3009381d47"}' -X POST \
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
Authorization: Bearer 191eb0aab6d3989e67918223fc8da902cc4df9c2e6f0361df0f54d087d1c59b1
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
    "company_id": 28,
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
	-H "Authorization: Bearer 191eb0aab6d3989e67918223fc8da902cc4df9c2e6f0361df0f54d087d1c59b1"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/127/flashcards
Content-Type: application/json
Authorization: Bearer 1af809caa92023960328523757ba2a9d800796d9331eb813537672fffbf80b07
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":127,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 61,
    "obfuscated_id": "Acd5zhQoy8g",
    "author_id": 740,
    "chapter_id": 127,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:57:45.265Z",
    "created_at": "2016-10-06T12:57:45.265Z",
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
curl "api.goskive.com/v2/chapters/127/flashcards" -d '{"flashcard":{"chapter_id":127,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1af809caa92023960328523757ba2a9d800796d9331eb813537672fffbf80b07"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/128/flashcards
Content-Type: application/json
Authorization: Bearer 12b8623049d4197f010762e36b603cf4c3f008beb808beec9c194c9cf11690ec
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
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 741,
      "chapter_id": 128,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:45.424Z",
      "created_at": "2016-10-06T12:57:45.424Z",
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
      "author_id": 741,
      "chapter_id": 128,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:45.459Z",
      "created_at": "2016-10-06T12:57:45.459Z",
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 741,
      "chapter_id": 128,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:45.493Z",
      "created_at": "2016-10-06T12:57:45.493Z",
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
curl "api.goskive.com/v2/chapters/128/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12b8623049d4197f010762e36b603cf4c3f008beb808beec9c194c9cf11690ec"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/131/questions
Content-Type: application/json
Authorization: Bearer 33f7f40bdadb44ab8e0ead57662764b58d4dfdc812e8769c52f02570e26e8edf
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 110,
    "obfuscated_id": "55JK4PuG2Hk",
    "author_id": 752,
    "chapter_id": 131,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:57:46.234Z",
    "created_at": "2016-10-06T12:57:46.234Z",
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
        "id": 221,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 222,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 223,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 224,
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
curl "api.goskive.com/v2/chapters/131/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":131,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33f7f40bdadb44ab8e0ead57662764b58d4dfdc812e8769c52f02570e26e8edf"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/132/questions
Content-Type: application/json
Authorization: Bearer 57e9314721deeb23f6d24b1b96587e9074b5089fe381af69445f68978eaca9e0
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":132,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 111,
    "obfuscated_id": "G-D-sgMUtTw",
    "author_id": 755,
    "chapter_id": 132,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:57:46.699Z",
    "created_at": "2016-10-06T12:57:46.699Z",
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
        "id": 225,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 226,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/132/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":132,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57e9314721deeb23f6d24b1b96587e9074b5089fe381af69445f68978eaca9e0"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/133/questions
Content-Type: application/json
Authorization: Bearer 403a85bb31cf6f0ecc27dd864f1abefbd48dfebbf1117229d4d5917a4239c305
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":133,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 112,
    "obfuscated_id": "7Qwj1ZvbWUI",
    "author_id": 758,
    "chapter_id": 133,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:57:47.015Z",
    "created_at": "2016-10-06T12:57:47.015Z",
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
        "id": 227,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 228,
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
curl "api.goskive.com/v2/chapters/133/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":133,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 403a85bb31cf6f0ecc27dd864f1abefbd48dfebbf1117229d4d5917a4239c305"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/130/questions
Content-Type: application/json
Authorization: Bearer cc74ac1aa6281a01a83aff8eb15b10f7936b829860736135bce1537c391a8cfd
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":130,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 749,
    "chapter_id": 130,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:57:45.834Z",
    "created_at": "2016-10-06T12:57:45.834Z",
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
        "id": 218,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 219,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 220,
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
curl "api.goskive.com/v2/chapters/130/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":130,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc74ac1aa6281a01a83aff8eb15b10f7936b829860736135bce1537c391a8cfd"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/135/questions
Content-Type: application/json
Authorization: Bearer 76e94620b3331e5b6782d7933cdd402f3e7f541e76b6bf0df70bc05ceb74b3ee
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
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 764,
      "chapter_id": 135,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:47.543Z",
      "created_at": "2016-10-06T12:57:47.433Z",
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
          "id": 229,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 230,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 765,
      "chapter_id": 135,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:47.726Z",
      "created_at": "2016-10-06T12:57:47.613Z",
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
          "id": 231,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 232,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 766,
      "chapter_id": 135,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-06T12:57:47.908Z",
      "created_at": "2016-10-06T12:57:47.798Z",
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
          "id": 233,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 234,
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
curl "api.goskive.com/v2/chapters/135/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76e94620b3331e5b6782d7933cdd402f3e7f541e76b6bf0df70bc05ceb74b3ee"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/89
Content-Type: application/json
Authorization: Bearer c299bd91febed025bbd46f7049b2d81e40bd1e543cf6f36ff62ffed8a6275e41
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
curl "api.goskive.com/v2/chapters/89" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c299bd91febed025bbd46f7049b2d81e40bd1e543cf6f36ff62ffed8a6275e41"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/91
Content-Type: application/json
Authorization: Bearer e90a57a16aa60f30e3647a029ad95e7597789ce35edc01030060a7c2301502ed
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
curl "api.goskive.com/v2/chapters/91" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e90a57a16aa60f30e3647a029ad95e7597789ce35edc01030060a7c2301502ed"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/84
Content-Type: application/json
Authorization: Bearer 4fcf38c2bee4d22208bc8d6ea292870a77ed8115e5b4404fc0252dcf46d12d24
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
curl "api.goskive.com/v2/chapters/84" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4fcf38c2bee4d22208bc8d6ea292870a77ed8115e5b4404fc0252dcf46d12d24"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/90
Content-Type: application/json
Authorization: Bearer 251d5c48e90b3d66915c2292ac240acae8cfe539155b316efaae5439ff89f5a7
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/90" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 251d5c48e90b3d66915c2292ac240acae8cfe539155b316efaae5439ff89f5a7"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/86
Content-Type: application/json
Authorization: Bearer a9be6ee8296fdec28577653f5e57a1b799fdd1bd14e8f6c805c4460f45267d24
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
    "id": 86,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-06T12:57:23.833Z",
    "course_id": 204,
    "author_id": 550,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-06T12:57:23.263Z",
    "questions_updated_at": "2016-10-06T12:57:23.263Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 554,
        "chapter_id": 86,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:23.815Z",
        "created_at": "2016-10-06T12:57:23.815Z",
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
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 552,
        "chapter_id": 86,
        "position": 69,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:23.699Z",
        "created_at": "2016-10-06T12:57:23.570Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/86" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9be6ee8296fdec28577653f5e57a1b799fdd1bd14e8f6c805c4460f45267d24"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/83
Content-Type: application/json
Authorization: Bearer 43c991fca3ff2e6a875528e65e297e9a50a80d45420f10b9a1da02536f404721
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
    "id": 83,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-06T12:57:22.921Z",
    "course_id": 201,
    "author_id": 542,
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
curl "api.goskive.com/v2/chapters/83" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43c991fca3ff2e6a875528e65e297e9a50a80d45420f10b9a1da02536f404721"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/4/replies
Content-Type: application/json
Authorization: Bearer 9813f7281d2c85f1accbcacdacf7b486fddbddfcd98c1ec1a77c8a778cff9489
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
    "id": 5,
    "author_id": 56,
    "reply_to_id": 4,
    "created_at": "2016-10-06T12:56:40.678Z",
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
curl "api.goskive.com/v2/comments/4/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9813f7281d2c85f1accbcacdacf7b486fddbddfcd98c1ec1a77c8a778cff9489"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/3/replies
Content-Type: application/json
Authorization: Bearer 3c836ae58260f498f437bc93f606002bbbcc5bcf81a1c0412747ffab629c18db
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
curl "api.goskive.com/v2/comments/3/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c836ae58260f498f437bc93f606002bbbcc5bcf81a1c0412747ffab629c18db"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 9236ffcd9f437179fca98010e9c15a3df1ffd6c8c9a7d9fbf5cfc945dcb939d1
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
	-H "Authorization: Bearer 9236ffcd9f437179fca98010e9c15a3df1ffd6c8c9a7d9fbf5cfc945dcb939d1"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/12/republish
Content-Type: application/json
Authorization: Bearer 8fe6c013ad2af262acddbc8c34b987b9c4dbfa000cb6a835dc513a16e232a6c7
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
curl "api.goskive.com/v2/comments/12/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8fe6c013ad2af262acddbc8c34b987b9c4dbfa000cb6a835dc513a16e232a6c7"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/51
Content-Type: application/json
Authorization: Bearer afa9fdbca19e6795c0d2b5c536202aaa8b9ecd2b3947b584d0f547e39097a785
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
	-H "Authorization: Bearer afa9fdbca19e6795c0d2b5c536202aaa8b9ecd2b3947b584d0f547e39097a785"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/52/report
Content-Type: application/json
Authorization: Bearer e55501e00e203f96e779de7f3fc0dc06f93d693363e48c34f1f6169658e27d6b
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e55501e00e203f96e779de7f3fc0dc06f93d693363e48c34f1f6169658e27d6b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/4
Content-Type: application/json
Authorization: Bearer bd9fa6cd6e37e395191c27a94cf200c484cc013d8c0c621e9b8c797e27df426e
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
    "updated_at": "2016-10-06T12:56:54.235Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd9fa6cd6e37e395191c27a94cf200c484cc013d8c0c621e9b8c797e27df426e"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 889a03612250c964c64fe71410b9b8f8636ba3dcb78fd460eb610d4ea7b46d48
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
      "id": 5,
      "name": "Fake Company Name 1",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-06T12:56:54.312Z"
    },
    {
      "id": 6,
      "name": "Fake Company Name 2",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-06T12:56:54.316Z"
    },
    {
      "id": 7,
      "name": "Fake Company Name 3",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-06T12:56:54.320Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 889a03612250c964c64fe71410b9b8f8636ba3dcb78fd460eb610d4ea7b46d48"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/2/company_profiles
Content-Type: application/json
Authorization: Bearer f4e31763150834b2b06f03d50d07050ebbdc60f8b272d181ba5ed108a7f728e0
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
curl "api.goskive.com/v2/companies/2/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4e31763150834b2b06f03d50d07050ebbdc60f8b272d181ba5ed108a7f728e0"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/1/company_profiles
Content-Type: application/json
Authorization: Bearer 582b50ee74994f1f0db2e6809bc5db9482408eea7ab792abcd3ecc4d0bc9513a
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
	-H "Authorization: Bearer 582b50ee74994f1f0db2e6809bc5db9482408eea7ab792abcd3ecc4d0bc9513a"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer c219c166cce79660fdec6b334ee9d252515fe39880ec00ab030904040f3afc8c
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
      "company_id": 16,
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
	-H "Authorization: Bearer c219c166cce79660fdec6b334ee9d252515fe39880ec00ab030904040f3afc8c"
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
Authorization: Bearer 1c512146b1a1df604c929e248935ee41aa9b9b3e193036b3bf3d5d34b028a78f
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
	-H "Authorization: Bearer 1c512146b1a1df604c929e248935ee41aa9b9b3e193036b3bf3d5d34b028a78f"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 31051a4a729d53f39dc386491a4a333c02ee7aea66275de12ea703d4853cf8a3
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
    "id": 138,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-06T12:57:48.725Z",
    "course_id": 258,
    "author_id": 779,
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
	-H "Authorization: Bearer 31051a4a729d53f39dc386491a4a333c02ee7aea66275de12ea703d4853cf8a3"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f58682e3bf3525b1f0f91b3ac2fc0dbaa0e31b23be2a905e9b2c21be5f8ce2db
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
      "id": 139,
      "title": "Clever Chapter Title 115",
      "position": 1,
      "updated_at": "2016-10-06T12:57:48.834Z",
      "course_id": 259,
      "author_id": 781,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 140,
      "title": "Clever Chapter Title 116",
      "position": 2,
      "updated_at": "2016-10-06T12:57:48.858Z",
      "course_id": 259,
      "author_id": 782,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 141,
      "title": "Clever Chapter Title 117",
      "position": 3,
      "updated_at": "2016-10-06T12:57:49.097Z",
      "course_id": 259,
      "author_id": 783,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-06T12:57:48.760Z",
      "questions_updated_at": "2016-10-06T12:57:48.760Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f58682e3bf3525b1f0f91b3ac2fc0dbaa0e31b23be2a905e9b2c21be5f8ce2db"
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
      "id": 145,
      "title": "Clever Chapter Title 121",
      "position": 1,
      "updated_at": "2016-10-06T12:57:49.562Z",
      "course_id": 262,
      "author_id": 795,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 146,
      "title": "Clever Chapter Title 122",
      "position": 2,
      "updated_at": "2016-10-06T12:57:49.586Z",
      "course_id": 262,
      "author_id": 796,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 147,
      "title": "Clever Chapter Title 123",
      "position": 3,
      "updated_at": "2016-10-06T12:57:49.824Z",
      "course_id": 262,
      "author_id": 797,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-06T12:57:49.487Z",
      "questions_updated_at": "2016-10-06T12:57:49.487Z",
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
Authorization: Bearer 6356c93d79305c04aec11986c52368f49beb15244ecbdbbb3875453b4d424322
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
      "id": 142,
      "title": "Clever Chapter Title 118",
      "position": 1,
      "updated_at": "2016-10-06T12:57:49.258Z",
      "course_id": 260,
      "author_id": 788,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 143,
      "title": "Clever Chapter Title 119",
      "position": 2,
      "updated_at": "2016-10-06T12:57:49.282Z",
      "course_id": 260,
      "author_id": 789,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 144,
      "title": "Clever Chapter Title 120",
      "position": 3,
      "updated_at": "2016-10-06T12:57:49.307Z",
      "course_id": 260,
      "author_id": 790,
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
	-H "Authorization: Bearer 6356c93d79305c04aec11986c52368f49beb15244ecbdbbb3875453b4d424322"
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
      "id": 148,
      "title": "Clever Chapter Title 124",
      "position": 1,
      "updated_at": "2016-10-06T12:57:49.941Z",
      "course_id": 263,
      "author_id": 801,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 149,
      "title": "Clever Chapter Title 125",
      "position": 2,
      "updated_at": "2016-10-06T12:57:49.965Z",
      "course_id": 263,
      "author_id": 802,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 150,
      "title": "Clever Chapter Title 126",
      "position": 3,
      "updated_at": "2016-10-06T12:57:49.989Z",
      "course_id": 263,
      "author_id": 803,
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
Authorization: Bearer f04a2c3a554c268066d0300b9fe4ef963c27c0ed918889fb04c8a6301b165ff3
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
    "id": 1,
    "course_id": 19,
    "user_id": 94,
    "updated_at": "2016-10-06T12:56:42.867Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f04a2c3a554c268066d0300b9fe4ef963c27c0ed918889fb04c8a6301b165ff3"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer df0e1b3b1f083e57ebcdb0b9ac139101ddb049ca520502a326c73281594233a0
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
      "id": 5,
      "course_id": 23,
      "user_id": 104,
      "updated_at": "2016-10-06T12:56:43.387Z"
    },
    {
      "id": 6,
      "course_id": 23,
      "user_id": 105,
      "updated_at": "2016-10-06T12:56:43.404Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df0e1b3b1f083e57ebcdb0b9ac139101ddb049ca520502a326c73281594233a0"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/115/files
Content-Type: application/json
Authorization: Bearer f4b24922f6ede53b8d4e5e02a691fdffd97eae8c4ddf9d7686eb661cfba0e33d
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
        "id": 345,
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
        "created_at": "2016-10-06T12:57:01.986Z",
        "updated_at": "2016-10-06T12:57:01.986Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-06T12:57:02.000Z",
      "updated_at": "2016-10-06T12:57:02.000Z",
      "course_id": 115,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 346,
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
        "created_at": "2016-10-06T12:57:02.008Z",
        "updated_at": "2016-10-06T12:57:02.008Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-06T12:57:02.017Z",
      "updated_at": "2016-10-06T12:57:02.017Z",
      "course_id": 115,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 347,
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
        "created_at": "2016-10-06T12:57:02.023Z",
        "updated_at": "2016-10-06T12:57:02.023Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-06T12:57:02.031Z",
      "updated_at": "2016-10-06T12:57:02.031Z",
      "course_id": 115,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/115/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4b24922f6ede53b8d4e5e02a691fdffd97eae8c4ddf9d7686eb661cfba0e33d"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/116/files
Content-Type: application/json
Authorization: Bearer d27dedc172744301c97c0d548abac7750cc08ed3fe57d6ef75d32c6593077a07
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
      "id": 350,
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
      "created_at": "2016-10-06T12:57:02.152Z",
      "updated_at": "2016-10-06T12:57:02.152Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-06T12:57:02.182Z",
    "updated_at": "2016-10-06T12:57:02.182Z",
    "course_id": 116,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/116/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d27dedc172744301c97c0d548abac7750cc08ed3fe57d6ef75d32c6593077a07"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/113/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 543294b5f93124c7e4aa284b10715c44f5c202993b5cac9d2393842bc8747193
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
    "key": "cache/16f896cf9073373e040aa2b09467567b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0wNlQxMzo1NzowMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8xNmY4OTZjZjkwNzMzNzNlMDQwYWEyYjA5NDY3NTY3Yi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAwNi9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMDZUMTI1NzAxWiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161006/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161006T125701Z",
    "x-amz-signature": "1cee3ed57243d094a19a69329b78f866aa7177f1706a7c3a10574b8b5b7332fb"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/113/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 543294b5f93124c7e4aa284b10715c44f5c202993b5cac9d2393842bc8747193"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 72d942b193ed1b15075619cb994666b335d3d7d99962a971ee7f2185c6232b7d
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
	-H "Authorization: Bearer 72d942b193ed1b15075619cb994666b335d3d7d99962a971ee7f2185c6232b7d"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c8150f9d174244469ed3e3d45a0bde1995424324889410875e2ca8ab65732236
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
	-H "Authorization: Bearer c8150f9d174244469ed3e3d45a0bde1995424324889410875e2ca8ab65732236"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer f94e7cd42a31ece6369597b1d7d0893497a6333ae4ed9e530e82762e2af1cf7c
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
	-H "Authorization: Bearer f94e7cd42a31ece6369597b1d7d0893497a6333ae4ed9e530e82762e2af1cf7c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 88836f65e5e87b8e8f342ba4d57b7de16c0c5379d37e43cc9b2aae69be72a147
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
	-H "Authorization: Bearer 88836f65e5e87b8e8f342ba4d57b7de16c0c5379d37e43cc9b2aae69be72a147"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 951a8258a4eff3189c465a52dee3696abd310a0db071baa0ecc44da69cfcf674
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
	-H "Authorization: Bearer 951a8258a4eff3189c465a52dee3696abd310a0db071baa0ecc44da69cfcf674"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 8964bfa7d5a1c375d8724aa879fd4b1e183830e1521e3db0cd72711aee9252c2
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
    "creator_id": 513,
    "id": 194,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 178,
    "additional_university_ids": [

    ],
    "topic_id": 204,
    "discipline_id": 205,
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
    "chapters_updated_at": "2016-10-06T12:57:17.668Z",
    "updated_at": "2016-10-06T12:57:19.227Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 75,
        "title": "Clever Chapter Title 72",
        "position": 1,
        "updated_at": "2016-10-06T12:57:19.172Z",
        "course_id": 194,
        "author_id": 513,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-06T12:57:17.668Z",
        "questions_updated_at": "2016-10-06T12:57:17.668Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 76,
        "title": "Clever Chapter Title 73",
        "position": 2,
        "updated_at": "2016-10-06T12:57:19.218Z",
        "course_id": 194,
        "author_id": 513,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-06T12:57:17.668Z",
        "questions_updated_at": "2016-10-06T12:57:17.668Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 514,
        "chapter_id": 75,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:19.001Z",
        "created_at": "2016-10-06T12:57:19.001Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 514,
        "chapter_id": 76,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:19.075Z",
        "created_at": "2016-10-06T12:57:19.075Z",
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
        "author_id": 514,
        "chapter_id": 75,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:19.043Z",
        "created_at": "2016-10-06T12:57:19.043Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 514,
        "chapter_id": 76,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:19.117Z",
        "created_at": "2016-10-06T12:57:19.117Z",
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
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 514,
        "chapter_id": 75,
        "position": 53,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:17.898Z",
        "created_at": "2016-10-06T12:57:17.776Z",
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
            "id": 124,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 125,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 514,
        "chapter_id": 75,
        "position": 54,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:18.077Z",
        "created_at": "2016-10-06T12:57:17.963Z",
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
            "id": 126,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 127,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 514,
        "chapter_id": 76,
        "position": 55,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:18.296Z",
        "created_at": "2016-10-06T12:57:18.164Z",
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
            "id": 128,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 129,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 514,
        "chapter_id": 76,
        "position": 56,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:18.510Z",
        "created_at": "2016-10-06T12:57:18.377Z",
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
            "id": 130,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 131,
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
	-H "Authorization: Bearer 8964bfa7d5a1c375d8724aa879fd4b1e183830e1521e3db0cd72711aee9252c2"
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
    "creator_id": 519,
    "id": 195,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 179,
    "additional_university_ids": [

    ],
    "topic_id": 205,
    "discipline_id": 206,
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
    "chapters_updated_at": "2016-10-06T12:57:19.364Z",
    "updated_at": "2016-10-06T12:57:20.937Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 77,
        "title": "Clever Chapter Title 74",
        "position": 1,
        "updated_at": "2016-10-06T12:57:20.885Z",
        "course_id": 195,
        "author_id": 519,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-06T12:57:19.364Z",
        "questions_updated_at": "2016-10-06T12:57:19.364Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 78,
        "title": "Clever Chapter Title 75",
        "position": 2,
        "updated_at": "2016-10-06T12:57:20.929Z",
        "course_id": 195,
        "author_id": 519,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-06T12:57:19.364Z",
        "questions_updated_at": "2016-10-06T12:57:19.364Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 519,
        "chapter_id": 77,
        "position": 59,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:19.585Z",
        "created_at": "2016-10-06T12:57:19.463Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 519,
        "chapter_id": 78,
        "position": 61,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-06T12:57:20.006Z",
        "created_at": "2016-10-06T12:57:19.879Z",
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
            "id": 140,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 141,
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
PUT /v2/courses/177/pin
Content-Type: application/json
Authorization: Bearer abea63829799482818b5edd897b5698633c9e089a7d14376692349ba34e4cfa0
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/177/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abea63829799482818b5edd897b5698633c9e089a7d14376692349ba34e4cfa0"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/191/pin
Content-Type: application/json
Authorization: Bearer 1723f49a1e1dceeb080876c89de682d5979ec8b70927efcd44951aa31b2748dc
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/191/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1723f49a1e1dceeb080876c89de682d5979ec8b70927efcd44951aa31b2748dc"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 63f61167650392f12f233933d3a09c039a05f9196b6f0dbf0eb539de102fe219
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
    "creator_id": 478,
    "id": 181,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "topic_id": 191,
    "discipline_id": 192,
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
    "updated_at": "2016-10-06T12:57:12.781Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63f61167650392f12f233933d3a09c039a05f9196b6f0dbf0eb539de102fe219"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 212dcf718375761416e3f28ccb727e4a95082d200c89d5fab011d0672282a713
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
    "id": 6,
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
    "created_at": "2016-10-06T12:56:36.193Z",
    "updated_at": "2016-10-06T12:56:36.193Z",
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
	-H "Authorization: Bearer 212dcf718375761416e3f28ccb727e4a95082d200c89d5fab011d0672282a713"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 59044a3a8f871379044239d55f4f1501cfe899356781a3c9228d16fdd8266503
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[1]}
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
    "id": 1,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      1
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-06T12:56:35.419Z",
    "updated_at": "2016-10-06T12:56:35.637Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[1]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59044a3a8f871379044239d55f4f1501cfe899356781a3c9228d16fdd8266503"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 022c5f6de9a6f6565c7963684387957d37602fb5fa2939d621ea60805c816de1
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
    "id": 4,
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
    "created_at": "2016-10-06T12:56:35.862Z",
    "updated_at": "2016-10-06T12:56:35.862Z",
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
	-H "Authorization: Bearer 022c5f6de9a6f6565c7963684387957d37602fb5fa2939d621ea60805c816de1"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f8eb343b5b858fa58cf7ae7eb5a97148f191213070f172e3d457893e12f284df
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[2]}
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
    "id": 2,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      2
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-06T12:56:35.726Z",
    "updated_at": "2016-10-06T12:56:35.726Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[2]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8eb343b5b858fa58cf7ae7eb5a97148f191213070f172e3d457893e12f284df"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 6928937544ba1a36649a93025541d6ed6e3dc2f0abcd3f5b7af3110afb84cda9
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

5
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
    "id": 5,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/71cc93aaf7d948668c0f116a8d6b43cf25676436.jpg",
    "university_id": null,
    "fields_of_study": [
      5
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-06T12:56:35.958Z",
    "updated_at": "2016-10-06T12:56:36.162Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/1ab344bd0d6e781b68b0dc8f5ad68604ae436d57.jpg",
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

5
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 6928937544ba1a36649a93025541d6ed6e3dc2f0abcd3f5b7af3110afb84cda9"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 42bb8c3a34b5dc3d3d0d4a7b86b440ba5276e456d7cdd3b653fde511abb592ad
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
      "bookmarkable_id": 119,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 120,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 121,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42bb8c3a34b5dc3d3d0d4a7b86b440ba5276e456d7cdd3b653fde511abb592ad"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 2058b251c351c53bd0fbc91541871f45908a73bbcf963860a99e2cae3b67f561
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
      "company_id": 36,
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
      "company_id": 37,
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
	-H "Authorization: Bearer 2058b251c351c53bd0fbc91541871f45908a73bbcf963860a99e2cae3b67f561"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer f594a8857239c2f231d1f2a3bd88c77fb786d2aa9f0bb522cac4e523c8d32546
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
      "company_id": 32,
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
	-H "Authorization: Bearer f594a8857239c2f231d1f2a3bd88c77fb786d2aa9f0bb522cac4e523c8d32546"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer b43bc4772e90ed518f4a59671a0a0bc2a2594d1878161e57ae12bb76cadd9dfb
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
      "creator_id": 324,
      "id": 103,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-97",
      "html_url": "https://goskive.com/course/mit-course-97",
      "slug": "mit-course-97",
      "university_id": 108,
      "additional_university_ids": [

      ],
      "topic_id": 113,
      "discipline_id": 114,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 97",
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
      "updated_at": "2016-10-06T12:57:00.083Z",
      "shortname": "mit-course-97"
    },
    {
      "creator_id": 325,
      "id": 104,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-98",
      "html_url": "https://goskive.com/course/mit-course-98",
      "slug": "mit-course-98",
      "university_id": 109,
      "additional_university_ids": [

      ],
      "topic_id": 114,
      "discipline_id": 115,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 98",
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
      "updated_at": "2016-10-06T12:57:00.163Z",
      "shortname": "mit-course-98"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b43bc4772e90ed518f4a59671a0a0bc2a2594d1878161e57ae12bb76cadd9dfb"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a3eb25a413451c9d5b38c3a9021b07b79461136a42097c3cf98cda30efb36e90
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
      "company_id": 13,
      "company": {
        "id": 13,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-06T12:56:54.784Z"
      },
      "created_at": "2016-10-06T12:56:54.788Z",
      "updated_at": "2016-10-06T12:56:54.788Z",
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
      "company_id": 14,
      "company": {
        "id": 14,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-06T12:56:54.797Z"
      },
      "created_at": "2016-10-06T12:56:54.800Z",
      "updated_at": "2016-10-06T12:56:54.800Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3eb25a413451c9d5b38c3a9021b07b79461136a42097c3cf98cda30efb36e90"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 50ef4e816bccce17b2858a61e8b47cf2894b311c9567cba4b916c369309c2891
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
      "company_id": 9,
      "company": {
        "id": 9,
        "name": "Fake Company Name 5",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-06T12:56:54.502Z"
      },
      "created_at": "2016-10-06T12:56:54.507Z",
      "updated_at": "2016-10-06T12:56:54.507Z",
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-06T12:56:54.522Z"
      },
      "created_at": "2016-10-06T12:56:54.526Z",
      "updated_at": "2016-10-06T12:56:54.526Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50ef4e816bccce17b2858a61e8b47cf2894b311c9567cba4b916c369309c2891"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer f5fd22c185013028db8da19aafff932e643a53796fd25f9d1c3cf55fe7a533e9
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
      "id": 12,
      "created_at": "2016-10-06T12:57:02.524Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 54,
      "updated_at": "2016-10-06T12:57:02.638Z",
      "author_id": "358",
      "thread_subject_id": "118",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 13,
      "created_at": "2016-10-06T12:57:02.625Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-10-06T12:57:02.641Z",
      "author_id": "361",
      "thread_subject_id": "119",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 14,
      "created_at": "2016-10-06T12:57:03.027Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-06T12:57:03.027Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 15,
      "created_at": "2016-10-06T12:57:03.412Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-10-06T12:57:03.412Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 16,
      "created_at": "2016-10-06T12:57:03.795Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-10-06T12:57:03.795Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 17,
      "created_at": "2016-10-06T12:57:04.096Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 40,
      "updated_at": "2016-10-06T12:57:04.096Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 18,
      "created_at": "2016-10-06T12:57:04.403Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 41,
      "updated_at": "2016-10-06T12:57:04.403Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 19,
      "created_at": "2016-10-06T12:57:04.697Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 42,
      "updated_at": "2016-10-06T12:57:04.697Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5fd22c185013028db8da19aafff932e643a53796fd25f9d1c3cf55fe7a533e9"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/11
Content-Type: application/json
Authorization: Bearer fcaf93a74297ab3021164fed7bc21a78ef1c991ca1a49a48a2013300f8005305
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-06T12:47:02.000Z"}}
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
    "id": 11,
    "created_at": "2016-10-06T12:57:02.313Z",
    "read_at": "2016-10-06T12:47:02.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 53,
    "updated_at": "2016-10-06T12:57:02.370Z",
    "author_id": "353",
    "thread_subject_id": "117",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/11" -d '{"notification":{"read_at":"2016-10-06T12:47:02.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcaf93a74297ab3021164fed7bc21a78ef1c991ca1a49a48a2013300f8005305"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 63416864c77d9d7d1b94affd7a3c3b3b446be44a949353068f1568c614f521f3
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
      "course_updated_at": "2016-10-06T12:56:59.750Z",
      "course_published": true,
      "updated_at": "2016-10-06T12:56:59.743Z"
    },
    {
      "id": 4,
      "course_id": 101,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-06T12:56:59.830Z",
      "course_published": true,
      "updated_at": "2016-10-06T12:56:59.823Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63416864c77d9d7d1b94affd7a3c3b3b446be44a949353068f1568c614f521f3"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 9648e7e44cfae3387876918ffa74b0e94926c32337b34c15fb39cdfd36ab03c8
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
    "course_updated_at": "2016-10-06T12:56:59.956Z",
    "course_published": true,
    "updated_at": "2016-10-06T12:56:59.949Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9648e7e44cfae3387876918ffa74b0e94926c32337b34c15fb39cdfd36ab03c8"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer bd1cb5f2fedf7d7509fb3221a4167d1a7daf2853a6fbccfa1489fe1de6ec2d1c
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
    "course_updated_at": "2016-10-06T12:56:59.609Z",
    "course_published": true,
    "updated_at": "2016-10-06T12:56:59.598Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd1cb5f2fedf7d7509fb3221a4167d1a7daf2853a6fbccfa1489fe1de6ec2d1c"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 8cd0df010e6cb598eadfa859df4654afbbe53f0f4b5475f6cce946145e0df23b
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
      "id": 13,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 102,
      "user_id": 706
    },
    {
      "id": 14,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 103,
      "user_id": 706
    },
    {
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 104,
      "user_id": 706
    },
    {
      "id": 16,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 105,
      "user_id": 706
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cd0df010e6cb598eadfa859df4654afbbe53f0f4b5475f6cce946145e0df23b"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/36
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
    "id": 36,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 36,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 36
      },
      {
        "id": 37,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 36
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/36" -X GET \
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
      "id": 37,
      "name": "Cross-platform even-keeled framework",
      "name_translations": {
        "en": "Cross-platform even-keeled framework"
      }
    },
    {
      "id": 38,
      "name": "Team-oriented explicit moratorium",
      "name_translations": {
        "en": "Team-oriented explicit moratorium"
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
PATCH /v2/feedbacks/24/close
Content-Type: application/json
Authorization: Bearer dd26a462fe35cd6355f303d2d1616c1bbed4ce4e12d1c55614eaa691d1047b17
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
    "id": 24,
    "user_id": 610,
    "feedbackable_id": 58,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-06T12:57:27.426Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/24/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dd26a462fe35cd6355f303d2d1616c1bbed4ce4e12d1c55614eaa691d1047b17"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/20/fix
Content-Type: application/json
Authorization: Bearer bcc146070f252df256fc002216d49047ccf682a05113588099e8f7aaf1b83dc1
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
    "id": 20,
    "user_id": 588,
    "feedbackable_id": 54,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-06T12:57:26.188Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/20/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcc146070f252df256fc002216d49047ccf682a05113588099e8f7aaf1b83dc1"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/22
Content-Type: application/json
Authorization: Bearer 438f18f39ede13cd5f77b975b1977e9d259ea412b0f09477b125c90e00d10288
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
    "id": 22,
    "user_id": 598,
    "feedbackable_id": 56,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-06T12:57:26.920Z",
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
curl "api.goskive.com/v2/feedbacks/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 438f18f39ede13cd5f77b975b1977e9d259ea412b0f09477b125c90e00d10288"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/18/fix
Content-Type: application/json
Authorization: Bearer eaa0afee14805d5fe1ee3d95a9ac264ca6318b8f75eb57514a20ad0192e2916c
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
curl "api.goskive.com/v2/feedbacks/18/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaa0afee14805d5fe1ee3d95a9ac264ca6318b8f75eb57514a20ad0192e2916c"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/19/fix
Content-Type: application/json
Authorization: Bearer 6fea8e8ea44989fc0ab3c8705f7e4701dd13f1d521daff38ed0dfe4d1bcc120b
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
curl "api.goskive.com/v2/feedbacks/19/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6fea8e8ea44989fc0ab3c8705f7e4701dd13f1d521daff38ed0dfe4d1bcc120b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/26/close
Content-Type: application/json
Authorization: Bearer d9f8f84523ad4ffedd682834b4133795888cc5cb101a9be8e0ad6d3cfdf73dd1
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
curl "api.goskive.com/v2/feedbacks/26/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d9f8f84523ad4ffedd682834b4133795888cc5cb101a9be8e0ad6d3cfdf73dd1"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/23
Content-Type: application/json
Authorization: Bearer f7ffbe5ae92ccd52d453736b461d071d535a1937926593a6f7992f09dd9b0d89
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
    "id": 23,
    "user_id": 603,
    "feedbackable_id": 57,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-06T12:57:27.223Z",
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
curl "api.goskive.com/v2/feedbacks/23" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7ffbe5ae92ccd52d453736b461d071d535a1937926593a6f7992f09dd9b0d89"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer e1143b7f0d345439faa75ed05ee80e53d2a8201d774257e64420683b13837e35
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Authorization: Bearer e1143b7f0d345439faa75ed05ee80e53d2a8201d774257e64420683b13837e35" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer 1dd4b4b0d7dcc6f0c7c961fdb7d543a5043f1c3e73a52dd19dc6424ca309112d
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
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Authorization: Bearer 1dd4b4b0d7dcc6f0c7c961fdb7d543a5043f1c3e73a52dd19dc6424ca309112d" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/10
Authorization: Bearer 367b962a6e41b2121c6d3c8d446585ca6e4fc5765f39460ed36f9802817a33d2
```

`GET /v2/files/:file_id`

#### Parameters


None known.


### Response

```
Content-Type: text/html; charset=utf-8
302 Found
```


```json
<html><body>You are being <a href="https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/1891644779408a46f381388a25e14d58.pdf?response-content-disposition=attachment%3B%20filename%3Dexample.pdf&amp;X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161006%2Feu-west-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20161006T125705Z&amp;X-Amz-Expires=900&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=9ca54f634d31a2d7d524311972d8a24ac73cbbea3fe7f30f5d38218e6271e45f">redirected</a>.</body></html>
```



```shell
curl "api.goskive.com/v2/files/10" -X GET \
	-H "Authorization: Bearer 367b962a6e41b2121c6d3c8d446585ca6e4fc5765f39460ed36f9802817a33d2"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Authorization: Bearer 95ca13d58512c6b296ba47c38892caedf33bc168704ce1fa04fb7a7196a05530
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
    "id": 11,
    "uploader": {
      "id": 401,
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
      "created_at": "2016-10-06T12:57:05.576Z",
      "updated_at": "2016-10-06T12:57:05.576Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-06T12:57:05.655Z",
    "updated_at": "2016-10-06T12:57:05.655Z",
    "course_id": 132,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Authorization: Bearer 95ca13d58512c6b296ba47c38892caedf33bc168704ce1fa04fb7a7196a05530" \
	-H "Content-Type: application/json"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/8/preview
Authorization: Bearer eddd855a5e8bd56e297ca8b319889ef23b26aa8591f9b12648d976908c18c7dc
```

`GET /v2/files/:file_id/preview`

#### Parameters


None known.


### Response

```
Content-Type: text/html; charset=utf-8
302 Found
```


```json
<html><body>You are being <a href="https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/926cbd43892fd4636c1994e8283d693d.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&amp;X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161006%2Feu-west-1%2Fs3%2Faws4_request&amp;X-Amz-Date=20161006T125705Z&amp;X-Amz-Expires=900&amp;X-Amz-SignedHeaders=host&amp;X-Amz-Signature=1c28f7fcd4e5b318ba25a4ef8f7072a0eb3894ec70cdfeec46112070b50205f3">redirected</a>.</body></html>
```



```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Authorization: Bearer eddd855a5e8bd56e297ca8b319889ef23b26aa8591f9b12648d976908c18c7dc"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/9/report
Authorization: Bearer cc4dca02d6970a7075b9d9a8c2f5e21a3589dc927b2e83498e2f51cdc0708c2a
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
curl "api.goskive.com/v2/files/9/report" -d '' -X PUT \
	-H "Authorization: Bearer cc4dca02d6970a7075b9d9a8c2f5e21a3589dc927b2e83498e2f51cdc0708c2a" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer 674bf75d2982e8011cb0c8fd9eef11c996b0f1966a4dcf19d05a66487f09dabe
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
    "id": 11,
    "author_id": 129,
    "reply_to_id": null,
    "created_at": "2016-10-06T12:56:45.441Z",
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
curl "api.goskive.com/v2/flashcards/13/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 674bf75d2982e8011cb0c8fd9eef11c996b0f1966a4dcf19d05a66487f09dabe"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer 46358904d16f16011ab03a8496bfee079d0a9d476c211d55c781721ef895a460
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
    "author_id": 123,
    "reply_to_id": null,
    "created_at": "2016-10-06T12:56:44.907Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 17,
      "user_id": 123,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:56:44.905Z",
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
curl "api.goskive.com/v2/flashcards/11/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46358904d16f16011ab03a8496bfee079d0a9d476c211d55c781721ef895a460"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer beaf92e67730e29d5c869567fb77085519822c9f6dee631041a63c72b5d5b0d7
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
      "author_id": 118,
      "reply_to_id": null,
      "created_at": "2016-10-06T12:56:44.467Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 119,
      "reply_to_id": null,
      "created_at": "2016-10-06T12:56:44.487Z",
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
	-H "Authorization: Bearer beaf92e67730e29d5c869567fb77085519822c9f6dee631041a63c72b5d5b0d7"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer 383bd4f8f76b2bd83a98eb6b05f773c82a0efe578f7cd98c1e5e7a3dc0eda828
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
curl "api.goskive.com/v2/flashcards/12/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 383bd4f8f76b2bd83a98eb6b05f773c82a0efe578f7cd98c1e5e7a3dc0eda828"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/1/feedbacks
Content-Type: application/json
Authorization: Bearer 1ac1c5de25bd92ad4c8bed2422c1aece114fa13a47fe56bfbe8f42b95cdef6ce
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
    "user_id": 57,
    "feedbackable_id": 1,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-06T12:56:41.011Z",
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
curl "api.goskive.com/v2/flashcards/1/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ac1c5de25bd92ad4c8bed2422c1aece114fa13a47fe56bfbe8f42b95cdef6ce"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/6/feedbacks
Content-Type: application/json
Authorization: Bearer 133777f02987585b9a2a07cf98be1ed73cf725679d5a87d190a4190b3486c2e7
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
      "id": 14,
      "user_id": 84,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:56:42.313Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 83,
      "feedbackable_id": 6,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:56:42.301Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/6/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 133777f02987585b9a2a07cf98be1ed73cf725679d5a87d190a4190b3486c2e7"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/16/votes
Content-Type: application/json
Authorization: Bearer bc7d02057b077379c5a3671b6092feeb6761f73d10768ce021f0e3d310f2aca8
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
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 16,
      "user_id": 419
    },
    {
      "id": 8,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 16,
      "user_id": 418
    },
    {
      "id": 7,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 16,
      "user_id": 417
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/16/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc7d02057b077379c5a3671b6092feeb6761f73d10768ce021f0e3d310f2aca8"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/71/republish
Content-Type: application/json
Authorization: Bearer d1fb7d90e6495472091dcfe452c251b87cb224f7734a7be8c5e9b52d283379c6
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
curl "api.goskive.com/v2/flashcards/71/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1fb7d90e6495472091dcfe452c251b87cb224f7734a7be8c5e9b52d283379c6"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/90/bookmark
Content-Type: application/json
Authorization: Bearer 62f532be7a366f2951e075ba97763c6c809f56ab8d50d2cb12edae9becb0fdda
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/90/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62f532be7a366f2951e075ba97763c6c809f56ab8d50d2cb12edae9becb0fdda"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/68
Content-Type: application/json
Authorization: Bearer 3094d193cfa9111a3fdb41d4a434cd1494039d3fa601b1918952ecc678e4c391
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/68" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3094d193cfa9111a3fdb41d4a434cd1494039d3fa601b1918952ecc678e4c391"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/91/downvote
Content-Type: application/json
Authorization: Bearer 6bc8b240eb29c92c9453c7ba05a1642d0e0469293c04dc9b38d5710f2e059734
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/91/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bc8b240eb29c92c9453c7ba05a1642d0e0469293c04dc9b38d5710f2e059734"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/74
Content-Type: application/json
Authorization: Bearer 5579874a9c1e955a348c4465d1fc8c2c95c3443f5f58dc44880807491ccd8fef
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
    "author_id": 863,
    "chapter_id": 169,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:58:01.748Z",
    "created_at": "2016-10-06T12:58:01.748Z",
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
	-H "Authorization: Bearer 5579874a9c1e955a348c4465d1fc8c2c95c3443f5f58dc44880807491ccd8fef"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/report
Content-Type: application/json
Authorization: Bearer 2e19613742efa9c163dc7b3bde1d808b704d04b17753507fc0bff434c7db39c5
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2e19613742efa9c163dc7b3bde1d808b704d04b17753507fc0bff434c7db39c5"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/72/bookmark
Content-Type: application/json
Authorization: Bearer 05034fa81a01e745890cc9b6d7e8c5832765c7ee30ebe8a605f410b602926500
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/72/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05034fa81a01e745890cc9b6d7e8c5832765c7ee30ebe8a605f410b602926500"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/73/upvote
Content-Type: application/json
Authorization: Bearer 36c95ea091cb9279e9a72efbcf67aaaa8b976f24294e1e34858fc069e0120987
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/73/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 36c95ea091cb9279e9a72efbcf67aaaa8b976f24294e1e34858fc069e0120987"
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
    "key": "cache/7a13a57aeefa9f1ab2cef4636c62d0f2.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0wNlQxMzo1NjozNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS83YTEzYTU3YWVlZmE5ZjFhYjJjZWY0NjM2YzYyZDBmMi5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAwNi9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMDZUMTI1NjM2WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161006/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161006T125636Z",
    "x-amz-signature": "fada7ebb6f1a0d4b3a548091358fb3a3d90e7769be528ede91bdac1c10465590"
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
Authorization: Bearer 627d6f73fe2d93002adcfd9d487e9a3c6dbc5226a11e018fb3c39ea03a479193
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
	-H "Authorization: Bearer 627d6f73fe2d93002adcfd9d487e9a3c6dbc5226a11e018fb3c39ea03a479193"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 766d3abafc73cad6764ac73afce505dc5692f69464ab3159784c621dea2f8951
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
	-H "Authorization: Bearer 766d3abafc73cad6764ac73afce505dc5692f69464ab3159784c621dea2f8951"
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
{"password":{"reset_password_token":"xy1XHHjV6mADT5bKgzgf","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 736,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-06T12:57:43.078Z",
  "updated_at": "2016-10-06T12:57:43.983Z",
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
  "audit_id": 5241
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"xy1XHHjV6mADT5bKgzgf","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
	-H "Content-Type: application/json"
```
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
{"password":{"reset_password_token":"AaU4YNyNq_UbDykNvXyY","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 1,
  "email": "jan.meier@hotmail.de",
  "created_at": "2016-10-06T12:57:44.848Z",
  "updated_at": "2016-10-06T12:57:45.016Z",
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
  "audit_id": 5244
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"AaU4YNyNq_UbDykNvXyY","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/126/comments
Content-Type: application/json
Authorization: Bearer 4eeddc5bf8d2b9f3bb4746478eaaab71dac11f3f8a30861349870006a77eeb9b
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
    "id": 60,
    "author_id": 936,
    "reply_to_id": null,
    "created_at": "2016-10-06T12:58:06.262Z",
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
curl "api.goskive.com/v2/questions/126/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eeddc5bf8d2b9f3bb4746478eaaab71dac11f3f8a30861349870006a77eeb9b"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/124/comments
Content-Type: application/json
Authorization: Bearer 403cfea7a982c972f45801c1c011bf827fe60f2e5ec7152d11d873e4bcb2ee3c
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
    "id": 59,
    "author_id": 930,
    "reply_to_id": null,
    "created_at": "2016-10-06T12:58:05.496Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 930,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:58:05.492Z",
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
curl "api.goskive.com/v2/questions/124/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 403cfea7a982c972f45801c1c011bf827fe60f2e5ec7152d11d873e4bcb2ee3c"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/123/comments
Content-Type: application/json
Authorization: Bearer dab2afe82e362fc266f52ecbe78823b7df58fc4ff3b9da2e5ffe14084228796d
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
      "id": 58,
      "author_id": 929,
      "reply_to_id": null,
      "created_at": "2016-10-06T12:58:05.147Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 928,
      "reply_to_id": null,
      "created_at": "2016-10-06T12:58:05.126Z",
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
curl "api.goskive.com/v2/questions/123/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dab2afe82e362fc266f52ecbe78823b7df58fc4ff3b9da2e5ffe14084228796d"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/125/comments
Content-Type: application/json
Authorization: Bearer 0341e6219c285607b7e71431dcf1a7c3b2c7a192cca348de91aac73d47e08702
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
curl "api.goskive.com/v2/questions/125/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0341e6219c285607b7e71431dcf1a7c3b2c7a192cca348de91aac73d47e08702"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/8/feedbacks
Content-Type: application/json
Authorization: Bearer 9d37ea09c43807d19f27371ba93e58c70f967f825ca28b106610abbdd8d3eb6d
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
    "id": 8,
    "user_id": 44,
    "feedbackable_id": 8,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-06T12:56:39.805Z",
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
curl "api.goskive.com/v2/questions/8/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d37ea09c43807d19f27371ba93e58c70f967f825ca28b106610abbdd8d3eb6d"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/3/feedbacks
Content-Type: application/json
Authorization: Bearer 16871a5d527f63bb78e497ca7ade284d0035e83d835088715725fed06e50cad1
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
      "user_id": 23,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:56:37.635Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 22,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-06T12:56:37.622Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/3/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16871a5d527f63bb78e497ca7ade284d0035e83d835088715725fed06e50cad1"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/108/votes
Content-Type: application/json
Authorization: Bearer 18348c4b926e7e3ccaf6144f3920b741b1ca45e446905f118a008d9af5147a8c
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
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 108,
      "user_id": 731
    },
    {
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 108,
      "user_id": 730
    },
    {
      "id": 18,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 108,
      "user_id": 729
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/108/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18348c4b926e7e3ccaf6144f3920b741b1ca45e446905f118a008d9af5147a8c"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/35/republish
Content-Type: application/json
Authorization: Bearer 3d4330e3cef84e1dba9e2b83dd609325ac12fe61d2a5dc4b6bdaeb36fd813617
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
curl "api.goskive.com/v2/questions/35/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d4330e3cef84e1dba9e2b83dd609325ac12fe61d2a5dc4b6bdaeb36fd813617"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/31/bookmark
Content-Type: application/json
Authorization: Bearer d956f815a4fade0ef456accb351f5015b850188871c1cb7f0ce7f3b65bd7a0af
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d956f815a4fade0ef456accb351f5015b850188871c1cb7f0ce7f3b65bd7a0af"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/33
Content-Type: application/json
Authorization: Bearer 156a8a4e16d47e417240fb4aefb0f767e2863023deed5071d2354b8373eb3ae8
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
	-H "Authorization: Bearer 156a8a4e16d47e417240fb4aefb0f767e2863023deed5071d2354b8373eb3ae8"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/34/downvote
Content-Type: application/json
Authorization: Bearer a7c40a91b2f9152931a9d4ac459d0edf645c6e668e1f551b403e664f2e06ec6b
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7c40a91b2f9152931a9d4ac459d0edf645c6e668e1f551b403e664f2e06ec6b"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/30
Content-Type: application/json
Authorization: Bearer 556614c916fe63286e0eb783475c795e7c7e4fa91473f2a67bd8a241f86d44b4
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
    "id": 30,
    "obfuscated_id": "virmgqGG22o",
    "author_id": 191,
    "chapter_id": 43,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:56:51.707Z",
    "created_at": "2016-10-06T12:56:51.591Z",
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
    "question": "Clever example question: why did the rspec test not pass?",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "This could never explain why it didn't pass. Maybe it did?",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 60,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 61,
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
curl "api.goskive.com/v2/questions/30" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 556614c916fe63286e0eb783475c795e7c7e4fa91473f2a67bd8a241f86d44b4"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/32/report
Content-Type: application/json
Authorization: Bearer 379564808e95f8b0efba55077ede7e247317ff85d45b2a8229bc8ec6b3efe53d
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/32/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 379564808e95f8b0efba55077ede7e247317ff85d45b2a8229bc8ec6b3efe53d"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/27/bookmark
Content-Type: application/json
Authorization: Bearer 472836afe6b7111e0761189dd8c755235adad7b0f84cfe88c5dd416bcd501c20
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 472836afe6b7111e0761189dd8c755235adad7b0f84cfe88c5dd416bcd501c20"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/29
Content-Type: application/json
Authorization: Bearer 5d70fe5ecf61bd6ea1fa205daeb0e2aef5b14aeb046498ef6b2ae14ee8a57f1b
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":29,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-06T12:56:51.087Z","updated_at":"2016-10-06T12:56:51.202Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":42,"author_id":188,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 29,
    "obfuscated_id": "rvs1sHrnKS4",
    "author_id": 188,
    "chapter_id": 42,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-06T12:56:51.311Z",
    "created_at": "2016-10-06T12:56:51.087Z",
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
    "question": "{\"id\"=>29, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-06T12:56:51.087Z\", \"updated_at\"=>\"2016-10-06T12:56:51.202Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>42, \"author_id\"=>188, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 59,
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
curl "api.goskive.com/v2/questions/29" -d '{"question":{"question":{"id":29,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-06T12:56:51.087Z","updated_at":"2016-10-06T12:56:51.202Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":42,"author_id":188,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d70fe5ecf61bd6ea1fa205daeb0e2aef5b14aeb046498ef6b2ae14ee8a57f1b"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/28/upvote
Content-Type: application/json
Authorization: Bearer 8ba4390bb7bee83f64fe78a4850d0d248af7ad8494d1fbbdd6018a07f3030e45
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/28/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ba4390bb7bee83f64fe78a4850d0d248af7ad8494d1fbbdd6018a07f3030e45"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 728c5ec91789f5355c612ec8f36335be3135097ddbe7242cadb0bc4bb9b8ab2c
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
      "creator_id": 337,
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 117,
      "additional_university_ids": [

      ],
      "topic_id": 120,
      "discipline_id": 121,
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
      "updated_at": "2016-10-06T12:57:01.394Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 728c5ec91789f5355c612ec8f36335be3135097ddbe7242cadb0bc4bb9b8ab2c"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer cdcb0baae81c8cf22a10803cb786817a05205afb8977c2ea06360330979fb845
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
      "id": 115,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-113",
      "html_url": "https://goskive.com/university/uni-113",
      "slug": "uni-113",
      "name": "National School of Pizza",
      "short_name": "Uni 113",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c81a8aee7b08da0c8fa2e528a434d06f079b9f35.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d9bc74d3abf8eee0a816b125076abff2b517b77b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-06T12:57:01.155Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 114,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-112",
      "html_url": "https://goskive.com/university/uni-112",
      "slug": "uni-112",
      "name": "National School of Pastry",
      "short_name": "Uni 112",
      "acronym": "NSPA",
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
      "updated_at": "2016-10-06T12:57:01.138Z",
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
	-H "Authorization: Bearer cdcb0baae81c8cf22a10803cb786817a05205afb8977c2ea06360330979fb845"
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
      "id": 63,
      "name": "Visionary disintermediate throughput",
      "name_translations": {
        "en": "Visionary disintermediate throughput"
      },
      "discipline_id": 64
    },
    {
      "id": 64,
      "name": "Virtual foreground architecture",
      "name_translations": {
        "en": "Virtual foreground architecture"
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
GET /v2/topics/65
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
    "id": 65,
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
curl "api.goskive.com/v2/topics/65" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 89c73a5277579a788730d4d513d237071ea7286da8886bea1dfdf490f82cbe09
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
      "id": 1,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-1",
      "html_url": "https://goskive.com/university/uni-1",
      "slug": "uni-1",
      "name": "University 1",
      "short_name": "Uni 1",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/38802f33528ba3ba141b3ec7e7bce0a2b851ee78.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51291693f690a69f7677e03637596dc7709b266f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-06T12:56:36.279Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "University 2",
      "short_name": "Uni 2",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/2a89a9c79d6373cf1f5ef1c3a160f560b4b8d6a3.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d16dc82a00061731dd68a80b60fdd432c556966d.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-06T12:56:36.294Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-3",
      "html_url": "https://goskive.com/university/uni-3",
      "slug": "uni-3",
      "name": "University 3",
      "short_name": "Uni 3",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0178e4c1b8a1e0379f3158851027049f94ddc463.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/51e7a1f572cf9347372a35d5e9ae2cc89f48eb30.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-06T12:56:36.309Z",
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
	-H "Authorization: Bearer 89c73a5277579a788730d4d513d237071ea7286da8886bea1dfdf490f82cbe09"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer fb7e3c893ced046eeeff25eff674bcac3c5fbf170b6423840005d78eb52fb51f
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
    "id": 4,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-06T12:56:36.444Z",
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
	-H "Authorization: Bearer fb7e3c893ced046eeeff25eff674bcac3c5fbf170b6423840005d78eb52fb51f"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 29d1f7deddad6400bc19365972398a736722e9331cd0e73e0e7007fee2dad9ea
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":185,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 465,
    "id": 175,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 159,
    "additional_university_ids": [

    ],
    "topic_id": 185,
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
    "chapters_updated_at": "2016-10-06T12:57:11.351Z",
    "updated_at": "2016-10-06T12:57:11.498Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 64,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-06T12:57:11.452Z",
        "course_id": 175,
        "author_id": 465,
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
        "id": 65,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-06T12:57:11.470Z",
        "course_id": 175,
        "author_id": 465,
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
        "id": 66,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-06T12:57:11.488Z",
        "course_id": 175,
        "author_id": 465,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":185,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 29d1f7deddad6400bc19365972398a736722e9331cd0e73e0e7007fee2dad9ea"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 07f3d5a3366072bcf59dfb441b16e1f616f14d522aabc38bef4177bdaa11211a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":184,"published":false}}
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
    "creator_id": 464,
    "id": 174,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 158,
    "additional_university_ids": [

    ],
    "topic_id": 184,
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
    "updated_at": "2016-10-06T12:57:11.307Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":184,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 07f3d5a3366072bcf59dfb441b16e1f616f14d522aabc38bef4177bdaa11211a"
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
      "creator_id": 437,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 148,
      "additional_university_ids": [

      ],
      "topic_id": 161,
      "discipline_id": 162,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
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
      "updated_at": "2016-10-06T12:57:08.716Z",
      "shortname": "fu-course-137"
    },
    {
      "creator_id": 437,
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 148,
      "additional_university_ids": [

      ],
      "topic_id": 162,
      "discipline_id": 163,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
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
      "chapters_updated_at": "2016-10-06T12:57:09.008Z",
      "updated_at": "2016-10-06T12:57:09.014Z",
      "shortname": "fu-course-138"
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
Authorization: Bearer ead6a131b80cb402184287384f8ea39d97f571b251ff29a0e8a28f8ca0576da1
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
      "creator_id": 454,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-153",
      "html_url": "https://goskive.com/course/fu-course-153",
      "slug": "fu-course-153",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 178,
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
      "updated_at": "2016-10-06T12:57:10.365Z",
      "shortname": "fu-course-153"
    },
    {
      "creator_id": 454,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-154",
      "html_url": "https://goskive.com/course/fu-course-154",
      "slug": "fu-course-154",
      "university_id": 154,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 154",
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
      "chapters_updated_at": "2016-10-06T12:57:10.668Z",
      "updated_at": "2016-10-06T12:57:10.675Z",
      "shortname": "fu-course-154"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ead6a131b80cb402184287384f8ea39d97f571b251ff29a0e8a28f8ca0576da1"
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
      "creator_id": 442,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 165,
      "discipline_id": 166,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
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
      "updated_at": "2016-10-06T12:57:09.231Z",
      "shortname": "fu-course-141"
    },
    {
      "creator_id": 442,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 150,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 167,
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
      "updated_at": "2016-10-06T12:57:09.271Z",
      "shortname": "fu-course-142"
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
Authorization: Bearer 69c097c185a0a71eec0934c0d56b0328250ec07a0cb1a53c1dea06f8aa7ef8f7
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
      "creator_id": 461,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-157",
      "html_url": "https://goskive.com/course/fu-course-157",
      "slug": "fu-course-157",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 157",
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
      "updated_at": "2016-10-06T12:57:10.975Z",
      "shortname": "fu-course-157"
    },
    {
      "creator_id": 461,
      "id": 172,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-158",
      "html_url": "https://goskive.com/course/fu-course-158",
      "slug": "fu-course-158",
      "university_id": 156,
      "additional_university_ids": [

      ],
      "topic_id": 182,
      "discipline_id": 183,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 158",
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
      "updated_at": "2016-10-06T12:57:11.019Z",
      "shortname": "fu-course-158"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69c097c185a0a71eec0934c0d56b0328250ec07a0cb1a53c1dea06f8aa7ef8f7"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer be1b86a72aa1e512736c9afb049be4644b68d92feb5cc968204d38666fed25fa
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
  "id": 420,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-06T12:57:06.989Z",
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
	-H "Authorization: Bearer be1b86a72aa1e512736c9afb049be4644b68d92feb5cc968204d38666fed25fa"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/768
Content-Type: application/json
Authorization: Bearer 9bd3119ff7691c6daeabd71f513bd5922c46a9a7730e4386e7605a7c9c45c14b
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
    "id": 768,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 239,
    "fields_of_study": [
      265,
      266
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-06T12:57:48.100Z",
    "updated_at": "2016-10-06T12:57:48.100Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/768" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bd3119ff7691c6daeabd71f513bd5922c46a9a7730e4386e7605a7c9c45c14b"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/770
Content-Type: application/json
Authorization: Bearer 1a2f5b0e9bdbc71a845049558c8892641e539fac045b7484ea8c7eb0b8628320
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
    "id": 770,
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
    "created_at": "2016-10-06T12:57:48.187Z",
    "updated_at": "2016-10-06T12:57:48.187Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/770" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a2f5b0e9bdbc71a845049558c8892641e539fac045b7484ea8c7eb0b8628320"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/12
Content-Type: application/json
Authorization: Bearer 24970e828e299358169b05a5efcf6841c8e73479add4b709291d33d782f7774d
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24970e828e299358169b05a5efcf6841c8e73479add4b709291d33d782f7774d"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/10
Content-Type: application/json
Authorization: Bearer 8721d2b4acd0ce0db3c34eef99645f304ca7a004b35f0c77b744806679948b1c
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
    "id": 10,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 74,
    "user_id": 529
  }
}
```



```shell
curl "api.goskive.com/v2/votes/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8721d2b4acd0ce0db3c34eef99645f304ca7a004b35f0c77b744806679948b1c"
```
