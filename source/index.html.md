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
Authorization: Basic OTg4MjU5NTU0OWRhNjcwODRiYTYwMzBjMjQ2NTQ0NDk2ZjM5OWZkNWNhODcz
YzM5OTI4ZGVlZTkzMGM2MzQ0ODo1ZGE5YzRiOWI3MjBhNjViZWMzYzBlNTA5
YjAwOGYyYzk2OGQ1NjViZjJhZTNkNDkwYzdlNDI4Yjc4MzVhZmNm

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
	-u 9882595549da67084ba6030c246544496f399fd5ca873c39928deee930c63448:5da9c4b9b720a65bec3c0e509b008f2c968d565bf2ae3d490c7e428b7835afcf
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"45a77b2b96b214add81b85ce9d5117cde214382202fb91da78d8df535b38788e","client_secret":"8349dc6c3ea1dc3a89cd063e9317ccd23459940267bdcb8a835d1dca24e20288"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"45a77b2b96b214add81b85ce9d5117cde214382202fb91da78d8df535b38788e","client_secret":"8349dc6c3ea1dc3a89cd063e9317ccd23459940267bdcb8a835d1dca24e20288"}' -X POST \
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
Authorization: Basic MjY3ODJlOWUyYzQwMjUzMzE2OTVmMjZjMTE1MGYyYjkwNzlmZmFjZTYwZjlj
Y2MyZTc1NWEzYjE0MDA2YThmZToyZGFmYWVhYjVjMGY5ZDY1MmI2YThjMDVj
ODQ2MzNiMGQ1MmFkNGZkMDFlZDE2MTdlNWEzMDkzNWNkZjEzYTkx

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
  "access_token": "9f49276c9d0cac696b49a51335f7412e498a446769603dfde7aab0c77f785fea",
  "token_type": "bearer",
  "created_at": 1477389814
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 26782e9e2c4025331695f26c1150f2b9079fface60f9ccc2e755a3b14006a8fe:2dafaeab5c0f9d652b6a8c05c84633b0d52ad4fd01ed1617e5a30935cdf13a91
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7db7d5a61b866a61efd8f51484d85053869599d3bcfa64c4667a79e8007d9a44","client_secret":"9b8144cc9c6da2f474620a534f016c95a1c0d56a977652b986fde98ea98f442f"}
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
  "access_token": "167260773cdd454613638ab17515d19f8a6ec756e06f5cf78f125d5580bf88ec",
  "token_type": "bearer",
  "created_at": 1477389814
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"7db7d5a61b866a61efd8f51484d85053869599d3bcfa64c4667a79e8007d9a44","client_secret":"9b8144cc9c6da2f474620a534f016c95a1c0d56a977652b986fde98ea98f442f"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"d13c8ec64e24cca490488d39df8e925efe5bca8071c55c9300ded6ffd21b30c1","client_secret":"4b3afca8965f5ace353de9538d54756d0e2644ccaa1cd3271c383df7de0cd84e"}
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
  "access_token": "db1591b64c693d15142bbd01110f39bbb3efecb82430edea3c16c4b95c0522c7",
  "token_type": "bearer",
  "created_at": 1477389814
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"d13c8ec64e24cca490488d39df8e925efe5bca8071c55c9300ded6ffd21b30c1","client_secret":"4b3afca8965f5ace353de9538d54756d0e2644ccaa1cd3271c383df7de0cd84e"}' -X POST \
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
Authorization: Bearer bf62ba4205fbe2bfe7d53fac4be3e3033cba484cd4420d17c7b646071b415ce0
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
	-H "Authorization: Bearer bf62ba4205fbe2bfe7d53fac4be3e3033cba484cd4420d17c7b646071b415ce0"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/18/flashcards
Content-Type: application/json
Authorization: Bearer f1ad5309b9059bcd963eb0d025fe4c43fd70bde5e71d1d8bb1779919d332c7ff
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":18,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 8,
    "obfuscated_id": "X2B_8FVuFe8",
    "author_id": 114,
    "chapter_id": 18,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:03:37.449Z",
    "created_at": "2016-10-25T10:03:37.449Z",
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
curl "api.goskive.com/v2/chapters/18/flashcards" -d '{"flashcard":{"chapter_id":18,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1ad5309b9059bcd963eb0d025fe4c43fd70bde5e71d1d8bb1779919d332c7ff"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/19/flashcards
Content-Type: application/json
Authorization: Bearer 0de36e1ff333dc1c3150e2847041f3e27264f5cd0cd099afa6a6cef3f7d2bb92
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
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 115,
      "chapter_id": 19,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:37.614Z",
      "created_at": "2016-10-25T10:03:37.614Z",
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
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 115,
      "chapter_id": 19,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:37.655Z",
      "created_at": "2016-10-25T10:03:37.655Z",
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 115,
      "chapter_id": 19,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:03:37.695Z",
      "created_at": "2016-10-25T10:03:37.695Z",
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
curl "api.goskive.com/v2/chapters/19/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0de36e1ff333dc1c3150e2847041f3e27264f5cd0cd099afa6a6cef3f7d2bb92"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/186/questions
Content-Type: application/json
Authorization: Bearer 9cac95d73452ea5a1d4a8e5da831fb4eeccaffaeb7cdf84716712c2a81f1c307
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":186,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 124,
    "obfuscated_id": "TD9SVjPLZ0Q",
    "author_id": 900,
    "chapter_id": 186,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:04:47.880Z",
    "created_at": "2016-10-25T10:04:47.880Z",
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
        "id": 249,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 250,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 251,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 252,
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
curl "api.goskive.com/v2/chapters/186/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":186,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cac95d73452ea5a1d4a8e5da831fb4eeccaffaeb7cdf84716712c2a81f1c307"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/184/questions
Content-Type: application/json
Authorization: Bearer e35c1610deef9397c64a38ef536278ab182cfebbee9656b06f4276057cc57a6f
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 122,
    "obfuscated_id": "cMWZX2w28hY",
    "author_id": 894,
    "chapter_id": 184,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:04:47.100Z",
    "created_at": "2016-10-25T10:04:47.100Z",
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
        "id": 244,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 245,
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
curl "api.goskive.com/v2/chapters/184/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":184,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e35c1610deef9397c64a38ef536278ab182cfebbee9656b06f4276057cc57a6f"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/187/questions
Content-Type: application/json
Authorization: Bearer 352870cd1f5f307593a8107c4d843f1ab05f16852e29716ddad332844a836636
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":187,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 125,
    "obfuscated_id": "K6zw0Yc6Me8",
    "author_id": 903,
    "chapter_id": 187,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:04:48.391Z",
    "created_at": "2016-10-25T10:04:48.391Z",
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
        "id": 253,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 254,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/187/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":187,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 352870cd1f5f307593a8107c4d843f1ab05f16852e29716ddad332844a836636"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/185/questions
Content-Type: application/json
Authorization: Bearer f6be43a7e5572c7032d47edaff3785d69d29d2e359e6198a5dd2318c1feb733e
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":185,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 123,
    "obfuscated_id": "N9-wuAhut60",
    "author_id": 897,
    "chapter_id": 185,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:04:47.455Z",
    "created_at": "2016-10-25T10:04:47.455Z",
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
        "id": 246,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 247,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 248,
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
curl "api.goskive.com/v2/chapters/185/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":185,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6be43a7e5572c7032d47edaff3785d69d29d2e359e6198a5dd2318c1feb733e"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/188/questions
Content-Type: application/json
Authorization: Bearer 8f5bbe593042527499476c6e6c99248daf3aa0bc358f99569960e4470e8597ef
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
      "id": 126,
      "obfuscated_id": "fKTMLttUR-w",
      "author_id": 906,
      "chapter_id": 188,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:48.848Z",
      "created_at": "2016-10-25T10:04:48.719Z",
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
    },
    {
      "id": 127,
      "obfuscated_id": "E3yfRgAzssw",
      "author_id": 907,
      "chapter_id": 188,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:49.052Z",
      "created_at": "2016-10-25T10:04:48.925Z",
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
          "id": 257,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 258,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 128,
      "obfuscated_id": "Q4ODZIcqv0E",
      "author_id": 908,
      "chapter_id": 188,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T10:04:49.254Z",
      "created_at": "2016-10-25T10:04:49.128Z",
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
          "id": 259,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 260,
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
curl "api.goskive.com/v2/chapters/188/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f5bbe593042527499476c6e6c99248daf3aa0bc358f99569960e4470e8597ef"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 5e13f935a04d1adfc81780b65e3c072dd8b851004b9f362878f06ed715e17bac
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
	-H "Authorization: Bearer 5e13f935a04d1adfc81780b65e3c072dd8b851004b9f362878f06ed715e17bac"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 05857544f3089c6d29b46b71ca0aaf1760dcbd27f869930e1decd0591a56abf1
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
	-H "Authorization: Bearer 05857544f3089c6d29b46b71ca0aaf1760dcbd27f869930e1decd0591a56abf1"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/4
Content-Type: application/json
Authorization: Bearer db86367f61f88aa065d8e618e136162f1a454ef5cafa7b9f2ad0ad42029a20d2
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
curl "api.goskive.com/v2/chapters/4" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db86367f61f88aa065d8e618e136162f1a454ef5cafa7b9f2ad0ad42029a20d2"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/8
Content-Type: application/json
Authorization: Bearer 2b5d5c87eb4f4d37bfffd8e67e73384bb1c60c6e094abeda66fa6b5ab3461c69
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b5d5c87eb4f4d37bfffd8e67e73384bb1c60c6e094abeda66fa6b5ab3461c69"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/2
Content-Type: application/json
Authorization: Bearer c7e005c135d9da0fa5ec22a9e8b3f88cc5d03bd39036bc0920e9dd1c022d8ef2
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
    "updated_at": "2016-10-25T10:03:29.333Z",
    "course_id": 7,
    "author_id": 20,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-25T10:03:28.742Z",
    "questions_updated_at": "2016-10-25T10:03:28.742Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 24,
        "chapter_id": 2,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:29.312Z",
        "created_at": "2016-10-25T10:03:29.312Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 22,
        "chapter_id": 2,
        "position": 4,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:29.189Z",
        "created_at": "2016-10-25T10:03:29.063Z",
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
            "id": 7,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 8,
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
	-H "Authorization: Bearer c7e005c135d9da0fa5ec22a9e8b3f88cc5d03bd39036bc0920e9dd1c022d8ef2"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/5
Content-Type: application/json
Authorization: Bearer 4959a5c8f53cb93fe99ca6e25809e44e00638d9203af0e7bdde8c3e72b9810b2
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
    "id": 5,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-25T10:03:29.927Z",
    "course_id": 10,
    "author_id": 33,
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
curl "api.goskive.com/v2/chapters/5" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4959a5c8f53cb93fe99ca6e25809e44e00638d9203af0e7bdde8c3e72b9810b2"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/6/replies
Content-Type: application/json
Authorization: Bearer b0a41c653087e5fa5537dcb24d4476aaabf2e201739f229ae71f2ad2c9903cdb
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
    "id": 7,
    "author_id": 305,
    "reply_to_id": 6,
    "created_at": "2016-10-25T10:03:58.624Z",
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
curl "api.goskive.com/v2/comments/6/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0a41c653087e5fa5537dcb24d4476aaabf2e201739f229ae71f2ad2c9903cdb"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/5/replies
Content-Type: application/json
Authorization: Bearer 34f2ac2cc55738640cb4de7ace1d51a5240446d642298b9df712b1de3cf553d4
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
curl "api.goskive.com/v2/comments/5/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34f2ac2cc55738640cb4de7ace1d51a5240446d642298b9df712b1de3cf553d4"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer 28e146fd9c596f30b992dba36d521058306512b2f2f28aada110535497ad394d
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
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28e146fd9c596f30b992dba36d521058306512b2f2f28aada110535497ad394d"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/53/republish
Content-Type: application/json
Authorization: Bearer cd6e9de03680a62aec19a52ccd06b1b496bb03b1cb189bfe0ee3b0ebd990eb0c
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
curl "api.goskive.com/v2/comments/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd6e9de03680a62aec19a52ccd06b1b496bb03b1cb189bfe0ee3b0ebd990eb0c"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/54
Content-Type: application/json
Authorization: Bearer fe7856097fbc856fc1e0a25f94bd9ab6045d4e1c0468a8d587fff09b034d936f
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/54" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe7856097fbc856fc1e0a25f94bd9ab6045d4e1c0468a8d587fff09b034d936f"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/57/report
Content-Type: application/json
Authorization: Bearer 5df6d389a7a0b47b225ca7a4d61a1ccdec9221ee35aa90bd372b21e5d6ce2460
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
	-H "Authorization: Bearer 5df6d389a7a0b47b225ca7a4d61a1ccdec9221ee35aa90bd372b21e5d6ce2460"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/36
Content-Type: application/json
Authorization: Bearer e2dec525cd60e995094a04f05c89f3a8cb49ca00060f98aac62531110090d9bc
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
    "updated_at": "2016-10-25T10:04:50.131Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2dec525cd60e995094a04f05c89f3a8cb49ca00060f98aac62531110090d9bc"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer faf6c310343b1e691425e8b2a878fe86f457ede52c2d079086495e7815fd6aa1
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
      "updated_at": "2016-10-25T10:04:50.217Z"
    },
    {
      "id": 38,
      "name": "Fake Company Name 33",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T10:04:50.224Z"
    },
    {
      "id": 39,
      "name": "Fake Company Name 34",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/16d198fc47e748100dc445f0d390e3c9890a6b28.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-25T10:04:50.229Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer faf6c310343b1e691425e8b2a878fe86f457ede52c2d079086495e7815fd6aa1"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/34/company_profiles
Content-Type: application/json
Authorization: Bearer d2cbca886f8acaaf49f63bbb33b99ef2a9e0c51a80db020683c97c423937e347
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
curl "api.goskive.com/v2/companies/34/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2cbca886f8acaaf49f63bbb33b99ef2a9e0c51a80db020683c97c423937e347"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/33/company_profiles
Content-Type: application/json
Authorization: Bearer abe2e363622c226f636d613b34231b8ca068111d3e285d8cf553e45f22023ec1
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
curl "api.goskive.com/v2/companies/33/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abe2e363622c226f636d613b34231b8ca068111d3e285d8cf553e45f22023ec1"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 36fc109980a75941eeed3b559fa7a6e3a0e5176e8e601e7318054c44a037950d
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
      "company_id": 18,
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
      "company_id": 21,
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
	-H "Authorization: Bearer 36fc109980a75941eeed3b559fa7a6e3a0e5176e8e601e7318054c44a037950d"
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
Authorization: Bearer 84d3acbc41df6dcbd9546a2f41288cd78456ab5fd018e70fcea5369aeeb6f2d2
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
	-H "Authorization: Bearer 84d3acbc41df6dcbd9546a2f41288cd78456ab5fd018e70fcea5369aeeb6f2d2"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c878832af6b1b6b5e9632fc33365b70d8ba5de43a9e4c4b20e8284e8ec475642
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
    "id": 161,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T10:04:44.084Z",
    "course_id": 277,
    "author_id": 841,
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
	-H "Authorization: Bearer c878832af6b1b6b5e9632fc33365b70d8ba5de43a9e4c4b20e8284e8ec475642"
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-25T10:04:45.226Z",
      "course_id": 283,
      "author_id": 861,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 170,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-25T10:04:45.252Z",
      "course_id": 283,
      "author_id": 862,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 171,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-25T10:04:45.531Z",
      "course_id": 283,
      "author_id": 863,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T10:04:45.148Z",
      "questions_updated_at": "2016-10-25T10:04:45.148Z",
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
Authorization: Bearer 0e0fac5c452472bc260e3fc25a77d4b729caf9029f807d40add6f9b79bded0a6
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
      "id": 175,
      "title": "Clever Chapter Title 157",
      "position": 1,
      "updated_at": "2016-10-25T10:04:45.960Z",
      "course_id": 286,
      "author_id": 872,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 176,
      "title": "Clever Chapter Title 158",
      "position": 2,
      "updated_at": "2016-10-25T10:04:45.984Z",
      "course_id": 286,
      "author_id": 873,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 177,
      "title": "Clever Chapter Title 159",
      "position": 3,
      "updated_at": "2016-10-25T10:04:46.242Z",
      "course_id": 286,
      "author_id": 874,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-25T10:04:45.881Z",
      "questions_updated_at": "2016-10-25T10:04:45.881Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e0fac5c452472bc260e3fc25a77d4b729caf9029f807d40add6f9b79bded0a6"
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
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-25T10:04:45.787Z",
      "course_id": 285,
      "author_id": 868,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 173,
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-25T10:04:45.813Z",
      "course_id": 285,
      "author_id": 869,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 174,
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-25T10:04:45.838Z",
      "course_id": 285,
      "author_id": 870,
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
Authorization: Bearer df001b8158dba6ae767e260ad5c17eeb55ea4761a2d6fcdbf8d4e247a2811ffe
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
      "id": 178,
      "title": "Clever Chapter Title 160",
      "position": 1,
      "updated_at": "2016-10-25T10:04:46.402Z",
      "course_id": 287,
      "author_id": 879,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 179,
      "title": "Clever Chapter Title 161",
      "position": 2,
      "updated_at": "2016-10-25T10:04:46.427Z",
      "course_id": 287,
      "author_id": 880,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 180,
      "title": "Clever Chapter Title 162",
      "position": 3,
      "updated_at": "2016-10-25T10:04:46.451Z",
      "course_id": 287,
      "author_id": 881,
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
	-H "Authorization: Bearer df001b8158dba6ae767e260ad5c17eeb55ea4761a2d6fcdbf8d4e247a2811ffe"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 1df8e2f02bd0f840c404f557d5289ec09f28d753aabeef9da395bfd292868995
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
    "course_id": 16,
    "user_id": 49,
    "updated_at": "2016-10-25T10:03:31.353Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1df8e2f02bd0f840c404f557d5289ec09f28d753aabeef9da395bfd292868995"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 0df113686aeceb23a6c8decaeccc4bf5ce803d9883ab831bfdbdf592956c92ab
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
      "id": 4,
      "course_id": 17,
      "user_id": 51,
      "updated_at": "2016-10-25T10:03:31.444Z"
    },
    {
      "id": 5,
      "course_id": 17,
      "user_id": 52,
      "updated_at": "2016-10-25T10:03:31.459Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0df113686aeceb23a6c8decaeccc4bf5ce803d9883ab831bfdbdf592956c92ab"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/298/files
Content-Type: application/json
Authorization: Bearer 6e51f43a897116e2cef90528a5bfd66c11843c7d4f4ca750473d0f9bed9b638e
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
      "id": 13,
      "uploader": {
        "id": 916,
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
        "created_at": "2016-10-25T10:04:49.772Z",
        "updated_at": "2016-10-25T10:04:49.772Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T10:04:49.783Z",
      "updated_at": "2016-10-25T10:04:49.783Z",
      "course_id": 298,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 14,
      "uploader": {
        "id": 917,
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
        "created_at": "2016-10-25T10:04:49.791Z",
        "updated_at": "2016-10-25T10:04:49.791Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T10:04:49.801Z",
      "updated_at": "2016-10-25T10:04:49.801Z",
      "course_id": 298,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 15,
      "uploader": {
        "id": 918,
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
        "created_at": "2016-10-25T10:04:49.810Z",
        "updated_at": "2016-10-25T10:04:49.810Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-10-25T10:04:49.821Z",
      "updated_at": "2016-10-25T10:04:49.821Z",
      "course_id": 298,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/298/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e51f43a897116e2cef90528a5bfd66c11843c7d4f4ca750473d0f9bed9b638e"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/297/files
Content-Type: application/json
Authorization: Bearer dc01db37f7d09df66c95e9607b5e2ede653dfc2427822d2bec889d176839b5cb
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
    "id": 12,
    "uploader": {
      "id": 914,
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
      "created_at": "2016-10-25T10:04:49.600Z",
      "updated_at": "2016-10-25T10:04:49.600Z"
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
    "created_at": "2016-10-25T10:04:49.632Z",
    "updated_at": "2016-10-25T10:04:49.632Z",
    "course_id": 297,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/297/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc01db37f7d09df66c95e9607b5e2ede653dfc2427822d2bec889d176839b5cb"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/300/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer df413070eab1d41d7a63514e786bcf38bebdeee89343ee6858901a6384a53c6f
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
    "key": "cache/71fc08033ba6623f0fbbe6adf328c763.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxMTowNDo1MFoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzcxZmMwODAzM2JhNjYyM2YwZmJiZTZhZGYzMjhjNzYzLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEwMjUvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMDI1VDEwMDQ1MFoifV19",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T100450Z",
    "x-amz-signature": "8116be17c7c3eb54b4a1854c738582361abf81de4d2547caaf0384c0ffabbcfa"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/300/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df413070eab1d41d7a63514e786bcf38bebdeee89343ee6858901a6384a53c6f"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer c402644d5c79bf6a48cb2d0b7373155699a4d7e86d391f01cb353d774954b627
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
	-H "Authorization: Bearer c402644d5c79bf6a48cb2d0b7373155699a4d7e86d391f01cb353d774954b627"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4bbc95c13da946f4a5750a7cf9ffc23d0dab2d93c79aa0bb7f3c3d1f4aa10ee1
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
	-H "Authorization: Bearer 4bbc95c13da946f4a5750a7cf9ffc23d0dab2d93c79aa0bb7f3c3d1f4aa10ee1"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e0e4a6f9c001b524bafe1614b9340870a1d492b28f703c00e3d546fc0c5070f4
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
	-H "Authorization: Bearer e0e4a6f9c001b524bafe1614b9340870a1d492b28f703c00e3d546fc0c5070f4"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d62695d6448a3a1628fa2685a7c4a6ccfc176304ec27e9d5d134cb3defddc8c1
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
	-H "Authorization: Bearer d62695d6448a3a1628fa2685a7c4a6ccfc176304ec27e9d5d134cb3defddc8c1"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a791b4b2d4ad48ddac139d86fc52689b010f84bb5a39946799c14a019976ed6c
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
	-H "Authorization: Bearer a791b4b2d4ad48ddac139d86fc52689b010f84bb5a39946799c14a019976ed6c"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer ef1b78ca3a9f083c7c906d7b2480e65ae3339f3683a41455f1b4fdd196f577b3
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
    "creator_id": 308,
    "id": 114,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 98,
    "additional_university_ids": [

    ],
    "topic_id": 114,
    "discipline_id": 114,
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
    "chapters_updated_at": "2016-10-25T10:03:58.907Z",
    "updated_at": "2016-10-25T10:04:00.734Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 63,
        "title": "Clever Chapter Title 48",
        "position": 1,
        "updated_at": "2016-10-25T10:04:00.677Z",
        "course_id": 114,
        "author_id": 308,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T10:03:58.907Z",
        "questions_updated_at": "2016-10-25T10:03:58.907Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 64,
        "title": "Clever Chapter Title 49",
        "position": 2,
        "updated_at": "2016-10-25T10:04:00.724Z",
        "course_id": 114,
        "author_id": 308,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T10:03:58.907Z",
        "questions_updated_at": "2016-10-25T10:03:58.907Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 20,
        "obfuscated_id": "4DFpearSrHk",
        "author_id": 309,
        "chapter_id": 63,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:00.477Z",
        "created_at": "2016-10-25T10:04:00.477Z",
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
        "author_id": 309,
        "chapter_id": 64,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:00.567Z",
        "created_at": "2016-10-25T10:04:00.567Z",
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
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 309,
        "chapter_id": 63,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:00.528Z",
        "created_at": "2016-10-25T10:04:00.528Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 309,
        "chapter_id": 64,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:00.615Z",
        "created_at": "2016-10-25T10:04:00.615Z",
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
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 309,
        "chapter_id": 63,
        "position": 46,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:59.162Z",
        "created_at": "2016-10-25T10:03:59.010Z",
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
            "id": 110,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 111,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 309,
        "chapter_id": 63,
        "position": 47,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:59.384Z",
        "created_at": "2016-10-25T10:03:59.240Z",
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
      },
      {
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 309,
        "chapter_id": 64,
        "position": 48,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:59.653Z",
        "created_at": "2016-10-25T10:03:59.487Z",
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
            "id": 114,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 115,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 309,
        "chapter_id": 64,
        "position": 49,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:03:59.888Z",
        "created_at": "2016-10-25T10:03:59.736Z",
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
            "id": 116,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 117,
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
	-H "Authorization: Bearer ef1b78ca3a9f083c7c906d7b2480e65ae3339f3683a41455f1b4fdd196f577b3"
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
    "creator_id": 320,
    "id": 116,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 100,
    "additional_university_ids": [

    ],
    "topic_id": 116,
    "discipline_id": 116,
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
    "chapters_updated_at": "2016-10-25T10:04:02.955Z",
    "updated_at": "2016-10-25T10:04:05.017Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 67,
        "title": "Clever Chapter Title 52",
        "position": 1,
        "updated_at": "2016-10-25T10:04:04.961Z",
        "course_id": 116,
        "author_id": 320,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T10:04:02.955Z",
        "questions_updated_at": "2016-10-25T10:04:02.955Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 68,
        "title": "Clever Chapter Title 53",
        "position": 2,
        "updated_at": "2016-10-25T10:04:05.007Z",
        "course_id": 116,
        "author_id": 320,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-25T10:04:02.955Z",
        "questions_updated_at": "2016-10-25T10:04:02.955Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 320,
        "chapter_id": 67,
        "position": 58,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:03.270Z",
        "created_at": "2016-10-25T10:04:03.069Z",
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
            "id": 134,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 135,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 320,
        "chapter_id": 68,
        "position": 60,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T10:04:03.811Z",
        "created_at": "2016-10-25T10:04:03.618Z",
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
            "id": 138,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 139,
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
PUT /v2/courses/118/pin
Content-Type: application/json
Authorization: Bearer 1447b472a2d52938eb69c2614f5cde810c3b96fa9d4519a7818a77e653fda8d9
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/118/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1447b472a2d52938eb69c2614f5cde810c3b96fa9d4519a7818a77e653fda8d9"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/113/pin
Content-Type: application/json
Authorization: Bearer fbfaeb81fcb9ec0df1960d5143f07c579d56f3d990cd948261cf5b4b08aa4bff
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/113/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbfaeb81fcb9ec0df1960d5143f07c579d56f3d990cd948261cf5b4b08aa4bff"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 43cbf7b3b954afcc6d60186539dc52033b02a55f427806829389dd2ae5db1a09
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
    "creator_id": 335,
    "id": 120,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 104,
    "additional_university_ids": [

    ],
    "topic_id": 120,
    "discipline_id": 120,
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
    "updated_at": "2016-10-25T10:04:07.722Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43cbf7b3b954afcc6d60186539dc52033b02a55f427806829389dd2ae5db1a09"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 9a42dcb8a9f9c95d896ccc23c8c56bcad82ab647ff18c91aaecb8fcda45649cb
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
    "id": 964,
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
    "created_at": "2016-10-25T10:04:53.291Z",
    "updated_at": "2016-10-25T10:04:53.291Z",
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
	-H "Authorization: Bearer 9a42dcb8a9f9c95d896ccc23c8c56bcad82ab647ff18c91aaecb8fcda45649cb"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 25f7ba95d88d40e470664b5496112fd15d754b14c1328f85ca9bb363b2d43320
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[318]}
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
    "id": 966,
    "first_name": "Sven",
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
    "created_at": "2016-10-25T10:04:53.726Z",
    "updated_at": "2016-10-25T10:04:53.766Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[318]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25f7ba95d88d40e470664b5496112fd15d754b14c1328f85ca9bb363b2d43320"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer bcd47e52a36be100cb4220f0d39b4c289ed5e62f886eb9128575dd992214f7e1
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
    "id": 967,
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
    "created_at": "2016-10-25T10:04:53.787Z",
    "updated_at": "2016-10-25T10:04:53.787Z",
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
	-H "Authorization: Bearer bcd47e52a36be100cb4220f0d39b4c289ed5e62f886eb9128575dd992214f7e1"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 9e9f9a1674d04b6c82ffc376de6142178f26c762755def007a50aef906d9cf5c
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[321]}
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
    "id": 969,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      321
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T10:04:53.968Z",
    "updated_at": "2016-10-25T10:04:53.968Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[321]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e9f9a1674d04b6c82ffc376de6142178f26c762755def007a50aef906d9cf5c"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 29acf9549788e2482ef549dd1e4a946069fbd74cc3152047a37bb9185a5a3e9b
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

317
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
    "id": 965,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/567b2ace1372c9cd11a461e875f93717004ad57e.jpg",
    "university_id": null,
    "fields_of_study": [
      317
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-25T10:04:53.386Z",
    "updated_at": "2016-10-25T10:04:53.671Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/2fa76858f2314df42d5f54e5739afdf93b2a0fdb.jpg",
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

317
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 29acf9549788e2482ef549dd1e4a946069fbd74cc3152047a37bb9185a5a3e9b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 6bc2b4bde577af10b6543a2d8271b31742f91090c92e6c004cc69e2669b26dd5
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
      "bookmarkable_id": 82,
      "bookmarkable_type": "Question"
    },
    {
      "id": 6,
      "bookmarkable_id": 83,
      "bookmarkable_type": "Question"
    },
    {
      "id": 7,
      "bookmarkable_id": 84,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bc2b4bde577af10b6543a2d8271b31742f91090c92e6c004cc69e2669b26dd5"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer fae1248cac44620e37552ef1e7da22bb469bbaaa339a8a83555d493dad1d361c
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
      "company_id": 29,
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
      "company_id": 30,
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
	-H "Authorization: Bearer fae1248cac44620e37552ef1e7da22bb469bbaaa339a8a83555d493dad1d361c"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 18c12bb776935407232e3a709da6c783b907fe2730d255cc7e0cc9aa9b00cd9d
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
      "company_id": 25,
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
	-H "Authorization: Bearer 18c12bb776935407232e3a709da6c783b907fe2730d255cc7e0cc9aa9b00cd9d"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 7aa2ed1c3931ec47e850666b7058ab4d173d1f9fbf05b9efd113549f9f962348
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
      "creator_id": 385,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-88",
      "html_url": "https://goskive.com/course/mit-course-88",
      "slug": "mit-course-88",
      "university_id": 123,
      "additional_university_ids": [

      ],
      "topic_id": 142,
      "discipline_id": 142,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 88",
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
      "updated_at": "2016-10-25T10:04:12.451Z",
      "shortname": "mit-course-88"
    },
    {
      "creator_id": 386,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-89",
      "html_url": "https://goskive.com/course/mit-course-89",
      "slug": "mit-course-89",
      "university_id": 124,
      "additional_university_ids": [

      ],
      "topic_id": 143,
      "discipline_id": 143,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 89",
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
      "updated_at": "2016-10-25T10:04:12.558Z",
      "shortname": "mit-course-89"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7aa2ed1c3931ec47e850666b7058ab4d173d1f9fbf05b9efd113549f9f962348"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 50d8ed51f7a5576186e6a5c13e9cc20d3e04a2d8726447a339613287fc0b6ac4
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
      "company_id": 9,
      "company": {
        "id": 9,
        "name": "Fake Company Name 9",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T10:03:36.846Z"
      },
      "created_at": "2016-10-25T10:03:36.850Z",
      "updated_at": "2016-10-25T10:03:36.850Z",
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
      "company_id": 10,
      "company": {
        "id": 10,
        "name": "Fake Company Name 10",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T10:03:36.859Z"
      },
      "created_at": "2016-10-25T10:03:36.863Z",
      "updated_at": "2016-10-25T10:03:36.863Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 50d8ed51f7a5576186e6a5c13e9cc20d3e04a2d8726447a339613287fc0b6ac4"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 8100873118e56b05fd90ad15440fbcffab03fde5026e8c24705d130b1f146945
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
      "company_id": 5,
      "company": {
        "id": 5,
        "name": "Fake Company Name 5",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/43081c49f5a649e7eaa12b6c57edd214ce5a5217.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T10:03:36.608Z"
      },
      "created_at": "2016-10-25T10:03:36.612Z",
      "updated_at": "2016-10-25T10:03:36.612Z",
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
      "company_id": 6,
      "company": {
        "id": 6,
        "name": "Fake Company Name 6",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b7b0a8111e517c46508952441a65ecd639bff481.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-25T10:03:36.625Z"
      },
      "created_at": "2016-10-25T10:03:36.629Z",
      "updated_at": "2016-10-25T10:03:36.629Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8100873118e56b05fd90ad15440fbcffab03fde5026e8c24705d130b1f146945"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 0e9535e9080f5d1745f0071828e82a10eff53fd8b688d0177f78ba51dbae5cde
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
      "id": 18,
      "created_at": "2016-10-25T10:04:50.680Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 58,
      "updated_at": "2016-10-25T10:04:50.796Z",
      "author_id": "933",
      "thread_subject_id": "301",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 19,
      "created_at": "2016-10-25T10:04:50.782Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 59,
      "updated_at": "2016-10-25T10:04:50.800Z",
      "author_id": "936",
      "thread_subject_id": "302",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-10-25T10:04:51.202Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 20,
      "updated_at": "2016-10-25T10:04:51.202Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 21,
      "created_at": "2016-10-25T10:04:51.601Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 21,
      "updated_at": "2016-10-25T10:04:51.601Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 22,
      "created_at": "2016-10-25T10:04:52.065Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 22,
      "updated_at": "2016-10-25T10:04:52.065Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 23,
      "created_at": "2016-10-25T10:04:52.395Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 132,
      "updated_at": "2016-10-25T10:04:52.395Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-10-25T10:04:52.719Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 133,
      "updated_at": "2016-10-25T10:04:52.719Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 25,
      "created_at": "2016-10-25T10:04:53.037Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 134,
      "updated_at": "2016-10-25T10:04:53.037Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0e9535e9080f5d1745f0071828e82a10eff53fd8b688d0177f78ba51dbae5cde"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/26
Content-Type: application/json
Authorization: Bearer 3ab91613c1e4a1417fc08ad0ea811fbf1e0521318a2c147dcb9f211799e9dcbc
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-25T09:54:53.000Z"}}
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
    "id": 26,
    "created_at": "2016-10-25T10:04:53.234Z",
    "read_at": "2016-10-25T09:54:53.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 60,
    "updated_at": "2016-10-25T10:04:53.274Z",
    "author_id": "962",
    "thread_subject_id": "309",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/26" -d '{"notification":{"read_at":"2016-10-25T09:54:53.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ab91613c1e4a1417fc08ad0ea811fbf1e0521318a2c147dcb9f211799e9dcbc"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 62b8ee2033ac524b1ce0cd634b10e35fd43f4a276dec5264bb1d626f9d4b2383
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
      "course_id": 150,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T10:04:16.629Z",
      "course_published": true,
      "updated_at": "2016-10-25T10:04:16.618Z"
    },
    {
      "id": 6,
      "course_id": 151,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-25T10:04:16.724Z",
      "course_published": true,
      "updated_at": "2016-10-25T10:04:16.713Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 62b8ee2033ac524b1ce0cd634b10e35fd43f4a276dec5264bb1d626f9d4b2383"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/8
Content-Type: application/json
Authorization: Bearer cf3ab9f875b03fdc6b3e1e2751deca7bd3e5fc44042641b1e55d06a908dccc0f
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
    "course_id": 153,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-25T10:04:17.029Z",
    "course_published": true,
    "updated_at": "2016-10-25T10:04:17.019Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/8" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf3ab9f875b03fdc6b3e1e2751deca7bd3e5fc44042641b1e55d06a908dccc0f"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/7
Content-Type: application/json
Authorization: Bearer ff859088497fb430273e1bf8cde86b2820d4b012762362bde98f555526f355ea
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
    "course_id": 152,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-25T10:04:16.915Z",
    "course_published": true,
    "updated_at": "2016-10-25T10:04:16.899Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/7" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff859088497fb430273e1bf8cde86b2820d4b012762362bde98f555526f355ea"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 6bd065add9b998168a031bcabf9aae206df80b5993e5c0aa29eca5dbfe4aeb05
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
      "votable_id": 85,
      "user_id": 399
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 86,
      "user_id": 399
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 87,
      "user_id": 399
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 88,
      "user_id": 399
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bd065add9b998168a031bcabf9aae206df80b5993e5c0aa29eca5dbfe4aeb05"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/183
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
    "id": 183,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 181,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 183
      },
      {
        "id": 182,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 183
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/183" -X GET \
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
      "id": 181,
      "name": "Seamless context-sensitive protocol",
      "name_translations": {
        "en": "Seamless context-sensitive protocol"
      }
    },
    {
      "id": 182,
      "name": "Team-oriented radical functionalities",
      "name_translations": {
        "en": "Team-oriented radical functionalities"
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
PATCH /v2/feedbacks/23/close
Content-Type: application/json
Authorization: Bearer 1fffb8152c653e6d5264053e5d8f109a25b69c3955cde1bec50c2ca3e2f09831
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
    "id": 23,
    "user_id": 642,
    "feedbackable_id": 88,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-25T10:04:31.637Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/23/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fffb8152c653e6d5264053e5d8f109a25b69c3955cde1bec50c2ca3e2f09831"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 203e3ce287f76f99e163fa4d223f89a6b6473668f6f7e38be2e3c5bd0d1c4d3d
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
    "id": 25,
    "user_id": 652,
    "feedbackable_id": 90,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-25T10:04:32.163Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 203e3ce287f76f99e163fa4d223f89a6b6473668f6f7e38be2e3c5bd0d1c4d3d"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/19
Content-Type: application/json
Authorization: Bearer da794546aa6c9e90cba8d2a890c8d5ebbf81f53a32384006bd47c3a0c24dd7c2
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
    "user_id": 620,
    "feedbackable_id": 84,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T10:04:30.525Z",
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
	-H "Authorization: Bearer da794546aa6c9e90cba8d2a890c8d5ebbf81f53a32384006bd47c3a0c24dd7c2"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/21/close
Content-Type: application/json
Authorization: Bearer f647430550e818b480b0df0a0b1784b7d2cd96e5ba9234d07baf6bafa2e12ceb
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
curl "api.goskive.com/v2/feedbacks/21/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f647430550e818b480b0df0a0b1784b7d2cd96e5ba9234d07baf6bafa2e12ceb"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer ed5743470c2dac283fa456b9a078a2246369ce6fe24e894b3747205e0f5616bd
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
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed5743470c2dac283fa456b9a078a2246369ce6fe24e894b3747205e0f5616bd"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/fix
Content-Type: application/json
Authorization: Bearer 4e2b31150d77407a4161e69ab57a724024c96994e6585b1ba8b3413d471612ad
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
curl "api.goskive.com/v2/feedbacks/27/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e2b31150d77407a4161e69ab57a724024c96994e6585b1ba8b3413d471612ad"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/20
Content-Type: application/json
Authorization: Bearer 33209cf47eb72a165ca3033939cde41b3e688405fbe9a2d7a8962cb1e45ec3c3
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
    "user_id": 625,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T10:04:30.833Z",
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
	-H "Authorization: Bearer 33209cf47eb72a165ca3033939cde41b3e688405fbe9a2d7a8962cb1e45ec3c3"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Content-Type: application/json
Authorization: Bearer 8e086299ef84552be37103a4ba0b7c2601fe6647eb8985992806e3d929fb62c6
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
	-H "Authorization: Bearer 8e086299ef84552be37103a4ba0b7c2601fe6647eb8985992806e3d929fb62c6"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer 2789d4bee2acfaa281ae443e55b46a3829a2381dc5c4fba571a365df4a8b4acb
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
	-H "Authorization: Bearer 2789d4bee2acfaa281ae443e55b46a3829a2381dc5c4fba571a365df4a8b4acb"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/7
Content-Type: application/json
Authorization: Bearer 41b0080bc9a8df850cc2291a582350537a1c3776afc077f8112cde8733721b14
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/122a796a8c4965d48a275bcc5d274420.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T100426Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=29bed80ef7e0ec97457482ec9cb4d68cf3e2c9e3a206c24d66a4b17629f84d7a"
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41b0080bc9a8df850cc2291a582350537a1c3776afc077f8112cde8733721b14"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/3/preview
Content-Type: application/json
Authorization: Bearer db4c9c50e3eecd8c743ef963b67cdb9ab44c1ffb3c6845c2847048a71e2e1f7f
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/5289939aaf35dcb6f3891226a6330bda.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161025%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161025T100425Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=40477483200e73b039167f81aeb92ea584f1913c4a827604819168d0258e8e0b"
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
	-H "Authorization: Bearer db4c9c50e3eecd8c743ef963b67cdb9ab44c1ffb3c6845c2847048a71e2e1f7f"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/6/metadata
Content-Type: application/json
Authorization: Bearer d3a5bdd0662744276b7087ac09faddf9f53770c21a188d94a13af92c25fc3082
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
    "id": 6,
    "uploader": {
      "id": 564,
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
      "created_at": "2016-10-25T10:04:26.040Z",
      "updated_at": "2016-10-25T10:04:26.040Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T10:04:26.121Z",
    "updated_at": "2016-10-25T10:04:26.121Z",
    "course_id": 192,
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
curl "api.goskive.com/v2/files/6/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3a5bdd0662744276b7087ac09faddf9f53770c21a188d94a13af92c25fc3082"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/1/matched_courses?required_cu_count=2
Authorization: Bearer ff369ba2c811f24aa792beb7033f7ae17fe2c5e735d0639f9caa83e909232594
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
      "creator_id": 143,
      "id": 37,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 37,
      "discipline_id": 37,
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
      "chapters_updated_at": "2016-10-25T10:03:39.397Z",
      "updated_at": "2016-10-25T10:03:41.171Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 148,
      "id": 38,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-eda1f507-95a4-40dc-af14-53614a69e772",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-eda1f507-95a4-40dc-af14-53614a69e772",
      "slug": "mit-the-great-british-bake-off-eda1f507-95a4-40dc-af14-53614a69e772",
      "university_id": 44,
      "additional_university_ids": [

      ],
      "topic_id": 38,
      "discipline_id": 38,
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
      "chapters_updated_at": "2016-10-25T10:03:39.397Z",
      "updated_at": "2016-10-25T10:03:41.769Z",
      "shortname": "mit-the-great-british-bake-off-eda1f507-95a4-40dc-af14-53614a69e772"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/1/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer ff369ba2c811f24aa792beb7033f7ae17fe2c5e735d0639f9caa83e909232594"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/8/report
Content-Type: application/json
Authorization: Bearer c8d5e07562464b71aedd65554bfb34a565dc2e6037590803c294af29a6542159
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8d5e07562464b71aedd65554bfb34a565dc2e6037590803c294af29a6542159"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/49/comments
Content-Type: application/json
Authorization: Bearer d5355d72a386a49befe9855372fba243544f461f3b212ef01824af1bca638a8d
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
    "author_id": 373,
    "reply_to_id": null,
    "created_at": "2016-10-25T10:04:11.713Z",
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
curl "api.goskive.com/v2/flashcards/49/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5355d72a386a49befe9855372fba243544f461f3b212ef01824af1bca638a8d"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/47/comments
Content-Type: application/json
Authorization: Bearer 68012bfbdc7900069fb5e3ac42f0dabadf730a6f9a6c3f78a882ede0c42d7d67
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
    "id": 8,
    "author_id": 367,
    "reply_to_id": null,
    "created_at": "2016-10-25T10:04:11.124Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 2,
      "user_id": 367,
      "feedbackable_id": 47,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:11.121Z",
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
curl "api.goskive.com/v2/flashcards/47/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68012bfbdc7900069fb5e3ac42f0dabadf730a6f9a6c3f78a882ede0c42d7d67"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/51/comments
Content-Type: application/json
Authorization: Bearer 8d8a4d9c0c9238309efcff75b813dd17475681198d39442b849b19128f347982
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
      "author_id": 383,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:12.312Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 382,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:04:12.295Z",
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
curl "api.goskive.com/v2/flashcards/51/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d8a4d9c0c9238309efcff75b813dd17475681198d39442b849b19128f347982"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/48/comments
Content-Type: application/json
Authorization: Bearer 85b470b1cc2ec6e16ecc36e158c34b71509d5d830feac8a7982884ccb6ca8e64
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
curl "api.goskive.com/v2/flashcards/48/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85b470b1cc2ec6e16ecc36e158c34b71509d5d830feac8a7982884ccb6ca8e64"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/77/feedbacks
Content-Type: application/json
Authorization: Bearer 60ac0e45544fd176dce1dd972389de7937f8ca728d46d57250936669b3727a64
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
    "id": 4,
    "user_id": 511,
    "feedbackable_id": 77,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-25T10:04:22.841Z",
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
curl "api.goskive.com/v2/flashcards/77/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60ac0e45544fd176dce1dd972389de7937f8ca728d46d57250936669b3727a64"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/82/feedbacks
Content-Type: application/json
Authorization: Bearer 291a8f1e599da4467095a42706901a12718dc936cdec9aafa28dcfeb65f6d761
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
      "id": 10,
      "user_id": 540,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:24.067Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 539,
      "feedbackable_id": 82,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:24.056Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/82/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 291a8f1e599da4467095a42706901a12718dc936cdec9aafa28dcfeb65f6d761"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/5/votes
Content-Type: application/json
Authorization: Bearer 7a90c2866c24e21eccc370aeaf11a30f41e03baa8c2f2fc93ca2d3df8cb89d9c
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
      "id": 3,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 5,
      "user_id": 98
    },
    {
      "id": 2,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 5,
      "user_id": 97
    },
    {
      "id": 1,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 5,
      "user_id": 96
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/5/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a90c2866c24e21eccc370aeaf11a30f41e03baa8c2f2fc93ca2d3df8cb89d9c"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/53/republish
Content-Type: application/json
Authorization: Bearer 590b249567f51cd869bda1f03a37aaa4cb2439083ec88c439c04eda68d889003
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
curl "api.goskive.com/v2/flashcards/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 590b249567f51cd869bda1f03a37aaa4cb2439083ec88c439c04eda68d889003"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/57/bookmark
Content-Type: application/json
Authorization: Bearer 1d5549e083fee14e3f7815d6f21197b5ffb2964af509f2e3d7b696915521e39c
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/57/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d5549e083fee14e3f7815d6f21197b5ffb2964af509f2e3d7b696915521e39c"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/75
Content-Type: application/json
Authorization: Bearer 7646675aa5df4d37372dfbaf1c3b293f63733df32a6690a28e5b3caa0b90225c
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7646675aa5df4d37372dfbaf1c3b293f63733df32a6690a28e5b3caa0b90225c"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/downvote
Content-Type: application/json
Authorization: Bearer d4a1a8c42314e44b473180a4a795210633732cf1d1e7755fbe484eb240cf88e0
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/56/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4a1a8c42314e44b473180a4a795210633732cf1d1e7755fbe484eb240cf88e0"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/55
Content-Type: application/json
Authorization: Bearer 911733a97e0f15bbee3b13ba37d7a3904a106da9fd2d5c26d9d42d23e31bcdb0
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
    "id": 55,
    "obfuscated_id": "VX19tR4fHZ8",
    "author_id": 437,
    "chapter_id": 92,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:04:18.466Z",
    "created_at": "2016-10-25T10:04:18.466Z",
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
curl "api.goskive.com/v2/flashcards/55" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 911733a97e0f15bbee3b13ba37d7a3904a106da9fd2d5c26d9d42d23e31bcdb0"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/52/report
Content-Type: application/json
Authorization: Bearer b0907fe0ed19335788dbd4ba1f9fd78b38395ac1859afdaee24e0b799d246807
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/52/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0907fe0ed19335788dbd4ba1f9fd78b38395ac1859afdaee24e0b799d246807"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/74/bookmark
Content-Type: application/json
Authorization: Bearer 769fe86038ac646750336b126e1a10467dc268a4d41e7a2b2b636a6673d43906
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 769fe86038ac646750336b126e1a10467dc268a4d41e7a2b2b636a6673d43906"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/58/upvote
Content-Type: application/json
Authorization: Bearer c6a257fec8ff3ad9661a5da118b559584bebb34a3370b3bd8bbdf8ce46002510
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/58/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c6a257fec8ff3ad9661a5da118b559584bebb34a3370b3bd8bbdf8ce46002510"
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
    "key": "cache/d6fc03a446df75551b37b948b0048618.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0yNVQxMTowNDozOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlL2Q2ZmMwM2E0NDZkZjc1NTUxYjM3Yjk0OGIwMDQ4NjE4LmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTAyNS9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMjVUMTAwNDM5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161025/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161025T100439Z",
    "x-amz-signature": "3d6afc24e7079ce378e3e8b20dd7d305a95fdbfb4a51532edc994c6dae9047bc"
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
Authorization: Bearer 48e3b66ed27b1ee11b52ad8fe83dabfc15ee802d61d2275560b2dd63efb90dd6
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
	-H "Authorization: Bearer 48e3b66ed27b1ee11b52ad8fe83dabfc15ee802d61d2275560b2dd63efb90dd6"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/3/sign_ups
Content-Type: application/json
Authorization: Bearer d9fea6d5f689881e478117240d05e0cee76f99dda96aea43c2ebef4980cec808
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
	-H "Authorization: Bearer d9fea6d5f689881e478117240d05e0cee76f99dda96aea43c2ebef4980cec808"
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
{"password":{"reset_password_token":"enamKZ4fssAhyxZxsvUs","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 91,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-25T10:03:35.490Z",
  "updated_at": "2016-10-25T10:03:35.647Z",
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
  "audit_id": 3648
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"enamKZ4fssAhyxZxsvUs","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/7/comments
Content-Type: application/json
Authorization: Bearer b525bf6525686838fd28c35a3c89153d86e3867b453042d0d6e765fbf306bb83
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
    "id": 1,
    "author_id": 62,
    "reply_to_id": null,
    "created_at": "2016-10-25T10:03:32.288Z",
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
curl "api.goskive.com/v2/questions/7/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b525bf6525686838fd28c35a3c89153d86e3867b453042d0d6e765fbf306bb83"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/8/comments
Content-Type: application/json
Authorization: Bearer 8a69746322cf9ea246a6ea4c7570f5b818e68a4a3eb0cbeee5f0d27d8ff369d3
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
    "author_id": 65,
    "reply_to_id": null,
    "created_at": "2016-10-25T10:03:32.831Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 65,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:03:32.827Z",
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
curl "api.goskive.com/v2/questions/8/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a69746322cf9ea246a6ea4c7570f5b818e68a4a3eb0cbeee5f0d27d8ff369d3"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/10/comments
Content-Type: application/json
Authorization: Bearer ff3e997d6a77e2beb5405077b3e04a3ab25b1a66205e29b6cad64f723dd80cc9
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
      "author_id": 75,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:03:33.686Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 74,
      "reply_to_id": null,
      "created_at": "2016-10-25T10:03:33.669Z",
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
curl "api.goskive.com/v2/questions/10/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff3e997d6a77e2beb5405077b3e04a3ab25b1a66205e29b6cad64f723dd80cc9"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/9/comments
Content-Type: application/json
Authorization: Bearer f8f09b3d11b4e33f64bb372f3d6349e99ad3a447dbe066f1b9b4538aa850497c
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
curl "api.goskive.com/v2/questions/9/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f8f09b3d11b4e33f64bb372f3d6349e99ad3a447dbe066f1b9b4538aa850497c"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/93/feedbacks
Content-Type: application/json
Authorization: Bearer 436c25d487138e4a56b2836747a61d79f0c2a41abac94cd257b6656c84d64570
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
    "user_id": 584,
    "feedbackable_id": 93,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-25T10:04:28.007Z",
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
curl "api.goskive.com/v2/questions/93/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 436c25d487138e4a56b2836747a61d79f0c2a41abac94cd257b6656c84d64570"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer 4e53a3e340f68a49e877d5360d33930d560ba85d8e1cc6de464c55b7166ff125
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
      "id": 14,
      "user_id": 594,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:28.848Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 593,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T10:04:28.836Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/95/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e53a3e340f68a49e877d5360d33930d560ba85d8e1cc6de464c55b7166ff125"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/91/votes
Content-Type: application/json
Authorization: Bearer c8c44f36ecdcaeee7326563af83f0cc35ef7d4ec147d384b10c2c8098a1e32fc
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
      "votable_id": 91,
      "user_id": 555
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 91,
      "user_id": 554
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 91,
      "user_id": 553
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/91/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8c44f36ecdcaeee7326563af83f0cc35ef7d4ec147d384b10c2c8098a1e32fc"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/28/republish
Content-Type: application/json
Authorization: Bearer 079b03a379b9536dd179dd505e0f092fb969954b56b53ca1ba58d1263632d189
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
curl "api.goskive.com/v2/questions/28/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 079b03a379b9536dd179dd505e0f092fb969954b56b53ca1ba58d1263632d189"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/33/bookmark
Content-Type: application/json
Authorization: Bearer e430924f6f9a1260b4e1e620051915a5ba0c98bc8f6399867a88eba10dd957b9
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/33/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e430924f6f9a1260b4e1e620051915a5ba0c98bc8f6399867a88eba10dd957b9"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/51
Content-Type: application/json
Authorization: Bearer a7257b07fe7f1a5036df55f2fddf9ab901478f117fa110c12fb26d24ba18ab6d
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a7257b07fe7f1a5036df55f2fddf9ab901478f117fa110c12fb26d24ba18ab6d"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/30/downvote
Content-Type: application/json
Authorization: Bearer f22f9d065a0d74db541244feac8dde0f9a93ae88fb4e06429cbd2f43689cfeae
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/30/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f22f9d065a0d74db541244feac8dde0f9a93ae88fb4e06429cbd2f43689cfeae"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/32
Content-Type: application/json
Authorization: Bearer c050b0585296ed7897156e6d99b8caa83213092e67cebe4bea83e124581fda43
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
    "id": 32,
    "obfuscated_id": "mUuSuaqqphM",
    "author_id": 227,
    "chapter_id": 40,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:03:50.011Z",
    "created_at": "2016-10-25T10:03:49.867Z",
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
        "id": 63,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 64,
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
curl "api.goskive.com/v2/questions/32" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c050b0585296ed7897156e6d99b8caa83213092e67cebe4bea83e124581fda43"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/29/report
Content-Type: application/json
Authorization: Bearer 671ed1dfe61663ad95bd01602d755d8468da595d7016b591184bf0a9895fa1a3
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/29/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 671ed1dfe61663ad95bd01602d755d8468da595d7016b591184bf0a9895fa1a3"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/34/bookmark
Content-Type: application/json
Authorization: Bearer 5d9a5825bfc407c872dd90460e4ea7f40e6148ab47f76fa8ed24108575388a8d
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/34/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d9a5825bfc407c872dd90460e4ea7f40e6148ab47f76fa8ed24108575388a8d"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/50
Content-Type: application/json
Authorization: Bearer 8805a70efd072412c65b63149fbeab3faa84572bc79070c8b3998694be4a96a4
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":50,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T10:03:56.262Z","updated_at":"2016-10-25T10:03:56.411Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":58,"author_id":286,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 50,
    "obfuscated_id": "3_Ybw_gc_HE",
    "author_id": 286,
    "chapter_id": 58,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-25T10:03:56.532Z",
    "created_at": "2016-10-25T10:03:56.262Z",
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
    "question": "{\"id\"=>50, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-25T10:03:56.262Z\", \"updated_at\"=>\"2016-10-25T10:03:56.411Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>58, \"author_id\"=>286, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
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
      },
      {
        "id": 101,
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
curl "api.goskive.com/v2/questions/50" -d '{"question":{"question":{"id":50,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-25T10:03:56.262Z","updated_at":"2016-10-25T10:03:56.411Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":58,"author_id":286,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8805a70efd072412c65b63149fbeab3faa84572bc79070c8b3998694be4a96a4"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/31/upvote
Content-Type: application/json
Authorization: Bearer 88706dc1e26fd897bf40165872b8d0cbdebb9e33dbaa08a135f5b86a0e1681c2
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/31/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 88706dc1e26fd897bf40165872b8d0cbdebb9e33dbaa08a135f5b86a0e1681c2"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 6b960e8ab7c4429eff8b6ddcb9cb9875441bec0a25e6ca5e7e34417aac6cdc06
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
      "creator_id": 1,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "topic_id": 2,
      "discipline_id": 2,
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
      "updated_at": "2016-10-25T10:03:26.191Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b960e8ab7c4429eff8b6ddcb9cb9875441bec0a25e6ca5e7e34417aac6cdc06"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer b2a9bd6514044e31a16894f7ce2092ea873de786ac51552b135cdc994e5cc752
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
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-4",
      "html_url": "https://goskive.com/university/uni-4",
      "slug": "uni-4",
      "name": "National School of Pizza",
      "short_name": "Uni 4",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/edb44fa3b950d3df02a9aafc728bb3e4bb8888b4.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/1a967dae2b7a644187c1fa03f10ee72b48c5ebcc.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T10:03:26.680Z",
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
      "name": "National School of Pastry",
      "short_name": "Uni 3",
      "acronym": "NSPA",
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
      "updated_at": "2016-10-25T10:03:26.663Z",
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
	-H "Authorization: Bearer b2a9bd6514044e31a16894f7ce2092ea873de786ac51552b135cdc994e5cc752"
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
      "id": 135,
      "name": "Adaptive content-based flexibility",
      "name_translations": {
        "en": "Adaptive content-based flexibility"
      },
      "discipline_id": 135
    },
    {
      "id": 136,
      "name": "Future-proofed intangible application",
      "name_translations": {
        "en": "Future-proofed intangible application"
      },
      "discipline_id": 136
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
GET /v2/topics/134
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
    "id": 134,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 134
  }
}
```



```shell
curl "api.goskive.com/v2/topics/134" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 70203641f333be83ffa969ebac92165d56aa51b66f82953e6afbe9cb55699c99
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
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-30",
      "html_url": "https://goskive.com/university/uni-30",
      "slug": "uni-30",
      "name": "University 10",
      "short_name": "Uni 30",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/f3740963af3b785d81e56101e31332294478c35b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/8b2eb16060f7c6a977153a523ce088cd8b6cb975.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T10:03:37.181Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 33,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-31",
      "html_url": "https://goskive.com/university/uni-31",
      "slug": "uni-31",
      "name": "University 11",
      "short_name": "Uni 31",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/af4a59026331ce71aecbe5b7ff54137522b16fcc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/57d36010c7e6070facf87bca901b7198bfd678c1.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T10:03:37.199Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 34,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-32",
      "html_url": "https://goskive.com/university/uni-32",
      "slug": "uni-32",
      "name": "University 12",
      "short_name": "Uni 32",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0d61fd9a3b13fb0d6dd102dc17319bce477758bc.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e8e2a10c46f2726618f4ded45065de8d43618bb9.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-25T10:03:37.217Z",
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
	-H "Authorization: Bearer 70203641f333be83ffa969ebac92165d56aa51b66f82953e6afbe9cb55699c99"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 8efff16e7afb86f434837b44a838039fa1f28f22646822d3959b6a1721a718b3
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
    "id": 31,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0b535ca5da2e9b29b5fbc2937a72466afa2de998.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f2aa41db8d47b411c27b0c58cd6fdb58f76e09ba.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-25T10:03:37.118Z",
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
	-H "Authorization: Bearer 8efff16e7afb86f434837b44a838039fa1f28f22646822d3959b6a1721a718b3"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f36c0434509ab7fd47623ad7ed925ff1c40a2ab927f99eb0c8a1e7d71ffe2a1b
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":83,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "id": 83,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 67,
    "additional_university_ids": [

    ],
    "topic_id": 83,
    "discipline_id": 83,
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
    "chapters_updated_at": "2016-10-25T10:03:47.203Z",
    "updated_at": "2016-10-25T10:03:47.352Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 32,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-25T10:03:47.301Z",
        "course_id": 83,
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
        "id": 33,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-25T10:03:47.321Z",
        "course_id": 83,
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
        "id": 34,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-25T10:03:47.340Z",
        "course_id": 83,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":83,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f36c0434509ab7fd47623ad7ed925ff1c40a2ab927f99eb0c8a1e7d71ffe2a1b"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 17b73c720f95263c974c067ef3ec11107592964b9a5eab9280aa28df516d67b9
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":84,"published":false}}
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
    "creator_id": 211,
    "id": 84,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 68,
    "additional_university_ids": [

    ],
    "topic_id": 84,
    "discipline_id": 84,
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
    "updated_at": "2016-10-25T10:03:47.533Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":84,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17b73c720f95263c974c067ef3ec11107592964b9a5eab9280aa28df516d67b9"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0558c37465b5918c98cdcf83c409813246caf8279e24899169e3355ebbc2bc59
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
      "creator_id": 172,
      "id": 51,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "topic_id": 51,
      "discipline_id": 51,
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
      "updated_at": "2016-10-25T10:03:43.528Z",
      "shortname": "fu-course-19"
    },
    {
      "creator_id": 172,
      "id": 52,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 53,
      "additional_university_ids": [

      ],
      "topic_id": 52,
      "discipline_id": 52,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
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
      "chapters_updated_at": "2016-10-25T10:03:43.845Z",
      "updated_at": "2016-10-25T10:03:43.853Z",
      "shortname": "fu-course-20"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0558c37465b5918c98cdcf83c409813246caf8279e24899169e3355ebbc2bc59"
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
      "creator_id": 182,
      "id": 59,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 59,
      "discipline_id": 59,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
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
      "updated_at": "2016-10-25T10:03:44.456Z",
      "shortname": "fu-course-27"
    },
    {
      "creator_id": 182,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 56,
      "additional_university_ids": [

      ],
      "topic_id": 60,
      "discipline_id": 60,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
      "chapters_updated_at": "2016-10-25T10:03:44.812Z",
      "updated_at": "2016-10-25T10:03:44.820Z",
      "shortname": "fu-course-28"
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
Authorization: Bearer 6cdcf74261f182f789af29387b10d8f6c43e81490cd782bb5828b2412ceda510
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
      "creator_id": 178,
      "id": 55,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 55,
      "discipline_id": 55,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
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
      "updated_at": "2016-10-25T10:03:44.121Z",
      "shortname": "fu-course-23"
    },
    {
      "creator_id": 178,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 54,
      "additional_university_ids": [

      ],
      "topic_id": 56,
      "discipline_id": 56,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
      "updated_at": "2016-10-25T10:03:44.164Z",
      "shortname": "fu-course-24"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cdcf74261f182f789af29387b10d8f6c43e81490cd782bb5828b2412ceda510"
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
      "creator_id": 187,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 63,
      "discipline_id": 63,
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
      "updated_at": "2016-10-25T10:03:45.015Z",
      "shortname": "fu-course-31"
    },
    {
      "creator_id": 187,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 57,
      "additional_university_ids": [

      ],
      "topic_id": 64,
      "discipline_id": 64,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
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
      "updated_at": "2016-10-25T10:03:45.057Z",
      "shortname": "fu-course-32"
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
Authorization: Bearer 4b51cff0c808a2dd8f4ebf109cef0136ed03b67564409dc8d1d45f2803234a23
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
  "id": 9,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-25T10:03:27.486Z",
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
	-H "Authorization: Bearer 4b51cff0c808a2dd8f4ebf109cef0136ed03b67564409dc8d1d45f2803234a23"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/929
Content-Type: application/json
Authorization: Bearer 799de7c19beb170c378db5c580434639e99b2e1470ccf31b30742af8382c6be2
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
    "id": 929,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 285,
    "fields_of_study": [
      306,
      307
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-25T10:04:50.506Z",
    "updated_at": "2016-10-25T10:04:50.506Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/929" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 799de7c19beb170c378db5c580434639e99b2e1470ccf31b30742af8382c6be2"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/927
Content-Type: application/json
Authorization: Bearer 9e6c8bedb38621a96b363c5f26eee4a0362ca4885c76d97c3fcdd9f5bda183bb
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
    "id": 927,
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
    "created_at": "2016-10-25T10:04:50.336Z",
    "updated_at": "2016-10-25T10:04:50.336Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/927" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e6c8bedb38621a96b363c5f26eee4a0362ca4885c76d97c3fcdd9f5bda183bb"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/7
Content-Type: application/json
Authorization: Bearer 65ca1455fd71df967330b8a024efca55655cf9c31b2bb92f137956ee2eb8907a
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65ca1455fd71df967330b8a024efca55655cf9c31b2bb92f137956ee2eb8907a"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/5
Content-Type: application/json
Authorization: Bearer e498ce65cf1984c48c92749436aac22e0ecbe7a9f0a422c1c23243294a1ddf6c
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
    "id": 5,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 12,
    "user_id": 121
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e498ce65cf1984c48c92749436aac22e0ecbe7a9f0a422c1c23243294a1ddf6c"
```
