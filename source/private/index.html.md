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
DELETE /v2/chapters/153
Content-Type: application/json
Authorization: Bearer 2b75cbd244672fd8718f939f95c2285ba5b6dc519e681d6bb833e8ece0ab7b0e
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/153" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b75cbd244672fd8718f939f95c2285ba5b6dc519e681d6bb833e8ece0ab7b0e"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/157
Content-Type: application/json
Authorization: Bearer 156ea347a90185ca716805eaee57e6e6b1aff8f860a38956b5595d73abbeee38
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
    "id": 157,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T11:36:16.366Z",
    "course_id": 271,
    "author_id": 819,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-14T11:36:15.808Z",
    "questions_updated_at": "2016-10-14T11:36:15.808Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 822,
        "chapter_id": 157,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:16.306Z",
        "created_at": "2016-10-14T11:36:16.306Z",
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
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 823,
        "chapter_id": 157,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:16.347Z",
        "created_at": "2016-10-14T11:36:16.347Z",
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
        "id": 115,
        "obfuscated_id": "tgK0VZO8yq4",
        "author_id": 820,
        "chapter_id": 157,
        "position": 102,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:16.034Z",
        "created_at": "2016-10-14T11:36:15.920Z",
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
        "author_id": 821,
        "chapter_id": 157,
        "position": 103,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:36:16.233Z",
        "created_at": "2016-10-14T11:36:16.109Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/157" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 156ea347a90185ca716805eaee57e6e6b1aff8f860a38956b5595d73abbeee38"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/152
Content-Type: application/json
Authorization: Bearer 454432d3e4ead44f5df9232f36429185ec7b193eb9624fb5cb2ef43e6df1abac
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
    "id": 152,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T11:36:14.812Z",
    "course_id": 266,
    "author_id": 804,
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
curl "api.goskive.com/v2/chapters/152" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 454432d3e4ead44f5df9232f36429185ec7b193eb9624fb5cb2ef43e6df1abac"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/46
Content-Type: application/json
Authorization: Bearer 46718410fbeaf704f649386b88273074ab221fe5b632e6f982d8b5903c23fa00
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/46" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 46718410fbeaf704f649386b88273074ab221fe5b632e6f982d8b5903c23fa00"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 37c6a3eff570484610782a1214cabdb780e8c6d28b23d1ac9f42c1b357dbab57
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
      "id": 18,
      "author_id": 400,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:42.413Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 402,
      "reply_to_id": 18,
      "created_at": "2016-10-14T11:35:42.499Z",
      "status": "published",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 404,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:42.583Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 406,
      "reply_to_id": 20,
      "created_at": "2016-10-14T11:35:42.666Z",
      "status": "published",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 408,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:42.753Z",
      "status": "reported",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 410,
      "reply_to_id": 22,
      "created_at": "2016-10-14T11:35:42.837Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 412,
      "reply_to_id": 22,
      "created_at": "2016-10-14T11:35:42.924Z",
      "status": "published",
      "subject_id": 154,
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
	-H "Authorization: Bearer 37c6a3eff570484610782a1214cabdb780e8c6d28b23d1ac9f42c1b357dbab57"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 8cb94956035fd9ff8084140ad004a29424ee480d966a5049f9a0f642dbb261ca
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
      "id": 39,
      "author_id": 445,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:44.394Z",
      "status": "published",
      "subject_id": 169,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 447,
      "reply_to_id": 39,
      "created_at": "2016-10-14T11:35:44.481Z",
      "status": "published",
      "subject_id": 170,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 449,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:44.569Z",
      "status": "published",
      "subject_id": 171,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 451,
      "reply_to_id": 41,
      "created_at": "2016-10-14T11:35:44.655Z",
      "status": "published",
      "subject_id": 172,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 453,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:44.741Z",
      "status": "reported",
      "subject_id": 173,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 455,
      "reply_to_id": 43,
      "created_at": "2016-10-14T11:35:44.825Z",
      "status": "published",
      "subject_id": 174,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 457,
      "reply_to_id": 43,
      "created_at": "2016-10-14T11:35:44.911Z",
      "status": "published",
      "subject_id": 175,
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
	-H "Authorization: Bearer 8cb94956035fd9ff8084140ad004a29424ee480d966a5049f9a0f642dbb261ca"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 411f0a2ca3720b39e25d5e802fa207dd7e01067ac6349265e55bf671833c369a
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
      "id": 26,
      "author_id": 417,
      "reply_to_id": 25,
      "created_at": "2016-10-14T11:35:43.150Z",
      "status": "published",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 421,
      "reply_to_id": 27,
      "created_at": "2016-10-14T11:35:43.319Z",
      "status": "published",
      "subject_id": 158,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 425,
      "reply_to_id": 29,
      "created_at": "2016-10-14T11:35:43.491Z",
      "status": "published",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 427,
      "reply_to_id": 29,
      "created_at": "2016-10-14T11:35:43.579Z",
      "status": "published",
      "subject_id": 161,
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
	-H "Authorization: Bearer 411f0a2ca3720b39e25d5e802fa207dd7e01067ac6349265e55bf671833c369a"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 0c5730913451438873c6d283b6217184c1c44f05d5ef8b8cc1cbc7fc6df38169
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
      "id": 36,
      "author_id": 438,
      "reply_to_id": null,
      "created_at": "2016-10-14T11:35:44.065Z",
      "status": "reported",
      "subject_id": 166,
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
	-H "Authorization: Bearer 0c5730913451438873c6d283b6217184c1c44f05d5ef8b8cc1cbc7fc6df38169"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/50/republish
Content-Type: application/json
Authorization: Bearer c8203e1aee930ff0f874d96649bb5964742f798585a3935014ff77aa8ed8ce43
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/50/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c8203e1aee930ff0f874d96649bb5964742f798585a3935014ff77aa8ed8ce43"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 93c5156bee7e6cdb8ee54dc5c36fb12c301d338bbfbb75bd73ebc137dd6bb812
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
    "id": 170,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T11:36:22.557Z",
    "course_id": 291,
    "author_id": 902,
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
	-H "Authorization: Bearer 93c5156bee7e6cdb8ee54dc5c36fb12c301d338bbfbb75bd73ebc137dd6bb812"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/293/chapters
Content-Type: application/json
Authorization: Bearer 1c595c0426086d620d8cc9fa8ffaca1a90f05e6dfd0331c3425296844db65c5f
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
    "updated_at": "2016-10-14T11:36:22.807Z",
    "course_id": 293,
    "author_id": 906,
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
curl "api.goskive.com/v2/courses/293/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c595c0426086d620d8cc9fa8ffaca1a90f05e6dfd0331c3425296844db65c5f"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 52b978451c8ccd53dfc2fa4dcf4aba3c99dc5b7605bc9411f0881cd4affb0eb0
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
      "title": "Clever Chapter Title 151",
      "position": 1,
      "updated_at": "2016-10-14T11:36:23.253Z",
      "course_id": 296,
      "author_id": 915,
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
      "id": 176,
      "title": "Clever Chapter Title 152",
      "position": 2,
      "updated_at": "2016-10-14T11:36:23.279Z",
      "course_id": 296,
      "author_id": 916,
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
      "id": 177,
      "title": "Clever Chapter Title 153",
      "position": 3,
      "updated_at": "2016-10-14T11:36:23.545Z",
      "course_id": 296,
      "author_id": 917,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-14T11:36:23.173Z",
      "questions_updated_at": "2016-10-14T11:36:23.173Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52b978451c8ccd53dfc2fa4dcf4aba3c99dc5b7605bc9411f0881cd4affb0eb0"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 86503a4b89a591454aa8ce0b2cf595885d55f325c390bb91f343a1b132b6f132
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
      "title": "Clever Chapter Title 154",
      "position": 1,
      "updated_at": "2016-10-14T11:36:23.698Z",
      "course_id": 297,
      "author_id": 922,
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
      "position": 2,
      "updated_at": "2016-10-14T11:36:23.724Z",
      "course_id": 297,
      "author_id": 923,
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
      "id": 180,
      "title": "Clever Chapter Title 156",
      "position": 3,
      "updated_at": "2016-10-14T11:36:23.750Z",
      "course_id": 297,
      "author_id": 924,
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
	-H "Authorization: Bearer 86503a4b89a591454aa8ce0b2cf595885d55f325c390bb91f343a1b132b6f132"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7432f3488f9eec3c7a0acf3756825e946fdf93b4295ceb050e0cdd4eb320da12
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
	-H "Authorization: Bearer 7432f3488f9eec3c7a0acf3756825e946fdf93b4295ceb050e0cdd4eb320da12"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/34
Content-Type: application/json
Authorization: Bearer 025badd187a0c522dbb6a80bc29d17441ffb4cc29a5e16bd3623850b2b759d68
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/34" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 025badd187a0c522dbb6a80bc29d17441ffb4cc29a5e16bd3623850b2b759d68"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer fd1f420177d30721ec61a51900b246c5a97352830c92fb84b184acd18f23594f
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
    "creator_id": 127,
    "id": 37,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 38,
    "additional_university_ids": [

    ],
    "topic_id": 47,
    "discipline_id": 47,
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
    "chapters_updated_at": "2016-10-14T11:35:19.457Z",
    "updated_at": "2016-10-14T11:35:21.098Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 24,
        "title": "Clever Chapter Title 24",
        "position": 1,
        "updated_at": "2016-10-14T11:35:21.045Z",
        "course_id": 37,
        "author_id": 127,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T11:35:19.457Z",
        "questions_updated_at": "2016-10-14T11:35:19.457Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 25,
        "title": "Clever Chapter Title 25",
        "position": 2,
        "updated_at": "2016-10-14T11:35:21.089Z",
        "course_id": 37,
        "author_id": 127,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T11:35:19.457Z",
        "questions_updated_at": "2016-10-14T11:35:19.457Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 127,
        "chapter_id": 24,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:20.867Z",
        "created_at": "2016-10-14T11:35:20.867Z",
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
        "author_id": 127,
        "chapter_id": 25,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:20.945Z",
        "created_at": "2016-10-14T11:35:20.945Z",
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
        "author_id": 127,
        "chapter_id": 24,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:20.911Z",
        "created_at": "2016-10-14T11:35:20.911Z",
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
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 127,
        "chapter_id": 25,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:20.990Z",
        "created_at": "2016-10-14T11:35:20.990Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 130,
        "chapter_id": 24,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:21.033Z",
        "created_at": "2016-10-14T11:35:21.033Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 131,
        "chapter_id": 25,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T11:35:21.078Z",
        "created_at": "2016-10-14T11:35:21.078Z",
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
	-H "Authorization: Bearer fd1f420177d30721ec61a51900b246c5a97352830c92fb84b184acd18f23594f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/25
Content-Type: application/json
Authorization: Bearer 70b520ff366303795d64a8bd4c95eaea5c64762005c9720ce3610b418ac85c99
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
    "creator_id": 94,
    "id": 25,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 26,
    "additional_university_ids": [

    ],
    "topic_id": 35,
    "discipline_id": 35,
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
    "updated_at": "2016-10-14T11:35:14.325Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/25" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70b520ff366303795d64a8bd4c95eaea5c64762005c9720ce3610b418ac85c99"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer e85667ce35368d5d096f89d99358ef42f31242b18d0a3abea920db91b3976b8c
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
    "creator_id": 89,
    "id": 22,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 23,
    "additional_university_ids": [

    ],
    "topic_id": 32,
    "discipline_id": 32,
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
    "updated_at": "2016-10-14T11:35:13.914Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e85667ce35368d5d096f89d99358ef42f31242b18d0a3abea920db91b3976b8c"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer c731e66e03a981d0dbb8ccdbb5723110d9da005310dfc490025691684bb2a878
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
      "id": 23,
      "user_id": 532,
      "feedbackable_id": 57,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:49.823Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 536,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:50.130Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 540,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:50.449Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 544,
      "feedbackable_id": 60,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:50.757Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 548,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T11:35:51.065Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c731e66e03a981d0dbb8ccdbb5723110d9da005310dfc490025691684bb2a878"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer a91deb314f3566de2f11aef13fb9f86c3a13b726c4da3feaef146def16db5f46
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
      "user_id": 569,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T11:35:52.723Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a91deb314f3566de2f11aef13fb9f86c3a13b726c4da3feaef146def16db5f46"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/10
Authorization: Bearer 0d2b8dc633e4978f8c0b1ae7265bb2de92ef1f6fec5a9614d039d4f98734e1c7
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
curl "api.goskive.com/v2/files/10" -d '' -X DELETE \
	-H "Authorization: Bearer 0d2b8dc633e4978f8c0b1ae7265bb2de92ef1f6fec5a9614d039d4f98734e1c7" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/4/feedbacks
Content-Type: application/json
Authorization: Bearer 9f47dee81cd0a5741d11503a294772ceaff087329676c01da0b5b00e9e2c3b8f
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
      "user_id": 69,
      "feedbackable_id": 4,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:11.731Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 68,
      "feedbackable_id": 4,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:35:11.718Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/4/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f47dee81cd0a5741d11503a294772ceaff087329676c01da0b5b00e9e2c3b8f"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer b57048b795652255767fcab5ea92de43fc496e9b2b1e64f95300fb89d05db43a
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 318,
      "chapter_id": 62,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:37.655Z",
      "created_at": "2016-10-14T11:35:37.655Z",
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 321,
      "chapter_id": 63,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:37.795Z",
      "created_at": "2016-10-14T11:35:37.795Z",
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
      "author_id": 324,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:37.930Z",
      "created_at": "2016-10-14T11:35:37.930Z",
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
      "author_id": 327,
      "chapter_id": 65,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:38.066Z",
      "created_at": "2016-10-14T11:35:38.066Z",
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
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 330,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:38.200Z",
      "created_at": "2016-10-14T11:35:38.200Z",
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
	-H "Authorization: Bearer b57048b795652255767fcab5ea92de43fc496e9b2b1e64f95300fb89d05db43a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer e19bbae90ab6704949d43f41eb05c8a149a5b2a0b2fa4765443e994d77b33a86
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
      "id": 67,
      "obfuscated_id": "btMCNJVyvlA",
      "author_id": 346,
      "chapter_id": 71,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:35:38.956Z",
      "created_at": "2016-10-14T11:35:38.956Z",
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
	-H "Authorization: Bearer e19bbae90ab6704949d43f41eb05c8a149a5b2a0b2fa4765443e994d77b33a86"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/52/republish
Content-Type: application/json
Authorization: Bearer 2dad8d336302c8725bada0918911b5afb892eb4653078f36ec904c1df88cafb5
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/52/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2dad8d336302c8725bada0918911b5afb892eb4653078f36ec904c1df88cafb5"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/125/feedbacks
Content-Type: application/json
Authorization: Bearer 1aa601472b57081f19425e01ad2e56ccf8feba56a51ace35d02320247ebb67df
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
      "user_id": 867,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:36:20.306Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 866,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T11:36:20.295Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/125/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1aa601472b57081f19425e01ad2e56ccf8feba56a51ace35d02320247ebb67df"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 1d2ee1889496ab44fbfff6796a9ab876d45a4d4b9a5a60823f092c4d6879ee96
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 723,
      "chapter_id": 126,
      "position": 84,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:06.035Z",
      "created_at": "2016-10-14T11:36:05.915Z",
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
          "id": 180,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 181,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 726,
      "chapter_id": 127,
      "position": 85,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:06.325Z",
      "created_at": "2016-10-14T11:36:06.204Z",
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
          "id": 182,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 183,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 729,
      "chapter_id": 128,
      "position": 86,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:06.618Z",
      "created_at": "2016-10-14T11:36:06.496Z",
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
          "id": 184,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 185,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 92,
      "obfuscated_id": "__OphzZQiQY",
      "author_id": 732,
      "chapter_id": 129,
      "position": 87,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:06.912Z",
      "created_at": "2016-10-14T11:36:06.791Z",
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
          "id": 186,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 187,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 735,
      "chapter_id": 130,
      "position": 88,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:07.265Z",
      "created_at": "2016-10-14T11:36:07.085Z",
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
          "id": 188,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 189,
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
	-H "Authorization: Bearer 1d2ee1889496ab44fbfff6796a9ab876d45a4d4b9a5a60823f092c4d6879ee96"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer ca810743c3b3e9631bd7341d31c524bb5ceb497f6e8ff6757ff930364ddae779
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
      "id": 103,
      "obfuscated_id": "AVhVflMAvL0",
      "author_id": 767,
      "chapter_id": 140,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T11:36:10.429Z",
      "created_at": "2016-10-14T11:36:10.315Z",
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
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca810743c3b3e9631bd7341d31c524bb5ceb497f6e8ff6757ff930364ddae779"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/105/republish
Content-Type: application/json
Authorization: Bearer ecda9b6daed19ffda25fec4a4ac7a1691e3d797112469dda2a28a8cb8df70ec6
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/105/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecda9b6daed19ffda25fec4a4ac7a1691e3d797112469dda2a28a8cb8df70ec6"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 809b8c0be41ee686fa39aa43dc18521847620338737726e951071ec1cc4bb5eb
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":97,"published":false}}
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
    "creator_id": 216,
    "id": 87,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 66,
    "additional_university_ids": [

    ],
    "topic_id": 97,
    "discipline_id": 97,
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
    "updated_at": "2016-10-14T11:35:29.113Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":97,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 809b8c0be41ee686fa39aa43dc18521847620338737726e951071ec1cc4bb5eb"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ebe648d7c74a381c9a0f24a04bbeb7dc66146e2fd81b7b6052842f3851138256
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
      "creator_id": 195,
      "id": 70,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-51",
      "html_url": "https://goskive.com/course/fu-course-51",
      "slug": "fu-course-51",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 80,
      "discipline_id": 80,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 51",
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
      "updated_at": "2016-10-14T11:35:27.118Z",
      "shortname": "fu-course-51"
    },
    {
      "creator_id": 195,
      "id": 71,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-52",
      "html_url": "https://goskive.com/course/fu-course-52",
      "slug": "fu-course-52",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 81,
      "discipline_id": 81,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 52",
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
      "updated_at": "2016-10-14T11:35:27.162Z",
      "shortname": "fu-course-52"
    },
    {
      "creator_id": 196,
      "id": 72,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-53",
      "html_url": "https://goskive.com/course/fu-course-53",
      "slug": "fu-course-53",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 82,
      "discipline_id": 82,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 53",
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
      "updated_at": "2016-10-14T11:35:27.214Z",
      "shortname": "fu-course-53"
    },
    {
      "creator_id": 196,
      "id": 73,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-54",
      "html_url": "https://goskive.com/course/fu-course-54",
      "slug": "fu-course-54",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 83,
      "discipline_id": 83,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 54",
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
      "chapters_updated_at": "2016-10-14T11:35:27.513Z",
      "updated_at": "2016-10-14T11:35:27.519Z",
      "shortname": "fu-course-54"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ebe648d7c74a381c9a0f24a04bbeb7dc66146e2fd81b7b6052842f3851138256"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e622295dc9cf34f329a989df84c1e05cf7588c5f1820ff263b50597e03f8fc3d
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
      "creator_id": 201,
      "id": 74,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-55",
      "html_url": "https://goskive.com/course/fu-course-55",
      "slug": "fu-course-55",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 84,
      "discipline_id": 84,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 55",
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
      "updated_at": "2016-10-14T11:35:27.671Z",
      "shortname": "fu-course-55"
    },
    {
      "creator_id": 201,
      "id": 75,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-56",
      "html_url": "https://goskive.com/course/fu-course-56",
      "slug": "fu-course-56",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 85,
      "discipline_id": 85,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
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
      "updated_at": "2016-10-14T11:35:27.714Z",
      "shortname": "fu-course-56"
    },
    {
      "creator_id": 202,
      "id": 76,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 86,
      "discipline_id": 86,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
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
      "updated_at": "2016-10-14T11:35:27.766Z",
      "shortname": "fu-course-57"
    },
    {
      "creator_id": 202,
      "id": 77,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 60,
      "additional_university_ids": [

      ],
      "topic_id": 87,
      "discipline_id": 87,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
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
      "updated_at": "2016-10-14T11:35:27.810Z",
      "shortname": "fu-course-58"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e622295dc9cf34f329a989df84c1e05cf7588c5f1820ff263b50597e03f8fc3d"
```
