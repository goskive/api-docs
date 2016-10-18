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
Authorization: Basic MzExZGFiMmI2YzBkNzc1YjhmNTVmYzgxNTRiYzM0ZTMxMjc1ZTcxM2Y1ZjA3
YzQ4NGI3OTlhOWMwNmU4YTZlYTpmMzI2OTgyZjc5MjhhMzI0OTNjOTFiNmE1
MDExZWRhNDU2M2NlYzQxMDQ4NGVhODEzN2IyNTg0Njc2OWY0NjBk

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
	-u 311dab2b6c0d775b8f55fc8154bc34e31275e713f5f07c484b799a9c06e8a6ea:f326982f7928a32493c91b6a5011eda4563cec410484ea8137b25846769f460d
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
```

`POST /v2/oauth/token`

#### Parameters


```json
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a6244cba00594e721e73cab5d4c4c01fcb54846e12518ea814c55447419de829","client_secret":"38a7c27e9af2a28cd8375ec52a3f385a5b340bb9514d94f34922ddecf50da7f5"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"a6244cba00594e721e73cab5d4c4c01fcb54846e12518ea814c55447419de829","client_secret":"38a7c27e9af2a28cd8375ec52a3f385a5b340bb9514d94f34922ddecf50da7f5"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"5114c8cfb1fa18fbe7800373aba69283407420f964e214ff2c8016889f87a6dc","client_secret":"2be2f1c0573516db2c8387ccec986a4f4e07498dbe7431f0ab55635000e80b63"}
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
  "access_token": "1092450219b3ecdef1c53a2185d3fefa97bf1c1636e8e4b2248ea323eb4d25fe",
  "token_type": "bearer",
  "created_at": 1476788952
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"5114c8cfb1fa18fbe7800373aba69283407420f964e214ff2c8016889f87a6dc","client_secret":"2be2f1c0573516db2c8387ccec986a4f4e07498dbe7431f0ab55635000e80b63"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic ZWUzMjg4NGU4OWQyYmQ2YTg1ZWNhMmMwNzA1NWQyMzhjMjQ5NWFiZTM1YmM5
NDkyNWYzNzRlNGMzZTI3NGE0MToyMTA1NThhOWE4YzYxNzg5MjA0YzIyMjk2
MTNhNzAxY2RkNmI1ZGQ0ZTQ1MzQzZTE3YWM1YmY2OWRlZTMyMjE2

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
  "access_token": "873a3d07235e1fb1cc4be5fe10ff80675858f8b8e62aee56f21e034e81b1366a",
  "token_type": "bearer",
  "created_at": 1476788952
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u ee32884e89d2bd6a85eca2c07055d238c2495abe35bc94925f374e4c3e274a41:210558a9a8c61789204c2229613a701cdd6b5dd4e45343e17ac5bf69dee32216
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1f0000d2d256bcd38743b7810da89692dcf8f98bc2f7a5458c58880c383b4b9a","client_secret":"f5a9fbc8689872f7678b875b7fb8a1b2b9814fafd746117363ef66a18a65fb49"}
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
  "access_token": "f7c0751a7182485347545d416376447aa4893a44c00b85f4086c49082fe112d7",
  "token_type": "bearer",
  "created_at": 1476788952
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"1f0000d2d256bcd38743b7810da89692dcf8f98bc2f7a5458c58880c383b4b9a","client_secret":"f5a9fbc8689872f7678b875b7fb8a1b2b9814fafd746117363ef66a18a65fb49"}' -X POST \
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
Authorization: Bearer 21c70af1fd8fd865ffaf64d49598c3dbe7a693fb34b5702138934941461699a1
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
	-H "Authorization: Bearer 21c70af1fd8fd865ffaf64d49598c3dbe7a693fb34b5702138934941461699a1"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/189/flashcards
Content-Type: application/json
Authorization: Bearer f8f3eeee2e6525c574cc2178c21b61ae839a7ea6a1cda8d0b41becbe826fcfe8
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":189,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 88,
    "obfuscated_id": "CDc29JqT-RA",
    "author_id": 833,
    "chapter_id": 189,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:09:29.618Z",
    "created_at": "2016-10-18T11:09:29.618Z",
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
curl "api.goskive.com/v2/chapters/189/flashcards" -d '{"flashcard":{"chapter_id":189,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8f3eeee2e6525c574cc2178c21b61ae839a7ea6a1cda8d0b41becbe826fcfe8"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/191/flashcards
Content-Type: application/json
Authorization: Bearer c5e941ffd38cb8bac205865e9519fd12c5cdf17f836f4248f3c51a429e4f8dab
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 837,
      "chapter_id": 191,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:29.947Z",
      "created_at": "2016-10-18T11:09:29.947Z",
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
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 837,
      "chapter_id": 191,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:29.987Z",
      "created_at": "2016-10-18T11:09:29.987Z",
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
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 837,
      "chapter_id": 191,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:09:30.027Z",
      "created_at": "2016-10-18T11:09:30.027Z",
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
curl "api.goskive.com/v2/chapters/191/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5e941ffd38cb8bac205865e9519fd12c5cdf17f836f4248f3c51a429e4f8dab"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/41/questions
Content-Type: application/json
Authorization: Bearer 86081720084459b8ac643cfbb25d058d34ce163ff937bc4ea568458b8772940e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":41,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 166,
    "chapter_id": 41,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:31.332Z",
    "created_at": "2016-10-18T11:08:31.332Z",
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
        "id": 67,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 68,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 69,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 70,
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
curl "api.goskive.com/v2/chapters/41/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":41,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86081720084459b8ac643cfbb25d058d34ce163ff937bc4ea568458b8772940e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/39/questions
Content-Type: application/json
Authorization: Bearer 5a0f824288297a040d12e9eb07edef3575142425af356ace12fa0175fe4b22a8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":39,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 160,
    "chapter_id": 39,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:30.672Z",
    "created_at": "2016-10-18T11:08:30.672Z",
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
        "id": 63,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 64,
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
curl "api.goskive.com/v2/chapters/39/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":39,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a0f824288297a040d12e9eb07edef3575142425af356ace12fa0175fe4b22a8"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/40/questions
Content-Type: application/json
Authorization: Bearer c3e9bf70e05a3b97faaf2201e1f2507ea6ba3f84f3f6715ec06b88eac3aff95e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":40,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 163,
    "chapter_id": 40,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:31.001Z",
    "created_at": "2016-10-18T11:08:31.001Z",
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
        "id": 65,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 66,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/40/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":40,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3e9bf70e05a3b97faaf2201e1f2507ea6ba3f84f3f6715ec06b88eac3aff95e"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/38/questions
Content-Type: application/json
Authorization: Bearer 59041c7e69b505e081f7a90ae97078dc12338872747dd1919f596809d68a5e0d
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":38,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 157,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:30.265Z",
    "created_at": "2016-10-18T11:08:30.265Z",
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
        "id": 60,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 61,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 62,
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
curl "api.goskive.com/v2/chapters/38/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":38,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59041c7e69b505e081f7a90ae97078dc12338872747dd1919f596809d68a5e0d"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/42/questions
Content-Type: application/json
Authorization: Bearer 1b1ecf304585089525ea38830685b03ef5e764ea75d462a7c30721c9c914af25
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 169,
      "chapter_id": 42,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:31.914Z",
      "created_at": "2016-10-18T11:08:31.799Z",
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
          "id": 71,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 72,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 170,
      "chapter_id": 42,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:32.103Z",
      "created_at": "2016-10-18T11:08:31.984Z",
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
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 171,
      "chapter_id": 42,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-18T11:08:32.299Z",
      "created_at": "2016-10-18T11:08:32.176Z",
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
          "id": 75,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 76,
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
curl "api.goskive.com/v2/chapters/42/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b1ecf304585089525ea38830685b03ef5e764ea75d462a7c30721c9c914af25"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/143
Content-Type: application/json
Authorization: Bearer 53a9bc0065d36764b78df03ef89bad3d8cb32580f9fc9905de895fd74735fad7
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
	-H "Authorization: Bearer 53a9bc0065d36764b78df03ef89bad3d8cb32580f9fc9905de895fd74735fad7"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/145
Content-Type: application/json
Authorization: Bearer f39b9488972bd12581f18a5a905ce29fac52856cf147ddedd69f641a34b5da96
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
curl "api.goskive.com/v2/chapters/145" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f39b9488972bd12581f18a5a905ce29fac52856cf147ddedd69f641a34b5da96"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/142
Content-Type: application/json
Authorization: Bearer 03510086ed729c8f1a06ba72206613381efab9ad874e4407aeaea48cbae075ff
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
curl "api.goskive.com/v2/chapters/142" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03510086ed729c8f1a06ba72206613381efab9ad874e4407aeaea48cbae075ff"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/144
Content-Type: application/json
Authorization: Bearer c18098dbfde1a5818cd346e6052ace924e1714afadc24574dc6a66579e585615
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/144" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c18098dbfde1a5818cd346e6052ace924e1714afadc24574dc6a66579e585615"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/147
Content-Type: application/json
Authorization: Bearer bfc649b9ff1646259dd78fcfccef134a9e2c6214938411c2012e5e5422a1e57b
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
    "updated_at": "2016-10-18T11:09:11.619Z",
    "course_id": 190,
    "author_id": 589,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-18T11:09:11.039Z",
    "questions_updated_at": "2016-10-18T11:09:11.039Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 593,
        "chapter_id": 147,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:11.599Z",
        "created_at": "2016-10-18T11:09:11.599Z",
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
        "id": 112,
        "obfuscated_id": "7Qwj1ZvbWUI",
        "author_id": 591,
        "chapter_id": 147,
        "position": 99,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:09:11.483Z",
        "created_at": "2016-10-18T11:09:11.351Z",
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
            "id": 227,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 228,
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
	-H "Authorization: Bearer bfc649b9ff1646259dd78fcfccef134a9e2c6214938411c2012e5e5422a1e57b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/141
Content-Type: application/json
Authorization: Bearer 5b1eff35552160002ec62d01ea8e2e181002f64386dff35038fc35ed27f2af7b
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
    "updated_at": "2016-10-18T11:09:09.888Z",
    "course_id": 184,
    "author_id": 572,
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
	-H "Authorization: Bearer 5b1eff35552160002ec62d01ea8e2e181002f64386dff35038fc35ed27f2af7b"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/13/replies
Content-Type: application/json
Authorization: Bearer ad4e9dab771bb782770755b6928531e76ab67c1d5dcbb9c5e5f6314de25c92f9
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
    "author_id": 365,
    "reply_to_id": 13,
    "created_at": "2016-10-18T11:08:47.920Z",
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
	-H "Authorization: Bearer ad4e9dab771bb782770755b6928531e76ab67c1d5dcbb9c5e5f6314de25c92f9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/15/replies
Content-Type: application/json
Authorization: Bearer 330d0a0538651b024ae85e1415145c66a5ea24c1c9827f1abb6ff3830b403fac
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
curl "api.goskive.com/v2/comments/15/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 330d0a0538651b024ae85e1415145c66a5ea24c1c9827f1abb6ff3830b403fac"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/58
Content-Type: application/json
Authorization: Bearer 23c8edf48efc5d5f9fd6ef639f5779c471b1f7b61c9e58f70ab81e47842308b4
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
curl "api.goskive.com/v2/comments/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 23c8edf48efc5d5f9fd6ef639f5779c471b1f7b61c9e58f70ab81e47842308b4"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/55/republish
Content-Type: application/json
Authorization: Bearer d588b93378dc094ee379dd09d0b4eb91078da0e007abc1af90d0b7697656cb27
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
curl "api.goskive.com/v2/comments/55/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d588b93378dc094ee379dd09d0b4eb91078da0e007abc1af90d0b7697656cb27"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/60
Content-Type: application/json
Authorization: Bearer 2da10307ca1ebdf2c4e6ba991695ed2e05fbd2ebcff2aa881e044107888c1053
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2da10307ca1ebdf2c4e6ba991695ed2e05fbd2ebcff2aa881e044107888c1053"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/57/report
Content-Type: application/json
Authorization: Bearer f937748c5fe6f9863ca3b02b197f76bf37aab1696b44eb816d6ddb79a95f2978
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f937748c5fe6f9863ca3b02b197f76bf37aab1696b44eb816d6ddb79a95f2978"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/15
Content-Type: application/json
Authorization: Bearer 5d5dab9580217e85a1e5d95c1ac20cede95933e5795ab505dd8b4ed63699e2ae
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
    "id": 15,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-18T11:09:18.412Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d5dab9580217e85a1e5d95c1ac20cede95933e5795ab505dd8b4ed63699e2ae"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 585668fa73c3a8f5f8b322f6ca6b94af9e9390842d03741e1b6c0ce94eadca80
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
      "id": 12,
      "name": "Fake Company Name 12",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T11:09:18.349Z"
    },
    {
      "id": 13,
      "name": "Fake Company Name 13",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T11:09:18.353Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 14",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-18T11:09:18.357Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 585668fa73c3a8f5f8b322f6ca6b94af9e9390842d03741e1b6c0ce94eadca80"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/38/company_profiles
Content-Type: application/json
Authorization: Bearer 4b81bd4553b41dc3fe97c2d61ff8c5a644eb0cf37533f2522a8a7ea7f2ff215d
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
	-H "Authorization: Bearer 4b81bd4553b41dc3fe97c2d61ff8c5a644eb0cf37533f2522a8a7ea7f2ff215d"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/37/company_profiles
Content-Type: application/json
Authorization: Bearer f407b08c7e963ada37cf21e8990d4f5ef4e3410633d7eda5977049b40859b685
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
	-H "Authorization: Bearer f407b08c7e963ada37cf21e8990d4f5ef4e3410633d7eda5977049b40859b685"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 4f0f0f7a0ef92a4644b5f615054066333591433282eb29df50573de5b3c099ca
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
	-H "Authorization: Bearer 4f0f0f7a0ef92a4644b5f615054066333591433282eb29df50573de5b3c099ca"
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
Authorization: Bearer 30ce70e32e8fb48d76ea4a668f353a3d83ede42abe1daa7214d8ed2b2b878510
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
	-H "Authorization: Bearer 30ce70e32e8fb48d76ea4a668f353a3d83ede42abe1daa7214d8ed2b2b878510"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7d240768637fd3e668c8ead0ff8f8dff3a36330ab42305631d3841871022c3a6
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
    "id": 69,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-18T11:08:42.731Z",
    "course_id": 113,
    "author_id": 295,
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
	-H "Authorization: Bearer 7d240768637fd3e668c8ead0ff8f8dff3a36330ab42305631d3841871022c3a6"
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
      "id": 70,
      "title": "Clever Chapter Title 58",
      "position": 1,
      "updated_at": "2016-10-18T11:08:42.945Z",
      "course_id": 115,
      "author_id": 299,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 71,
      "title": "Clever Chapter Title 59",
      "position": 2,
      "updated_at": "2016-10-18T11:08:42.969Z",
      "course_id": 115,
      "author_id": 300,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 72,
      "title": "Clever Chapter Title 60",
      "position": 3,
      "updated_at": "2016-10-18T11:08:43.236Z",
      "course_id": 115,
      "author_id": 301,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T11:08:42.870Z",
      "questions_updated_at": "2016-10-18T11:08:42.870Z",
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
Authorization: Bearer ce209b5b5efc716a39b0aad1965902957ebea2cbc83c74db2e1410fad2903f35
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
      "id": 76,
      "title": "Clever Chapter Title 64",
      "position": 1,
      "updated_at": "2016-10-18T11:08:43.609Z",
      "course_id": 118,
      "author_id": 310,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 77,
      "title": "Clever Chapter Title 65",
      "position": 2,
      "updated_at": "2016-10-18T11:08:43.634Z",
      "course_id": 118,
      "author_id": 311,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 78,
      "title": "Clever Chapter Title 66",
      "position": 3,
      "updated_at": "2016-10-18T11:08:43.899Z",
      "course_id": 118,
      "author_id": 312,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-18T11:08:43.532Z",
      "questions_updated_at": "2016-10-18T11:08:43.532Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce209b5b5efc716a39b0aad1965902957ebea2cbc83c74db2e1410fad2903f35"
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
      "id": 73,
      "title": "Clever Chapter Title 61",
      "position": 1,
      "updated_at": "2016-10-18T11:08:43.362Z",
      "course_id": 116,
      "author_id": 305,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 74,
      "title": "Clever Chapter Title 62",
      "position": 2,
      "updated_at": "2016-10-18T11:08:43.388Z",
      "course_id": 116,
      "author_id": 306,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 75,
      "title": "Clever Chapter Title 63",
      "position": 3,
      "updated_at": "2016-10-18T11:08:43.414Z",
      "course_id": 116,
      "author_id": 307,
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
Authorization: Bearer e2af5830a77889685650e8f80a5ebe4d66bce8e2d2c74526a4a7827f4942526c
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
      "id": 79,
      "title": "Clever Chapter Title 67",
      "position": 1,
      "updated_at": "2016-10-18T11:08:44.186Z",
      "course_id": 120,
      "author_id": 319,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 80,
      "title": "Clever Chapter Title 68",
      "position": 2,
      "updated_at": "2016-10-18T11:08:44.211Z",
      "course_id": 120,
      "author_id": 320,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 81,
      "title": "Clever Chapter Title 69",
      "position": 3,
      "updated_at": "2016-10-18T11:08:44.236Z",
      "course_id": 120,
      "author_id": 321,
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
	-H "Authorization: Bearer e2af5830a77889685650e8f80a5ebe4d66bce8e2d2c74526a4a7827f4942526c"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 9b737db79c40d1686570c8df8014375deb8daa895068d9049690e8ccb25fa4dc
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
    "course_id": 199,
    "user_id": 634,
    "updated_at": "2016-10-18T11:09:14.491Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b737db79c40d1686570c8df8014375deb8daa895068d9049690e8ccb25fa4dc"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 1e1fe741f74e7bb00ece559353bf020551f91134473f21c1143a1e2801b45168
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
      "course_id": 197,
      "user_id": 628,
      "updated_at": "2016-10-18T11:09:14.165Z"
    },
    {
      "id": 4,
      "course_id": 197,
      "user_id": 629,
      "updated_at": "2016-10-18T11:09:14.181Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e1fe741f74e7bb00ece559353bf020551f91134473f21c1143a1e2801b45168"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/215/files
Content-Type: application/json
Authorization: Bearer 7df0ea7fd88598c317927b2d873499386d0ba448a3e459e110f06c4cad900083
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
      "id": 8,
      "uploader": {
        "id": 690,
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
        "created_at": "2016-10-18T11:09:19.620Z",
        "updated_at": "2016-10-18T11:09:19.620Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T11:09:19.629Z",
      "updated_at": "2016-10-18T11:09:19.629Z",
      "course_id": 215,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 9,
      "uploader": {
        "id": 691,
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
        "created_at": "2016-10-18T11:09:19.638Z",
        "updated_at": "2016-10-18T11:09:19.638Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T11:09:19.645Z",
      "updated_at": "2016-10-18T11:09:19.645Z",
      "course_id": 215,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 10,
      "uploader": {
        "id": 692,
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
        "created_at": "2016-10-18T11:09:19.653Z",
        "updated_at": "2016-10-18T11:09:19.653Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-18T11:09:19.661Z",
      "updated_at": "2016-10-18T11:09:19.661Z",
      "course_id": 215,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/215/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7df0ea7fd88598c317927b2d873499386d0ba448a3e459e110f06c4cad900083"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/218/files
Content-Type: application/json
Authorization: Bearer 59ebcee20dc8311954c00314365763f202201e821bf758990ea9de1fe667e9d2
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
    "id": 11,
    "uploader": {
      "id": 699,
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
      "created_at": "2016-10-18T11:09:20.011Z",
      "updated_at": "2016-10-18T11:09:20.011Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-18T11:09:20.042Z",
    "updated_at": "2016-10-18T11:09:20.042Z",
    "course_id": 218,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/218/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59ebcee20dc8311954c00314365763f202201e821bf758990ea9de1fe667e9d2"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/217/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer b5646aab458157137a60f211676cffc1374e3226e26b0ee6e4d00141bfe16c39
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
    "key": "cache/004c363174f33150393eef8568679b67.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMjowOToxOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS8wMDRjMzYzMTc0ZjMzMTUwMzkzZWVmODU2ODY3OWI2Ny5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOC9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMThUMTEwOTE5WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T110919Z",
    "x-amz-signature": "b1208346a2e1fceff729b797bdf77d0d6dad1119ebc72af8b79cf0baa2e9c992"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/217/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5646aab458157137a60f211676cffc1374e3226e26b0ee6e4d00141bfe16c39"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer ef5dad7d4bf3b607b782437ea449043be584c5998ed6982d04781f6d33f07ef9
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
	-H "Authorization: Bearer ef5dad7d4bf3b607b782437ea449043be584c5998ed6982d04781f6d33f07ef9"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d732aeec64797e67786764183935cbdf62af07475d5c128f045495cfa9dfecac
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
	-H "Authorization: Bearer d732aeec64797e67786764183935cbdf62af07475d5c128f045495cfa9dfecac"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6d0261969cccbab6e7356907f1e555fecd8bbc214efd50f23550dbe0b8f5f97f
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
	-H "Authorization: Bearer 6d0261969cccbab6e7356907f1e555fecd8bbc214efd50f23550dbe0b8f5f97f"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9812c754d05af3a0ada94e3a4b2a1501a7f361445219ae8f4005e087c301f4e8
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
	-H "Authorization: Bearer 9812c754d05af3a0ada94e3a4b2a1501a7f361445219ae8f4005e087c301f4e8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e0c268e66a5d884c0786722b29713c29458ce6f8da117ab4cd0c244a778097fe
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
	-H "Authorization: Bearer e0c268e66a5d884c0786722b29713c29458ce6f8da117ab4cd0c244a778097fe"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer a461ee39dc88d56f3afdf1725f111b57fd28521fe20cb628df7fdd6b1e87696d
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
    "creator_id": 383,
    "id": 139,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 119,
    "additional_university_ids": [

    ],
    "topic_id": 144,
    "discipline_id": 144,
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
    "chapters_updated_at": "2016-10-18T11:08:49.426Z",
    "updated_at": "2016-10-18T11:08:51.032Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 99,
        "title": "Clever Chapter Title 87",
        "position": 1,
        "updated_at": "2016-10-18T11:08:50.950Z",
        "course_id": 139,
        "author_id": 383,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T11:08:49.426Z",
        "questions_updated_at": "2016-10-18T11:08:49.426Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 100,
        "title": "Clever Chapter Title 88",
        "position": 2,
        "updated_at": "2016-10-18T11:08:51.023Z",
        "course_id": 139,
        "author_id": 383,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T11:08:49.426Z",
        "questions_updated_at": "2016-10-18T11:08:49.426Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 384,
        "chapter_id": 99,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.764Z",
        "created_at": "2016-10-18T11:08:50.764Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 384,
        "chapter_id": 100,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.850Z",
        "created_at": "2016-10-18T11:08:50.850Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 384,
        "chapter_id": 99,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.810Z",
        "created_at": "2016-10-18T11:08:50.810Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 384,
        "chapter_id": 100,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.894Z",
        "created_at": "2016-10-18T11:08:50.894Z",
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
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 384,
        "chapter_id": 99,
        "position": 50,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:49.652Z",
        "created_at": "2016-10-18T11:08:49.529Z",
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
            "id": 129,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 130,
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
        "author_id": 384,
        "chapter_id": 99,
        "position": 51,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:49.839Z",
        "created_at": "2016-10-18T11:08:49.722Z",
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
            "id": 131,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 132,
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
        "author_id": 384,
        "chapter_id": 100,
        "position": 52,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.058Z",
        "created_at": "2016-10-18T11:08:49.927Z",
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
            "id": 133,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 134,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 66,
        "obfuscated_id": "H7dODBospvw",
        "author_id": 384,
        "chapter_id": 100,
        "position": 53,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:50.258Z",
        "created_at": "2016-10-18T11:08:50.134Z",
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
            "id": 135,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 136,
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
	-H "Authorization: Bearer a461ee39dc88d56f3afdf1725f111b57fd28521fe20cb628df7fdd6b1e87696d"
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
    "creator_id": 395,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 121,
    "additional_university_ids": [

    ],
    "topic_id": 146,
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
    "chapters_updated_at": "2016-10-18T11:08:52.869Z",
    "updated_at": "2016-10-18T11:08:54.479Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 103,
        "title": "Clever Chapter Title 91",
        "position": 1,
        "updated_at": "2016-10-18T11:08:54.425Z",
        "course_id": 141,
        "author_id": 395,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T11:08:52.869Z",
        "questions_updated_at": "2016-10-18T11:08:52.869Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 104,
        "title": "Clever Chapter Title 92",
        "position": 2,
        "updated_at": "2016-10-18T11:08:54.470Z",
        "course_id": 141,
        "author_id": 395,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-18T11:08:52.869Z",
        "questions_updated_at": "2016-10-18T11:08:52.869Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 395,
        "chapter_id": 103,
        "position": 62,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:53.097Z",
        "created_at": "2016-10-18T11:08:52.968Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 395,
        "chapter_id": 104,
        "position": 64,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-18T11:08:53.526Z",
        "created_at": "2016-10-18T11:08:53.389Z",
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
            "id": 157,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 158,
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
PUT /v2/courses/134/pin
Content-Type: application/json
Authorization: Bearer 7f3d071d2f9d799b2038f28feb7f7899d98add31e4fcc4431232e3860256af48
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/134/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f3d071d2f9d799b2038f28feb7f7899d98add31e4fcc4431232e3860256af48"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/152/pin
Content-Type: application/json
Authorization: Bearer f33e93233df7d12a4c9f3eb88b2a70f803eb93a2bafe0565364fc7bcde5dd8ac
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/152/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f33e93233df7d12a4c9f3eb88b2a70f803eb93a2bafe0565364fc7bcde5dd8ac"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3dc4b5036cf6cd76fe08037559b7e93e588ee181622aa120be052a5c8d0b3f27
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
    "creator_id": 380,
    "id": 137,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 117,
    "additional_university_ids": [

    ],
    "topic_id": 142,
    "discipline_id": 142,
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
    "updated_at": "2016-10-18T11:08:49.253Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3dc4b5036cf6cd76fe08037559b7e93e588ee181622aa120be052a5c8d0b3f27"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 73d86e91e4a1a93baa3f6143c3ea3ee85b03f59b2009eaac6b633139589fcbf7
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
    "id": 959,
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
    "created_at": "2016-10-18T11:09:37.231Z",
    "updated_at": "2016-10-18T11:09:37.231Z",
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
	-H "Authorization: Bearer 73d86e91e4a1a93baa3f6143c3ea3ee85b03f59b2009eaac6b633139589fcbf7"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7c8876de0f7ff8b348a06912d97200b58c8932a7ee6533da2283cbfcce79da9c
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[315]}
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
    "id": 960,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      315
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T11:09:37.328Z",
    "updated_at": "2016-10-18T11:09:37.367Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[315]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c8876de0f7ff8b348a06912d97200b58c8932a7ee6533da2283cbfcce79da9c"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 32a42d4a456c3e23930c3828be503fb4eae47e859ab556015601bbb937b49921
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
    "id": 962,
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
    "created_at": "2016-10-18T11:09:37.471Z",
    "updated_at": "2016-10-18T11:09:37.471Z",
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
	-H "Authorization: Bearer 32a42d4a456c3e23930c3828be503fb4eae47e859ab556015601bbb937b49921"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 3cafd8eceffb80b3107b594956aad5e9483d02d0c3763d0005592e646a3aa201
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[318]}
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
    "id": 963,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      318
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T11:09:37.574Z",
    "updated_at": "2016-10-18T11:09:37.574Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[318]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3cafd8eceffb80b3107b594956aad5e9483d02d0c3763d0005592e646a3aa201"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 822dd0f67099b16d77d0d65df3bb7f45abbdd5cc57addbde1e8029c42f23f8cc
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

319
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
    "id": 964,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/9517d5394cc8e61e4099261bc917254d1f48b7c6.jpg",
    "university_id": null,
    "fields_of_study": [
      319
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-18T11:09:37.653Z",
    "updated_at": "2016-10-18T11:09:37.899Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/2c5da3c9e6f309a15866d26667b050cec0b0e7c5.jpg",
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

319
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 822dd0f67099b16d77d0d65df3bb7f45abbdd5cc57addbde1e8029c42f23f8cc"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 4d5f441e0bb039b2f587b32fa8eb1e42f9ac19077ae63a2a6418188cab294ad1
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
      "bookmarkable_id": 37,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 38,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 39,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d5f441e0bb039b2f587b32fa8eb1e42f9ac19077ae63a2a6418188cab294ad1"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 99d59952a7f3f6113923b3792d617ae2e2beee62198440255c035da11b35a042
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
      "company_id": 33,
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
      "company_id": 34,
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
	-H "Authorization: Bearer 99d59952a7f3f6113923b3792d617ae2e2beee62198440255c035da11b35a042"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 897ed612d3cc442a8fa4a181eb2e94e5907fc33bb390a506f808028e5164aae9
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
      "company_id": 29,
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
	-H "Authorization: Bearer 897ed612d3cc442a8fa4a181eb2e94e5907fc33bb390a506f808028e5164aae9"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 952f4331bd6866f2ea644793e659c7a90d86f1f9e843e4cf8590c70e61f4bf7f
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
      "creator_id": 702,
      "id": 219,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-156",
      "html_url": "https://goskive.com/course/mit-course-156",
      "slug": "mit-course-156",
      "university_id": 199,
      "additional_university_ids": [

      ],
      "topic_id": 226,
      "discipline_id": 227,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 156",
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
      "updated_at": "2016-10-18T11:09:20.374Z",
      "shortname": "mit-course-156"
    },
    {
      "creator_id": 703,
      "id": 220,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-157",
      "html_url": "https://goskive.com/course/mit-course-157",
      "slug": "mit-course-157",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 227,
      "discipline_id": 228,
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
      "updated_at": "2016-10-18T11:09:20.468Z",
      "shortname": "mit-course-157"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 952f4331bd6866f2ea644793e659c7a90d86f1f9e843e4cf8590c70e61f4bf7f"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 05511d900a6b4ebed5cf693f896bbcb1c926ed21af65da942b72fb582ff1c38d
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
        "updated_at": "2016-10-18T11:09:14.931Z"
      },
      "created_at": "2016-10-18T11:09:14.934Z",
      "updated_at": "2016-10-18T11:09:14.934Z",
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
        "updated_at": "2016-10-18T11:09:14.943Z"
      },
      "created_at": "2016-10-18T11:09:14.947Z",
      "updated_at": "2016-10-18T11:09:14.947Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05511d900a6b4ebed5cf693f896bbcb1c926ed21af65da942b72fb582ff1c38d"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer d7c512a8fc143079bf265c35f00822b76111301c2cdcbb3fa3bd843c03c09572
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
        "updated_at": "2016-10-18T11:09:14.713Z"
      },
      "created_at": "2016-10-18T11:09:14.718Z",
      "updated_at": "2016-10-18T11:09:14.718Z",
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
        "updated_at": "2016-10-18T11:09:14.734Z"
      },
      "created_at": "2016-10-18T11:09:14.738Z",
      "updated_at": "2016-10-18T11:09:14.738Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7c512a8fc143079bf265c35f00822b76111301c2cdcbb3fa3bd843c03c09572"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 746b8c6c6771beb1f7a555b1ad9f63172885a8034f0614a1f1329bd98b2888a2
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
      "created_at": "2016-10-18T11:09:15.846Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 18,
      "updated_at": "2016-10-18T11:09:15.962Z",
      "author_id": "649",
      "thread_subject_id": "202",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 16,
      "created_at": "2016-10-18T11:09:15.950Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 19,
      "updated_at": "2016-10-18T11:09:15.965Z",
      "author_id": "652",
      "thread_subject_id": "203",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 17,
      "created_at": "2016-10-18T11:09:16.375Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 11,
      "updated_at": "2016-10-18T11:09:16.375Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 18,
      "created_at": "2016-10-18T11:09:16.792Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 12,
      "updated_at": "2016-10-18T11:09:16.792Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 19,
      "created_at": "2016-10-18T11:09:17.214Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 13,
      "updated_at": "2016-10-18T11:09:17.214Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 20,
      "created_at": "2016-10-18T11:09:17.543Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 118,
      "updated_at": "2016-10-18T11:09:17.543Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 21,
      "created_at": "2016-10-18T11:09:17.875Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 119,
      "updated_at": "2016-10-18T11:09:17.875Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 22,
      "created_at": "2016-10-18T11:09:18.198Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 120,
      "updated_at": "2016-10-18T11:09:18.198Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 746b8c6c6771beb1f7a555b1ad9f63172885a8034f0614a1f1329bd98b2888a2"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/14
Content-Type: application/json
Authorization: Bearer e30bc43a29584e119d7c3bb11de56616c6d0bb91f2b7cc8b5bf64ef7594440d6
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-18T10:59:15.000Z"}}
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
    "id": 14,
    "created_at": "2016-10-18T11:09:15.671Z",
    "read_at": "2016-10-18T10:59:15.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 17,
    "updated_at": "2016-10-18T11:09:15.731Z",
    "author_id": "645",
    "thread_subject_id": "201",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/14" -d '{"notification":{"read_at":"2016-10-18T10:59:15.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e30bc43a29584e119d7c3bb11de56616c6d0bb91f2b7cc8b5bf64ef7594440d6"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 1c1611abb322f784a50b450c80244439969c76180f588eb46eb1bd3cb206e836
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
      "id": 7,
      "course_id": 252,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T11:09:27.789Z",
      "course_published": true,
      "updated_at": "2016-10-18T11:09:27.781Z"
    },
    {
      "id": 8,
      "course_id": 253,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-18T11:09:27.874Z",
      "course_published": true,
      "updated_at": "2016-10-18T11:09:27.866Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c1611abb322f784a50b450c80244439969c76180f588eb46eb1bd3cb206e836"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 99f2d734e15cc6af5b03775f79cfaf7569711fc9aaee2974a35954668a8e5981
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
    "course_id": 250,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-18T11:09:27.476Z",
    "course_published": true,
    "updated_at": "2016-10-18T11:09:27.469Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99f2d734e15cc6af5b03775f79cfaf7569711fc9aaee2974a35954668a8e5981"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer eb65011ea0f2bf89b66c85e21069ba61f93e3311ca4f64a6d0fcae049cf1203c
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
    "course_id": 251,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-18T11:09:27.649Z",
    "course_published": true,
    "updated_at": "2016-10-18T11:09:27.638Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb65011ea0f2bf89b66c85e21069ba61f93e3311ca4f64a6d0fcae049cf1203c"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer d0409638f615608f65ea725e6c3d42de032039339deb8b9a65f9f560eef0d082
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
      "id": 3,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 26,
      "user_id": 137
    },
    {
      "id": 4,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 27,
      "user_id": 137
    },
    {
      "id": 5,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 28,
      "user_id": 137
    },
    {
      "id": 6,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 29,
      "user_id": 137
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0409638f615608f65ea725e6c3d42de032039339deb8b9a65f9f560eef0d082"
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
        "id": 224,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 224
      },
      {
        "id": 225,
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
      "id": 225,
      "name": "Advanced dedicated service-desk",
      "name_translations": {
        "en": "Advanced dedicated service-desk"
      }
    },
    {
      "id": 226,
      "name": "Upgradable object-oriented analyzer",
      "name_translations": {
        "en": "Upgradable object-oriented analyzer"
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
PATCH /v2/feedbacks/22/close
Content-Type: application/json
Authorization: Bearer f8797a989e864f272154c673e1031b33a29404674f245430cb353aff8398d563
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
    "id": 22,
    "user_id": 448,
    "feedbackable_id": 50,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-18T11:08:58.970Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/22/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8797a989e864f272154c673e1031b33a29404674f245430cb353aff8398d563"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/43/fix
Content-Type: application/json
Authorization: Bearer 69f89ef108d10f1b47cb38394f33e1fbeef2d95260e14ec51bd599a46f035eb3
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
    "id": 43,
    "user_id": 539,
    "feedbackable_id": 52,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-18T11:09:06.497Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/43/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69f89ef108d10f1b47cb38394f33e1fbeef2d95260e14ec51bd599a46f035eb3"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer 1ddb94add064be0d493205f46e562202efb011873f2f4a06e618d4bb3a20360b
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
    "id": 19,
    "user_id": 431,
    "feedbackable_id": 47,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T11:08:58.149Z",
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
curl "api.goskive.com/v2/feedbacks/19" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ddb94add064be0d493205f46e562202efb011873f2f4a06e618d4bb3a20360b"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer 5e0db7893b03b035525bb9d6e1b5657d97cf4db9bfe2649c93c6e8db0004af7a
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
curl "api.goskive.com/v2/feedbacks/23/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5e0db7893b03b035525bb9d6e1b5657d97cf4db9bfe2649c93c6e8db0004af7a"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/45/fix
Content-Type: application/json
Authorization: Bearer e2ff2f08c908030649415a0fbd8452ff40d69fd78307c4771876bd00b7c7ca70
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
curl "api.goskive.com/v2/feedbacks/45/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2ff2f08c908030649415a0fbd8452ff40d69fd78307c4771876bd00b7c7ca70"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/46/fix
Content-Type: application/json
Authorization: Bearer 50fe358ab79b71cc08cd6647b7015172b48e461fbf0477b941c29685e198d691
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
curl "api.goskive.com/v2/feedbacks/46/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50fe358ab79b71cc08cd6647b7015172b48e461fbf0477b941c29685e198d691"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 166dc9dae1d63d14b8dc9f1f74872f0e277e01d3ad366ea83cc16bf87314441c
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
    "id": 20,
    "user_id": 436,
    "feedbackable_id": 48,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T11:08:58.441Z",
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
curl "api.goskive.com/v2/feedbacks/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 166dc9dae1d63d14b8dc9f1f74872f0e277e01d3ad366ea83cc16bf87314441c"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/3
Authorization: Bearer 6379bff9ce33b10f72d089e3690dff5b560c6c85176c3f82ea1c1cc73d4591d8
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
curl "api.goskive.com/v2/files/3" -d '' -X DELETE \
	-H "Authorization: Bearer 6379bff9ce33b10f72d089e3690dff5b560c6c85176c3f82ea1c1cc73d4591d8" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/5
Authorization: Bearer 1bb25a4a1dd9790f8786fe7eba2219d7c9075b61b7eb7a6abf9cdc45c436d9d0
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
curl "api.goskive.com/v2/files/5" -d '' -X DELETE \
	-H "Authorization: Bearer 1bb25a4a1dd9790f8786fe7eba2219d7c9075b61b7eb7a6abf9cdc45c436d9d0" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/1
Authorization: Bearer b580d130ea0eadd660176d4a1f713534dba4cc05609033f323bf2f755cafe9d3
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/7c2c0585e52e99edefecd60e691cda84.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T110816Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=36ed9fb2436a3d9bed0ff47bd8339ad30be19d2241ba01ceeb9da5e47879c821"
  }
}
```



```shell
curl "api.goskive.com/v2/files/1" -X GET \
	-H "Authorization: Bearer b580d130ea0eadd660176d4a1f713534dba4cc05609033f323bf2f755cafe9d3"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Authorization: Bearer 5fbb4f32bc568b4d9d191c8bc2652e18474505c7cf0cc6c798d9ec281a86d840
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
    "id": 7,
    "uploader": {
      "id": 18,
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
      "created_at": "2016-10-18T11:08:17.435Z",
      "updated_at": "2016-10-18T11:08:17.435Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-18T11:08:17.505Z",
    "updated_at": "2016-10-18T11:08:17.505Z",
    "course_id": 7,
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
	-H "Authorization: Bearer 5fbb4f32bc568b4d9d191c8bc2652e18474505c7cf0cc6c798d9ec281a86d840" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/12/matched_courses?required_cu_count=2
Authorization: Bearer 251f0b2728473002234167adaae2c7942a311f8e57924ee355f0adb7d6422ed8
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
      "creator_id": 943,
      "id": 304,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 289,
      "additional_university_ids": [

      ],
      "topic_id": 311,
      "discipline_id": 312,
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
      "chapters_updated_at": "2016-10-18T11:09:34.673Z",
      "updated_at": "2016-10-18T11:09:36.330Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 948,
      "id": 305,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-cc8e43fd-53f5-452e-9ce2-da11299172de",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-cc8e43fd-53f5-452e-9ce2-da11299172de",
      "slug": "mit-the-great-british-bake-off-cc8e43fd-53f5-452e-9ce2-da11299172de",
      "university_id": 290,
      "additional_university_ids": [

      ],
      "topic_id": 312,
      "discipline_id": 313,
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
      "chapters_updated_at": "2016-10-18T11:09:34.673Z",
      "updated_at": "2016-10-18T11:09:36.910Z",
      "shortname": "mit-the-great-british-bake-off-cc8e43fd-53f5-452e-9ce2-da11299172de"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/12/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 251f0b2728473002234167adaae2c7942a311f8e57924ee355f0adb7d6422ed8"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/2/preview
Authorization: Bearer a69d03a7edf3da7cff0f9680b4b5a3a23952f2f77720e9b1d64b6afe811534f8
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/0853b7b6af1fd799f8c2ebc05ba5ef4e.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161018%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161018T110816Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=4b47aed408db5490ee737245e5d38ddc9c80aee17037ec7a69ee528c96c6f7d1"
  }
}
```



```shell
curl "api.goskive.com/v2/files/2/preview" -X GET \
	-H "Authorization: Bearer a69d03a7edf3da7cff0f9680b4b5a3a23952f2f77720e9b1d64b6afe811534f8"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/6/report
Authorization: Bearer c3e0e933886876cfe85beb542676312fe26a68753c0db7ad4fcebc1d273c4be4
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
curl "api.goskive.com/v2/files/6/report" -d '' -X PUT \
	-H "Authorization: Bearer c3e0e933886876cfe85beb542676312fe26a68753c0db7ad4fcebc1d273c4be4" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/10/comments
Content-Type: application/json
Authorization: Bearer 26a5e2515601d21b777cdde81c854d8bf746581b00779d75b82245e56c864cd3
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
    "id": 3,
    "author_id": 190,
    "reply_to_id": null,
    "created_at": "2016-10-18T11:08:33.832Z",
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
curl "api.goskive.com/v2/flashcards/10/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26a5e2515601d21b777cdde81c854d8bf746581b00779d75b82245e56c864cd3"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/11/comments
Content-Type: application/json
Authorization: Bearer 53937a7f213a93fd5d42d685b24a9cbf7132ce3f5f3a9a64a841d3c9f9f428ed
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
    "author_id": 193,
    "reply_to_id": null,
    "created_at": "2016-10-18T11:08:34.155Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 193,
      "feedbackable_id": 11,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:34.150Z",
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
	-H "Authorization: Bearer 53937a7f213a93fd5d42d685b24a9cbf7132ce3f5f3a9a64a841d3c9f9f428ed"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/12/comments
Content-Type: application/json
Authorization: Bearer 8263edd352dd4a307b49a4dc8d83d87a62792094fdd5f5e03839c25d2042013f
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
      "id": 5,
      "author_id": 199,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:08:34.447Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 200,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:08:34.463Z",
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
curl "api.goskive.com/v2/flashcards/12/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8263edd352dd4a307b49a4dc8d83d87a62792094fdd5f5e03839c25d2042013f"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/9/comments
Content-Type: application/json
Authorization: Bearer a46b0e9ed91a7afed5e71b8128f1f9eb99632bdece3d57f9d1f73fa791529e79
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
curl "api.goskive.com/v2/flashcards/9/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a46b0e9ed91a7afed5e71b8128f1f9eb99632bdece3d57f9d1f73fa791529e79"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/2/feedbacks
Content-Type: application/json
Authorization: Bearer d50265900070eb8cc930c6c1bf0affd4152e761980aa808617da2ea21e0fcf32
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
    "id": 2,
    "user_id": 24,
    "feedbackable_id": 2,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-18T11:08:18.446Z",
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
curl "api.goskive.com/v2/flashcards/2/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d50265900070eb8cc930c6c1bf0affd4152e761980aa808617da2ea21e0fcf32"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/5/feedbacks
Content-Type: application/json
Authorization: Bearer 983971a8676499da88907b9e9e5e04096cf7787340823839919008e36ffc0e21
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
      "user_id": 45,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:19.240Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 44,
      "feedbackable_id": 5,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:19.228Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 983971a8676499da88907b9e9e5e04096cf7787340823839919008e36ffc0e21"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/61/votes
Content-Type: application/json
Authorization: Bearer 9ce194be107e877da94953969abc9c878d9698fa8fc77ae3e6314d82b9c7059d
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
      "votable_id": 61,
      "user_id": 617
    },
    {
      "id": 9,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 61,
      "user_id": 616
    },
    {
      "id": 8,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 61,
      "user_id": 615
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/61/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ce194be107e877da94953969abc9c878d9698fa8fc77ae3e6314d82b9c7059d"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/64/republish
Content-Type: application/json
Authorization: Bearer 9db432bafe968bd138b2a3726ab351c376044d5fa1ff0fb63d7de8deba18a48e
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
	-H "Authorization: Bearer 9db432bafe968bd138b2a3726ab351c376044d5fa1ff0fb63d7de8deba18a48e"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/86/bookmark
Content-Type: application/json
Authorization: Bearer 65147d5c226e52d582e54883934ea961f46e2fe66225df7e8eebc44516250cea
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
	-H "Authorization: Bearer 65147d5c226e52d582e54883934ea961f46e2fe66225df7e8eebc44516250cea"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/85
Content-Type: application/json
Authorization: Bearer f569b63ad66b8b78618450595ddf9a6ec136f025fb89b13c019a08e8211fb74f
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/85" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f569b63ad66b8b78618450595ddf9a6ec136f025fb89b13c019a08e8211fb74f"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/84/downvote
Content-Type: application/json
Authorization: Bearer 95285ded3665948fe83f397612a8240b2b5bd22f5b3967c1684c19fa0ed2b41f
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
	-H "Authorization: Bearer 95285ded3665948fe83f397612a8240b2b5bd22f5b3967c1684c19fa0ed2b41f"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/63
Content-Type: application/json
Authorization: Bearer ee832ac2a8ef2b5b971136bef901134ad086ea73e30c7da18d9e454489179795
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
    "id": 63,
    "obfuscated_id": "k3ebr8XrqxE",
    "author_id": 705,
    "chapter_id": 158,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:09:20.699Z",
    "created_at": "2016-10-18T11:09:20.699Z",
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
curl "api.goskive.com/v2/flashcards/63" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ee832ac2a8ef2b5b971136bef901134ad086ea73e30c7da18d9e454489179795"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/66/report
Content-Type: application/json
Authorization: Bearer 0be5d80cef54ad67c9e8101a9306d48a35eda484d0ce4d24372506d219db97f8
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0be5d80cef54ad67c9e8101a9306d48a35eda484d0ce4d24372506d219db97f8"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/83/bookmark
Content-Type: application/json
Authorization: Bearer 935e55a39e836fe04b9f0fceaabc9e88e864898f417f58619383c749b4ff16df
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
	-H "Authorization: Bearer 935e55a39e836fe04b9f0fceaabc9e88e864898f417f58619383c749b4ff16df"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/67/upvote
Content-Type: application/json
Authorization: Bearer b2f527bf0bde218f6587b16fc3e76f54a3159b3a8b65e1bb7eece09f53b6affb
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/67/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2f527bf0bde218f6587b16fc3e76f54a3159b3a8b65e1bb7eece09f53b6affb"
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
    "key": "cache/667fca749cd179d16f7a9904edd294af.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOFQxMjowOTowN1oiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS82NjdmY2E3NDljZDE3OWQxNmY3YTk5MDRlZGQyOTRhZi5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE4L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOFQxMTA5MDdaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161018/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161018T110907Z",
    "x-amz-signature": "8e4202cac32bb9e42c61a15109b8ecdf65cb80b097af601ec24bf8731d83a574"
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
Authorization: Bearer 01d359f4d367e01d3bf847ee53d11af82738b66c24d83082d1e756c950a836a3
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
	-H "Authorization: Bearer 01d359f4d367e01d3bf847ee53d11af82738b66c24d83082d1e756c950a836a3"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer fabed7eefe7a92831550cb7ff15a6ba01d1f89327d517bdab72ce0b471ebfa39
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
	-H "Authorization: Bearer fabed7eefe7a92831550cb7ff15a6ba01d1f89327d517bdab72ce0b471ebfa39"
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
{"password":{"reset_password_token":"DLNUfH4NC8DG8g-Cz3xX","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 566,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-18T11:09:09.411Z",
  "updated_at": "2016-10-18T11:09:09.581Z",
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
  "audit_id": 4348
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"DLNUfH4NC8DG8g-Cz3xX","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/58/comments
Content-Type: application/json
Authorization: Bearer 509ace4153d55be3c273e3bb2e195a222430b8f0095cf4694a6a6e94e728ceab
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
    "id": 11,
    "author_id": 355,
    "reply_to_id": null,
    "created_at": "2016-10-18T11:08:46.692Z",
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
curl "api.goskive.com/v2/questions/58/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 509ace4153d55be3c273e3bb2e195a222430b8f0095cf4694a6a6e94e728ceab"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/59/comments
Content-Type: application/json
Authorization: Bearer 8aeb57ed668f35436b55d1b8774e30ae2dbfb2987e71274ba30d388ebdb180e8
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
    "id": 12,
    "author_id": 358,
    "reply_to_id": null,
    "created_at": "2016-10-18T11:08:47.240Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 18,
      "user_id": 358,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:47.236Z",
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
curl "api.goskive.com/v2/questions/59/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8aeb57ed668f35436b55d1b8774e30ae2dbfb2987e71274ba30d388ebdb180e8"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/56/comments
Content-Type: application/json
Authorization: Bearer 806e4fa583284d997c2317da6a6e9f4a55893928e2ad9025bae9c93ffaf79867
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
      "id": 10,
      "author_id": 351,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:08:45.988Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 350,
      "reply_to_id": null,
      "created_at": "2016-10-18T11:08:45.971Z",
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
curl "api.goskive.com/v2/questions/56/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 806e4fa583284d997c2317da6a6e9f4a55893928e2ad9025bae9c93ffaf79867"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/57/comments
Content-Type: application/json
Authorization: Bearer 0742657d09d976e29f23f5c070c3b8630425041fcde5ca55dbeccff998639d2f
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
curl "api.goskive.com/v2/questions/57/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0742657d09d976e29f23f5c070c3b8630425041fcde5ca55dbeccff998639d2f"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/50/feedbacks
Content-Type: application/json
Authorization: Bearer 851707b71e68f7399294619b4c97e795e323f9ca5cac33374da9a92fe2d2703d
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
    "id": 16,
    "user_id": 284,
    "feedbackable_id": 50,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-18T11:08:41.725Z",
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
curl "api.goskive.com/v2/questions/50/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 851707b71e68f7399294619b4c97e795e323f9ca5cac33374da9a92fe2d2703d"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/46/feedbacks
Content-Type: application/json
Authorization: Bearer 736fc2b4206fb3c8b839faa4a9a3928be8fb04c4abe21b18c4c6fe2c2537ee35
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
      "id": 13,
      "user_id": 266,
      "feedbackable_id": 46,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:40.304Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 265,
      "feedbackable_id": 46,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-18T11:08:40.293Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/46/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 736fc2b4206fb3c8b839faa4a9a3928be8fb04c4abe21b18c4c6fe2c2537ee35"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/123/votes
Content-Type: application/json
Authorization: Bearer b47e2875856cf33edb7b664deb2e58f504edea9879f2542d7d21604a8a03ea6b
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
      "id": 19,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 797
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 796
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 123,
      "user_id": 795
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/123/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b47e2875856cf33edb7b664deb2e58f504edea9879f2542d7d21604a8a03ea6b"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/10/republish
Content-Type: application/json
Authorization: Bearer f1b99159e711086a9e8a8aac8d773acbbd8e9abcbc061346ef7b9b6244b4a6fc
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
curl "api.goskive.com/v2/questions/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1b99159e711086a9e8a8aac8d773acbbd8e9abcbc061346ef7b9b6244b4a6fc"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/3/bookmark
Content-Type: application/json
Authorization: Bearer 7733c69f65db52ea7031f225d45c128d88e2aea48698b3d6dd19305846127d4e
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/3/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7733c69f65db52ea7031f225d45c128d88e2aea48698b3d6dd19305846127d4e"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/5
Content-Type: application/json
Authorization: Bearer d34b25f12752e904e0d822cf7428ab539d561362d901f9bf085dcf5d57843d77
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d34b25f12752e904e0d822cf7428ab539d561362d901f9bf085dcf5d57843d77"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/7/downvote
Content-Type: application/json
Authorization: Bearer b326151bc085a9f22ecf6588d9b567c05d7736faed450f815c3c6256c51c1f8a
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/7/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b326151bc085a9f22ecf6588d9b567c05d7736faed450f815c3c6256c51c1f8a"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/6
Content-Type: application/json
Authorization: Bearer 1a3eca97e636accb86887b88e0584c29d30e7bbe5aada821a7a508c128db1ac3
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
    "id": 6,
    "obfuscated_id": "eyxYPTvoIb8",
    "author_id": 72,
    "chapter_id": 14,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:22.384Z",
    "created_at": "2016-10-18T11:08:22.256Z",
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
        "id": 12,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 13,
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
curl "api.goskive.com/v2/questions/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a3eca97e636accb86887b88e0584c29d30e7bbe5aada821a7a508c128db1ac3"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/1/report
Content-Type: application/json
Authorization: Bearer c7df6f4cbe5833663567834c71b0764bfe32e1143e3cd73d230bf7bf0d36b9a7
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/1/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7df6f4cbe5833663567834c71b0764bfe32e1143e3cd73d230bf7bf0d36b9a7"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/4/bookmark
Content-Type: application/json
Authorization: Bearer d2ecf06294097c388ed79122c62d1133cae403f925b7ecbfdeced7cf399466db
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/4/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2ecf06294097c388ed79122c62d1133cae403f925b7ecbfdeced7cf399466db"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/2
Content-Type: application/json
Authorization: Bearer daea1fe7981890ef8f8156f4a05abb5a49dcd2362f78046f487d27487be1e87c
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":2,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T11:08:20.543Z","updated_at":"2016-10-18T11:08:20.658Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":10,"author_id":60,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 2,
    "obfuscated_id": "yHhUU9c1C7Y",
    "author_id": 60,
    "chapter_id": 10,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-18T11:08:20.767Z",
    "created_at": "2016-10-18T11:08:20.543Z",
    "tags": [
      {
        "id": 4,
        "name": "expert",
        "taggings_count": 1
      },
      {
        "id": 3,
        "name": "hard",
        "taggings_count": 1
      }
    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "{\"id\"=>2, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-18T11:08:20.543Z\", \"updated_at\"=>\"2016-10-18T11:08:20.658Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>10, \"author_id\"=>60, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 3,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 4,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 5,
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
curl "api.goskive.com/v2/questions/2" -d '{"question":{"question":{"id":2,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-18T11:08:20.543Z","updated_at":"2016-10-18T11:08:20.658Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":10,"author_id":60,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daea1fe7981890ef8f8156f4a05abb5a49dcd2362f78046f487d27487be1e87c"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/8/upvote
Content-Type: application/json
Authorization: Bearer b38765d551701db64e0a6a2d9932b11ce64c3c9e4ec006791d3f0e0f9746e7c9
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/8/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b38765d551701db64e0a6a2d9932b11ce64c3c9e4ec006791d3f0e0f9746e7c9"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6d85c5de2ce204fe24f6d3914bd2f0e67782cebc357282d2d90ab7ae18c51387
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
      "creator_id": 205,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 62,
      "discipline_id": 62,
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
      "updated_at": "2016-10-18T11:08:34.818Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d85c5de2ce204fe24f6d3914bd2f0e67782cebc357282d2d90ab7ae18c51387"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 7ca050f089fa387a2c44482630aae1b9c210b9e1a1cffb9b89a89d98cb5b1e1b
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
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-63",
      "html_url": "https://goskive.com/university/uni-63",
      "slug": "uni-63",
      "name": "National School of Pizza",
      "short_name": "Uni 63",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f0455cb406a50dfa205f9dfc8a84dec6ed607634.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ee88380d46739e088ac23d7ad0ef1eb91c7c5fb1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T11:08:35.078Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-62",
      "html_url": "https://goskive.com/university/uni-62",
      "slug": "uni-62",
      "name": "National School of Pastry",
      "short_name": "Uni 62",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/123583053f30d60d57698c0742b45baeaaeea45e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/467253d3f01c670a10060a75442205258e791570.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T11:08:35.061Z",
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
	-H "Authorization: Bearer 7ca050f089fa387a2c44482630aae1b9c210b9e1a1cffb9b89a89d98cb5b1e1b"
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
      "id": 133,
      "name": "Streamlined needs-based hierarchy",
      "name_translations": {
        "en": "Streamlined needs-based hierarchy"
      },
      "discipline_id": 133
    },
    {
      "id": 134,
      "name": "Reduced 4th generation functionalities",
      "name_translations": {
        "en": "Reduced 4th generation functionalities"
      },
      "discipline_id": 134
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
GET /v2/topics/135
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
    "id": 135,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 135
  }
}
```



```shell
curl "api.goskive.com/v2/topics/135" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 4acc8cea4da3c9ab65c3309d66bbeddd2329ea413f334e039ab627896bf4cf6a
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
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-207",
      "html_url": "https://goskive.com/university/uni-207",
      "slug": "uni-207",
      "name": "University 147",
      "short_name": "Uni 207",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d4a93c927995b518f0ed147705cc1adcbcba7302.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c601cc4c49af77397e019500f54613c65ddac27e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T11:09:25.086Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-208",
      "html_url": "https://goskive.com/university/uni-208",
      "slug": "uni-208",
      "name": "University 148",
      "short_name": "Uni 208",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f6443463c59d71641e860ea19b1f98a2fa74ab2f.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/58229f866b1f2595a180c2552c3660ba91209b11.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T11:09:25.104Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-209",
      "html_url": "https://goskive.com/university/uni-209",
      "slug": "uni-209",
      "name": "University 149",
      "short_name": "Uni 209",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3a5cfcda6927c38a5f855943a8a66eeef6616188.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c0bde4774cc0523fbdfa23f0a4e671be0fbfe4c0.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-18T11:09:25.121Z",
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
	-H "Authorization: Bearer 4acc8cea4da3c9ab65c3309d66bbeddd2329ea413f334e039ab627896bf4cf6a"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 17063dd6a2ddd24b28897c7744972c5fc7c3b24804496d1daf73581fe6028743
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
    "id": 226,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/8845f9dd62b4591fcf4eee8e4da13bb47f55ee9a.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/d2e0e3fabe19bda9a917a5eb9f64113cd317619e.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-18T11:09:25.027Z",
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
	-H "Authorization: Bearer 17063dd6a2ddd24b28897c7744972c5fc7c3b24804496d1daf73581fe6028743"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 619c050fbffcd8645df749698aed8b558901fd703d05d83cd7cf06a1e35ca55e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":66,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 210,
    "id": 64,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 66,
    "additional_university_ids": [

    ],
    "topic_id": 66,
    "discipline_id": 66,
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
    "chapters_updated_at": "2016-10-18T11:08:35.303Z",
    "updated_at": "2016-10-18T11:08:35.433Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 52,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-18T11:08:35.392Z",
        "course_id": 64,
        "author_id": 210,
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
        "id": 53,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-18T11:08:35.408Z",
        "course_id": 64,
        "author_id": 210,
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
        "id": 54,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-18T11:08:35.424Z",
        "course_id": 64,
        "author_id": 210,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":66,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 619c050fbffcd8645df749698aed8b558901fd703d05d83cd7cf06a1e35ca55e"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 83828d5ed4a1fbf3d20d6224b6403dac70159c5e94eb9cd8a8ef195729cd4ba1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":65,"published":false}}
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
    "creator_id": 209,
    "id": 63,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 65,
    "additional_university_ids": [

    ],
    "topic_id": 65,
    "discipline_id": 65,
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
    "updated_at": "2016-10-18T11:08:35.259Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":65,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83828d5ed4a1fbf3d20d6224b6403dac70159c5e94eb9cd8a8ef195729cd4ba1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 611c0cdae5b6a807fed3ec95bf3d52c47b8fc4f0b45da29a618643b944f932c4
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
      "creator_id": 228,
      "id": 81,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-67",
      "html_url": "https://goskive.com/course/fu-course-67",
      "slug": "fu-course-67",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "topic_id": 83,
      "discipline_id": 83,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
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
      "updated_at": "2016-10-18T11:08:37.020Z",
      "shortname": "fu-course-67"
    },
    {
      "creator_id": 228,
      "id": 82,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-68",
      "html_url": "https://goskive.com/course/fu-course-68",
      "slug": "fu-course-68",
      "university_id": 74,
      "additional_university_ids": [

      ],
      "topic_id": 84,
      "discipline_id": 84,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
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
      "chapters_updated_at": "2016-10-18T11:08:37.309Z",
      "updated_at": "2016-10-18T11:08:37.316Z",
      "shortname": "fu-course-68"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 611c0cdae5b6a807fed3ec95bf3d52c47b8fc4f0b45da29a618643b944f932c4"
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
      "creator_id": 238,
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-75",
      "html_url": "https://goskive.com/course/fu-course-75",
      "slug": "fu-course-75",
      "university_id": 77,
      "additional_university_ids": [

      ],
      "topic_id": 91,
      "discipline_id": 91,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 75",
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
      "updated_at": "2016-10-18T11:08:37.874Z",
      "shortname": "fu-course-75"
    },
    {
      "creator_id": 238,
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-76",
      "html_url": "https://goskive.com/course/fu-course-76",
      "slug": "fu-course-76",
      "university_id": 77,
      "additional_university_ids": [

      ],
      "topic_id": 92,
      "discipline_id": 92,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 76",
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
      "chapters_updated_at": "2016-10-18T11:08:38.167Z",
      "updated_at": "2016-10-18T11:08:38.174Z",
      "shortname": "fu-course-76"
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
Authorization: Bearer 761885d0f5035cf2c929b1a330a88b52bf4415c9db9c9755f56868ec90fd1089
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
      "creator_id": 235,
      "id": 85,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-71",
      "html_url": "https://goskive.com/course/fu-course-71",
      "slug": "fu-course-71",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "topic_id": 87,
      "discipline_id": 87,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 71",
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
      "updated_at": "2016-10-18T11:08:37.591Z",
      "shortname": "fu-course-71"
    },
    {
      "creator_id": 235,
      "id": 86,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-72",
      "html_url": "https://goskive.com/course/fu-course-72",
      "slug": "fu-course-72",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "topic_id": 88,
      "discipline_id": 88,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 72",
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
      "updated_at": "2016-10-18T11:08:37.632Z",
      "shortname": "fu-course-72"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 761885d0f5035cf2c929b1a330a88b52bf4415c9db9c9755f56868ec90fd1089"
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
      "creator_id": 243,
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-79",
      "html_url": "https://goskive.com/course/fu-course-79",
      "slug": "fu-course-79",
      "university_id": 78,
      "additional_university_ids": [

      ],
      "topic_id": 95,
      "discipline_id": 95,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 79",
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
      "updated_at": "2016-10-18T11:08:38.369Z",
      "shortname": "fu-course-79"
    },
    {
      "creator_id": 243,
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-80",
      "html_url": "https://goskive.com/course/fu-course-80",
      "slug": "fu-course-80",
      "university_id": 78,
      "additional_university_ids": [

      ],
      "topic_id": 96,
      "discipline_id": 96,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 80",
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
      "updated_at": "2016-10-18T11:08:38.408Z",
      "shortname": "fu-course-80"
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
Authorization: Bearer dbe3846e6d8ee48df3117151ac4c504153b406ba82090a1ca4a53c42e09528b5
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
  "id": 608,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-18T11:09:12.622Z",
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
	-H "Authorization: Bearer dbe3846e6d8ee48df3117151ac4c504153b406ba82090a1ca4a53c42e09528b5"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/153
Content-Type: application/json
Authorization: Bearer b5722a5865a2bdc45a1891613a32e9db4e1b951107d7942f503037cfac9b7d03
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
    "id": 153,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 45,
    "fields_of_study": [
      45,
      46
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-18T11:08:30.071Z",
    "updated_at": "2016-10-18T11:08:30.071Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/153" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b5722a5865a2bdc45a1891613a32e9db4e1b951107d7942f503037cfac9b7d03"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/151
Content-Type: application/json
Authorization: Bearer 280c1f7d34c77370df615c1139557210fdd9387e14874bc89d639758ba561023
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
    "id": 151,
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
    "created_at": "2016-10-18T11:08:29.922Z",
    "updated_at": "2016-10-18T11:08:29.922Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/151" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 280c1f7d34c77370df615c1139557210fdd9387e14874bc89d639758ba561023"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/21
Content-Type: application/json
Authorization: Bearer cbbcab2ea7ead58950a81dd7f6bf4d3566956cc1dad7935e9e4d98140920c932
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
	-H "Authorization: Bearer cbbcab2ea7ead58950a81dd7f6bf4d3566956cc1dad7935e9e4d98140920c932"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/20
Content-Type: application/json
Authorization: Bearer fbed2a579611b93385f6c0a1ffc1786972e06f9be75ead1011b0fd03e607c4a9
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
    "id": 20,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 124,
    "user_id": 819
  }
}
```



```shell
curl "api.goskive.com/v2/votes/20" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbed2a579611b93385f6c0a1ffc1786972e06f9be75ead1011b0fd03e607c4a9"
```
