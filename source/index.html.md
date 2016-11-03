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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"4c2b55636361f2a3933c710e68dda6f90e9d6787f5b931893c8e115a63a95ee3","client_secret":"2c518ce6878600b3ebb549c6e625a16d13df0049a7794449e9d0384c7dc91c26"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"4c2b55636361f2a3933c710e68dda6f90e9d6787f5b931893c8e115a63a95ee3","client_secret":"2c518ce6878600b3ebb549c6e625a16d13df0049a7794449e9d0384c7dc91c26"}' -X POST \
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
Authorization: Basic ODY4ZmQ2ZGY4Y2EyZmU0MmFhNzZhZjZmOTA5NTdkZmJkMjZhMmUxMzUxNDUy
MGIzYzAyN2UxZjE4OTY3ODkzMDpjMzc0YzEyNGJlYjgwOTE5MjdhNDE1YzA1
NmE5NzhlNGQ1YzgyYmY2NDE1ZjhmODM2ZDUwMTNkNGViZmQzZDNh

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
	-u 868fd6df8ca2fe42aa76af6f90957dfbd26a2e13514520b3c027e1f189678930:c374c124beb8091927a415c056a978e4d5c82bf6415f8f836d5013d4ebfd3d3a
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
{"grant_type":"client_credentials","client_id":"c9177e923f356062fb60a98cc6356ca3c7ea601306f4fffaa7cf38d603b32245","client_secret":"ba84e5f18600df3411dc62eaa31ca2fdbc9d424ea8282fb9a2b36e9340a074ce"}
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
  "access_token": "5f6562f24c45591899d2eeaa3f367044609127b73968fc32d0728b84c9f4ef1b",
  "token_type": "bearer",
  "created_at": 1478176474
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"c9177e923f356062fb60a98cc6356ca3c7ea601306f4fffaa7cf38d603b32245","client_secret":"ba84e5f18600df3411dc62eaa31ca2fdbc9d424ea8282fb9a2b36e9340a074ce"}' -X POST \
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2e942ca1ad390e1d3a6102cc5d8ede5a1e884a94c307330f7b48bca9f1e6fae9","client_secret":"271449797f7f8ffda85c838b802c1cd90065afda7c5cd27a354ab5151c255d2e"}
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
  "access_token": "3f12f56ca29bf2626ed0fee7a756c28da769f94b39b809043341f42350a37250",
  "token_type": "bearer",
  "created_at": 1478176474
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"2e942ca1ad390e1d3a6102cc5d8ede5a1e884a94c307330f7b48bca9f1e6fae9","client_secret":"271449797f7f8ffda85c838b802c1cd90065afda7c5cd27a354ab5151c255d2e"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZDgzMzFkMjRmOGNiZmM0NzdjMmVlM2Y2MGUzMjIxMDVhZTM2YmE2Nzg4NjEz
OGQ4ODQ5NGU3ODA3NzAyNjIxMDoyNjlhZDcwMzBlZjZkZjNjNTNhOTdkZjE3
Njc4NTZhN2Y3MzU1NzdhNGQ0OThhNzg0NDA2NDQ3OGZmYTgwNmJj

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
  "access_token": "1cb766fc2fc3d8f91305c6e04ad68c89c9f5ffc65ec6fbec3f0849bd94580e08",
  "token_type": "bearer",
  "created_at": 1478176474
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u d8331d24f8cbfc477c2ee3f60e322105ae36ba67886138d88494e78077026210:269ad7030ef6df3c53a97df1767856a7f735577a4d498a7844064478ffa806bc
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
Authorization: Bearer 160ba5748bee68c6954374ef2313b3c6a49086b45435acd4bd9306f81f501f6c
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
	-H "Authorization: Bearer 160ba5748bee68c6954374ef2313b3c6a49086b45435acd4bd9306f81f501f6c"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/154/flashcards
Content-Type: application/json
Authorization: Bearer 32e3ca6c9761b122488c8ac6708d4d4305343a3149f8801e461300dc3aa13c65
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":154,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 80,
    "obfuscated_id": "94gVa2GR5x8",
    "author_id": 746,
    "chapter_id": 154,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:34:22.427Z",
    "created_at": "2016-11-03T12:34:22.427Z",
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
curl "api.goskive.com/v2/chapters/154/flashcards" -d '{"flashcard":{"chapter_id":154,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32e3ca6c9761b122488c8ac6708d4d4305343a3149f8801e461300dc3aa13c65"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/153/flashcards
Content-Type: application/json
Authorization: Bearer faec8e152d9abaa4293a941dddc6b444acfb7a55b6a207fb14672c585b62e2a0
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 741,
      "chapter_id": 153,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:22.152Z",
      "created_at": "2016-11-03T12:34:22.152Z",
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 741,
      "chapter_id": 153,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:22.188Z",
      "created_at": "2016-11-03T12:34:22.188Z",
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
      "id": 79,
      "obfuscated_id": "BFjsqYG0c2I",
      "author_id": 741,
      "chapter_id": 153,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:22.223Z",
      "created_at": "2016-11-03T12:34:22.223Z",
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
curl "api.goskive.com/v2/chapters/153/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faec8e152d9abaa4293a941dddc6b444acfb7a55b6a207fb14672c585b62e2a0"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/174/questions
Content-Type: application/json
Authorization: Bearer a35302fec3c6f5791d260c3c2413fb0e2495aaa60cfaae860c686d08c15215c9
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":174,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 115,
    "obfuscated_id": "tgK0VZO8yq4",
    "author_id": 882,
    "chapter_id": 174,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:34:34.087Z",
    "created_at": "2016-11-03T12:34:34.087Z",
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
        "id": 231,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 232,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 233,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 234,
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
curl "api.goskive.com/v2/chapters/174/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":174,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a35302fec3c6f5791d260c3c2413fb0e2495aaa60cfaae860c686d08c15215c9"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/172/questions
Content-Type: application/json
Authorization: Bearer a9f287eb0a097bdce3c48d869544fca1ce8c50c360187914a96a5eba5d15ad33
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 113,
    "obfuscated_id": "pcyz_ZHBlMU",
    "author_id": 876,
    "chapter_id": 172,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:34:33.407Z",
    "created_at": "2016-11-03T12:34:33.407Z",
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
        "id": 227,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 228,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/172/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":172,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a9f287eb0a097bdce3c48d869544fca1ce8c50c360187914a96a5eba5d15ad33"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/173/questions
Content-Type: application/json
Authorization: Bearer 9887a8b5d580534807abfa16942f07e84ee8e85f16bf43a4e00c483d5cff7c2c
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":173,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 114,
    "obfuscated_id": "RwCVsRO9fcs",
    "author_id": 879,
    "chapter_id": 173,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:34:33.730Z",
    "created_at": "2016-11-03T12:34:33.730Z",
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
        "id": 229,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 230,
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
curl "api.goskive.com/v2/chapters/173/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":173,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9887a8b5d580534807abfa16942f07e84ee8e85f16bf43a4e00c483d5cff7c2c"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/171/questions
Content-Type: application/json
Authorization: Bearer f66381bb56d4ab5a906ee23f69e9ceacbedba4a7df581f2223d5b1549cacb1ee
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":171,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 873,
    "chapter_id": 171,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:34:33.007Z",
    "created_at": "2016-11-03T12:34:33.007Z",
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
        "id": 224,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 225,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 226,
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
curl "api.goskive.com/v2/chapters/171/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":171,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f66381bb56d4ab5a906ee23f69e9ceacbedba4a7df581f2223d5b1549cacb1ee"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/169/questions
Content-Type: application/json
Authorization: Bearer 0d5a51fdfe118f013e016072961e8b31bcd77fa5a82c6084fe0d0d7e4e154c98
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
      "id": 109,
      "obfuscated_id": "VSPyck5c2RY",
      "author_id": 864,
      "chapter_id": 169,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:32.225Z",
      "created_at": "2016-11-03T12:34:32.102Z",
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
    },
    {
      "id": 110,
      "obfuscated_id": "55JK4PuG2Hk",
      "author_id": 865,
      "chapter_id": 169,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:32.419Z",
      "created_at": "2016-11-03T12:34:32.301Z",
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
          "id": 220,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 221,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 111,
      "obfuscated_id": "G-D-sgMUtTw",
      "author_id": 866,
      "chapter_id": 169,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:34:32.626Z",
      "created_at": "2016-11-03T12:34:32.498Z",
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
          "id": 222,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 223,
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
curl "api.goskive.com/v2/chapters/169/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d5a51fdfe118f013e016072961e8b31bcd77fa5a82c6084fe0d0d7e4e154c98"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/193
Content-Type: application/json
Authorization: Bearer 85a53cbf198a217e02860d4dcfd82fafb4bfa314ea027a59ed5eb2a699311d27
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
curl "api.goskive.com/v2/chapters/193" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85a53cbf198a217e02860d4dcfd82fafb4bfa314ea027a59ed5eb2a699311d27"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/195
Content-Type: application/json
Authorization: Bearer 851f42c9f17669e231282ccf6556fbdbaa50425726e794251732022f8db2dd82
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
curl "api.goskive.com/v2/chapters/195" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 851f42c9f17669e231282ccf6556fbdbaa50425726e794251732022f8db2dd82"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/187
Content-Type: application/json
Authorization: Bearer 306bacd80779cfa98ddec09e36de76d72f712efbd0108d67512d76532de81ce8
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
curl "api.goskive.com/v2/chapters/187" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 306bacd80779cfa98ddec09e36de76d72f712efbd0108d67512d76532de81ce8"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/194
Content-Type: application/json
Authorization: Bearer 7b2f0ced76ae44b1ba69053467d2f3d1845d9459f5763da31128ac99b404bdbc
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/194" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b2f0ced76ae44b1ba69053467d2f3d1845d9459f5763da31128ac99b404bdbc"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 17f9d094f536f5c9f9b4445580c3b068b78ea94cf04c6d9ff04ca869cdfa8a1b
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
    "id": 191,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T12:34:41.604Z",
    "course_id": 312,
    "author_id": 965,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-11-03T12:34:41.096Z",
    "questions_updated_at": "2016-11-03T12:34:41.096Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 969,
        "chapter_id": 191,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:41.588Z",
        "created_at": "2016-11-03T12:34:41.588Z",
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
        "id": 132,
        "obfuscated_id": "RECRPLqMrqE",
        "author_id": 967,
        "chapter_id": 191,
        "position": 119,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:41.486Z",
        "created_at": "2016-11-03T12:34:41.370Z",
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
            "id": 267,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 268,
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
curl "api.goskive.com/v2/chapters/191" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17f9d094f536f5c9f9b4445580c3b068b78ea94cf04c6d9ff04ca869cdfa8a1b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 16273872793101475146a710b2263d07a6e966d04ffdd60c0a78864813b24e5a
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
    "id": 189,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T12:34:40.440Z",
    "course_id": 310,
    "author_id": 956,
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
curl "api.goskive.com/v2/chapters/189" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16273872793101475146a710b2263d07a6e966d04ffdd60c0a78864813b24e5a"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/51/replies
Content-Type: application/json
Authorization: Bearer 6602e04bd6dd15499b64c4b23757344eb3396e8b7041f324586ee4c457ad1ffc
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
    "id": 52,
    "author_id": 678,
    "reply_to_id": 51,
    "created_at": "2016-11-03T12:34:18.608Z",
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
curl "api.goskive.com/v2/comments/51/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6602e04bd6dd15499b64c4b23757344eb3396e8b7041f324586ee4c457ad1ffc"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/53/replies
Content-Type: application/json
Authorization: Bearer beee36b19bcd22e4cf7106da43459d7cf1bf1e0b03dcb8453fa8404605e1dd08
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
curl "api.goskive.com/v2/comments/53/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer beee36b19bcd22e4cf7106da43459d7cf1bf1e0b03dcb8453fa8404605e1dd08"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/5
Content-Type: application/json
Authorization: Bearer 7c58e24a513a5c10142c16b9acd66ddf91b3faa1a35860daed2a1a4e68ab7927
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
curl "api.goskive.com/v2/comments/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c58e24a513a5c10142c16b9acd66ddf91b3faa1a35860daed2a1a4e68ab7927"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/2/republish
Content-Type: application/json
Authorization: Bearer 9e24aef4f014cf7b7951cb3e2b31a17b9efbdf739c73f12618bd135b701f0d79
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
curl "api.goskive.com/v2/comments/2/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e24aef4f014cf7b7951cb3e2b31a17b9efbdf739c73f12618bd135b701f0d79"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/4
Content-Type: application/json
Authorization: Bearer cae64748c278da560c02f5985cbddc6ccb3682f4bb7fee9328af2825094060ac
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cae64748c278da560c02f5985cbddc6ccb3682f4bb7fee9328af2825094060ac"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/42/report
Content-Type: application/json
Authorization: Bearer 09187bde32ff50ba864d689702da243b766979a56ed280b47b2fd99f328976f4
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/42/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09187bde32ff50ba864d689702da243b766979a56ed280b47b2fd99f328976f4"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/19
Content-Type: application/json
Authorization: Bearer 01d090cd1405835741b428953a3261107a35cc28f3a18dcd21adac5ac87e5350
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
    "id": 19,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a1ce8822aa73a6dc18ff1d7e16ae0bc62030798e.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-11-03T12:34:27.799Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 01d090cd1405835741b428953a3261107a35cc28f3a18dcd21adac5ac87e5350"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 1e6dab73674a8bc27165b5c88d69d2a59f849055ab75b0009b1131a3c54e62b9
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
      "id": 16,
      "name": "Fake Company Name 12",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T12:34:27.679Z"
    },
    {
      "id": 17,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e484c00890bdf1ca97cde19c89def85eb31f8933.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T12:34:27.683Z"
    },
    {
      "id": 18,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/76c0058f46bff75ade3993139c75182acdd0c364.png",
      "brand_color": "#000000",
      "updated_at": "2016-11-03T12:34:27.686Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e6dab73674a8bc27165b5c88d69d2a59f849055ab75b0009b1131a3c54e62b9"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/15/company_profiles
Content-Type: application/json
Authorization: Bearer 18e761c75201bbe01e2fb179262e763136efeff96eb0a5301183fb84ab62b9f2
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
curl "api.goskive.com/v2/companies/15/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18e761c75201bbe01e2fb179262e763136efeff96eb0a5301183fb84ab62b9f2"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/13/company_profiles
Content-Type: application/json
Authorization: Bearer 70f8da584407c0a7fe6450ff99064698a61b216b6f6419da84afc159504b01f4
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
curl "api.goskive.com/v2/companies/13/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70f8da584407c0a7fe6450ff99064698a61b216b6f6419da84afc159504b01f4"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer a5f18f167e0eb1eee5f2da2a75683e0e59c3a8f06826db376494940cc30a1617
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
      "id": 6,
      "title": "Campaign 5",
      "company_id": 26,
      "precluded_campaign_ids": [

      ],
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
      "id": 9,
      "title": "Campaign 8",
      "company_id": 29,
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/campaigns" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5f18f167e0eb1eee5f2da2a75683e0e59c3a8f06826db376494940cc30a1617"
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
Authorization: Bearer ccf22aadb7f7d336e1996093df3b0605eba7d23167a3d28b98bbd206a7d3f121
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
	-H "Authorization: Bearer ccf22aadb7f7d336e1996093df3b0605eba7d23167a3d28b98bbd206a7d3f121"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 313633d9ebb1ade41226da6237fede5c66b3bcefc3f24bf0f705d976c59edc62
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
    "id": 151,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T12:34:21.884Z",
    "course_id": 219,
    "author_id": 737,
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
	-H "Authorization: Bearer 313633d9ebb1ade41226da6237fede5c66b3bcefc3f24bf0f705d976c59edc62"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6b71e281e23821a8c5ad4692568106efa135f6cb2e30ceb500b8008bb90c99cf
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
      "title": "Clever Chapter Title 128",
      "position": 1,
      "updated_at": "2016-11-03T12:34:19.152Z",
      "course_id": 205,
      "author_id": 685,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 129,
      "title": "Clever Chapter Title 129",
      "position": 2,
      "updated_at": "2016-11-03T12:34:19.176Z",
      "course_id": 205,
      "author_id": 686,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 130,
      "title": "Clever Chapter Title 130",
      "position": 3,
      "updated_at": "2016-11-03T12:34:19.421Z",
      "course_id": 205,
      "author_id": 687,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T12:34:19.078Z",
      "questions_updated_at": "2016-11-03T12:34:19.078Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b71e281e23821a8c5ad4692568106efa135f6cb2e30ceb500b8008bb90c99cf"
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
      "id": 134,
      "title": "Clever Chapter Title 134",
      "position": 1,
      "updated_at": "2016-11-03T12:34:19.880Z",
      "course_id": 208,
      "author_id": 699,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 135,
      "title": "Clever Chapter Title 135",
      "position": 2,
      "updated_at": "2016-11-03T12:34:19.905Z",
      "course_id": 208,
      "author_id": 700,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 136,
      "title": "Clever Chapter Title 136",
      "position": 3,
      "updated_at": "2016-11-03T12:34:20.148Z",
      "course_id": 208,
      "author_id": 701,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-11-03T12:34:19.810Z",
      "questions_updated_at": "2016-11-03T12:34:19.810Z",
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
Authorization: Bearer 265afa5d56fe1d460eea119aa0250d21035c459a7eacfcc2ed2c613237bb1deb
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
      "title": "Clever Chapter Title 131",
      "position": 1,
      "updated_at": "2016-11-03T12:34:19.596Z",
      "course_id": 206,
      "author_id": 692,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 132,
      "title": "Clever Chapter Title 132",
      "position": 2,
      "updated_at": "2016-11-03T12:34:19.619Z",
      "course_id": 206,
      "author_id": 693,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 133,
      "title": "Clever Chapter Title 133",
      "position": 3,
      "updated_at": "2016-11-03T12:34:19.642Z",
      "course_id": 206,
      "author_id": 694,
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
	-H "Authorization: Bearer 265afa5d56fe1d460eea119aa0250d21035c459a7eacfcc2ed2c613237bb1deb"
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
      "id": 137,
      "title": "Clever Chapter Title 137",
      "position": 1,
      "updated_at": "2016-11-03T12:34:20.337Z",
      "course_id": 210,
      "author_id": 706,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 138,
      "title": "Clever Chapter Title 138",
      "position": 2,
      "updated_at": "2016-11-03T12:34:20.360Z",
      "course_id": 210,
      "author_id": 707,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 139,
      "title": "Clever Chapter Title 139",
      "position": 3,
      "updated_at": "2016-11-03T12:34:20.384Z",
      "course_id": 210,
      "author_id": 708,
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
Authorization: Bearer 3fb4d7b2ca890b2db38bc11c853a95629772c861ff951de098acac50a7da7903
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
    "course_id": 6,
    "user_id": 16,
    "updated_at": "2016-11-03T12:33:27.807Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fb4d7b2ca890b2db38bc11c853a95629772c861ff951de098acac50a7da7903"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 31d42d264484e2227eef592a7136bdec31a125913e89150a7e97906d19c51993
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
      "course_id": 1,
      "user_id": 2,
      "updated_at": "2016-11-03T12:33:26.942Z"
    },
    {
      "id": 2,
      "course_id": 1,
      "user_id": 3,
      "updated_at": "2016-11-03T12:33:26.959Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31d42d264484e2227eef592a7136bdec31a125913e89150a7e97906d19c51993"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/280/files
Content-Type: application/json
Authorization: Bearer 277da5a643a101c7bc7415edec0ef2486b99d9c17b5580f9c0447e0ee3f91a13
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
      "id": 17,
      "uploader": {
        "id": 849,
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
        "created_at": "2016-11-03T12:34:31.181Z",
        "updated_at": "2016-11-03T12:34:31.181Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T12:34:31.192Z",
      "updated_at": "2016-11-03T12:34:31.192Z",
      "course_id": 280,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 18,
      "uploader": {
        "id": 850,
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
        "created_at": "2016-11-03T12:34:31.199Z",
        "updated_at": "2016-11-03T12:34:31.199Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T12:34:31.209Z",
      "updated_at": "2016-11-03T12:34:31.209Z",
      "course_id": 280,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 19,
      "uploader": {
        "id": 851,
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
        "created_at": "2016-11-03T12:34:31.216Z",
        "updated_at": "2016-11-03T12:34:31.216Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-11-03T12:34:31.226Z",
      "updated_at": "2016-11-03T12:34:31.226Z",
      "course_id": 280,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/280/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 277da5a643a101c7bc7415edec0ef2486b99d9c17b5580f9c0447e0ee3f91a13"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/283/files
Content-Type: application/json
Authorization: Bearer faaf0bc7a75fa209b21928d92b047afe411e3997de2b82f6f0e57a0b91e5f0f1
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
    "id": 20,
    "uploader": {
      "id": 858,
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
      "created_at": "2016-11-03T12:34:31.545Z",
      "updated_at": "2016-11-03T12:34:31.545Z"
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
    "created_at": "2016-11-03T12:34:31.575Z",
    "updated_at": "2016-11-03T12:34:31.575Z",
    "course_id": 283,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/283/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faaf0bc7a75fa209b21928d92b047afe411e3997de2b82f6f0e57a0b91e5f0f1"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/282/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer a3a8ba13241785685157c3db97a215f8f5ae25efc1b773648a3baafdccfaaef3
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
    "key": "cache/51d2e8c395f5eb02013f8cdd9eff4296.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxMzozNDozMVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzUxZDJlOGMzOTVmNWViMDIwMTNmOGNkZDllZmY0Mjk2LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjExMDMvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMTAzVDEyMzQzMVoifV19",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T123431Z",
    "x-amz-signature": "a6e262e38a62e45ced0f5c6c279cd582c25eae8a90aec5cb805ed8201be4d4da"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/282/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3a8ba13241785685157c3db97a215f8f5ae25efc1b773648a3baafdccfaaef3"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer e4e1e40cfca9a8cfce075b51f299d3b11a4bcf61d0e0bf8e2182472611ea5ca4
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
	-H "Authorization: Bearer e4e1e40cfca9a8cfce075b51f299d3b11a4bcf61d0e0bf8e2182472611ea5ca4"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9bc75cb80f70d7fc82cb7a4551f69c5d0fa0bd1b30650325befcadf393296d0d
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
	-H "Authorization: Bearer 9bc75cb80f70d7fc82cb7a4551f69c5d0fa0bd1b30650325befcadf393296d0d"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 899770dbfbf492aebab6cdc1b4e90cbd8516589008de7e914295f0a421e45ab1
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
	-H "Authorization: Bearer 899770dbfbf492aebab6cdc1b4e90cbd8516589008de7e914295f0a421e45ab1"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 431b28562dd83379c71803c24747621ccaa49a613696a3c8379043e48dc7afa8
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
	-H "Authorization: Bearer 431b28562dd83379c71803c24747621ccaa49a613696a3c8379043e48dc7afa8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c85dddfca504282eafb9d845278cbfe0b8791d51bb645b51999f98014277ec88
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
	-H "Authorization: Bearer c85dddfca504282eafb9d845278cbfe0b8791d51bb645b51999f98014277ec88"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 24d6582efe06e900d5f1a814cda73e0b20f702d7cd5ee894ef426410db91eca0
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
    "creator_id": 619,
    "id": 191,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 197,
    "additional_university_ids": [

    ],
    "topic_id": 193,
    "discipline_id": 193,
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
    "chapters_updated_at": "2016-11-03T12:34:11.955Z",
    "updated_at": "2016-11-03T12:34:13.373Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 112,
        "title": "Clever Chapter Title 112",
        "position": 1,
        "updated_at": "2016-11-03T12:34:13.328Z",
        "course_id": 191,
        "author_id": 619,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T12:34:11.955Z",
        "questions_updated_at": "2016-11-03T12:34:11.955Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 113,
        "title": "Clever Chapter Title 113",
        "position": 2,
        "updated_at": "2016-11-03T12:34:13.366Z",
        "course_id": 191,
        "author_id": 619,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T12:34:11.955Z",
        "questions_updated_at": "2016-11-03T12:34:11.955Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 620,
        "chapter_id": 112,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:13.168Z",
        "created_at": "2016-11-03T12:34:13.168Z",
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
        "author_id": 620,
        "chapter_id": 113,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:13.240Z",
        "created_at": "2016-11-03T12:34:13.240Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 620,
        "chapter_id": 112,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:13.209Z",
        "created_at": "2016-11-03T12:34:13.209Z",
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
        "id": 51,
        "obfuscated_id": "fXx2Zpse_KI",
        "author_id": 620,
        "chapter_id": 113,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:13.279Z",
        "created_at": "2016-11-03T12:34:13.279Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 620,
        "chapter_id": 112,
        "position": 66,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:12.171Z",
        "created_at": "2016-11-03T12:34:12.057Z",
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
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 620,
        "chapter_id": 112,
        "position": 67,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:12.341Z",
        "created_at": "2016-11-03T12:34:12.233Z",
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
      },
      {
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 620,
        "chapter_id": 113,
        "position": 68,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:12.541Z",
        "created_at": "2016-11-03T12:34:12.420Z",
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
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 620,
        "chapter_id": 113,
        "position": 69,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:12.719Z",
        "created_at": "2016-11-03T12:34:12.607Z",
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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24d6582efe06e900d5f1a814cda73e0b20f702d7cd5ee894ef426410db91eca0"
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
    "creator_id": 625,
    "id": 192,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 198,
    "additional_university_ids": [

    ],
    "topic_id": 194,
    "discipline_id": 194,
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
    "chapters_updated_at": "2016-11-03T12:34:13.496Z",
    "updated_at": "2016-11-03T12:34:14.919Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 114,
        "title": "Clever Chapter Title 114",
        "position": 1,
        "updated_at": "2016-11-03T12:34:14.873Z",
        "course_id": 192,
        "author_id": 625,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T12:34:13.496Z",
        "questions_updated_at": "2016-11-03T12:34:13.496Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 115,
        "title": "Clever Chapter Title 115",
        "position": 2,
        "updated_at": "2016-11-03T12:34:14.912Z",
        "course_id": 192,
        "author_id": 625,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-11-03T12:34:13.496Z",
        "questions_updated_at": "2016-11-03T12:34:13.496Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 625,
        "chapter_id": 114,
        "position": 72,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:13.724Z",
        "created_at": "2016-11-03T12:34:13.609Z",
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
      },
      {
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 625,
        "chapter_id": 115,
        "position": 74,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:14.096Z",
        "created_at": "2016-11-03T12:34:13.976Z",
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
PUT /v2/courses/194/pin
Content-Type: application/json
Authorization: Bearer e3ca7e5edbb39cf0b93c88e69a6bd61697585a904d6b32fd11b3fe15122593f1
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/194/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3ca7e5edbb39cf0b93c88e69a6bd61697585a904d6b32fd11b3fe15122593f1"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/189/pin
Content-Type: application/json
Authorization: Bearer 45bae8918370b6b02459f4561260d3b95815e5ca2bd81fbbc18cebe3cda4e8ca
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/189/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45bae8918370b6b02459f4561260d3b95815e5ca2bd81fbbc18cebe3cda4e8ca"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cfabd7e50acb4fbab43c3576a4d84fb3753a2de9e18e0255de2b1e7129bcf872
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
    "creator_id": 608,
    "id": 187,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 193,
    "additional_university_ids": [

    ],
    "topic_id": 189,
    "discipline_id": 189,
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
    "updated_at": "2016-11-03T12:34:10.196Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfabd7e50acb4fbab43c3576a4d84fb3753a2de9e18e0255de2b1e7129bcf872"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer a388d53445f51a79cb02fab7bf4b6e40b4bf156cd45d76f4e8af43d42c9228f3
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
    "id": 988,
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
    "created_at": "2016-11-03T12:34:43.245Z",
    "updated_at": "2016-11-03T12:34:43.245Z",
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
	-H "Authorization: Bearer a388d53445f51a79cb02fab7bf4b6e40b4bf156cd45d76f4e8af43d42c9228f3"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 0221b29147a86af673260f71b7ffd9af1352b3f91b37596b22f14edba0822598
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[325]}
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
    "id": 984,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      325
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T12:34:42.994Z",
    "updated_at": "2016-11-03T12:34:43.028Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[325]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0221b29147a86af673260f71b7ffd9af1352b3f91b37596b22f14edba0822598"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer f3022f9bba6ee9fead2f37f2ed493eb984be2d43c2a574c2daf36d769a46f74b
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
    "id": 987,
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
    "created_at": "2016-11-03T12:34:43.179Z",
    "updated_at": "2016-11-03T12:34:43.179Z",
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
	-H "Authorization: Bearer f3022f9bba6ee9fead2f37f2ed493eb984be2d43c2a574c2daf36d769a46f74b"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b30c0d754ac888be5c67bfccc85942bc4bf35cb90caa7083ffb0e5dc145dc6be
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[326]}
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
    "id": 985,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      326
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T12:34:43.066Z",
    "updated_at": "2016-11-03T12:34:43.066Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[326]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b30c0d754ac888be5c67bfccc85942bc4bf35cb90caa7083ffb0e5dc145dc6be"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer cc9b4974e424f2c619544623f96fee4da8dc9e49a5cb8a03441caa5840a979a3
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

324
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
    "id": 983,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/974108bc990e9762a002cc9af91dc6fea132a906.jpg",
    "university_id": null,
    "fields_of_study": [
      324
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-11-03T12:34:42.630Z",
    "updated_at": "2016-11-03T12:34:42.936Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/36872856caf9023d8d9f84ef5d9517a6dbc0637a.jpg",
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

324
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer cc9b4974e424f2c619544623f96fee4da8dc9e49a5cb8a03441caa5840a979a3"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 1cbb6296465d07bdd589d76cb260e0d97a43efa0e14e1dd00f892c73597f7e10
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
      "id": 3,
      "bookmarkable_id": 55,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 56,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 57,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cbb6296465d07bdd589d76cb260e0d97a43efa0e14e1dd00f892c73597f7e10"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer e3e543b710f0a134922634d7041f78469df9e32c7b480851afb697f7cc906566
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
	-H "Authorization: Bearer e3e543b710f0a134922634d7041f78469df9e32c7b480851afb697f7cc906566"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer c38e3c5e2bd450787c0b5c53fe936047f71454f68bc9dd62ddc0505b20f8ecd0
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
	-H "Authorization: Bearer c38e3c5e2bd450787c0b5c53fe936047f71454f68bc9dd62ddc0505b20f8ecd0"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer c2826cc3d8e08bd2761144948b62264a682e8aa4a766097d9988b2a5a51835ef
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
      "id": 223,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-184",
      "html_url": "https://goskive.com/course/mit-course-184",
      "slug": "mit-course-184",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 225,
      "discipline_id": 225,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 184",
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
      "updated_at": "2016-11-03T12:34:22.545Z",
      "shortname": "mit-course-184"
    },
    {
      "creator_id": 749,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-185",
      "html_url": "https://goskive.com/course/mit-course-185",
      "slug": "mit-course-185",
      "university_id": 230,
      "additional_university_ids": [

      ],
      "topic_id": 226,
      "discipline_id": 226,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
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
      "updated_at": "2016-11-03T12:34:22.625Z",
      "shortname": "mit-course-185"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2826cc3d8e08bd2761144948b62264a682e8aa4a766097d9988b2a5a51835ef"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 94b0abc4a3bb2cb19cc48696e07cdbd9d2ee2b02f2d1a5fc42306c0f734315d2
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
        "created_at": "2016-11-03T12:33:59.036Z",
        "updated_at": "2016-11-03T12:33:59.036Z",
        "file_url": "memory://d17fb8546e9e73f57cea82858669b0a0.pdf",
        "course_id": 146,
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
        "created_at": "2016-11-03T12:33:59.116Z",
        "updated_at": "2016-11-03T12:33:59.116Z",
        "file_url": "memory://8a0f7c9de8fd008c73e5b0d5f9b56a50.pdf",
        "course_id": 147,
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
        "created_at": "2016-11-03T12:33:59.193Z",
        "updated_at": "2016-11-03T12:33:59.193Z",
        "file_url": "memory://331de9a9d6b2d4e03a85705a2ec3ec43.pdf",
        "course_id": 148,
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
	-H "Authorization: Bearer 94b0abc4a3bb2cb19cc48696e07cdbd9d2ee2b02f2d1a5fc42306c0f734315d2"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a4bbb6fea1438ffebe33d8e9ff437c59109d0fe379bcdd7f205e717bb38725ff
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
        "updated_at": "2016-11-03T12:34:02.443Z"
      },
      "created_at": "2016-11-03T12:34:02.447Z",
      "updated_at": "2016-11-03T12:34:02.447Z",
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
        "updated_at": "2016-11-03T12:34:02.455Z"
      },
      "created_at": "2016-11-03T12:34:02.458Z",
      "updated_at": "2016-11-03T12:34:02.458Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4bbb6fea1438ffebe33d8e9ff437c59109d0fe379bcdd7f205e717bb38725ff"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 6a4cf3a45cb16164a4c87a74557b3d3c1a6743ac7271e524e126b99a2b46a831
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
        "updated_at": "2016-11-03T12:34:02.185Z"
      },
      "created_at": "2016-11-03T12:34:02.190Z",
      "updated_at": "2016-11-03T12:34:02.190Z",
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
        "updated_at": "2016-11-03T12:34:02.204Z"
      },
      "created_at": "2016-11-03T12:34:02.208Z",
      "updated_at": "2016-11-03T12:34:02.208Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a4cf3a45cb16164a4c87a74557b3d3c1a6743ac7271e524e126b99a2b46a831"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 90a6bc1ecd1825d0a66366e5f307e7e96ae6578ba1a26d0562aeb11c2f11f349
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
      "id": 17,
      "created_at": "2016-11-03T12:34:28.817Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 55,
      "updated_at": "2016-11-03T12:34:28.920Z",
      "author_id": "821",
      "thread_subject_id": "272",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 18,
      "created_at": "2016-11-03T12:34:28.909Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-11-03T12:34:28.923Z",
      "author_id": "824",
      "thread_subject_id": "273",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-11-03T12:34:29.298Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-11-03T12:34:29.298Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-11-03T12:34:29.652Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-11-03T12:34:29.652Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 21,
      "created_at": "2016-11-03T12:34:30.017Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 19,
      "updated_at": "2016-11-03T12:34:30.017Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 22,
      "created_at": "2016-11-03T12:34:30.303Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 106,
      "updated_at": "2016-11-03T12:34:30.303Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-11-03T12:34:30.617Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 107,
      "updated_at": "2016-11-03T12:34:30.617Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-11-03T12:34:30.907Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 108,
      "updated_at": "2016-11-03T12:34:30.907Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90a6bc1ecd1825d0a66366e5f307e7e96ae6578ba1a26d0562aeb11c2f11f349"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/16
Content-Type: application/json
Authorization: Bearer 8e9303fc455eea26cd61f970fef4976504326a295b7f9a810da3eccc5b4f943d
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-11-03T12:24:28.000Z"}}
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
    "id": 16,
    "created_at": "2016-11-03T12:34:28.657Z",
    "read_at": "2016-11-03T12:24:28.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 54,
    "updated_at": "2016-11-03T12:34:28.711Z",
    "author_id": "817",
    "thread_subject_id": "271",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/16" -d '{"notification":{"read_at":"2016-11-03T12:24:28.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e9303fc455eea26cd61f970fef4976504326a295b7f9a810da3eccc5b4f943d"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 5b0e098450134f23dede068ad5771b36a716beaa8409a539ddf40fe886acf84e
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
      "course_id": 38,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T12:33:36.936Z",
      "course_published": true,
      "updated_at": "2016-11-03T12:33:36.928Z"
    },
    {
      "id": 4,
      "course_id": 39,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-11-03T12:33:37.010Z",
      "course_published": true,
      "updated_at": "2016-11-03T12:33:37.003Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b0e098450134f23dede068ad5771b36a716beaa8409a539ddf40fe886acf84e"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer bf9b6e674d197a423d1bc8225d75decc44a9a9c30e9fd0159231dfd605c7cfab
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
    "id": 1,
    "course_id": 36,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-11-03T12:33:36.612Z",
    "course_published": true,
    "updated_at": "2016-11-03T12:33:36.603Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf9b6e674d197a423d1bc8225d75decc44a9a9c30e9fd0159231dfd605c7cfab"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/2
Content-Type: application/json
Authorization: Bearer 5ae0980629003ab8c5d85388d9d530854e9b229ecf28382b35e4f43ebd7bd328
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
    "course_id": 37,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-11-03T12:33:36.802Z",
    "course_published": true,
    "updated_at": "2016-11-03T12:33:36.792Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/2" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ae0980629003ab8c5d85388d9d530854e9b229ecf28382b35e4f43ebd7bd328"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer bcc482779b91ff49aa4ea861146228b8f9bf3c42ea37a5de32e5a0d3f027d4e7
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
      "votable_id": 48,
      "user_id": 353
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 49,
      "user_id": 353
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 50,
      "user_id": 353
    },
    {
      "id": 10,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 51,
      "user_id": 353
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcc482779b91ff49aa4ea861146228b8f9bf3c42ea37a5de32e5a0d3f027d4e7"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/227
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
    "id": 227,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 227,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 227
      },
      {
        "id": 228,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 227
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/227" -X GET \
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
      "id": 228,
      "name": "Reduced multi-state core",
      "name_translations": {
        "en": "Reduced multi-state core"
      }
    },
    {
      "id": 229,
      "name": "Implemented stable database",
      "name_translations": {
        "en": "Implemented stable database"
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
Authorization: Bearer ce26ee2256d71ea2651e47f6d5b328d5576b925505a7372c24b864c0fea54dc3
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
    "user_id": 25,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-11-03T12:33:28.601Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/2/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce26ee2256d71ea2651e47f6d5b328d5576b925505a7372c24b864c0fea54dc3"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 51f451b5cfe8bd156f79d9078c84c864ab1493c6d58efff4208917891a41d1b3
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
    "user_id": 138,
    "feedbackable_id": 8,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-11-03T12:33:35.928Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51f451b5cfe8bd156f79d9078c84c864ab1493c6d58efff4208917891a41d1b3"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/4
Content-Type: application/json
Authorization: Bearer 2323b996953d47c0fdf7bd5e9ed5be6550b2f68d183a7406f94044a06ef8cb6e
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
    "user_id": 35,
    "feedbackable_id": 4,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T12:33:29.093Z",
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
	-H "Authorization: Bearer 2323b996953d47c0fdf7bd5e9ed5be6550b2f68d183a7406f94044a06ef8cb6e"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/3/close
Content-Type: application/json
Authorization: Bearer 2d0c2c5c7178e7b7c9d2fd30d3e0edafc0e1b205658b34153e9f6cbdec4ab695
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
	-H "Authorization: Bearer 2d0c2c5c7178e7b7c9d2fd30d3e0edafc0e1b205658b34153e9f6cbdec4ab695"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer cb6c8daaaf3f555e846486d0968f4a602e9ceefb8012ef3e4be34e5b71621752
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
	-H "Authorization: Bearer cb6c8daaaf3f555e846486d0968f4a602e9ceefb8012ef3e4be34e5b71621752"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/28/fix
Content-Type: application/json
Authorization: Bearer 66b4d760b8516acd391a7decc1bfefee46604c1ac47e1a984035cd24bb681eb3
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
	-H "Authorization: Bearer 66b4d760b8516acd391a7decc1bfefee46604c1ac47e1a984035cd24bb681eb3"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/5
Content-Type: application/json
Authorization: Bearer bc99fc2f0caaf6b5209a6ac0464f629c56c6ad1dbc598b8fb84ad8ddc4e70055
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
    "user_id": 40,
    "feedbackable_id": 5,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T12:33:29.432Z",
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
	-H "Authorization: Bearer bc99fc2f0caaf6b5209a6ac0464f629c56c6ad1dbc598b8fb84ad8ddc4e70055"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer 48e1623c3c1ecd8ecba135dbee67e78eab35f5c8b6ae877b7b74d30cab4b8caf
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
	-H "Authorization: Bearer 48e1623c3c1ecd8ecba135dbee67e78eab35f5c8b6ae877b7b74d30cab4b8caf"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/6/bookmark
Content-Type: application/json
Authorization: Bearer a1f488185f713be708da664efd35339d445ead3a5e1bb3bf0eb5d3e4b54f724a
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1f488185f713be708da664efd35339d445ead3a5e1bb3bf0eb5d3e4b54f724a"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer afe04fbf66ced0899f7b7dbfb5945089a5401a12dabce279c67f69553f04efae
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer afe04fbf66ced0899f7b7dbfb5945089a5401a12dabce279c67f69553f04efae"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/10
Content-Type: application/json
Authorization: Bearer 621284de2ce51a8cd777152bbe086d697079c5cc791266c9d6e68be77b894eb4
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/4ad6f14f6aa1f3abb39b6c914a90644c.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T123403Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=db4d28b89dbb52a782407cdd0a1774183604b2ecab1b08f6aca8904d6d9d8a9f",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 621284de2ce51a8cd777152bbe086d697079c5cc791266c9d6e68be77b894eb4"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/4/preview
Content-Type: application/json
Authorization: Bearer ad01a0a7eb4180d4fee6a5137b57c853d6163f24eaedc5eba4dd6533e6439506
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/70032f547c7ebd6cc48a34e9203b4989.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161103%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161103T123402Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=0e6cc74ac414c829ca74906db9b02b4c5c4b685e48c37fd06cba38796621f3f6",
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
	-H "Authorization: Bearer ad01a0a7eb4180d4fee6a5137b57c853d6163f24eaedc5eba4dd6533e6439506"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 9e07409e724a92d87219e388c907d37294fade5be889b3634b98717d08487be8
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
    "id": 8,
    "uploader": {
      "id": 526,
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
      "created_at": "2016-11-03T12:34:03.139Z",
      "updated_at": "2016-11-03T12:34:03.139Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-11-03T12:34:03.245Z",
    "updated_at": "2016-11-03T12:34:03.245Z",
    "course_id": 161,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e07409e724a92d87219e388c907d37294fade5be889b3634b98717d08487be8"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/22/matched_courses?required_cu_count=2
Authorization: Bearer e651b8c5e42f560d52441e53767e13615c4c5cd20ab3f35fa25f1c4c018aea49
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
      "creator_id": 919,
      "id": 300,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 285,
      "additional_university_ids": [

      ],
      "topic_id": 307,
      "discipline_id": 308,
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
      "chapters_updated_at": "2016-11-03T12:34:35.995Z",
      "updated_at": "2016-11-03T12:34:37.517Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 924,
      "id": 301,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-8d9e8593-b371-442d-b88f-6bcc3e93582b",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-8d9e8593-b371-442d-b88f-6bcc3e93582b",
      "slug": "mit-the-great-british-bake-off-8d9e8593-b371-442d-b88f-6bcc3e93582b",
      "university_id": 286,
      "additional_university_ids": [

      ],
      "topic_id": 308,
      "discipline_id": 309,
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
      "chapters_updated_at": "2016-11-03T12:34:35.995Z",
      "updated_at": "2016-11-03T12:34:38.043Z",
      "shortname": "mit-the-great-british-bake-off-8d9e8593-b371-442d-b88f-6bcc3e93582b"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/22/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer e651b8c5e42f560d52441e53767e13615c4c5cd20ab3f35fa25f1c4c018aea49"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/5/download
Content-Type: application/json
Authorization: Bearer f2344c9d455ae3916938f20a17e8d081492719ed69ea409b182b01590d93fa59
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/5/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2344c9d455ae3916938f20a17e8d081492719ed69ea409b182b01590d93fa59"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/16/report
Content-Type: application/json
Authorization: Bearer f0ce33771cf617b83952698236d520db5db700648d74beeb5960938a766c25af
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f0ce33771cf617b83952698236d520db5db700648d74beeb5960938a766c25af"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/12/bookmark
Content-Type: application/json
Authorization: Bearer 14cf51259abd1a15b87e43564de30545db78dc9e7effe591954fff4ee750ac9b
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14cf51259abd1a15b87e43564de30545db78dc9e7effe591954fff4ee750ac9b"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/11/upvote
Content-Type: application/json
Authorization: Bearer 542c5ac2a12666c5bb96da21cdbc346fb39f30b70f71020e063cbdeea1891880
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 542c5ac2a12666c5bb96da21cdbc346fb39f30b70f71020e063cbdeea1891880"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/37/comments
Content-Type: application/json
Authorization: Bearer 4c3d7712f48547caa1de9a6a0c1cbbab710c90cac17cc1a9a4cfebdbed45f802
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
    "id": 46,
    "author_id": 565,
    "reply_to_id": null,
    "created_at": "2016-11-03T12:34:05.935Z",
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
curl "api.goskive.com/v2/flashcards/37/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c3d7712f48547caa1de9a6a0c1cbbab710c90cac17cc1a9a4cfebdbed45f802"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/35/comments
Content-Type: application/json
Authorization: Bearer 8905ca9af6c425c646b6f59ba024736c2a8b97c1c1395c366fb1e24e698bfeed
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
    "id": 45,
    "author_id": 559,
    "reply_to_id": null,
    "created_at": "2016-11-03T12:34:05.469Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 37,
      "user_id": 559,
      "feedbackable_id": 35,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:05.466Z",
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
curl "api.goskive.com/v2/flashcards/35/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8905ca9af6c425c646b6f59ba024736c2a8b97c1c1395c366fb1e24e698bfeed"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/39/comments
Content-Type: application/json
Authorization: Bearer 75a212a7f1c2d5014fe45eba4cbc10e11761171e6d8e7b92b4a404f732608ef9
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
      "id": 47,
      "author_id": 574,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:34:06.389Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 575,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:34:06.404Z",
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
curl "api.goskive.com/v2/flashcards/39/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75a212a7f1c2d5014fe45eba4cbc10e11761171e6d8e7b92b4a404f732608ef9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/36/comments
Content-Type: application/json
Authorization: Bearer 8d9e0f7bd9e389867690e16febf3d4fdc1aa7d3f6ef8798020c6c7c953a4d373
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
curl "api.goskive.com/v2/flashcards/36/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d9e0f7bd9e389867690e16febf3d4fdc1aa7d3f6ef8798020c6c7c953a4d373"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer 1e5564bb5deefedb43510c08edd0b5409041ff7ca67fb70f42b21f075fe52320
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
    "id": 38,
    "user_id": 638,
    "feedbackable_id": 66,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-11-03T12:34:16.740Z",
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
curl "api.goskive.com/v2/flashcards/66/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e5564bb5deefedb43510c08edd0b5409041ff7ca67fb70f42b21f075fe52320"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/73/feedbacks
Content-Type: application/json
Authorization: Bearer 5744c654df1edbbd46a3363cf88ad40f1ef4ced2f0e595e8ee852aaf2a9c92bc
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
      "id": 45,
      "user_id": 673,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:18.244Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 672,
      "feedbackable_id": 73,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:18.234Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/73/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5744c654df1edbbd46a3363cf88ad40f1ef4ced2f0e595e8ee852aaf2a9c92bc"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/86/votes
Content-Type: application/json
Authorization: Bearer d92f830a80fd7b7f60fff8da3e96ded19bb0b21014a4ce10d9820758ecb9c4fc
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
      "votable_id": 86,
      "user_id": 902
    },
    {
      "id": 21,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 86,
      "user_id": 901
    },
    {
      "id": 20,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 86,
      "user_id": 900
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/86/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d92f830a80fd7b7f60fff8da3e96ded19bb0b21014a4ce10d9820758ecb9c4fc"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/14/republish
Content-Type: application/json
Authorization: Bearer 4b93725b54db341889b48c23f20190b5dd202bdf98e8f01ae8f052c946da10a5
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
curl "api.goskive.com/v2/flashcards/14/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4b93725b54db341889b48c23f20190b5dd202bdf98e8f01ae8f052c946da10a5"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/17/bookmark
Content-Type: application/json
Authorization: Bearer 2569e7a236aed18a1b40f84fea7f5ac41fae327454f51d23bf2626308380df25
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/17/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2569e7a236aed18a1b40f84fea7f5ac41fae327454f51d23bf2626308380df25"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/15
Content-Type: application/json
Authorization: Bearer 8a910c07e394a2ab67e0ee60fc90e367e61d267a9e975ccdfe1d74d126bb044a
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a910c07e394a2ab67e0ee60fc90e367e61d267a9e975ccdfe1d74d126bb044a"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/34/downvote
Content-Type: application/json
Authorization: Bearer b45e8f67cb6dfb7bdac45f558bab9c0a1b6447cc4ce1cfe4a7e4e6953ff8639b
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b45e8f67cb6dfb7bdac45f558bab9c0a1b6447cc4ce1cfe4a7e4e6953ff8639b"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/11
Content-Type: application/json
Authorization: Bearer ba343c199a00cc37aeb9753a185bc31051f06a9792ae5d5d7ddf4bfc6175a439
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
    "id": 11,
    "obfuscated_id": "KS_N8rRWCuE",
    "author_id": 392,
    "chapter_id": 68,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:33:55.103Z",
    "created_at": "2016-11-03T12:33:55.103Z",
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
curl "api.goskive.com/v2/flashcards/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ba343c199a00cc37aeb9753a185bc31051f06a9792ae5d5d7ddf4bfc6175a439"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/report
Content-Type: application/json
Authorization: Bearer 0466dc5595bf63865272ce3ef5080264476476370030fd7a9fb3d333875140ad
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0466dc5595bf63865272ce3ef5080264476476370030fd7a9fb3d333875140ad"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/12/bookmark
Content-Type: application/json
Authorization: Bearer 7eb4856bbd35f92407b3ddc76e872834b5cd99de4a3bc70db7f16a07b5df22a5
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/12/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7eb4856bbd35f92407b3ddc76e872834b5cd99de4a3bc70db7f16a07b5df22a5"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/16/upvote
Content-Type: application/json
Authorization: Bearer 2a176b9f84008e7c164dd68ccd6034c5a6568656a24b511d4fa5ffb65fa9093c
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a176b9f84008e7c164dd68ccd6034c5a6568656a24b511d4fa5ffb65fa9093c"
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
    "key": "cache/bde462987d613d3a2e505b6c283efb30.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMS0wM1QxMzozNDowOFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2JkZTQ2Mjk4N2Q2MTNkM2EyZTUwNWI2YzI4M2VmYjMwLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTEwMy9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjExMDNUMTIzNDA4WiJ9XX0=",
    "x-amz-credential": "FAKE/20161103/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161103T123408Z",
    "x-amz-signature": "e959d9d1825c68f6e3684b1199d1695a4099c2eea5836bcca15f5910b4ed7ccb"
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
Authorization: Bearer bc851eead45a9b7bb1ada96bb25032ffca3c140571f3ba7061f676ee1e58e8dc
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
	-H "Authorization: Bearer bc851eead45a9b7bb1ada96bb25032ffca3c140571f3ba7061f676ee1e58e8dc"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/7/sign_ups
Content-Type: application/json
Authorization: Bearer 1256ed5beaa7f82345230712890af23541f975a28e1aa03d1c2b3776ec395413
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
	-H "Authorization: Bearer 1256ed5beaa7f82345230712890af23541f975a28e1aa03d1c2b3776ec395413"
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
{"password":{"reset_password_token":"gfz5WYapgCkhZVxXSWGx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 576,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-11-03T12:34:06.450Z",
  "updated_at": "2016-11-03T12:34:07.050Z",
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
  "audit_id": 4278
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"gfz5WYapgCkhZVxXSWGx","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/125/comments
Content-Type: application/json
Authorization: Bearer 449d8601e2a8df7698764f4613feeb876f7f795e7fd0be66fb298cf474f9dbe6
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
    "id": 57,
    "author_id": 935,
    "reply_to_id": null,
    "created_at": "2016-11-03T12:34:38.827Z",
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
curl "api.goskive.com/v2/questions/125/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 449d8601e2a8df7698764f4613feeb876f7f795e7fd0be66fb298cf474f9dbe6"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/126/comments
Content-Type: application/json
Authorization: Bearer a74cba6123d82186961bbd89e94d9f9d4ce28b0b7733eb30bf4b1b26cc527ef9
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
    "id": 58,
    "author_id": 938,
    "reply_to_id": null,
    "created_at": "2016-11-03T12:34:39.272Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 46,
      "user_id": 938,
      "feedbackable_id": 126,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:39.268Z",
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
curl "api.goskive.com/v2/questions/126/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a74cba6123d82186961bbd89e94d9f9d4ce28b0b7733eb30bf4b1b26cc527ef9"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/127/comments
Content-Type: application/json
Authorization: Bearer 69bf60bf4456356f4777ee11de6065c70f23305d12c016aab9eaf7c0aad0fb79
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
      "id": 60,
      "author_id": 945,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:34:39.721Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 59,
      "author_id": 944,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:34:39.706Z",
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
curl "api.goskive.com/v2/questions/127/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69bf60bf4456356f4777ee11de6065c70f23305d12c016aab9eaf7c0aad0fb79"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/124/comments
Content-Type: application/json
Authorization: Bearer 6dacb19888d41f71b015c94714e2a7713c5dc3a15540676d8b768e0d4237a94e
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
curl "api.goskive.com/v2/questions/124/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dacb19888d41f71b015c94714e2a7713c5dc3a15540676d8b768e0d4237a94e"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/64/feedbacks
Content-Type: application/json
Authorization: Bearer c79ee396a045cb5e2b2c74c3f6468e9faa2a499c241589a7be17c49397a834fb
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
    "id": 35,
    "user_id": 506,
    "feedbackable_id": 64,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-11-03T12:34:01.511Z",
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
curl "api.goskive.com/v2/questions/64/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c79ee396a045cb5e2b2c74c3f6468e9faa2a499c241589a7be17c49397a834fb"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/61/feedbacks
Content-Type: application/json
Authorization: Bearer 571b1aea888f8abceaf7716144f82668335ae56b77e996a1824818198464557e
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
      "id": 32,
      "user_id": 491,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:00.481Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 490,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:00.469Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/61/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 571b1aea888f8abceaf7716144f82668335ae56b77e996a1824818198464557e"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/21/votes
Content-Type: application/json
Authorization: Bearer 9b446c4f91c0761aaeb0e1a04728ce50183612bf185127b5d74485ff2e41af21
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
      "votable_id": 21,
      "user_id": 171
    },
    {
      "id": 3,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 21,
      "user_id": 170
    },
    {
      "id": 2,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 21,
      "user_id": 169
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/21/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b446c4f91c0761aaeb0e1a04728ce50183612bf185127b5d74485ff2e41af21"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/47/republish
Content-Type: application/json
Authorization: Bearer 2d93860aaf08e308c7f4d0750e0c4d1fff5fb92cb374d6a8de7fc06a81b979a0
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
curl "api.goskive.com/v2/questions/47/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d93860aaf08e308c7f4d0750e0c4d1fff5fb92cb374d6a8de7fc06a81b979a0"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/25/bookmark
Content-Type: application/json
Authorization: Bearer 1bbc28a0ae66c6d26d5ea4bde2efa7f795b6ff70f0594b50b552e4768c434164
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/25/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bbc28a0ae66c6d26d5ea4bde2efa7f795b6ff70f0594b50b552e4768c434164"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/27
Content-Type: application/json
Authorization: Bearer 45031e3bc01f1e3a99f877c5afaac4ea5e39eb793ce55e4d35f9e98cbb2dccb5
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/27" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 45031e3bc01f1e3a99f877c5afaac4ea5e39eb793ce55e4d35f9e98cbb2dccb5"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/26/downvote
Content-Type: application/json
Authorization: Bearer 6840ce81952d435e8c0c2ff3c47fc56427c2ae3d74b0b3c137dd255156ab0af6
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/26/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6840ce81952d435e8c0c2ff3c47fc56427c2ae3d74b0b3c137dd255156ab0af6"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/43
Content-Type: application/json
Authorization: Bearer 22d32dcf79bebd442080c92f655d7eaf1f33747f51414926ec166adab6299f00
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
    "id": 43,
    "obfuscated_id": "uapnSdBCag8",
    "author_id": 240,
    "chapter_id": 52,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:33:45.342Z",
    "created_at": "2016-11-03T12:33:45.230Z",
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
}
```



```shell
curl "api.goskive.com/v2/questions/43" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22d32dcf79bebd442080c92f655d7eaf1f33747f51414926ec166adab6299f00"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/44/report
Content-Type: application/json
Authorization: Bearer fb0a908968980069119aa282ae28472ef65d2cbc9aebf3ddc45d4f2fcab38f41
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/44/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb0a908968980069119aa282ae28472ef65d2cbc9aebf3ddc45d4f2fcab38f41"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/24/bookmark
Content-Type: application/json
Authorization: Bearer a1f2210b5ce507d885deaa32fa8dda058eba9ab64b068e16a8bd19bef6aa24c1
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/24/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1f2210b5ce507d885deaa32fa8dda058eba9ab64b068e16a8bd19bef6aa24c1"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/23
Content-Type: application/json
Authorization: Bearer 52f3e5ec457711bffab952d031149f44b95515c41e546ea0f5a6224ac1f30c9d
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":23,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T12:33:38.949Z","updated_at":"2016-11-03T12:33:39.058Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":32,"author_id":175,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 23,
    "obfuscated_id": "eUsQCUPDncM",
    "author_id": 175,
    "chapter_id": 32,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-11-03T12:33:39.196Z",
    "created_at": "2016-11-03T12:33:38.949Z",
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
    "question": "{\"id\"=>23, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-11-03T12:33:38.949Z\", \"updated_at\"=>\"2016-11-03T12:33:39.058Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>32, \"author_id\"=>175, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 45,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 46,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 47,
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
curl "api.goskive.com/v2/questions/23" -d '{"question":{"question":{"id":23,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-11-03T12:33:38.949Z","updated_at":"2016-11-03T12:33:39.058Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":32,"author_id":175,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52f3e5ec457711bffab952d031149f44b95515c41e546ea0f5a6224ac1f30c9d"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/45/upvote
Content-Type: application/json
Authorization: Bearer c4c214c7393984c38b2cfe718af7607f4fd69c3513f82fa04ff7e3c78c2025ab
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4c214c7393984c38b2cfe718af7607f4fd69c3513f82fa04ff7e3c78c2025ab"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 482e91f63f825179891b46c9bfe07d60a4f91aa0188f89c47950c05f124c9a0f
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
      "creator_id": 890,
      "id": 291,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 274,
      "additional_university_ids": [

      ],
      "topic_id": 298,
      "discipline_id": 299,
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
      "updated_at": "2016-11-03T12:34:34.755Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 482e91f63f825179891b46c9bfe07d60a4f91aa0188f89c47950c05f124c9a0f"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer cdd558f23c42730e43e54176f3bdd9370e0fa747c72a01daffaabc8cf1a313c6
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
      "id": 277,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-257",
      "html_url": "https://goskive.com/university/uni-257",
      "slug": "uni-257",
      "name": "National School of Pizza",
      "short_name": "Uni 257",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6189ce3ca7ff042fc2c341aa624f3178f99d4bf4.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/55f5964a1205c667878a4707415ac747d953a94b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T12:34:34.994Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 276,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-256",
      "html_url": "https://goskive.com/university/uni-256",
      "slug": "uni-256",
      "name": "National School of Pastry",
      "short_name": "Uni 256",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/e187b40d5c88ebf5f4ae2db7d5fd22938b12dfe6.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/faa33f9bffd7dfbce3ef586ec9f34124b0f8022b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T12:34:34.978Z",
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
	-H "Authorization: Bearer cdd558f23c42730e43e54176f3bdd9370e0fa747c72a01daffaabc8cf1a313c6"
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
      "id": 285,
      "name": "Self-enabling national approach",
      "name_translations": {
        "en": "Self-enabling national approach"
      },
      "discipline_id": 286
    },
    {
      "id": 286,
      "name": "Optimized 5th generation support",
      "name_translations": {
        "en": "Optimized 5th generation support"
      },
      "discipline_id": 287
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
GET /v2/topics/284
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
    "id": 284,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 285
  }
}
```



```shell
curl "api.goskive.com/v2/topics/284" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 2ea63ad086c1e10952de25dd3b63f585e7e236f3f261e9d2132e1ba80ef4e6b9
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
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-71",
      "html_url": "https://goskive.com/university/uni-71",
      "slug": "uni-71",
      "name": "University 65",
      "short_name": "Uni 71",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/6815e8d7e9cbcb148f1da5faa12acfad6db49257.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b48f9d0cebdb7956f7b23dc7411c7261eca3d96a.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T12:33:46.987Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-72",
      "html_url": "https://goskive.com/university/uni-72",
      "slug": "uni-72",
      "name": "University 66",
      "short_name": "Uni 72",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/eb17af409208ca654f585bc4d7642861365b7674.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/a2acc3b39b369b62935ab17303fbc0d252cb6b91.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T12:33:47.004Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-73",
      "html_url": "https://goskive.com/university/uni-73",
      "slug": "uni-73",
      "name": "University 67",
      "short_name": "Uni 73",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/5ea26c0fe407ac9aecae4409b94b03910c0208ce.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9af5cde7ee37bf1949b95d1335e8e2a4af7a4bf8.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-11-03T12:33:47.020Z",
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
	-H "Authorization: Bearer 2ea63ad086c1e10952de25dd3b63f585e7e236f3f261e9d2132e1ba80ef4e6b9"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer c0b70e13c6832374167f750a6c02106074929eb94db6c3a8dff1e6647e0ada42
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
    "id": 74,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cb2a218358d44a5056fe2e55e738cd09577c8a5c.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b5ad29aed1943ad0d14839f7d56c62a22a0b6452.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-11-03T12:33:47.082Z",
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
	-H "Authorization: Bearer c0b70e13c6832374167f750a6c02106074929eb94db6c3a8dff1e6647e0ada42"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 6cfc6eaa12b9de00c97d90751352b98ec34c74f8a8c3981ac1fc153bd727246a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":268,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 801,
    "id": 264,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 248,
    "additional_university_ids": [

    ],
    "topic_id": 268,
    "discipline_id": 269,
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
    "chapters_updated_at": "2016-11-03T12:34:27.245Z",
    "updated_at": "2016-11-03T12:34:27.380Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 160,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-11-03T12:34:27.338Z",
        "course_id": 264,
        "author_id": 801,
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
        "id": 161,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-11-03T12:34:27.355Z",
        "course_id": 264,
        "author_id": 801,
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
        "id": 162,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-11-03T12:34:27.371Z",
        "course_id": 264,
        "author_id": 801,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":268,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cfc6eaa12b9de00c97d90751352b98ec34c74f8a8c3981ac1fc153bd727246a"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer edceec482a5733d5b9c0a80687b5f55b4632430df2b8dbb1d577f14c75168df8
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":267,"published":false}}
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
    "creator_id": 800,
    "id": 263,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 247,
    "additional_university_ids": [

    ],
    "topic_id": 267,
    "discipline_id": 268,
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
    "updated_at": "2016-11-03T12:34:27.210Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":267,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer edceec482a5733d5b9c0a80687b5f55b4632430df2b8dbb1d577f14c75168df8"
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
      "creator_id": 770,
      "id": 237,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-198",
      "html_url": "https://goskive.com/course/fu-course-198",
      "slug": "fu-course-198",
      "university_id": 236,
      "additional_university_ids": [

      ],
      "topic_id": 241,
      "discipline_id": 242,
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
      "updated_at": "2016-11-03T12:34:24.625Z",
      "shortname": "fu-course-198"
    },
    {
      "creator_id": 770,
      "id": 238,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-199",
      "html_url": "https://goskive.com/course/fu-course-199",
      "slug": "fu-course-199",
      "university_id": 236,
      "additional_university_ids": [

      ],
      "topic_id": 242,
      "discipline_id": 243,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 199",
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
      "chapters_updated_at": "2016-11-03T12:34:24.902Z",
      "updated_at": "2016-11-03T12:34:24.908Z",
      "shortname": "fu-course-199"
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
Authorization: Bearer 7999b1b2215035191be4b3ba05c59ac57cf5f27f0fe39bbdcb7b52bff32a0658
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
      "creator_id": 787,
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 242,
      "additional_university_ids": [

      ],
      "topic_id": 257,
      "discipline_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
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
      "updated_at": "2016-11-03T12:34:26.145Z",
      "shortname": "fu-course-214"
    },
    {
      "creator_id": 787,
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 242,
      "additional_university_ids": [

      ],
      "topic_id": 258,
      "discipline_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
      "chapters_updated_at": "2016-11-03T12:34:26.419Z",
      "updated_at": "2016-11-03T12:34:26.425Z",
      "shortname": "fu-course-215"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7999b1b2215035191be4b3ba05c59ac57cf5f27f0fe39bbdcb7b52bff32a0658"
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
      "creator_id": 775,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-202",
      "html_url": "https://goskive.com/course/fu-course-202",
      "slug": "fu-course-202",
      "university_id": 237,
      "additional_university_ids": [

      ],
      "topic_id": 245,
      "discipline_id": 246,
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
      "updated_at": "2016-11-03T12:34:25.082Z",
      "shortname": "fu-course-202"
    },
    {
      "creator_id": 775,
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-203",
      "html_url": "https://goskive.com/course/fu-course-203",
      "slug": "fu-course-203",
      "university_id": 237,
      "additional_university_ids": [

      ],
      "topic_id": 246,
      "discipline_id": 247,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 203",
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
      "updated_at": "2016-11-03T12:34:25.121Z",
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
Authorization: Bearer 08f5965e21e655859c4aa261b1419a6af82a3951ba17c5a2be515ddc24e9c74d
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
      "creator_id": 793,
      "id": 257,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-218",
      "html_url": "https://goskive.com/course/fu-course-218",
      "slug": "fu-course-218",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 261,
      "discipline_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 218",
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
      "updated_at": "2016-11-03T12:34:26.638Z",
      "shortname": "fu-course-218"
    },
    {
      "creator_id": 793,
      "id": 258,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-219",
      "html_url": "https://goskive.com/course/fu-course-219",
      "slug": "fu-course-219",
      "university_id": 243,
      "additional_university_ids": [

      ],
      "topic_id": 262,
      "discipline_id": 263,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 219",
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
      "updated_at": "2016-11-03T12:34:26.678Z",
      "shortname": "fu-course-219"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08f5965e21e655859c4aa261b1419a6af82a3951ba17c5a2be515ddc24e9c74d"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer e7d2c7b0a95b7af272d6e7aa2de9c0ffc4fa90c3b507ec5d0695c89e528c5fd0
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
  "id": 161,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-11-03T12:33:37.285Z",
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
	-H "Authorization: Bearer e7d2c7b0a95b7af272d6e7aa2de9c0ffc4fa90c3b507ec5d0695c89e528c5fd0"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/145
Content-Type: application/json
Authorization: Bearer 9cc4992571c0bb81ed157054fb1bc6d1145e069f82bab5556d8a8f175a9a04aa
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
    "id": 145,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 36,
    "fields_of_study": [
      36,
      37
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-11-03T12:33:36.375Z",
    "updated_at": "2016-11-03T12:33:36.375Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/145" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cc4992571c0bb81ed157054fb1bc6d1145e069f82bab5556d8a8f175a9a04aa"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/147
Content-Type: application/json
Authorization: Bearer 88f1245095e3ec8ec8c1aa6cf74d1f7d884d5b0c3bb696e22a866f0b0426ab34
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
    "id": 147,
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
    "created_at": "2016-11-03T12:33:36.480Z",
    "updated_at": "2016-11-03T12:33:36.480Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/147" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88f1245095e3ec8ec8c1aa6cf74d1f7d884d5b0c3bb696e22a866f0b0426ab34"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/13
Content-Type: application/json
Authorization: Bearer 0814dd329efbb6371fa73ab11efe7feeaf5a77f3e6641b3af71fb163a5ad8669
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
	-H "Authorization: Bearer 0814dd329efbb6371fa73ab11efe7feeaf5a77f3e6641b3af71fb163a5ad8669"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/11
Content-Type: application/json
Authorization: Bearer 38f20da66d72aa65cee81e133cdb5961b8c21a42e6509ab53ff9c0d81ae6d118
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
    "id": 11,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 52,
    "user_id": 366
  }
}
```



```shell
curl "api.goskive.com/v2/votes/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38f20da66d72aa65cee81e133cdb5961b8c21a42e6509ab53ff9c0d81ae6d118"
```
