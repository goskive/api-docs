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
Authorization: Basic NmQ1NjUxMzdjNjQzOWU1NGI4YjdjMmVkOTVlZGZkZjU0OTNjMzNmNWE1ODg3
YmRhMDBmZjY1ZDkyZTJmMzZhMTo2MDhjMDZkNDJlZWViYmJmNzBmNjY5N2I0
NWI3N2I4NmZiM2EyOGYyMzU3YmIxOTExOTAwNzFjY2M0ZTBhZDZm

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
	-u 6d565137c6439e54b8b7c2ed95edfdf5493c33f5a5887bda00ff65d92e2f36a1:608c06d42eeebbbf70f6697b45b77b86fb3a28f2357bb191190071ccc4e0ad6f
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
{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2d9b38f21ceec44d2bbb688c4b0f1886d35278e328c86f80bc8ab7a3838bcdce","client_secret":"89236ba7d087bb56e7462bb28af77825d9fed8c618cf73ca2dc9f84301d11747"}
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
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.com","password":"wrongpassw0rd","client_id":"2d9b38f21ceec44d2bbb688c4b0f1886d35278e328c86f80bc8ab7a3838bcdce","client_secret":"89236ba7d087bb56e7462bb28af77825d9fed8c618cf73ca2dc9f84301d11747"}' -X POST \
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
{"grant_type":"client_credentials","client_id":"ca426b699e0ceca7e429fa7ae79506916b48164e43f4600cbb94c3016e2241c9","client_secret":"54c445d103c953c6c7e5b31f1e7df27986a4661c47656918693597dbfa1153da"}
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
  "access_token": "0ab4ed8bab0d4fc9c94af223568551151f247d291b7cdd5b547ef2d88ef5ce12",
  "token_type": "bearer",
  "created_at": 1476867643
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"client_credentials","client_id":"ca426b699e0ceca7e429fa7ae79506916b48164e43f4600cbb94c3016e2241c9","client_secret":"54c445d103c953c6c7e5b31f1e7df27986a4661c47656918693597dbfa1153da"}' -X POST \
	-H "Content-Type: application/json"
```
## Create a token


### Request

#### Endpoint

```
POST /v2/oauth/token
Content-Type: application/json
Authorization: Basic OTViNzJhZTdiMzJmNjZmY2NlNTNhZTA1OGQyYTFlYzA0ZGYxNTc4YjIyMDE4
NTkyYjZmMTRjMTE1NTU4ODZjNzplYTU0MTJjYjU1MzhkOWRjYTUxNjUzZjFm
MjY5MmVkOGY5NjQ5NzVjNDE2Njk4MDJmNmFmNTBhOGE1N2JhYTcz

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
  "access_token": "c411a30bbd5fe768b66ae888e60d98c0971dac80493a1d0378823c293c7f5494",
  "token_type": "bearer",
  "created_at": 1476867643
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli"}' -X POST \
	-H "Content-Type: application/json" \
	-u 95b72ae7b32f66fcce53ae058d2a1ec04df1578b22018592b6f14c11555886c7:ea5412cb5538d9dca51653f1f2692ed8f964975c41669802f6af50a8a57baa73
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
{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"d834138e1dc81c1a3c7126ca632bceaa55dd491dbff8d6148103496453968244","client_secret":"aa74c5cb81c2e758aa1274fe37550b9340d63d52e0b7efe906810aedc1aac180"}
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
  "access_token": "b9aebb95bd282c5f13032973847f7d22a7cf89d2d861318a81b452f9755693ba",
  "token_type": "bearer",
  "created_at": 1476867643
}
```



```shell
curl "api.goskive.com/v2/oauth/token" -d '{"grant_type":"password","username":"jan.turnosky@hotmail.sk","password":"Vykupiteli","client_id":"d834138e1dc81c1a3c7126ca632bceaa55dd491dbff8d6148103496453968244","client_secret":"aa74c5cb81c2e758aa1274fe37550b9340d63d52e0b7efe906810aedc1aac180"}' -X POST \
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
Authorization: Bearer c00669c9636c81917b581f2e3905e4b57b5d84762151360b2adc989101f7e73e
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
    "company_id": 12,
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
	-H "Authorization: Bearer c00669c9636c81917b581f2e3905e4b57b5d84762151360b2adc989101f7e73e"
```
# Chapter Flashcards

## Create a flashcard


### Request

#### Endpoint

```
POST /v2/chapters/35/flashcards
Content-Type: application/json
Authorization: Bearer cd518954e04e7add60310782c990b247d3e7c94910586c7936186b70a37ab4f2
```

`POST /v2/chapters/:chapter_id/flashcards`

#### Parameters


```json
{"flashcard":{"chapter_id":35,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}
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
    "id": 36,
    "obfuscated_id": "01Tx8eTrCOA",
    "author_id": 196,
    "chapter_id": 35,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:59:46.605Z",
    "created_at": "2016-10-19T08:59:46.605Z",
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
curl "api.goskive.com/v2/chapters/35/flashcards" -d '{"flashcard":{"chapter_id":35,"front_content_html":"Function of \u003cstrong\u003eeggs\u003c/strong\u003e in choux pastry","back_content_html":"Helps things \u003cstrong\u003eraise\u003c/strong\u003e","language_code":"fr"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd518954e04e7add60310782c990b247d3e7c94910586c7936186b70a37ab4f2"
```
## Get a list of chapter flashcards


### Request

#### Endpoint

```
GET /v2/chapters/37/flashcards
Content-Type: application/json
Authorization: Bearer d0eda4bd47f417dddae49e4e6d6348d04fb0f201668e8a9534affffef4ea5f0c
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
      "id": 37,
      "obfuscated_id": "95m_4XdR9PU",
      "author_id": 200,
      "chapter_id": 37,
      "position": 1,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:46.909Z",
      "created_at": "2016-10-19T08:59:46.909Z",
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
      "author_id": 200,
      "chapter_id": 37,
      "position": 2,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:46.947Z",
      "created_at": "2016-10-19T08:59:46.947Z",
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
      "author_id": 200,
      "chapter_id": 37,
      "position": 3,
      "reviewed": false,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T08:59:46.987Z",
      "created_at": "2016-10-19T08:59:46.987Z",
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
curl "api.goskive.com/v2/chapters/37/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0eda4bd47f417dddae49e4e6d6348d04fb0f201668e8a9534affffef4ea5f0c"
```
# Chapter Questions

## Create a multiple-choice question


### Request

#### Endpoint

```
POST /v2/chapters/147/questions
Content-Type: application/json
Authorization: Bearer 87df7ccfe4b830a6430cefface249cc2874c6abe346fc473dbfad8004d17b4b1
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":147,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}
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
    "author_id": 776,
    "chapter_id": 147,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T09:00:29.318Z",
    "created_at": "2016-10-19T09:00:29.318Z",
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
        "id": 228,
        "position": 1,
        "content": "Tomatoes",
        "content_html": "<p>Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 229,
        "position": 2,
        "content": "Flour",
        "content_html": "<p>Flour</p>",
        "correct": true
      },
      {
        "id": 230,
        "position": 3,
        "content": "Mozzarella",
        "content_html": "<p>Mozzarella.</p>",
        "correct": false
      },
      {
        "id": 231,
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
curl "api.goskive.com/v2/chapters/147/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":147,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Tomatoes","content_html":"\u003cp\u003eTomatoes.\u003c/p\u003e","correct":false},{"content":"Flour","content_html":"\u003cp\u003eFlour\u003c/p\u003e","correct":true},{"content":"Mozzarella","content_html":"\u003cp\u003eMozzarella.\u003c/p\u003e","correct":false},{"content":"Eggs","content_html":"\u003cp\u003eEggs\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 87df7ccfe4b830a6430cefface249cc2874c6abe346fc473dbfad8004d17b4b1"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/145/questions
Content-Type: application/json
Authorization: Bearer d0cdc9b8395ae8851cf03607176db08219f825a61b59f146e8843f961addbb4b
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 770,
    "chapter_id": 145,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T09:00:28.637Z",
    "created_at": "2016-10-19T09:00:28.637Z",
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
        "id": 224,
        "position": 1,
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 225,
        "position": 2,
        "content_html": "<p>Flour and eggs.</p>",
        "correct": true
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/145/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":145,"question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0cdc9b8395ae8851cf03607176db08219f825a61b59f146e8843f961addbb4b"
```
## Create a question


### Request

#### Endpoint

```
POST /v2/chapters/146/questions
Content-Type: application/json
Authorization: Bearer c3bd180fcdf01ddef0880ba6d1d211c6d36cc5c32490c475ed737d13e81901ab
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":146,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}
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
    "author_id": 773,
    "chapter_id": 146,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T09:00:28.983Z",
    "created_at": "2016-10-19T09:00:28.983Z",
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
        "id": 226,
        "position": 1,
        "content": "Mozzarella and Tomatoes",
        "content_html": "<p>Mozzarella and Tomatoes.</p>",
        "correct": false
      },
      {
        "id": 227,
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
curl "api.goskive.com/v2/chapters/146/questions" -d '{"question":{"explanation":"the explanation is simple: **eggs**","chapter_id":146,"question":"How do you make **Choux**?","question_html":"How do you make \u003cstrong\u003eChoux\u003c/strong\u003e?","explanation_html":"the explanation is simple: \u003cstrong\u003eeggs\u003c/strong\u003e","answer_options":[{"content":"Mozzarella and Tomatoes","content_html":"\u003cp\u003eMozzarella and Tomatoes.\u003c/p\u003e","correct":false},{"content":"Flour and eggs","content_html":"\u003cp\u003eFlour and eggs.\u003c/p\u003e","correct":true}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3bd180fcdf01ddef0880ba6d1d211c6d36cc5c32490c475ed737d13e81901ab"
```
## Create a single choice question


### Request

#### Endpoint

```
POST /v2/chapters/148/questions
Content-Type: application/json
Authorization: Bearer 09475e045f16a414d3494722e8cfae9bde77a5d49e0c17c96c8c775bf6c82de8
```

`POST /v2/chapters/:chapter_id/questions`

#### Parameters


```json
{"question":{"explanation":"Think about German humor.","chapter_id":148,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}
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
    "author_id": 779,
    "chapter_id": 148,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T09:00:29.812Z",
    "created_at": "2016-10-19T09:00:29.812Z",
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
        "id": 232,
        "position": 1,
        "content": "None. We use energy saving lamps.",
        "content_html": "<p>None. We use energy saving lamps.</p>",
        "correct": false
      },
      {
        "id": 233,
        "position": 2,
        "content": "One. We have no humor.",
        "content_html": "<p>One. We have no humor</p>",
        "correct": true
      },
      {
        "id": 234,
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
curl "api.goskive.com/v2/chapters/148/questions" -d '{"question":{"explanation":"Think about German humor.","chapter_id":148,"question":"How many Germans does it take to change a light bulb?","question_html":"How many Germans does it take to change a \u003cstrong\u003elight bulb\u003c/strong\u003e?","explanation_html":"Think about German \u003cstrong\u003ehumor\u003c/strong\u003e","answer_options":[{"content":"None. We use energy saving lamps.","content_html":"\u003cp\u003eNone. We use energy saving lamps.\u003c/p\u003e","correct":false},{"content":"One. We have no humor.","content_html":"\u003cp\u003eOne. We have no humor\u003c/p\u003e","correct":true},{"content":"Two. One that changes it and one that makes this joke work.","content_html":"\u003cp\u003eTwo. One that changes it and one that makes this joke work.\u003c/p\u003e","correct":false}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 09475e045f16a414d3494722e8cfae9bde77a5d49e0c17c96c8c775bf6c82de8"
```
## Get a list of chapter questions


### Request

#### Endpoint

```
GET /v2/chapters/149/questions
Content-Type: application/json
Authorization: Bearer 7c9a5f46dbc45220375bae5c8accfc736edf561575d0eacf1915252251702c2c
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
      "id": 116,
      "obfuscated_id": "PhHGVKqnHFA",
      "author_id": 782,
      "chapter_id": 149,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:30.309Z",
      "created_at": "2016-10-19T09:00:30.191Z",
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
      "author_id": 783,
      "chapter_id": 149,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:30.500Z",
      "created_at": "2016-10-19T09:00:30.381Z",
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
      "author_id": 784,
      "chapter_id": 149,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-19T09:00:30.698Z",
      "created_at": "2016-10-19T09:00:30.576Z",
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
```



```shell
curl "api.goskive.com/v2/chapters/149/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7c9a5f46dbc45220375bae5c8accfc736edf561575d0eacf1915252251702c2c"
```
# Chapters

## Authorisation error on delete

A student may not delete another chapter.

### Request

#### Endpoint

```
DELETE /v2/chapters/3
Content-Type: application/json
Authorization: Bearer 992d6b062454db7a7b5379d9cd033ed0d85a1b49b414623d72001d75b3f9a1eb
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
curl "api.goskive.com/v2/chapters/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 992d6b062454db7a7b5379d9cd033ed0d85a1b49b414623d72001d75b3f9a1eb"
```
## Authorisation error on delete

A student may not delete a chapter with content.

### Request

#### Endpoint

```
DELETE /v2/chapters/4
Content-Type: application/json
Authorization: Bearer 0fae7d51da1e393fafea38abe2765d73ce06f34e85033ec27a41aadfe5235648
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
curl "api.goskive.com/v2/chapters/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0fae7d51da1e393fafea38abe2765d73ce06f34e85033ec27a41aadfe5235648"
```
## Authorisation error on update

A student may not update another chapter.

### Request

#### Endpoint

```
PATCH /v2/chapters/8
Content-Type: application/json
Authorization: Bearer 9b340becb03fec248a62ea3f398f32c3faad10037421ff8113b651d9f30fd554
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
curl "api.goskive.com/v2/chapters/8" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b340becb03fec248a62ea3f398f32c3faad10037421ff8113b651d9f30fd554"
```
## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/5
Content-Type: application/json
Authorization: Bearer 3b8b7b5ab2206ce1d60355dc6fd8ef5c8248b7d807bbad0cae862e7959ac0395
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/5" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b8b7b5ab2206ce1d60355dc6fd8ef5c8248b7d807bbad0cae862e7959ac0395"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/2
Content-Type: application/json
Authorization: Bearer f6ada946fc935fbeb1d120bf2bed59ba4054373db10610670381752ed9005b6a
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
    "updated_at": "2016-10-19T08:59:26.516Z",
    "course_id": 2,
    "author_id": 9,
    "permissions": [

    ],
    "flashcards_updated_at": "2016-10-19T08:59:25.954Z",
    "questions_updated_at": "2016-10-19T08:59:25.954Z",
    "flashcards_count": 1,
    "questions_count": 1,
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 13,
        "chapter_id": 2,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:26.489Z",
        "created_at": "2016-10-19T08:59:26.489Z",
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
        "author_id": 11,
        "chapter_id": 2,
        "position": 4,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:26.369Z",
        "created_at": "2016-10-19T08:59:26.245Z",
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
	-H "Authorization: Bearer f6ada946fc935fbeb1d120bf2bed59ba4054373db10610670381752ed9005b6a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/9
Content-Type: application/json
Authorization: Bearer 4539b8b208536979236b37ccab8b1edd1d1c4a0f205f9d54ab7cf9b716f22a9a
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
    "updated_at": "2016-10-19T08:59:27.972Z",
    "course_id": 9,
    "author_id": 34,
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
	-H "Authorization: Bearer 4539b8b208536979236b37ccab8b1edd1d1c4a0f205f9d54ab7cf9b716f22a9a"
```
# Comment Replies

## Create a reply


### Request

#### Endpoint

```
POST /v2/comments/58/replies
Content-Type: application/json
Authorization: Bearer ae4b30ec7c0a2417666105328f483f20b6088c6b4d030e9f0f45a523d5044738
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
    "author_id": 964,
    "reply_to_id": 58,
    "created_at": "2016-10-19T09:00:44.076Z",
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
	-H "Authorization: Bearer ae4b30ec7c0a2417666105328f483f20b6088c6b4d030e9f0f45a523d5044738"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/comments/60/replies
Content-Type: application/json
Authorization: Bearer 1eee197f7cfb792f4841a2e7f945a08c822b863699762bf2540f40e3d85a4927
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
	-H "Authorization: Bearer 1eee197f7cfb792f4841a2e7f945a08c822b863699762bf2540f40e3d85a4927"
```
# Comments

## Authorisation error on delete

A student may not delete another comment.

### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer f1875ff063f2d90e81ffcc9361af5aab3b0ce6cbf409f39fb1af4335a2c3d22c
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
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1875ff063f2d90e81ffcc9361af5aab3b0ce6cbf409f39fb1af4335a2c3d22c"
```
## Authorisation error on republish

A student may not republish their own comment.

### Request

#### Endpoint

```
PUT /v2/comments/46/republish
Content-Type: application/json
Authorization: Bearer d219ad8f08360091d92460620efe4b75bb2f0821a20649b56901dce424a31c1d
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
curl "api.goskive.com/v2/comments/46/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d219ad8f08360091d92460620efe4b75bb2f0821a20649b56901dce424a31c1d"
```
## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/49
Content-Type: application/json
Authorization: Bearer 849e39d887b213fd03801f48f9b742282101527096264bdc340de32911b6bbde
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 849e39d887b213fd03801f48f9b742282101527096264bdc340de32911b6bbde"
```
## Report a comment


### Request

#### Endpoint

```
PUT /v2/comments/50/report
Content-Type: application/json
Authorization: Bearer e9c4261bb09fe1e72a09fa76721caf7852e273543e1f44f4afd3c0e67bd32096
```

`PUT /v2/comments/:comment_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/50/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9c4261bb09fe1e72a09fa76721caf7852e273543e1f44f4afd3c0e67bd32096"
```
# Companies

## Get a company


### Request

#### Endpoint

```
GET /v2/companies/16
Content-Type: application/json
Authorization: Bearer 46bf0a45c78e6a48b2d48a0ab7087025a1b0f4a8906545a83deca19f4adc3162
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
    "id": 16,
    "name": "Pastry Corp",
    "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/913e3ec20f37cbd6a1dfb047cea89954a97d5f29.png",
    "brand_color": "#ffcc00",
    "updated_at": "2016-10-19T08:59:46.402Z"
  }
}
```



```shell
curl "api.goskive.com/v2/companies/16" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46bf0a45c78e6a48b2d48a0ab7087025a1b0f4a8906545a83deca19f4adc3162"
```
## Get a list of companies


### Request

#### Endpoint

```
GET /v2/companies
Content-Type: application/json
Authorization: Bearer 9580bc0eda396a676d8a71c87527bb522528c3e44524f09152f5dd240e80b275
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
      "id": 13,
      "name": "Fake Company Name 9",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/5b8fcad03b420eed2a2157f47839d2410b3a056a.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:59:46.267Z"
    },
    {
      "id": 14,
      "name": "Fake Company Name 10",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/fc51f20685bc60599135bc56298d6e89ee56c5f5.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:59:46.272Z"
    },
    {
      "id": 15,
      "name": "Fake Company Name 11",
      "logo_url": "file:///home/ubuntu/skive-backend/public/system/companies/original/b8b92ea1b4add90b9256816b993b3558a1bb92c4.png",
      "brand_color": "#000000",
      "updated_at": "2016-10-19T08:59:46.276Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/companies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9580bc0eda396a676d8a71c87527bb522528c3e44524f09152f5dd240e80b275"
```
# Company Profiles

## Get a list of company profiles


### Request

#### Endpoint

```
GET /v2/companies/10/company_profiles
Content-Type: application/json
Authorization: Bearer babc034b7fea5548cf1ed3e188410dddb06fa35769438317e541cbbbaf9ea180
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
curl "api.goskive.com/v2/companies/10/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer babc034b7fea5548cf1ed3e188410dddb06fa35769438317e541cbbbaf9ea180"
```
## Get a list of company profiles with embedded widgets


### Request

#### Endpoint

```
GET /v2/companies/9/company_profiles
Content-Type: application/json
Authorization: Bearer b9efa652e0f3565220da62583859a6d1b83604bc228da352cc8883891a787fed
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
curl "api.goskive.com/v2/companies/9/company_profiles" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9efa652e0f3565220da62583859a6d1b83604bc228da352cc8883891a787fed"
```
# Course Campaigns

## Get a list of course campaigns


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/campaigns
Content-Type: application/json
Authorization: Bearer cb538bdd44214957b1de6ffa0ac81de46f429c9d574a8d67d4efd0b0042549a0
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
	-H "Authorization: Bearer cb538bdd44214957b1de6ffa0ac81de46f429c9d574a8d67d4efd0b0042549a0"
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
Authorization: Bearer a9c4f1e0f34ac93c338bdfcaa774da89b6fc7ee41be976bbb09ed4d22ddbab55
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
	-H "Authorization: Bearer a9c4f1e0f34ac93c338bdfcaa774da89b6fc7ee41be976bbb09ed4d22ddbab55"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b658ac390ec3369e474deb50366839b2920d8f57974d2944b98dda19aaf45ad5
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
    "id": 153,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-19T09:00:31.510Z",
    "course_id": 265,
    "author_id": 796,
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
	-H "Authorization: Bearer b658ac390ec3369e474deb50366839b2920d8f57974d2944b98dda19aaf45ad5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 74caa9068af73573cc59d041697953740f822558ead42ad90994910d84f974e7
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
      "title": "Clever Chapter Title 130",
      "position": 1,
      "updated_at": "2016-10-19T09:00:31.647Z",
      "course_id": 266,
      "author_id": 798,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 155,
      "title": "Clever Chapter Title 131",
      "position": 2,
      "updated_at": "2016-10-19T09:00:31.672Z",
      "course_id": 266,
      "author_id": 799,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 156,
      "title": "Clever Chapter Title 132",
      "position": 3,
      "updated_at": "2016-10-19T09:00:31.931Z",
      "course_id": 266,
      "author_id": 800,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T09:00:31.545Z",
      "questions_updated_at": "2016-10-19T09:00:31.545Z",
      "flashcards_count": 0,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 74caa9068af73573cc59d041697953740f822558ead42ad90994910d84f974e7"
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
      "id": 160,
      "title": "Clever Chapter Title 136",
      "position": 1,
      "updated_at": "2016-10-19T09:00:32.406Z",
      "course_id": 269,
      "author_id": 812,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 161,
      "title": "Clever Chapter Title 137",
      "position": 2,
      "updated_at": "2016-10-19T09:00:32.432Z",
      "course_id": 269,
      "author_id": 813,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 162,
      "title": "Clever Chapter Title 138",
      "position": 3,
      "updated_at": "2016-10-19T09:00:32.683Z",
      "course_id": 269,
      "author_id": 814,
      "permissions": [

      ],
      "flashcards_updated_at": "2016-10-19T09:00:32.327Z",
      "questions_updated_at": "2016-10-19T09:00:32.327Z",
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
Authorization: Bearer b32e27bb2df81bc8cafa85f9025909d4ac236f0f89d9dbf804dbc804e217cfca
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
      "title": "Clever Chapter Title 133",
      "position": 1,
      "updated_at": "2016-10-19T09:00:32.096Z",
      "course_id": 267,
      "author_id": 805,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 158,
      "title": "Clever Chapter Title 134",
      "position": 2,
      "updated_at": "2016-10-19T09:00:32.122Z",
      "course_id": 267,
      "author_id": 806,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 159,
      "title": "Clever Chapter Title 135",
      "position": 3,
      "updated_at": "2016-10-19T09:00:32.148Z",
      "course_id": 267,
      "author_id": 807,
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
	-H "Authorization: Bearer b32e27bb2df81bc8cafa85f9025909d4ac236f0f89d9dbf804dbc804e217cfca"
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
      "id": 163,
      "title": "Clever Chapter Title 139",
      "position": 1,
      "updated_at": "2016-10-19T09:00:32.880Z",
      "course_id": 271,
      "author_id": 819,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 164,
      "title": "Clever Chapter Title 140",
      "position": 2,
      "updated_at": "2016-10-19T09:00:32.905Z",
      "course_id": 271,
      "author_id": 820,
      "permissions": [

      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0
    },
    {
      "id": 165,
      "title": "Clever Chapter Title 141",
      "position": 3,
      "updated_at": "2016-10-19T09:00:32.930Z",
      "course_id": 271,
      "author_id": 821,
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
Authorization: Bearer c815f8e0e97a45e8bd3df3f42b2005ec7b93be8a55693a9f812f8beeb009c231
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
    "id": 2,
    "course_id": 278,
    "user_id": 846,
    "updated_at": "2016-10-19T09:00:34.318Z"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c815f8e0e97a45e8bd3df3f42b2005ec7b93be8a55693a9f812f8beeb009c231"
```
## Get a list of course course requests


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/course_requests
Content-Type: application/json
Authorization: Bearer 27cfe3092a274eea664ab24fa56da0662e00879dc97687d8077782c6cbabbcda
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
      "course_id": 279,
      "user_id": 848,
      "updated_at": "2016-10-19T09:00:34.410Z"
    },
    {
      "id": 4,
      "course_id": 279,
      "user_id": 849,
      "updated_at": "2016-10-19T09:00:34.426Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/course_requests" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 27cfe3092a274eea664ab24fa56da0662e00879dc97687d8077782c6cbabbcda"
```
# Course Files

## Get a list of course files


### Request

#### Endpoint

```
GET /v2/courses/150/files
Content-Type: application/json
Authorization: Bearer e8bad38e78bb3d16bc6904ca4d980dbf9028e49f691722145d6e594c1caf8068
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
      "id": 10,
      "uploader": {
        "id": 436,
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
        "created_at": "2016-10-19T09:00:06.524Z",
        "updated_at": "2016-10-19T09:00:06.524Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T09:00:06.531Z",
      "updated_at": "2016-10-19T09:00:06.531Z",
      "course_id": 150,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 11,
      "uploader": {
        "id": 437,
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
        "created_at": "2016-10-19T09:00:06.539Z",
        "updated_at": "2016-10-19T09:00:06.539Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T09:00:06.545Z",
      "updated_at": "2016-10-19T09:00:06.545Z",
      "course_id": 150,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    },
    {
      "id": 12,
      "uploader": {
        "id": 438,
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
        "created_at": "2016-10-19T09:00:06.552Z",
        "updated_at": "2016-10-19T09:00:06.552Z"
      },
      "status": "published",
      "download_count": 3000,
      "mime_type": "application/pdf",
      "size": 6893,
      "permissions": [

      ],
      "created_at": "2016-10-19T09:00:06.558Z",
      "updated_at": "2016-10-19T09:00:06.558Z",
      "course_id": 150,
      "filename": "101 of cheating",
      "category": "summary",
      "is_anonymous": false
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/150/files" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8bad38e78bb3d16bc6904ca4d980dbf9028e49f691722145d6e594c1caf8068"
```
## creates the file


### Request

#### Endpoint

```
POST /v2/courses/152/files
Content-Type: application/json
Authorization: Bearer e007c01e8f2c17f4964ce9b6584812ea456e50f121a05c4d10125c13e3c9bff4
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
    "id": 13,
    "uploader": {
      "id": 443,
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
      "created_at": "2016-10-19T09:00:06.788Z",
      "updated_at": "2016-10-19T09:00:06.788Z"
    },
    "status": "published",
    "download_count": 0,
    "mime_type": null,
    "size": null,
    "permissions": [

    ],
    "created_at": "2016-10-19T09:00:06.817Z",
    "updated_at": "2016-10-19T09:00:06.817Z",
    "course_id": 152,
    "filename": "who you gonna call?",
    "category": "summary",
    "is_anonymous": false
  }
}
```



```shell
curl "api.goskive.com/v2/courses/152/files" -d '{"file":{"category":"summary","filename":"who you gonna call?","file_url":"http://awkward-linkisch.com/file.pdf"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e007c01e8f2c17f4964ce9b6584812ea456e50f121a05c4d10125c13e3c9bff4"
```
## presigns an upload


### Request

#### Endpoint

```
GET /v2/courses/149/file_upload/cache/presign?extension=.jpg
Content-Type: application/json
Authorization: Bearer 85369e6a92e32cda7b226e9b61f5f08a6b37eed954112c3051a70b284ab526bb
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
    "key": "cache/b0c5babe92c43181762a4ee564318d9f.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxMDowMDowNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9iMGM1YmFiZTkyYzQzMTgxNzYyYTRlZTU2NDMxOGQ5Zi5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDUyNDI4ODAwXSx7IngtYW16LWNyZWRlbnRpYWwiOiJBS0lBSUdNRlkyWks3TFJYRUZSQS8yMDE2MTAxOS9ldS13ZXN0LTEvczMvYXdzNF9yZXF1ZXN0In0seyJ4LWFtei1hbGdvcml0aG0iOiJBV1M0LUhNQUMtU0hBMjU2In0seyJ4LWFtei1kYXRlIjoiMjAxNjEwMTlUMDkwMDA2WiJ9XX0=",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T090006Z",
    "x-amz-signature": "fb3f42fb7050d61587ce129bf35cb4c2c57ccc9ced9735461bbd721e22309bd2"
  }
}
```



```shell
curl "api.goskive.com/v2/courses/149/file_upload/cache/presign?extension=.jpg" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 85369e6a92e32cda7b226e9b61f5f08a6b37eed954112c3051a70b284ab526bb"
```
# Course Requests

## Delete a course request


### Request

#### Endpoint

```
DELETE /v2/course_requests/7
Content-Type: application/json
Authorization: Bearer 1c0e77e558304b846f9966530d16a714bc3eac621c9e9bbe4e7edf6ceb15032a
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
	-H "Authorization: Bearer 1c0e77e558304b846f9966530d16a714bc3eac621c9e9bbe4e7edf6ceb15032a"
```
# Courses

## Authorisation error on delete

A student may not delete another course.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 68435b52b2672b6fc49ab7e9a551eb35ad7b7bb8c553e069855c76cb7f58465b
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
	-H "Authorization: Bearer 68435b52b2672b6fc49ab7e9a551eb35ad7b7bb8c553e069855c76cb7f58465b"
```
## Authorisation error on delete

A student may not delete a course if it has content.

### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4c91cb230b6881e58c08aa012b206cdb60ecaa5d7640b8790e145fa39e1e07bd
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
	-H "Authorization: Bearer 4c91cb230b6881e58c08aa012b206cdb60ecaa5d7640b8790e145fa39e1e07bd"
```
## Authorisation error on update

A student may not update another course.

### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 6e4293dce0c14d9baeec80ca2deee0c1925f14c3ef7033e74d20a1d41b53a77e
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
	-H "Authorization: Bearer 6e4293dce0c14d9baeec80ca2deee0c1925f14c3ef7033e74d20a1d41b53a77e"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ed1195208bb720d3cb568a298c3a689b0f35a699eae125f669676108f0105c5f
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
	-H "Authorization: Bearer ed1195208bb720d3cb568a298c3a689b0f35a699eae125f669676108f0105c5f"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=questions%2C+flashcards
Content-Type: application/json
Authorization: Bearer 601d2d073df8efc2e7b6c850e14b94a3b10afc41fe95ab3c8ceb8c68bc32904f
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
    "creator_id": 143,
    "id": 70,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 49,
    "additional_university_ids": [

    ],
    "topic_id": 70,
    "discipline_id": 70,
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
    "chapters_updated_at": "2016-10-19T08:59:39.127Z",
    "updated_at": "2016-10-19T08:59:40.642Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 25,
        "title": "Clever Chapter Title 13",
        "position": 1,
        "updated_at": "2016-10-19T08:59:40.597Z",
        "course_id": 70,
        "author_id": 143,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:59:39.127Z",
        "questions_updated_at": "2016-10-19T08:59:39.127Z",
        "flashcards_count": 2,
        "questions_count": 2
      },
      {
        "id": 26,
        "title": "Clever Chapter Title 14",
        "position": 2,
        "updated_at": "2016-10-19T08:59:40.635Z",
        "course_id": 70,
        "author_id": 143,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:59:39.127Z",
        "questions_updated_at": "2016-10-19T08:59:39.127Z",
        "flashcards_count": 2,
        "questions_count": 2
      }
    ],
    "flashcards": [
      {
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 144,
        "chapter_id": 25,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:40.406Z",
        "created_at": "2016-10-19T08:59:40.406Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 144,
        "chapter_id": 26,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:40.511Z",
        "created_at": "2016-10-19T08:59:40.511Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 144,
        "chapter_id": 25,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:40.470Z",
        "created_at": "2016-10-19T08:59:40.470Z",
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
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 144,
        "chapter_id": 26,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:40.550Z",
        "created_at": "2016-10-19T08:59:40.550Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 144,
        "chapter_id": 25,
        "position": 22,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:39.392Z",
        "created_at": "2016-10-19T08:59:39.257Z",
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
            "id": 43,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 44,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 144,
        "chapter_id": 25,
        "position": 23,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:39.580Z",
        "created_at": "2016-10-19T08:59:39.462Z",
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
          }
        ]
      },
      {
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 144,
        "chapter_id": 26,
        "position": 24,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:39.775Z",
        "created_at": "2016-10-19T08:59:39.661Z",
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
            "id": 47,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 48,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 144,
        "chapter_id": 26,
        "position": 25,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:39.945Z",
        "created_at": "2016-10-19T08:59:39.836Z",
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
            "id": 49,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 50,
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
	-H "Authorization: Bearer 601d2d073df8efc2e7b6c850e14b94a3b10afc41fe95ab3c8ceb8c68bc32904f"
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
    "creator_id": 149,
    "id": 71,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 50,
    "additional_university_ids": [

    ],
    "topic_id": 71,
    "discipline_id": 71,
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
    "chapters_updated_at": "2016-10-19T08:59:40.768Z",
    "updated_at": "2016-10-19T08:59:42.267Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 27,
        "title": "Clever Chapter Title 15",
        "position": 1,
        "updated_at": "2016-10-19T08:59:42.223Z",
        "course_id": 71,
        "author_id": 149,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:59:40.768Z",
        "questions_updated_at": "2016-10-19T08:59:40.768Z",
        "flashcards_count": 1,
        "questions_count": 1
      },
      {
        "id": 28,
        "title": "Clever Chapter Title 16",
        "position": 2,
        "updated_at": "2016-10-19T08:59:42.260Z",
        "course_id": 71,
        "author_id": 149,
        "permissions": [

        ],
        "flashcards_updated_at": "2016-10-19T08:59:40.768Z",
        "questions_updated_at": "2016-10-19T08:59:40.768Z",
        "flashcards_count": 1,
        "questions_count": 1
      }
    ],
    "questions": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 149,
        "chapter_id": 27,
        "position": 28,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:40.973Z",
        "created_at": "2016-10-19T08:59:40.862Z",
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
            "id": 55,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 56,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 149,
        "chapter_id": 28,
        "position": 30,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-19T08:59:41.336Z",
        "created_at": "2016-10-19T08:59:41.220Z",
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
            "id": 59,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 60,
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
PUT /v2/courses/87/pin
Content-Type: application/json
Authorization: Bearer 224a55534c048c511e79e7b9a6793385b5008f4b3b378e02543624dbc5abba75
```

`PUT /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/87/pin" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 224a55534c048c511e79e7b9a6793385b5008f4b3b378e02543624dbc5abba75"
```
## Unpin a course


### Request

#### Endpoint

```
DELETE /v2/courses/86/pin
Content-Type: application/json
Authorization: Bearer 41faf7c93fe1123039d6b15669b6cee83496aa7b16eb209f7e36b2a26ea293d3
```

`DELETE /v2/courses/:course_id/pin`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/86/pin" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41faf7c93fe1123039d6b15669b6cee83496aa7b16eb209f7e36b2a26ea293d3"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e6b95be5912a22a014dd78aff7efb1d01bba396959fffadfc1e4fd58c200bafe
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
    "creator_id": 184,
    "id": 84,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 63,
    "additional_university_ids": [

    ],
    "topic_id": 84,
    "discipline_id": 84,
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
    "updated_at": "2016-10-19T08:59:45.837Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6b95be5912a22a014dd78aff7efb1d01bba396959fffadfc1e4fd58c200bafe"
```
# Current user

## Get a user


### Request

#### Endpoint

```
GET /v2/me/user
Content-Type: application/json
Authorization: Bearer 8b692cf7aab26983d822461ae64dd785a8e12b57f8f2bf5032c1a4b151679687
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
    "id": 304,
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
    "created_at": "2016-10-19T08:59:58.030Z",
    "updated_at": "2016-10-19T08:59:58.030Z",
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
	-H "Authorization: Bearer 8b692cf7aab26983d822461ae64dd785a8e12b57f8f2bf5032c1a4b151679687"
```
## Update current user


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 056a9768e82b250555ffa4dc023726c032e4b717438e8f8ea3a931e35a8dfa9a
```

`PATCH /v2/me/user`

#### Parameters


```json
{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[125]}
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
    "id": 300,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      125
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:59:57.701Z",
    "updated_at": "2016-10-19T08:59:57.738Z",
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
curl "api.goskive.com/v2/me/user" -d '{"email":"magnus@gmail.sk","first_name":"Sven","fields_of_study":[125]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 056a9768e82b250555ffa4dc023726c032e4b717438e8f8ea3a931e35a8dfa9a"
```
## Update current user removing fields of study ids if an empty array is sent


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer 438f2ae62d9b18adf317d796af97043a15c27feecb5ee8a67711488a43c27f70
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
    "id": 302,
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
    "created_at": "2016-10-19T08:59:57.837Z",
    "updated_at": "2016-10-19T08:59:57.837Z",
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
	-H "Authorization: Bearer 438f2ae62d9b18adf317d796af97043a15c27feecb5ee8a67711488a43c27f70"
```
## Update current user removing previously set topic if excluded from the list


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: application/json
Authorization: Bearer a77ef3f1c4717950c8d852b6dd24349e6ced3da2658764f921018952df4788d1
```

`PATCH /v2/me/user`

#### Parameters


```json
{"fields_of_study":[126]}
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
    "id": 301,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": null,
    "fields_of_study": [
      126
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:59:57.780Z",
    "updated_at": "2016-10-19T08:59:57.780Z",
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
curl "api.goskive.com/v2/me/user" -d '{"fields_of_study":[126]}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a77ef3f1c4717950c8d852b6dd24349e6ced3da2658764f921018952df4788d1"
```
## Update current user with an image


### Request

#### Endpoint

```
PATCH /v2/me/user
Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1
Authorization: Bearer 343e2592e95d1c087f154a3a8352ab82a03be879d1d2785db4390245c8ba27af
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

124
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
    "id": 299,
    "first_name": "Sven",
    "last_name": "Ahlström",
    "nickname": "strömström",
    "type": "Student",
    "avatar_thumb_url": "file:///home/ubuntu/skive-backend/public/system/students/thumb/f62869fe747289fd4919e45ea8f78a6a77fe4eed.jpg",
    "university_id": null,
    "fields_of_study": [
      124
    ],
    "study_level": null,
    "graduation_year": null,
    "created_at": "2016-10-19T08:59:57.351Z",
    "updated_at": "2016-10-19T08:59:57.639Z",
    "email": "magnus@gmail.sk",
    "locale": "sk",
    "avatar_url": "file:///home/ubuntu/skive-backend/public/system/students/original/83978566691723bfd8aeb9c45255eee3c357e9fe.jpg",
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

124
------------XnJLe9ZIbbGUYtzPQJ16u1
Content-Disposition: form-data; name="image"; filename="contact_avatar.jpg"
Content-Type: image/jpeg
Content-Length: 12418

[uploaded data]
------------XnJLe9ZIbbGUYtzPQJ16u1--' -X PATCH \
	-H "Content-Type: multipart/form-data; boundary=----------XnJLe9ZIbbGUYtzPQJ16u1" \
	-H "Authorization: Bearer 343e2592e95d1c087f154a3a8352ab82a03be879d1d2785db4390245c8ba27af"
```
# Current user Bookmarks

## Get a list of current user bookmarks


### Request

#### Endpoint

```
GET /v2/me/bookmarks
Content-Type: application/json
Authorization: Bearer 176aa139f5fbf89b7f14335d299c0c11df38144a56eb48a3cb7e7ea018b3152f
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
      "bookmarkable_id": 89,
      "bookmarkable_type": "Question"
    },
    {
      "id": 4,
      "bookmarkable_id": 90,
      "bookmarkable_type": "Question"
    },
    {
      "id": 5,
      "bookmarkable_id": 91,
      "bookmarkable_type": "Question"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/bookmarks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 176aa139f5fbf89b7f14335d299c0c11df38144a56eb48a3cb7e7ea018b3152f"
```
# Current user Campaigns

## Get a list of current user campaigns


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer de3a11e3ba98146075540ef41fe89aee7967eb20ea49a3c60cd7da1a2bbc8497
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
	-H "Authorization: Bearer de3a11e3ba98146075540ef41fe89aee7967eb20ea49a3c60cd7da1a2bbc8497"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/campaigns
Content-Type: application/json
Authorization: Bearer 111494e8348eb37ef1b9b0e5c24c90e238af85d8197c77b5e0ae37eeccc465f6
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
	-H "Authorization: Bearer 111494e8348eb37ef1b9b0e5c24c90e238af85d8197c77b5e0ae37eeccc465f6"
```
# Current user Courses

## Get a list of current user courses


### Request

#### Endpoint

```
GET /v2/me/courses
Content-Type: application/json
Authorization: Bearer 094f8b7082674c609ef09eecae6fa93efd6c60069be5cd708d1ae3bd0e7d5d0f
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
      "creator_id": 951,
      "id": 306,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-234",
      "html_url": "https://goskive.com/course/mit-course-234",
      "slug": "mit-course-234",
      "university_id": 291,
      "additional_university_ids": [

      ],
      "topic_id": 318,
      "discipline_id": 319,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 234",
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
      "updated_at": "2016-10-19T09:00:43.387Z",
      "shortname": "mit-course-234"
    },
    {
      "creator_id": 952,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-course-235",
      "html_url": "https://goskive.com/course/mit-course-235",
      "slug": "mit-course-235",
      "university_id": 292,
      "additional_university_ids": [

      ],
      "topic_id": 319,
      "discipline_id": 320,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 235",
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
      "updated_at": "2016-10-19T09:00:43.466Z",
      "shortname": "mit-course-235"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 094f8b7082674c609ef09eecae6fa93efd6c60069be5cd708d1ae3bd0e7d5d0f"
```
# Current user Jobs

## Get a list of current user jobs


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer d2877277e26f6c0a37e18e2197568059587ce2e3124d5eaaca4a48d37deff53b
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
        "updated_at": "2016-10-19T08:59:36.277Z"
      },
      "created_at": "2016-10-19T08:59:36.281Z",
      "updated_at": "2016-10-19T08:59:36.281Z",
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
        "updated_at": "2016-10-19T08:59:36.290Z"
      },
      "created_at": "2016-10-19T08:59:36.294Z",
      "updated_at": "2016-10-19T08:59:36.294Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2877277e26f6c0a37e18e2197568059587ce2e3124d5eaaca4a48d37deff53b"
```
## includes the score


### Request

#### Endpoint

```
GET /v2/me/jobs
Content-Type: application/json
Authorization: Bearer 0bbf11d2a7bd963815e46394160dc7c551ceb1cb6c45580c611fb345e4be2f88
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
        "updated_at": "2016-10-19T08:59:36.050Z"
      },
      "created_at": "2016-10-19T08:59:36.055Z",
      "updated_at": "2016-10-19T08:59:36.055Z",
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
        "updated_at": "2016-10-19T08:59:36.070Z"
      },
      "created_at": "2016-10-19T08:59:36.074Z",
      "updated_at": "2016-10-19T08:59:36.074Z",
      "score": 0.0
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/jobs" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0bbf11d2a7bd963815e46394160dc7c551ceb1cb6c45580c611fb345e4be2f88"
```
# Current user Notifications

## Get a list of current user notifications


### Request

#### Endpoint

```
GET /v2/me/notifications
Content-Type: application/json
Authorization: Bearer 7489a95402bfd35d0f3e36586c622ff357b0c229d159f4bf50f2091d331aabd0
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
      "created_at": "2016-10-19T09:00:39.462Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 56,
      "updated_at": "2016-10-19T09:00:39.586Z",
      "author_id": "908",
      "thread_subject_id": "294",
      "thread_subject_type": "Course"
    },
    {
      "type": "CommentNotification",
      "id": 18,
      "created_at": "2016-10-19T09:00:39.571Z",
      "read_at": null,
      "subject_type": "Commenting::Comment",
      "subject_id": 57,
      "updated_at": "2016-10-19T09:00:39.590Z",
      "author_id": "911",
      "thread_subject_id": "295",
      "thread_subject_type": "Course"
    },
    {
      "type": "UpvoteNotification",
      "id": 19,
      "created_at": "2016-10-19T09:00:39.998Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 16,
      "updated_at": "2016-10-19T09:00:39.998Z"
    },
    {
      "type": "UpvoteNotification",
      "id": 20,
      "created_at": "2016-10-19T09:00:40.377Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 17,
      "updated_at": "2016-10-19T09:00:40.377Z"
    },
    {
      "type": "DownvoteNotification",
      "id": 21,
      "created_at": "2016-10-19T09:00:40.740Z",
      "read_at": null,
      "subject_type": "Vote",
      "subject_id": 18,
      "updated_at": "2016-10-19T09:00:40.740Z"
    },
    {
      "type": "ContentUnitReportedNotification",
      "id": 22,
      "created_at": "2016-10-19T09:00:41.028Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 126,
      "updated_at": "2016-10-19T09:00:41.028Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 23,
      "created_at": "2016-10-19T09:00:41.321Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 127,
      "updated_at": "2016-10-19T09:00:41.321Z"
    },
    {
      "type": "ContentUnitPublishedNotification",
      "id": 24,
      "created_at": "2016-10-19T09:00:41.631Z",
      "read_at": null,
      "subject_type": "Question",
      "subject_id": 128,
      "updated_at": "2016-10-19T09:00:41.631Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/notifications" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7489a95402bfd35d0f3e36586c622ff357b0c229d159f4bf50f2091d331aabd0"
```
## Update a notification


### Request

#### Endpoint

```
PATCH /v2/me/notifications/16
Content-Type: application/json
Authorization: Bearer 6e46b97fcac7f875df34af1ddc63da48f2de40e737cba25063aa6d28ba120a44
```

`PATCH /v2/me/notifications/:notification_id`

#### Parameters


```json
{"notification":{"read_at":"2016-10-19T08:50:39.000Z"}}
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
    "created_at": "2016-10-19T09:00:39.256Z",
    "read_at": "2016-10-19T08:50:39.000Z",
    "subject_type": "Commenting::Comment",
    "subject_id": 55,
    "updated_at": "2016-10-19T09:00:39.321Z",
    "author_id": "904",
    "thread_subject_id": "293",
    "thread_subject_type": "Course"
  }
}
```



```shell
curl "api.goskive.com/v2/me/notifications/16" -d '{"notification":{"read_at":"2016-10-19T08:50:39.000Z"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e46b97fcac7f875df34af1ddc63da48f2de40e737cba25063aa6d28ba120a44"
```
# Current user User Courses

## Get a list of current user user courses


### Request

#### Endpoint

```
GET /v2/me/user_courses
Content-Type: application/json
Authorization: Bearer 52930e430cf2777ef1778afafdfae1bca4359cc0faa4eb078fbd8706605d911a
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
      "course_id": 159,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T09:00:09.782Z",
      "course_published": true,
      "updated_at": "2016-10-19T09:00:09.774Z"
    },
    {
      "id": 3,
      "course_id": 160,
      "pinned": true,
      "score": 0,
      "course_updated_at": "2016-10-19T09:00:09.861Z",
      "course_published": true,
      "updated_at": "2016-10-19T09:00:09.854Z"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/user_courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52930e430cf2777ef1778afafdfae1bca4359cc0faa4eb078fbd8706605d911a"
```
## Get a user course


### Request

#### Endpoint

```
GET /v2/me/user_courses/5
Content-Type: application/json
Authorization: Bearer 92156f6e74ad877f5ffc70a8aee86d9395a94fb51579ff5ef3400784ef4ba479
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
    "course_id": 163,
    "pinned": true,
    "score": 0,
    "course_updated_at": "2016-10-19T09:00:10.251Z",
    "course_published": true,
    "updated_at": "2016-10-19T09:00:10.244Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 92156f6e74ad877f5ffc70a8aee86d9395a94fb51579ff5ef3400784ef4ba479"
```
## Update a user course


### Request

#### Endpoint

```
PATCH /v2/me/user_courses/6
Content-Type: application/json
Authorization: Bearer 8217b9343f6ee091935541f83e289eff611224191b44c5517813e8051e9cea0d
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
    "course_id": 164,
    "pinned": false,
    "score": 0,
    "course_updated_at": "2016-10-19T09:00:10.436Z",
    "course_published": true,
    "updated_at": "2016-10-19T09:00:10.426Z"
  }
}
```



```shell
curl "api.goskive.com/v2/me/user_courses/6" -d '{"user_course":{"pinned":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8217b9343f6ee091935541f83e289eff611224191b44c5517813e8051e9cea0d"
```
# Current user Votes

## Get a list of current user votes


### Request

#### Endpoint

```
GET /v2/me/votes
Content-Type: application/json
Authorization: Bearer 3f79c7612cda3af32c138f476826b539a895d2bf7037a02cc38898ba6ec4b40b
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
      "id": 8,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 108,
      "user_id": 661
    },
    {
      "id": 9,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 109,
      "user_id": 661
    },
    {
      "id": 10,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 110,
      "user_id": 661
    },
    {
      "id": 11,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 111,
      "user_id": 661
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/me/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f79c7612cda3af32c138f476826b539a895d2bf7037a02cc38898ba6ec4b40b"
```
# Disciplines

## Get a discipline and translations


### Request

#### Endpoint

```
GET /v2/disciplines/91
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
    "id": 91,
    "name": "Languages",
    "name_translations": {
      "en": "Languages",
      "de": "Sprachen",
      "fr": "Langues"
    },
    "topics": [
      {
        "id": 91,
        "name": "German",
        "name_translations": {
          "en": "German",
          "de": "Deutsch",
          "fr": "Allemand"
        },
        "discipline_id": 91
      },
      {
        "id": 92,
        "name": "Dutch",
        "name_translations": {
          "en": "Dutch",
          "de": "Niederländisch",
          "fr": "Néerlandais"
        },
        "discipline_id": 91
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/disciplines/91" -X GET \
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
      "id": 92,
      "name": "Function-based directional knowledge user",
      "name_translations": {
        "en": "Function-based directional knowledge user"
      }
    },
    {
      "id": 93,
      "name": "Grass-roots asynchronous access",
      "name_translations": {
        "en": "Grass-roots asynchronous access"
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
PATCH /v2/feedbacks/29/close
Content-Type: application/json
Authorization: Bearer 6143320586c3834f5062c14cea8d9e44db989c35652136d97354e940a18388bc
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
    "id": 29,
    "user_id": 431,
    "feedbackable_id": 48,
    "feedbackable_type": "Flashcard",
    "workflow_state": "closed",
    "updated_at": "2016-10-19T09:00:06.188Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/29/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6143320586c3834f5062c14cea8d9e44db989c35652136d97354e940a18388bc"
```
## Change feedback state to &#39;fixed&#39;


### Request

#### Endpoint

```
PATCH /v2/feedbacks/25/fix
Content-Type: application/json
Authorization: Bearer 5b1305520720889af69d261c104a2a2b250d8089c1c05cb8bc251837a9f46f00
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
    "user_id": 411,
    "feedbackable_id": 44,
    "feedbackable_type": "Flashcard",
    "workflow_state": "fixed",
    "updated_at": "2016-10-19T09:00:04.953Z",
    "flags": 2,
    "message": ""
  }
}
```



```shell
curl "api.goskive.com/v2/feedbacks/25/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b1305520720889af69d261c104a2a2b250d8089c1c05cb8bc251837a9f46f00"
```
## Get a feedback


### Request

#### Endpoint

```
GET /v2/feedbacks/21
Content-Type: application/json
Authorization: Bearer 1bd4972a61418e7d5626b17e8a0e5053aa161ea1b3221576f9d0f6e830a9c1aa
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
    "id": 21,
    "user_id": 389,
    "feedbackable_id": 40,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T09:00:04.086Z",
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
curl "api.goskive.com/v2/feedbacks/21" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1bd4972a61418e7d5626b17e8a0e5053aa161ea1b3221576f9d0f6e830a9c1aa"
```
## Validation error on feedback state change

A validation error is given if the content unit was not
          corrected.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/23/fix
Content-Type: application/json
Authorization: Bearer 509db4772e380a498a5c04578a28d83f337c39a5c53dfef20abfc7107934ddcd
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
curl "api.goskive.com/v2/feedbacks/23/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 509db4772e380a498a5c04578a28d83f337c39a5c53dfef20abfc7107934ddcd"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/24/fix
Content-Type: application/json
Authorization: Bearer 3c11e81b293eb9e9bbc259b462aec5c1775a79177656c31f7286927dde393e14
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
curl "api.goskive.com/v2/feedbacks/24/fix" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c11e81b293eb9e9bbc259b462aec5c1775a79177656c31f7286927dde393e14"
```
## Validation error on feedback state change

An invalid feedback state change gives a validation error.

### Request

#### Endpoint

```
PATCH /v2/feedbacks/27/close
Content-Type: application/json
Authorization: Bearer 6d467e9f801856c5d5532a5d125821bc3f7e84c93b63388a20bef0ebc3889155
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
curl "api.goskive.com/v2/feedbacks/27/close" -d '' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6d467e9f801856c5d5532a5d125821bc3f7e84c93b63388a20bef0ebc3889155"
```
## responds with message from attached comment


### Request

#### Endpoint

```
GET /v2/feedbacks/22
Content-Type: application/json
Authorization: Bearer bcd26b245868319c209bc13c7e12dffb97776080d0559d518b1a2bc8cd17304f
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
    "user_id": 394,
    "feedbackable_id": 41,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T09:00:04.374Z",
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
curl "api.goskive.com/v2/feedbacks/22" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcd26b245868319c209bc13c7e12dffb97776080d0559d518b1a2bc8cd17304f"
```
# Files

## Authorisation error on delete

A student may not delete another file.

### Request

#### Endpoint

```
DELETE /v2/files/9
Authorization: Bearer 554c3bd05808d5a81b09267af332e7726cb41ca09bd9bdc09bd52c04ec5f44b1
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
curl "api.goskive.com/v2/files/9" -d '' -X DELETE \
	-H "Authorization: Bearer 554c3bd05808d5a81b09267af332e7726cb41ca09bd9bdc09bd52c04ec5f44b1" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Authorization: Bearer 22e39a0bd5d536f41ebed723a72809c2f0a5d717e4888a845851c44234debaf0
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
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Authorization: Bearer 22e39a0bd5d536f41ebed723a72809c2f0a5d717e4888a845851c44234debaf0" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
## Download a file


### Request

#### Endpoint

```
GET /v2/files/5
Authorization: Bearer 93e2349b2a550422c81e43e73da48a94c86b341b83ec52fce052cbbd42754ff4
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/81921657c3fcf21153f493d1b285c239.pdf?response-content-disposition=attachment&X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T085933Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=981ed5615ff56733f8d34e52ac3ff69940b50e0a2cf47b12eabecf8d797c5f98"
  }
}
```



```shell
curl "api.goskive.com/v2/files/5" -X GET \
	-H "Authorization: Bearer 93e2349b2a550422c81e43e73da48a94c86b341b83ec52fce052cbbd42754ff4"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/3/metadata
Authorization: Bearer 68d9a8bb6fa559395684a78d4071ed92fadec4e54908b0956acec3cf92977ad2
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
    "id": 3,
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
      "created_at": "2016-10-19T08:59:32.594Z",
      "updated_at": "2016-10-19T08:59:32.594Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [

    ],
    "created_at": "2016-10-19T08:59:32.663Z",
    "updated_at": "2016-10-19T08:59:32.663Z",
    "course_id": 52,
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
curl "api.goskive.com/v2/files/3/metadata" -X GET \
	-H "Authorization: Bearer 68d9a8bb6fa559395684a78d4071ed92fadec4e54908b0956acec3cf92977ad2" \
	-H "Content-Type: application/json"
```
## Get a list of all courses


### Request

#### Endpoint

```
GET /v2/files/14/matched_courses?required_cu_count=2
Authorization: Bearer 37186fd9c5b946a09620883df62c6169e1a351544a3fa0ec0b62eca81de14946
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
      "creator_id": 644,
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off",
      "slug": "mit-the-great-british-bake-off",
      "university_id": 192,
      "additional_university_ids": [

      ],
      "topic_id": 219,
      "discipline_id": 220,
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
      "chapters_updated_at": "2016-10-19T09:00:19.546Z",
      "updated_at": "2016-10-19T09:00:21.182Z",
      "shortname": "mit-the-great-british-bake-off"
    },
    {
      "creator_id": 649,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-the-great-british-bake-off-4af06c7c-98df-4812-9da6-2c8ec50545c1",
      "html_url": "https://goskive.com/course/mit-the-great-british-bake-off-4af06c7c-98df-4812-9da6-2c8ec50545c1",
      "slug": "mit-the-great-british-bake-off-4af06c7c-98df-4812-9da6-2c8ec50545c1",
      "university_id": 193,
      "additional_university_ids": [

      ],
      "topic_id": 220,
      "discipline_id": 221,
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
      "chapters_updated_at": "2016-10-19T09:00:19.546Z",
      "updated_at": "2016-10-19T09:00:21.757Z",
      "shortname": "mit-the-great-british-bake-off-4af06c7c-98df-4812-9da6-2c8ec50545c1"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/files/14/matched_courses?required_cu_count=2" -X GET \
	-H "Authorization: Bearer 37186fd9c5b946a09620883df62c6169e1a351544a3fa0ec0b62eca81de14946"
```
## Preview a file inline


### Request

#### Endpoint

```
GET /v2/files/6/preview
Authorization: Bearer 6022c59cc8159100042eab9e948628b254425e4850190f0056d3783ea3dac93e
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
    "location": "https://s3-eu-west-1.amazonaws.com/cms-staging-upload.qlearning.de/cache/ffe3c9005b98d08a953d38bdec13c572.pdf?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAIGMFY2ZK7LRXEFRA%2F20161019%2Feu-west-1%2Fs3%2Faws4_request&X-Amz-Date=20161019T085933Z&X-Amz-Expires=900&X-Amz-SignedHeaders=host&X-Amz-Signature=5c9155dc2fdc869b9ef7858accc3192fd774a5aa1f472cb607f8fdfe24358fdb"
  }
}
```



```shell
curl "api.goskive.com/v2/files/6/preview" -X GET \
	-H "Authorization: Bearer 6022c59cc8159100042eab9e948628b254425e4850190f0056d3783ea3dac93e"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/files/4/report
Authorization: Bearer 2f845c8323d7b0bcee016bf27182b51c3ce529d98b8d54690248c1f4303c9a21
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
curl "api.goskive.com/v2/files/4/report" -d '' -X PUT \
	-H "Authorization: Bearer 2f845c8323d7b0bcee016bf27182b51c3ce529d98b8d54690248c1f4303c9a21" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Comments

## Create a comment


### Request

#### Endpoint

```
POST /v2/flashcards/91/comments
Content-Type: application/json
Authorization: Bearer 5c60d8f71be9a12cb56ff7f57a822e7d689d127e973a3b2d60779338417491cd
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
    "id": 51,
    "author_id": 871,
    "reply_to_id": null,
    "created_at": "2016-10-19T09:00:35.942Z",
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
curl "api.goskive.com/v2/flashcards/91/comments" -d '{"comment":{"message":"This flashcard is particularly helpful!"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c60d8f71be9a12cb56ff7f57a822e7d689d127e973a3b2d60779338417491cd"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/flashcards/92/comments
Content-Type: application/json
Authorization: Bearer 5cf32d4d3c631e25968a7ed83cc1d29a49b84b1d8aafb535848e3a281b321a66
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
    "id": 52,
    "author_id": 874,
    "reply_to_id": null,
    "created_at": "2016-10-19T09:00:36.267Z",
    "status": "published",
    "replies": [

    ],
    "message": "Hard to see the formulae.",
    "feedback": {
      "id": 46,
      "user_id": 874,
      "feedbackable_id": 92,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:36.264Z",
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
curl "api.goskive.com/v2/flashcards/92/comments" -d '{"comment":{"message":"Hard to see the formulae.","feedback":{"flags":3}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5cf32d4d3c631e25968a7ed83cc1d29a49b84b1d8aafb535848e3a281b321a66"
```
## Get a list of flashcard comments


### Request

#### Endpoint

```
GET /v2/flashcards/95/comments
Content-Type: application/json
Authorization: Bearer 4079c9c61e9f8a7e0c679134e65eb71a3f783fba722ee070c8f5f8c1775d2775
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
      "id": 54,
      "author_id": 887,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:36.937Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 886,
      "reply_to_id": null,
      "created_at": "2016-10-19T09:00:36.921Z",
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
curl "api.goskive.com/v2/flashcards/95/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4079c9c61e9f8a7e0c679134e65eb71a3f783fba722ee070c8f5f8c1775d2775"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/flashcards/93/comments
Content-Type: application/json
Authorization: Bearer c55ddd5f75761823c5f6e16ce577ebdf857f3e3cfbd8887e3c024f10a6cbacf8
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
curl "api.goskive.com/v2/flashcards/93/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c55ddd5f75761823c5f6e16ce577ebdf857f3e3cfbd8887e3c024f10a6cbacf8"
```
# Flashcard Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/flashcards/55/feedbacks
Content-Type: application/json
Authorization: Bearer f785eda84987a95cd6d818e8c1ea8e23cc15ce77ec4e5d6660f609e7f90326e5
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
    "id": 36,
    "user_id": 512,
    "feedbackable_id": 55,
    "feedbackable_type": "Flashcard",
    "workflow_state": "new",
    "updated_at": "2016-10-19T09:00:11.729Z",
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
curl "api.goskive.com/v2/flashcards/55/feedbacks" -d '{"feedback":{"message":"No comprendo","flags":0}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f785eda84987a95cd6d818e8c1ea8e23cc15ce77ec4e5d6660f609e7f90326e5"
```
## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/50/feedbacks
Content-Type: application/json
Authorization: Bearer 0af804a7fe99732506cbcde08c85560d4c2d35d195bcc279ce5977ca8bd8ef4b
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
      "id": 31,
      "user_id": 489,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:10.757Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 488,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:10.745Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0af804a7fe99732506cbcde08c85560d4c2d35d195bcc279ce5977ca8bd8ef4b"
```
# Flashcard Votes

## Get a list of flashcard votes


### Request

#### Endpoint

```
GET /v2/flashcards/88/votes
Content-Type: application/json
Authorization: Bearer 61e3f789b37b685cbe77701fd442d9ac41b4e23ae572c70ae7f1a271f877b695
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
      "id": 14,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 88,
      "user_id": 864
    },
    {
      "id": 13,
      "type": "DownVote",
      "votable_type": "Flashcard",
      "votable_id": 88,
      "user_id": 863
    },
    {
      "id": 12,
      "type": "UpVote",
      "votable_type": "Flashcard",
      "votable_id": 88,
      "user_id": 862
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/88/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 61e3f789b37b685cbe77701fd442d9ac41b4e23ae572c70ae7f1a271f877b695"
```
# Flashcards

## Authorisation error on republish

A student may not republish their own flashcard.

### Request

#### Endpoint

```
PUT /v2/flashcards/78/republish
Content-Type: application/json
Authorization: Bearer ffc9c6808f0c495df1ae03af375b55009dc5614be267927cb5d73b092e5a278f
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
curl "api.goskive.com/v2/flashcards/78/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffc9c6808f0c495df1ae03af375b55009dc5614be267927cb5d73b092e5a278f"
```
## Bookmark a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/80/bookmark
Content-Type: application/json
Authorization: Bearer 1186fe74cfd3243ddb29842001c86f40401a4a899de9aa7ef8e8964b56d0e6a7
```

`PUT /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/80/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1186fe74cfd3243ddb29842001c86f40401a4a899de9aa7ef8e8964b56d0e6a7"
```
## Delete a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/57
Content-Type: application/json
Authorization: Bearer fcea8ae17fb0088ea6842b6f43cacfdacc1c7c8a09df8fcaa46adb680c722361
```

`DELETE /v2/flashcards/:flashcard_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcea8ae17fb0088ea6842b6f43cacfdacc1c7c8a09df8fcaa46adb680c722361"
```
## Downvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/77/downvote
Content-Type: application/json
Authorization: Bearer b413de32adc02fae191128d87c6b80d44fd8efcc460b7c4581e8ca40be2865ec
```

`PUT /v2/flashcards/:flashcard_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/77/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b413de32adc02fae191128d87c6b80d44fd8efcc460b7c4581e8ca40be2865ec"
```
## Get a flashcard


### Request

#### Endpoint

```
GET /v2/flashcards/73
Content-Type: application/json
Authorization: Bearer 76a96c367f030c5786c4fc9e8a2e4803e36e2364dc22647f9ee7c1694ad21a35
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
    "id": 73,
    "obfuscated_id": "LJvjpBojvP0",
    "author_id": 607,
    "chapter_id": 129,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T09:00:17.635Z",
    "created_at": "2016-10-19T09:00:17.635Z",
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
curl "api.goskive.com/v2/flashcards/73" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 76a96c367f030c5786c4fc9e8a2e4803e36e2364dc22647f9ee7c1694ad21a35"
```
## Report a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/report
Content-Type: application/json
Authorization: Bearer 47d2d7c4c63ccb271d8c4babe0ca10efb7444ee4ad7181b29c99e3a46e403df5
```

`PUT /v2/flashcards/:flashcard_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47d2d7c4c63ccb271d8c4babe0ca10efb7444ee4ad7181b29c99e3a46e403df5"
```
## Unbookmark a flashcard


### Request

#### Endpoint

```
DELETE /v2/flashcards/75/bookmark
Content-Type: application/json
Authorization: Bearer d5281385f0799afa4ed48046cec40042ebf394dc4a8e619078ca38e521ce1a88
```

`DELETE /v2/flashcards/:flashcard_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/75/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5281385f0799afa4ed48046cec40042ebf394dc4a8e619078ca38e521ce1a88"
```
## Upvote a flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/76/upvote
Content-Type: application/json
Authorization: Bearer e7bc9152fb728005365ab424accf34ecd344ba7f721cdc27db9c9b874c137cbf
```

`PUT /v2/flashcards/:flashcard_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/76/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e7bc9152fb728005365ab424accf34ecd344ba7f721cdc27db9c9b874c137cbf"
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
    "key": "cache/f1956f5c412cc5b8107d995dc0ad3ce4.jpg",
    "policy": "eyJleHBpcmF0aW9uIjoiMjAxNi0xMC0xOVQxMDowMDowNloiLCJjb25kaXRpb25zIjpbeyJidWNrZXQiOiJjbXMtc3RhZ2luZy11cGxvYWQucWxlYXJuaW5nLmRlIn0seyJrZXkiOiJjYWNoZS9mMTk1NmY1YzQxMmNjNWI4MTA3ZDk5NWRjMGFkM2NlNC5qcGcifSxbImNvbnRlbnQtbGVuZ3RoLXJhbmdlIiwwLDIwOTcxNTJdLHsieC1hbXotY3JlZGVudGlhbCI6IkFLSUFJR01GWTJaSzdMUlhFRlJBLzIwMTYxMDE5L2V1LXdlc3QtMS9zMy9hd3M0X3JlcXVlc3QifSx7IngtYW16LWFsZ29yaXRobSI6IkFXUzQtSE1BQy1TSEEyNTYifSx7IngtYW16LWRhdGUiOiIyMDE2MTAxOVQwOTAwMDZaIn1dfQ==",
    "x-amz-credential": "AKIAIGMFY2ZK7LRXEFRA/20161019/eu-west-1/s3/aws4_request",
    "x-amz-algorithm": "AWS4-HMAC-SHA256",
    "x-amz-date": "20161019T090006Z",
    "x-amz-signature": "917ea2d60b1150d40cae55d9e3a27b264069a6fcf77ef88015455cba14811399"
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
Authorization: Bearer 81fb8a1aab427e6cb8973d6417c718d82b304e3475a4b6f1b1df9c104d787380
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
	-H "Authorization: Bearer 81fb8a1aab427e6cb8973d6417c718d82b304e3475a4b6f1b1df9c104d787380"
```
## Validation error on sign up

A missing `email_address` gives a validation error.

### Request

#### Endpoint

```
POST /v2/me/jobs/9/sign_ups
Content-Type: application/json
Authorization: Bearer 4aa39760c359e2ee42297332a923fd15692bc32090d5837bee1fb8fbe3f773a8
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
	-H "Authorization: Bearer 4aa39760c359e2ee42297332a923fd15692bc32090d5837bee1fb8fbe3f773a8"
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
{"password":{"reset_password_token":"1E7igFx4zpuauBcvViAK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}
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
  "id": 890,
  "email": "jan.turnosky@hotmail.sk",
  "created_at": "2016-10-19T09:00:37.429Z",
  "updated_at": "2016-10-19T09:00:37.635Z",
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
  "audit_id": 5061
}
```



```shell
curl "api.goskive.com/v2/password" -d '{"password":{"reset_password_token":"1E7igFx4zpuauBcvViAK","password":"new-passw0rd","password_confirmation":"new-passw0rd"}}' -X PUT \
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
POST /v2/questions/13/comments
Content-Type: application/json
Authorization: Bearer 436972446ce7a47282f6f1df59d5ca7576946d14aa0d15099e39379d021f758d
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
    "author_id": 113,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:59:34.981Z",
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
curl "api.goskive.com/v2/questions/13/comments" -d '{"comment":{"message":"Not sure what this question means."}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 436972446ce7a47282f6f1df59d5ca7576946d14aa0d15099e39379d021f758d"
```
## Create a comment with feedback


### Request

#### Endpoint

```
POST /v2/questions/14/comments
Content-Type: application/json
Authorization: Bearer 8ef790e5f1fc11d28b770a0ca48b7b925bdfbf4af6772ecd7dd9a3bbe5c05760
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
    "author_id": 116,
    "reply_to_id": null,
    "created_at": "2016-10-19T08:59:35.473Z",
    "status": "published",
    "replies": [

    ],
    "message": "Really bad grammar.",
    "feedback": {
      "id": 1,
      "user_id": 116,
      "feedbackable_id": 14,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T08:59:35.469Z",
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
curl "api.goskive.com/v2/questions/14/comments" -d '{"comment":{"message":"Really bad grammar.","feedback":{"flags":2}}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ef790e5f1fc11d28b770a0ca48b7b925bdfbf4af6772ecd7dd9a3bbe5c05760"
```
## Get a list of question comments


### Request

#### Endpoint

```
GET /v2/questions/12/comments
Content-Type: application/json
Authorization: Bearer c633b981b6adef6a71c8c7c07ea0cbbacb10dfe9ad8945e2ea9de0aad40d78c3
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
      "id": 1,
      "author_id": 111,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:59:34.557Z",
      "status": "published",
      "replies": [

      ],
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 112,
      "reply_to_id": null,
      "created_at": "2016-10-19T08:59:34.592Z",
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
curl "api.goskive.com/v2/questions/12/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c633b981b6adef6a71c8c7c07ea0cbbacb10dfe9ad8945e2ea9de0aad40d78c3"
```
## Validation error on create

A missing `message` gives a validation error.

### Request

#### Endpoint

```
POST /v2/questions/15/comments
Content-Type: application/json
Authorization: Bearer c2362c480e9feb605ecbc305dace22b97fd009b9a27fca65d46221ee8cd0db38
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
curl "api.goskive.com/v2/questions/15/comments" -d '{}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2362c480e9feb605ecbc305dace22b97fd009b9a27fca65d46221ee8cd0db38"
```
# Question Feedbacks

## Create feedback


### Request

#### Endpoint

```
POST /v2/questions/93/feedbacks
Content-Type: application/json
Authorization: Bearer bb4c1acd5749eac60bd497b7612ec67c126b6203ace3d8a67386460d5c0e75f4
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
    "id": 39,
    "user_id": 521,
    "feedbackable_id": 93,
    "feedbackable_type": "Question",
    "workflow_state": "new",
    "updated_at": "2016-10-19T09:00:12.954Z",
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
	-H "Authorization: Bearer bb4c1acd5749eac60bd497b7612ec67c126b6203ace3d8a67386460d5c0e75f4"
```
## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/99/feedbacks
Content-Type: application/json
Authorization: Bearer c69ae3b6cbf57a5acbbbb4539f4cd9ac7edc8e9da672bb102501f915c3933556
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
      "id": 45,
      "user_id": 553,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:15.085Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 552,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-19T09:00:15.073Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/99/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c69ae3b6cbf57a5acbbbb4539f4cd9ac7edc8e9da672bb102501f915c3933556"
```
# Question Votes

## Get a list of question votes


### Request

#### Endpoint

```
GET /v2/questions/130/votes
Content-Type: application/json
Authorization: Bearer e0142f536d4a3ea2c847eef0ce9e01ec2c9335659579d3c00dabddd2b7565767
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
      "votable_id": 130,
      "user_id": 943
    },
    {
      "id": 20,
      "type": "DownVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 942
    },
    {
      "id": 19,
      "type": "UpVote",
      "votable_type": "Question",
      "votable_id": 130,
      "user_id": 941
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/130/votes" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e0142f536d4a3ea2c847eef0ce9e01ec2c9335659579d3c00dabddd2b7565767"
```
# Questions

## Authorisation error on republish

A student may not republish their own question.

### Request

#### Endpoint

```
PUT /v2/questions/48/republish
Content-Type: application/json
Authorization: Bearer 4d0bfb6d4313c79e2ac6e492bef6414d9d1b8611ea66dfcb0a938fc47fa2f12e
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
	-H "Authorization: Bearer 4d0bfb6d4313c79e2ac6e492bef6414d9d1b8611ea66dfcb0a938fc47fa2f12e"
```
## Bookmark a question


### Request

#### Endpoint

```
PUT /v2/questions/45/bookmark
Content-Type: application/json
Authorization: Bearer a59bf5a7d61312f360a8d04296c0120358042d27d0e77373aaaa3df21fe00694
```

`PUT /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/45/bookmark" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a59bf5a7d61312f360a8d04296c0120358042d27d0e77373aaaa3df21fe00694"
```
## Delete a question


### Request

#### Endpoint

```
DELETE /v2/questions/43
Content-Type: application/json
Authorization: Bearer 456f591dd14de9efd0014a580238950da05e4528b101a5a6be2dc26ef949c6cf
```

`DELETE /v2/questions/:question_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/43" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 456f591dd14de9efd0014a580238950da05e4528b101a5a6be2dc26ef949c6cf"
```
## Downvote a question


### Request

#### Endpoint

```
PUT /v2/questions/66/downvote
Content-Type: application/json
Authorization: Bearer f7e998002d2003cb91a39c346d0b593b11f5281fb385df0b0e4e6913c43ca766
```

`PUT /v2/questions/:question_id/downvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/66/downvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7e998002d2003cb91a39c346d0b593b11f5281fb385df0b0e4e6913c43ca766"
```
## Get a question


### Request

#### Endpoint

```
GET /v2/questions/44
Content-Type: application/json
Authorization: Bearer fb65ac812d3dd99e65d9894beada6f002b26be0e3ad480ae9d4696126dac46a9
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
    "id": 44,
    "obfuscated_id": "bbNlnrscV_w",
    "author_id": 213,
    "chapter_id": 40,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:59:48.878Z",
    "created_at": "2016-10-19T08:59:48.763Z",
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
  }
}
```



```shell
curl "api.goskive.com/v2/questions/44" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb65ac812d3dd99e65d9894beada6f002b26be0e3ad480ae9d4696126dac46a9"
```
## Report a question


### Request

#### Endpoint

```
PUT /v2/questions/42/report
Content-Type: application/json
Authorization: Bearer 9bffef83989d673b3eb5f836f223801968a88e84f5afacbad161c99a7f56031b
```

`PUT /v2/questions/:question_id/report`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/report" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9bffef83989d673b3eb5f836f223801968a88e84f5afacbad161c99a7f56031b"
```
## Unbookmark a question


### Request

#### Endpoint

```
DELETE /v2/questions/65/bookmark
Content-Type: application/json
Authorization: Bearer 22ccbc768a348bdd77f3d9db06f285977399a6feefc56c3a12b92eaf6ec5215a
```

`DELETE /v2/questions/:question_id/bookmark`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/65/bookmark" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22ccbc768a348bdd77f3d9db06f285977399a6feefc56c3a12b92eaf6ec5215a"
```
## Update a question


### Request

#### Endpoint

```
PATCH /v2/questions/47
Content-Type: application/json
Authorization: Bearer 6b36f905a250a6593c3dc7c34ac3f3942a634f859379bd824b085324e0760d33
```

`PATCH /v2/questions/:question_id`

#### Parameters


```json
{"question":{"question":{"id":47,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T08:59:49.858Z","updated_at":"2016-10-19T08:59:49.979Z","more":"This could never explain why it didn't pass. Maybe it did?","chapter_id":43,"author_id":222,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn't pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}
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
    "id": 47,
    "obfuscated_id": "rpshod_7JeU",
    "author_id": 222,
    "chapter_id": 43,
    "position": 1,
    "reviewed": false,
    "upvotes_count": 0,
    "downvotes_count": 0,
    "updated_at": "2016-10-19T08:59:50.090Z",
    "created_at": "2016-10-19T08:59:49.858Z",
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
    "question": "{\"id\"=>47, \"position\"=>1, \"type\"=>0, \"question\"=>\"Clever example question: why did the rspec test not pass?\", \"created_at\"=>\"2016-10-19T08:59:49.858Z\", \"updated_at\"=>\"2016-10-19T08:59:49.979Z\", \"more\"=>\"This could never explain why it didn't pass. Maybe it did?\", \"chapter_id\"=>43, \"author_id\"=>222, \"question_html\"=>\"<p>Clever example question: why did the rspec test not pass?</p>\", \"more_html\"=>\"<p>This could never explain why it didn't pass. Maybe it did?<p>\", \"seconds\"=>30, \"multiple_choice\"=>false, \"shuffle_answers\"=>true, \"up_votes_count\"=>0, \"down_votes_count\"=>0, \"answer_options_count\"=>4, \"language_code\"=>\"de\", \"audit_id\"=>nil, \"status\"=>\"published\"}",
    "question_html": "<p>Clever example question: why did the rspec test not pass?</p>",
    "shuffle_answers": true,
    "multiple_choice": false,
    "explanation": "Eggs do all the work",
    "explanation_html": "<p>This could never explain why it didn't pass. Maybe it did?<p>",
    "answer_options": [
      {
        "id": 93,
        "position": 1,
        "content": "MyText",
        "content_html": "MyText",
        "correct": true
      },
      {
        "id": 94,
        "position": 2,
        "content": "MyText",
        "content_html": "MyText",
        "correct": false
      },
      {
        "id": 95,
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
curl "api.goskive.com/v2/questions/47" -d '{"question":{"question":{"id":47,"position":1,"type":0,"question":"Clever example question: why did the rspec test not pass?","created_at":"2016-10-19T08:59:49.858Z","updated_at":"2016-10-19T08:59:49.979Z","more":"This could never explain why it didn\u0027t pass. Maybe it did?","chapter_id":43,"author_id":222,"question_html":"\u003cp\u003eClever example question: why did the rspec test not pass?\u003c/p\u003e","more_html":"\u003cp\u003eThis could never explain why it didn\u0027t pass. Maybe it did?\u003cp\u003e","seconds":30,"multiple_choice":false,"shuffle_answers":true,"up_votes_count":0,"down_votes_count":0,"answer_options_count":4,"language_code":"de","audit_id":null,"status":"published"},"explanation":"Eggs do all the work","answer_options":[{"content":"Choux needs baking powder.","content_html":"\u003cp\u003eChoux needs baking powder.\u003c/p\u003e","correct":false}]}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b36f905a250a6593c3dc7c34ac3f3942a634f859379bd824b085324e0760d33"
```
## Upvote a question


### Request

#### Endpoint

```
PUT /v2/questions/46/upvote
Content-Type: application/json
Authorization: Bearer 392c1358f4b3481dd8aadd2f5b914cc707f92a43573a4884ad119b914057286e
```

`PUT /v2/questions/:question_id/upvote`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46/upvote" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 392c1358f4b3481dd8aadd2f5b914cc707f92a43573a4884ad119b914057286e"
```
# Search

## Perform a course search


### Request

#### Endpoint

```
GET /v2/search/courses?query=Pi
Content-Type: application/json
Authorization: Bearer 0eca8dca2901afc7d38db442f60f3f3cc229ec318c5a7c24217ba2a4178f8049
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
      "creator_id": 131,
      "id": 66,
      "self_url": "http://api.goskive.test/api/v2/courses/mit-pizza-201",
      "html_url": "https://goskive.com/course/mit-pizza-201",
      "slug": "mit-pizza-201",
      "university_id": 43,
      "additional_university_ids": [

      ],
      "topic_id": 66,
      "discipline_id": 66,
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
      "updated_at": "2016-10-19T08:59:37.096Z",
      "shortname": "mit-pizza-201"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/search/courses?query=Pi" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0eca8dca2901afc7d38db442f60f3f3cc229ec318c5a7c24217ba2a4178f8049"
```
## Perform a university search


### Request

#### Endpoint

```
GET /v2/search/universities?query=NSP
Content-Type: application/json
Authorization: Bearer 2eee3ba8a933def32e1b9fb0dd11d0a8d50cd96fa48ccddee38ba66fbccdaf63
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
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-28",
      "html_url": "https://goskive.com/university/uni-28",
      "slug": "uni-28",
      "name": "National School of Pizza",
      "short_name": "Uni 28",
      "acronym": "NSPI",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/d1a9b052cb589d3b9637242e29368256dc61b861.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/f2cc0e8549ba6457eafa38e277c10692eb12fe43.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:59:37.394Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 45,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-27",
      "html_url": "https://goskive.com/university/uni-27",
      "slug": "uni-27",
      "name": "National School of Pastry",
      "short_name": "Uni 27",
      "acronym": "NSPA",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/3b5c10f1506b2b541b26c7b22aa8dbe9fbeb14bb.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/2c56013ff790bb0862c4c4583aac0ac3929a762b.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:59:37.377Z",
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
	-H "Authorization: Bearer 2eee3ba8a933def32e1b9fb0dd11d0a8d50cd96fa48ccddee38ba66fbccdaf63"
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
      "id": 166,
      "name": "Cross-platform background paradigm",
      "name_translations": {
        "en": "Cross-platform background paradigm"
      },
      "discipline_id": 167
    },
    {
      "id": 167,
      "name": "Object-based interactive success",
      "name_translations": {
        "en": "Object-based interactive success"
      },
      "discipline_id": 168
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
GET /v2/topics/165
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
    "id": 165,
    "name": "Paleogenetic",
    "name_translations": {
      "en": "Paleogenetic",
      "de": "Paläogenetik",
      "fr": "Paléogénétique"
    },
    "discipline_id": 166
  }
}
```



```shell
curl "api.goskive.com/v2/topics/165" -X GET \
	-H "Content-Type: application/json"
```
# Universities

## Get a list of universities


### Request

#### Endpoint

```
GET /v2/universities
Content-Type: application/json
Authorization: Bearer 8a00187562db64a087da8a9abf0bbf78a4405ca3e5192522a246801ee956335d
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
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-52",
      "html_url": "https://goskive.com/university/uni-52",
      "slug": "uni-52",
      "name": "University 20",
      "short_name": "Uni 52",
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
      "updated_at": "2016-10-19T08:59:47.229Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-53",
      "html_url": "https://goskive.com/university/uni-53",
      "slug": "uni-53",
      "name": "University 21",
      "short_name": "Uni 53",
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
      "updated_at": "2016-10-19T08:59:47.247Z",
      "url": "http://goskive.com",
      "latitude": "52.496403",
      "longitude": "13.357812",
      "published": true
    },
    {
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/universities/uni-54",
      "html_url": "https://goskive.com/university/uni-54",
      "slug": "uni-54",
      "name": "University 22",
      "short_name": "Uni 54",
      "acronym": "MIT",
      "country_code": "DE",
      "city": "Berlin",
      "searchable_text": "",
      "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/cb2a218358d44a5056fe2e55e738cd09577c8a5c.png",
      "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/b5ad29aed1943ad0d14839f7d56c62a22a0b6452.png",
      "postal_code": "10781",
      "street": "Winterfeldtstraße",
      "street_number": "21",
      "display_priority": 1,
      "courses_count": 0,
      "updated_at": "2016-10-19T08:59:47.264Z",
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
	-H "Authorization: Bearer 8a00187562db64a087da8a9abf0bbf78a4405ca3e5192522a246801ee956335d"
```
## Get a university


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin
Content-Type: application/json
Authorization: Bearer 714b5efb410b077ae4eaeaa837d0e0d8c23965262d12120cd2c879ab427c6d2c
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
    "id": 70,
    "self_url": "http://api.goskive.test/api/v2/universities/fu-berlin",
    "html_url": "https://goskive.com/university/fu-berlin",
    "slug": "fu-berlin",
    "name": "Freie Universität Berlin",
    "short_name": "FU Berlin",
    "acronym": "FU",
    "country_code": "DE",
    "city": "Berlin",
    "searchable_text": "",
    "image_url": "file:///home/ubuntu/skive-backend/public/system/universities/original/fe68b2e1c81a7d5c35fd1107da0e373597f006d5.png",
    "image_thumb_url": "file:///home/ubuntu/skive-backend/public/system/universities/thumb/e85940cf8561c3a456df79e408c963432af4ba51.png",
    "postal_code": "14195",
    "street": "Kaiserswerther Str.",
    "street_number": "16-18",
    "display_priority": 9,
    "courses_count": 0,
    "updated_at": "2016-10-19T08:59:47.086Z",
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
	-H "Authorization: Bearer 714b5efb410b077ae4eaeaa837d0e0d8c23965262d12120cd2c879ab427c6d2c"
```
# University Courses

## Create a published course with chapters


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d15d32e06ca8fc5eec8e684ff35e8f8f9553ee22204a949d03ebde11139696a7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":48,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}
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
    "creator_id": 78,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 26,
    "additional_university_ids": [

    ],
    "topic_id": 48,
    "discipline_id": 48,
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
    "chapters_updated_at": "2016-10-19T08:59:31.971Z",
    "updated_at": "2016-10-19T08:59:32.110Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [
      {
        "id": 14,
        "title": "Etymology of Choux",
        "position": 1,
        "updated_at": "2016-10-19T08:59:32.067Z",
        "course_id": 48,
        "author_id": 78,
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
        "id": 15,
        "title": "Pastry Making in Medieval France",
        "position": 2,
        "updated_at": "2016-10-19T08:59:32.083Z",
        "course_id": 48,
        "author_id": 78,
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
        "id": 16,
        "title": "Pastry for Neophytes",
        "position": 3,
        "updated_at": "2016-10-19T08:59:32.100Z",
        "course_id": 48,
        "author_id": 78,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":48,"chapters":[{"title":"Etymology of Choux"},{"title":"Pastry Making in Medieval France"},{"title":"Pastry for Neophytes"}]}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d15d32e06ca8fc5eec8e684ff35e8f8f9553ee22204a949d03ebde11139696a7"
```
## Create a published course, ignoring unpermitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8ef4e94dd972824927684d073ecf884cc5760f95d25e7cf95192e96629ea3372
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":47,"published":false}}
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
    "creator_id": 77,
    "id": 47,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 25,
    "additional_university_ids": [

    ],
    "topic_id": 47,
    "discipline_id": 47,
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
    "updated_at": "2016-10-19T08:59:31.935Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":47,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ef4e94dd972824927684d073ecf884cc5760f95d25e7cf95192e96629ea3372"
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
      "creator_id": 40,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "topic_id": 16,
      "discipline_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
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
      "updated_at": "2016-10-19T08:59:28.541Z",
      "shortname": "fu-course-7"
    },
    {
      "creator_id": 40,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "topic_id": 17,
      "discipline_id": 17,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 8",
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
      "chapters_updated_at": "2016-10-19T08:59:28.817Z",
      "updated_at": "2016-10-19T08:59:28.823Z",
      "shortname": "fu-course-8"
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
Authorization: Bearer a0aaa9e84cec6e5e22bce945643cda24ad40f6e5fdaf16503d9d062261e1381f
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
      "creator_id": 47,
      "id": 24,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 24,
      "discipline_id": 24,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
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
      "updated_at": "2016-10-19T08:59:29.239Z",
      "shortname": "fu-course-15"
    },
    {
      "creator_id": 47,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 25,
      "discipline_id": 25,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
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
      "chapters_updated_at": "2016-10-19T08:59:29.526Z",
      "updated_at": "2016-10-19T08:59:29.533Z",
      "shortname": "fu-course-16"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0aaa9e84cec6e5e22bce945643cda24ad40f6e5fdaf16503d9d062261e1381f"
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
      "creator_id": 45,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 14,
      "additional_university_ids": [

      ],
      "topic_id": 20,
      "discipline_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
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
      "updated_at": "2016-10-19T08:59:29.023Z",
      "shortname": "fu-course-11"
    },
    {
      "creator_id": 45,
      "id": 21,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 14,
      "additional_university_ids": [

      ],
      "topic_id": 21,
      "discipline_id": 21,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
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
      "updated_at": "2016-10-19T08:59:29.061Z",
      "shortname": "fu-course-12"
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
Authorization: Bearer 1423190a6bb5aac1ac3696d353e9ebaeec68b66239fbedbcb77e1c79b7f3a1c9
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
      "creator_id": 54,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-19",
      "html_url": "https://goskive.com/course/fu-course-19",
      "slug": "fu-course-19",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 28,
      "discipline_id": 28,
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
      "updated_at": "2016-10-19T08:59:29.799Z",
      "shortname": "fu-course-19"
    },
    {
      "creator_id": 54,
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-20",
      "html_url": "https://goskive.com/course/fu-course-20",
      "slug": "fu-course-20",
      "university_id": 17,
      "additional_university_ids": [

      ],
      "topic_id": 29,
      "discipline_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 20",
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
      "updated_at": "2016-10-19T08:59:29.838Z",
      "shortname": "fu-course-20"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1423190a6bb5aac1ac3696d353e9ebaeec68b66239fbedbcb77e1c79b7f3a1c9"
```
# User Sign Up [v1]

## Sign up a user


### Request

#### Endpoint

```
POST /users
Content-Type: application/json
Authorization: Bearer 364f88280deff04d66ac44e7ea405844780a87b75aa943dcec7b953ec62afd2f
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
  "id": 674,
  "first_name": "Jan",
  "last_name": "Turnosky",
  "display_nickname": "Jan Turnosky",
  "type": "Student",
  "image_url": null,
  "created_at": "2016-10-19T09:00:23.809Z",
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
	-H "Authorization: Bearer 364f88280deff04d66ac44e7ea405844780a87b75aa943dcec7b953ec62afd2f"
```
# Users

## Get a complete user profile


### Request

#### Endpoint

```
GET /v2/users/289
Content-Type: application/json
Authorization: Bearer aaf9d003ff4b5f954094f209db3aa89094fa96e70edb32f11f9927831c89745b
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
    "id": 289,
    "first_name": "Magnus",
    "last_name": "Ahlström",
    "nickname": "awesome-magnus",
    "type": "Student",
    "avatar_thumb_url": null,
    "university_id": 100,
    "fields_of_study": [
      118,
      119
    ],
    "study_level": "bachelor",
    "graduation_year": 2015,
    "created_at": "2016-10-19T08:59:56.440Z",
    "updated_at": "2016-10-19T08:59:56.440Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/289" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aaf9d003ff4b5f954094f209db3aa89094fa96e70edb32f11f9927831c89745b"
```
## Get a minimal user profile


### Request

#### Endpoint

```
GET /v2/users/287
Content-Type: application/json
Authorization: Bearer e8f4aec87de71a9f732f6c21318d233a76439ef37c5d3a25fd701e6df14ab296
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
    "id": 287,
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
    "created_at": "2016-10-19T08:59:56.282Z",
    "updated_at": "2016-10-19T08:59:56.282Z"
  }
}
```



```shell
curl "api.goskive.com/v2/users/287" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8f4aec87de71a9f732f6c21318d233a76439ef37c5d3a25fd701e6df14ab296"
```
# Votes

## Delete a vote


### Request

#### Endpoint

```
DELETE /v2/votes/3
Content-Type: application/json
Authorization: Bearer f0c8cccb7c2570abceafbf1e2d987e991dce9081112262b18465d4003bb1f7d2
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
	-H "Authorization: Bearer f0c8cccb7c2570abceafbf1e2d987e991dce9081112262b18465d4003bb1f7d2"
```
## Get a vote


### Request

#### Endpoint

```
GET /v2/votes/5
Content-Type: application/json
Authorization: Bearer 8614b1616508c960c7c906d40c2c50023a5b786ff96f03fd6ecae550cbd3ab57
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
    "votable_id": 88,
    "user_id": 452
  }
}
```



```shell
curl "api.goskive.com/v2/votes/5" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8614b1616508c960c7c906d40c2c50023a5b786ff96f03fd6ecae550cbd3ab57"
```
