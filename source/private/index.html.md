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
DELETE /v2/chapters/145
Content-Type: application/json
Authorization: Bearer 1d05bdb5e5890c1e4528cf55c58f0741d1b2242e0e7d342b0a2538f31540ba9a
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/145" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1d05bdb5e5890c1e4528cf55c58f0741d1b2242e0e7d342b0a2538f31540ba9a"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/146
Content-Type: application/json
Authorization: Bearer baa50ef74e6d09983ea8dd568613d57b949114f055e739e915838b6c2d7c35a0
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
    "id": 146,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-04T16:01:06.704Z",
    "course_id": 267,
    "author_id": 792,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-04T16:01:06.162Z",
    "questions_updated_at": "2016-11-04T16:01:06.162Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 795,
        "chapter_id": 146,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:06.647Z",
        "created_at": "2016-11-04T16:01:06.647Z",
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
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 796,
        "chapter_id": 146,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:06.685Z",
        "created_at": "2016-11-04T16:01:06.685Z",
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
        "id": 96,
        "obfuscated_id": "SEtQvXxfwHo",
        "author_id": 793,
        "chapter_id": 146,
        "position": 92,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:06.383Z",
        "created_at": "2016-11-04T16:01:06.272Z",
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
            "id": 194,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 195,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 97,
        "obfuscated_id": "qdTHUgSdSV8",
        "author_id": 794,
        "chapter_id": 146,
        "position": 93,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:01:06.575Z",
        "created_at": "2016-11-04T16:01:06.455Z",
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
            "id": 196,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 197,
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
curl "api.goskive.com/v2/chapters/146" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer baa50ef74e6d09983ea8dd568613d57b949114f055e739e915838b6c2d7c35a0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/139
Content-Type: application/json
Authorization: Bearer abe2737633b7d13678b9fe24413c23cb13113ffea2a87b0a07dffab6b653ef7c
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
    "id": 139,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-04T16:01:04.891Z",
    "course_id": 260,
    "author_id": 772,
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
curl "api.goskive.com/v2/chapters/139" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer abe2737633b7d13678b9fe24413c23cb13113ffea2a87b0a07dffab6b653ef7c"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer 75d8e1ca440603bead760abb7873381cde3c819b29f49d0a29675933abb36455
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75d8e1ca440603bead760abb7873381cde3c819b29f49d0a29675933abb36455"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer b2da630203445a99b3420eb292739e68359058bf395f7b226d5137276565c454
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
      "id": 19,
      "author_id": 586,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:51.211Z",
      "status": "published",
      "subject_id": 175,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 588,
      "reply_to_id": 19,
      "created_at": "2016-11-04T16:00:51.292Z",
      "status": "published",
      "subject_id": 176,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 590,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:51.374Z",
      "status": "published",
      "subject_id": 177,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 592,
      "reply_to_id": 21,
      "created_at": "2016-11-04T16:00:51.457Z",
      "status": "published",
      "subject_id": 178,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 594,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:51.540Z",
      "status": "reported",
      "subject_id": 179,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 596,
      "reply_to_id": 23,
      "created_at": "2016-11-04T16:00:51.625Z",
      "status": "published",
      "subject_id": 180,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 598,
      "reply_to_id": 23,
      "created_at": "2016-11-04T16:00:51.708Z",
      "status": "published",
      "subject_id": 181,
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
	-H "Authorization: Bearer b2da630203445a99b3420eb292739e68359058bf395f7b226d5137276565c454"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5c865196953da1bdde99877b95711222ab47666d7269a518e58c505e4b662323
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
      "id": 40,
      "author_id": 631,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:53.122Z",
      "status": "published",
      "subject_id": 196,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 633,
      "reply_to_id": 40,
      "created_at": "2016-11-04T16:00:53.209Z",
      "status": "published",
      "subject_id": 197,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 635,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:53.297Z",
      "status": "published",
      "subject_id": 198,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 637,
      "reply_to_id": 42,
      "created_at": "2016-11-04T16:00:53.410Z",
      "status": "published",
      "subject_id": 199,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 639,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:53.495Z",
      "status": "reported",
      "subject_id": 200,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 641,
      "reply_to_id": 44,
      "created_at": "2016-11-04T16:00:53.576Z",
      "status": "published",
      "subject_id": 201,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 643,
      "reply_to_id": 44,
      "created_at": "2016-11-04T16:00:53.658Z",
      "status": "published",
      "subject_id": 202,
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
	-H "Authorization: Bearer 5c865196953da1bdde99877b95711222ab47666d7269a518e58c505e4b662323"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 940b84b5a06f9f6a62eaddc140a8be02b5dd274943e343101bb2e26eb679887b
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
      "id": 34,
      "author_id": 618,
      "reply_to_id": 33,
      "created_at": "2016-11-04T16:00:52.564Z",
      "status": "published",
      "subject_id": 190,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 622,
      "reply_to_id": 35,
      "created_at": "2016-11-04T16:00:52.731Z",
      "status": "published",
      "subject_id": 192,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 626,
      "reply_to_id": 37,
      "created_at": "2016-11-04T16:00:52.901Z",
      "status": "published",
      "subject_id": 194,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 628,
      "reply_to_id": 37,
      "created_at": "2016-11-04T16:00:52.988Z",
      "status": "published",
      "subject_id": 195,
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
	-H "Authorization: Bearer 940b84b5a06f9f6a62eaddc140a8be02b5dd274943e343101bb2e26eb679887b"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 7388335936fd0096d51c12a12aec10de5fe2f8b0802c0f7b40822b4f6f60da94
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
      "id": 16,
      "author_id": 579,
      "reply_to_id": null,
      "created_at": "2016-11-04T16:00:50.887Z",
      "status": "reported",
      "subject_id": 172,
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
	-H "Authorization: Bearer 7388335936fd0096d51c12a12aec10de5fe2f8b0802c0f7b40822b4f6f60da94"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/10/republish
Content-Type: application/json
Authorization: Bearer dcecf217de1b9095172b4fa7fb7dd5a72f380ba05166f898bcdea4f80f0914fe
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/10/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dcecf217de1b9095172b4fa7fb7dd5a72f380ba05166f898bcdea4f80f0914fe"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer af238d0372b9a1bc9e74eb03f20a98a9565eaaf964b5db35d8fe82b71bbd49dc
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
    "id": 23,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-04T16:00:04.961Z",
    "course_id": 14,
    "author_id": 52,
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
	-H "Authorization: Bearer af238d0372b9a1bc9e74eb03f20a98a9565eaaf964b5db35d8fe82b71bbd49dc"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/15/chapters
Content-Type: application/json
Authorization: Bearer c7af01e4737cae2f486b99d7fdb999c904a53f971d773161059a90fccb338b99
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
    "id": 24,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-04T16:00:05.093Z",
    "course_id": 15,
    "author_id": 54,
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
curl "api.goskive.com/v2/courses/15/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c7af01e4737cae2f486b99d7fdb999c904a53f971d773161059a90fccb338b99"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 4f98f232b4497247363c1823d1cb506422b24e95db2dbed010dda64f72b863cf
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
      "id": 1,
      "title": "Clever Chapter Title 1",
      "position": 1,
      "updated_at": "2016-11-04T16:00:02.027Z",
      "course_id": 1,
      "author_id": 2,
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
      "id": 2,
      "title": "Clever Chapter Title 2",
      "position": 2,
      "updated_at": "2016-11-04T16:00:02.057Z",
      "course_id": 1,
      "author_id": 3,
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
      "id": 3,
      "title": "Clever Chapter Title 3",
      "position": 3,
      "updated_at": "2016-11-04T16:00:02.408Z",
      "course_id": 1,
      "author_id": 4,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-04T16:00:01.147Z",
      "questions_updated_at": "2016-11-04T16:00:01.147Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4f98f232b4497247363c1823d1cb506422b24e95db2dbed010dda64f72b863cf"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a3b60026d80f86a3f36d8930f7866c3c3c76258c1393cb3739f09f08667e4461
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
      "id": 4,
      "title": "Clever Chapter Title 4",
      "position": 1,
      "updated_at": "2016-11-04T16:00:02.718Z",
      "course_id": 2,
      "author_id": 9,
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
      "id": 5,
      "title": "Clever Chapter Title 5",
      "position": 2,
      "updated_at": "2016-11-04T16:00:02.741Z",
      "course_id": 2,
      "author_id": 10,
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
      "id": 6,
      "title": "Clever Chapter Title 6",
      "position": 3,
      "updated_at": "2016-11-04T16:00:02.764Z",
      "course_id": 2,
      "author_id": 11,
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
	-H "Authorization: Bearer a3b60026d80f86a3f36d8930f7866c3c3c76258c1393cb3739f09f08667e4461"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 391aac1143f40a1f147d0d51e5bc447c4828f179e8e3187c58fe8aed4cf44d1a
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
	-H "Authorization: Bearer 391aac1143f40a1f147d0d51e5bc447c4828f179e8e3187c58fe8aed4cf44d1a"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/72
Content-Type: application/json
Authorization: Bearer f2901ebcc488d0c2ff67dc6aa5bf0185dc04d89a9db7f4e16908f9b6661ec37a
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/72" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f2901ebcc488d0c2ff67dc6aa5bf0185dc04d89a9db7f4e16908f9b6661ec37a"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 7da804a5e198702feb3a529b4d14dccef96f70cda709665d7679cce6f3a446a4
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
    "creator_id": 288,
    "id": 75,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 75,
    "additional_university_ids": [

    ],
    "topic_id": 75,
    "discipline_id": 75,
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
    "chapters_updated_at": "2016-11-04T16:00:25.861Z",
    "updated_at": "2016-11-04T16:00:27.612Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 70,
        "title": "Clever Chapter Title 67",
        "position": 1,
        "updated_at": "2016-11-04T16:00:27.561Z",
        "course_id": 75,
        "author_id": 288,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-04T16:00:25.861Z",
        "questions_updated_at": "2016-11-04T16:00:25.861Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 71,
        "title": "Clever Chapter Title 68",
        "position": 2,
        "updated_at": "2016-11-04T16:00:27.603Z",
        "course_id": 75,
        "author_id": 288,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-04T16:00:25.861Z",
        "questions_updated_at": "2016-11-04T16:00:25.861Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 32,
        "obfuscated_id": "mUuSuaqqphM",
        "author_id": 288,
        "chapter_id": 70,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.378Z",
        "created_at": "2016-11-04T16:00:27.378Z",
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
        "author_id": 288,
        "chapter_id": 71,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.461Z",
        "created_at": "2016-11-04T16:00:27.461Z",
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
        "author_id": 288,
        "chapter_id": 70,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.426Z",
        "created_at": "2016-11-04T16:00:27.426Z",
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
        "author_id": 288,
        "chapter_id": 71,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.507Z",
        "created_at": "2016-11-04T16:00:27.507Z",
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
        "author_id": 291,
        "chapter_id": 70,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.549Z",
        "created_at": "2016-11-04T16:00:27.549Z",
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
        "author_id": 292,
        "chapter_id": 71,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-04T16:00:27.591Z",
        "created_at": "2016-11-04T16:00:27.591Z",
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
	-H "Authorization: Bearer 7da804a5e198702feb3a529b4d14dccef96f70cda709665d7679cce6f3a446a4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/77
Content-Type: application/json
Authorization: Bearer 7576d1f11cbd96a36663b504a1cf31d2fcf7128af8e48e11696a0a9e56218669
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
    "creator_id": 300,
    "id": 77,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 77,
    "additional_university_ids": [

    ],
    "topic_id": 77,
    "discipline_id": 77,
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
    "updated_at": "2016-11-04T16:00:29.680Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/77" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7576d1f11cbd96a36663b504a1cf31d2fcf7128af8e48e11696a0a9e56218669"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 14751741b62440c9b0553edabbb0fec41bd988a619f9c13b77e11ded285bd73b
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
    "creator_id": 305,
    "id": 80,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 80,
    "additional_university_ids": [

    ],
    "topic_id": 80,
    "discipline_id": 80,
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
    "updated_at": "2016-11-04T16:00:30.072Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14751741b62440c9b0553edabbb0fec41bd988a619f9c13b77e11ded285bd73b"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 5548da7794c842826a0eabb0a1fb31daadd22cec10fe4ecdc78a63c53498168f
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
      "id": 7,
      "user_id": 91,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:07.518Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 95,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:07.807Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 99,
      "feedbackable_id": 6,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:08.101Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 103,
      "feedbackable_id": 7,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:08.396Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 107,
      "feedbackable_id": 8,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-04T16:00:08.693Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5548da7794c842826a0eabb0a1fb31daadd22cec10fe4ecdc78a63c53498168f"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer dfb45c2d3a72d1888e4ad3ff37604fa5c2080fce397e20ba062a094767ae2fc0
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
      "id": 25,
      "user_id": 165,
      "feedbackable_id": 22,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-04T16:00:13.042Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dfb45c2d3a72d1888e4ad3ff37604fa5c2080fce397e20ba062a094767ae2fc0"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 76e3241cd18fd4d54105d3ad09cf82bff5dca88f4996799846b097959cb5bd98
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
	-H "Authorization: Bearer 76e3241cd18fd4d54105d3ad09cf82bff5dca88f4996799846b097959cb5bd98"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/14/metadata
Content-Type: application/json
Authorization: Bearer 7611701533cdcad29586a9f28372620c32ecda18b2584fddac2f89f2173b8456
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
    "id": 14,
    "uploader": {
      "id": 369,
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
      "created_at": "2016-11-04T16:00:34.933Z",
      "updated_at": "2016-11-04T16:00:34.933Z"
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
    "created_at": "2016-11-04T16:00:35.010Z",
    "updated_at": "2016-11-04T16:00:35.010Z",
    "course_id": 101,
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
curl "api.goskive.com/v2/files/14/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7611701533cdcad29586a9f28372620c32ecda18b2584fddac2f89f2173b8456"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/91/feedbacks
Content-Type: application/json
Authorization: Bearer 8d0d97c96a31873938d01c9dccee6e0b3d2e7ef0ec36d6a96e0853fc344a748f
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
      "id": 42,
      "user_id": 962,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:01:23.835Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 961,
      "feedbackable_id": 91,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:01:23.823Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/91/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8d0d97c96a31873938d01c9dccee6e0b3d2e7ef0ec36d6a96e0853fc344a748f"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 329828a658cea09c4eb467ffd9d0c52bf234f2d5c74d02d86199409826feb8c6
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
      "id": 69,
      "obfuscated_id": "1EDi_PBgOnI",
      "author_id": 481,
      "chapter_id": 101,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:42.551Z",
      "created_at": "2016-11-04T16:00:42.551Z",
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
      "author_id": 484,
      "chapter_id": 102,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:42.687Z",
      "created_at": "2016-11-04T16:00:42.687Z",
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
      "author_id": 487,
      "chapter_id": 103,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:42.819Z",
      "created_at": "2016-11-04T16:00:42.819Z",
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
      "author_id": 490,
      "chapter_id": 104,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:42.952Z",
      "created_at": "2016-11-04T16:00:42.952Z",
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 493,
      "chapter_id": 105,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:43.083Z",
      "created_at": "2016-11-04T16:00:43.083Z",
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
	-H "Authorization: Bearer 329828a658cea09c4eb467ffd9d0c52bf234f2d5c74d02d86199409826feb8c6"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 05a439bfd3bb63ac0c6a56251932da35493817e8850e82e9e9595a37de1ed34a
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
      "author_id": 461,
      "chapter_id": 95,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:00:41.671Z",
      "created_at": "2016-11-04T16:00:41.671Z",
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
	-H "Authorization: Bearer 05a439bfd3bb63ac0c6a56251932da35493817e8850e82e9e9595a37de1ed34a"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/56/republish
Content-Type: application/json
Authorization: Bearer c718df9d50a360f3aa0293a6b9ebedb3b8bd62c9bec5f49ce8f5cae0c22f78d8
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
	-H "Authorization: Bearer c718df9d50a360f3aa0293a6b9ebedb3b8bd62c9bec5f49ce8f5cae0c22f78d8"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/87/feedbacks
Content-Type: application/json
Authorization: Bearer ccf711660ca66612d3acee604b913b478020a99d2e554de7db76183e049451d5
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
      "id": 35,
      "user_id": 716,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:59.206Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 715,
      "feedbackable_id": 87,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-04T16:00:59.195Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/87/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ccf711660ca66612d3acee604b913b478020a99d2e554de7db76183e049451d5"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 8a2788973c1d601d3974883a51001cee2c3df15dbbdd4f0585b7067373078252
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
      "id": 123,
      "obfuscated_id": "N9-wuAhut60",
      "author_id": 915,
      "chapter_id": 176,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:19.032Z",
      "created_at": "2016-11-04T16:01:18.912Z",
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
          "id": 248,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 249,
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
      "author_id": 906,
      "chapter_id": 173,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:18.184Z",
      "created_at": "2016-11-04T16:01:18.064Z",
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
          "id": 242,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 243,
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
      "author_id": 909,
      "chapter_id": 174,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:18.465Z",
      "created_at": "2016-11-04T16:01:18.344Z",
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
          "id": 244,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 245,
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
      "author_id": 912,
      "chapter_id": 175,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:18.752Z",
      "created_at": "2016-11-04T16:01:18.631Z",
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
    },
    {
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 918,
      "chapter_id": 177,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:19.309Z",
      "created_at": "2016-11-04T16:01:19.196Z",
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
          "id": 250,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 251,
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
	-H "Authorization: Bearer 8a2788973c1d601d3974883a51001cee2c3df15dbbdd4f0585b7067373078252"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer b53f3ff3e5fdb92051b2c707232619dd3618dc0e36431087412caa7c01d63c27
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
      "id": 129,
      "obfuscated_id": "x8EyeGrWnN4",
      "author_id": 934,
      "chapter_id": 182,
      "position": 120,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-04T16:01:20.796Z",
      "created_at": "2016-11-04T16:01:20.683Z",
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
          "id": 260,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 261,
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
	-H "Authorization: Bearer b53f3ff3e5fdb92051b2c707232619dd3618dc0e36431087412caa7c01d63c27"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/110/republish
Content-Type: application/json
Authorization: Bearer 5caa641d183252edea7fc297812144ef15d5a9358999569db1dfe91c9c29cb22
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/110/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5caa641d183252edea7fc297812144ef15d5a9358999569db1dfe91c9c29cb22"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 4cb582811111114cc029ff2db8c2febde1958163352b7670f766d85e178f2427
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":230,"published":false}}
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
    "creator_id": 726,
    "id": 220,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 222,
    "additional_university_ids": [

    ],
    "topic_id": 230,
    "discipline_id": 230,
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
    "updated_at": "2016-11-04T16:01:00.594Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":230,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4cb582811111114cc029ff2db8c2febde1958163352b7670f766d85e178f2427"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cd3cdb9aaedfa6c1e636b57c92fe6062d2b6d8530cd461afa1101079697f088e
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
      "creator_id": 754,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 234,
      "additional_university_ids": [

      ],
      "topic_id": 254,
      "discipline_id": 254,
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
      "updated_at": "2016-11-04T16:01:03.202Z",
      "shortname": "fu-course-181"
    },
    {
      "creator_id": 754,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 234,
      "additional_university_ids": [

      ],
      "topic_id": 255,
      "discipline_id": 255,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-11-04T16:01:03.242Z",
      "shortname": "fu-course-182"
    },
    {
      "creator_id": 755,
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-183",
      "html_url": "https://goskive.com/course/fu-course-183",
      "slug": "fu-course-183",
      "university_id": 234,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 256,
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
      "updated_at": "2016-11-04T16:01:03.291Z",
      "shortname": "fu-course-183"
    },
    {
      "creator_id": 755,
      "id": 247,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-184",
      "html_url": "https://goskive.com/course/fu-course-184",
      "slug": "fu-course-184",
      "university_id": 234,
      "additional_university_ids": [

      ],
      "topic_id": 257,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 184",
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
      "chapters_updated_at": "2016-11-04T16:01:03.579Z",
      "updated_at": "2016-11-04T16:01:03.586Z",
      "shortname": "fu-course-184"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cd3cdb9aaedfa6c1e636b57c92fe6062d2b6d8530cd461afa1101079697f088e"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a8f62fd9c2694dad40b895e93bc9a9d1d8d4d801c95631d830caa4933e7c3a07
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
      "creator_id": 760,
      "id": 248,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-185",
      "html_url": "https://goskive.com/course/fu-course-185",
      "slug": "fu-course-185",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 258,
      "discipline_id": 258,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 185",
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
      "updated_at": "2016-11-04T16:01:03.730Z",
      "shortname": "fu-course-185"
    },
    {
      "creator_id": 760,
      "id": 249,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-186",
      "html_url": "https://goskive.com/course/fu-course-186",
      "slug": "fu-course-186",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 259,
      "discipline_id": 259,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 186",
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
      "updated_at": "2016-11-04T16:01:03.786Z",
      "shortname": "fu-course-186"
    },
    {
      "creator_id": 761,
      "id": 250,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-187",
      "html_url": "https://goskive.com/course/fu-course-187",
      "slug": "fu-course-187",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 260,
      "discipline_id": 260,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 187",
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
      "updated_at": "2016-11-04T16:01:03.833Z",
      "shortname": "fu-course-187"
    },
    {
      "creator_id": 761,
      "id": 251,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-188",
      "html_url": "https://goskive.com/course/fu-course-188",
      "slug": "fu-course-188",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 261,
      "discipline_id": 261,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 188",
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
      "updated_at": "2016-11-04T16:01:03.873Z",
      "shortname": "fu-course-188"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a8f62fd9c2694dad40b895e93bc9a9d1d8d4d801c95631d830caa4933e7c3a07"
```
