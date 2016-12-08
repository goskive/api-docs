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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0bb7e170b37a5bd399e5425b489bc6ef0342c9dec2d395f619f2e715719b7c73","client_secret":"41e01dd750d04ccf1f5d6d49ec11caf761294cfc65d90bc34513934c9d8bfa17"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"0bb7e170b37a5bd399e5425b489bc6ef0342c9dec2d395f619f2e715719b7c73","client_secret":"41e01dd750d04ccf1f5d6d49ec11caf761294cfc65d90bc34513934c9d8bfa17"}' -X POST \
	-H "Content-Type: application/json"
```
## Authentication error on create

Incorrect credentials gives a validation error.

### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MGNmODQ4NDk3ZmMwYzYxMjk0ZjkxZGY2ODEyNTA4MWMxNTY1MDU3OTc2MGFl
YzVkYWQxMWE1ODkwMGM2NjkyNjpjZDE0OTk3Y2YzZDI4YzYxZWNhYmFmNDk5
NjBjOGVlMDQ5NzJjM2NjNWIwNDMwM2ZlZWI3YzFmYzk3ODFkMTlh

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
	-u 0cf848497fc0c61294f91df68125081c15650579760aec5dad11a58900c66926:cd14997cf3d28c61ecabaf49960c8ee04972c3cc5b04303feeb7c1fc9781d19a
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"506cdc66e31bf74342a9f52e8d2819581d17d6b36541568c1ad584c74e822267","client_secret":"f73ff92b53a6f251300aeedca11f97585be8c8744c6d66105b3c81d28a184c1e"}
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
  "access_token": "cf4c2d54e3314ec56cc4c641c1f82a50f9d2eb330a234a2bd181773ae408f696",
  "token_type": "bearer",
  "created_at": 1481188247
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"506cdc66e31bf74342a9f52e8d2819581d17d6b36541568c1ad584c74e822267","client_secret":"f73ff92b53a6f251300aeedca11f97585be8c8744c6d66105b3c81d28a184c1e"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic MjM3ZGE3ODliNzYwMjlmZGZkYzRiN2I0ZWZkMjgwYjgxYzZiYTA1YTliOTg3
NzY5OGMyYmQxMmExMWQyNjZkYTo0YjkzOTAyODMwMzZjNjdkYmJmZTY0MDA4
YTQzOWY4YzA5NWJhZmI4YjMwYzZhMjM3MDBkNzk0M2JlZWNhYzNk

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
  "access_token": "3b110b5489fcd83b72b1d587557c79498cdb3a170b607dc3819f4e5ad7d879a7",
  "token_type": "bearer",
  "created_at": 1481188247
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 237da789b76029fdfdc4b7b4efd280b81c6ba05a9b9877698c2bd12a11d266da:4b9390283036c67dbbfe64008a439f8c095bafb8b30c6a23700d7943beecac3d
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
{"grant_type":"client_credentials","client_id":"c79511e3e2ea922efccd8327e54cede00c3128f4b479fee9b97020708d44cfe7","client_secret":"53a3cbaecc96b140b1042e4905449556488655a1e70f7f1c1b669c3d5ab90b9b"}
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
  "access_token": "924ed44a4ca49bf3504df12b6ba84a9ff013c7d2787c5160a6569098fe8c1ad7",
  "token_type": "bearer",
  "created_at": 1481188247
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"c79511e3e2ea922efccd8327e54cede00c3128f4b479fee9b97020708d44cfe7","client_secret":"53a3cbaecc96b140b1042e4905449556488655a1e70f7f1c1b669c3d5ab90b9b"}' -X POST \
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
GET /v2/campaigns/4
Content-Type: application/json
Authorization: Bearer 9b57374b018d56eba921e1b5be79b6fce5fae6434e619e8c26cdd546966d9d05
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
    "company_id": 19,
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
	-H "Authorization: Bearer 9b57374b018d56eba921e1b5be79b6fce5fae6434e619e8c26cdd546966d9d05"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/122/flashcards
Content-Type: application/json
Authorization: Bearer fd809634f00dfbf9fefc3aa95942d723ecfefe8e417bc8a400b5fad08f139669
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":122,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 77,
    "obfuscated_id": "v-Dlx6JosLA",
    "author_id": 721,
    "chapter_id": 122,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:10:26.507Z",
    "created_at": "2016-12-08T09:10:26.507Z",
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
curl "api.goskive.com/v2/chapters/122/flashcards" -d '{"flashcard":{"chapter_id":122,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd809634f00dfbf9fefc3aa95942d723ecfefe8e417bc8a400b5fad08f139669"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/123/flashcards
Content-Type: application/json
Authorization: Bearer d715b438e9840a264b4f235cf5b4302623222376bb1292c4681421c794f564e3
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 722,
      "chapter_id": 123,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:26.773Z",
      "created_at": "2016-12-08T09:10:26.773Z",
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
      "author_id": 722,
      "chapter_id": 123,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:26.815Z",
      "created_at": "2016-12-08T09:10:26.815Z",
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
      "id": 80,
      "obfuscated_id": "94gVa2GR5x8",
      "author_id": 722,
      "chapter_id": 123,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:26.856Z",
      "created_at": "2016-12-08T09:10:26.856Z",
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
curl "api.goskive.com/v2/chapters/123/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d715b438e9840a264b4f235cf5b4302623222376bb1292c4681421c794f564e3"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/37/questions
Content-Type: application/json
Authorization: Bearer 0cdc2582922b11e77b4afc59c081f2c7097a61484e3d4c8405e2f6a1c5369936
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":37,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 51,
    "obfuscated_id": "fXx2Zpse_KI",
    "author_id": 196,
    "chapter_id": 37,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:09:49.781Z",
    "created_at": "2016-12-08T09:09:49.781Z",
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
        "id": 101,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 102,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 103,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 104,
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
curl "api.goskive.com/v2/chapters/37/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":37,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0cdc2582922b11e77b4afc59c081f2c7097a61484e3d4c8405e2f6a1c5369936"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/35/questions
Content-Type: application/json
Authorization: Bearer 4145ba6536da085dbbac859113a0c10a5a73f162dcdd6597bca86b5bf544916e
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
    "id": 49,
    "obfuscated_id": "GNsH7ObIVl0",
    "author_id": 190,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:09:48.632Z",
    "created_at": "2016-12-08T09:09:48.632Z",
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
        "id": 97,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 98,
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
	-H "Authorization: Bearer 4145ba6536da085dbbac859113a0c10a5a73f162dcdd6597bca86b5bf544916e"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/36/questions
Content-Type: application/json
Authorization: Bearer 17f137f93e98f0bca1b976219028106b9e15af35f80fe20746213ffd3cdb4a60
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
    "id": 50,
    "obfuscated_id": "3_Ybw_gc_HE",
    "author_id": 193,
    "chapter_id": 36,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:09:49.214Z",
    "created_at": "2016-12-08T09:09:49.214Z",
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
        "id": 99,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 100,
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
	-H "Authorization: Bearer 17f137f93e98f0bca1b976219028106b9e15af35f80fe20746213ffd3cdb4a60"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/38/questions
Content-Type: application/json
Authorization: Bearer 10cb692d57e8b7e1fd7fbcf65794702c117362d79b577c68212a4a52a48b3544
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
    "id": 52,
    "obfuscated_id": "_rmh4zxMC_8",
    "author_id": 199,
    "chapter_id": 38,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:09:50.458Z",
    "created_at": "2016-12-08T09:09:50.458Z",
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
        "id": 105,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 106,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 107,
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
	-H "Authorization: Bearer 10cb692d57e8b7e1fd7fbcf65794702c117362d79b577c68212a4a52a48b3544"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/40/questions
Content-Type: application/json
Authorization: Bearer 6d22d1478a71282c91b15175f6b5e7f344d6ea4ac8230f6c8413f5f27b3b4df0
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
      "id": 53,
      "obfuscated_id": "XffxqHkTsbc",
      "author_id": 205,
      "chapter_id": 40,
      "position": 49,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:09:51.199Z",
      "created_at": "2016-12-08T09:09:51.094Z",
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
          "id": 108,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 109,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 54,
      "obfuscated_id": "cKxlQSpHm5w",
      "author_id": 206,
      "chapter_id": 40,
      "position": 50,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:09:51.380Z",
      "created_at": "2016-12-08T09:09:51.275Z",
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
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 207,
      "chapter_id": 40,
      "position": 51,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:09:51.565Z",
      "created_at": "2016-12-08T09:09:51.458Z",
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
```



```shell
curl "api.goskive.com/v2/chapters/40/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d22d1478a71282c91b15175f6b5e7f344d6ea4ac8230f6c8413f5f27b3b4df0"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/188
Content-Type: application/json
Authorization: Bearer 90e469696cff4c66726f3b853d93221298b5707b94a3653d5dae9b14cab32d51
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
	-H "Authorization: Bearer 90e469696cff4c66726f3b853d93221298b5707b94a3653d5dae9b14cab32d51"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/189
Content-Type: application/json
Authorization: Bearer a090bef7d3863d331f70224872d7d1b507bb5b6cec4bc39c3582d21caa14f7bd
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
curl "api.goskive.com/v2/chapters/189" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a090bef7d3863d331f70224872d7d1b507bb5b6cec4bc39c3582d21caa14f7bd"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/193
Content-Type: application/json
Authorization: Bearer dfd61bb53f973f24003f146528337dedf11253bd3a38ffeed3cfadfe8eadee28
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
curl "api.goskive.com/v2/chapters/193" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfd61bb53f973f24003f146528337dedf11253bd3a38ffeed3cfadfe8eadee28"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/187
Content-Type: application/json
Authorization: Bearer fd7061a82660d8e62c6e79fc98a69f257acbf0ed54ff7ff5210fcc67b3cb67d0
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/187" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd7061a82660d8e62c6e79fc98a69f257acbf0ed54ff7ff5210fcc67b3cb67d0"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/192
Content-Type: application/json
Authorization: Bearer b24d5d96a5b5380c8c0397142bbd0d0aa847862b91594c4f8472a7a417634af9
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
    "id": 192,
    "updated_at": "2016-12-08T09:10:46.374Z",
    "course_id": 310,
    "author_id": 962,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-12-08T09:10:45.906Z",
    "questions_updated_at": "2016-12-08T09:10:45.906Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 966,
        "chapter_id": 192,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:46.355Z",
        "created_at": "2016-12-08T09:10:46.355Z",
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
        "id": 134,
        "obfuscated_id": "tjpSvaJuWx4",
        "author_id": 964,
        "chapter_id": 192,
        "position": 121,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:46.250Z",
        "created_at": "2016-12-08T09:10:46.163Z",
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
            "id": 271,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 272,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/192" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b24d5d96a5b5380c8c0397142bbd0d0aa847862b91594c4f8472a7a417634af9"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/194
Content-Type: application/json
Authorization: Bearer 1fd050f31288ffd2633efc6dcc4728f415d59410243dbd86af531bed36e5e83c
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
    "id": 194,
    "updated_at": "2016-12-08T09:10:46.717Z",
    "course_id": 312,
    "author_id": 972,
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

    ],
    "title": "Eggs and Flour",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/194" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fd050f31288ffd2633efc6dcc4728f415d59410243dbd86af531bed36e5e83c"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/53/replies
Content-Type: application/json
Authorization: Bearer c62e79960d85629b50dd249ecea31f7aab3809355e24a090c6da5a18d594fb53
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
    "id": 54,
    "author_id": 617,
    "reply_to_id": 53,
    "created_at": "2016-12-08T09:10:18.495Z",
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
curl "api.goskive.com/v2/comments/53/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c62e79960d85629b50dd249ecea31f7aab3809355e24a090c6da5a18d594fb53"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/52/replies
Content-Type: application/json
Authorization: Bearer 1d90083f590566eaebfe441863a6ca51eae2581241a257e83d39a26b905e629a
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
curl "api.goskive.com/v2/comments/52/replies" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d90083f590566eaebfe441863a6ca51eae2581241a257e83d39a26b905e629a"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/14
Content-Type: application/json
Authorization: Bearer 16eedc14891bc4b49646df88ac9e434444d3a43e642b61d3b4db3d1539fa61f0
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
curl "api.goskive.com/v2/comments/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16eedc14891bc4b49646df88ac9e434444d3a43e642b61d3b4db3d1539fa61f0"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/12/republish
Content-Type: application/json
Authorization: Bearer a2ea35562722d95d99c78fbcd4301587c3d67d9f5d2cc7a6600afe5c3eea6afa
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
	-H "Authorization: Bearer a2ea35562722d95d99c78fbcd4301587c3d67d9f5d2cc7a6600afe5c3eea6afa"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/15
Content-Type: application/json
Authorization: Bearer 5760d4befd538a013eea25da44f7408588bcbdf83b3c2cff5b5ee7687fdeab43
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5760d4befd538a013eea25da44f7408588bcbdf83b3c2cff5b5ee7687fdeab43"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/51/report
Content-Type: application/json
Authorization: Bearer 7a7cbbc248cd0e9a884f813acc4d74156c6f06ca696385d215a62cbaa039414b
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
	-H "Authorization: Bearer 7a7cbbc248cd0e9a884f813acc4d74156c6f06ca696385d215a62cbaa039414b"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/7
Content-Type: application/json
Authorization: Bearer 03248184cbbc382ecea811a91ec69d2a3f0ee55c5fdf5b91eaaf46c7ddf22089
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
    "id": 7,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/ee07e3c1dbfd9b0742bac1025a12f4991c814c05.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-12-08T09:09:39.077Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/7" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03248184cbbc382ecea811a91ec69d2a3f0ee55c5fdf5b91eaaf46c7ddf22089"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer a3c87073641f40c5602ac9e7357114898bdeea45cab60af7c5dda4812b1d3351
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
      "id": 8,
      "name": "Fake Company Name 4",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/753c2bdec204ddfbf301748c92aa8410827672df.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T09:09:39.202Z"
    },
    {
      "id": 9,
      "name": "Fake Company Name 5",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T09:09:39.206Z"
    },
    {
      "id": 10,
      "name": "Fake Company Name 6",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/025ac3b1d278887cc2e2d460347ff7a7aed50b3d.png",
      "brand_color": "#000000",
      "updated_at": "2016-12-08T09:09:39.210Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3c87073641f40c5602ac9e7357114898bdeea45cab60af7c5dda4812b1d3351"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/5/company_profiles
Content-Type: application/json
Authorization: Bearer 13636652cb27a2389030c6365992032ac0179470e9204aa5790abad1dd5955e6
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
curl "api.goskive.com/v2/companies/5/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13636652cb27a2389030c6365992032ac0179470e9204aa5790abad1dd5955e6"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/4/company_profiles
Content-Type: application/json
Authorization: Bearer 28da6ad3d8a02aaf9cfd7feb1b2a64d14c71cb60a645f17cd6cdfcdef2d376bb
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
curl "api.goskive.com/v2/companies/4/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28da6ad3d8a02aaf9cfd7feb1b2a64d14c71cb60a645f17cd6cdfcdef2d376bb"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer be19992f84b4ecbd0ca2eaec67b3dd4129dab82f2751411ef16bef28dd3bb344
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
      "company_id": 20,
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
      "company_id": 23,
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
	-H "Authorization: Bearer be19992f84b4ecbd0ca2eaec67b3dd4129dab82f2751411ef16bef28dd3bb344"
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
Authorization: Bearer c008fbacc6a648c98998e902c5ffd5cbc31975b47b2b400e3d71a397b7092b6a
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
	-H "Authorization: Bearer c008fbacc6a648c98998e902c5ffd5cbc31975b47b2b400e3d71a397b7092b6a"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5fb6582628412b2a1bf1bf3b03ebf40c777292fd942b4e67fa37211062953d0b
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
    "id": 152,
    "updated_at": "2016-12-08T09:10:37.062Z",
    "course_id": 273,
    "author_id": 825,
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

    ],
    "title": "Preparing the oven",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fb6582628412b2a1bf1bf3b03ebf40c777292fd942b4e67fa37211062953d0b"
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
      "id": 163,
      "updated_at": "2016-12-08T09:10:38.419Z",
      "course_id": 280,
      "author_id": 850,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 148",
      "position": 1
    },
    {
      "id": 164,
      "updated_at": "2016-12-08T09:10:38.444Z",
      "course_id": 280,
      "author_id": 851,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 149",
      "position": 2
    },
    {
      "id": 165,
      "updated_at": "2016-12-08T09:10:38.668Z",
      "course_id": 280,
      "author_id": 852,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T09:10:38.346Z",
      "questions_updated_at": "2016-12-08T09:10:38.346Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 150",
      "position": 3
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
Authorization: Bearer bfd741167490b25a22faa7f112f58f79db91982742a7c1c1992ec15edbfb1d26
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
      "updated_at": "2016-12-08T09:10:39.053Z",
      "course_id": 283,
      "author_id": 861,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 154",
      "position": 1
    },
    {
      "id": 170,
      "updated_at": "2016-12-08T09:10:39.079Z",
      "course_id": 283,
      "author_id": 862,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 155",
      "position": 2
    },
    {
      "id": 171,
      "updated_at": "2016-12-08T09:10:39.303Z",
      "course_id": 283,
      "author_id": 863,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-12-08T09:10:38.979Z",
      "questions_updated_at": "2016-12-08T09:10:38.979Z",
      "flashcards_count": 0,
      "questions_count": 1,
      "title": "Clever Chapter Title 156",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfd741167490b25a22faa7f112f58f79db91982742a7c1c1992ec15edbfb1d26"
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
      "id": 166,
      "updated_at": "2016-12-08T09:10:38.795Z",
      "course_id": 281,
      "author_id": 856,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 151",
      "position": 1
    },
    {
      "id": 167,
      "updated_at": "2016-12-08T09:10:38.822Z",
      "course_id": 281,
      "author_id": 857,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 152",
      "position": 2
    },
    {
      "id": 168,
      "updated_at": "2016-12-08T09:10:38.847Z",
      "course_id": 281,
      "author_id": 858,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 153",
      "position": 3
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
Authorization: Bearer b7c9a2504004c2de8180d0de891012cc30c581fce8e2f8fb7cd26b13dcac6797
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
      "updated_at": "2016-12-08T09:10:39.479Z",
      "course_id": 284,
      "author_id": 868,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 157",
      "position": 1
    },
    {
      "id": 173,
      "updated_at": "2016-12-08T09:10:39.505Z",
      "course_id": 284,
      "author_id": 869,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 158",
      "position": 2
    },
    {
      "id": 174,
      "updated_at": "2016-12-08T09:10:39.533Z",
      "course_id": 284,
      "author_id": 870,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 159",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7c9a2504004c2de8180d0de891012cc30c581fce8e2f8fb7cd26b13dcac6797"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 624ac0f2043dbc9409fadf11e1e158b4ce40219f529f72b238964d3af70ee379
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
    "course_id": 57,
    "user_id": 211,
    "updated_at": "2016-12-08T09:09:51.935Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 624ac0f2043dbc9409fadf11e1e158b4ce40219f529f72b238964d3af70ee379"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 99a503daaa8b52db7231aff903954005a66f6439f23d09f248cdbebcfd4f2c3e
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
      "course_id": 62,
      "user_id": 223,
      "updated_at": "2016-12-08T09:09:52.588Z"
    },
    {
      "id": 6,
      "course_id": 62,
      "user_id": 224,
      "updated_at": "2016-12-08T09:09:52.605Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 99a503daaa8b52db7231aff903954005a66f6439f23d09f248cdbebcfd4f2c3e"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/40/files
Content-Type: application/json
Authorization: Bearer 5ee96b5d8823665da9927493f4eba1a5c4b38279b9257df153328d47a50a61af
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
      "id": 2,
      "uploader": {
        "id": 149,
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
        "created_at": "2016-12-08T09:09:45.759Z",
        "updated_at": "2016-12-08T09:09:45.759Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T09:09:45.773Z",
      "updated_at": "2016-12-08T09:09:45.773Z",
      "course_id": 40,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 150,
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
        "created_at": "2016-12-08T09:09:45.784Z",
        "updated_at": "2016-12-08T09:09:45.784Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T09:09:45.794Z",
      "updated_at": "2016-12-08T09:09:45.794Z",
      "course_id": 40,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    },
    {
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
        "created_at": "2016-12-08T09:09:45.805Z",
        "updated_at": "2016-12-08T09:09:45.805Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "up_votes_count": 0,
      "created_at": "2016-12-08T09:09:45.814Z",
      "updated_at": "2016-12-08T09:09:45.814Z",
      "course_id": 40,
      "filename": "example.pdf",
      "description": null,
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/40/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ee96b5d8823665da9927493f4eba1a5c4b38279b9257df153328d47a50a61af"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/39/files
Content-Type: application/json
Authorization: Bearer 989fd732f9edd9f63cf7c7621cba31178e1ddc6459ff9ca137df2ecb8f17430f
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
    "id": 1,
    "uploader": {
      "id": 147,
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
      "created_at": "2016-12-08T09:09:45.493Z",
      "updated_at": "2016-12-08T09:09:45.493Z"
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
    "created_at": "2016-12-08T09:09:45.553Z",
    "updated_at": "2016-12-08T09:09:45.553Z",
    "course_id": 39,
    "filename": "who you gonna call?",
    "description": "Leading paranormal research in Manhattan",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/39/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf","description":"Leading paranormal research in Manhattan  "}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 989fd732f9edd9f63cf7c7621cba31178e1ddc6459ff9ca137df2ecb8f17430f"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/38/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 4208ec0d14ab2b3a72e61130e3b7bb7c0f3be6b7656d79c8dce0d753ea2cb82d
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
    "key": "cache/7a9f61cb996d36f574891eb0f4d9003a.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxMDowOTo0NVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzdhOWY2MWNiOTk2ZDM2ZjU3NDg5MWViMGY0ZDkwMDNhLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsNTI0Mjg4MDBdLHsieC1hbXotY3JlZGVudGlhbCI6IkZBS0UvMjAxNjEyMDgvZXUtY2VudHJhbC0xL3MzL2F3czRfcmVxdWVzdCJ9LHsieC1hbXotYWxnb3JpdGhtIjoiQVdTNC1ITUFDLVNIQTI1NiJ9LHsieC1hbXotZGF0ZSI6IjIwMTYxMjA4VDA5MDk0NVoifV19",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T090945Z",
    "x-amz-signature": "39e223bd8b74399fde1d3904f5cb58e04ee7d7cd250c789c2d7fe711b142ecaf"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/38/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4208ec0d14ab2b3a72e61130e3b7bb7c0f3be6b7656d79c8dce0d753ea2cb82d"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 1b384c3bbbc52a38776e9d9d0d1562b9df65c479b07e8292c81bcc4ca67fed33
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
	-H "Authorization: Bearer 1b384c3bbbc52a38776e9d9d0d1562b9df65c479b07e8292c81bcc4ca67fed33"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 162c8ea59f6ceffe3a9df88684eefdf8f19b4bbcf0948a17b495169bc70e8843
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
	-H "Authorization: Bearer 162c8ea59f6ceffe3a9df88684eefdf8f19b4bbcf0948a17b495169bc70e8843"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 096a7aba45facdcf3ec625bed7d72961291564218c2d8596de1304239afb168b
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
	-H "Authorization: Bearer 096a7aba45facdcf3ec625bed7d72961291564218c2d8596de1304239afb168b"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 56ba7a0a965216adab751416f1a121018b8767ccde9357afaa46e499e7f000a3
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
	-H "Authorization: Bearer 56ba7a0a965216adab751416f1a121018b8767ccde9357afaa46e499e7f000a3"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b47f99c735b97ec5dba06f5df369a0a0f9c4dc8f276a780a6e18e2e0f47a14fe
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
	-H "Authorization: Bearer b47f99c735b97ec5dba06f5df369a0a0f9c4dc8f276a780a6e18e2e0f47a14fe"
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
    "creator_id": 10,
    "id": 2,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 2,
    "additional_university_ids": [

    ],
    "discipline_id": 5,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 2,
    "questions_count": 2,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T09:09:30.333Z",
    "updated_at": "2016-12-08T09:09:31.553Z",
    "shortname": "fu-choux-pastry-101",
    "questions": [
      {
        "id": 7,
        "obfuscated_id": "XFkue8saGAM",
        "author_id": 10,
        "chapter_id": 3,
        "position": 7,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:30.512Z",
        "created_at": "2016-12-08T09:09:30.424Z",
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
            "id": 13,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 14,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 10,
        "chapter_id": 4,
        "position": 9,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:30.819Z",
        "created_at": "2016-12-08T09:09:30.730Z",
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
      }
    ],
    "chapters": [
      {
        "id": 3,
        "updated_at": "2016-12-08T09:09:31.501Z",
        "course_id": 2,
        "author_id": 10,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T09:09:30.333Z",
        "questions_updated_at": "2016-12-08T09:09:30.333Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 3",
        "position": 1
      },
      {
        "id": 4,
        "updated_at": "2016-12-08T09:09:31.543Z",
        "course_id": 2,
        "author_id": 10,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T09:09:30.333Z",
        "questions_updated_at": "2016-12-08T09:09:30.333Z",
        "flashcards_count": 1,
        "questions_count": 1,
        "title": "Clever Chapter Title 4",
        "position": 2
      }
    ],
    "topic_id": 4,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": ""
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
Authorization: Bearer 12583c0a2621cf3d9796d528d0d3a04f5119ed541a7c3d233aabec6a76d8170a
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
    "creator_id": 15,
    "id": 3,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 3,
    "additional_university_ids": [

    ],
    "discipline_id": 6,
    "permissions": [

    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 4,
    "questions_count": 4,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T09:09:31.617Z",
    "updated_at": "2016-12-08T09:09:32.889Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 16,
        "chapter_id": 5,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.657Z",
        "created_at": "2016-12-08T09:09:32.657Z",
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
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 16,
        "chapter_id": 6,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.737Z",
        "created_at": "2016-12-08T09:09:32.737Z",
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
        "id": 14,
        "obfuscated_id": "gbKzjBR_8tw",
        "author_id": 16,
        "chapter_id": 5,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.702Z",
        "created_at": "2016-12-08T09:09:32.702Z",
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
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 16,
        "chapter_id": 6,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.782Z",
        "created_at": "2016-12-08T09:09:32.782Z",
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
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 16,
        "chapter_id": 5,
        "position": 13,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:31.806Z",
        "created_at": "2016-12-08T09:09:31.717Z",
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
        "author_id": 16,
        "chapter_id": 5,
        "position": 14,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:31.947Z",
        "created_at": "2016-12-08T09:09:31.866Z",
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
        "author_id": 16,
        "chapter_id": 6,
        "position": 15,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.132Z",
        "created_at": "2016-12-08T09:09:32.039Z",
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
      },
      {
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 16,
        "chapter_id": 6,
        "position": 16,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:32.278Z",
        "created_at": "2016-12-08T09:09:32.196Z",
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
      }
    ],
    "chapters": [
      {
        "id": 5,
        "updated_at": "2016-12-08T09:09:32.836Z",
        "course_id": 3,
        "author_id": 15,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T09:09:31.617Z",
        "questions_updated_at": "2016-12-08T09:09:31.617Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 5",
        "position": 1
      },
      {
        "id": 6,
        "updated_at": "2016-12-08T09:09:32.879Z",
        "course_id": 3,
        "author_id": 15,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-12-08T09:09:31.617Z",
        "questions_updated_at": "2016-12-08T09:09:31.617Z",
        "flashcards_count": 2,
        "questions_count": 2,
        "title": "Clever Chapter Title 6",
        "position": 2
      }
    ],
    "topic_id": 5,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12583c0a2621cf3d9796d528d0d3a04f5119ed541a7c3d233aabec6a76d8170a"
```
## Pin a course


### Request

#### Endpoint

```
PUT /v2/courses/10/pin
Content-Type: application/json
Authorization: Bearer 1d9e4b08e38a369637bba29f3928932a350b3b13a4e7ebea95e7ec0d2982fdfb
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/10/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d9e4b08e38a369637bba29f3928932a350b3b13a4e7ebea95e7ec0d2982fdfb"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/9/pin
Content-Type: application/json
Authorization: Bearer 1219efa4989f3200a6cb88667a52b5196377bec76d18b605c2f17060745fcab7
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/9/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1219efa4989f3200a6cb88667a52b5196377bec76d18b605c2f17060745fcab7"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e27d25a7a47eecbd7c03bf979ee414b17fa84dc238dd9edc3d19aa04037fdf31
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
    "creator_id": 31,
    "id": 7,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 7,
    "additional_university_ids": [

    ],
    "discipline_id": 10,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-08T09:09:34.894Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 9,
    "language_code": "fr",
    "exam_months": [

    ],
    "title": "Choux pastry 102",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e27d25a7a47eecbd7c03bf979ee414b17fa84dc238dd9edc3d19aa04037fdf31"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer bd5d38ae3f10e7d12af114e599c1d5f322276e804188e1782a884692d8bb7d7e
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
    "id": 678,
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
    "created_at": "2016-12-08T09:10:24.123Z",
    "updated_at": "2016-12-08T09:10:24.123Z",
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
	-H "Authorization: Bearer bd5d38ae3f10e7d12af114e599c1d5f322276e804188e1782a884692d8bb7d7e"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 6aea807c1c1a66c167fd7b35cb03486bfdb743e00d7c0cd57018e0924875444a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[235]}
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
    "id": 673,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      235
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T09:10:23.450Z",
    "updated_at": "2016-12-08T09:10:23.503Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[235]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6aea807c1c1a66c167fd7b35cb03486bfdb743e00d7c0cd57018e0924875444a"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a27c169bcfecaab7685809eb77c2ba999340e4df3f05da4de200a07628880da0
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
    "id": 676,
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
    "created_at": "2016-12-08T09:10:23.699Z",
    "updated_at": "2016-12-08T09:10:23.699Z",
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
	-H "Authorization: Bearer a27c169bcfecaab7685809eb77c2ba999340e4df3f05da4de200a07628880da0"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 7d2e7be32325661e669e9dd9c1c23f382bf4392103ee556e10064674f4733c9f
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[237]}
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
    "id": 675,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      237
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T09:10:23.634Z",
    "updated_at": "2016-12-08T09:10:23.634Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[237]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d2e7be32325661e669e9dd9c1c23f382bf4392103ee556e10064674f4733c9f"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer ea76c1548c022737de8d4b0b8d4372a7abc86402844678d4eb36a9fbd980801b
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

239
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
    "id": 677,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/26c1c6aad08f4832304a03dcef626e68dbeb9c1e.jpg",
    "university_id": null,
    "fields_of_study": [
      239
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-12-08T09:10:23.797Z",
    "updated_at": "2016-12-08T09:10:24.087Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/02a3da55382cfbe222a872a15b622bdf978f049e.jpg",
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

239
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer ea76c1548c022737de8d4b0b8d4372a7abc86402844678d4eb36a9fbd980801b"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 55e8834caf964a03d8609b5b1db49896e1fa2afc631dc2f5e207e6afea1f7d6c
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
      "bookmarkable_id": 89,
      "bookmarkable_type": "Question"
    },
    {
      "id": 3,
      "bookmarkable_id": 90,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 91,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55e8834caf964a03d8609b5b1db49896e1fa2afc631dc2f5e207e6afea1f7d6c"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer abd7ae5f41bc273216581847c998e3671aaceca0ebb0419b78bb09c5e0e438c6
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
      "company_id": 15,
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
      "id": 3,
      "title": "Campaign 3",
      "company_id": 16,
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
	-H "Authorization: Bearer abd7ae5f41bc273216581847c998e3671aaceca0ebb0419b78bb09c5e0e438c6"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 897166938e22c64b7aa921dee8beb50cd1718b879d95f72292b78fdefc4ff3b5
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
      "company_id": 11,
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
	-H "Authorization: Bearer 897166938e22c64b7aa921dee8beb50cd1718b879d95f72292b78fdefc4ff3b5"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 9b85c3cf3f45d310ec3fe3c88d97bb77e16a10844208504786d9483d3d59c76e
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
      "creator_id": 60,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-5",
      "html_url": "https://goskive.com/course/mit-course-5",
      "slug": "mit-course-5",
      "university_id": 20,
      "additional_university_ids": [

      ],
      "discipline_id": 23,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:37.152Z",
      "shortname": "mit-course-5",
      "topic_id": 22,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 61,
      "id": 21,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-6",
      "html_url": "https://goskive.com/course/mit-course-6",
      "slug": "mit-course-6",
      "university_id": 21,
      "additional_university_ids": [

      ],
      "discipline_id": 24,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:37.255Z",
      "shortname": "mit-course-6",
      "topic_id": 23,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b85c3cf3f45d310ec3fe3c88d97bb77e16a10844208504786d9483d3d59c76e"
```
# Current user Files

## Get the files for the user


### Request

#### Endpoint

```
GET /v2/me/files
Content-Type: application/json
Authorization: Bearer 37b410f8a10e49c0f05667a249c1c30e79127fe5212dae3d264fa53577190e35
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
        "id": 20,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [
          "update",
          "delete"
        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T09:10:47.058Z",
        "updated_at": "2016-12-08T09:10:47.058Z",
        "file_url": "memory://505fa7de59d6bc90320afb3889e05626.pdf",
        "course_id": 314,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "downloaded_files": [
      {
        "id": 21,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T09:10:47.138Z",
        "updated_at": "2016-12-08T09:10:47.138Z",
        "file_url": "memory://8dd687b171a4ffd4e9e59817446bee9a.pdf",
        "course_id": 315,
        "filename": "example.pdf",
        "description": null,
        "category": "summary",
        "is_anonymous": false
      }
    ],
    "bookmarked_files": [
      {
        "id": 22,
        "status": "published",
        "download_count": 3000,
        "mime_type": "application/pdf",
        "size": 6893,
        "permissions": [

        ],
        "up_votes_count": 0,
        "created_at": "2016-12-08T09:10:47.218Z",
        "updated_at": "2016-12-08T09:10:47.218Z",
        "file_url": "memory://8b9afcaf321c5c36b6189be92ce04db8.pdf",
        "course_id": 316,
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
	-H "Authorization: Bearer 37b410f8a10e49c0f05667a249c1c30e79127fe5212dae3d264fa53577190e35"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 2c9004317f3ec9be2409fbb3a621f8cf88bbcc2570acad30382308bd5b66d757
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
      "company_id": 37,
      "company": {
        "id": 37,
        "name": "Fake Company Name 32",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/98d5a5c73380c272e4c1b11473e40b72ea5dea93.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T09:10:39.968Z"
      },
      "created_at": "2016-12-08T09:10:39.972Z",
      "updated_at": "2016-12-08T09:10:39.972Z",
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
      "company_id": 38,
      "company": {
        "id": 38,
        "name": "Fake Company Name 33",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/7d3f3878a696ff46f0886dffefc58ca7a2291295.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T09:10:39.981Z"
      },
      "created_at": "2016-12-08T09:10:39.984Z",
      "updated_at": "2016-12-08T09:10:39.984Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c9004317f3ec9be2409fbb3a621f8cf88bbcc2570acad30382308bd5b66d757"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer a85d4bf274aba8489364b093394816ec07c527a479ddc841f16825fc09501616
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
      "company_id": 33,
      "company": {
        "id": 33,
        "name": "Fake Company Name 28",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/93e1f192fbc483546cf4e043b0cd470b38fdf1a9.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T09:10:39.760Z"
      },
      "created_at": "2016-12-08T09:10:39.764Z",
      "updated_at": "2016-12-08T09:10:39.764Z",
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
      "company_id": 34,
      "company": {
        "id": 34,
        "name": "Fake Company Name 29",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/1da6e1ffe4381f9fbc4cfbd9951d35edeab29202.png",
        "brand_color": "#000000",
        "updated_at": "2016-12-08T09:10:39.782Z"
      },
      "created_at": "2016-12-08T09:10:39.786Z",
      "updated_at": "2016-12-08T09:10:39.786Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a85d4bf274aba8489364b093394816ec07c527a479ddc841f16825fc09501616"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer e4c464e70d8d526e3a24730ee8c086e5f22380b9133a10985c542018d98778c9
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
      "id": 5,
      "created_at": "2016-12-08T09:09:46.087Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 7,
      "updated_at": "2016-12-08T09:09:46.193Z",
      "author_id": "157",
      "thread_subject_id": "42",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 6,
      "created_at": "2016-12-08T09:09:46.182Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 8,
      "updated_at": "2016-12-08T09:09:46.196Z",
      "author_id": "160",
      "thread_subject_id": "43",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 7,
      "created_at": "2016-12-08T09:09:46.598Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 4,
      "updated_at": "2016-12-08T09:09:46.598Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 8,
      "created_at": "2016-12-08T09:09:46.971Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 5,
      "updated_at": "2016-12-08T09:09:46.971Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 9,
      "created_at": "2016-12-08T09:09:47.358Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 6,
      "updated_at": "2016-12-08T09:09:47.358Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 10,
      "created_at": "2016-12-08T09:09:47.644Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 46,
      "updated_at": "2016-12-08T09:09:47.644Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 11,
      "created_at": "2016-12-08T09:09:47.940Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 47,
      "updated_at": "2016-12-08T09:09:47.940Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 12,
      "created_at": "2016-12-08T09:09:48.218Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 48,
      "updated_at": "2016-12-08T09:09:48.218Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e4c464e70d8d526e3a24730ee8c086e5f22380b9133a10985c542018d98778c9"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/13
Content-Type: application/json
Authorization: Bearer 418081abef1af247c6330eabfa6fc86c680219241eec2ee6497c305b5c084782
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-12-08T08:59:48.000Z"}}
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
    "id": 13,
    "created_at": "2016-12-08T09:09:48.416Z",
    "read_at": "2016-12-08T08:59:48.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 9,
    "updated_at": "2016-12-08T09:09:48.458Z",
    "author_id": "186",
    "thread_subject_id": "50",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/13" -d '{"notification":{"read_at":"2016-12-08T08:59:48.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 418081abef1af247c6330eabfa6fc86c680219241eec2ee6497c305b5c084782"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 28805b4afad8646f7bd6efa92ffdb839397257dec26dcdb38593066086075384
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
      "course_id": 289,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T09:10:40.787Z",
      "course_published": true,
      "updated_at": "2016-12-08T09:10:40.782Z"
    },
    {
      "id": 7,
      "course_id": 290,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-12-08T09:10:40.865Z",
      "course_published": true,
      "updated_at": "2016-12-08T09:10:40.860Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28805b4afad8646f7bd6efa92ffdb839397257dec26dcdb38593066086075384"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/4
Content-Type: application/json
Authorization: Bearer 7df5074304e74d8c0f1010963ece774fb801baff8ce7b82b1ad1c481e6a65530
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
    "course_id": 287,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-12-08T09:10:40.504Z",
    "course_published": true,
    "updated_at": "2016-12-08T09:10:40.499Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/4" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7df5074304e74d8c0f1010963ece774fb801baff8ce7b82b1ad1c481e6a65530"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer c8b1c101a73e2c85f180d16bb96186bb10d6c2fc726e071dc3ab6c3b8edfd4f3
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
    "course_id": 288,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-12-08T09:10:40.688Z",
    "course_published": true,
    "updated_at": "2016-12-08T09:10:40.680Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8b1c101a73e2c85f180d16bb96186bb10d6c2fc726e071dc3ab6c3b8edfd4f3"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer ab13dfbb1d77c5f6eabd651cc1e09ee2df5025d8cc7a3bb1197f9fc4f36404dc
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
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 92,
      "user_id": 630
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 93,
      "user_id": 630
    },
    {
      "id": 11,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 94,
      "user_id": 630
    },
    {
      "id": 12,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 95,
      "user_id": 630
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab13dfbb1d77c5f6eabd651cc1e09ee2df5025d8cc7a3bb1197f9fc4f36404dc"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/1
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
    "id": 1,
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
        "discipline_id": 1
      },
      {
        "id": 2,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 1
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/1" -X GET \
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
      "id": 2,
      "name": "Reactive attitude-oriented instruction set",
      "name_translations": {
        "en": "Reactive attitude-oriented instruction set"
      }
    },
    {
      "id": 3,
      "name": "Seamless multi-tasking secured line",
      "name_translations": {
        "en": "Seamless multi-tasking secured line"
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
PATCH /v2/feedbacks/12/close
Content-Type: application/json
Authorization: Bearer 746fc3769fb206c143ac62a904214b672890f7126593ec870fedb82bae9d420a
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
    "id": 12,
    "user_id": 317,
    "feedbackable_id": 37,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-12-08T09:10:00.598Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/12/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 746fc3769fb206c143ac62a904214b672890f7126593ec870fedb82bae9d420a"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/35/fix
Content-Type: application/json
Authorization: Bearer a5a53118e597b9b3868919080468a5de26da97f08b68e91eb19be74e783c62ed
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
    "id": 35,
    "user_id": 418,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-12-08T09:10:07.654Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/35/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a5a53118e597b9b3868919080468a5de26da97f08b68e91eb19be74e783c62ed"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/10
Content-Type: application/json
Authorization: Bearer 20007ff8e7eee60321c558a411464745e4f5f0bad3d7739d459bf007a76d3665
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
    "id": 10,
    "user_id": 305,
    "feedbackable_id": 35,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T09:10:00.061Z",
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
curl "api.goskive.com/v2/feedbacks/10" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 20007ff8e7eee60321c558a411464745e4f5f0bad3d7739d459bf007a76d3665"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/14/close
Content-Type: application/json
Authorization: Bearer b0e8e5f5664ffbb5b7be73c5270dc20196846c85fd69e25b5183a5defa444b33
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
curl "api.goskive.com/v2/feedbacks/14/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b0e8e5f5664ffbb5b7be73c5270dc20196846c85fd69e25b5183a5defa444b33"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/34/fix
Content-Type: application/json
Authorization: Bearer ed0f9e11e7eb09417b24b7c641bab9b514570c90f030e95fcf1950fee1882692
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
curl "api.goskive.com/v2/feedbacks/34/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed0f9e11e7eb09417b24b7c641bab9b514570c90f030e95fcf1950fee1882692"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/37/fix
Content-Type: application/json
Authorization: Bearer 8cd949d95b41b987ec2d70fba8d638b143a9e00f712242b9acb785411c5923df
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
curl "api.goskive.com/v2/feedbacks/37/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cd949d95b41b987ec2d70fba8d638b143a9e00f712242b9acb785411c5923df"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/11
Content-Type: application/json
Authorization: Bearer d60f3d8135ac2ccb396e0975e04dfdc928ac8914a9782d2590608643f6962874
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
    "id": 11,
    "user_id": 310,
    "feedbackable_id": 36,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T09:10:00.358Z",
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
curl "api.goskive.com/v2/feedbacks/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d60f3d8135ac2ccb396e0975e04dfdc928ac8914a9782d2590608643f6962874"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 8e613f84b434800b22dc21f6edcdbbd16f91142f971ef225f57bc343ecd08381
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
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e613f84b434800b22dc21f6edcdbbd16f91142f971ef225f57bc343ecd08381"
```
## Bookmark a file


### Request

#### Endpoint

```
PUT /v2/files/16/bookmark
Content-Type: application/json
Authorization: Bearer 3eb56a958ea2f5072a6fd85e9fe6684626e17b00dd9faa1df3c047b3bab669cf
```

`PUT /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3eb56a958ea2f5072a6fd85e9fe6684626e17b00dd9faa1df3c047b3bab669cf"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Content-Type: application/json
Authorization: Bearer e1433fdff63a71001ba6b2e07f76fa0fd19877ff1b4fdd633b52d5c0719deb8a
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
	-H "Authorization: Bearer e1433fdff63a71001ba6b2e07f76fa0fd19877ff1b4fdd633b52d5c0719deb8a"
```
## Get a file download link


### Request

#### Endpoint

```
GET /v2/files/7
Content-Type: application/json
Authorization: Bearer 1aee42934c9e4a39dc1cdcb1f491974d53e5ff7091876fcc1d47f231db79cff0
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/8bda00e6870246f901b2a3c3ad1f097e.pdf?response-content-disposition=attachment%3B%20filename%3D%22example.pdf%22&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T091024Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=784017ff4a78a397dd07f031023f756a660b634a133a0aecaea03d9ffae2ca9c",
    "expires_in": 86400
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
	-H "Authorization: Bearer 1aee42934c9e4a39dc1cdcb1f491974d53e5ff7091876fcc1d47f231db79cff0"
```
## Get a file inline preview link


### Request

#### Endpoint

```
GET /v2/files/8/preview
Content-Type: application/json
Authorization: Bearer af7c3026d460e1718200d057c1066e49027aa42fa5e65a4797f316a1d5186501
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
    "location": "https://s3.eu-central-1.amazonaws.com/upload.goskive.com/cache/d6e5f01847f225be33296b37c40a6084.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=FAKE%2F20161208%2Feu-central-1%2Fs3%2Faws4_request&X-Amz-Date=20161208T091024Z&X-Amz-Expires=86400&X-Amz-SignedHeaders=host&X-Amz-Signature=059495ceed76c6665973473ef2d47866d45fca66662b657be99665f0c33f632f",
    "expires_in": 86400
  }
}
```



#### Fields

| Name       | Description         |
|:-----------|:--------------------|
| file_link[location] | Location URL |


```shell
curl "api.goskive.com/v2/files/8/preview" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af7c3026d460e1718200d057c1066e49027aa42fa5e65a4797f316a1d5186501"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/18/metadata
Content-Type: application/json
Authorization: Bearer c4d2a267d3e8d451c077d83a97cf430ef3d275b7b338b9e02275d45f8eb484de
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
    "id": 18,
    "uploader": {
      "id": 714,
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
      "created_at": "2016-12-08T09:10:26.120Z",
      "updated_at": "2016-12-08T09:10:26.120Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "up_votes_count": 0,
    "created_at": "2016-12-08T09:10:26.193Z",
    "updated_at": "2016-12-08T09:10:26.193Z",
    "course_id": 240,
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
curl "api.goskive.com/v2/files/18/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4d2a267d3e8d451c077d83a97cf430ef3d275b7b338b9e02275d45f8eb484de"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/6/matched_courses?required_cu_count=2
Authorization: Bearer 21d2e5718be0d695734ca0c4878205b5e39915e0c244f06a39bc19fbeabc48ea
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
      "creator_id": 289,
      "id": 110,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 95,
      "additional_university_ids": [

      ],
      "discipline_id": 118,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T09:09:57.599Z",
      "updated_at": "2016-12-08T09:09:59.206Z",
      "shortname": "mit-the-great-british-bake-off",
      "topic_id": 117,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 294,
      "id": 111,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-c9c92ca1-bdea-4feb-8cb1-d16397330ce8",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-c9c92ca1-bdea-4feb-8cb1-d16397330ce8",
      "slug": "mit-the-great-british-bake-off-c9c92ca1-bdea-4feb-8cb1-d16397330ce8",
      "university_id": 96,
      "additional_university_ids": [

      ],
      "discipline_id": 119,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
      "questions_count": 2,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T09:09:57.599Z",
      "updated_at": "2016-12-08T09:09:59.747Z",
      "shortname": "mit-the-great-british-bake-off-c9c92ca1-bdea-4feb-8cb1-d16397330ce8",
      "topic_id": 118,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "The Great British Bake Off",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/6/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 21d2e5718be0d695734ca0c4878205b5e39915e0c244f06a39bc19fbeabc48ea"
```
## Notify of a download of a file


### Request

#### Endpoint

```
PUT /v2/files/15/download
Content-Type: application/json
Authorization: Bearer 9889d8733f41008366b39281fcee62d3151c8dc87ef3e781e40f7435afe6f330
```

`PUT /v2/files/:file_id/download`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15/download" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9889d8733f41008366b39281fcee62d3151c8dc87ef3e781e40f7435afe6f330"
```
## Report a file


### Request

#### Endpoint

```
PUT /v2/files/14/report
Content-Type: application/json
Authorization: Bearer c146759d55bda3c06182f2eff4c16122ff6cd00e018e8d848467b95d8b1e0e34
```

`PUT /v2/files/:file_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c146759d55bda3c06182f2eff4c16122ff6cd00e018e8d848467b95d8b1e0e34"
```
## Unbookmark a file


### Request

#### Endpoint

```
DELETE /v2/files/9/bookmark
Content-Type: application/json
Authorization: Bearer 8f7b7a0a96c8f3638ff4889bca75349c5e30c764eac070b1b71502fdfc815a37
```

`DELETE /v2/files/:file_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/9/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8f7b7a0a96c8f3638ff4889bca75349c5e30c764eac070b1b71502fdfc815a37"
```
## Upvote a file


### Request

#### Endpoint

```
PUT /v2/files/13/upvote
Content-Type: application/json
Authorization: Bearer dcd050518f58f8537e81ecdf153fadc3059050b10782ccf4ec239a7e4459c643
```

`PUT /v2/files/:file_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcd050518f58f8537e81ecdf153fadc3059050b10782ccf4ec239a7e4459c643"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/71/comments
Content-Type: application/json
Authorization: Bearer 7b5863d188145976a6d4f8f2c085ce4754a20ec447f97ed5009012670c65e7d9
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
    "author_id": 656,
    "reply_to_id": null,
    "created_at": "2016-12-08T09:10:22.275Z",
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
curl "api.goskive.com/v2/flashcards/71/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b5863d188145976a6d4f8f2c085ce4754a20ec447f97ed5009012670c65e7d9"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/72/comments
Content-Type: application/json
Authorization: Bearer d5b714980795ec936ff842bf4505bbb5fb44fe1515712a040133996c36baeed3
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
    "id": 56,
    "author_id": 659,
    "reply_to_id": null,
    "created_at": "2016-12-08T09:10:22.633Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 38,
      "user_id": 659,
      "feedbackable_id": 72,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:22.630Z",
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
curl "api.goskive.com/v2/flashcards/72/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5b714980795ec936ff842bf4505bbb5fb44fe1515712a040133996c36baeed3"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/75/comments
Content-Type: application/json
Authorization: Bearer fd2d959a837605a6728dbb2c9a2af3e66c57f956055de507f93503986159f347
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
      "id": 58,
      "author_id": 672,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:23.380Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 671,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:23.363Z",
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
curl "api.goskive.com/v2/flashcards/75/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fd2d959a837605a6728dbb2c9a2af3e66c57f956055de507f93503986159f347"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/73/comments
Content-Type: application/json
Authorization: Bearer 2108bbfb7f03416281988bc1b4c85877114d322f7b6eca65a79eee46ba6ed08b
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
curl "api.goskive.com/v2/flashcards/73/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2108bbfb7f03416281988bc1b4c85877114d322f7b6eca65a79eee46ba6ed08b"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/85/feedbacks
Content-Type: application/json
Authorization: Bearer 5afcda8eed636ebc9b435cafc1295cb2cc7cac5ea104ddaebae8df8d6c745ec0
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
    "user_id": 895,
    "feedbackable_id": 85,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-12-08T09:10:41.706Z",
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
curl "api.goskive.com/v2/flashcards/85/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5afcda8eed636ebc9b435cafc1295cb2cc7cac5ea104ddaebae8df8d6c745ec0"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/91/feedbacks
Content-Type: application/json
Authorization: Bearer 0c2a8c3a90dabd63e173bbcffde42d44083a7da33567c7ee70a2c2861363865e
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
      "user_id": 927,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:43.071Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 926,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:43.060Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0c2a8c3a90dabd63e173bbcffde42d44083a7da33567c7ee70a2c2861363865e"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/68/votes
Content-Type: application/json
Authorization: Bearer 38bd578938ccca66a7d16661b84886e819d51c860a4b8027f562e42b096d4df9
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
      "id": 15,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 648
    },
    {
      "id": 14,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 647
    },
    {
      "id": 13,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 68,
      "user_id": 646
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/68/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38bd578938ccca66a7d16661b84886e819d51c860a4b8027f562e42b096d4df9"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/44/republish
Content-Type: application/json
Authorization: Bearer d118097a4c707f7f63701b9811a75cfbc5e4fc29114b294587b83389ed5d4fae
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
curl "api.goskive.com/v2/flashcards/44/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d118097a4c707f7f63701b9811a75cfbc5e4fc29114b294587b83389ed5d4fae"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/67/bookmark
Content-Type: application/json
Authorization: Bearer ebe75d9c868ac9bcf908b79bfba0643cdf6f4e3e36da1167c67a8817cddf2215
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/67/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebe75d9c868ac9bcf908b79bfba0643cdf6f4e3e36da1167c67a8817cddf2215"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/50
Content-Type: application/json
Authorization: Bearer 0cf594e4ed1d9ace3732ea8f1229f0790f1b5e055c83dc15a1cddc40b554a872
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
	-H "Authorization: Bearer 0cf594e4ed1d9ace3732ea8f1229f0790f1b5e055c83dc15a1cddc40b554a872"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/47/downvote
Content-Type: application/json
Authorization: Bearer b681e6c5b77b86143c34400eacf40c03577e834c0b8ced8ea7a1c1dffe43bcae
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/47/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b681e6c5b77b86143c34400eacf40c03577e834c0b8ced8ea7a1c1dffe43bcae"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/66
Content-Type: application/json
Authorization: Bearer 6bdc8d901d38d8423a1da76a5d8d504f38974469afcad96960abfb362f63c080
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 501,
    "chapter_id": 102,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:10:12.749Z",
    "created_at": "2016-12-08T09:10:12.749Z",
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
curl "api.goskive.com/v2/flashcards/66" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6bdc8d901d38d8423a1da76a5d8d504f38974469afcad96960abfb362f63c080"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/49/report
Content-Type: application/json
Authorization: Bearer 55576b1f78e25bd4ee965c2857d2ea9b2433e5974b2971d7ce850944934c42d1
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/49/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55576b1f78e25bd4ee965c2857d2ea9b2433e5974b2971d7ce850944934c42d1"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/46/bookmark
Content-Type: application/json
Authorization: Bearer 2fb8e9de322cd1d4789cde56784735423a92b9bae7d71c7f5180f722db67f7a3
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/46/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2fb8e9de322cd1d4789cde56784735423a92b9bae7d71c7f5180f722db67f7a3"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/48/upvote
Content-Type: application/json
Authorization: Bearer 5280d13143263fe6234142277c0e368524327243386968b47f75769c2be27cb6
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/48/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5280d13143263fe6234142277c0e368524327243386968b47f75769c2be27cb6"
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
    "key": "cache/34d5c4e3fc4a098bc40adf4079c7811b.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMi0wOFQxMDowOTozOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJ1cGxvYWQuZ29za2l2ZS5jb20ifSx7ImtleSI6ImNhY2hlLzM0ZDVjNGUzZmM0YTA5OGJjNDBhZGY0MDc5Yzc4MTFiLmpwZyJ9LFsiY29udGVudC1sZW5ndGgtcmFuZ2UiLDAsMjA5NzE1Ml0seyJ4LWFtei1jcmVkZW50aWFsIjoiRkFLRS8yMDE2MTIwOC9ldS1jZW50cmFsLTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEyMDhUMDkwOTM5WiJ9XX0=",
    "x-amz-credential": "FAKE/20161208/eu-central-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161208T090939Z",
    "x-amz-signature": "0a6326b23b34a3a9806f0f3a207862a91f98aa8c3192e555d6b769ad62638b8e"
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
Authorization: Bearer 377eb0b98f27636db50f944d2139068b6983028cb8becd7acb411f32a1463b19
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
	-H "Authorization: Bearer 377eb0b98f27636db50f944d2139068b6983028cb8becd7acb411f32a1463b19"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer 916a98306ebadbeb692b063cac3a5f53816203ac25518f7344f07ea78d5b883f
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
	-H "Authorization: Bearer 916a98306ebadbeb692b063cac3a5f53816203ac25518f7344f07ea78d5b883f"
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
{"password":{"reset_password_token":"Rosjjm5EUuKmzWUukWVW","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 818,
  "email": "jan.turnosky@hotmail.sk",
  "phone_number_country_code": null,
  "phone_number": null,
  "avatar_file_name": null,
  "avatar_content_type": null,
  "university_id": null,
  "study_level": null,
  "created_at": "2016-12-08T09:10:36.524Z",
  "updated_at": "2016-12-08T09:10:36.683Z",
  "company_id": null,
  "first_name": "Kasper",
  "last_name": "Skive",
  "deleted_at": null,
  "purchases_count": 0,
  "receipts_count": 0,
  "devices_count": 0,
  "nickname": null,
  "locale": "en",
  "avatar_file_size": null,
  "avatar_updated_at": null,
  "properties": {
  },
  "last_api_access_at": null,
  "subbrand_id": 0,
  "graduation_year": null,
  "audit_id": 8698
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"Rosjjm5EUuKmzWUukWVW","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Content-Type: application/json
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
Content-Type: application/json
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
POST /v2/questions/38/comments
Content-Type: application/json
Authorization: Bearer 8b68d7a60e7f8bbb5ed9e6a52b9aa8ad02767aff1fc11b31ac5428ebcb80fbf0
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
    "author_id": 127,
    "reply_to_id": null,
    "created_at": "2016-12-08T09:09:43.737Z",
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
curl "api.goskive.com/v2/questions/38/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b68d7a60e7f8bbb5ed9e6a52b9aa8ad02767aff1fc11b31ac5428ebcb80fbf0"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/39/comments
Content-Type: application/json
Authorization: Bearer 0bfd23a755bc1cdd7a7924e64e8f631b1a8c727556e8da3c1eec360990296e9a
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
    "author_id": 130,
    "reply_to_id": null,
    "created_at": "2016-12-08T09:09:44.207Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 9,
      "user_id": 130,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:09:44.204Z",
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
curl "api.goskive.com/v2/questions/39/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bfd23a755bc1cdd7a7924e64e8f631b1a8c727556e8da3c1eec360990296e9a"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/42/comments
Content-Type: application/json
Authorization: Bearer 460c22606341b661aa23d29dab5b6ad3d98b9b97eeb3803d7bce07f642155321
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
      "author_id": 142,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:09:45.264Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 143,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:09:45.282Z",
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
curl "api.goskive.com/v2/questions/42/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 460c22606341b661aa23d29dab5b6ad3d98b9b97eeb3803d7bce07f642155321"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/40/comments
Content-Type: application/json
Authorization: Bearer e41ec00e17c592d79694dfdc63462e4ffa7f1c66b99ae8b2eef2a3c5d92b67cf
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
curl "api.goskive.com/v2/questions/40/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e41ec00e17c592d79694dfdc63462e4ffa7f1c66b99ae8b2eef2a3c5d92b67cf"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/37/feedbacks
Content-Type: application/json
Authorization: Bearer d49af48288c8080e29e1fd3b3d421fb147642b9293859345ece490ef8cbbd7e3
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
    "user_id": 117,
    "feedbackable_id": 37,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-12-08T09:09:42.349Z",
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
curl "api.goskive.com/v2/questions/37/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d49af48288c8080e29e1fd3b3d421fb147642b9293859345ece490ef8cbbd7e3"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/30/feedbacks
Content-Type: application/json
Authorization: Bearer 42f17f4e84473a947f4e916560d7445b886365447130511478b415d4621281d9
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
      "id": 2,
      "user_id": 88,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:09:39.826Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 1,
      "user_id": 87,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:09:39.814Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/30/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42f17f4e84473a947f4e916560d7445b886365447130511478b415d4621281d9"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/128/votes
Content-Type: application/json
Authorization: Bearer 0b133819d808a46a630c2772ef8c5a9749422419411be16551c5b4678c1f153d
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
      "id": 23,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 939
    },
    {
      "id": 22,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 938
    },
    {
      "id": 21,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 128,
      "user_id": 937
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/128/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b133819d808a46a630c2772ef8c5a9749422419411be16551c5b4678c1f153d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/100/republish
Content-Type: application/json
Authorization: Bearer dc87b05e9e6624a7d69e7a4b4527c06272d217546db8d78a7e70e964dcdf4fbf
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
curl "api.goskive.com/v2/questions/100/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc87b05e9e6624a7d69e7a4b4527c06272d217546db8d78a7e70e964dcdf4fbf"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/121/bookmark
Content-Type: application/json
Authorization: Bearer 5799cf98acea6163bb4251c18c99082e08ab21cd400dbe10165028828b75cca4
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/121/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5799cf98acea6163bb4251c18c99082e08ab21cd400dbe10165028828b75cca4"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/98
Content-Type: application/json
Authorization: Bearer cb04527c0e8e29a692105da5c04651d778ab3f0a5351eb9210f4975378a3a389
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/98" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb04527c0e8e29a692105da5c04651d778ab3f0a5351eb9210f4975378a3a389"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/120/downvote
Content-Type: application/json
Authorization: Bearer 57be8fc43bda0c9e2161e2320216ba1506096fee59c5896ea1d46ee35a40a9af
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/120/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57be8fc43bda0c9e2161e2320216ba1506096fee59c5896ea1d46ee35a40a9af"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/101
Content-Type: application/json
Authorization: Bearer 3f9592bbada68d1363aaf158e3f4c77aa4f58b1f8e96a46e8253aa7b0278d911
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
    "id": 101,
    "obfuscated_id": "PprZyBVq_gc",
    "author_id": 744,
    "chapter_id": 130,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:10:29.019Z",
    "created_at": "2016-12-08T09:10:28.934Z",
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
        "id": 204,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 205,
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
curl "api.goskive.com/v2/questions/101" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f9592bbada68d1363aaf158e3f4c77aa4f58b1f8e96a46e8253aa7b0278d911"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/97/report
Content-Type: application/json
Authorization: Bearer fe1db7b9ec5294c49ec99f36e12a46b32fb8533ba1b09cedb211b9dbd9d81597
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/97/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe1db7b9ec5294c49ec99f36e12a46b32fb8533ba1b09cedb211b9dbd9d81597"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/102/bookmark
Content-Type: application/json
Authorization: Bearer 899a1e7b2baf5d345ce823ba4eed4ef80c3c701ca272e109680958ac72d5077f
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/102/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 899a1e7b2baf5d345ce823ba4eed4ef80c3c701ca272e109680958ac72d5077f"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/119
Content-Type: application/json
Authorization: Bearer cfd283a20d14e4f4f59bc7d15079cc3c493d6cebdc015796d2d6dc85258783e8
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":119,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T09:10:33.686Z","updated_at":"2016-12-08T09:10:33.773Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":148,"author_id":803,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 119,
    "obfuscated_id": "JRh8sWka24Y",
    "author_id": 803,
    "chapter_id": 148,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-12-08T09:10:33.865Z",
    "created_at": "2016-12-08T09:10:33.686Z",
    "tags": [

    ],
    "status": "published",
    "published": true,
    "language_code": "de",
    "question": "#<ActionController::Parameters:0x00000004eb86e8>",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 240,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 241,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 242,
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
curl "api.goskive.com/v2/questions/119" -d '{"question":{"question":{"id":119,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-12-08T09:10:33.686Z","updated_at":"2016-12-08T09:10:33.773Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":148,"author_id":803,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfd283a20d14e4f4f59bc7d15079cc3c493d6cebdc015796d2d6dc85258783e8"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/118/upvote
Content-Type: application/json
Authorization: Bearer b4e5c72163283e59809545bd67f44cd736f6ac4ce01fa956fdcef3999b78a60b
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/118/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4e5c72163283e59809545bd67f44cd736f6ac4ce01fa956fdcef3999b78a60b"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 578b65611137183df0f16bcd7233629ec55f7a405c0dc7b2f0b0674e5a2706ec
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
      "creator_id": 228,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 72,
      "additional_university_ids": [

      ],
      "discipline_id": 72,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:52.929Z",
      "shortname": "mit-pizza-201",
      "topic_id": 71,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Pizza 201",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 578b65611137183df0f16bcd7233629ec55f7a405c0dc7b2f0b0674e5a2706ec"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer d02981532fc0c85dfc9ed9a612253a87bda5686b85276b8a1b75808c6b2fe399
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
      "id": 70,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-68",
      "html_url": "https://goskive.com/university/uni-68",
      "slug": "uni-68",
      "name": "National School of Pizza",
      "short_name": "Uni 68",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe68b2e1c81a7d5c35fd1107da0e373597f006d5.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e85940cf8561c3a456df79e408c963432af4ba51.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T09:09:52.710Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 69,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-67",
      "html_url": "https://goskive.com/university/uni-67",
      "slug": "uni-67",
      "name": "National School of Pastry",
      "short_name": "Uni 67",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/708a005b52f81ade5d5c9481071b7a8cff7c4cd9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/822e4ae5676b385680a75a35bb9799eaca85f11e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T09:09:52.693Z",
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
	-H "Authorization: Bearer d02981532fc0c85dfc9ed9a612253a87bda5686b85276b8a1b75808c6b2fe399"
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
      "id": 36,
      "name": "Devolved empowering pricing structure",
      "name_translations": {
        "en": "Devolved empowering pricing structure"
      },
      "discipline_id": 37
    },
    {
      "id": 37,
      "name": "Proactive discrete interface",
      "name_translations": {
        "en": "Proactive discrete interface"
      },
      "discipline_id": 38
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
GET /v2/topics/35
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
    "id": 35,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 36
  }
}
```



```shell
curl "api.goskive.com/v2/topics/35" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer f0fe9247528788654fe789cf4cb28be1495cf531f49d68b4e2493a2eedf8fd2d
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
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-27",
      "html_url": "https://goskive.com/university/uni-27",
      "slug": "uni-27",
      "name": "University 12",
      "short_name": "Uni 27",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/304ae157986dd569dea48362e51bee432e419196.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/cf72c04ee41f93c5e3de90878b17dec10f89dee7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T09:09:39.314Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-25",
      "html_url": "https://goskive.com/university/uni-25",
      "slug": "uni-25",
      "name": "University 10",
      "short_name": "Uni 25",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/ae81d1f5d9e49d983905c81a4cb44b4673820d67.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/c4e9fc670e7b18129119ade770d7da2251ce0df7.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T09:09:39.280Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-26",
      "html_url": "https://goskive.com/university/uni-26",
      "slug": "uni-26",
      "name": "University 11",
      "short_name": "Uni 26",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/89e9b153031acf375a336870bfce3a7d17ec2f1b.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/9eac444cb58170c4797dc004099a3c0ff73ea304.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-12-08T09:09:39.297Z",
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
	-H "Authorization: Bearer f0fe9247528788654fe789cf4cb28be1495cf531f49d68b4e2493a2eedf8fd2d"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer ed1f093554b709a7209148f952d6c647cb309634bb4f35f09990b1debb1d39a9
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
    "id": 28,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe4573e6024e1dcbb559e8c92df9bcbf0b713f1d.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/62dc2fbffc76c59220d7254a885c01bfc78a3d58.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-12-08T09:09:39.430Z",
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
	-H "Authorization: Bearer ed1f093554b709a7209148f952d6c647cb309634bb4f35f09990b1debb1d39a9"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bfe0cdff762614caa28e9c12d2a323c0cac315fe6b40b2867be8d44124926aa1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":111,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 273,
    "id": 104,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 89,
    "additional_university_ids": [

    ],
    "discipline_id": 112,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 3,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "chapters_updated_at": "2016-12-08T09:09:56.947Z",
    "updated_at": "2016-12-08T09:09:57.064Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 45,
        "updated_at": "2016-12-08T09:09:57.051Z",
        "course_id": 104,
        "author_id": 273,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Etymology of Choux",
        "position": 1
      },
      {
        "id": 46,
        "updated_at": "2016-12-08T09:09:57.066Z",
        "course_id": 104,
        "author_id": 273,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Pastry Making in Medieval France",
        "position": 2
      },
      {
        "id": 47,
        "updated_at": "2016-12-08T09:09:57.082Z",
        "course_id": 104,
        "author_id": 273,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": null,
        "questions_updated_at": null,
        "flashcards_count": 0,
        "questions_count": 0,
        "title": "Pastry for Neophytes",
        "position": 3
      }
    ],
    "topic_id": 111,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":111,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfe0cdff762614caa28e9c12d2a323c0cac315fe6b40b2867be8d44124926aa1"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f07b86f0e5d577294f002f0430b3cefc09c26d8f4c4ef85694a7e9e2ed9e5e57
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":112,"published":false}}
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
    "creator_id": 274,
    "id": 105,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 90,
    "additional_university_ids": [

    ],
    "discipline_id": 113,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 0,
    "course_requests_count": 0,
    "flashcards_count": 0,
    "questions_count": 0,
    "files_count": 0,
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
    "updated_at": "2016-12-08T09:09:57.273Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 112,
    "language_code": "en",
    "exam_months": [

    ],
    "title": "Choux pastry 201",
    "organizational_identifier": null,
    "instructor_name": ""
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":112,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f07b86f0e5d577294f002f0430b3cefc09c26d8f4c4ef85694a7e9e2ed9e5e57"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 08f2dd2923892745b8efa27537ad9ffc658fc189a879f02996e227ba5ee6b791
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
      "creator_id": 236,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-42",
      "html_url": "https://goskive.com/course/fu-course-42",
      "slug": "fu-course-42",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "discipline_id": 81,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:53.591Z",
      "shortname": "fu-course-42",
      "topic_id": 80,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 42",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 236,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-43",
      "html_url": "https://goskive.com/course/fu-course-43",
      "slug": "fu-course-43",
      "university_id": 76,
      "additional_university_ids": [

      ],
      "discipline_id": 82,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T09:09:53.458Z",
      "updated_at": "2016-12-08T09:09:53.889Z",
      "shortname": "fu-course-43",
      "topic_id": 81,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 43",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08f2dd2923892745b8efa27537ad9ffc658fc189a879f02996e227ba5ee6b791"
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
      "creator_id": 256,
      "id": 89,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 82,
      "additional_university_ids": [

      ],
      "discipline_id": 97,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:55.331Z",
      "shortname": "fu-course-58",
      "topic_id": 96,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 256,
      "id": 90,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 82,
      "additional_university_ids": [

      ],
      "discipline_id": 98,
      "permissions": [

      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 1,
      "files_count": 0,
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
      "chapters_updated_at": "2016-12-08T09:09:55.198Z",
      "updated_at": "2016-12-08T09:09:55.627Z",
      "shortname": "fu-course-59",
      "topic_id": 97,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 59",
      "organizational_identifier": null,
      "instructor_name": ""
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
Authorization: Bearer ac53507952848df29d03e5046c4be5e8e3e16374448e82d97b8e2a4090d67b4e
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
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 78,
      "additional_university_ids": [

      ],
      "discipline_id": 85,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:54.202Z",
      "shortname": "fu-course-46",
      "topic_id": 84,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 46",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 243,
      "id": 78,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 78,
      "additional_university_ids": [

      ],
      "discipline_id": 86,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:54.237Z",
      "shortname": "fu-course-47",
      "topic_id": 85,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ac53507952848df29d03e5046c4be5e8e3e16374448e82d97b8e2a4090d67b4e"
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
      "creator_id": 261,
      "id": 93,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-62",
      "html_url": "https://goskive.com/course/fu-course-62",
      "slug": "fu-course-62",
      "university_id": 83,
      "additional_university_ids": [

      ],
      "discipline_id": 101,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:55.798Z",
      "shortname": "fu-course-62",
      "topic_id": 100,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 62",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 261,
      "id": 94,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-63",
      "html_url": "https://goskive.com/course/fu-course-63",
      "slug": "fu-course-63",
      "university_id": 83,
      "additional_university_ids": [

      ],
      "discipline_id": 102,
      "permissions": [

      ],
      "chapters_count": 0,
      "course_requests_count": 0,
      "flashcards_count": 0,
      "questions_count": 0,
      "files_count": 0,
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
      "updated_at": "2016-12-08T09:09:55.833Z",
      "shortname": "fu-course-63",
      "topic_id": 101,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 63",
      "organizational_identifier": null,
      "instructor_name": ""
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
Authorization: Bearer b90cd77e061d431882101cec64014f67799c9022072ba9534d0f6ab4a2335df4
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
  "id": 655,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-12-08T09:10:21.900Z",
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
	-H "Authorization: Bearer b90cd77e061d431882101cec64014f67799c9022072ba9534d0f6ab4a2335df4"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/125
Content-Type: application/json
Authorization: Bearer 7efca16b11713f201efc0e57060671db14302bc384c90bc262922e878b7cf343
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
    "id": 125,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 38,
    "fields_of_study": [
      38,
      39
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-12-08T09:09:43.338Z",
    "updated_at": "2016-12-08T09:09:43.338Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/125" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7efca16b11713f201efc0e57060671db14302bc384c90bc262922e878b7cf343"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/123
Content-Type: application/json
Authorization: Bearer d6e3f427bac8fe502a7c314387fbcfb16f71f66f78689c92935016a32f97f482
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
    "id": 123,
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
    "created_at": "2016-12-08T09:09:43.180Z",
    "updated_at": "2016-12-08T09:09:43.180Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/123" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6e3f427bac8fe502a7c314387fbcfb16f71f66f78689c92935016a32f97f482"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/3
Content-Type: application/json
Authorization: Bearer 7f23947e0df2bdea39206126fbd9b1680048b49ca10f9c0a037fc2436cf90363
```

`DELETE /v2/votes/:vote_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/votes/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f23947e0df2bdea39206126fbd9b1680048b49ca10f9c0a037fc2436cf90363"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/2
Content-Type: application/json
Authorization: Bearer a8273623f1e4e476cd1dfe69cb506433e4aafb42769e77421b74faa53e1b765e
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
    "votable_id": 28,
    "user_id": 66
  }
}
```



```shell
curl "api.goskive.com/v2/votes/2" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8273623f1e4e476cd1dfe69cb506433e4aafb42769e77421b74faa53e1b765e"
```
