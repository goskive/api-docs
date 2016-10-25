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
DELETE /v2/chapters/8
Content-Type: application/json
Authorization: Bearer 6265a0e0bea3f003dc067890031e1d10ad3a61ff0973569c3f1465fdd11e03e8
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
	-H "Authorization: Bearer 6265a0e0bea3f003dc067890031e1d10ad3a61ff0973569c3f1465fdd11e03e8"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/3
Content-Type: application/json
Authorization: Bearer 435bf5ef081c596ee00445f1ee2b65e41a0da98cf0f5b0293da27a01a543ea68
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
    "id": 3,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-25T20:31:37.916Z",
    "course_id": 44,
    "author_id": 106,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-25T20:31:37.327Z",
    "questions_updated_at": "2016-10-25T20:31:37.327Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 109,
        "chapter_id": 3,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.855Z",
        "created_at": "2016-10-25T20:31:37.855Z",
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
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 110,
        "chapter_id": 3,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.896Z",
        "created_at": "2016-10-25T20:31:37.896Z",
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
        "author_id": 107,
        "chapter_id": 3,
        "position": 4,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.573Z",
        "created_at": "2016-10-25T20:31:37.456Z",
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
      },
      {
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 108,
        "chapter_id": 3,
        "position": 5,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:31:37.780Z",
        "created_at": "2016-10-25T20:31:37.650Z",
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
            "id": 9,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 10,
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
curl "api.goskive.com/v2/chapters/3" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 435bf5ef081c596ee00445f1ee2b65e41a0da98cf0f5b0293da27a01a543ea68"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/5
Content-Type: application/json
Authorization: Bearer 2e4954515789f8601a88d128d8bd0ef101bcb0a95ded924f771f191c3b3f2eac
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
    "updated_at": "2016-10-25T20:31:38.346Z",
    "course_id": 46,
    "author_id": 115,
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
	-H "Authorization: Bearer 2e4954515789f8601a88d128d8bd0ef101bcb0a95ded924f771f191c3b3f2eac"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/40
Content-Type: application/json
Authorization: Bearer 2273e91b2ea3fceab097665be68549401ada7529a5b7bc441d7a0e2e7f4b4564
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2273e91b2ea3fceab097665be68549401ada7529a5b7bc441d7a0e2e7f4b4564"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 0dd4ce47a81e08bb9d5bbe8374e69f0b74380c4586c9ca8a5fd60ce09c281795
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
      "id": 1,
      "author_id": 7,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:32.329Z",
      "status": "published",
      "subject_id": 2,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 2,
      "author_id": 9,
      "reply_to_id": 1,
      "created_at": "2016-10-25T20:31:32.446Z",
      "status": "published",
      "subject_id": 3,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 3,
      "author_id": 11,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:32.535Z",
      "status": "published",
      "subject_id": 4,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 4,
      "author_id": 13,
      "reply_to_id": 3,
      "created_at": "2016-10-25T20:31:32.622Z",
      "status": "published",
      "subject_id": 5,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 15,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:32.709Z",
      "status": "reported",
      "subject_id": 6,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 17,
      "reply_to_id": 5,
      "created_at": "2016-10-25T20:31:32.796Z",
      "status": "published",
      "subject_id": 7,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 19,
      "reply_to_id": 5,
      "created_at": "2016-10-25T20:31:32.885Z",
      "status": "published",
      "subject_id": 8,
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
	-H "Authorization: Bearer 0dd4ce47a81e08bb9d5bbe8374e69f0b74380c4586c9ca8a5fd60ce09c281795"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c5a31d0030883d94a0789a8156e370950f47c76b87b698adb4f475d9496a678f
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
      "id": 29,
      "author_id": 67,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:35.002Z",
      "status": "published",
      "subject_id": 30,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 69,
      "reply_to_id": 29,
      "created_at": "2016-10-25T20:31:35.095Z",
      "status": "published",
      "subject_id": 31,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 71,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:35.188Z",
      "status": "published",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 73,
      "reply_to_id": 31,
      "created_at": "2016-10-25T20:31:35.275Z",
      "status": "published",
      "subject_id": 33,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 75,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:35.360Z",
      "status": "reported",
      "subject_id": 34,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 77,
      "reply_to_id": 33,
      "created_at": "2016-10-25T20:31:35.446Z",
      "status": "published",
      "subject_id": 35,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 79,
      "reply_to_id": 33,
      "created_at": "2016-10-25T20:31:35.531Z",
      "status": "published",
      "subject_id": 36,
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
	-H "Authorization: Bearer c5a31d0030883d94a0789a8156e370950f47c76b87b698adb4f475d9496a678f"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer ff49cdad8cc54c68df7a4e7387a2bcfeee6948230a4dc5c7c6020a29ac77c544
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
      "id": 23,
      "author_id": 54,
      "reply_to_id": 22,
      "created_at": "2016-10-25T20:31:34.430Z",
      "status": "published",
      "subject_id": 24,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 58,
      "reply_to_id": 24,
      "created_at": "2016-10-25T20:31:34.586Z",
      "status": "published",
      "subject_id": 26,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 62,
      "reply_to_id": 26,
      "created_at": "2016-10-25T20:31:34.776Z",
      "status": "published",
      "subject_id": 28,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 64,
      "reply_to_id": 26,
      "created_at": "2016-10-25T20:31:34.861Z",
      "status": "published",
      "subject_id": 29,
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
	-H "Authorization: Bearer ff49cdad8cc54c68df7a4e7387a2bcfeee6948230a4dc5c7c6020a29ac77c544"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer fc7b33e86cfe8ffded7325edcc1fb0b0675015c30b37959b24d71ff7580e48da
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
      "id": 19,
      "author_id": 45,
      "reply_to_id": null,
      "created_at": "2016-10-25T20:31:34.072Z",
      "status": "reported",
      "subject_id": 20,
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
	-H "Authorization: Bearer fc7b33e86cfe8ffded7325edcc1fb0b0675015c30b37959b24d71ff7580e48da"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/36/republish
Content-Type: application/json
Authorization: Bearer 80dee6edb26b267b6498bda18adf36b01deee6dfece02eb94867b6c8146a1805
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/36/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 80dee6edb26b267b6498bda18adf36b01deee6dfece02eb94867b6c8146a1805"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3799d72425cbccd17a8516e9fdedbb2ef8f94c3d3efe131a9a4d119e809b23d4
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
    "id": 171,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:32:46.823Z",
    "course_id": 285,
    "author_id": 878,
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
	-H "Authorization: Bearer 3799d72425cbccd17a8516e9fdedbb2ef8f94c3d3efe131a9a4d119e809b23d4"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/288/chapters
Content-Type: application/json
Authorization: Bearer b062eaadb2c0fdd63a31732a5cd23fed3a63c33c001fc472d3118a8ad8e6e847
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
    "id": 173,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-25T20:32:47.207Z",
    "course_id": 288,
    "author_id": 884,
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
curl "api.goskive.com/v2/courses/288/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b062eaadb2c0fdd63a31732a5cd23fed3a63c33c001fc472d3118a8ad8e6e847"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 216e56fe2c6f8558c3f6d339f811dbefbd69013e38dc8676af1c0078f643c296
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
      "id": 177,
      "title": "Clever Chapter Title 153",
      "position": 1,
      "updated_at": "2016-10-25T20:32:47.629Z",
      "course_id": 291,
      "author_id": 893,
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
      "id": 178,
      "title": "Clever Chapter Title 154",
      "position": 2,
      "updated_at": "2016-10-25T20:32:47.652Z",
      "course_id": 291,
      "author_id": 894,
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
      "id": 179,
      "title": "Clever Chapter Title 155",
      "position": 3,
      "updated_at": "2016-10-25T20:32:47.896Z",
      "course_id": 291,
      "author_id": 895,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-25T20:32:47.556Z",
      "questions_updated_at": "2016-10-25T20:32:47.556Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 216e56fe2c6f8558c3f6d339f811dbefbd69013e38dc8676af1c0078f643c296"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c4ffe8b559f176503adac7d8c2c836538031d45a5b40859ba2f1bc0cee6957ab
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
      "id": 180,
      "title": "Clever Chapter Title 156",
      "position": 1,
      "updated_at": "2016-10-25T20:32:48.134Z",
      "course_id": 293,
      "author_id": 902,
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
      "id": 181,
      "title": "Clever Chapter Title 157",
      "position": 2,
      "updated_at": "2016-10-25T20:32:48.156Z",
      "course_id": 293,
      "author_id": 903,
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
      "id": 182,
      "title": "Clever Chapter Title 158",
      "position": 3,
      "updated_at": "2016-10-25T20:32:48.180Z",
      "course_id": 293,
      "author_id": 904,
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
	-H "Authorization: Bearer c4ffe8b559f176503adac7d8c2c836538031d45a5b40859ba2f1bc0cee6957ab"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e8c01b4fb576dab25bfe72a645d7c0b5d0679dac82aea317608882015befcb6d
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
	-H "Authorization: Bearer e8c01b4fb576dab25bfe72a645d7c0b5d0679dac82aea317608882015befcb6d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/174
Content-Type: application/json
Authorization: Bearer 089aa209eb65ca1a2ef47a917f95f8bc4cc4b34388afa4561390669ce0124bf1
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/174" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 089aa209eb65ca1a2ef47a917f95f8bc4cc4b34388afa4561390669ce0124bf1"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 48a02a2d82f1765ed45103a2bbea92dbc3c35455cc98053de314201d299120f1
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
    "creator_id": 578,
    "id": 178,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 185,
    "additional_university_ids": [

    ],
    "topic_id": 182,
    "discipline_id": 183,
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
    "chapters_updated_at": "2016-10-25T20:32:20.815Z",
    "updated_at": "2016-10-25T20:32:22.299Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 114,
        "title": "Clever Chapter Title 96",
        "position": 1,
        "updated_at": "2016-10-25T20:32:22.252Z",
        "course_id": 178,
        "author_id": 578,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T20:32:20.815Z",
        "questions_updated_at": "2016-10-25T20:32:20.815Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 115,
        "title": "Clever Chapter Title 97",
        "position": 2,
        "updated_at": "2016-10-25T20:32:22.292Z",
        "course_id": 178,
        "author_id": 578,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-25T20:32:20.815Z",
        "questions_updated_at": "2016-10-25T20:32:20.815Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 578,
        "chapter_id": 114,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.090Z",
        "created_at": "2016-10-25T20:32:22.090Z",
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
        "author_id": 578,
        "chapter_id": 115,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.161Z",
        "created_at": "2016-10-25T20:32:22.161Z",
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
        "author_id": 578,
        "chapter_id": 114,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.129Z",
        "created_at": "2016-10-25T20:32:22.129Z",
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
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 578,
        "chapter_id": 115,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.201Z",
        "created_at": "2016-10-25T20:32:22.201Z",
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
        "author_id": 581,
        "chapter_id": 114,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.242Z",
        "created_at": "2016-10-25T20:32:22.242Z",
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
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 582,
        "chapter_id": 115,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-25T20:32:22.282Z",
        "created_at": "2016-10-25T20:32:22.282Z",
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
	-H "Authorization: Bearer 48a02a2d82f1765ed45103a2bbea92dbc3c35455cc98053de314201d299120f1"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/180
Content-Type: application/json
Authorization: Bearer 4785422b368c8197003d9e7989256e69a09fde61fd408479e83af4d6af2f1a83
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
    "creator_id": 589,
    "id": 180,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 187,
    "additional_university_ids": [

    ],
    "topic_id": 184,
    "discipline_id": 185,
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
    "updated_at": "2016-10-25T20:32:24.027Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/180" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4785422b368c8197003d9e7989256e69a09fde61fd408479e83af4d6af2f1a83"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ffea451f9a9f5bf077239d999aefd4479cd27df77161253b1941d7e2189775aa
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
    "creator_id": 594,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 190,
    "additional_university_ids": [

    ],
    "topic_id": 187,
    "discipline_id": 188,
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
    "updated_at": "2016-10-25T20:32:24.415Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ffea451f9a9f5bf077239d999aefd4479cd27df77161253b1941d7e2189775aa"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer c473ca68c06e8d26a94ec646ad15f4f68d2d657cb59c6830e5b1692db3bc6079
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
      "id": 28,
      "user_id": 781,
      "feedbackable_id": 122,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:40.348Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 785,
      "feedbackable_id": 123,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:40.648Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 789,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:40.960Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 793,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:41.270Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 797,
      "feedbackable_id": 126,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T20:32:41.576Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c473ca68c06e8d26a94ec646ad15f4f68d2d657cb59c6830e5b1692db3bc6079"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 8572f225df0233c9d648bd4a7f27129c689706f143528ebdf1e033c099da7990
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
      "id": 37,
      "user_id": 818,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-25T20:32:43.186Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8572f225df0233c9d648bd4a7f27129c689706f143528ebdf1e033c099da7990"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer af06279001551a05c7409c3172291edda83d04090fe5ab7d745d0f66572f13f4
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/12" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af06279001551a05c7409c3172291edda83d04090fe5ab7d745d0f66572f13f4"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/8/metadata
Content-Type: application/json
Authorization: Bearer 0c3dbfc13c70fabf400b68d17d8b1db9ad4fab1f3dfaf792d92af1134a9752c1
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
      "id": 474,
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
      "created_at": "2016-10-25T20:32:09.958Z",
      "updated_at": "2016-10-25T20:32:09.958Z"
    },
    "status": "published",
    "download_count": 2,
    "mime_type": "application/pdf",
    "size": 6893,
    "permissions": [
      "update",
      "delete"
    ],
    "up_votes_count": 0,
    "created_at": "2016-10-25T20:32:10.034Z",
    "updated_at": "2016-10-25T20:32:10.034Z",
    "course_id": 147,
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
	-H "Authorization: Bearer 0c3dbfc13c70fabf400b68d17d8b1db9ad4fab1f3dfaf792d92af1134a9752c1"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/15/feedbacks
Content-Type: application/json
Authorization: Bearer 31edb72838c60fa0f93f1025d998823d0f97dd7a47047df4ec3904def32f0a97
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
      "id": 7,
      "user_id": 174,
      "feedbackable_id": 15,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:42.652Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 173,
      "feedbackable_id": 15,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:31:42.640Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/15/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31edb72838c60fa0f93f1025d998823d0f97dd7a47047df4ec3904def32f0a97"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 314fc2178895647b9c2079de73e976f256b0d410f9b6945486ab2b37468507cf
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 389,
      "chapter_id": 75,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:03.879Z",
      "created_at": "2016-10-25T20:32:03.879Z",
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 392,
      "chapter_id": 76,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:04.021Z",
      "created_at": "2016-10-25T20:32:04.021Z",
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
      "author_id": 395,
      "chapter_id": 77,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:04.164Z",
      "created_at": "2016-10-25T20:32:04.164Z",
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
      "author_id": 398,
      "chapter_id": 78,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:04.306Z",
      "created_at": "2016-10-25T20:32:04.306Z",
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
      "author_id": 401,
      "chapter_id": 79,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:04.448Z",
      "created_at": "2016-10-25T20:32:04.448Z",
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
	-H "Authorization: Bearer 314fc2178895647b9c2079de73e976f256b0d410f9b6945486ab2b37468507cf"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer a59664b34395a5b79d0a5d317097919bc82e3b3d0863dde259339f02fd18cdd7
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
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 417,
      "chapter_id": 84,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:32:05.223Z",
      "created_at": "2016-10-25T20:32:05.223Z",
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
	-H "Authorization: Bearer a59664b34395a5b79d0a5d317097919bc82e3b3d0863dde259339f02fd18cdd7"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/22/republish
Content-Type: application/json
Authorization: Bearer b20ab2cc41535f2a0ff3fe69983b0c15dcb9b329aec7df9ed5a2acf1068ce3a5
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/22/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b20ab2cc41535f2a0ff3fe69983b0c15dcb9b329aec7df9ed5a2acf1068ce3a5"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/106/feedbacks
Content-Type: application/json
Authorization: Bearer 649d0dd94d85c8026884f4147063b347f4d383b2c1d915049c24710786a05cae
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
      "id": 16,
      "user_id": 703,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:33.915Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 702,
      "feedbackable_id": 106,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-25T20:32:33.903Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/106/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 649d0dd94d85c8026884f4147063b347f4d383b2c1d915049c24710786a05cae"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 5914ff6df495e9dca89d5df51011ab81ec25a04d4d372527af6be9006ca9b5ba
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
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 265,
      "chapter_id": 47,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:52.160Z",
      "created_at": "2016-10-25T20:31:52.015Z",
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
          "id": 67,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 68,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 256,
      "chapter_id": 44,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:51.164Z",
      "created_at": "2016-10-25T20:31:51.022Z",
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
          "id": 61,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 62,
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
      "author_id": 259,
      "chapter_id": 45,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:51.495Z",
      "created_at": "2016-10-25T20:31:51.352Z",
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
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 262,
      "chapter_id": 46,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:51.821Z",
      "created_at": "2016-10-25T20:31:51.677Z",
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
          "id": 65,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 66,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 268,
      "chapter_id": 48,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:52.487Z",
      "created_at": "2016-10-25T20:31:52.347Z",
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
          "id": 69,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 70,
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
	-H "Authorization: Bearer 5914ff6df495e9dca89d5df51011ab81ec25a04d4d372527af6be9006ca9b5ba"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer dfe8f2c553f35ac1abbbed34f587f264cb62253be1885effbc233de23c0f39f1
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 252,
      "chapter_id": 43,
      "position": 17,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-25T20:31:50.784Z",
      "created_at": "2016-10-25T20:31:50.648Z",
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
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfe8f2c553f35ac1abbbed34f587f264cb62253be1885effbc233de23c0f39f1"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/19/republish
Content-Type: application/json
Authorization: Bearer a352623a350c5712ee449b2ee3dc2890f17363833ed5ea8a5a041fcac0c400ab
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/19/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a352623a350c5712ee449b2ee3dc2890f17363833ed5ea8a5a041fcac0c400ab"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1802a7f5c5691a3e2524507dfa0a24252c542d4f2c2f334db3ed3719aef90681
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":228,"published":false}}
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
    "creator_id": 642,
    "id": 224,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 209,
    "additional_university_ids": [

    ],
    "topic_id": 228,
    "discipline_id": 229,
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
    "updated_at": "2016-10-25T20:32:28.875Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":228,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1802a7f5c5691a3e2524507dfa0a24252c542d4f2c2f334db3ed3719aef90681"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bda12252b8082a626405ba3000ff55c1c35beb1a2c4b40906226ffb874978e53
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
      "creator_id": 622,
      "id": 205,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 209,
      "discipline_id": 210,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 162",
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
      "updated_at": "2016-10-25T20:32:26.820Z",
      "shortname": "fu-course-162"
    },
    {
      "creator_id": 622,
      "id": 206,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 210,
      "discipline_id": 211,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
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
      "updated_at": "2016-10-25T20:32:26.860Z",
      "shortname": "fu-course-163"
    },
    {
      "creator_id": 623,
      "id": 207,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-164",
      "html_url": "https://goskive.com/course/fu-course-164",
      "slug": "fu-course-164",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 211,
      "discipline_id": 212,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 164",
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
      "updated_at": "2016-10-25T20:32:26.910Z",
      "shortname": "fu-course-164"
    },
    {
      "creator_id": 623,
      "id": 208,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 200,
      "additional_university_ids": [

      ],
      "topic_id": 212,
      "discipline_id": 213,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
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
      "chapters_updated_at": "2016-10-25T20:32:27.208Z",
      "updated_at": "2016-10-25T20:32:27.215Z",
      "shortname": "fu-course-165"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bda12252b8082a626405ba3000ff55c1c35beb1a2c4b40906226ffb874978e53"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 963f53879069f42850c19a2230c331017d5ed2624336820d06417916f4fab3a7
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
      "creator_id": 629,
      "id": 209,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 213,
      "discipline_id": 214,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
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
      "updated_at": "2016-10-25T20:32:27.409Z",
      "shortname": "fu-course-166"
    },
    {
      "creator_id": 629,
      "id": 210,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 214,
      "discipline_id": 215,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
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
      "updated_at": "2016-10-25T20:32:27.446Z",
      "shortname": "fu-course-167"
    },
    {
      "creator_id": 630,
      "id": 211,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 215,
      "discipline_id": 216,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
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
      "updated_at": "2016-10-25T20:32:27.492Z",
      "shortname": "fu-course-168"
    },
    {
      "creator_id": 630,
      "id": 212,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 202,
      "additional_university_ids": [

      ],
      "topic_id": 216,
      "discipline_id": 217,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
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
      "updated_at": "2016-10-25T20:32:27.532Z",
      "shortname": "fu-course-169"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 963f53879069f42850c19a2230c331017d5ed2624336820d06417916f4fab3a7"
```
