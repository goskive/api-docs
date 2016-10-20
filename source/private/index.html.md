---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
---

# Chapters

## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/79
Content-Type: application/json
Authorization: Bearer 55f875e512381a7c8c5e85cf2daed7c93756010c3d2fb9d5c76bf277db855d78
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/79" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 55f875e512381a7c8c5e85cf2daed7c93756010c3d2fb9d5c76bf277db855d78"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/77
Content-Type: application/json
Authorization: Bearer 77965c77f7acb680ddb32a69bf6d103b90bca19877c0fe6f212f9e979bb0cbd0
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
    "id": 77,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-20T09:46:14.263Z",
    "course_id": 131,
    "author_id": 453,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-20T09:46:13.650Z",
    "questions_updated_at": "2016-10-20T09:46:13.650Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 456,
        "chapter_id": 77,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:14.195Z",
        "created_at": "2016-10-20T09:46:14.195Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 457,
        "chapter_id": 77,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:14.241Z",
        "created_at": "2016-10-20T09:46:14.241Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 454,
        "chapter_id": 77,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:13.887Z",
        "created_at": "2016-10-20T09:46:13.757Z",
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
      },
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 455,
        "chapter_id": 77,
        "position": 39,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:14.112Z",
        "created_at": "2016-10-20T09:46:13.969Z",
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
            "id": 77,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 78,
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
curl "api.goskive.com/v2/chapters/77" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77965c77f7acb680ddb32a69bf6d103b90bca19877c0fe6f212f9e979bb0cbd0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/75
Content-Type: application/json
Authorization: Bearer f848aebc783be74382dc697c69eb71a435e4c62abb8cd7a3e5f2e55b594188da
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
    "id": 75,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-20T09:46:12.918Z",
    "course_id": 129,
    "author_id": 443,
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
curl "api.goskive.com/v2/chapters/75" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f848aebc783be74382dc697c69eb71a435e4c62abb8cd7a3e5f2e55b594188da"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer d6df2c89310bb758c7224257b2e442aaace770f1d602b7b045533f279a37cb8a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6df2c89310bb758c7224257b2e442aaace770f1d602b7b045533f279a37cb8a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5fa64cffa1bd7543221867a636dff7166b6bd1b89469879b5f26aff7c9d7c1cd
```

`GET /v2/comments`

#### Parameters



| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| level  | [Filter] Level: all(default)|top-level|replies |
| page  | [Pagination] Page (max. 100 comments per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 24,
      "author_id": 227,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:57.668Z",
      "status": "published",
      "subject_id": 64,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 229,
      "reply_to_id": 24,
      "created_at": "2016-10-20T09:45:57.752Z",
      "status": "published",
      "subject_id": 65,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 231,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:57.836Z",
      "status": "published",
      "subject_id": 66,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 233,
      "reply_to_id": 26,
      "created_at": "2016-10-20T09:45:57.919Z",
      "status": "published",
      "subject_id": 67,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 235,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:58.005Z",
      "status": "reported",
      "subject_id": 68,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 237,
      "reply_to_id": 28,
      "created_at": "2016-10-20T09:45:58.089Z",
      "status": "published",
      "subject_id": 69,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 239,
      "reply_to_id": 28,
      "created_at": "2016-10-20T09:45:58.173Z",
      "status": "published",
      "subject_id": 70,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5fa64cffa1bd7543221867a636dff7166b6bd1b89469879b5f26aff7c9d7c1cd"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a4aaeac91ff6ada2452eee4d91e5ef3e9b5a85a9dc75245d3b5ba8e70dd351c0
```

`GET /v2/comments`

#### Parameters



| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| level  | [Filter] Level: all(default)|top-level|replies |
| page  | [Pagination] Page (max. 100 comments per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 38,
      "author_id": 257,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:58.933Z",
      "status": "published",
      "subject_id": 78,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 259,
      "reply_to_id": 38,
      "created_at": "2016-10-20T09:45:59.017Z",
      "status": "published",
      "subject_id": 79,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 261,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:59.100Z",
      "status": "published",
      "subject_id": 80,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 263,
      "reply_to_id": 40,
      "created_at": "2016-10-20T09:45:59.181Z",
      "status": "published",
      "subject_id": 81,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 265,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:59.267Z",
      "status": "reported",
      "subject_id": 82,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 267,
      "reply_to_id": 42,
      "created_at": "2016-10-20T09:45:59.350Z",
      "status": "published",
      "subject_id": 83,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 269,
      "reply_to_id": 42,
      "created_at": "2016-10-20T09:45:59.433Z",
      "status": "published",
      "subject_id": 84,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4aaeac91ff6ada2452eee4d91e5ef3e9b5a85a9dc75245d3b5ba8e70dd351c0"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer b52c89d8ba8f9f28ea1451bd2e0bf27fb3b84a9e1e8803e50d2c54c84daab707
```

`GET /v2/comments`

#### Parameters


```json
level: replies
```


| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| level  | [Filter] Level: all(default)|top-level|replies |
| page  | [Pagination] Page (max. 100 comments per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 32,
      "author_id": 244,
      "reply_to_id": 31,
      "created_at": "2016-10-20T09:45:58.383Z",
      "status": "published",
      "subject_id": 72,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 248,
      "reply_to_id": 33,
      "created_at": "2016-10-20T09:45:58.540Z",
      "status": "published",
      "subject_id": 74,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 252,
      "reply_to_id": 35,
      "created_at": "2016-10-20T09:45:58.721Z",
      "status": "published",
      "subject_id": 76,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 254,
      "reply_to_id": 35,
      "created_at": "2016-10-20T09:45:58.802Z",
      "status": "published",
      "subject_id": 77,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b52c89d8ba8f9f28ea1451bd2e0bf27fb3b84a9e1e8803e50d2c54c84daab707"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 4ca90eafa09f6a8f61df32d4733a5f36d72b3582db48819a72f5bccadc0a585b
```

`GET /v2/comments`

#### Parameters


```json
status: reported
```


| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| level  | [Filter] Level: all(default)|top-level|replies |
| page  | [Pagination] Page (max. 100 comments per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "comments": [
    {
      "id": 21,
      "author_id": 220,
      "reply_to_id": null,
      "created_at": "2016-10-20T09:45:57.381Z",
      "status": "reported",
      "subject_id": 61,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/comments?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4ca90eafa09f6a8f61df32d4733a5f36d72b3582db48819a72f5bccadc0a585b"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer 3ea3f3eb109c3d893b62c9e34e2a119c53e6c34fa2f409ebef49879eb297a479
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ea3f3eb109c3d893b62c9e34e2a119c53e6c34fa2f409ebef49879eb297a479"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c275c52cbca6d471aa1113b6932a238d6a7ac099605fdeb9bdf627aad528f682
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
    "id": 103,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T09:46:25.860Z",
    "course_id": 204,
    "author_id": 611,
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
	-H "Authorization: Bearer c275c52cbca6d471aa1113b6932a238d6a7ac099605fdeb9bdf627aad528f682"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/205/chapters
Content-Type: application/json
Authorization: Bearer 8364502d53a912b1a75c6099a55e7f02d24c600062676a986fa34ff6cd556a9c
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
    "id": 104,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-20T09:46:25.996Z",
    "course_id": 205,
    "author_id": 613,
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
curl "api.goskive.com/v2/courses/205/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8364502d53a912b1a75c6099a55e7f02d24c600062676a986fa34ff6cd556a9c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8218970d729d3b47245e0bead982f87fb0d626efc0e0486aa907843bd412403c
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
      "id": 105,
      "title": "Clever Chapter Title 90",
      "position": 1,
      "updated_at": "2016-10-20T09:46:26.106Z",
      "course_id": 206,
      "author_id": 615,
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
      "id": 106,
      "title": "Clever Chapter Title 91",
      "position": 2,
      "updated_at": "2016-10-20T09:46:26.130Z",
      "course_id": 206,
      "author_id": 616,
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
      "id": 107,
      "title": "Clever Chapter Title 92",
      "position": 3,
      "updated_at": "2016-10-20T09:46:26.376Z",
      "course_id": 206,
      "author_id": 617,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-20T09:46:26.031Z",
      "questions_updated_at": "2016-10-20T09:46:26.031Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8218970d729d3b47245e0bead982f87fb0d626efc0e0486aa907843bd412403c"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fe29015c4eef8e78bf9d15563c69924241a0a708fe9058e1eb613ba46b1eaaff
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
      "id": 108,
      "title": "Clever Chapter Title 93",
      "position": 1,
      "updated_at": "2016-10-20T09:46:26.622Z",
      "course_id": 208,
      "author_id": 624,
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
      "id": 109,
      "title": "Clever Chapter Title 94",
      "position": 2,
      "updated_at": "2016-10-20T09:46:26.646Z",
      "course_id": 208,
      "author_id": 625,
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
      "id": 110,
      "title": "Clever Chapter Title 95",
      "position": 3,
      "updated_at": "2016-10-20T09:46:26.671Z",
      "course_id": 208,
      "author_id": 626,
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
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fe29015c4eef8e78bf9d15563c69924241a0a708fe9058e1eb613ba46b1eaaff"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 263ec2cccd97dd9de1a66b220beb38fee0573ec6fbb02355940ebdc8ef8b4856
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
	-H "Authorization: Bearer 263ec2cccd97dd9de1a66b220beb38fee0573ec6fbb02355940ebdc8ef8b4856"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/266
Content-Type: application/json
Authorization: Bearer db6ae4cc46389f50110cdcdf6d4bea2fb1977b1e9a3f2891720228a74db7c3b6
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/266" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db6ae4cc46389f50110cdcdf6d4bea2fb1977b1e9a3f2891720228a74db7c3b6"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer bd6425e2aaa5cb3c7970e7eaf7d761843f3d6f9537e418327a8cacfabc0661b1
```

`GET /v2/courses/:course_slug`

#### Parameters


```json
include: flashcards, invalid_resources
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
    "creator_id": 855,
    "id": 275,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 259,
    "additional_university_ids": [

    ],
    "topic_id": 287,
    "discipline_id": 288,
    "language_code": "de",
    "exam_months": [

    ],
    "title": "Choux pastry 101",
    "organizational_identifier": null,
    "instructor_name": "",
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 6,
    "questions_count": 6,
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
    "chapters_updated_at": "2016-10-20T09:46:47.349Z",
    "updated_at": "2016-10-20T09:46:48.784Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 164,
        "title": "Clever Chapter Title 140",
        "position": 1,
        "updated_at": "2016-10-20T09:46:48.736Z",
        "course_id": 275,
        "author_id": 855,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-20T09:46:47.349Z",
        "questions_updated_at": "2016-10-20T09:46:47.349Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 165,
        "title": "Clever Chapter Title 141",
        "position": 2,
        "updated_at": "2016-10-20T09:46:48.776Z",
        "course_id": 275,
        "author_id": 855,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-20T09:46:47.349Z",
        "questions_updated_at": "2016-10-20T09:46:47.349Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 855,
        "chapter_id": 164,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.573Z",
        "created_at": "2016-10-20T09:46:48.573Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 855,
        "chapter_id": 165,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.645Z",
        "created_at": "2016-10-20T09:46:48.645Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 855,
        "chapter_id": 164,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.613Z",
        "created_at": "2016-10-20T09:46:48.613Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 855,
        "chapter_id": 165,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.686Z",
        "created_at": "2016-10-20T09:46:48.686Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 858,
        "chapter_id": 164,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.726Z",
        "created_at": "2016-10-20T09:46:48.726Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 859,
        "chapter_id": 165,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-20T09:46:48.766Z",
        "created_at": "2016-10-20T09:46:48.766Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd6425e2aaa5cb3c7970e7eaf7d761843f3d6f9537e418327a8cacfabc0661b1"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/270
Content-Type: application/json
Authorization: Bearer 2727becbfcf0d814bc2eca208a1c1848958eea92e6de3fbe1963eb3b206fd4c9
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
200 OK
```


```json
{
  "course": {
    "creator_id": 838,
    "id": 270,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 254,
    "additional_university_ids": [

    ],
    "topic_id": 282,
    "discipline_id": 283,
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
    "updated_at": "2016-10-20T09:46:43.996Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/270" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2727becbfcf0d814bc2eca208a1c1848958eea92e6de3fbe1963eb3b206fd4c9"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 535caa9f0fde51d628e9bf764dd882800b2df91935044e77ebe4826c531bf1c7
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
    "creator_id": 835,
    "id": 268,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 252,
    "additional_university_ids": [

    ],
    "topic_id": 280,
    "discipline_id": 281,
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
    "user_generated": false,
    "published": false,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-10-20T09:46:43.713Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 535caa9f0fde51d628e9bf764dd882800b2df91935044e77ebe4826c531bf1c7"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 0d228ffc9bbf136503b5e45b4aec7e5f3a3e6bcb5920a28650d94af3e5aa636c
```

`GET /v2/feedbacks`

#### Parameters



| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|new|fixed|reminded|ultimatum_given|abandoned|closed |
| page  | [Pagination] Page (max. 100 comments per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "feedbacks": [
    {
      "id": 24,
      "user_id": 111,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:49.940Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 115,
      "feedbackable_id": 16,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:50.234Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 119,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:50.540Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 123,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:50.848Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 127,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-20T09:45:51.156Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0d228ffc9bbf136503b5e45b4aec7e5f3a3e6bcb5920a28650d94af3e5aa636c"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer cbaee76f8b6c252656758554c4334d7c560adfbac626b398ab80f5cdd0274684
```

`GET /v2/feedbacks`

#### Parameters


```json
status: abandoned
```


| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|new|fixed|reminded|ultimatum_given|abandoned|closed |
| page  | [Pagination] Page (max. 100 comments per page) |



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
      "user_id": 69,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-20T09:45:46.927Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbaee76f8b6c252656758554c4334d7c560adfbac626b398ab80f5cdd0274684"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Content-Type: application/json
Authorization: Bearer 48ecf5b7844d12d9d0e847ea62e16df658be9d48a371a83bc7c131fe4ca886e8
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/4" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48ecf5b7844d12d9d0e847ea62e16df658be9d48a371a83bc7c131fe4ca886e8"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 0043f557250e8930d924ef8ed081e0622bdbe04f9119e0a178a4f8bd4e38242c
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
      "id": 569,
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
      "created_at": "2016-10-20T09:46:22.619Z",
      "updated_at": "2016-10-20T09:46:22.619Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "created_at": "2016-10-20T09:46:22.690Z",
    "updated_at": "2016-10-20T09:46:22.690Z",
    "course_id": 190,
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
curl "api.goskive.com/v2/files/8/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0043f557250e8930d924ef8ed081e0622bdbe04f9119e0a178a4f8bd4e38242c"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/57/feedbacks
Content-Type: application/json
Authorization: Bearer e8a1de35ac01fa9efde26a2f5df89fc674b9f62e252e12a1dd61788690b2093f
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
      "user_id": 506,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:17.146Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 505,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:46:17.135Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8a1de35ac01fa9efde26a2f5df89fc674b9f62e252e12a1dd61788690b2093f"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer f5f032238c60fe3c5565e65be14a59344808f9b300f500bfa83a90ecd55cdedc
```

`GET /v2/flashcards`

#### Parameters



| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| page  | [Pagination] Page (max. 100 flashcards per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcards": [
    {
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 388,
      "chapter_id": 60,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:09.339Z",
      "created_at": "2016-10-20T09:46:09.339Z",
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 391,
      "chapter_id": 61,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:09.484Z",
      "created_at": "2016-10-20T09:46:09.484Z",
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
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 394,
      "chapter_id": 62,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:09.629Z",
      "created_at": "2016-10-20T09:46:09.629Z",
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
      "author_id": 397,
      "chapter_id": 63,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:09.773Z",
      "created_at": "2016-10-20T09:46:09.773Z",
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
      "author_id": 400,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:09.944Z",
      "created_at": "2016-10-20T09:46:09.944Z",
      "tags": [

      ],
      "status": "reported",
      "published": false,
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
curl "api.goskive.com/v2/flashcards" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5f032238c60fe3c5565e65be14a59344808f9b300f500bfa83a90ecd55cdedc"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer d50deec51c33d5dfd8957e5553f4e38fa11187efeb557ce1fe1261335359fd86
```

`GET /v2/flashcards`

#### Parameters


```json
status: reported
```


| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| page  | [Pagination] Page (max. 100 flashcards per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "flashcards": [
    {
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 416,
      "chapter_id": 69,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:10.764Z",
      "created_at": "2016-10-20T09:46:10.764Z",
      "tags": [

      ],
      "status": "reported",
      "published": false,
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
curl "api.goskive.com/v2/flashcards?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d50deec51c33d5dfd8957e5553f4e38fa11187efeb557ce1fe1261335359fd86"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/21/republish
Content-Type: application/json
Authorization: Bearer 0dfcd0ff134170c9863ac4c0d468b7746dd0597a5b737fa4438bc44240bf000e
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/21/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dfcd0ff134170c9863ac4c0d468b7746dd0597a5b737fa4438bc44240bf000e"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/27/feedbacks
Content-Type: application/json
Authorization: Bearer d768da19bbeb14275550bf62972f607f19ca0503a30a5bda9be090ba951f41ac
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
      "user_id": 164,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:54.258Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 163,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-20T09:45:54.247Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/27/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d768da19bbeb14275550bf62972f607f19ca0503a30a5bda9be090ba951f41ac"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 6f4ea33fd9ac1f7122bcf54955b89f97d002776e479126e5996af0b7d819f9c9
```

`GET /v2/questions`

#### Parameters



| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| page  | [Pagination] Page (max. 100 questions per page) |



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
      "author_id": 898,
      "chapter_id": 177,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:53.352Z",
      "created_at": "2016-10-20T09:46:53.232Z",
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
          "id": 234,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 235,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 889,
      "chapter_id": 174,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:52.516Z",
      "created_at": "2016-10-20T09:46:52.402Z",
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
          "id": 228,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 229,
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
      "author_id": 892,
      "chapter_id": 175,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:52.791Z",
      "created_at": "2016-10-20T09:46:52.677Z",
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
          "id": 230,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 231,
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
      "author_id": 895,
      "chapter_id": 176,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:53.071Z",
      "created_at": "2016-10-20T09:46:52.955Z",
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
          "id": 232,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 233,
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
      "author_id": 901,
      "chapter_id": 178,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:53.628Z",
      "created_at": "2016-10-20T09:46:53.517Z",
      "tags": [

      ],
      "status": "reported",
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
          "id": 236,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 237,
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f4ea33fd9ac1f7122bcf54955b89f97d002776e479126e5996af0b7d819f9c9"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer cd9eefb12373d1e2bc40bc08a91aaa3c6cf860d7f85907a890524e2c891859d3
```

`GET /v2/questions`

#### Parameters


```json
status: reported
```


| Name | Description |
|:-----|:------------|
| status  | [Filter] Status: all(default)|published|unpublished|draft|reported |
| page  | [Pagination] Page (max. 100 questions per page) |



### Response

```
Content-Type: application/json; charset=utf-8
200 OK
```


```json
{
  "questions": [
    {
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 917,
      "chapter_id": 183,
      "position": 117,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-20T09:46:55.093Z",
      "created_at": "2016-10-20T09:46:54.980Z",
      "tags": [

      ],
      "status": "reported",
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
          "id": 246,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 247,
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
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd9eefb12373d1e2bc40bc08a91aaa3c6cf860d7f85907a890524e2c891859d3"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/123/republish
Content-Type: application/json
Authorization: Bearer b464c1815e40151caac054ce4b2f4b774156b8a2fb77c241e97d359217e73f72
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/123/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b464c1815e40151caac054ce4b2f4b774156b8a2fb77c241e97d359217e73f72"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b62560261355804cef0595c88e71b3dcee7701ebda4b1680a5f88ba1d2f55b79
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":153,"published":false}}
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
    "creator_id": 509,
    "id": 146,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 147,
    "additional_university_ids": [

    ],
    "topic_id": 153,
    "discipline_id": 153,
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
    "user_generated": false,
    "published": false,
    "official": false,
    "has_training": true,
    "has_exam": true,
    "has_flashcards": false,
    "has_challenge_mode": true,
    "campaign_ids": [

    ],
    "chapters_updated_at": null,
    "updated_at": "2016-10-20T09:46:17.637Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":153,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b62560261355804cef0595c88e71b3dcee7701ebda4b1680a5f88ba1d2f55b79"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 43a3b81b9a0a93cd13f6d5f024158e7f0efefc5fd447a5364c5c1383b47fa8f3
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
      "creator_id": 511,
      "id": 148,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-125",
      "html_url": "https://goskive.com/course/fu-course-125",
      "slug": "fu-course-125",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 155,
      "discipline_id": 155,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 125",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-20T09:46:17.842Z",
      "shortname": "fu-course-125"
    },
    {
      "creator_id": 511,
      "id": 149,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 156,
      "discipline_id": 156,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-20T09:46:17.882Z",
      "shortname": "fu-course-126"
    },
    {
      "creator_id": 512,
      "id": 150,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 157,
      "discipline_id": 157,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-10-20T09:46:17.930Z",
      "shortname": "fu-course-127"
    },
    {
      "creator_id": 512,
      "id": 151,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 149,
      "additional_university_ids": [

      ],
      "topic_id": 158,
      "discipline_id": 158,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
      "organizational_identifier": null,
      "instructor_name": "",
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
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
      "chapters_updated_at": "2016-10-20T09:46:18.260Z",
      "updated_at": "2016-10-20T09:46:18.268Z",
      "shortname": "fu-course-128"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43a3b81b9a0a93cd13f6d5f024158e7f0efefc5fd447a5364c5c1383b47fa8f3"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7db65aa0c01a701aa40fefe1b9dd2e452548e5e5c4f4d0eb8f64a100f95e6903
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
      "creator_id": 518,
      "id": 152,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-129",
      "html_url": "https://goskive.com/course/fu-course-129",
      "slug": "fu-course-129",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 159,
      "discipline_id": 159,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 129",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-20T09:46:18.482Z",
      "shortname": "fu-course-129"
    },
    {
      "creator_id": 518,
      "id": 153,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 160,
      "discipline_id": 160,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 130",
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
      "user_generated": false,
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-20T09:46:18.532Z",
      "shortname": "fu-course-130"
    },
    {
      "creator_id": 519,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-131",
      "html_url": "https://goskive.com/course/fu-course-131",
      "slug": "fu-course-131",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 161,
      "discipline_id": 161,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 131",
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
      "updated_at": "2016-10-20T09:46:18.581Z",
      "shortname": "fu-course-131"
    },
    {
      "creator_id": 519,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 162,
      "discipline_id": 162,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
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
      "updated_at": "2016-10-20T09:46:18.622Z",
      "shortname": "fu-course-132"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7db65aa0c01a701aa40fefe1b9dd2e452548e5e5c4f4d0eb8f64a100f95e6903"
```
