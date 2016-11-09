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
DELETE /v2/chapters/51
Content-Type: application/json
Authorization: Bearer 2c26d29ef380a9b12411d9258ce89b46f59cda3e3106892c45daac2024698675
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/51" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c26d29ef380a9b12411d9258ce89b46f59cda3e3106892c45daac2024698675"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/50
Content-Type: application/json
Authorization: Bearer ad40eeb9455321cddcb4d45bcd63a9eeacbff641649d6af6b13fe4e5436ec481
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
    "id": 50,
    "updated_at": "2016-11-09T13:40:49.398Z",
    "course_id": 91,
    "author_id": 233,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-09T13:40:48.879Z",
    "questions_updated_at": "2016-11-09T13:40:48.879Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 8,
        "obfuscated_id": "X2B_8FVuFe8",
        "author_id": 236,
        "chapter_id": 50,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:40:49.345Z",
        "created_at": "2016-11-09T13:40:49.345Z",
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
        "id": 9,
        "obfuscated_id": "DMbUb8tMXMw",
        "author_id": 237,
        "chapter_id": 50,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:40:49.380Z",
        "created_at": "2016-11-09T13:40:49.380Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 234,
        "chapter_id": 50,
        "position": 35,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:40:49.093Z",
        "created_at": "2016-11-09T13:40:48.986Z",
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
            "id": 88,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 89,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 235,
        "chapter_id": 50,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:40:49.279Z",
        "created_at": "2016-11-09T13:40:49.162Z",
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
            "id": 90,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 91,
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
curl "api.goskive.com/v2/chapters/50" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ad40eeb9455321cddcb4d45bcd63a9eeacbff641649d6af6b13fe4e5436ec481"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/46
Content-Type: application/json
Authorization: Bearer 91b224be12c9c83830f9f899e8cb301ce49451fa55c56d6453e516073b628fd4
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
    "id": 46,
    "updated_at": "2016-11-09T13:40:47.837Z",
    "course_id": 87,
    "author_id": 218,
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
curl "api.goskive.com/v2/chapters/46" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91b224be12c9c83830f9f899e8cb301ce49451fa55c56d6453e516073b628fd4"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer 32ea4d81ad2e39461f58aa64ad3c518a064a3a5bc23c3feec560b1a8a472545b
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/47" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32ea4d81ad2e39461f58aa64ad3c518a064a3a5bc23c3feec560b1a8a472545b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 67da711ab1b57c9c9aa439b1237b9942efbe502362446774d538e8e79d643905
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
      "author_id": 780,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:31.838Z",
      "status": "published",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 782,
      "reply_to_id": 17,
      "created_at": "2016-11-09T13:41:31.920Z",
      "status": "published",
      "subject_id": 248,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 784,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:32.005Z",
      "status": "published",
      "subject_id": 249,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 786,
      "reply_to_id": 19,
      "created_at": "2016-11-09T13:41:32.088Z",
      "status": "published",
      "subject_id": 250,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 788,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:32.174Z",
      "status": "reported",
      "subject_id": 251,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 790,
      "reply_to_id": 21,
      "created_at": "2016-11-09T13:41:32.258Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 792,
      "reply_to_id": 21,
      "created_at": "2016-11-09T13:41:32.342Z",
      "status": "published",
      "subject_id": 253,
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
	-H "Authorization: Bearer 67da711ab1b57c9c9aa439b1237b9942efbe502362446774d538e8e79d643905"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 9e88495e57bc662fa1091bbd423e6d41fb62c88c1ac24c6dd8cb281c2b70d2cc
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
      "author_id": 795,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:32.483Z",
      "status": "published",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 797,
      "reply_to_id": 24,
      "created_at": "2016-11-09T13:41:32.568Z",
      "status": "published",
      "subject_id": 255,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 799,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:32.648Z",
      "status": "published",
      "subject_id": 256,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 801,
      "reply_to_id": 26,
      "created_at": "2016-11-09T13:41:32.732Z",
      "status": "published",
      "subject_id": 257,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 803,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:32.816Z",
      "status": "reported",
      "subject_id": 258,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 805,
      "reply_to_id": 28,
      "created_at": "2016-11-09T13:41:32.899Z",
      "status": "published",
      "subject_id": 259,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 807,
      "reply_to_id": 28,
      "created_at": "2016-11-09T13:41:32.980Z",
      "status": "published",
      "subject_id": 260,
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
	-H "Authorization: Bearer 9e88495e57bc662fa1091bbd423e6d41fb62c88c1ac24c6dd8cb281c2b70d2cc"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 6aa9ea6cf9f59ccc696d23678995e1ecd9e40842809f2147a15b708e411d4bd0
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
      "author_id": 812,
      "reply_to_id": 31,
      "created_at": "2016-11-09T13:41:33.200Z",
      "status": "published",
      "subject_id": 262,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 816,
      "reply_to_id": 33,
      "created_at": "2016-11-09T13:41:33.363Z",
      "status": "published",
      "subject_id": 264,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 820,
      "reply_to_id": 35,
      "created_at": "2016-11-09T13:41:33.530Z",
      "status": "published",
      "subject_id": 266,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 822,
      "reply_to_id": 35,
      "created_at": "2016-11-09T13:41:33.642Z",
      "status": "published",
      "subject_id": 267,
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
	-H "Authorization: Bearer 6aa9ea6cf9f59ccc696d23678995e1ecd9e40842809f2147a15b708e411d4bd0"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer c133b168de2a9cc444d5dda18eb796ae705c58fe767989e52e35b23e8eb02998
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
      "id": 14,
      "author_id": 773,
      "reply_to_id": null,
      "created_at": "2016-11-09T13:41:31.546Z",
      "status": "reported",
      "subject_id": 244,
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
	-H "Authorization: Bearer c133b168de2a9cc444d5dda18eb796ae705c58fe767989e52e35b23e8eb02998"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/45/republish
Content-Type: application/json
Authorization: Bearer 13e8e3fcecd73c0043d4ab8133264c74a61d1c67a31865aa7adc0ffc30ad06e2
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/45/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13e8e3fcecd73c0043d4ab8133264c74a61d1c67a31865aa7adc0ffc30ad06e2"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/168/chapters
Content-Type: application/json
Authorization: Bearer 24f76a786f7c7bfa80812d0af2a3b32818c1908b3bd40c1a732376ae848022a5
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
    "id": 108,
    "updated_at": "2016-11-09T13:41:06.389Z",
    "course_id": 168,
    "author_id": 505,
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
curl "api.goskive.com/v2/courses/168/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24f76a786f7c7bfa80812d0af2a3b32818c1908b3bd40c1a732376ae848022a5"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a7b5ac308a9c6b5af0faa3ba2059de0e6db4c60b0508afa9213120965587de62
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
    "id": 110,
    "updated_at": "2016-11-09T13:41:06.909Z",
    "course_id": 171,
    "author_id": 511,
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
	-H "Authorization: Bearer a7b5ac308a9c6b5af0faa3ba2059de0e6db4c60b0508afa9213120965587de62"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 402ba81cfeb20b66aa1a3f20c57ee585319143150ebbe3c4298da391d112a670
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
      "id": 114,
      "updated_at": "2016-11-09T13:41:07.392Z",
      "course_id": 174,
      "author_id": 520,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 99",
      "position": 1
    },
    {
      "id": 115,
      "updated_at": "2016-11-09T13:41:07.417Z",
      "course_id": 174,
      "author_id": 521,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 100",
      "position": 2
    },
    {
      "id": 116,
      "updated_at": "2016-11-09T13:41:07.683Z",
      "course_id": 174,
      "author_id": 522,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-09T13:41:07.314Z",
      "questions_updated_at": "2016-11-09T13:41:07.314Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 101",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 402ba81cfeb20b66aa1a3f20c57ee585319143150ebbe3c4298da391d112a670"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 48dd02b0919a9974025eed34da66b850574f28e2d6cff0ce5607ed9d22d44ce8
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
      "id": 117,
      "updated_at": "2016-11-09T13:41:07.856Z",
      "course_id": 175,
      "author_id": 527,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 102",
      "position": 1
    },
    {
      "id": 118,
      "updated_at": "2016-11-09T13:41:07.880Z",
      "course_id": 175,
      "author_id": 528,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 103",
      "position": 2
    },
    {
      "id": 119,
      "updated_at": "2016-11-09T13:41:07.905Z",
      "course_id": 175,
      "author_id": 529,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 104",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 48dd02b0919a9974025eed34da66b850574f28e2d6cff0ce5607ed9d22d44ce8"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/199
Content-Type: application/json
Authorization: Bearer b8476ac04c65bfe9e6b187c505cd3d469ed32598d9611307aab770b10abb3f85
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/199" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8476ac04c65bfe9e6b187c505cd3d469ed32598d9611307aab770b10abb3f85"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 662528fa046211dbecf45ea7c099d3d5bdf4e9f1fb13dec3dfc6df533cb4b7a4
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
	-H "Authorization: Bearer 662528fa046211dbecf45ea7c099d3d5bdf4e9f1fb13dec3dfc6df533cb4b7a4"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer f217b0187a67230c1be7401ac5c80f6c6ec8f278b20bfac2baa91cf51b575087
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
    "creator_id": 641,
    "id": 211,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 195,
    "additional_university_ids": [

    ],
    "discipline_id": 216,
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
    "chapters_updated_at": "2016-11-09T13:41:19.981Z",
    "updated_at": "2016-11-09T13:41:21.484Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 63,
        "obfuscated_id": "k3ebr8XrqxE",
        "author_id": 641,
        "chapter_id": 151,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.274Z",
        "created_at": "2016-11-09T13:41:21.274Z",
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
        "author_id": 641,
        "chapter_id": 152,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.347Z",
        "created_at": "2016-11-09T13:41:21.347Z",
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
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 641,
        "chapter_id": 151,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.316Z",
        "created_at": "2016-11-09T13:41:21.316Z",
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
        "id": 66,
        "obfuscated_id": "H7dODBospvw",
        "author_id": 641,
        "chapter_id": 152,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.387Z",
        "created_at": "2016-11-09T13:41:21.387Z",
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
        "id": 67,
        "obfuscated_id": "btMCNJVyvlA",
        "author_id": 644,
        "chapter_id": 151,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.427Z",
        "created_at": "2016-11-09T13:41:21.427Z",
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
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 645,
        "chapter_id": 152,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-09T13:41:21.466Z",
        "created_at": "2016-11-09T13:41:21.466Z",
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
        "id": 151,
        "updated_at": "2016-11-09T13:41:21.438Z",
        "course_id": 211,
        "author_id": 641,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T13:41:19.981Z",
        "questions_updated_at": "2016-11-09T13:41:19.981Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 136",
        "position": 1
      },
      {
        "id": 152,
        "updated_at": "2016-11-09T13:41:21.477Z",
        "course_id": 211,
        "author_id": 641,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-09T13:41:19.981Z",
        "questions_updated_at": "2016-11-09T13:41:19.981Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 137",
        "position": 2
      }
    ],
    "topic_id": 215,
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
	-H "Authorization: Bearer f217b0187a67230c1be7401ac5c80f6c6ec8f278b20bfac2baa91cf51b575087"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/195
Content-Type: application/json
Authorization: Bearer 22fee0c51170c9eea925ace5ea5816e16675f6a15e9aa01897176080a698246c
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
    "creator_id": 601,
    "id": 195,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 179,
    "additional_university_ids": [

    ],
    "discipline_id": 200,
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
    "updated_at": "2016-11-09T13:41:13.908Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 199,
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
curl "api.goskive.com/v2/courses/195" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22fee0c51170c9eea925ace5ea5816e16675f6a15e9aa01897176080a698246c"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0be9a874ffd83c3b25c9cf2f25ec3f98ef437d4ce6261547fb1c36450f686b8f
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
    "creator_id": 606,
    "id": 198,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 182,
    "additional_university_ids": [

    ],
    "discipline_id": 203,
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
    "updated_at": "2016-11-09T13:41:14.901Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 202,
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
	-H "Authorization: Bearer 0be9a874ffd83c3b25c9cf2f25ec3f98ef437d4ce6261547fb1c36450f686b8f"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 9b3e453fd49f0b79d51be06c267274fcd6c1742764affdde17016d267fe096a2
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
      "user_id": 406,
      "feedbackable_id": 63,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:00.786Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 410,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:01.083Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 414,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:01.383Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 418,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:01.685Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 422,
      "feedbackable_id": 67,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T13:41:01.989Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b3e453fd49f0b79d51be06c267274fcd6c1742764affdde17016d267fe096a2"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 22709842a0736fc5bb176f19f167cfee195df5bfe72d340ac93eaa7107d0b0de
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
      "id": 22,
      "user_id": 401,
      "feedbackable_id": 62,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-09T13:41:00.456Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22709842a0736fc5bb176f19f167cfee195df5bfe72d340ac93eaa7107d0b0de"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 2c4f6167546b271ccc7297c004d7051430f32e8b2ea30779816eec0b9dfb8e29
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2c4f6167546b271ccc7297c004d7051430f32e8b2ea30779816eec0b9dfb8e29"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer 0efe240aa0fbb7d869b6c0c8712852837850050a7ea7f72184c8ed566be00087
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
      "id": 673,
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
      "created_at": "2016-11-09T13:41:24.672Z",
      "updated_at": "2016-11-09T13:41:24.672Z"
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
    "created_at": "2016-11-09T13:41:24.743Z",
    "updated_at": "2016-11-09T13:41:24.743Z",
    "course_id": 220,
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
	-H "Authorization: Bearer 0efe240aa0fbb7d869b6c0c8712852837850050a7ea7f72184c8ed566be00087"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/84/feedbacks
Content-Type: application/json
Authorization: Bearer e1469bcd0afcc5b15144b2d07c55e67cd8fa003bfa0eb271ef0434a7f26a3f47
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
      "id": 43,
      "user_id": 729,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:27.127Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 728,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:41:27.116Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e1469bcd0afcc5b15144b2d07c55e67cd8fa003bfa0eb271ef0434a7f26a3f47"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 23552e83ce3355e5eb3422dd0c1cfd447d89d9d78430899b387d798d24128ea0
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 283,
      "chapter_id": 62,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:53.216Z",
      "created_at": "2016-11-09T13:40:53.216Z",
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
      "author_id": 286,
      "chapter_id": 63,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:53.346Z",
      "created_at": "2016-11-09T13:40:53.346Z",
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 289,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:53.477Z",
      "created_at": "2016-11-09T13:40:53.477Z",
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 292,
      "chapter_id": 65,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:53.615Z",
      "created_at": "2016-11-09T13:40:53.615Z",
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
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 295,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:53.744Z",
      "created_at": "2016-11-09T13:40:53.744Z",
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
	-H "Authorization: Bearer 23552e83ce3355e5eb3422dd0c1cfd447d89d9d78430899b387d798d24128ea0"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 772a1b20e9b55a0c4d9a8f7efbb68f729410fd60b870f2164d1a4d127c891f7d
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 327,
      "chapter_id": 76,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:55.145Z",
      "created_at": "2016-11-09T13:40:55.145Z",
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
	-H "Authorization: Bearer 772a1b20e9b55a0c4d9a8f7efbb68f729410fd60b870f2164d1a4d127c891f7d"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/16/republish
Content-Type: application/json
Authorization: Bearer e8d7672d9ce694e020fda6eb77d875c688b6f76e8277e6e9f3b6b9e4f2c98cb9
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/16/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e8d7672d9ce694e020fda6eb77d875c688b6f76e8277e6e9f3b6b9e4f2c98cb9"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/5/feedbacks
Content-Type: application/json
Authorization: Bearer 95629c80313d1273e983895cca3d85a9b5733d5ecd08bf8d63feea25b85c2193
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
      "id": 6,
      "user_id": 33,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:40:27.371Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 32,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-09T13:40:27.361Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/5/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95629c80313d1273e983895cca3d85a9b5733d5ecd08bf8d63feea25b85c2193"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 9f7bc90746e609d772d8d9de8d330d9f047bb62b16348af8e76458b4912009bd
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 69,
      "chapter_id": 17,
      "position": 10,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:32.367Z",
      "created_at": "2016-11-09T13:40:32.244Z",
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
          "id": 31,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 32,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 72,
      "chapter_id": 18,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:32.676Z",
      "created_at": "2016-11-09T13:40:32.554Z",
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
          "id": 33,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 34,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 75,
      "chapter_id": 19,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:32.958Z",
      "created_at": "2016-11-09T13:40:32.832Z",
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
    },
    {
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 78,
      "chapter_id": 20,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:33.242Z",
      "created_at": "2016-11-09T13:40:33.116Z",
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
          "id": 37,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 38,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 81,
      "chapter_id": 21,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:33.523Z",
      "created_at": "2016-11-09T13:40:33.402Z",
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9f7bc90746e609d772d8d9de8d330d9f047bb62b16348af8e76458b4912009bd"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 7f9ae4ec88315197813867eb341e52d4f8f5a6e692751dce6203f1b06b04c013
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 97,
      "chapter_id": 26,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-09T13:40:35.010Z",
      "created_at": "2016-11-09T13:40:34.890Z",
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
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f9ae4ec88315197813867eb341e52d4f8f5a6e692751dce6203f1b06b04c013"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/10/republish
Content-Type: application/json
Authorization: Bearer 6899209618c69ef8f11545e7df1b0f01222572446753bb2838afd2b89005aa7f
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
	-H "Authorization: Bearer 6899209618c69ef8f11545e7df1b0f01222572446753bb2838afd2b89005aa7f"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 7463ef11540f2bd0e294fcf637622ec51f2a296d9a4ec1fcadcf7e0772acfddb
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":37,"published":false}}
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
    "creator_id": 129,
    "id": 37,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 37,
    "additional_university_ids": [

    ],
    "discipline_id": 37,
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
    "updated_at": "2016-11-09T13:40:39.219Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 37,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":37,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7463ef11540f2bd0e294fcf637622ec51f2a296d9a4ec1fcadcf7e0772acfddb"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer a0625bf75731e87fccccba05e1cd63bed6afc1cd663b7a4d08dffb8a2219bf32
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
      "creator_id": 152,
      "id": 56,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-52",
      "html_url": "https://goskive.com/course/fu-course-52",
      "slug": "fu-course-52",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "discipline_id": 56,
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
      "updated_at": "2016-11-09T13:40:41.432Z",
      "shortname": "fu-course-52",
      "topic_id": 56,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 52",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 152,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-53",
      "html_url": "https://goskive.com/course/fu-course-53",
      "slug": "fu-course-53",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "discipline_id": 57,
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
      "updated_at": "2016-11-09T13:40:41.468Z",
      "shortname": "fu-course-53",
      "topic_id": 57,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 53",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 153,
      "id": 58,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-54",
      "html_url": "https://goskive.com/course/fu-course-54",
      "slug": "fu-course-54",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "discipline_id": 58,
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
      "updated_at": "2016-11-09T13:40:41.514Z",
      "shortname": "fu-course-54",
      "topic_id": 58,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 54",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 153,
      "id": 59,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-55",
      "html_url": "https://goskive.com/course/fu-course-55",
      "slug": "fu-course-55",
      "university_id": 46,
      "additional_university_ids": [

      ],
      "discipline_id": 59,
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
      "chapters_updated_at": "2016-11-09T13:40:41.354Z",
      "updated_at": "2016-11-09T13:40:41.817Z",
      "shortname": "fu-course-55",
      "topic_id": 59,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 55",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0625bf75731e87fccccba05e1cd63bed6afc1cd663b7a4d08dffb8a2219bf32"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e769b56c9df49374d4a7fb471a97a409fa844cb511ad169589154b96f68de1b4
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
      "creator_id": 159,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-56",
      "html_url": "https://goskive.com/course/fu-course-56",
      "slug": "fu-course-56",
      "university_id": 48,
      "additional_university_ids": [

      ],
      "discipline_id": 60,
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
      "updated_at": "2016-11-09T13:40:42.001Z",
      "shortname": "fu-course-56",
      "topic_id": 60,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 56",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 159,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-57",
      "html_url": "https://goskive.com/course/fu-course-57",
      "slug": "fu-course-57",
      "university_id": 48,
      "additional_university_ids": [

      ],
      "discipline_id": 61,
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
      "updated_at": "2016-11-09T13:40:42.036Z",
      "shortname": "fu-course-57",
      "topic_id": 61,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 57",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 160,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-58",
      "html_url": "https://goskive.com/course/fu-course-58",
      "slug": "fu-course-58",
      "university_id": 48,
      "additional_university_ids": [

      ],
      "discipline_id": 62,
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
      "updated_at": "2016-11-09T13:40:42.078Z",
      "shortname": "fu-course-58",
      "topic_id": 62,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 58",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 160,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-59",
      "html_url": "https://goskive.com/course/fu-course-59",
      "slug": "fu-course-59",
      "university_id": 48,
      "additional_university_ids": [

      ],
      "discipline_id": 63,
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
      "updated_at": "2016-11-09T13:40:42.113Z",
      "shortname": "fu-course-59",
      "topic_id": 63,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 59",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e769b56c9df49374d4a7fb471a97a409fa844cb511ad169589154b96f68de1b4"
```
