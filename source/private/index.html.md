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
DELETE /v2/chapters/40
Content-Type: application/json
Authorization: Bearer 4520f37375305337fb50c733f9bc97723a6026552f53eb507d24ab081c6c9e03
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/40" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4520f37375305337fb50c733f9bc97723a6026552f53eb507d24ab081c6c9e03"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/36
Content-Type: application/json
Authorization: Bearer 81f4d8d0db345cc2aab2925a6b5249f13753ed578d0e5a8988a3fcfebc834008
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
    "id": 36,
    "updated_at": "2016-12-08T20:51:35.411Z",
    "course_id": 50,
    "author_id": 206,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-08T20:51:34.941Z",
    "questions_updated_at": "2016-12-08T20:51:34.941Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 15,
        "obfuscated_id": "j5PwoYQzNCc",
        "author_id": 209,
        "chapter_id": 36,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:35.355Z",
        "created_at": "2016-12-08T20:51:35.355Z",
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
        "author_id": 210,
        "chapter_id": 36,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:35.393Z",
        "created_at": "2016-12-08T20:51:35.393Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 207,
        "chapter_id": 36,
        "position": 25,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:35.146Z",
        "created_at": "2016-12-08T20:51:35.072Z",
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
      },
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 208,
        "chapter_id": 36,
        "position": 26,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:51:35.294Z",
        "created_at": "2016-12-08T20:51:35.210Z",
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
            "id": 51,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 52,
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
curl "api.goskive.com/v2/chapters/36" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81f4d8d0db345cc2aab2925a6b5249f13753ed578d0e5a8988a3fcfebc834008"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/37
Content-Type: application/json
Authorization: Bearer a603212c8b7f816b07f8d9831df2598028e8415671ba637a4cf0303ee8a28761
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
    "id": 37,
    "updated_at": "2016-12-08T20:51:35.657Z",
    "course_id": 51,
    "author_id": 213,
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
curl "api.goskive.com/v2/chapters/37" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a603212c8b7f816b07f8d9831df2598028e8415671ba637a4cf0303ee8a28761"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 1215502432924529315b439711502c4c6b7188d2af40d6fc3f8a0300f3be6b0f
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
	-H "Authorization: Bearer 1215502432924529315b439711502c4c6b7188d2af40d6fc3f8a0300f3be6b0f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer ed10e8bac159dee13ced766992b0e963c94d5a9def2fda4de2c4901a7d27dfea
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
      "id": 9,
      "author_id": 458,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:55.537Z",
      "status": "published",
      "subject_id": 124,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 460,
      "reply_to_id": 9,
      "created_at": "2016-12-08T20:51:55.645Z",
      "status": "published",
      "subject_id": 125,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 462,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:55.777Z",
      "status": "published",
      "subject_id": 126,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 464,
      "reply_to_id": 11,
      "created_at": "2016-12-08T20:51:55.879Z",
      "status": "published",
      "subject_id": 127,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 466,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:55.982Z",
      "status": "reported",
      "subject_id": 128,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 468,
      "reply_to_id": 13,
      "created_at": "2016-12-08T20:51:56.086Z",
      "status": "published",
      "subject_id": 129,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 470,
      "reply_to_id": 13,
      "created_at": "2016-12-08T20:51:56.190Z",
      "status": "published",
      "subject_id": 130,
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
	-H "Authorization: Bearer ed10e8bac159dee13ced766992b0e963c94d5a9def2fda4de2c4901a7d27dfea"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 37d38b541b00eb2e82f85aafe1736fe46f90b15b45d44cbf1cea5403df4bc156
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
      "id": 16,
      "author_id": 473,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:56.356Z",
      "status": "published",
      "subject_id": 131,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 475,
      "reply_to_id": 16,
      "created_at": "2016-12-08T20:51:56.462Z",
      "status": "published",
      "subject_id": 132,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 477,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:56.568Z",
      "status": "published",
      "subject_id": 133,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 479,
      "reply_to_id": 18,
      "created_at": "2016-12-08T20:51:56.674Z",
      "status": "published",
      "subject_id": 134,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 481,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:56.780Z",
      "status": "reported",
      "subject_id": 135,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 483,
      "reply_to_id": 20,
      "created_at": "2016-12-08T20:51:56.884Z",
      "status": "published",
      "subject_id": 136,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 485,
      "reply_to_id": 20,
      "created_at": "2016-12-08T20:51:56.992Z",
      "status": "published",
      "subject_id": 137,
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
	-H "Authorization: Bearer 37d38b541b00eb2e82f85aafe1736fe46f90b15b45d44cbf1cea5403df4bc156"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer b1a559a8fade395d41625e614c7146f7fbed7c4959fbfcdce966daf62627a876
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
      "id": 31,
      "author_id": 505,
      "reply_to_id": 30,
      "created_at": "2016-12-08T20:51:58.068Z",
      "status": "published",
      "subject_id": 146,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 509,
      "reply_to_id": 32,
      "created_at": "2016-12-08T20:51:58.288Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 513,
      "reply_to_id": 34,
      "created_at": "2016-12-08T20:51:58.539Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 515,
      "reply_to_id": 34,
      "created_at": "2016-12-08T20:51:58.650Z",
      "status": "published",
      "subject_id": 151,
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
	-H "Authorization: Bearer b1a559a8fade395d41625e614c7146f7fbed7c4959fbfcdce966daf62627a876"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 63dbb9a14f848caa94228274ee049ff90e67313997b18c344c294a327aa320a9
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
      "id": 41,
      "author_id": 526,
      "reply_to_id": null,
      "created_at": "2016-12-08T20:51:59.286Z",
      "status": "reported",
      "subject_id": 156,
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
	-H "Authorization: Bearer 63dbb9a14f848caa94228274ee049ff90e67313997b18c344c294a327aa320a9"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer e2c1bdbd3d35c97db14e0211bf7288ffa0c601553a0943fdba34c08eb9ed2f88
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
	-H "Authorization: Bearer e2c1bdbd3d35c97db14e0211bf7288ffa0c601553a0943fdba34c08eb9ed2f88"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5e75faa2a4b3a26da5e54711eda96915cb69a58d6dd32ae40c320a27b897eab2
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
    "id": 77,
    "updated_at": "2016-12-08T20:51:44.349Z",
    "course_id": 82,
    "author_id": 331,
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
	-H "Authorization: Bearer 5e75faa2a4b3a26da5e54711eda96915cb69a58d6dd32ae40c320a27b897eab2"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/84/chapters
Content-Type: application/json
Authorization: Bearer 5a59f642a4cac11daf2bc9a0a68660f0cd6119294b6b23f9eb6f15ed85bc0f32
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
    "id": 79,
    "updated_at": "2016-12-08T20:51:44.679Z",
    "course_id": 84,
    "author_id": 335,
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
curl "api.goskive.com/v2/courses/84/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a59f642a4cac11daf2bc9a0a68660f0cd6119294b6b23f9eb6f15ed85bc0f32"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c39d67c27bed1fface915b64255bd14fef59a42a93e9c9d2f59a80c92960be5f
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
      "id": 56,
      "updated_at": "2016-12-08T20:51:41.469Z",
      "course_id": 70,
      "author_id": 283,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 47",
      "position": 1
    },
    {
      "id": 57,
      "updated_at": "2016-12-08T20:51:41.494Z",
      "course_id": 70,
      "author_id": 284,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 48",
      "position": 2
    },
    {
      "id": 58,
      "updated_at": "2016-12-08T20:51:41.710Z",
      "course_id": 70,
      "author_id": 285,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-08T20:51:41.371Z",
      "questions_updated_at": "2016-12-08T20:51:41.371Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 49",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c39d67c27bed1fface915b64255bd14fef59a42a93e9c9d2f59a80c92960be5f"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer daba0d81be649b54cefd7c6a1991e58f4463991644d57dcc4687fa6036c69548
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
      "id": 59,
      "updated_at": "2016-12-08T20:51:42.015Z",
      "course_id": 72,
      "author_id": 292,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 50",
      "position": 1
    },
    {
      "id": 60,
      "updated_at": "2016-12-08T20:51:42.041Z",
      "course_id": 72,
      "author_id": 293,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 51",
      "position": 2
    },
    {
      "id": 61,
      "updated_at": "2016-12-08T20:51:42.067Z",
      "course_id": 72,
      "author_id": 294,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 52",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer daba0d81be649b54cefd7c6a1991e58f4463991644d57dcc4687fa6036c69548"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/165
Content-Type: application/json
Authorization: Bearer 8cc5608e08aff8466e12e922767730dedd67ac8b1fc811f7cff4363027608369
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/165" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cc5608e08aff8466e12e922767730dedd67ac8b1fc811f7cff4363027608369"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5dda30f358d1bae1c05cc1176e3ebd530cd55734808407bb33535463d53e19ad
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
	-H "Authorization: Bearer 5dda30f358d1bae1c05cc1176e3ebd530cd55734808407bb33535463d53e19ad"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer f6ed104bc674ce4bbb9206b312006d11401de97ccc578b200c98a326674a8ad2
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
    "creator_id": 575,
    "id": 176,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 177,
    "additional_university_ids": [

    ],
    "discipline_id": 184,
    "permissions": [
      "update",
      "delete"
    ],
    "chapters_count": 2,
    "course_requests_count": 0,
    "flashcards_count": 6,
    "questions_count": 6,
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
    "chapters_updated_at": "2016-12-08T20:52:05.572Z",
    "updated_at": "2016-12-08T20:52:06.905Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 575,
        "chapter_id": 100,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.666Z",
        "created_at": "2016-12-08T20:52:06.666Z",
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
        "author_id": 575,
        "chapter_id": 101,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.748Z",
        "created_at": "2016-12-08T20:52:06.748Z",
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
        "author_id": 575,
        "chapter_id": 100,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.713Z",
        "created_at": "2016-12-08T20:52:06.713Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 575,
        "chapter_id": 101,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.793Z",
        "created_at": "2016-12-08T20:52:06.793Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 578,
        "chapter_id": 100,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.837Z",
        "created_at": "2016-12-08T20:52:06.837Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 579,
        "chapter_id": 101,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T20:52:06.882Z",
        "created_at": "2016-12-08T20:52:06.882Z",
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
    "chapters": [
      {
        "id": 100,
        "updated_at": "2016-12-08T20:52:06.848Z",
        "course_id": 176,
        "author_id": 575,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T20:52:05.572Z",
        "questions_updated_at": "2016-12-08T20:52:05.572Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 88",
        "position": 1
      },
      {
        "id": 101,
        "updated_at": "2016-12-08T20:52:06.894Z",
        "course_id": 176,
        "author_id": 575,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T20:52:05.572Z",
        "questions_updated_at": "2016-12-08T20:52:05.572Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 89",
        "position": 2
      }
    ],
    "topic_id": 184,
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
curl "api.goskive.com/v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6ed104bc674ce4bbb9206b312006d11401de97ccc578b200c98a326674a8ad2"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/164
Content-Type: application/json
Authorization: Bearer e66a0c83d53996f50bd0903b10de69117d329008c95def7bbf9228d1b7e1c65e
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
    "creator_id": 542,
    "id": 164,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 165,
    "additional_university_ids": [

    ],
    "discipline_id": 172,
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
    "updated_at": "2016-12-08T20:52:00.606Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 172,
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
curl "api.goskive.com/v2/courses/164" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e66a0c83d53996f50bd0903b10de69117d329008c95def7bbf9228d1b7e1c65e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0158fe63b0de431b8a4565572a7fc026debe6eb696ac60f677bdace23b12ca03
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
    "creator_id": 539,
    "id": 162,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "discipline_id": 170,
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
    "updated_at": "2016-12-08T20:52:00.212Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 170,
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
	-H "Authorization: Bearer 0158fe63b0de431b8a4565572a7fc026debe6eb696ac60f677bdace23b12ca03"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 4cc2ef32ec73756b5c65cee44fffd21ab00b7a528d68934375e15ce5abdf5c05
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
      "id": 15,
      "user_id": 94,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:27.787Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 98,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:28.056Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 102,
      "feedbackable_id": 20,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:28.328Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 106,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:28.602Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 110,
      "feedbackable_id": 22,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T20:51:28.877Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cc2ef32ec73756b5c65cee44fffd21ab00b7a528d68934375e15ce5abdf5c05"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 3a6b351ae168022c49c49f618cd12cb539a477022dba0f057670f930d47d9041
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
      "user_id": 89,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T20:51:27.477Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a6b351ae168022c49c49f618cd12cb539a477022dba0f057670f930d47d9041"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 17660c3631b195fd0e99f7d58a39efa3ab282f417be074348c33178e07e62438
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
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17660c3631b195fd0e99f7d58a39efa3ab282f417be074348c33178e07e62438"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/5/metadata
Content-Type: application/json
Authorization: Bearer 08960eb55d2a1f533faf89798912dce97dd273bf5defdd37bdfe0362e01ed4fd
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
    "id": 5,
    "uploader": {
      "id": 172,
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
      "created_at": "2016-12-08T20:51:32.936Z",
      "updated_at": "2016-12-08T20:51:32.936Z"
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
    "created_at": "2016-12-08T20:51:33.034Z",
    "updated_at": "2016-12-08T20:51:33.034Z",
    "course_id": 40,
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
curl "api.goskive.com/v2/files/5/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 08960eb55d2a1f533faf89798912dce97dd273bf5defdd37bdfe0362e01ed4fd"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/91/feedbacks
Content-Type: application/json
Authorization: Bearer 7cb6066368e7be58a5992cf0c7581f3ba669bdc715999c84b63d50adbbca7ebb
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
      "user_id": 811,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:25.917Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 810,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:52:25.906Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cb6066368e7be58a5992cf0c7581f3ba669bdc715999c84b63d50adbbca7ebb"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer b6d3aac1115f647625781b5d67becc7a6b38b7349f5f94f09e6dfd7579229c1c
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
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 675,
      "chapter_id": 124,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:15.120Z",
      "created_at": "2016-12-08T20:52:15.120Z",
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
      "id": 65,
      "obfuscated_id": "Pu1fo5_Q1vk",
      "author_id": 678,
      "chapter_id": 125,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:15.291Z",
      "created_at": "2016-12-08T20:52:15.291Z",
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
      "id": 66,
      "obfuscated_id": "H7dODBospvw",
      "author_id": 681,
      "chapter_id": 126,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:15.458Z",
      "created_at": "2016-12-08T20:52:15.458Z",
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 684,
      "chapter_id": 127,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:15.630Z",
      "created_at": "2016-12-08T20:52:15.630Z",
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
      "author_id": 687,
      "chapter_id": 128,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:15.800Z",
      "created_at": "2016-12-08T20:52:15.800Z",
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
	-H "Authorization: Bearer b6d3aac1115f647625781b5d67becc7a6b38b7349f5f94f09e6dfd7579229c1c"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 68175083d90d9ca3536922a569e6990b6eecd38426a61f3131b8c04c681b4e41
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 671,
      "chapter_id": 123,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:14.914Z",
      "created_at": "2016-12-08T20:52:14.914Z",
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
	-H "Authorization: Bearer 68175083d90d9ca3536922a569e6990b6eecd38426a61f3131b8c04c681b4e41"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/republish
Content-Type: application/json
Authorization: Bearer 44122d78e77a489d8f965cb7c6e084e55377d1d804990b66b07ee884fd348a64
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 44122d78e77a489d8f965cb7c6e084e55377d1d804990b66b07ee884fd348a64"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/30/feedbacks
Content-Type: application/json
Authorization: Bearer 22b8039105d980014dae4387473955f4131ceb6fbdd5836f6eec2670b944557b
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
      "id": 30,
      "user_id": 239,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:37.532Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 238,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T20:51:37.521Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/30/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22b8039105d980014dae4387473955f4131ceb6fbdd5836f6eec2670b944557b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 8b73b05a21aa52d7f200e75d402481e0898404e47d451b41792eb984204e9766
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
      "id": 107,
      "obfuscated_id": "_2rgp7tgq8o",
      "author_id": 860,
      "chapter_id": 166,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:30.778Z",
      "created_at": "2016-12-08T20:52:30.698Z",
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
          "id": 214,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 215,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 108,
      "obfuscated_id": "3MKez0MLRBM",
      "author_id": 863,
      "chapter_id": 167,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:31.030Z",
      "created_at": "2016-12-08T20:52:30.948Z",
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
          "id": 216,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 217,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 105,
      "obfuscated_id": "3yX9LpVrF_M",
      "author_id": 854,
      "chapter_id": 164,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:30.272Z",
      "created_at": "2016-12-08T20:52:30.192Z",
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
          "id": 210,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 211,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 106,
      "obfuscated_id": "GEL902caNek",
      "author_id": 857,
      "chapter_id": 165,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:30.522Z",
      "created_at": "2016-12-08T20:52:30.442Z",
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
          "id": 212,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 213,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 109,
      "obfuscated_id": "VSPyck5c2RY",
      "author_id": 866,
      "chapter_id": 168,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:31.273Z",
      "created_at": "2016-12-08T20:52:31.199Z",
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
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b73b05a21aa52d7f200e75d402481e0898404e47d451b41792eb984204e9766"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 2aa80d6fdce2b07c7cca98e6e4ca81a57b9a6b8d34f5e699d202039e28579e67
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
      "id": 114,
      "obfuscated_id": "RwCVsRO9fcs",
      "author_id": 882,
      "chapter_id": 173,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T20:52:32.602Z",
      "created_at": "2016-12-08T20:52:32.528Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2aa80d6fdce2b07c7cca98e6e4ca81a57b9a6b8d34f5e699d202039e28579e67"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/98/republish
Content-Type: application/json
Authorization: Bearer 528cb21d0a5d70d1d7f3e97f571608a40bc7a40b3ee6ba41c390a61701a3f6d7
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/98/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 528cb21d0a5d70d1d7f3e97f571608a40bc7a40b3ee6ba41c390a61701a3f6d7"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a30a3aec3053447f0fd831f110927d4ba3260bc8353ee9401e15a1fff982bdba
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":229,"published":false}}
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
    "creator_id": 729,
    "id": 219,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 221,
    "additional_university_ids": [

    ],
    "discipline_id": 229,
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
    "updated_at": "2016-12-08T20:52:19.039Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 229,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":229,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a30a3aec3053447f0fd831f110927d4ba3260bc8353ee9401e15a1fff982bdba"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c1a8b025a61dbb40c878646cb8c7a260150dec51ad69f57d8ba076cb0dee86b1
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
      "creator_id": 736,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 236,
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
      "updated_at": "2016-12-08T20:52:19.993Z",
      "shortname": "fu-course-163",
      "topic_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 736,
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-164",
      "html_url": "https://goskive.com/course/fu-course-164",
      "slug": "fu-course-164",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 237,
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
      "updated_at": "2016-12-08T20:52:20.027Z",
      "shortname": "fu-course-164",
      "topic_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 164",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 737,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-165",
      "html_url": "https://goskive.com/course/fu-course-165",
      "slug": "fu-course-165",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 238,
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
      "updated_at": "2016-12-08T20:52:20.069Z",
      "shortname": "fu-course-165",
      "topic_id": 238,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 165",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 737,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-166",
      "html_url": "https://goskive.com/course/fu-course-166",
      "slug": "fu-course-166",
      "university_id": 226,
      "additional_university_ids": [

      ],
      "discipline_id": 239,
      "permissions": [
        "update",
        "delete"
      ],
      "chapters_count": 1,
      "course_requests_count": 0,
      "flashcards_count": 1,
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
      "chapters_updated_at": "2016-12-08T20:52:19.910Z",
      "updated_at": "2016-12-08T20:52:20.348Z",
      "shortname": "fu-course-166",
      "topic_id": 239,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 166",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1a8b025a61dbb40c878646cb8c7a260150dec51ad69f57d8ba076cb0dee86b1"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 9762816333beaf0f59826afbbbd7e30a744919ef2b3a16b529b1b14bb9139109
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
      "creator_id": 743,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-167",
      "html_url": "https://goskive.com/course/fu-course-167",
      "slug": "fu-course-167",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 240,
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
      "updated_at": "2016-12-08T20:52:20.630Z",
      "shortname": "fu-course-167",
      "topic_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 167",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 743,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-168",
      "html_url": "https://goskive.com/course/fu-course-168",
      "slug": "fu-course-168",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 241,
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
      "updated_at": "2016-12-08T20:52:20.664Z",
      "shortname": "fu-course-168",
      "topic_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 168",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 744,
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-169",
      "html_url": "https://goskive.com/course/fu-course-169",
      "slug": "fu-course-169",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 242,
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
      "updated_at": "2016-12-08T20:52:20.706Z",
      "shortname": "fu-course-169",
      "topic_id": 242,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 169",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 744,
      "id": 233,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-170",
      "html_url": "https://goskive.com/course/fu-course-170",
      "slug": "fu-course-170",
      "university_id": 228,
      "additional_university_ids": [

      ],
      "discipline_id": 243,
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
      "updated_at": "2016-12-08T20:52:20.741Z",
      "shortname": "fu-course-170",
      "topic_id": 243,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 170",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9762816333beaf0f59826afbbbd7e30a744919ef2b3a16b529b1b14bb9139109"
```
