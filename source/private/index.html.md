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
DELETE /v2/chapters/102
Content-Type: application/json
Authorization: Bearer 6b9780aee1e96a91d0b1dd07f916900c7d0facb0197f32a98c865d1a32b810d0
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/102" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b9780aee1e96a91d0b1dd07f916900c7d0facb0197f32a98c865d1a32b810d0"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/105
Content-Type: application/json
Authorization: Bearer ab4568b3a04b6301aa9494dc68be3ed0533394c2b0691fb00b9dc6ec6957c78a
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
    "id": 105,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T11:27:41.724Z",
    "course_id": 164,
    "author_id": 555,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-03T11:27:41.225Z",
    "questions_updated_at": "2016-11-03T11:27:41.225Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 558,
        "chapter_id": 105,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.673Z",
        "created_at": "2016-11-03T11:27:41.673Z",
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
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 559,
        "chapter_id": 105,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.708Z",
        "created_at": "2016-11-03T11:27:41.708Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 556,
        "chapter_id": 105,
        "position": 73,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.428Z",
        "created_at": "2016-11-03T11:27:41.325Z",
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
      },
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 557,
        "chapter_id": 105,
        "position": 74,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:41.607Z",
        "created_at": "2016-11-03T11:27:41.495Z",
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
            "id": 158,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 159,
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
curl "api.goskive.com/v2/chapters/105" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab4568b3a04b6301aa9494dc68be3ed0533394c2b0691fb00b9dc6ec6957c78a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/107
Content-Type: application/json
Authorization: Bearer 46abbd5cdd4fcdbcf3859189132c4d1b2a48319ec8ed435b9ef125c750ed1a77
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
    "id": 107,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T11:27:42.041Z",
    "course_id": 166,
    "author_id": 565,
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
curl "api.goskive.com/v2/chapters/107" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46abbd5cdd4fcdbcf3859189132c4d1b2a48319ec8ed435b9ef125c750ed1a77"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/18
Content-Type: application/json
Authorization: Bearer 9ec1c4adf24342572729a64384a11e7a696134ddad6ab51f81d76cde816f5628
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ec1c4adf24342572729a64384a11e7a696134ddad6ab51f81d76cde816f5628"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2705dff46d6a1dea5b0ca3486c627c4c6e2915ec3120e50b89f30132260a2d94
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
      "id": 28,
      "author_id": 412,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:28.419Z",
      "status": "published",
      "subject_id": 111,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 414,
      "reply_to_id": 28,
      "created_at": "2016-11-03T11:27:28.497Z",
      "status": "published",
      "subject_id": 112,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 416,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:28.578Z",
      "status": "published",
      "subject_id": 113,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 418,
      "reply_to_id": 30,
      "created_at": "2016-11-03T11:27:28.658Z",
      "status": "published",
      "subject_id": 114,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 420,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:28.738Z",
      "status": "reported",
      "subject_id": 115,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 422,
      "reply_to_id": 32,
      "created_at": "2016-11-03T11:27:28.818Z",
      "status": "published",
      "subject_id": 116,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 424,
      "reply_to_id": 32,
      "created_at": "2016-11-03T11:27:28.899Z",
      "status": "published",
      "subject_id": 117,
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
	-H "Authorization: Bearer 2705dff46d6a1dea5b0ca3486c627c4c6e2915ec3120e50b89f30132260a2d94"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer f9dfb799f2a3414619f44165c37e8d5928420e03353d9e79419b507a08329166
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
      "id": 35,
      "author_id": 427,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:29.032Z",
      "status": "published",
      "subject_id": 118,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 429,
      "reply_to_id": 35,
      "created_at": "2016-11-03T11:27:29.110Z",
      "status": "published",
      "subject_id": 119,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 431,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:29.190Z",
      "status": "published",
      "subject_id": 120,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 433,
      "reply_to_id": 37,
      "created_at": "2016-11-03T11:27:29.269Z",
      "status": "published",
      "subject_id": 121,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 435,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:29.375Z",
      "status": "reported",
      "subject_id": 122,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 437,
      "reply_to_id": 39,
      "created_at": "2016-11-03T11:27:29.451Z",
      "status": "published",
      "subject_id": 123,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 439,
      "reply_to_id": 39,
      "created_at": "2016-11-03T11:27:29.529Z",
      "status": "published",
      "subject_id": 124,
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
	-H "Authorization: Bearer f9dfb799f2a3414619f44165c37e8d5928420e03353d9e79419b507a08329166"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer a34a884f69ffbe29e1e2920b9b4e999b503d125744649aacedbf82a0ae1e2cbd
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
      "id": 22,
      "author_id": 399,
      "reply_to_id": 21,
      "created_at": "2016-11-03T11:27:27.900Z",
      "status": "published",
      "subject_id": 105,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 403,
      "reply_to_id": 23,
      "created_at": "2016-11-03T11:27:28.056Z",
      "status": "published",
      "subject_id": 107,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 407,
      "reply_to_id": 25,
      "created_at": "2016-11-03T11:27:28.211Z",
      "status": "published",
      "subject_id": 109,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 409,
      "reply_to_id": 25,
      "created_at": "2016-11-03T11:27:28.290Z",
      "status": "published",
      "subject_id": 110,
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
	-H "Authorization: Bearer a34a884f69ffbe29e1e2920b9b4e999b503d125744649aacedbf82a0ae1e2cbd"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 9935b5f7a670d0c61a4a877573c616b89656b24c05d0965608372184a1f781e5
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
      "id": 46,
      "author_id": 450,
      "reply_to_id": null,
      "created_at": "2016-11-03T11:27:29.971Z",
      "status": "reported",
      "subject_id": 129,
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
	-H "Authorization: Bearer 9935b5f7a670d0c61a4a877573c616b89656b24c05d0965608372184a1f781e5"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/17/republish
Content-Type: application/json
Authorization: Bearer 901ac4950b7d6337ad8773c2f753eba60c85188f209d90027e517ff366d6ac0a
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/17/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 901ac4950b7d6337ad8773c2f753eba60c85188f209d90027e517ff366d6ac0a"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 5264d0d8f51e0ec665001bb64922e36827071d06cae937a5cb0de65df34ad25e
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
    "id": 35,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T11:27:08.087Z",
    "course_id": 33,
    "author_id": 128,
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
	-H "Authorization: Bearer 5264d0d8f51e0ec665001bb64922e36827071d06cae937a5cb0de65df34ad25e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/35/chapters
Content-Type: application/json
Authorization: Bearer 1de4969e8cea160c80dbf838d9d3989ac588416df6ae6c518391727bfda6e4c5
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
    "id": 37,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T11:27:08.341Z",
    "course_id": 35,
    "author_id": 132,
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
curl "api.goskive.com/v2/courses/35/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1de4969e8cea160c80dbf838d9d3989ac588416df6ae6c518391727bfda6e4c5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4243c0f93ef519d3baf589c3f227036f82782b0da8ae023c4a8794ae00aef3f1
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
      "id": 23,
      "title": "Clever Chapter Title 23",
      "position": 1,
      "updated_at": "2016-11-03T11:27:06.691Z",
      "course_id": 26,
      "author_id": 101,
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
      "id": 24,
      "title": "Clever Chapter Title 24",
      "position": 2,
      "updated_at": "2016-11-03T11:27:06.713Z",
      "course_id": 26,
      "author_id": 102,
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
      "id": 25,
      "title": "Clever Chapter Title 25",
      "position": 3,
      "updated_at": "2016-11-03T11:27:06.956Z",
      "course_id": 26,
      "author_id": 103,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-03T11:27:06.620Z",
      "questions_updated_at": "2016-11-03T11:27:06.620Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4243c0f93ef519d3baf589c3f227036f82782b0da8ae023c4a8794ae00aef3f1"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 0f83c730e75bcf3789c3e90df92d67ce41d82c076f4d3be7af808ce60b29ed29
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
      "id": 26,
      "title": "Clever Chapter Title 26",
      "position": 1,
      "updated_at": "2016-11-03T11:27:07.094Z",
      "course_id": 27,
      "author_id": 108,
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
      "id": 27,
      "title": "Clever Chapter Title 27",
      "position": 2,
      "updated_at": "2016-11-03T11:27:07.116Z",
      "course_id": 27,
      "author_id": 109,
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
      "id": 28,
      "title": "Clever Chapter Title 28",
      "position": 3,
      "updated_at": "2016-11-03T11:27:07.139Z",
      "course_id": 27,
      "author_id": 110,
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
	-H "Authorization: Bearer 0f83c730e75bcf3789c3e90df92d67ce41d82c076f4d3be7af808ce60b29ed29"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/145
Content-Type: application/json
Authorization: Bearer 46228569c6388e9528b85248c3ec6660e56c332a6729fb0260c266aa8f72c5ad
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/145" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46228569c6388e9528b85248c3ec6660e56c332a6729fb0260c266aa8f72c5ad"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 79775e9592be5d3fb922a61e127b2bbcfe2eccc5c8d4cdd96a50ee5f6f149b13
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
	-H "Authorization: Bearer 79775e9592be5d3fb922a61e127b2bbcfe2eccc5c8d4cdd96a50ee5f6f149b13"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 7526387e9d82708fe2981697f9f69b8bd0e0e2fc5ed054b7677b5a58b93bcda5
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
    "creator_id": 479,
    "id": 141,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 142,
    "additional_university_ids": [

    ],
    "topic_id": 146,
    "discipline_id": 147,
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
    "chapters_updated_at": "2016-11-03T11:27:32.380Z",
    "updated_at": "2016-11-03T11:27:33.747Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 89,
        "title": "Clever Chapter Title 77",
        "position": 1,
        "updated_at": "2016-11-03T11:27:33.703Z",
        "course_id": 141,
        "author_id": 479,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T11:27:32.380Z",
        "questions_updated_at": "2016-11-03T11:27:32.380Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 90,
        "title": "Clever Chapter Title 78",
        "position": 2,
        "updated_at": "2016-11-03T11:27:33.740Z",
        "course_id": 141,
        "author_id": 479,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T11:27:32.380Z",
        "questions_updated_at": "2016-11-03T11:27:32.380Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 479,
        "chapter_id": 89,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.553Z",
        "created_at": "2016-11-03T11:27:33.553Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 479,
        "chapter_id": 90,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.619Z",
        "created_at": "2016-11-03T11:27:33.619Z",
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
        "author_id": 479,
        "chapter_id": 89,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.590Z",
        "created_at": "2016-11-03T11:27:33.590Z",
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
        "author_id": 479,
        "chapter_id": 90,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.657Z",
        "created_at": "2016-11-03T11:27:33.657Z",
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
        "author_id": 482,
        "chapter_id": 89,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.694Z",
        "created_at": "2016-11-03T11:27:33.694Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 483,
        "chapter_id": 90,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T11:27:33.730Z",
        "created_at": "2016-11-03T11:27:33.730Z",
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
	-H "Authorization: Bearer 7526387e9d82708fe2981697f9f69b8bd0e0e2fc5ed054b7677b5a58b93bcda5"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/154
Content-Type: application/json
Authorization: Bearer 32a938e7f64d1a1da11b6fe31ab48d9d91fc3624f226f1400859af76e4a4dc57
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
    "creator_id": 518,
    "id": 154,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 155,
    "additional_university_ids": [

    ],
    "topic_id": 159,
    "discipline_id": 160,
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
    "updated_at": "2016-11-03T11:27:38.403Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/154" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32a938e7f64d1a1da11b6fe31ab48d9d91fc3624f226f1400859af76e4a4dc57"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d7b36c5293cf099711972e629f72197a8b073d614ca05c939649bcfec9e07d8d
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
    "creator_id": 520,
    "id": 155,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 156,
    "additional_university_ids": [

    ],
    "topic_id": 160,
    "discipline_id": 161,
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
    "updated_at": "2016-11-03T11:27:38.532Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7b36c5293cf099711972e629f72197a8b073d614ca05c939649bcfec9e07d8d"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer b6beded0f306218cc977d7000ceec5d67ddea78abdafc399880b52ad852e5841
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
      "user_id": 163,
      "feedbackable_id": 9,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:10.753Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 167,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:11.039Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 171,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:11.326Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 175,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:11.610Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 179,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T11:27:11.900Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6beded0f306218cc977d7000ceec5d67ddea78abdafc399880b52ad852e5841"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer dac8e1261722cd3bbd8a45c13b5aaf70e74267e05a503e8ee2c76f754130655b
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
      "user_id": 158,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T11:27:10.439Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dac8e1261722cd3bbd8a45c13b5aaf70e74267e05a503e8ee2c76f754130655b"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer dc4eaf7f8d5800d52c10c015ec7c004889bc7dde16e59e54fa2d97cd62d37fc6
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc4eaf7f8d5800d52c10c015ec7c004889bc7dde16e59e54fa2d97cd62d37fc6"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/16/metadata
Content-Type: application/json
Authorization: Bearer fab5561ebc729ae81a122d010821055073d2088744f03109330a1b8529fdc5d5
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
    "id": 16,
    "uploader": {
      "id": 687,
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
      "created_at": "2016-11-03T11:27:49.431Z",
      "updated_at": "2016-11-03T11:27:49.431Z"
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
    "created_at": "2016-11-03T11:27:49.501Z",
    "updated_at": "2016-11-03T11:27:49.501Z",
    "course_id": 204,
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
curl "api.goskive.com/v2/files/16/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fab5561ebc729ae81a122d010821055073d2088744f03109330a1b8529fdc5d5"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/10/feedbacks
Content-Type: application/json
Authorization: Bearer 3ddf8ba5027431e7ea7173b784bd6be9bb25bb111aafe5c3e7f42c116720f09b
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
      "user_id": 46,
      "feedbackable_id": 10,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:02.129Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 45,
      "feedbackable_id": 10,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:27:02.117Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/10/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ddf8ba5027431e7ea7173b784bd6be9bb25bb111aafe5c3e7f42c116720f09b"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 198a3e3873a8641b399aa9e1e32d347127baa193df9660b5e301790a0d8c9422
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
      "id": 68,
      "obfuscated_id": "yVS_7NAdP6s",
      "author_id": 608,
      "chapter_id": 116,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:45.477Z",
      "created_at": "2016-11-03T11:27:45.477Z",
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
      "author_id": 611,
      "chapter_id": 117,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:45.602Z",
      "created_at": "2016-11-03T11:27:45.602Z",
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
      "id": 70,
      "obfuscated_id": "EDEz1xzotLc",
      "author_id": 614,
      "chapter_id": 118,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:45.727Z",
      "created_at": "2016-11-03T11:27:45.727Z",
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 617,
      "chapter_id": 119,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:45.852Z",
      "created_at": "2016-11-03T11:27:45.852Z",
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 620,
      "chapter_id": 120,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:45.978Z",
      "created_at": "2016-11-03T11:27:45.978Z",
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
	-H "Authorization: Bearer 198a3e3873a8641b399aa9e1e32d347127baa193df9660b5e301790a0d8c9422"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer a1572b8f315ff2066a3ed40e7d36920634aa461373853f6dd4384af85ac2a6fc
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 636,
      "chapter_id": 125,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:27:46.648Z",
      "created_at": "2016-11-03T11:27:46.648Z",
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
	-H "Authorization: Bearer a1572b8f315ff2066a3ed40e7d36920634aa461373853f6dd4384af85ac2a6fc"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/65/republish
Content-Type: application/json
Authorization: Bearer 3d5fdb2222057fb1345ffda368af888855acf78f58eb0e7d3e4205a33c0bf490
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/65/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d5fdb2222057fb1345ffda368af888855acf78f58eb0e7d3e4205a33c0bf490"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/105/feedbacks
Content-Type: application/json
Authorization: Bearer d988c3c0f284f5ec8193c093a8e0860215d9347ab57bb5893713aea66b539651
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
      "id": 42,
      "user_id": 871,
      "feedbackable_id": 105,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:28:04.546Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 870,
      "feedbackable_id": 105,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T11:28:04.536Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/105/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d988c3c0f284f5ec8193c093a8e0860215d9347ab57bb5893713aea66b539651"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 794990586bcd97429fad7f5521c082acd2fde1fe589c9bc1753056d263f2d87a
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
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 921,
      "chapter_id": 176,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:09.246Z",
      "created_at": "2016-11-03T11:28:09.133Z",
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
    },
    {
      "id": 119,
      "obfuscated_id": "JRh8sWka24Y",
      "author_id": 924,
      "chapter_id": 177,
      "position": 108,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:09.513Z",
      "created_at": "2016-11-03T11:28:09.399Z",
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
          "id": 241,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 242,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 121,
      "obfuscated_id": "LQhaXfRg6ZA",
      "author_id": 930,
      "chapter_id": 179,
      "position": 110,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:10.054Z",
      "created_at": "2016-11-03T11:28:09.939Z",
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
          "id": 245,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 246,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 120,
      "obfuscated_id": "vEr9LtFjURM",
      "author_id": 927,
      "chapter_id": 178,
      "position": 109,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:09.783Z",
      "created_at": "2016-11-03T11:28:09.668Z",
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
          "id": 243,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 244,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 122,
      "obfuscated_id": "cMWZX2w28hY",
      "author_id": 933,
      "chapter_id": 180,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:10.320Z",
      "created_at": "2016-11-03T11:28:10.210Z",
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
          "id": 247,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 248,
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
	-H "Authorization: Bearer 794990586bcd97429fad7f5521c082acd2fde1fe589c9bc1753056d263f2d87a"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 1adb0f02a373b5ea734ceaa3bc22775938b7372d27b778bb0bbf9d66110f4a7e
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
      "id": 132,
      "obfuscated_id": "RECRPLqMrqE",
      "author_id": 965,
      "chapter_id": 190,
      "position": 121,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T11:28:13.123Z",
      "created_at": "2016-11-03T11:28:13.014Z",
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
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1adb0f02a373b5ea734ceaa3bc22775938b7372d27b778bb0bbf9d66110f4a7e"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/111/republish
Content-Type: application/json
Authorization: Bearer 10fc51698a818e3263f5f20e61922e9762eff58fce76e777df90408faa0ea7f4
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/111/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 10fc51698a818e3263f5f20e61922e9762eff58fce76e777df90408faa0ea7f4"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c04787a0ebf50ad9522035c7d1fdbbe21eee8b66b580e5ac67af174a482de427
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":254,"published":false}}
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
    "creator_id": 815,
    "id": 242,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 249,
    "additional_university_ids": [

    ],
    "topic_id": 254,
    "discipline_id": 255,
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
    "updated_at": "2016-11-03T11:27:59.368Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":254,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c04787a0ebf50ad9522035c7d1fdbbe21eee8b66b580e5ac67af174a482de427"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cda8280540e7099d52a7cbf805c92199107268298c7e457c47e51743afd29cf4
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
      "creator_id": 821,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 260,
      "discipline_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "updated_at": "2016-11-03T11:27:59.865Z",
      "shortname": "fu-course-176"
    },
    {
      "creator_id": 821,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-177",
      "html_url": "https://goskive.com/course/fu-course-177",
      "slug": "fu-course-177",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 261,
      "discipline_id": 262,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 177",
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
      "updated_at": "2016-11-03T11:27:59.903Z",
      "shortname": "fu-course-177"
    },
    {
      "creator_id": 822,
      "id": 250,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-178",
      "html_url": "https://goskive.com/course/fu-course-178",
      "slug": "fu-course-178",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 262,
      "discipline_id": 263,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 178",
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
      "updated_at": "2016-11-03T11:27:59.949Z",
      "shortname": "fu-course-178"
    },
    {
      "creator_id": 822,
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-179",
      "html_url": "https://goskive.com/course/fu-course-179",
      "slug": "fu-course-179",
      "university_id": 253,
      "additional_university_ids": [

      ],
      "topic_id": 263,
      "discipline_id": 264,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
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
      "chapters_updated_at": "2016-11-03T11:28:00.228Z",
      "updated_at": "2016-11-03T11:28:00.235Z",
      "shortname": "fu-course-179"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cda8280540e7099d52a7cbf805c92199107268298c7e457c47e51743afd29cf4"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ff17084f51f5398f2618bb5c736b6d36f7eaf6d3cdda700ac0ce547ea9bfe13e
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
      "creator_id": 827,
      "id": 252,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-180",
      "html_url": "https://goskive.com/course/fu-course-180",
      "slug": "fu-course-180",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 264,
      "discipline_id": 265,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 180",
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
      "updated_at": "2016-11-03T11:28:00.372Z",
      "shortname": "fu-course-180"
    },
    {
      "creator_id": 827,
      "id": 253,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 265,
      "discipline_id": 266,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 181",
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
      "updated_at": "2016-11-03T11:28:00.409Z",
      "shortname": "fu-course-181"
    },
    {
      "creator_id": 828,
      "id": 254,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 266,
      "discipline_id": 267,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 182",
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
      "updated_at": "2016-11-03T11:28:00.454Z",
      "shortname": "fu-course-182"
    },
    {
      "creator_id": 828,
      "id": 255,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-183",
      "html_url": "https://goskive.com/course/fu-course-183",
      "slug": "fu-course-183",
      "university_id": 254,
      "additional_university_ids": [

      ],
      "topic_id": 267,
      "discipline_id": 268,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 183",
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
      "updated_at": "2016-11-03T11:28:00.492Z",
      "shortname": "fu-course-183"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ff17084f51f5398f2618bb5c736b6d36f7eaf6d3cdda700ac0ce547ea9bfe13e"
```
