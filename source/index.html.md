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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"68df15219b2438a313cf618ffccc76e46dac163fd4366d5c874f4a4b9a4870b9","client_secret":"dd18680b6c89500533f0b35584fd0ffd23c32595cb9246f20376a15fe78162b0"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"68df15219b2438a313cf618ffccc76e46dac163fd4366d5c874f4a4b9a4870b9","client_secret":"dd18680b6c89500533f0b35584fd0ffd23c32595cb9246f20376a15fe78162b0"}' -X POST \
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
Authorization: Basic YzE1NTRiZmQ1ZTI3NTVhOTNjZDUxYjM3MDhkOTAyOTJmYzRmYTRlN2U3NDEw
ODY4MDRhYjBlY2U5YzMwMDFmZDo3NWZhZmEzYjAyZTNjNWI5YzJmYzZjYmJk
NGEyOTAxZDg2MDZmMTdmYzRjNTI2NGMxYTdiYWJmNTEzY2Q0OTVl

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
	-u c1554bfd5e2755a93cd51b3708d90292fc4fa4e7e741086804ab0ece9c3001fd:75fafa3b02e3c5b9c2fc6cbbd4a2901d8606f17fc4c5264c1a7babf513cd495e
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"3a795f6ad3306a9961ed59adb1900ff812a28940e50132d14fda8bc0a99497ff","client_secret":"b6235098aa52cb9361fd30a878410b7866a47cf497a1c9866187b8a7c078a1c7"}
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
  "access_token": "da0cfc3ac0af6159088ccba6c971ef7ec19228759cbc6855db0821d166d5081b",
  "token_type": "bearer",
  "created_at": 1476366018
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"3a795f6ad3306a9961ed59adb1900ff812a28940e50132d14fda8bc0a99497ff","client_secret":"b6235098aa52cb9361fd30a878410b7866a47cf497a1c9866187b8a7c078a1c7"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic NmEwN2NkZDY4ZThmN2IzZDNmODBlMTgzM2IwMDMzYzNhMTY4NjM5N2ViYzQz
YTdmNDgxOTg3M2U1MGQxNzc3Zjo4ZTk1YmIwMzcxZjg5ODgyOTI2ZDMyMjNk
ODkzZGZmNzEzOGEyYmJjMGM3Yjk1NTJiNmU5OGY4NmZiMzZjNWMy

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
  "access_token": "ffc80823b6f0a4a3ada325a6ef974bceb7102abe3e4fd3b40afbc15da926eb9c",
  "token_type": "bearer",
  "created_at": 1476366018
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 6a07cdd68e8f7b3d3f80e1833b0033c3a1686397ebc43a7f4819873e50d1777f:8e95bb0371f89882926d3223d893dff7138a2bbc0c7b9552b6e98f86fb36c5c2
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
{"grant_type":"client_credentials","client_id":"0aab468a18f9eec4712aed100a18fc6431020fde45186e9b1f82a7a85e629f29","client_secret":"c173a73a2d36c931b45cf845a826ee38dc28a43a2f65722f4128fe95f9b532d2"}
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
  "access_token": "d72523e66e6f5f0b10e30c46557af7c2458367303fec7fb4f734c33398642dee",
  "token_type": "bearer",
  "created_at": 1476366018
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"0aab468a18f9eec4712aed100a18fc6431020fde45186e9b1f82a7a85e629f29","client_secret":"c173a73a2d36c931b45cf845a826ee38dc28a43a2f65722f4128fe95f9b532d2"}' -X POST \
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
Authorization: Bearer 6558c9aef9e556f8c95511e4cb60e0eac788cc7c7e7f5dbeec12088b0d56e397
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
    "company_id": 39,
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
	-H "Authorization: Bearer 6558c9aef9e556f8c95511e4cb60e0eac788cc7c7e7f5dbeec12088b0d56e397"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/175/flashcards
Content-Type: application/json
Authorization: Bearer c961b01c1be120cfd13b910a777cfb1c2b7288756a8a783b0f3e74c71573d9a9
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":175,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 66,
    "obfuscated_id": "H7dODBospvw",
    "author_id": 878,
    "chapter_id": 175,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:37.208Z",
    "created_at": "2016-10-13T13:40:37.208Z",
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
curl "api.goskive.com/v2/chapters/175/flashcards" -d '{"flashcard":{"chapter_id":175,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c961b01c1be120cfd13b910a777cfb1c2b7288756a8a783b0f3e74c71573d9a9"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/176/flashcards
Content-Type: application/json
Authorization: Bearer ea427115d62e13e4cba5765ea2673658369c281b5a16d74e97ccd23699365dc5
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 879,
      "chapter_id": 176,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:37.361Z",
      "created_at": "2016-10-13T13:40:37.361Z",
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 879,
      "chapter_id": 176,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:37.400Z",
      "created_at": "2016-10-13T13:40:37.400Z",
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
      "author_id": 879,
      "chapter_id": 176,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:37.438Z",
      "created_at": "2016-10-13T13:40:37.438Z",
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
curl "api.goskive.com/v2/chapters/176/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea427115d62e13e4cba5765ea2673658369c281b5a16d74e97ccd23699365dc5"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/182/questions
Content-Type: application/json
Authorization: Bearer 2b47ee9ef559682059258b23c6cebfa4d4fdd3e2567eb62f36af783fd6b97384
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":182,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "id": 107,
    "obfuscated_id": "_2rgp7tgq8o",
    "author_id": 907,
    "chapter_id": 182,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:39.874Z",
    "created_at": "2016-10-13T13:40:39.874Z",
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
        "id": 215,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 216,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 217,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 218,
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
curl "api.goskive.com/v2/chapters/182/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":182,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b47ee9ef559682059258b23c6cebfa4d4fdd3e2567eb62f36af783fd6b97384"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/180/questions
Content-Type: application/json
Authorization: Bearer d10b3da989f515af331c108b4121fadb202322f45aff2c804e139afc67c3a932
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":180,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 105,
    "obfuscated_id": "3yX9LpVrF_M",
    "author_id": 901,
    "chapter_id": 180,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:39.094Z",
    "created_at": "2016-10-13T13:40:39.094Z",
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
        "id": 210,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 211,
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
curl "api.goskive.com/v2/chapters/180/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":180,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d10b3da989f515af331c108b4121fadb202322f45aff2c804e139afc67c3a932"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/183/questions
Content-Type: application/json
Authorization: Bearer b1e3244beb447946c75390b9b79aae2aa951e1ac0d427a70fa0e8aa54d13fb19
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "id": 108,
    "obfuscated_id": "3MKez0MLRBM",
    "author_id": 910,
    "chapter_id": 183,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:40.389Z",
    "created_at": "2016-10-13T13:40:40.389Z",
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
        "id": 219,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 220,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/183/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":183,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1e3244beb447946c75390b9b79aae2aa951e1ac0d427a70fa0e8aa54d13fb19"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/181/questions
Content-Type: application/json
Authorization: Bearer 3de9bd06d7ab2f1996714037c4c033e9804854a6999d5ae80fae8da78f7b4799
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":181,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "id": 106,
    "obfuscated_id": "GEL902caNek",
    "author_id": 904,
    "chapter_id": 181,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:39.441Z",
    "created_at": "2016-10-13T13:40:39.441Z",
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
        "id": 212,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 213,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 214,
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
curl "api.goskive.com/v2/chapters/181/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":181,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3de9bd06d7ab2f1996714037c4c033e9804854a6999d5ae80fae8da78f7b4799"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/178/questions
Content-Type: application/json
Authorization: Bearer 48319a3ff23c3d9f8eec98dd5da827f672af0fbec505f9da64b0f7f4467d7704
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
      "id": 102,
      "obfuscated_id": "jFy90P7ldB4",
      "author_id": 892,
      "chapter_id": 178,
      "position": 93,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:38.291Z",
      "created_at": "2016-10-13T13:40:38.172Z",
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
    },
    {
      "id": 103,
      "obfuscated_id": "AVhVflMAvL0",
      "author_id": 893,
      "chapter_id": 178,
      "position": 94,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:38.490Z",
      "created_at": "2016-10-13T13:40:38.368Z",
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
          "id": 206,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 207,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 104,
      "obfuscated_id": "nIg2bhYRjos",
      "author_id": 894,
      "chapter_id": 178,
      "position": 95,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T13:40:38.692Z",
      "created_at": "2016-10-13T13:40:38.566Z",
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
          "id": 208,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 209,
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
curl "api.goskive.com/v2/chapters/178/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48319a3ff23c3d9f8eec98dd5da827f672af0fbec505f9da64b0f7f4467d7704"
```
# Chapters

## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/14
Content-Type: application/json
Authorization: Bearer b08c4a1062d888e89d83d9dc4f201578b41c1fc9198ac7a56889d7d4fdca0285
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
curl "api.goskive.com/v2/chapters/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b08c4a1062d888e89d83d9dc4f201578b41c1fc9198ac7a56889d7d4fdca0285"
```
## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/15
Content-Type: application/json
Authorization: Bearer 2422426641c2a0d80eb938f2e65e139c71b6b77c3fd445c7565da6dc54abf4de
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
curl "api.goskive.com/v2/chapters/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2422426641c2a0d80eb938f2e65e139c71b6b77c3fd445c7565da6dc54abf4de"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 2be528e56a7789087233567978108981f9057b4a863be2846e224ec8f84a4c8e
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
curl "api.goskive.com/v2/chapters/7" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2be528e56a7789087233567978108981f9057b4a863be2846e224ec8f84a4c8e"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/13
Content-Type: application/json
Authorization: Bearer 4af7630a89920f4c7b4a2db4342f616a4ec89cdbaefc97e357adcc17dc400cc8
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4af7630a89920f4c7b4a2db4342f616a4ec89cdbaefc97e357adcc17dc400cc8"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/11
Content-Type: application/json
Authorization: Bearer 7ad42b9890e69abe60a6c365721ebd33f993a621ed811128d5d099c81627e990
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
    "id": 11,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T13:39:28.343Z",
    "course_id": 19,
    "author_id": 57,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-13T13:39:27.765Z",
    "questions_updated_at": "2016-10-13T13:39:27.765Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 61,
        "chapter_id": 11,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:28.321Z",
        "created_at": "2016-10-13T13:39:28.321Z",
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
        "id": 10,
        "obfuscated_id": "aY5v9ahzH5c",
        "author_id": 59,
        "chapter_id": 11,
        "position": 10,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:39:28.203Z",
        "created_at": "2016-10-13T13:39:28.075Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/11" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7ad42b9890e69abe60a6c365721ebd33f993a621ed811128d5d099c81627e990"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 47a590875efc5159dbee7a0e614522b5ca9c0665fde1ae494fc2dbf40dad6b8d
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
    "id": 9,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T13:39:26.998Z",
    "course_id": 17,
    "author_id": 48,
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
curl "api.goskive.com/v2/chapters/9" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47a590875efc5159dbee7a0e614522b5ca9c0665fde1ae494fc2dbf40dad6b8d"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/10/replies
Content-Type: application/json
Authorization: Bearer 2749bf5e3393eaa22c0e8f5dd7acd415f19a652fda013655c14caa58416cae65
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
    "id": 11,
    "author_id": 170,
    "reply_to_id": 10,
    "created_at": "2016-10-13T13:39:38.184Z",
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
curl "api.goskive.com/v2/comments/10/replies" -d '{"comment":{"message":"Just keeping the thread alive!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2749bf5e3393eaa22c0e8f5dd7acd415f19a652fda013655c14caa58416cae65"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/12/replies
Content-Type: application/json
Authorization: Bearer c3209b4c83f8219736acb6447fd9c5bdb7bdafa8155948668b32db1d258a1ff4
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
	-H "Authorization: Bearer c3209b4c83f8219736acb6447fd9c5bdb7bdafa8155948668b32db1d258a1ff4"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/59
Content-Type: application/json
Authorization: Bearer 365fd9f5e6123afab861f87ee2a0c715ffda485d35dc010a60286efcee02646f
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
curl "api.goskive.com/v2/comments/59" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 365fd9f5e6123afab861f87ee2a0c715ffda485d35dc010a60286efcee02646f"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/56/republish
Content-Type: application/json
Authorization: Bearer 286557f4dc75d6ce56286d9ef5a8829a74210bdd717df3eb856130843be6dec0
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
curl "api.goskive.com/v2/comments/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 286557f4dc75d6ce56286d9ef5a8829a74210bdd717df3eb856130843be6dec0"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/57
Content-Type: application/json
Authorization: Bearer 581e6dcfcbf3be19573bbf7748c45d5467ba26ce4ecc359ac72c6f3d91c8270c
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 581e6dcfcbf3be19573bbf7748c45d5467ba26ce4ecc359ac72c6f3d91c8270c"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/60/report
Content-Type: application/json
Authorization: Bearer 41a0b5fa3990a5b59c39c474b5d118aa83b2824adbac16e59b5e47252631faf1
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
	-H "Authorization: Bearer 41a0b5fa3990a5b59c39c474b5d118aa83b2824adbac16e59b5e47252631faf1"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/9
Content-Type: application/json
Authorization: Bearer 2c70b2b24648ebf3225850c7f37debb37107ddb483ef1966f1b9daebd3555431
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
    "id": 9,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/94c83855f6a5299b550b7cd786d8681b60977898.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-13T13:39:54.235Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/9" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c70b2b24648ebf3225850c7f37debb37107ddb483ef1966f1b9daebd3555431"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer bc1e6b2d9c62e1f7544bfbeaabb1603585dc79316004a5a16327d3d8ba3d27ca
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
      "updated_at": "2016-10-13T13:39:54.310Z"
    },
    {
      "id": 11,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/a7f4ed851ff0ca786562d024f4486022b2a89d3e.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T13:39:54.314Z"
    },
    {
      "id": 12,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/493bcdf71e61940532460dac0cfa6de4d3b874bb.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-13T13:39:54.318Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc1e6b2d9c62e1f7544bfbeaabb1603585dc79316004a5a16327d3d8ba3d27ca"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/18/company_profiles
Content-Type: application/json
Authorization: Bearer 3535943bb6b29fa1e3eb6907304f4f4724c408413e681ce994e0f3d8775607fb
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
	-H "Authorization: Bearer 3535943bb6b29fa1e3eb6907304f4f4724c408413e681ce994e0f3d8775607fb"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/16/company_profiles
Content-Type: application/json
Authorization: Bearer 42059c20920d845c8b234035eae34551f91360c16a068564fff8e80054249dff
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
curl "api.goskive.com/v2/companies/16/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 42059c20920d845c8b234035eae34551f91360c16a068564fff8e80054249dff"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer 71ce4ff3c1e838241babe83d6c675109af680d32421fc085a95aa22ec7abc4cb
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
      "id": 8,
      "title": "Campaign 8",
      "company_id": 33,
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
      "id": 11,
      "title": "Campaign 11",
      "company_id": 36,
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
	-H "Authorization: Bearer 71ce4ff3c1e838241babe83d6c675109af680d32421fc085a95aa22ec7abc4cb"
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
Authorization: Bearer 2228f32df59f42ca4fb8640ddfbb31c485839ca22d0d886c707469fdd326d830
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
	-H "Authorization: Bearer 2228f32df59f42ca4fb8640ddfbb31c485839ca22d0d886c707469fdd326d830"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer aac57f692d7983aa9adc2d1c3a876e86bd57fcf27cbd4b77118574992e55fe12
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
    "updated_at": "2016-10-13T13:40:30.556Z",
    "course_id": 232,
    "author_id": 764,
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
	-H "Authorization: Bearer aac57f692d7983aa9adc2d1c3a876e86bd57fcf27cbd4b77118574992e55fe12"
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
      "id": 151,
      "title": "Clever Chapter Title 139",
      "position": 1,
      "updated_at": "2016-10-13T13:40:28.311Z",
      "course_id": 223,
      "author_id": 725,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 152,
      "title": "Clever Chapter Title 140",
      "position": 2,
      "updated_at": "2016-10-13T13:40:28.338Z",
      "course_id": 223,
      "author_id": 726,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 153,
      "title": "Clever Chapter Title 141",
      "position": 3,
      "updated_at": "2016-10-13T13:40:28.606Z",
      "course_id": 223,
      "author_id": 727,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T13:40:28.229Z",
      "questions_updated_at": "2016-10-13T13:40:28.229Z",
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
Authorization: Bearer bb4f50e872a2a1f14ce2628a23ce4075ecf29b461e85f92a1ee08d262c77f89b
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
      "id": 157,
      "title": "Clever Chapter Title 145",
      "position": 1,
      "updated_at": "2016-10-13T13:40:28.994Z",
      "course_id": 226,
      "author_id": 736,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 158,
      "title": "Clever Chapter Title 146",
      "position": 2,
      "updated_at": "2016-10-13T13:40:29.020Z",
      "course_id": 226,
      "author_id": 737,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 159,
      "title": "Clever Chapter Title 147",
      "position": 3,
      "updated_at": "2016-10-13T13:40:29.288Z",
      "course_id": 226,
      "author_id": 738,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-13T13:40:28.912Z",
      "questions_updated_at": "2016-10-13T13:40:28.912Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bb4f50e872a2a1f14ce2628a23ce4075ecf29b461e85f92a1ee08d262c77f89b"
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
      "id": 154,
      "title": "Clever Chapter Title 142",
      "position": 1,
      "updated_at": "2016-10-13T13:40:28.816Z",
      "course_id": 225,
      "author_id": 732,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 155,
      "title": "Clever Chapter Title 143",
      "position": 2,
      "updated_at": "2016-10-13T13:40:28.843Z",
      "course_id": 225,
      "author_id": 733,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 156,
      "title": "Clever Chapter Title 144",
      "position": 3,
      "updated_at": "2016-10-13T13:40:28.870Z",
      "course_id": 225,
      "author_id": 734,
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
Authorization: Bearer b12551a6cbfc7f217966a6ae155a4844f75f8ed79a0406a400b62848c99e0f7c
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
      "id": 160,
      "title": "Clever Chapter Title 148",
      "position": 1,
      "updated_at": "2016-10-13T13:40:29.454Z",
      "course_id": 227,
      "author_id": 743,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 161,
      "title": "Clever Chapter Title 149",
      "position": 2,
      "updated_at": "2016-10-13T13:40:29.480Z",
      "course_id": 227,
      "author_id": 744,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 162,
      "title": "Clever Chapter Title 150",
      "position": 3,
      "updated_at": "2016-10-13T13:40:29.506Z",
      "course_id": 227,
      "author_id": 745,
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
	-H "Authorization: Bearer b12551a6cbfc7f217966a6ae155a4844f75f8ed79a0406a400b62848c99e0f7c"
```
# Course Course Requests

## Create a course request


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer b7750dab039e1d74b638c6fe0c1a2dd48370a4cd263354670f6735204c49a0cf
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
    "course_id": 72,
    "user_id": 256,
    "updated_at": "2016-10-13T13:39:43.353Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7750dab039e1d74b638c6fe0c1a2dd48370a4cd263354670f6735204c49a0cf"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer d795e80c85a4c7e52b1ff3d3d07c3fbf8ea6a13802ff1f91e8fc53a4b665fb45
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
      "course_id": 74,
      "user_id": 260,
      "updated_at": "2016-10-13T13:39:43.596Z"
    },
    {
      "id": 5,
      "course_id": 74,
      "user_id": 261,
      "updated_at": "2016-10-13T13:39:43.612Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d795e80c85a4c7e52b1ff3d3d07c3fbf8ea6a13802ff1f91e8fc53a4b665fb45"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/26/files
Content-Type: application/json
Authorization: Bearer aaa123af84d943de0db4a61a16ad2f5edef0e1f12f3a4608ccc96f8f9e07c702
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
        "id": 80,
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
        "created_at": "2016-10-13T13:39:29.736Z",
        "updated_at": "2016-10-13T13:39:29.736Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T13:39:29.750Z",
      "updated_at": "2016-10-13T13:39:29.750Z",
      "course_id": 26,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 2,
      "uploader": {
        "id": 81,
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
        "created_at": "2016-10-13T13:39:29.759Z",
        "updated_at": "2016-10-13T13:39:29.759Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T13:39:29.766Z",
      "updated_at": "2016-10-13T13:39:29.766Z",
      "course_id": 26,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 3,
      "uploader": {
        "id": 82,
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
        "created_at": "2016-10-13T13:39:29.773Z",
        "updated_at": "2016-10-13T13:39:29.773Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "created_at": "2016-10-13T13:39:29.780Z",
      "updated_at": "2016-10-13T13:39:29.780Z",
      "course_id": 26,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/26/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aaa123af84d943de0db4a61a16ad2f5edef0e1f12f3a4608ccc96f8f9e07c702"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/27/files
Content-Type: application/json
Authorization: Bearer 33594d3e1a38c8524b9b268474d525670bac772a078f8376e71b754778883d3b
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
      "id": 85,
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
      "created_at": "2016-10-13T13:39:29.914Z",
      "updated_at": "2016-10-13T13:39:29.914Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "created_at": "2016-10-13T13:39:29.945Z",
    "updated_at": "2016-10-13T13:39:29.945Z",
    "course_id": 27,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/27/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 33594d3e1a38c8524b9b268474d525670bac772a078f8376e71b754778883d3b"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/24/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 280775bf05ce63f6f331f1133e8476c54f684d31806c4f4876c1cda2797fa0b5
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
    "key": "cache/7ac0f58abf5cae8f71bf43661d4ad085.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxNDozOToyOVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS83YWMwZjU4YWJmNWNhZThmNzFiZjQzNjYxZDRhZDA4NS5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTMzOTI5WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T133929Z",
    "x-amz-signature": "b515aa333642aadaa77d025d79f4b6dabbd8d0d54a24346af1bbd52582e26566"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/24/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 280775bf05ce63f6f331f1133e8476c54f684d31806c4f4876c1cda2797fa0b5"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/1
Content-Type: application/json
Authorization: Bearer 0adeb82019749d1f21e27c2ef71a122fe265183cd6ed338523a93eb9c4e8981c
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
	-H "Authorization: Bearer 0adeb82019749d1f21e27c2ef71a122fe265183cd6ed338523a93eb9c4e8981c"
```
# Courses

## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e45d3b6ebc41e3e8997681179da89e9678ab779163fbb8c942bcebc269e0c98e
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
	-H "Authorization: Bearer e45d3b6ebc41e3e8997681179da89e9678ab779163fbb8c942bcebc269e0c98e"
```
## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 64ccec57be591f520ded1792adc0a2bb35ddebc91f3acb3403236b1159bcf55c
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
	-H "Authorization: Bearer 64ccec57be591f520ded1792adc0a2bb35ddebc91f3acb3403236b1159bcf55c"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 440a91c2a67f1f98e1b906f2188439a8cff1dc30ebdaa37b07de70a35e503688
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
	-H "Authorization: Bearer 440a91c2a67f1f98e1b906f2188439a8cff1dc30ebdaa37b07de70a35e503688"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 597ec373d0eb1dbebb26ede63c8d3e5d03eb3b982aebf2de9bf841b4c130be00
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
	-H "Authorization: Bearer 597ec373d0eb1dbebb26ede63c8d3e5d03eb3b982aebf2de9bf841b4c130be00"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 8b900de94baba874471a4fa5d33e0565d314ccdaf4e13df67764e9be0958fc22
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
    "creator_id": 917,
    "id": 290,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 275,
    "additional_university_ids": [

    ],
    "topic_id": 302,
    "discipline_id": 303,
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
    "chapters_updated_at": "2016-10-13T13:40:42.245Z",
    "updated_at": "2016-10-13T13:40:43.781Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 186,
        "title": "Clever Chapter Title 162",
        "position": 1,
        "updated_at": "2016-10-13T13:40:43.730Z",
        "course_id": 290,
        "author_id": 917,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:40:42.245Z",
        "questions_updated_at": "2016-10-13T13:40:42.245Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 187,
        "title": "Clever Chapter Title 163",
        "position": 2,
        "updated_at": "2016-10-13T13:40:43.773Z",
        "course_id": 290,
        "author_id": 917,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:40:42.245Z",
        "questions_updated_at": "2016-10-13T13:40:42.245Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 918,
        "chapter_id": 186,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:43.555Z",
        "created_at": "2016-10-13T13:40:43.555Z",
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
        "author_id": 918,
        "chapter_id": 187,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:43.632Z",
        "created_at": "2016-10-13T13:40:43.632Z",
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
        "author_id": 918,
        "chapter_id": 186,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:43.598Z",
        "created_at": "2016-10-13T13:40:43.598Z",
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
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 918,
        "chapter_id": 187,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:43.676Z",
        "created_at": "2016-10-13T13:40:43.676Z",
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
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 918,
        "chapter_id": 186,
        "position": 102,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:42.476Z",
        "created_at": "2016-10-13T13:40:42.353Z",
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
      },
      {
        "id": 116,
        "obfuscated_id": "PhHGVKqnHFA",
        "author_id": 918,
        "chapter_id": 186,
        "position": 103,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:42.661Z",
        "created_at": "2016-10-13T13:40:42.544Z",
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
            "id": 235,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 236,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 117,
        "obfuscated_id": "BsA8mEPn8aM",
        "author_id": 918,
        "chapter_id": 187,
        "position": 104,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:42.875Z",
        "created_at": "2016-10-13T13:40:42.748Z",
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
            "id": 237,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 238,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 918,
        "chapter_id": 187,
        "position": 105,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:43.066Z",
        "created_at": "2016-10-13T13:40:42.945Z",
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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b900de94baba874471a4fa5d33e0565d314ccdaf4e13df67764e9be0958fc22"
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
    "creator_id": 929,
    "id": 292,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 277,
    "additional_university_ids": [

    ],
    "topic_id": 304,
    "discipline_id": 305,
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
    "chapters_updated_at": "2016-10-13T13:40:45.534Z",
    "updated_at": "2016-10-13T13:40:47.038Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 190,
        "title": "Clever Chapter Title 166",
        "position": 1,
        "updated_at": "2016-10-13T13:40:46.990Z",
        "course_id": 292,
        "author_id": 929,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:40:45.534Z",
        "questions_updated_at": "2016-10-13T13:40:45.534Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 191,
        "title": "Clever Chapter Title 167",
        "position": 2,
        "updated_at": "2016-10-13T13:40:47.031Z",
        "course_id": 292,
        "author_id": 929,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-13T13:40:45.534Z",
        "questions_updated_at": "2016-10-13T13:40:45.534Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 127,
        "obfuscated_id": "E3yfRgAzssw",
        "author_id": 929,
        "chapter_id": 190,
        "position": 114,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:45.751Z",
        "created_at": "2016-10-13T13:40:45.632Z",
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
        "id": 129,
        "obfuscated_id": "x8EyeGrWnN4",
        "author_id": 929,
        "chapter_id": 191,
        "position": 116,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T13:40:46.146Z",
        "created_at": "2016-10-13T13:40:46.019Z",
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
            "id": 261,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 262,
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
PUT /v2/courses/303/pin
Content-Type: application/json
Authorization: Bearer 57223ef40cc25720ae76568c0c7515b726d941e922139b3334d235f0571a8df5
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/303/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57223ef40cc25720ae76568c0c7515b726d941e922139b3334d235f0571a8df5"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/293/pin
Content-Type: application/json
Authorization: Bearer d5841862d55d885a3b1e0f8f0719e641eb537d42f9926be50279a7cdbeec81c5
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/293/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5841862d55d885a3b1e0f8f0719e641eb537d42f9926be50279a7cdbeec81c5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b95a1fac425a17e13e0683cb68a8998fe33d2d46ff233ac31debcd00c5d868d6
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
    "creator_id": 960,
    "id": 305,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 290,
    "additional_university_ids": [

    ],
    "topic_id": 317,
    "discipline_id": 318,
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
    "updated_at": "2016-10-13T13:40:49.230Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b95a1fac425a17e13e0683cb68a8998fe33d2d46ff233ac31debcd00c5d868d6"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 1009827bd68a549fcc9c4572539b329397b4cc086ca130b62719e6414e981586
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
    "id": 397,
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
    "created_at": "2016-10-13T13:39:53.524Z",
    "updated_at": "2016-10-13T13:39:53.524Z",
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
	-H "Authorization: Bearer 1009827bd68a549fcc9c4572539b329397b4cc086ca130b62719e6414e981586"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 384fbbc22429f5bfe05e32c89f2b6ed94c41efad3a9f8ce7bcd61f4a3bc4f34f
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[106]}
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
    "id": 398,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      106
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T13:39:53.615Z",
    "updated_at": "2016-10-13T13:39:53.659Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[106]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 384fbbc22429f5bfe05e32c89f2b6ed94c41efad3a9f8ce7bcd61f4a3bc4f34f"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer b7b9645454f8521cc69c2429fb4fcf0084a2980f51873e209b0bf2cb677133a3
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
    "id": 399,
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
    "created_at": "2016-10-13T13:39:53.681Z",
    "updated_at": "2016-10-13T13:39:53.681Z",
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
	-H "Authorization: Bearer b7b9645454f8521cc69c2429fb4fcf0084a2980f51873e209b0bf2cb677133a3"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer d4d67d179c1f81172236f973011142c11bf6124f22326e616e01f9df1b671e09
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[109]}
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
    "id": 401,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      109
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T13:39:53.856Z",
    "updated_at": "2016-10-13T13:39:53.856Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[109]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4d67d179c1f81172236f973011142c11bf6124f22326e616e01f9df1b671e09"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 75584c83c2d219bee29ac4ee6a3d760121bced3fcd6402c6faa034029435e09e
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

110
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
    "id": 402,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/ee0318957b81836c29dfedcacc286693e87b0a29.jpg",
    "university_id": null,
    "fields_of_study": [
      110
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-13T13:39:53.929Z",
    "updated_at": "2016-10-13T13:39:54.207Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/05198b9ac666b7afa2af505291357087ffd66ea2.jpg",
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

110
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 75584c83c2d219bee29ac4ee6a3d760121bced3fcd6402c6faa034029435e09e"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer d3d6d42cfddce02f17e55583cf1515280d17da1637328fcfeab8a98d88364534
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
      "bookmarkable_id": 43,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 44,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 45,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d3d6d42cfddce02f17e55583cf1515280d17da1637328fcfeab8a98d88364534"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer fb8c3c2b94408b3bbf3f31ef3907ba6ce6f68f514fd7df1bc53cc7ab37cc79fa
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
      "company_id": 5,
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
      "id": 3,
      "title": "Campaign 3",
      "company_id": 6,
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
	-H "Authorization: Bearer fb8c3c2b94408b3bbf3f31ef3907ba6ce6f68f514fd7df1bc53cc7ab37cc79fa"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer dea22d9a7a66a68b4f7f7115a7d1d389e31def509cdd5c95ad7a8f5c9f3b171a
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
      "company_id": 1,
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
	-H "Authorization: Bearer dea22d9a7a66a68b4f7f7115a7d1d389e31def509cdd5c95ad7a8f5c9f3b171a"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 9e120397f5476b320835769274ee1a58d4614f2f81bfc0cad6f192b418c92d2b
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
      "creator_id": 675,
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-178",
      "html_url": "https://goskive.com/course/mit-course-178",
      "slug": "mit-course-178",
      "university_id": 190,
      "additional_university_ids": [

      ],
      "topic_id": 216,
      "discipline_id": 216,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 178",
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
      "updated_at": "2016-10-13T13:40:24.364Z",
      "shortname": "mit-course-178"
    },
    {
      "creator_id": 676,
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-179",
      "html_url": "https://goskive.com/course/mit-course-179",
      "slug": "mit-course-179",
      "university_id": 191,
      "additional_university_ids": [

      ],
      "topic_id": 217,
      "discipline_id": 217,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
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
      "updated_at": "2016-10-13T13:40:24.453Z",
      "shortname": "mit-course-179"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9e120397f5476b320835769274ee1a58d4614f2f81bfc0cad6f192b418c92d2b"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer f579b0ecc62ff9226ede79061ac44f329cc09322afbc84fdb6c5f1ed7e0c9905
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
      "company_id": 24,
      "company": {
        "id": 24,
        "name": "Fake Company Name 20",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/09f70a515a4dad8202eb040deb696cdaf210b1cc.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T13:40:00.873Z"
      },
      "created_at": "2016-10-13T13:40:00.877Z",
      "updated_at": "2016-10-13T13:40:00.877Z",
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
      "company_id": 25,
      "company": {
        "id": 25,
        "name": "Fake Company Name 21",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/8ff5ed961552a2c0623031f058da37f63a332145.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T13:40:00.886Z"
      },
      "created_at": "2016-10-13T13:40:00.889Z",
      "updated_at": "2016-10-13T13:40:00.889Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f579b0ecc62ff9226ede79061ac44f329cc09322afbc84fdb6c5f1ed7e0c9905"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer dc7162e919f376e55f7ef24960b6554fa0a7791cad259c8cb5374898c7fcdad7
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
      "company_id": 20,
      "company": {
        "id": 20,
        "name": "Fake Company Name 16",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/e04b5bd4d1b2a9fa5770226b80769bb90d30e5d4.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T13:40:00.651Z"
      },
      "created_at": "2016-10-13T13:40:00.654Z",
      "updated_at": "2016-10-13T13:40:00.654Z",
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
      "company_id": 21,
      "company": {
        "id": 21,
        "name": "Fake Company Name 17",
        "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/f01143c6c30f4054d83391b477da68091c594bf7.png",
        "brand_color": "#000000",
        "updated_at": "2016-10-13T13:40:00.668Z"
      },
      "created_at": "2016-10-13T13:40:00.672Z",
      "updated_at": "2016-10-13T13:40:00.672Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc7162e919f376e55f7ef24960b6554fa0a7791cad259c8cb5374898c7fcdad7"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer a48122cc2d4fa0a1f03f4b65d10d43f847afc8b266ef40f043b2946bf20ba81b
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
      "id": 2,
      "created_at": "2016-10-13T13:39:24.119Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 2,
      "updated_at": "2016-10-13T13:39:24.229Z",
      "author_id": "14",
      "thread_subject_id": "7",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 3,
      "created_at": "2016-10-13T13:39:24.217Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 3,
      "updated_at": "2016-10-13T13:39:24.232Z",
      "author_id": "17",
      "thread_subject_id": "8",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 4,
      "created_at": "2016-10-13T13:39:24.726Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 1,
      "updated_at": "2016-10-13T13:39:24.726Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 5,
      "created_at": "2016-10-13T13:39:25.112Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 2,
      "updated_at": "2016-10-13T13:39:25.112Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 6,
      "created_at": "2016-10-13T13:39:25.503Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 3,
      "updated_at": "2016-10-13T13:39:25.503Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 7,
      "created_at": "2016-10-13T13:39:25.807Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 4,
      "updated_at": "2016-10-13T13:39:25.807Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 8,
      "created_at": "2016-10-13T13:39:26.119Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 5,
      "updated_at": "2016-10-13T13:39:26.119Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 9,
      "created_at": "2016-10-13T13:39:26.449Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 6,
      "updated_at": "2016-10-13T13:39:26.449Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a48122cc2d4fa0a1f03f4b65d10d43f847afc8b266ef40f043b2946bf20ba81b"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/1
Content-Type: application/json
Authorization: Bearer 4f8276c95bf946a187347e5d2bb62f34a2799c4707574c5b74ed60483848b209
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-13T13:29:23.000Z"}}
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
    "id": 1,
    "created_at": "2016-10-13T13:39:23.937Z",
    "read_at": "2016-10-13T13:29:23.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 1,
    "updated_at": "2016-10-13T13:39:24.004Z",
    "author_id": "10",
    "thread_subject_id": "6",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/1" -d '{"notification":{"read_at":"2016-10-13T13:29:23.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f8276c95bf946a187347e5d2bb62f34a2799c4707574c5b74ed60483848b209"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer be63476f61311ed1107807dae29a57c1ca0ea15f751d6a00de0bb5e7a74f35f5
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
      "id": 2,
      "course_id": 118,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T13:40:00.139Z",
      "course_published": true,
      "updated_at": "2016-10-13T13:40:00.130Z"
    },
    {
      "id": 3,
      "course_id": 119,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-13T13:40:00.233Z",
      "course_published": true,
      "updated_at": "2016-10-13T13:40:00.224Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer be63476f61311ed1107807dae29a57c1ca0ea15f751d6a00de0bb5e7a74f35f5"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer b7fd5fd51b050a7f1d536325450aa0d83d140230a90d7b4f2a9de36a0d4ec978
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
    "course_id": 122,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-13T13:40:00.588Z",
    "course_published": true,
    "updated_at": "2016-10-13T13:40:00.579Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b7fd5fd51b050a7f1d536325450aa0d83d140230a90d7b4f2a9de36a0d4ec978"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/1
Content-Type: application/json
Authorization: Bearer 58f08eab04ed0f35e6ebe9053c4ea291639971da37a4ef89ac5bc523f9da48e2
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
    "id": 1,
    "course_id": 117,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-13T13:39:59.956Z",
    "course_published": true,
    "updated_at": "2016-10-13T13:39:59.943Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/1" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 58f08eab04ed0f35e6ebe9053c4ea291639971da37a4ef89ac5bc523f9da48e2"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer cb507ca2a2c8ea70b55e1c7b43f5899ac2f86de4e7af74385ea9f297ed4269b4
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
      "id": 15,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 80,
      "user_id": 601
    },
    {
      "id": 16,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 81,
      "user_id": 601
    },
    {
      "id": 17,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 82,
      "user_id": 601
    },
    {
      "id": 18,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 83,
      "user_id": 601
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb507ca2a2c8ea70b55e1c7b43f5899ac2f86de4e7af74385ea9f297ed4269b4"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/285
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
    "id": 285,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 285,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 285
      },
      {
        "id": 286,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 285
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/285" -X GET \
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
      "id": 286,
      "name": "Cross-platform background installation",
      "name_translations": {
        "en": "Cross-platform background installation"
      }
    },
    {
      "id": 287,
      "name": "Synergized full-range capability",
      "name_translations": {
        "en": "Synergized full-range capability"
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
PATCH /v2/feedbacks/17/close
Content-Type: application/json
Authorization: Bearer 4eb4ad680fd837989fcf1c5132ac68c57907271f2fa6a50d638ec204ea008e9e
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
    "id": 17,
    "user_id": 309,
    "feedbackable_id": 49,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-13T13:39:45.970Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/17/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4eb4ad680fd837989fcf1c5132ac68c57907271f2fa6a50d638ec204ea008e9e"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/10/fix
Content-Type: application/json
Authorization: Bearer d4d8a25f4234daf8a84d3a7e226dc5fc29c8cc8304fa30a19aab1cf4fd3130ce
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
    "id": 10,
    "user_id": 272,
    "feedbackable_id": 42,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-13T13:39:44.103Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/10/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4d8a25f4234daf8a84d3a7e226dc5fc29c8cc8304fa30a19aab1cf4fd3130ce"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/14
Content-Type: application/json
Authorization: Bearer 836fa1664331f3c0baac6d5046cb596a8187ec46264938ba2ccbc8fd5892fece
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
    "id": 14,
    "user_id": 292,
    "feedbackable_id": 46,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T13:39:45.292Z",
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
curl "api.goskive.com/v2/feedbacks/14" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 836fa1664331f3c0baac6d5046cb596a8187ec46264938ba2ccbc8fd5892fece"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/12/fix
Content-Type: application/json
Authorization: Bearer f1813bd15e10d7f3e95cff547f14ab18d2050b491cff2432aef62dca04a3e0ea
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
curl "api.goskive.com/v2/feedbacks/12/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1813bd15e10d7f3e95cff547f14ab18d2050b491cff2432aef62dca04a3e0ea"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/13/fix
Content-Type: application/json
Authorization: Bearer 1398d8eb633927fc7e3e29c0c1d4cf1066fb7a4471b38ed249c23aafca4c7edd
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
curl "api.goskive.com/v2/feedbacks/13/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1398d8eb633927fc7e3e29c0c1d4cf1066fb7a4471b38ed249c23aafca4c7edd"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/16/close
Content-Type: application/json
Authorization: Bearer f6f025eecb3b1538eb19c02a23a47d91e8958bd8828bf2ce40578bf2018d2a7c
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
curl "api.goskive.com/v2/feedbacks/16/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6f025eecb3b1538eb19c02a23a47d91e8958bd8828bf2ce40578bf2018d2a7c"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/15
Content-Type: application/json
Authorization: Bearer 177adca3b32b4e3b61e7ebf6b953f66664d7e80e3df5bcdcb52052cd9d4ce9c5
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
    "id": 15,
    "user_id": 297,
    "feedbackable_id": 47,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T13:39:45.575Z",
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
curl "api.goskive.com/v2/feedbacks/15" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 177adca3b32b4e3b61e7ebf6b953f66664d7e80e3df5bcdcb52052cd9d4ce9c5"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/7
Authorization: Bearer d0c17fc27a8ee72189747a54bea711a4bcd71c8045fdca3482291b5dc9b732ef
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
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Authorization: Bearer d0c17fc27a8ee72189747a54bea711a4bcd71c8045fdca3482291b5dc9b732ef" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Authorization: Bearer 03cdf28836aa6d97310896fabe466ece1c471e6c66b7f06da61d4d18ec1d24be
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
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Authorization: Bearer 03cdf28836aa6d97310896fabe466ece1c471e6c66b7f06da61d4d18ec1d24be" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/9
Authorization: Bearer 074d90c9c1a2d4d449e0c0c65913d4dbac45e5adfd3051c39036a54358fc61ec
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/dcfb37323777d7731c73824daaac1223.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T134001Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=b1d5fb0c1b7cd49f93547d5a9f4661277bb219c5b8f185bbbd98560b317488a5"
  }
}
```



```shell
curl "api.goskive.com/v2/files/9" -X GET \
	-H "Authorization: Bearer 074d90c9c1a2d4d449e0c0c65913d4dbac45e5adfd3051c39036a54358fc61ec"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Authorization: Bearer 3c792c655edcd4058c517982f351b0712ab7bfb31f7da191886213c735829d37
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
      "id": 485,
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
      "created_at": "2016-10-13T13:40:01.787Z",
      "updated_at": "2016-10-13T13:40:01.787Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "created_at": "2016-10-13T13:40:01.865Z",
    "updated_at": "2016-10-13T13:40:01.865Z",
    "course_id": 129,
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
	-H "Authorization: Bearer 3c792c655edcd4058c517982f351b0712ab7bfb31f7da191886213c735829d37" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/12/matched_courses
Authorization: Bearer 092fd16fb3b4cf35360170d69b1c3d2a7f91cbae1cbb0de6cd35156c1c81886b
```

`GET /v2/files/:file_id/matched_courses`

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
      "creator_id": 498,
      "id": 132,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 133,
      "additional_university_ids": [

      ],
      "topic_id": 137,
      "discipline_id": 137,
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
      "chapters_updated_at": "2016-10-13T13:40:01.914Z",
      "updated_at": "2016-10-13T13:40:03.943Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 503,
      "id": 133,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-33f019d8-c67d-42c7-864f-56e0db2a4752",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-33f019d8-c67d-42c7-864f-56e0db2a4752",
      "slug": "mit-the-great-british-bake-off-33f019d8-c67d-42c7-864f-56e0db2a4752",
      "university_id": 134,
      "additional_university_ids": [

      ],
      "topic_id": 138,
      "discipline_id": 138,
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
      "chapters_updated_at": "2016-10-13T13:40:01.914Z",
      "updated_at": "2016-10-13T13:40:04.619Z",
      "shortname": "mit-the-great-british-bake-off-33f019d8-c67d-42c7-864f-56e0db2a4752"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/12/matched_courses" -X GET \
	-H "Authorization: Bearer 092fd16fb3b4cf35360170d69b1c3d2a7f91cbae1cbb0de6cd35156c1c81886b"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/10/preview
Authorization: Bearer bfde86c5945733da6317a0281bc73458eadebc9058817c4b6cc6c6feb8f935f1
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/325465fcc84dbeb79d32b4fc2d3c5240.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161013%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161013T134001Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=81bdf647f42b75f56ca19a93376f110b71f2da9e66c909083ddbd6e209386eb4"
  }
}
```



```shell
curl "api.goskive.com/v2/files/10/preview" -X GET \
	-H "Authorization: Bearer bfde86c5945733da6317a0281bc73458eadebc9058817c4b6cc6c6feb8f935f1"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/5/report
Authorization: Bearer ae1b76e9ff58a1d762d66556e765a043c387f5a03fcaf1e48fbffa7fb53c5061
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
curl "api.goskive.com/v2/files/5/report" -d '' -X PUT \
	-H "Authorization: Bearer ae1b76e9ff58a1d762d66556e765a043c387f5a03fcaf1e48fbffa7fb53c5061" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/17/comments
Content-Type: application/json
Authorization: Bearer af6f0828968d8026d6c0e860f1f78efab38c0eef819f61435c00f8382926b5c4
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
    "author_id": 136,
    "reply_to_id": null,
    "created_at": "2016-10-13T13:39:33.513Z",
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
curl "api.goskive.com/v2/flashcards/17/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af6f0828968d8026d6c0e860f1f78efab38c0eef819f61435c00f8382926b5c4"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/15/comments
Content-Type: application/json
Authorization: Bearer 02104f32de6c96b7d10b64660931193262091e3151ad514cb772c5bf3b3d502c
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
    "author_id": 130,
    "reply_to_id": null,
    "created_at": "2016-10-13T13:39:32.990Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 9,
      "user_id": 130,
      "feedbackable_id": 15,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:32.988Z",
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
curl "api.goskive.com/v2/flashcards/15/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 02104f32de6c96b7d10b64660931193262091e3151ad514cb772c5bf3b3d502c"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/13/comments
Content-Type: application/json
Authorization: Bearer 48d85baa3014d5a516ae5efd248296bd46589ce4bdc51cef017f3c3343819005
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
      "author_id": 125,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:39:32.558Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 126,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:39:32.574Z",
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
curl "api.goskive.com/v2/flashcards/13/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48d85baa3014d5a516ae5efd248296bd46589ce4bdc51cef017f3c3343819005"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/16/comments
Content-Type: application/json
Authorization: Bearer a8d129c1d2383a847456047d2076a581c87270d272332f7f24b7b679d0dc3443
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
curl "api.goskive.com/v2/flashcards/16/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8d129c1d2383a847456047d2076a581c87270d272332f7f24b7b679d0dc3443"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/6/feedbacks
Content-Type: application/json
Authorization: Bearer 5147ff145f332a804d86bc4788255a530a4b5dd27ba8a9c8b791c9bff684dd56
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
    "user_id": 89,
    "feedbackable_id": 6,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-13T13:39:30.885Z",
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
curl "api.goskive.com/v2/flashcards/6/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5147ff145f332a804d86bc4788255a530a4b5dd27ba8a9c8b791c9bff684dd56"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/9/feedbacks
Content-Type: application/json
Authorization: Bearer 13c458f6cdb74202a5e763ded188d970ff4b0ca375e2bf10c4d0dff4635f7888
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
      "user_id": 110,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:31.742Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 109,
      "feedbackable_id": 9,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:31.730Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/9/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13c458f6cdb74202a5e763ded188d970ff4b0ca375e2bf10c4d0dff4635f7888"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/53/votes
Content-Type: application/json
Authorization: Bearer 19b12f2731e069b0897840389ce50e38d9206947a58035de6208659be24ec4ed
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
      "votable_id": 53,
      "user_id": 452
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 53,
      "user_id": 451
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 53,
      "user_id": 450
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/53/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19b12f2731e069b0897840389ce50e38d9206947a58035de6208659be24ec4ed"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/36/republish
Content-Type: application/json
Authorization: Bearer 4d4706f9fe77ced30b3558cabdd1af5e0733b4e051cbaf676e8481e35a2c5482
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
curl "api.goskive.com/v2/flashcards/36/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d4706f9fe77ced30b3558cabdd1af5e0733b4e051cbaf676e8481e35a2c5482"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/bookmark
Content-Type: application/json
Authorization: Bearer 8b19ae7701a12dbce71ca9129a34239abd145654523dbbf1723f72943a9e4a89
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b19ae7701a12dbce71ca9129a34239abd145654523dbbf1723f72943a9e4a89"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/41
Content-Type: application/json
Authorization: Bearer def67fac461033ee99e5525ea412a8488ddc7794dd27f9e970bffbd9374e9f0d
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/41" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer def67fac461033ee99e5525ea412a8488ddc7794dd27f9e970bffbd9374e9f0d"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/33/downvote
Content-Type: application/json
Authorization: Bearer a74177fc793bf7cc231f71bca7bae7264c5ce0a26d954e6cfc512cf147ca99df
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/33/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a74177fc793bf7cc231f71bca7bae7264c5ce0a26d954e6cfc512cf147ca99df"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/39
Content-Type: application/json
Authorization: Bearer 9848fbf6d1f3ae035468d599b424f81fd6497ec04e2e829ea47d77095ed0e61c
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
    "id": 39,
    "obfuscated_id": "N0Vv2_jrTfU",
    "author_id": 244,
    "chapter_id": 56,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:39:42.601Z",
    "created_at": "2016-10-13T13:39:42.601Z",
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
curl "api.goskive.com/v2/flashcards/39" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9848fbf6d1f3ae035468d599b424f81fd6497ec04e2e829ea47d77095ed0e61c"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/38/report
Content-Type: application/json
Authorization: Bearer b6f1efa919ac07923555dc3d7ac70b229ab089c0573a932bcb8f60f7ff03fabb
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/38/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6f1efa919ac07923555dc3d7ac70b229ab089c0573a932bcb8f60f7ff03fabb"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/34/bookmark
Content-Type: application/json
Authorization: Bearer 97db3320d1c13f0f4f82fa699d6a1e8008c801a2b6009153605fd5824fda8e6f
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 97db3320d1c13f0f4f82fa699d6a1e8008c801a2b6009153605fd5824fda8e6f"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/40/upvote
Content-Type: application/json
Authorization: Bearer 7f97a7d4b86ef9058ffa4c42c7e5064ff7d06c24d060db71f36efdba502db2e8
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/40/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f97a7d4b86ef9058ffa4c42c7e5064ff7d06c24d060db71f36efdba502db2e8"
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
    "key": "cache/ff7c1275228f283cf03509caad180e24.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xM1QxNDozOTo1OVoiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9mZjdjMTI3NTIyOGYyODNjZjAzNTA5Y2FhZDE4MGUyNC5qcGcifSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxMy9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTNUMTMzOTU5WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161013/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161013T133959Z",
    "x-amz-signature": "db279eb5b95ea8d3610e365cd1c71685f34a1970d33f38cf85378a2a0486e3f3"
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
Authorization: Bearer 9875b2c3bcc0467e88ec2391d76aa3befe2eb5b971686cd310cfdcd6ab23987d
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
	-H "Authorization: Bearer 9875b2c3bcc0467e88ec2391d76aa3befe2eb5b971686cd310cfdcd6ab23987d"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/1/sign_ups
Content-Type: application/json
Authorization: Bearer d791e0efecf811672af2fe704f383cf575038c0169a04f6762cd90f502b08eca
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
	-H "Authorization: Bearer d791e0efecf811672af2fe704f383cf575038c0169a04f6762cd90f502b08eca"
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
{"password":{"reset_password_token":"SQDM8aZoTm_XDSf2xve_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 156,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-13T13:39:36.242Z",
  "updated_at": "2016-10-13T13:39:36.450Z",
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
  "audit_id": 3309
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"SQDM8aZoTm_XDSf2xve_","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
Authorization: Bearer 289c01c01763a64d1f20df4886c1be52c9439743a24ada426f8bbbdfb6443c7c
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
    "id": 17,
    "author_id": 420,
    "reply_to_id": null,
    "created_at": "2016-10-13T13:39:56.449Z",
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
	-H "Authorization: Bearer 289c01c01763a64d1f20df4886c1be52c9439743a24ada426f8bbbdfb6443c7c"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/40/comments
Content-Type: application/json
Authorization: Bearer 7896c41ed2f01c2eecbc1271c8ad26238bc68bd47ff8d0ad6bba59e18e280dd1
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
    "id": 16,
    "author_id": 414,
    "reply_to_id": null,
    "created_at": "2016-10-13T13:39:55.559Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 38,
      "user_id": 414,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:39:55.557Z",
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
curl "api.goskive.com/v2/questions/40/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7896c41ed2f01c2eecbc1271c8ad26238bc68bd47ff8d0ad6bba59e18e280dd1"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/39/comments
Content-Type: application/json
Authorization: Bearer 77ef150f509d3f2d891149589e3324a92915483760661a1be70cec5e5ae1c3bb
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
      "id": 15,
      "author_id": 413,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:39:55.144Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 412,
      "reply_to_id": null,
      "created_at": "2016-10-13T13:39:55.127Z",
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
curl "api.goskive.com/v2/questions/39/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77ef150f509d3f2d891149589e3324a92915483760661a1be70cec5e5ae1c3bb"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/41/comments
Content-Type: application/json
Authorization: Bearer a69c0dfa1df6fd860bf51f650e5064be5f9b1e7381f557a8dd21ab70b6c083f1
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
curl "api.goskive.com/v2/questions/41/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a69c0dfa1df6fd860bf51f650e5064be5f9b1e7381f557a8dd21ab70b6c083f1"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/95/feedbacks
Content-Type: application/json
Authorization: Bearer 6a1a45d0c8c2d7be800c5ee4259979f7a34254cf3f6bc6b63e67449a6c2d530e
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
    "id": 46,
    "user_id": 710,
    "feedbackable_id": 95,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-13T13:40:27.411Z",
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
curl "api.goskive.com/v2/questions/95/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6a1a45d0c8c2d7be800c5ee4259979f7a34254cf3f6bc6b63e67449a6c2d530e"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/88/feedbacks
Content-Type: application/json
Authorization: Bearer d7062fef96100a7b3c43f3a08e8755543aa282b9548644cc7dcfa5ead36206f2
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
      "id": 40,
      "user_id": 681,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:40:24.819Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 680,
      "feedbackable_id": 88,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T13:40:24.806Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/88/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7062fef96100a7b3c43f3a08e8755543aa282b9548644cc7dcfa5ead36206f2"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/99/votes
Content-Type: application/json
Authorization: Bearer 14c814f7b6940e14d649cd9544c621bb05a8f201c18bebb6fc9907fde917bb5d
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
      "votable_id": 99,
      "user_id": 869
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 99,
      "user_id": 868
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 99,
      "user_id": 867
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/99/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14c814f7b6940e14d649cd9544c621bb05a8f201c18bebb6fc9907fde917bb5d"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/75/republish
Content-Type: application/json
Authorization: Bearer 7d4081cd557b49f9ac12b9ca07fa66793c70d4d39a1b0bdf104983f105d1814a
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
curl "api.goskive.com/v2/questions/75/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d4081cd557b49f9ac12b9ca07fa66793c70d4d39a1b0bdf104983f105d1814a"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/55/bookmark
Content-Type: application/json
Authorization: Bearer d7901056489f71238b5a7939aa4deb96a661e282c1290aaee6f21a5f1928f634
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/55/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7901056489f71238b5a7939aa4deb96a661e282c1290aaee6f21a5f1928f634"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/78
Content-Type: application/json
Authorization: Bearer 1bf072c7e9d95d1c62f083d8370fdb83e34917cb20b06b821b467a063da9003d
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/78" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bf072c7e9d95d1c62f083d8370fdb83e34917cb20b06b821b467a063da9003d"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/56/downvote
Content-Type: application/json
Authorization: Bearer 041c719668145d835c22635043edffd32b8d47a47b44a4c3f815a5597432ae23
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/56/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 041c719668145d835c22635043edffd32b8d47a47b44a4c3f815a5597432ae23"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/73
Content-Type: application/json
Authorization: Bearer 44b5fb712a5dfab6fb284a06a6bed2b5f21402342729790b35bfce98043cd053
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
    "id": 73,
    "obfuscated_id": "LJvjpBojvP0",
    "author_id": 579,
    "chapter_id": 122,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:13.037Z",
    "created_at": "2016-10-13T13:40:12.862Z",
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
        "id": 146,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 147,
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
curl "api.goskive.com/v2/questions/73" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44b5fb712a5dfab6fb284a06a6bed2b5f21402342729790b35bfce98043cd053"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/76/report
Content-Type: application/json
Authorization: Bearer ce15926d1420659d3b3ccf8ed82a614261000f892c4a4dcb4e943e5cefeab0f6
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/76/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce15926d1420659d3b3ccf8ed82a614261000f892c4a4dcb4e943e5cefeab0f6"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/72/bookmark
Content-Type: application/json
Authorization: Bearer c4a59ae585385e3067175804e91b02d08155cf41e7084434669d38487d24d9c0
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/72/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4a59ae585385e3067175804e91b02d08155cf41e7084434669d38487d24d9c0"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/54
Content-Type: application/json
Authorization: Bearer 1ecab2e3697b91a0cd394b0f52763a7c37be567f83b8fcc0e46dd007cc6dcb57
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":54,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T13:40:05.254Z","updated_at":"2016-10-13T13:40:05.415Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":103,"author_id":517,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 54,
    "obfuscated_id": "cKxlQSpHm5w",
    "author_id": 517,
    "chapter_id": 103,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-13T13:40:05.572Z",
    "created_at": "2016-10-13T13:40:05.254Z",
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
    "question": "{\"id\"=>54, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-13T13:40:05.254Z\", \"updated_at\"=>\"2016-10-13T13:40:05.415Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>103, \"author_id\"=>517, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 107,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 108,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 109,
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
curl "api.goskive.com/v2/questions/54" -d '{"question":{"question":{"id":54,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-13T13:40:05.254Z","updated_at":"2016-10-13T13:40:05.415Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":103,"author_id":517,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ecab2e3697b91a0cd394b0f52763a7c37be567f83b8fcc0e46dd007cc6dcb57"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/77/upvote
Content-Type: application/json
Authorization: Bearer 66ac36c9bf3c7ef2d7165f648a7b2fb01fe4ffaed1455009e5160f5a00baa898
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/77/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 66ac36c9bf3c7ef2d7165f648a7b2fb01fe4ffaed1455009e5160f5a00baa898"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer e2af763dddea87e56f8f3ee169f10428b06486b210c044703f09919593d4ecc5
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
      "creator_id": 3,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 4,
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
      "updated_at": "2016-10-13T13:39:23.382Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2af763dddea87e56f8f3ee169f10428b06486b210c044703f09919593d4ecc5"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 79a66cd752adec463b02b7556b68c261dd8873c5a912479238d0895f16d7f945
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
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-2",
      "html_url": "https://goskive.com/university/uni-2",
      "slug": "uni-2",
      "name": "National School of Pizza",
      "short_name": "Uni 2",
      "acronym": "NSPI",
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
      "updated_at": "2016-10-13T13:39:23.079Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 1,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-1",
      "html_url": "https://goskive.com/university/uni-1",
      "slug": "uni-1",
      "name": "National School of Pastry",
      "short_name": "Uni 1",
      "acronym": "NSPA",
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
      "updated_at": "2016-10-13T13:39:23.061Z",
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
	-H "Authorization: Bearer 79a66cd752adec463b02b7556b68c261dd8873c5a912479238d0895f16d7f945"
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
      "id": 290,
      "name": "Enterprise-wide zero defect project",
      "name_translations": {
        "en": "Enterprise-wide zero defect project"
      },
      "discipline_id": 291
    },
    {
      "id": 291,
      "name": "Phased contextually-based approach",
      "name_translations": {
        "en": "Phased contextually-based approach"
      },
      "discipline_id": 292
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
GET /v2/topics/292
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
    "id": 292,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 293
  }
}
```



```shell
curl "api.goskive.com/v2/topics/292" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer f3c31d48ddf958e5a4b55fa96749bd3fe901dac7cfb55dbfc0c7d50771d8a098
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
      "id": 202,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-182",
      "html_url": "https://goskive.com/university/uni-182",
      "slug": "uni-182",
      "name": "University 158",
      "short_name": "Uni 182",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/53cf0a027dec3ee4e219225f175ad0a6ac708abb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/150da6941a7bb6c0ffb622257f3bfc4c9455017e.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T13:40:27.769Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 203,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-183",
      "html_url": "https://goskive.com/university/uni-183",
      "slug": "uni-183",
      "name": "University 159",
      "short_name": "Uni 183",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/0787bd81d62837873bedc17bd0d5aeee4e9334b9.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/ff1205fa3f7bcacb835982cda574c9a4b422b51f.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T13:40:27.787Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 204,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-184",
      "html_url": "https://goskive.com/university/uni-184",
      "slug": "uni-184",
      "name": "University 160",
      "short_name": "Uni 184",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/42dd9c34213a9a543905d58e4769eb52a519a76e.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/29fa93d677a3211d73830c53d8f094dc24d853fe.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-13T13:40:27.805Z",
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
	-H "Authorization: Bearer f3c31d48ddf958e5a4b55fa96749bd3fe901dac7cfb55dbfc0c7d50771d8a098"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 3e2de8404a40b558ad26ee046517f14fb4663097126ebbe8af7e5adc589fd4c7
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
    "id": 201,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/c6b5e9f1fb6370af948a5cc219cde0f47ac91fad.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e9114493bd3e35fdb90895fdaee6349e1d673847.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-13T13:40:27.707Z",
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
	-H "Authorization: Bearer 3e2de8404a40b558ad26ee046517f14fb4663097126ebbe8af7e5adc589fd4c7"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d06e0c22ef474ad3f701eedcd8de1a78b774ecae15461254fd1e431bed6e8835
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":177,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 629,
    "id": 172,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 173,
    "additional_university_ids": [

    ],
    "topic_id": 177,
    "discipline_id": 177,
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
    "chapters_updated_at": "2016-10-13T13:40:19.647Z",
    "updated_at": "2016-10-13T13:40:19.799Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 133,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-13T13:40:19.743Z",
        "course_id": 172,
        "author_id": 629,
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
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-13T13:40:19.765Z",
        "course_id": 172,
        "author_id": 629,
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
        "id": 135,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-13T13:40:19.787Z",
        "course_id": 172,
        "author_id": 629,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":177,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d06e0c22ef474ad3f701eedcd8de1a78b774ecae15461254fd1e431bed6e8835"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer dbbc9c131783ee708bcaaf5f646dfd708e58e4000cdfaefa6a0f4a5d59ef56d6
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":178,"published":false}}
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
    "creator_id": 630,
    "id": 173,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 174,
    "additional_university_ids": [

    ],
    "topic_id": 178,
    "discipline_id": 178,
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
    "updated_at": "2016-10-13T13:40:19.957Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":178,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dbbc9c131783ee708bcaaf5f646dfd708e58e4000cdfaefa6a0f4a5d59ef56d6"
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
      "creator_id": 647,
      "id": 189,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 181,
      "additional_university_ids": [

      ],
      "topic_id": 194,
      "discipline_id": 194,
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
      "updated_at": "2016-10-13T13:40:21.751Z",
      "shortname": "fu-course-156"
    },
    {
      "creator_id": 647,
      "id": 190,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-157",
      "html_url": "https://goskive.com/course/fu-course-157",
      "slug": "fu-course-157",
      "university_id": 181,
      "additional_university_ids": [

      ],
      "topic_id": 195,
      "discipline_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 157",
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
      "chapters_updated_at": "2016-10-13T13:40:22.103Z",
      "updated_at": "2016-10-13T13:40:22.111Z",
      "shortname": "fu-course-157"
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
Authorization: Bearer 89a878df52d91b0af934008c474e8029e1f6d0074aca9c1b78a598a6f4296e01
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
      "creator_id": 664,
      "id": 205,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-172",
      "html_url": "https://goskive.com/course/fu-course-172",
      "slug": "fu-course-172",
      "university_id": 187,
      "additional_university_ids": [

      ],
      "topic_id": 210,
      "discipline_id": 210,
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
      "updated_at": "2016-10-13T13:40:23.454Z",
      "shortname": "fu-course-172"
    },
    {
      "creator_id": 664,
      "id": 206,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-173",
      "html_url": "https://goskive.com/course/fu-course-173",
      "slug": "fu-course-173",
      "university_id": 187,
      "additional_university_ids": [

      ],
      "topic_id": 211,
      "discipline_id": 211,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 173",
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
      "chapters_updated_at": "2016-10-13T13:40:23.757Z",
      "updated_at": "2016-10-13T13:40:23.764Z",
      "shortname": "fu-course-173"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 89a878df52d91b0af934008c474e8029e1f6d0074aca9c1b78a598a6f4296e01"
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
      "creator_id": 652,
      "id": 193,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-160",
      "html_url": "https://goskive.com/course/fu-course-160",
      "slug": "fu-course-160",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "topic_id": 198,
      "discipline_id": 198,
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
      "updated_at": "2016-10-13T13:40:22.302Z",
      "shortname": "fu-course-160"
    },
    {
      "creator_id": 652,
      "id": 194,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-161",
      "html_url": "https://goskive.com/course/fu-course-161",
      "slug": "fu-course-161",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "topic_id": 199,
      "discipline_id": 199,
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
      "updated_at": "2016-10-13T13:40:22.343Z",
      "shortname": "fu-course-161"
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
Authorization: Bearer 0bc9c34f1502675900a26288e2093a8fabd266372f3ffd307db45ed3b9198517
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
      "creator_id": 671,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "topic_id": 214,
      "discipline_id": 214,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "updated_at": "2016-10-13T13:40:24.089Z",
      "shortname": "fu-course-176"
    },
    {
      "creator_id": 671,
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-177",
      "html_url": "https://goskive.com/course/fu-course-177",
      "slug": "fu-course-177",
      "university_id": 189,
      "additional_university_ids": [

      ],
      "topic_id": 215,
      "discipline_id": 215,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 177",
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
      "updated_at": "2016-10-13T13:40:24.130Z",
      "shortname": "fu-course-177"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bc9c34f1502675900a26288e2093a8fabd266372f3ffd307db45ed3b9198517"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 05d4bdb87b57004961087eada36d5eb5f3a64627e4eba9c559775a4d581b64d7
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
  "id": 440,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-13T13:39:58.606Z",
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
	-H "Authorization: Bearer 05d4bdb87b57004961087eada36d5eb5f3a64627e4eba9c559775a4d581b64d7"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/885
Content-Type: application/json
Authorization: Bearer 0bba88bfed3f77a01d979eb5951c3c39feb4f81683d11188ac6b6801cdbc6328
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
    "id": 885,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 267,
    "fields_of_study": [
      293,
      294
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-13T13:40:37.861Z",
    "updated_at": "2016-10-13T13:40:37.861Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/885" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bba88bfed3f77a01d979eb5951c3c39feb4f81683d11188ac6b6801cdbc6328"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/887
Content-Type: application/json
Authorization: Bearer 898535091577e564617f00fed78535d0d49344d22b827b6dee1fe1278a258322
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
    "id": 887,
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
    "created_at": "2016-10-13T13:40:37.950Z",
    "updated_at": "2016-10-13T13:40:37.950Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/887" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 898535091577e564617f00fed78535d0d49344d22b827b6dee1fe1278a258322"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/5
Content-Type: application/json
Authorization: Bearer d54d5c059cd67c5e2def4fa3ff9aaa13013cbc8be047c08f5dde6d9d938dbe32
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
	-H "Authorization: Bearer d54d5c059cd67c5e2def4fa3ff9aaa13013cbc8be047c08f5dde6d9d938dbe32"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/6
Content-Type: application/json
Authorization: Bearer 664b6b0238eefc8f63260c753bdd650f2851d15b2a0693c4809a12b059b5ae47
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
    "id": 6,
    "type": "UpVote",
    "votable_type": "Question",
    "votable_id": 15,
    "user_id": 150
  }
}
```



```shell
curl "api.goskive.com/v2/votes/6" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 664b6b0238eefc8f63260c753bdd650f2851d15b2a0693c4809a12b059b5ae47"
```
