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
DELETE /v2/chapters/186
Content-Type: application/json
Authorization: Bearer 11f14e0802da60eb5740b56c8f9d10a33ca437b750fca09d7b5a224bf90a8eed
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/186" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 11f14e0802da60eb5740b56c8f9d10a33ca437b750fca09d7b5a224bf90a8eed"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/184
Content-Type: application/json
Authorization: Bearer b6d0c45d6e4dbb3146f4aacdcd1e32192ff64df71d3be2f66c3ea7be09023cea
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
    "id": 184,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T18:44:42.313Z",
    "course_id": 296,
    "author_id": 921,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-14T18:44:41.787Z",
    "questions_updated_at": "2016-10-14T18:44:41.787Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 924,
        "chapter_id": 184,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.257Z",
        "created_at": "2016-10-14T18:44:42.257Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 925,
        "chapter_id": 184,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.296Z",
        "created_at": "2016-10-14T18:44:42.296Z",
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
        "id": 126,
        "obfuscated_id": "fKTMLttUR-w",
        "author_id": 922,
        "chapter_id": 184,
        "position": 113,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.004Z",
        "created_at": "2016-10-14T18:44:41.898Z",
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
        "author_id": 923,
        "chapter_id": 184,
        "position": 114,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:44:42.188Z",
        "created_at": "2016-10-14T18:44:42.074Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/184" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b6d0c45d6e4dbb3146f4aacdcd1e32192ff64df71d3be2f66c3ea7be09023cea"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 122819edb366c8d09b80d563b547154fb732ff0ffdd817db7f32258e47a43ec7
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
    "id": 191,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T18:44:44.192Z",
    "course_id": 303,
    "author_id": 950,
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
curl "api.goskive.com/v2/chapters/191" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 122819edb366c8d09b80d563b547154fb732ff0ffdd817db7f32258e47a43ec7"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/17
Content-Type: application/json
Authorization: Bearer 78991738ba3fd75f1074364f0df6d23416ffa869a4db5364f6608311d83cb87c
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78991738ba3fd75f1074364f0df6d23416ffa869a4db5364f6608311d83cb87c"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 645f73ee8d4ee0125dc6abae2e630d2e0f8c03f869b39ca631b761ff60b4ed65
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
      "id": 27,
      "author_id": 800,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:34.644Z",
      "status": "published",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 802,
      "reply_to_id": 27,
      "created_at": "2016-10-14T18:44:34.732Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 804,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:34.824Z",
      "status": "published",
      "subject_id": 253,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 806,
      "reply_to_id": 29,
      "created_at": "2016-10-14T18:44:34.916Z",
      "status": "published",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 808,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:35.012Z",
      "status": "reported",
      "subject_id": 255,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 810,
      "reply_to_id": 31,
      "created_at": "2016-10-14T18:44:35.103Z",
      "status": "published",
      "subject_id": 256,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 812,
      "reply_to_id": 31,
      "created_at": "2016-10-14T18:44:35.230Z",
      "status": "published",
      "subject_id": 257,
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
	-H "Authorization: Bearer 645f73ee8d4ee0125dc6abae2e630d2e0f8c03f869b39ca631b761ff60b4ed65"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 99bb3c86381059b42c36f8ee47b543a14e194179d0bd0dc10a28ba08f3827dec
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
      "id": 34,
      "author_id": 815,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:35.381Z",
      "status": "published",
      "subject_id": 258,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 817,
      "reply_to_id": 34,
      "created_at": "2016-10-14T18:44:35.472Z",
      "status": "published",
      "subject_id": 259,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 819,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:35.569Z",
      "status": "published",
      "subject_id": 260,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 821,
      "reply_to_id": 36,
      "created_at": "2016-10-14T18:44:35.658Z",
      "status": "published",
      "subject_id": 261,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 823,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:35.749Z",
      "status": "reported",
      "subject_id": 262,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 825,
      "reply_to_id": 38,
      "created_at": "2016-10-14T18:44:35.838Z",
      "status": "published",
      "subject_id": 263,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 827,
      "reply_to_id": 38,
      "created_at": "2016-10-14T18:44:35.929Z",
      "status": "published",
      "subject_id": 264,
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
	-H "Authorization: Bearer 99bb3c86381059b42c36f8ee47b543a14e194179d0bd0dc10a28ba08f3827dec"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer c9623a42f3e2021fefd82f2998b52d13d8bdb75b2b7995e9d65b62851ae50219
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
      "id": 49,
      "author_id": 847,
      "reply_to_id": 48,
      "created_at": "2016-10-14T18:44:36.852Z",
      "status": "published",
      "subject_id": 273,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 851,
      "reply_to_id": 50,
      "created_at": "2016-10-14T18:44:37.033Z",
      "status": "published",
      "subject_id": 275,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 855,
      "reply_to_id": 52,
      "created_at": "2016-10-14T18:44:37.220Z",
      "status": "published",
      "subject_id": 277,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 54,
      "author_id": 857,
      "reply_to_id": 52,
      "created_at": "2016-10-14T18:44:37.314Z",
      "status": "published",
      "subject_id": 278,
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
	-H "Authorization: Bearer c9623a42f3e2021fefd82f2998b52d13d8bdb75b2b7995e9d65b62851ae50219"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 2adae101a78ba15560ec90464d4356ae4433d5ed4b2aaf074c900234a1632b93
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
      "id": 24,
      "author_id": 793,
      "reply_to_id": null,
      "created_at": "2016-10-14T18:44:34.337Z",
      "status": "reported",
      "subject_id": 248,
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
	-H "Authorization: Bearer 2adae101a78ba15560ec90464d4356ae4433d5ed4b2aaf074c900234a1632b93"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/14/republish
Content-Type: application/json
Authorization: Bearer fb44f8ccbbbe9c71edea9ae96365655aefea5bb3aa2cf48498f19d50068b007d
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/14/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb44f8ccbbbe9c71edea9ae96365655aefea5bb3aa2cf48498f19d50068b007d"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e23d1f1271c2038d8a45b8ac843900b2e29a44c27a4b841a8499ac04bd9d2f7d
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
    "id": 148,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T18:44:27.847Z",
    "course_id": 211,
    "author_id": 683,
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
	-H "Authorization: Bearer e23d1f1271c2038d8a45b8ac843900b2e29a44c27a4b841a8499ac04bd9d2f7d"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/214/chapters
Content-Type: application/json
Authorization: Bearer 1f706a09721e1fe4c232824581b6a448c3ffd9c1fc7275ae31e8fd706027838c
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
    "id": 150,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T18:44:28.243Z",
    "course_id": 214,
    "author_id": 689,
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
curl "api.goskive.com/v2/courses/214/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f706a09721e1fe4c232824581b6a448c3ffd9c1fc7275ae31e8fd706027838c"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer cd0d58d87d4d63d2ff3997d11460adbe2fa4ddaa3ef9e9e9b0a9b9723c0bed8f
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-14T18:44:30.123Z",
      "course_id": 223,
      "author_id": 723,
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
      "id": 167,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-14T18:44:30.149Z",
      "course_id": 223,
      "author_id": 724,
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
      "id": 168,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-14T18:44:30.434Z",
      "course_id": 223,
      "author_id": 725,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-14T18:44:30.045Z",
      "questions_updated_at": "2016-10-14T18:44:30.045Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd0d58d87d4d63d2ff3997d11460adbe2fa4ddaa3ef9e9e9b0a9b9723c0bed8f"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4d424905d28ea70fca76d64c9197a63371766c87c75fff177921dd6d0c579e00
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
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-14T18:44:30.699Z",
      "course_id": 225,
      "author_id": 732,
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
      "id": 170,
      "title": "Clever Chapter Title 155",
      "position": 2,
      "updated_at": "2016-10-14T18:44:30.725Z",
      "course_id": 225,
      "author_id": 733,
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
      "id": 171,
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-14T18:44:30.751Z",
      "course_id": 225,
      "author_id": 734,
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
	-H "Authorization: Bearer 4d424905d28ea70fca76d64c9197a63371766c87c75fff177921dd6d0c579e00"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bccbea7d4fa77606adfaaebba1b2a05e681e76badc0023671d69c4aeacf02de6
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
	-H "Authorization: Bearer bccbea7d4fa77606adfaaebba1b2a05e681e76badc0023671d69c4aeacf02de6"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/67
Content-Type: application/json
Authorization: Bearer b694f47062f0be826310e34aa299610e9cd660f4568a84a348c2b10b0394defe
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/67" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b694f47062f0be826310e34aa299610e9cd660f4568a84a348c2b10b0394defe"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer c05e014e795d9077a8833db3083f210d2129c3e4166ad44000865a008a19a1ca
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
    "creator_id": 240,
    "id": 72,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 78,
    "additional_university_ids": [

    ],
    "topic_id": 79,
    "discipline_id": 79,
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
    "chapters_updated_at": "2016-10-14T18:43:49.071Z",
    "updated_at": "2016-10-14T18:43:50.820Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 59,
        "title": "Clever Chapter Title 56",
        "position": 1,
        "updated_at": "2016-10-14T18:43:50.766Z",
        "course_id": 72,
        "author_id": 240,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T18:43:49.071Z",
        "questions_updated_at": "2016-10-14T18:43:49.071Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 60,
        "title": "Clever Chapter Title 57",
        "position": 2,
        "updated_at": "2016-10-14T18:43:50.811Z",
        "course_id": 72,
        "author_id": 240,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T18:43:49.071Z",
        "questions_updated_at": "2016-10-14T18:43:49.071Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 240,
        "chapter_id": 59,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.578Z",
        "created_at": "2016-10-14T18:43:50.578Z",
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
        "author_id": 240,
        "chapter_id": 60,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.664Z",
        "created_at": "2016-10-14T18:43:50.664Z",
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
        "author_id": 240,
        "chapter_id": 59,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.627Z",
        "created_at": "2016-10-14T18:43:50.627Z",
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
        "id": 35,
        "obfuscated_id": "soCS52BooV0",
        "author_id": 240,
        "chapter_id": 60,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.710Z",
        "created_at": "2016-10-14T18:43:50.710Z",
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
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 243,
        "chapter_id": 59,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.755Z",
        "created_at": "2016-10-14T18:43:50.755Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 244,
        "chapter_id": 60,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T18:43:50.799Z",
        "created_at": "2016-10-14T18:43:50.799Z",
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
	-H "Authorization: Bearer c05e014e795d9077a8833db3083f210d2129c3e4166ad44000865a008a19a1ca"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/58
Content-Type: application/json
Authorization: Bearer 2160ce931dd59c940cdde5f61542c29aa33cc927702151aedaadeca08fcbf3a1
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
    "creator_id": 203,
    "id": 58,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 64,
    "additional_university_ids": [

    ],
    "topic_id": 65,
    "discipline_id": 65,
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
    "updated_at": "2016-10-14T18:43:43.701Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/58" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2160ce931dd59c940cdde5f61542c29aa33cc927702151aedaadeca08fcbf3a1"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9916a26db89409bf0c7019d03de10eee1841bee5802dafd4ea472d0725541c39
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
    "creator_id": 198,
    "id": 55,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 61,
    "additional_university_ids": [

    ],
    "topic_id": 62,
    "discipline_id": 62,
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
    "updated_at": "2016-10-14T18:43:43.329Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9916a26db89409bf0c7019d03de10eee1841bee5802dafd4ea472d0725541c39"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer b8e30c2279a4e76b4df3e6819a12e2da527e3015430eefe1e71aafc2c88203bc
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
      "id": 42,
      "user_id": 515,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:44:15.393Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 519,
      "feedbackable_id": 98,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:44:15.684Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 523,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:44:15.978Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 45,
      "user_id": 527,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:44:16.278Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 46,
      "user_id": 531,
      "feedbackable_id": 101,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T18:44:16.584Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8e30c2279a4e76b4df3e6819a12e2da527e3015430eefe1e71aafc2c88203bc"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer d1d134bb2d4e68bc515b0585d2e0f2b6e9fc3cdef9cc4e3b5823e2acf912da3a
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
      "id": 32,
      "user_id": 473,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T18:44:12.278Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1d134bb2d4e68bc515b0585d2e0f2b6e9fc3cdef9cc4e3b5823e2acf912da3a"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/4
Authorization: Bearer 5ec070b1a738526b32c7ee8c58a33f1414429637c586b6bccb05237c054ecd3f
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
curl "api.goskive.com/v2/files/4" -d '' -X DELETE \
	-H "Authorization: Bearer 5ec070b1a738526b32c7ee8c58a33f1414429637c586b6bccb05237c054ecd3f" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/8/feedbacks
Content-Type: application/json
Authorization: Bearer d5a28fe9ccfdc0655b24d53d51ddf2da258c99977d547c25f25a71a31f11f607
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
      "id": 9,
      "user_id": 77,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:31.415Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 76,
      "feedbackable_id": 8,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:31.402Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/8/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5a28fe9ccfdc0655b24d53d51ddf2da258c99977d547c25f25a71a31f11f607"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer b032d1e0eb14a72cab379b388ada194d03690043c9ee3fb1835271d7654a8764
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
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 641,
      "chapter_id": 139,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:24.500Z",
      "created_at": "2016-10-14T18:44:24.500Z",
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
      "author_id": 644,
      "chapter_id": 140,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:24.635Z",
      "created_at": "2016-10-14T18:44:24.635Z",
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
      "author_id": 647,
      "chapter_id": 141,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:24.772Z",
      "created_at": "2016-10-14T18:44:24.772Z",
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
      "author_id": 650,
      "chapter_id": 142,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:24.906Z",
      "created_at": "2016-10-14T18:44:24.906Z",
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
      "id": 81,
      "obfuscated_id": "jHF1owx40fU",
      "author_id": 653,
      "chapter_id": 143,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:25.041Z",
      "created_at": "2016-10-14T18:44:25.041Z",
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
	-H "Authorization: Bearer b032d1e0eb14a72cab379b388ada194d03690043c9ee3fb1835271d7654a8764"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 87d56d1d22581f5395aceca1152460dfa3ad0f9e2af7dfed2406cb9a55278b36
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
      "id": 71,
      "obfuscated_id": "--JhLc6KEBw",
      "author_id": 621,
      "chapter_id": 133,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:44:23.560Z",
      "created_at": "2016-10-14T18:44:23.560Z",
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
	-H "Authorization: Bearer 87d56d1d22581f5395aceca1152460dfa3ad0f9e2af7dfed2406cb9a55278b36"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/60/republish
Content-Type: application/json
Authorization: Bearer 1cf713c81a118bd2f324987ccdcd182d2f5db49ef0cb5ccd48eec3de6d3e2d12
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/60/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1cf713c81a118bd2f324987ccdcd182d2f5db49ef0cb5ccd48eec3de6d3e2d12"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/65/feedbacks
Content-Type: application/json
Authorization: Bearer 5d1a31271e36a885d1b74d54d51c15994a9775b99a16e769ee4b29e2182bea23
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
      "user_id": 287,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:55.461Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 286,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T18:43:55.450Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/65/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d1a31271e36a885d1b74d54d51c15994a9775b99a16e769ee4b29e2182bea23"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 929c17aaf10cd194b2c327c7d8f834bc05457bea9632257de8a5f9f49eba487f
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 137,
      "chapter_id": 35,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:37.537Z",
      "created_at": "2016-10-14T18:43:37.406Z",
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
          "id": 53,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 54,
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
      "author_id": 128,
      "chapter_id": 32,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:36.674Z",
      "created_at": "2016-10-14T18:43:36.549Z",
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
      "author_id": 131,
      "chapter_id": 33,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:36.957Z",
      "created_at": "2016-10-14T18:43:36.831Z",
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
      "author_id": 134,
      "chapter_id": 34,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:37.240Z",
      "created_at": "2016-10-14T18:43:37.113Z",
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
    },
    {
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 140,
      "chapter_id": 36,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:37.817Z",
      "created_at": "2016-10-14T18:43:37.697Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 929c17aaf10cd194b2c327c7d8f834bc05457bea9632257de8a5f9f49eba487f"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 602f3fcf53f53ca60d4d5b5debae25ff20e72281c6f002bd3c40be836a1c8b2b
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 108,
      "chapter_id": 26,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T18:43:34.849Z",
      "created_at": "2016-10-14T18:43:34.733Z",
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
          "id": 35,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 36,
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
	-H "Authorization: Bearer 602f3fcf53f53ca60d4d5b5debae25ff20e72281c6f002bd3c40be836a1c8b2b"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/10/republish
Content-Type: application/json
Authorization: Bearer 405df84ebb78e49707e6b44099789f730ada07f4c834b374edda75977a798678
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 405df84ebb78e49707e6b44099789f730ada07f4c834b374edda75977a798678"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 748ad2a77ce9062b06eefaf8db0c0e8ed57e8ae12ec867cf0ce5496d7b7149f7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":156,"published":false}}
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
    "creator_id": 537,
    "id": 144,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 150,
    "additional_university_ids": [

    ],
    "topic_id": 156,
    "discipline_id": 157,
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
    "updated_at": "2016-10-14T18:44:17.197Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":156,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 748ad2a77ce9062b06eefaf8db0c0e8ed57e8ae12ec867cf0ce5496d7b7149f7"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer efd5ca1d184d6e9400cbb8dcd48d160040145481ecbb5ac09743f59075f9341f
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
      "creator_id": 569,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-141",
      "html_url": "https://goskive.com/course/fu-course-141",
      "slug": "fu-course-141",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 185,
      "discipline_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 141",
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
      "updated_at": "2016-10-14T18:44:20.164Z",
      "shortname": "fu-course-141"
    },
    {
      "creator_id": 569,
      "id": 174,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-142",
      "html_url": "https://goskive.com/course/fu-course-142",
      "slug": "fu-course-142",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 186,
      "discipline_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 142",
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
      "updated_at": "2016-10-14T18:44:20.206Z",
      "shortname": "fu-course-142"
    },
    {
      "creator_id": 570,
      "id": 175,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-143",
      "html_url": "https://goskive.com/course/fu-course-143",
      "slug": "fu-course-143",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 187,
      "discipline_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 143",
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
      "updated_at": "2016-10-14T18:44:20.255Z",
      "shortname": "fu-course-143"
    },
    {
      "creator_id": 570,
      "id": 176,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-144",
      "html_url": "https://goskive.com/course/fu-course-144",
      "slug": "fu-course-144",
      "university_id": 162,
      "additional_university_ids": [

      ],
      "topic_id": 188,
      "discipline_id": 189,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 144",
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
      "chapters_updated_at": "2016-10-14T18:44:20.551Z",
      "updated_at": "2016-10-14T18:44:20.558Z",
      "shortname": "fu-course-144"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer efd5ca1d184d6e9400cbb8dcd48d160040145481ecbb5ac09743f59075f9341f"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d7ff752c65a5ac93265a5105570db32e0d397b7acc4535ec385cb0fc8d34d11e
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
      "creator_id": 576,
      "id": 177,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 189,
      "discipline_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
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
      "updated_at": "2016-10-14T18:44:20.766Z",
      "shortname": "fu-course-145"
    },
    {
      "creator_id": 576,
      "id": 178,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 190,
      "discipline_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
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
      "updated_at": "2016-10-14T18:44:20.833Z",
      "shortname": "fu-course-146"
    },
    {
      "creator_id": 577,
      "id": 179,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 191,
      "discipline_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
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
      "updated_at": "2016-10-14T18:44:20.882Z",
      "shortname": "fu-course-147"
    },
    {
      "creator_id": 577,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 164,
      "additional_university_ids": [

      ],
      "topic_id": 192,
      "discipline_id": 193,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
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
      "updated_at": "2016-10-14T18:44:20.923Z",
      "shortname": "fu-course-148"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7ff752c65a5ac93265a5105570db32e0d397b7acc4535ec385cb0fc8d34d11e"
```
