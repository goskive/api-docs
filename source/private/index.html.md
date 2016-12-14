---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Chapters

## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/142
Content-Type: application/json
Authorization: Bearer 007d2d72aef05b31cc95c553f525f435477fd4ba5dedf382d6639c3ba6dce013
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/142" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 007d2d72aef05b31cc95c553f525f435477fd4ba5dedf382d6639c3ba6dce013"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/140
Content-Type: application/json
Authorization: Bearer 1f4efdbcd7860a171ceedad345f39672eb430ea293d56ea86db4fbf7f2e6d26a
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
    "id": 140,
    "updated_at": "2016-12-14T16:47:42.779Z",
    "course_id": 201,
    "author_id": 624,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-14T16:47:42.192Z",
    "questions_updated_at": "2016-12-14T16:47:42.192Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 627,
        "chapter_id": 140,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:42.714Z",
        "created_at": "2016-12-14T16:47:42.714Z",
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
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 628,
        "chapter_id": 140,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:42.757Z",
        "created_at": "2016-12-14T16:47:42.757Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 625,
        "chapter_id": 140,
        "position": 68,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:42.435Z",
        "created_at": "2016-12-14T16:47:42.333Z",
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
            "id": 165,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 166,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 626,
        "chapter_id": 140,
        "position": 69,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:42.639Z",
        "created_at": "2016-12-14T16:47:42.526Z",
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
            "id": 167,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 168,
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
curl "api.goskive.com/v2/chapters/140" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1f4efdbcd7860a171ceedad345f39672eb430ea293d56ea86db4fbf7f2e6d26a"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/145
Content-Type: application/json
Authorization: Bearer b2f9cc66d5d2cba6030db38681de9f7f02332618cacd42a5a32f0b00a97f91ab
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
    "id": 145,
    "updated_at": "2016-12-14T16:47:43.986Z",
    "course_id": 206,
    "author_id": 643,
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
curl "api.goskive.com/v2/chapters/145" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b2f9cc66d5d2cba6030db38681de9f7f02332618cacd42a5a32f0b00a97f91ab"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/53
Content-Type: application/json
Authorization: Bearer 350c28acd971d88c9bf6397c7b407f36dcdfcd5483be9ea9fed480988d73e07a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/53" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 350c28acd971d88c9bf6397c7b407f36dcdfcd5483be9ea9fed480988d73e07a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 9b6ce7765f3b8ad7b06692c5e4d523598f7cfb17f5bb1ebf942b0c267a41a18e
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
      "id": 17,
      "author_id": 854,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:04.100Z",
      "status": "published",
      "subject_id": 265,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 856,
      "reply_to_id": 17,
      "created_at": "2016-12-14T16:48:04.204Z",
      "status": "published",
      "subject_id": 266,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 858,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:04.308Z",
      "status": "published",
      "subject_id": 267,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 860,
      "reply_to_id": 19,
      "created_at": "2016-12-14T16:48:04.414Z",
      "status": "published",
      "subject_id": 268,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 862,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:04.525Z",
      "status": "reported",
      "subject_id": 269,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 864,
      "reply_to_id": 21,
      "created_at": "2016-12-14T16:48:04.667Z",
      "status": "published",
      "subject_id": 270,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 866,
      "reply_to_id": 21,
      "created_at": "2016-12-14T16:48:04.785Z",
      "status": "published",
      "subject_id": 271,
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
	-H "Authorization: Bearer 9b6ce7765f3b8ad7b06692c5e4d523598f7cfb17f5bb1ebf942b0c267a41a18e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 14b9c22cff48117639d2848fc0bb036129a28b4e4579169574bf9e557c5ce2f7
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
      "id": 31,
      "author_id": 884,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:05.767Z",
      "status": "published",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 886,
      "reply_to_id": 31,
      "created_at": "2016-12-14T16:48:05.877Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 888,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:05.993Z",
      "status": "published",
      "subject_id": 281,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 890,
      "reply_to_id": 33,
      "created_at": "2016-12-14T16:48:06.116Z",
      "status": "published",
      "subject_id": 282,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 892,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:06.238Z",
      "status": "reported",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 894,
      "reply_to_id": 35,
      "created_at": "2016-12-14T16:48:06.363Z",
      "status": "published",
      "subject_id": 284,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 896,
      "reply_to_id": 35,
      "created_at": "2016-12-14T16:48:06.483Z",
      "status": "published",
      "subject_id": 285,
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
	-H "Authorization: Bearer 14b9c22cff48117639d2848fc0bb036129a28b4e4579169574bf9e557c5ce2f7"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 25c99949b754741f879a5012be22edbd0f43ebc85be0465d33861cf0484f5134
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
      "id": 46,
      "author_id": 916,
      "reply_to_id": 45,
      "created_at": "2016-12-14T16:48:07.648Z",
      "status": "published",
      "subject_id": 294,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 920,
      "reply_to_id": 47,
      "created_at": "2016-12-14T16:48:07.861Z",
      "status": "published",
      "subject_id": 296,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 924,
      "reply_to_id": 49,
      "created_at": "2016-12-14T16:48:08.078Z",
      "status": "published",
      "subject_id": 298,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 926,
      "reply_to_id": 49,
      "created_at": "2016-12-14T16:48:08.181Z",
      "status": "published",
      "subject_id": 299,
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
	-H "Authorization: Bearer 25c99949b754741f879a5012be22edbd0f43ebc85be0465d33861cf0484f5134"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 6692617e46a4075fb81108de64f72ae7462e2d38c81667765e07b6b0eb97b04f
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
      "id": 28,
      "author_id": 877,
      "reply_to_id": null,
      "created_at": "2016-12-14T16:48:05.382Z",
      "status": "reported",
      "subject_id": 276,
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
	-H "Authorization: Bearer 6692617e46a4075fb81108de64f72ae7462e2d38c81667765e07b6b0eb97b04f"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/56/republish
Content-Type: application/json
Authorization: Bearer cbdc91b021b8debd5530be5e175566ab87b74d3720a69d29c55e3c5c64c378e3
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/56/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cbdc91b021b8debd5530be5e175566ab87b74d3720a69d29c55e3c5c64c378e3"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6423e95ec268ff87fe7631122fdfb835da89f884645ae575ab2d52ba903c1634
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
    "id": 55,
    "updated_at": "2016-12-14T16:47:06.562Z",
    "course_id": 56,
    "author_id": 190,
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
	-H "Authorization: Bearer 6423e95ec268ff87fe7631122fdfb835da89f884645ae575ab2d52ba903c1634"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/59/chapters
Content-Type: application/json
Authorization: Bearer c5863f833ba96bd59b340aed9272d96c701ec461a8af2d8b177f446a984b894b
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
    "id": 57,
    "updated_at": "2016-12-14T16:47:07.038Z",
    "course_id": 59,
    "author_id": 196,
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
curl "api.goskive.com/v2/courses/59/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c5863f833ba96bd59b340aed9272d96c701ec461a8af2d8b177f446a984b894b"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a1a8981b83c1383c00ffb5ccbac29463e0b6933313f5777ed088a876527f0a10
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
      "id": 46,
      "updated_at": "2016-12-14T16:47:05.264Z",
      "course_id": 51,
      "author_id": 169,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 46",
      "position": 1
    },
    {
      "id": 47,
      "updated_at": "2016-12-14T16:47:05.290Z",
      "course_id": 51,
      "author_id": 170,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 47",
      "position": 2
    },
    {
      "id": 48,
      "updated_at": "2016-12-14T16:47:05.520Z",
      "course_id": 51,
      "author_id": 171,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-14T16:47:05.162Z",
      "questions_updated_at": "2016-12-14T16:47:05.162Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 48",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1a8981b83c1383c00ffb5ccbac29463e0b6933313f5777ed088a876527f0a10"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d8a6e0a2dbe8be258ce1e1af1000812ea86f251a6a24c1d280b131eeb24d0ca5
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
      "id": 49,
      "updated_at": "2016-12-14T16:47:05.831Z",
      "course_id": 53,
      "author_id": 178,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 49",
      "position": 1
    },
    {
      "id": 50,
      "updated_at": "2016-12-14T16:47:05.858Z",
      "course_id": 53,
      "author_id": 179,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 50",
      "position": 2
    },
    {
      "id": 51,
      "updated_at": "2016-12-14T16:47:05.884Z",
      "course_id": 53,
      "author_id": 180,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 51",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8a6e0a2dbe8be258ce1e1af1000812ea86f251a6a24c1d280b131eeb24d0ca5"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cf4a883feb3e172794c488fda6453fbcde71f02913bd4b2c1972c392f361e5bd
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
	-H "Authorization: Bearer cf4a883feb3e172794c488fda6453fbcde71f02913bd4b2c1972c392f361e5bd"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/220
Content-Type: application/json
Authorization: Bearer 16522f6d9614522615a1b402d0a29b85472f82c2aa188409ac9ab3a5e889f5be
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/220" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 16522f6d9614522615a1b402d0a29b85472f82c2aa188409ac9ab3a5e889f5be"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 877da34d90385cccec9da47f0e46ce95b68738bb4a278058eee1e1463ce9391c
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
    "creator_id": 686,
    "id": 226,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 206,
    "additional_university_ids": [

    ],
    "discipline_id": 231,
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
    "chapters_updated_at": "2016-12-14T16:47:47.574Z",
    "updated_at": "2016-12-14T16:47:48.740Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 686,
        "chapter_id": 152,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.534Z",
        "created_at": "2016-12-14T16:47:48.534Z",
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
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 686,
        "chapter_id": 153,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.605Z",
        "created_at": "2016-12-14T16:47:48.605Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 686,
        "chapter_id": 152,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.573Z",
        "created_at": "2016-12-14T16:47:48.573Z",
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
        "id": 62,
        "obfuscated_id": "fj_KMGohXD4",
        "author_id": 686,
        "chapter_id": 153,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.644Z",
        "created_at": "2016-12-14T16:47:48.644Z",
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
        "author_id": 689,
        "chapter_id": 152,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.683Z",
        "created_at": "2016-12-14T16:47:48.683Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 690,
        "chapter_id": 153,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T16:47:48.721Z",
        "created_at": "2016-12-14T16:47:48.721Z",
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
        "id": 152,
        "updated_at": "2016-12-14T16:47:48.692Z",
        "course_id": 226,
        "author_id": 686,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-14T16:47:47.574Z",
        "questions_updated_at": "2016-12-14T16:47:47.574Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 131",
        "position": 1
      },
      {
        "id": 153,
        "updated_at": "2016-12-14T16:47:48.731Z",
        "course_id": 226,
        "author_id": 686,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-14T16:47:47.574Z",
        "questions_updated_at": "2016-12-14T16:47:47.574Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 132",
        "position": 2
      }
    ],
    "topic_id": 230,
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
	-H "Authorization: Bearer 877da34d90385cccec9da47f0e46ce95b68738bb4a278058eee1e1463ce9391c"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/225
Content-Type: application/json
Authorization: Bearer 513cd4123f8c89679b86a68bf6bb0fb26205ce7d4044cc26204100f26c741734
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
    "creator_id": 684,
    "id": 225,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 205,
    "additional_university_ids": [

    ],
    "discipline_id": 230,
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
    "updated_at": "2016-12-14T16:47:47.536Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 229,
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
curl "api.goskive.com/v2/courses/225" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 513cd4123f8c89679b86a68bf6bb0fb26205ce7d4044cc26204100f26c741734"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9aedd37adfff26e36af09cb76a9e00c3454c6dffb8662e063ff7d254c5f6bacc
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
    "creator_id": 681,
    "id": 223,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 203,
    "additional_university_ids": [

    ],
    "discipline_id": 228,
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
    "updated_at": "2016-12-14T16:47:47.162Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 227,
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
	-H "Authorization: Bearer 9aedd37adfff26e36af09cb76a9e00c3454c6dffb8662e063ff7d254c5f6bacc"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 5d0874c1fbc003515d388fc20bf7ebaeddfceb6631980dfcffc49ae8a1dc6a44
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
      "id": 25,
      "user_id": 511,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:33.494Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 515,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:33.799Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 519,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:34.097Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 523,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:47:34.405Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 527,
      "feedbackable_id": 68,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-14T16:47:34.718Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5d0874c1fbc003515d388fc20bf7ebaeddfceb6631980dfcffc49ae8a1dc6a44"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 9b27014f88f85933e094d055528efb6a5c2ba1b5e673b4eca14acd90c1a95031
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
      "id": 34,
      "user_id": 548,
      "feedbackable_id": 73,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-14T16:47:36.331Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b27014f88f85933e094d055528efb6a5c2ba1b5e673b4eca14acd90c1a95031"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 1012ac8ba2d08f7bd76f3665855d8be6b43e2bf5cc69d0dae96bb3796da1b689
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
	-H "Authorization: Bearer 1012ac8ba2d08f7bd76f3665855d8be6b43e2bf5cc69d0dae96bb3796da1b689"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer ca7a4d803e0296b3c2f091de986035d202f5c8724a67833b23380cafe2a378bc
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
    "id": 12,
    "uploader": {
      "id": 366,
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
      "created_at": "2016-12-14T16:47:21.059Z",
      "updated_at": "2016-12-14T16:47:21.059Z"
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
    "created_at": "2016-12-14T16:47:21.157Z",
    "updated_at": "2016-12-14T16:47:21.157Z",
    "course_id": 109,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca7a4d803e0296b3c2f091de986035d202f5c8724a67833b23380cafe2a378bc"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/3/feedbacks
Content-Type: application/json
Authorization: Bearer 60a1d8c9d78cedc32e1e93fbaa29b263a0151b22643c50e05390cba60d7fdc06
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
      "id": 4,
      "user_id": 35,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:46:52.339Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 34,
      "feedbackable_id": 3,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:46:52.328Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/3/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 60a1d8c9d78cedc32e1e93fbaa29b263a0151b22643c50e05390cba60d7fdc06"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 25caae5cd36259047be17ea20618160a6505078dc33ca1e275c29d1687dfcb1a
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 281,
      "chapter_id": 77,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:15.744Z",
      "created_at": "2016-12-14T16:47:15.744Z",
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
      "author_id": 284,
      "chapter_id": 78,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:15.902Z",
      "created_at": "2016-12-14T16:47:15.902Z",
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
      "author_id": 287,
      "chapter_id": 79,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:16.063Z",
      "created_at": "2016-12-14T16:47:16.063Z",
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 290,
      "chapter_id": 80,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:16.228Z",
      "created_at": "2016-12-14T16:47:16.228Z",
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 293,
      "chapter_id": 81,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:16.397Z",
      "created_at": "2016-12-14T16:47:16.397Z",
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
	-H "Authorization: Bearer 25caae5cd36259047be17ea20618160a6505078dc33ca1e275c29d1687dfcb1a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 6cad9c634837b242bd665906b57bfc8eb1de71f3302fcfee7a05956cf2f0feb0
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 277,
      "chapter_id": 76,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:15.545Z",
      "created_at": "2016-12-14T16:47:15.545Z",
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
	-H "Authorization: Bearer 6cad9c634837b242bd665906b57bfc8eb1de71f3302fcfee7a05956cf2f0feb0"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/37/republish
Content-Type: application/json
Authorization: Bearer fb9fa4d0a061d2b650164f9384802124f37e673cc4980e4a6a3bcf43087c5e5a
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/37/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fb9fa4d0a061d2b650164f9384802124f37e673cc4980e4a6a3bcf43087c5e5a"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/125/feedbacks
Content-Type: application/json
Authorization: Bearer 00e50eb0835a0fd67a60c5adc2a7785a1decdf96a99f2a3312e28e5254ce9071
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
      "id": 44,
      "user_id": 806,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:48:00.348Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 805,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T16:48:00.339Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/125/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00e50eb0835a0fd67a60c5adc2a7785a1decdf96a99f2a3312e28e5254ce9071"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 0a79c21465e7924805af71a8cba7fed8307d36eeea00f8fa39a314e1bc69773b
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
      "id": 6,
      "obfuscated_id": "eyxYPTvoIb8",
      "author_id": 71,
      "chapter_id": 14,
      "position": 2,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:46:56.084Z",
      "created_at": "2016-12-14T16:46:56.001Z",
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
          "id": 11,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 12,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 74,
      "chapter_id": 15,
      "position": 3,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:46:56.346Z",
      "created_at": "2016-12-14T16:46:56.264Z",
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
      "id": 8,
      "obfuscated_id": "X2B_8FVuFe8",
      "author_id": 77,
      "chapter_id": 16,
      "position": 4,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:46:56.600Z",
      "created_at": "2016-12-14T16:46:56.519Z",
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
          "id": 15,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 16,
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
      "author_id": 80,
      "chapter_id": 17,
      "position": 5,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:46:56.854Z",
      "created_at": "2016-12-14T16:46:56.770Z",
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
    },
    {
      "id": 10,
      "obfuscated_id": "aY5v9ahzH5c",
      "author_id": 83,
      "chapter_id": 18,
      "position": 6,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:46:57.132Z",
      "created_at": "2016-12-14T16:46:57.030Z",
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
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0a79c21465e7924805af71a8cba7fed8307d36eeea00f8fa39a314e1bc69773b"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c5713aaf7ca047dd870456e687c48883927e81a9ad49e70b8ddb7b2ab967ce28
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 115,
      "chapter_id": 28,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T16:47:00.013Z",
      "created_at": "2016-12-14T16:46:59.934Z",
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
          "id": 39,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 40,
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
	-H "Authorization: Bearer c5713aaf7ca047dd870456e687c48883927e81a9ad49e70b8ddb7b2ab967ce28"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/3/republish
Content-Type: application/json
Authorization: Bearer 451a47ba435296e659a2e1d92e5a0e502271eb0da7f5a7d23b73be5dcc187bac
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/3/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 451a47ba435296e659a2e1d92e5a0e502271eb0da7f5a7d23b73be5dcc187bac"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1293b007ec2edcad06199a65041fc94977778a68098d108ae620ec4220d74f0d
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
    "creator_id": 432,
    "id": 153,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 132,
    "additional_university_ids": [

    ],
    "discipline_id": 153,
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
    "updated_at": "2016-12-14T16:47:27.623Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 153,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":153,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1293b007ec2edcad06199a65041fc94977778a68098d108ae620ec4220d74f0d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ebeba552b294d7bbe1a53262f8489fec3361cb008811c4b4af22d5b1d5721879
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
      "creator_id": 417,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-103",
      "html_url": "https://goskive.com/course/fu-course-103",
      "slug": "fu-course-103",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "discipline_id": 140,
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
      "updated_at": "2016-12-14T16:47:26.168Z",
      "shortname": "fu-course-103",
      "topic_id": 140,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 103",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 417,
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-104",
      "html_url": "https://goskive.com/course/fu-course-104",
      "slug": "fu-course-104",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "discipline_id": 141,
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
      "updated_at": "2016-12-14T16:47:26.204Z",
      "shortname": "fu-course-104",
      "topic_id": 141,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 104",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 418,
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "discipline_id": 142,
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
      "updated_at": "2016-12-14T16:47:26.244Z",
      "shortname": "fu-course-105",
      "topic_id": 142,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 418,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "discipline_id": 143,
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
      "chapters_updated_at": "2016-12-14T16:47:26.087Z",
      "updated_at": "2016-12-14T16:47:26.514Z",
      "shortname": "fu-course-106",
      "topic_id": 143,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebeba552b294d7bbe1a53262f8489fec3361cb008811c4b4af22d5b1d5721879"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3f8102dd72d8e654b8b2d9078b702885a07ba3469e49e843172a6d151b109f77
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
      "creator_id": 424,
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "discipline_id": 144,
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
      "updated_at": "2016-12-14T16:47:26.785Z",
      "shortname": "fu-course-107",
      "topic_id": 144,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 424,
      "id": 145,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "discipline_id": 145,
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
      "updated_at": "2016-12-14T16:47:26.818Z",
      "shortname": "fu-course-108",
      "topic_id": 145,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 425,
      "id": 146,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "discipline_id": 146,
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
      "updated_at": "2016-12-14T16:47:26.860Z",
      "shortname": "fu-course-109",
      "topic_id": 146,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 425,
      "id": 147,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 128,
      "additional_university_ids": [

      ],
      "discipline_id": 147,
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
      "updated_at": "2016-12-14T16:47:26.893Z",
      "shortname": "fu-course-110",
      "topic_id": 147,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3f8102dd72d8e654b8b2d9078b702885a07ba3469e49e843172a6d151b109f77"
```
