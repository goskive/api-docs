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
DELETE /v2/chapters/192
Content-Type: application/json
Authorization: Bearer 3d92eb4b4525a367a2e03ee65ca7e82af4cef540a094f56b29af09267044bebb
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/192" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d92eb4b4525a367a2e03ee65ca7e82af4cef540a094f56b29af09267044bebb"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 81e345baa443825e245e0a16dc6b8aec70f7e7540994e387fa447ea6cccdd77c
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
    "id": 190,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T19:46:10.022Z",
    "course_id": 307,
    "author_id": 954,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-26T19:46:09.463Z",
    "questions_updated_at": "2016-10-26T19:46:09.463Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 957,
        "chapter_id": 190,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:09.965Z",
        "created_at": "2016-10-26T19:46:09.965Z",
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
        "author_id": 958,
        "chapter_id": 190,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:10.002Z",
        "created_at": "2016-10-26T19:46:10.002Z",
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
        "id": 129,
        "obfuscated_id": "x8EyeGrWnN4",
        "author_id": 955,
        "chapter_id": 190,
        "position": 116,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:09.700Z",
        "created_at": "2016-10-26T19:46:09.580Z",
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
      },
      {
        "id": 130,
        "obfuscated_id": "N-qIf0IsvWM",
        "author_id": 956,
        "chapter_id": 190,
        "position": 117,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:09.893Z",
        "created_at": "2016-10-26T19:46:09.774Z",
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
            "id": 263,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 264,
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
curl "api.goskive.com/v2/chapters/190" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81e345baa443825e245e0a16dc6b8aec70f7e7540994e387fa447ea6cccdd77c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/189
Content-Type: application/json
Authorization: Bearer 8ffad80be1df8aea8b705ef2dbf353521717ae24f12f2c8f1fd9d5fcd061788b
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
    "id": 189,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T19:46:09.433Z",
    "course_id": 306,
    "author_id": 951,
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
curl "api.goskive.com/v2/chapters/189" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8ffad80be1df8aea8b705ef2dbf353521717ae24f12f2c8f1fd9d5fcd061788b"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/15
Content-Type: application/json
Authorization: Bearer 852828a3cc09d4b2614d05c54e8357623209ba9787a1ec087321abc7fc451a61
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 852828a3cc09d4b2614d05c54e8357623209ba9787a1ec087321abc7fc451a61"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer dc6265b5a6b7734e1573a26eccffba67959a0acfadf295278b01c7643ff2dc20
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
      "author_id": 714,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:46.504Z",
      "status": "published",
      "subject_id": 229,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 716,
      "reply_to_id": 31,
      "created_at": "2016-10-26T19:45:46.582Z",
      "status": "published",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 718,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:46.662Z",
      "status": "published",
      "subject_id": 231,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 720,
      "reply_to_id": 33,
      "created_at": "2016-10-26T19:45:46.742Z",
      "status": "published",
      "subject_id": 232,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 722,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:46.824Z",
      "status": "reported",
      "subject_id": 233,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 724,
      "reply_to_id": 35,
      "created_at": "2016-10-26T19:45:46.910Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 726,
      "reply_to_id": 35,
      "created_at": "2016-10-26T19:45:46.997Z",
      "status": "published",
      "subject_id": 235,
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
	-H "Authorization: Bearer dc6265b5a6b7734e1573a26eccffba67959a0acfadf295278b01c7643ff2dc20"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 02074cca4ad939e3ad1f0d9a301e1c60f1ecf201f2fd1aaf93d69447db9d6ebe
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
      "id": 45,
      "author_id": 744,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:47.787Z",
      "status": "published",
      "subject_id": 243,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 746,
      "reply_to_id": 45,
      "created_at": "2016-10-26T19:45:47.871Z",
      "status": "published",
      "subject_id": 244,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 748,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:47.956Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 750,
      "reply_to_id": 47,
      "created_at": "2016-10-26T19:45:48.036Z",
      "status": "published",
      "subject_id": 246,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 752,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:48.116Z",
      "status": "reported",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 754,
      "reply_to_id": 49,
      "created_at": "2016-10-26T19:45:48.199Z",
      "status": "published",
      "subject_id": 248,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 756,
      "reply_to_id": 49,
      "created_at": "2016-10-26T19:45:48.281Z",
      "status": "published",
      "subject_id": 249,
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
	-H "Authorization: Bearer 02074cca4ad939e3ad1f0d9a301e1c60f1ecf201f2fd1aaf93d69447db9d6ebe"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 52046970d337ed181cbe4595645988ad6d1842e769bd20cfc78f62279f9aa232
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
      "id": 39,
      "author_id": 731,
      "reply_to_id": 38,
      "created_at": "2016-10-26T19:45:47.218Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 735,
      "reply_to_id": 40,
      "created_at": "2016-10-26T19:45:47.380Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 739,
      "reply_to_id": 42,
      "created_at": "2016-10-26T19:45:47.547Z",
      "status": "published",
      "subject_id": 241,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 741,
      "reply_to_id": 42,
      "created_at": "2016-10-26T19:45:47.657Z",
      "status": "published",
      "subject_id": 242,
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
	-H "Authorization: Bearer 52046970d337ed181cbe4595645988ad6d1842e769bd20cfc78f62279f9aa232"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 0ea1944ffd2723b646fa649bc801e59faa9ca62fe7584cba2b6ba7d73d621ccb
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
      "author_id": 692,
      "reply_to_id": null,
      "created_at": "2016-10-26T19:45:45.616Z",
      "status": "reported",
      "subject_id": 219,
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
	-H "Authorization: Bearer 0ea1944ffd2723b646fa649bc801e59faa9ca62fe7584cba2b6ba7d73d621ccb"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/12/republish
Content-Type: application/json
Authorization: Bearer eae12d9678c6a53516e5ec6067627d6e7f41e12ee0ed306ba2a7241959e536ee
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/12/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eae12d9678c6a53516e5ec6067627d6e7f41e12ee0ed306ba2a7241959e536ee"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 2571abab60d5b1cd34e2f1dc6ffabb5268d6fd514c479fd6e6c4e57cd77a592e
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
    "id": 92,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:45:33.179Z",
    "course_id": 157,
    "author_id": 485,
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
	-H "Authorization: Bearer 2571abab60d5b1cd34e2f1dc6ffabb5268d6fd514c479fd6e6c4e57cd77a592e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/159/chapters
Content-Type: application/json
Authorization: Bearer 5ff63fa6e54c6460f3d9a50b80a7848f3e0e83bf9ba55c9a9e47b166038b9752
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
    "id": 94,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T19:45:33.452Z",
    "course_id": 159,
    "author_id": 489,
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
curl "api.goskive.com/v2/courses/159/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ff63fa6e54c6460f3d9a50b80a7848f3e0e83bf9ba55c9a9e47b166038b9752"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6f6ea2b591e0f6a9c76482c498d83233ba23e2bc6c13f8d3478f065c9ec5d095
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
      "id": 101,
      "title": "Clever Chapter Title 95",
      "position": 1,
      "updated_at": "2016-10-26T19:45:34.212Z",
      "course_id": 163,
      "author_id": 502,
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
      "id": 102,
      "title": "Clever Chapter Title 96",
      "position": 2,
      "updated_at": "2016-10-26T19:45:34.237Z",
      "course_id": 163,
      "author_id": 503,
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
      "id": 103,
      "title": "Clever Chapter Title 97",
      "position": 3,
      "updated_at": "2016-10-26T19:45:34.484Z",
      "course_id": 163,
      "author_id": 504,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-26T19:45:34.135Z",
      "questions_updated_at": "2016-10-26T19:45:34.135Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f6ea2b591e0f6a9c76482c498d83233ba23e2bc6c13f8d3478f065c9ec5d095"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7a1a4533a2916933cc82db87bfc1898eb229898cfa484b0cf859cb0253854e15
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
      "id": 104,
      "title": "Clever Chapter Title 98",
      "position": 1,
      "updated_at": "2016-10-26T19:45:34.686Z",
      "course_id": 164,
      "author_id": 509,
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
      "id": 105,
      "title": "Clever Chapter Title 99",
      "position": 2,
      "updated_at": "2016-10-26T19:45:34.709Z",
      "course_id": 164,
      "author_id": 510,
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
      "title": "Clever Chapter Title 100",
      "position": 3,
      "updated_at": "2016-10-26T19:45:34.733Z",
      "course_id": 164,
      "author_id": 511,
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
	-H "Authorization: Bearer 7a1a4533a2916933cc82db87bfc1898eb229898cfa484b0cf859cb0253854e15"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer da5048e7c2324c0a880cbc434910deefccee47ca2ea549d0796ec9093845bb8c
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
	-H "Authorization: Bearer da5048e7c2324c0a880cbc434910deefccee47ca2ea549d0796ec9093845bb8c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/285
Content-Type: application/json
Authorization: Bearer 3aec9dc4c1ed747fd97ba2dbe15dee646462a53513fdcbcb1c6984c8d6463ef4
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/285" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3aec9dc4c1ed747fd97ba2dbe15dee646462a53513fdcbcb1c6984c8d6463ef4"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 3ca481dbb67baf6cadc5646f1224a642bc7a9bf626d1223d482358a1118a943f
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
    "creator_id": 902,
    "id": 293,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 278,
    "additional_university_ids": [

    ],
    "topic_id": 305,
    "discipline_id": 306,
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
    "chapters_updated_at": "2016-10-26T19:46:02.643Z",
    "updated_at": "2016-10-26T19:46:04.087Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 174,
        "title": "Clever Chapter Title 159",
        "position": 1,
        "updated_at": "2016-10-26T19:46:04.039Z",
        "course_id": 293,
        "author_id": 902,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T19:46:02.643Z",
        "questions_updated_at": "2016-10-26T19:46:02.643Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 175,
        "title": "Clever Chapter Title 160",
        "position": 2,
        "updated_at": "2016-10-26T19:46:04.079Z",
        "course_id": 293,
        "author_id": 902,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T19:46:02.643Z",
        "questions_updated_at": "2016-10-26T19:46:02.643Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 902,
        "chapter_id": 174,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:03.878Z",
        "created_at": "2016-10-26T19:46:03.878Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 902,
        "chapter_id": 175,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:03.949Z",
        "created_at": "2016-10-26T19:46:03.949Z",
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
        "author_id": 902,
        "chapter_id": 174,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:03.918Z",
        "created_at": "2016-10-26T19:46:03.918Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 902,
        "chapter_id": 175,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:03.990Z",
        "created_at": "2016-10-26T19:46:03.990Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 905,
        "chapter_id": 174,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:04.030Z",
        "created_at": "2016-10-26T19:46:04.030Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 906,
        "chapter_id": 175,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T19:46:04.069Z",
        "created_at": "2016-10-26T19:46:04.069Z",
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
	-H "Authorization: Bearer 3ca481dbb67baf6cadc5646f1224a642bc7a9bf626d1223d482358a1118a943f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/289
Content-Type: application/json
Authorization: Bearer 736f8d7ecf8818330dda57e2b0f4371c058b7a215e56f97388306afd77593efc
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
    "creator_id": 887,
    "id": 289,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 274,
    "additional_university_ids": [

    ],
    "topic_id": 301,
    "discipline_id": 302,
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
    "updated_at": "2016-10-26T19:45:59.330Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/289" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 736f8d7ecf8818330dda57e2b0f4371c058b7a215e56f97388306afd77593efc"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3099386b0de26d084a7fb1dddc7cfca608618fa8942d1c674af75ad3219d7fb8
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
    "creator_id": 882,
    "id": 286,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 271,
    "additional_university_ids": [

    ],
    "topic_id": 298,
    "discipline_id": 299,
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
    "updated_at": "2016-10-26T19:45:58.968Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3099386b0de26d084a7fb1dddc7cfca608618fa8942d1c674af75ad3219d7fb8"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 974dae6dbcc4a6a42edf1a17d200908cc2698692e232f6feaa88cd1ae14e4e94
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
      "id": 1,
      "user_id": 148,
      "feedbackable_id": 33,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:09.824Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 2,
      "user_id": 152,
      "feedbackable_id": 34,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:10.111Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 156,
      "feedbackable_id": 35,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:10.388Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 160,
      "feedbackable_id": 36,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:10.673Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 164,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T19:45:10.958Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 974dae6dbcc4a6a42edf1a17d200908cc2698692e232f6feaa88cd1ae14e4e94"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 528626364cfac7a74b9df3b564ce26fb224cd735dec5564f69f7426c1fda18c4
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
      "id": 19,
      "user_id": 222,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T19:45:15.277Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 528626364cfac7a74b9df3b564ce26fb224cd735dec5564f69f7426c1fda18c4"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/12
Content-Type: application/json
Authorization: Bearer 84269730c18c8c0f0fc42b980fefdb5e5ef48abda8db8cab2ebc79e6b8627672
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
	-H "Authorization: Bearer 84269730c18c8c0f0fc42b980fefdb5e5ef48abda8db8cab2ebc79e6b8627672"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/7/metadata
Content-Type: application/json
Authorization: Bearer d1b5e9555ce4c6a2140076b1166fb2ca3cbea95f26682da8b0bf749a85fd693a
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
    "id": 7,
    "uploader": {
      "id": 434,
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
      "created_at": "2016-10-26T19:45:29.182Z",
      "updated_at": "2016-10-26T19:45:29.182Z"
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
    "created_at": "2016-10-26T19:45:29.258Z",
    "updated_at": "2016-10-26T19:45:29.258Z",
    "course_id": 140,
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
curl "api.goskive.com/v2/files/7/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d1b5e9555ce4c6a2140076b1166fb2ca3cbea95f26682da8b0bf749a85fd693a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/20/feedbacks
Content-Type: application/json
Authorization: Bearer 457bac2853be32bfc48f5818c4ccfcce7cee6d9283e5727d84bd5dee0c4ceb9a
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
      "id": 32,
      "user_id": 316,
      "feedbackable_id": 20,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:20.420Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 315,
      "feedbackable_id": 20,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:20.409Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/20/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 457bac2853be32bfc48f5818c4ccfcce7cee6d9283e5727d84bd5dee0c4ceb9a"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 0f7314a846efe7c0c894ef32236a0ee44100e7678111dec00327e6abfd22f3f9
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
      "id": 40,
      "obfuscated_id": "lir5nwklJts",
      "author_id": 608,
      "chapter_id": 129,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.325Z",
      "created_at": "2016-10-26T19:45:41.325Z",
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
      "author_id": 611,
      "chapter_id": 130,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.453Z",
      "created_at": "2016-10-26T19:45:41.453Z",
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
      "author_id": 614,
      "chapter_id": 131,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.581Z",
      "created_at": "2016-10-26T19:45:41.581Z",
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
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 617,
      "chapter_id": 132,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.710Z",
      "created_at": "2016-10-26T19:45:41.710Z",
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
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 620,
      "chapter_id": 133,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.834Z",
      "created_at": "2016-10-26T19:45:41.834Z",
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
	-H "Authorization: Bearer 0f7314a846efe7c0c894ef32236a0ee44100e7678111dec00327e6abfd22f3f9"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 37c828c6dd945d8c2575cfe3864fe129748114924d59b85643ce27633c1a6d9e
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
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 604,
      "chapter_id": 128,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:41.165Z",
      "created_at": "2016-10-26T19:45:41.165Z",
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
	-H "Authorization: Bearer 37c828c6dd945d8c2575cfe3864fe129748114924d59b85643ce27633c1a6d9e"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/52/republish
Content-Type: application/json
Authorization: Bearer 4c9e3b869e738dc6ba35f1592c4fcf19230063126bc644539babfe5adf33c7f2
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
	-H "Authorization: Bearer 4c9e3b869e738dc6ba35f1592c4fcf19230063126bc644539babfe5adf33c7f2"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/79/feedbacks
Content-Type: application/json
Authorization: Bearer 1482f5bae698ae0bc742c4478817d41d1331937cc9564fd4cbb6c9a04310415a
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
      "id": 43,
      "user_id": 793,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:50.868Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 792,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T19:45:50.858Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/79/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1482f5bae698ae0bc742c4478817d41d1331937cc9564fd4cbb6c9a04310415a"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 9eacee37d35ce74c7a711cd438c0bce75fa83c235a836826d9d90a173f3f91cf
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 121,
      "chapter_id": 31,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:07.148Z",
      "created_at": "2016-10-26T19:45:07.012Z",
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
          "id": 56,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 57,
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
      "author_id": 112,
      "chapter_id": 28,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:06.253Z",
      "created_at": "2016-10-26T19:45:06.124Z",
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
          "id": 50,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 51,
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
      "author_id": 115,
      "chapter_id": 29,
      "position": 17,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:06.550Z",
      "created_at": "2016-10-26T19:45:06.423Z",
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
          "id": 52,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 53,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 118,
      "chapter_id": 30,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:06.847Z",
      "created_at": "2016-10-26T19:45:06.716Z",
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
          "id": 54,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 55,
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
      "author_id": 124,
      "chapter_id": 32,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:07.455Z",
      "created_at": "2016-10-26T19:45:07.324Z",
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
          "id": 58,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 59,
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
	-H "Authorization: Bearer 9eacee37d35ce74c7a711cd438c0bce75fa83c235a836826d9d90a173f3f91cf"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 2d5bb32c64730fc44872637d1a5dfc5701a9bd2e8dbffa8a5f8b1d40f8a4d559
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 108,
      "chapter_id": 27,
      "position": 15,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T19:45:05.914Z",
      "created_at": "2016-10-26T19:45:05.792Z",
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
          "id": 48,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 49,
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
	-H "Authorization: Bearer 2d5bb32c64730fc44872637d1a5dfc5701a9bd2e8dbffa8a5f8b1d40f8a4d559"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/10/republish
Content-Type: application/json
Authorization: Bearer 81c5a0d73729d90784337efae83ed116d004343edd2c7b611e43ef3bbd1a0a86
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
	-H "Authorization: Bearer 81c5a0d73729d90784337efae83ed116d004343edd2c7b611e43ef3bbd1a0a86"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 026c68633434c2ab41723441f114695e153523afbe04f39ef131b69d3004fb2e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":1,"published":false}}
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
    "creator_id": 1,
    "id": 1,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 1,
    "additional_university_ids": [

    ],
    "topic_id": 1,
    "discipline_id": 1,
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
    "updated_at": "2016-10-26T19:44:54.366Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":1,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 026c68633434c2ab41723441f114695e153523afbe04f39ef131b69d3004fb2e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f17494b8f95b6f89a52fbf81343658c555c8f677f03b62fb26bcb0c1a8acfe9f
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
      "creator_id": 26,
      "id": 25,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-21",
      "html_url": "https://goskive.com/course/fu-course-21",
      "slug": "fu-course-21",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 25,
      "discipline_id": 25,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 21",
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
      "updated_at": "2016-10-26T19:44:56.836Z",
      "shortname": "fu-course-21"
    },
    {
      "creator_id": 26,
      "id": 26,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-22",
      "html_url": "https://goskive.com/course/fu-course-22",
      "slug": "fu-course-22",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 26,
      "discipline_id": 26,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 22",
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
      "updated_at": "2016-10-26T19:44:56.871Z",
      "shortname": "fu-course-22"
    },
    {
      "creator_id": 27,
      "id": 27,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-23",
      "html_url": "https://goskive.com/course/fu-course-23",
      "slug": "fu-course-23",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 27,
      "discipline_id": 27,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 23",
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
      "updated_at": "2016-10-26T19:44:56.913Z",
      "shortname": "fu-course-23"
    },
    {
      "creator_id": 27,
      "id": 28,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-24",
      "html_url": "https://goskive.com/course/fu-course-24",
      "slug": "fu-course-24",
      "university_id": 13,
      "additional_university_ids": [

      ],
      "topic_id": 28,
      "discipline_id": 28,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 24",
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
      "chapters_updated_at": "2016-10-26T19:44:57.182Z",
      "updated_at": "2016-10-26T19:44:57.189Z",
      "shortname": "fu-course-24"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f17494b8f95b6f89a52fbf81343658c555c8f677f03b62fb26bcb0c1a8acfe9f"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2b5d169c18f3dcfcdb2b7abb817137358db09fff9f7b560e5956d30768e3e527
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
      "creator_id": 33,
      "id": 29,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-25",
      "html_url": "https://goskive.com/course/fu-course-25",
      "slug": "fu-course-25",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 29,
      "discipline_id": 29,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 25",
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
      "updated_at": "2016-10-26T19:44:57.404Z",
      "shortname": "fu-course-25"
    },
    {
      "creator_id": 33,
      "id": 30,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-26",
      "html_url": "https://goskive.com/course/fu-course-26",
      "slug": "fu-course-26",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 30,
      "discipline_id": 30,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 26",
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
      "updated_at": "2016-10-26T19:44:57.442Z",
      "shortname": "fu-course-26"
    },
    {
      "creator_id": 34,
      "id": 31,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 31,
      "discipline_id": 31,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
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
      "updated_at": "2016-10-26T19:44:57.488Z",
      "shortname": "fu-course-27"
    },
    {
      "creator_id": 34,
      "id": 32,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 15,
      "additional_university_ids": [

      ],
      "topic_id": 32,
      "discipline_id": 32,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
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
      "updated_at": "2016-10-26T19:44:57.526Z",
      "shortname": "fu-course-28"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2b5d169c18f3dcfcdb2b7abb817137358db09fff9f7b560e5956d30768e3e527"
```
