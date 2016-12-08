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
DELETE /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 84166404b76b970a6cf83ab63c8b99dbdc937dbf01d6de18ee08d3553e966e9f
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/190" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 84166404b76b970a6cf83ab63c8b99dbdc937dbf01d6de18ee08d3553e966e9f"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/191
Content-Type: application/json
Authorization: Bearer 2242bf01d234af565f10af1510e0023f8ddc8e830b0a8f194d99f284c2760819
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
    "id": 191,
    "updated_at": "2016-12-08T09:10:45.806Z",
    "course_id": 309,
    "author_id": 955,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-08T09:10:45.337Z",
    "questions_updated_at": "2016-12-08T09:10:45.337Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 958,
        "chapter_id": 191,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:45.746Z",
        "created_at": "2016-12-08T09:10:45.746Z",
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
        "author_id": 959,
        "chapter_id": 191,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:45.788Z",
        "created_at": "2016-12-08T09:10:45.788Z",
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
        "id": 131,
        "obfuscated_id": "gCw8isdgMKE",
        "author_id": 956,
        "chapter_id": 191,
        "position": 118,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:45.525Z",
        "created_at": "2016-12-08T09:10:45.447Z",
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
            "id": 265,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 266,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 132,
        "obfuscated_id": "RECRPLqMrqE",
        "author_id": 957,
        "chapter_id": 191,
        "position": 119,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:10:45.679Z",
        "created_at": "2016-12-08T09:10:45.592Z",
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
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/191" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2242bf01d234af565f10af1510e0023f8ddc8e830b0a8f194d99f284c2760819"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/195
Content-Type: application/json
Authorization: Bearer c467ee48b64350f1af59d1f7f8ada8a5ccf845bcd038839d6e8d543518ba24c8
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
    "id": 195,
    "updated_at": "2016-12-08T09:10:46.887Z",
    "course_id": 313,
    "author_id": 974,
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
curl "api.goskive.com/v2/chapters/195" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c467ee48b64350f1af59d1f7f8ada8a5ccf845bcd038839d6e8d543518ba24c8"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/13
Content-Type: application/json
Authorization: Bearer 32b7f6aa782340e90aa5d4188242d70ab58494c642ac756f8f0a92256b1eb99e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 32b7f6aa782340e90aa5d4188242d70ab58494c642ac756f8f0a92256b1eb99e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a9ed77fc93f6063baf434c9395d88d06584de12e2a17bd48a64d2254e46c4d03
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
      "author_id": 521,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:13.737Z",
      "status": "published",
      "subject_id": 171,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 523,
      "reply_to_id": 16,
      "created_at": "2016-12-08T09:10:13.819Z",
      "status": "published",
      "subject_id": 172,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 525,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:13.901Z",
      "status": "published",
      "subject_id": 173,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 527,
      "reply_to_id": 18,
      "created_at": "2016-12-08T09:10:13.982Z",
      "status": "published",
      "subject_id": 174,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 529,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:14.064Z",
      "status": "reported",
      "subject_id": 175,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 531,
      "reply_to_id": 20,
      "created_at": "2016-12-08T09:10:14.145Z",
      "status": "published",
      "subject_id": 176,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 533,
      "reply_to_id": 20,
      "created_at": "2016-12-08T09:10:14.227Z",
      "status": "published",
      "subject_id": 177,
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
	-H "Authorization: Bearer a9ed77fc93f6063baf434c9395d88d06584de12e2a17bd48a64d2254e46c4d03"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d0e08481c5cf55d35624196a41eadce6e58802028d3408949f87846daf3427c5
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
      "id": 44,
      "author_id": 581,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:16.276Z",
      "status": "published",
      "subject_id": 199,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 583,
      "reply_to_id": 44,
      "created_at": "2016-12-08T09:10:16.356Z",
      "status": "published",
      "subject_id": 200,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 585,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:16.438Z",
      "status": "published",
      "subject_id": 201,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 587,
      "reply_to_id": 46,
      "created_at": "2016-12-08T09:10:16.522Z",
      "status": "published",
      "subject_id": 202,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 589,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:16.608Z",
      "status": "reported",
      "subject_id": 203,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 591,
      "reply_to_id": 48,
      "created_at": "2016-12-08T09:10:16.691Z",
      "status": "published",
      "subject_id": 204,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 593,
      "reply_to_id": 48,
      "created_at": "2016-12-08T09:10:16.774Z",
      "status": "published",
      "subject_id": 205,
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
	-H "Authorization: Bearer d0e08481c5cf55d35624196a41eadce6e58802028d3408949f87846daf3427c5"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 3a7f1ec2ef171a5d968c53035e64d0cb0ed7de47217c371ca0d1032a287d0bb7
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
      "author_id": 553,
      "reply_to_id": 30,
      "created_at": "2016-12-08T09:10:15.078Z",
      "status": "published",
      "subject_id": 186,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 557,
      "reply_to_id": 32,
      "created_at": "2016-12-08T09:10:15.242Z",
      "status": "published",
      "subject_id": 188,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 561,
      "reply_to_id": 34,
      "created_at": "2016-12-08T09:10:15.436Z",
      "status": "published",
      "subject_id": 190,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 563,
      "reply_to_id": 34,
      "created_at": "2016-12-08T09:10:15.518Z",
      "status": "published",
      "subject_id": 191,
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
	-H "Authorization: Bearer 3a7f1ec2ef171a5d968c53035e64d0cb0ed7de47217c371ca0d1032a287d0bb7"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer d08e94e794b6870f76ae102a62596c37b87f234c015b3bf051f4903281a5fd4d
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
      "id": 27,
      "author_id": 544,
      "reply_to_id": null,
      "created_at": "2016-12-08T09:10:14.707Z",
      "status": "reported",
      "subject_id": 182,
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
	-H "Authorization: Bearer d08e94e794b6870f76ae102a62596c37b87f234c015b3bf051f4903281a5fd4d"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/11/republish
Content-Type: application/json
Authorization: Bearer 91bb32b363b60f88cf7bb4c2194046b6a8521f04ead492aaa18e3f3254e7f0c0
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91bb32b363b60f88cf7bb4c2194046b6a8521f04ead492aaa18e3f3254e7f0c0"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b599f015d7dbcc39d34d2f830897fe07bc89c9306b76b9414a0616b6c9b039a0
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
    "id": 151,
    "updated_at": "2016-12-08T09:10:36.918Z",
    "course_id": 272,
    "author_id": 823,
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
	-H "Authorization: Bearer b599f015d7dbcc39d34d2f830897fe07bc89c9306b76b9414a0616b6c9b039a0"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/274/chapters
Content-Type: application/json
Authorization: Bearer 4da7560bf04705ef969a23eae82123e9e969f5e6cc2de9fa3775c5ad76e32198
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
    "id": 153,
    "updated_at": "2016-12-08T09:10:37.209Z",
    "course_id": 274,
    "author_id": 827,
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
curl "api.goskive.com/v2/courses/274/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4da7560bf04705ef969a23eae82123e9e969f5e6cc2de9fa3775c5ad76e32198"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b56a0e91e6001fbe0cad2b40b7f3a73e686c516ff1b87ba43b84dde54ca7ebeb
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
      "id": 157,
      "updated_at": "2016-12-08T09:10:37.695Z",
      "course_id": 277,
      "author_id": 836,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 142",
      "position": 1
    },
    {
      "id": 158,
      "updated_at": "2016-12-08T09:10:37.722Z",
      "course_id": 277,
      "author_id": 837,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 143",
      "position": 2
    },
    {
      "id": 159,
      "updated_at": "2016-12-08T09:10:37.945Z",
      "course_id": 277,
      "author_id": 838,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-08T09:10:37.620Z",
      "questions_updated_at": "2016-12-08T09:10:37.620Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 144",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b56a0e91e6001fbe0cad2b40b7f3a73e686c516ff1b87ba43b84dde54ca7ebeb"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 19fb7d0353b2cb39a0a947bd0495f70688e311bab1249f63acf4131cd6da80fe
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
      "id": 160,
      "updated_at": "2016-12-08T09:10:38.102Z",
      "course_id": 278,
      "author_id": 843,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 145",
      "position": 1
    },
    {
      "id": 161,
      "updated_at": "2016-12-08T09:10:38.128Z",
      "course_id": 278,
      "author_id": 844,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 146",
      "position": 2
    },
    {
      "id": 162,
      "updated_at": "2016-12-08T09:10:38.156Z",
      "course_id": 278,
      "author_id": 845,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 147",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19fb7d0353b2cb39a0a947bd0495f70688e311bab1249f63acf4131cd6da80fe"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a54009718769e92d2919f34401a6944bf3fb180043614864e2d66b6b762dec9c
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
	-H "Authorization: Bearer a54009718769e92d2919f34401a6944bf3fb180043614864e2d66b6b762dec9c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/19
Content-Type: application/json
Authorization: Bearer 1c6e2a883588fbddca797f2ef9368091c750bc9f528c3315060f166ce77b7d68
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c6e2a883588fbddca797f2ef9368091c750bc9f528c3315060f166ce77b7d68"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 593b741df25e569b2ee5425dc20afbe65d1f97ea69e6be65935e01a27212d84f
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
    "creator_id": 4,
    "id": 1,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 1,
    "additional_university_ids": [

    ],
    "discipline_id": 4,
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
    "chapters_updated_at": "2016-12-08T09:09:28.523Z",
    "updated_at": "2016-12-08T09:09:30.134Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 4,
        "chapter_id": 1,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:29.903Z",
        "created_at": "2016-12-08T09:09:29.903Z",
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
        "id": 3,
        "obfuscated_id": "bco7bNtr_d4",
        "author_id": 4,
        "chapter_id": 2,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:29.984Z",
        "created_at": "2016-12-08T09:09:29.984Z",
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
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 4,
        "chapter_id": 1,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:29.949Z",
        "created_at": "2016-12-08T09:09:29.949Z",
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
        "author_id": 4,
        "chapter_id": 2,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:30.028Z",
        "created_at": "2016-12-08T09:09:30.028Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 7,
        "chapter_id": 1,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:30.070Z",
        "created_at": "2016-12-08T09:09:30.070Z",
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
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 8,
        "chapter_id": 2,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-08T09:09:30.113Z",
        "created_at": "2016-12-08T09:09:30.113Z",
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
        "id": 1,
        "updated_at": "2016-12-08T09:09:30.081Z",
        "course_id": 1,
        "author_id": 4,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T09:09:28.523Z",
        "questions_updated_at": "2016-12-08T09:09:28.523Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 1",
        "position": 1
      },
      {
        "id": 2,
        "updated_at": "2016-12-08T09:09:30.124Z",
        "course_id": 1,
        "author_id": 4,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-08T09:09:28.523Z",
        "questions_updated_at": "2016-12-08T09:09:28.523Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 2",
        "position": 2
      }
    ],
    "topic_id": 3,
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
	-H "Authorization: Bearer 593b741df25e569b2ee5425dc20afbe65d1f97ea69e6be65935e01a27212d84f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/8
Content-Type: application/json
Authorization: Bearer bcac82893ff36da521b1e380effed6ccf07464a7feb7c5325e0a5169a545b288
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
    "creator_id": 32,
    "id": 8,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 8,
    "additional_university_ids": [

    ],
    "discipline_id": 11,
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
    "updated_at": "2016-12-08T09:09:35.061Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 10,
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
curl "api.goskive.com/v2/courses/8" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bcac82893ff36da521b1e380effed6ccf07464a7feb7c5325e0a5169a545b288"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 688542cc511429e8a6358b41039008c12d2382957ea631c1b0e098d004fa2e99
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
    "creator_id": 29,
    "id": 6,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 6,
    "additional_university_ids": [

    ],
    "discipline_id": 9,
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
    "updated_at": "2016-12-08T09:09:34.739Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 8,
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
	-H "Authorization: Bearer 688542cc511429e8a6358b41039008c12d2382957ea631c1b0e098d004fa2e99"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 47663e25ce63fa1e328f6b71679685ba219c286355b069a04afb968a48f92236
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
      "user_id": 370,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:04.468Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 374,
      "feedbackable_id": 78,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:04.767Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 378,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:05.062Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 382,
      "feedbackable_id": 80,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:05.362Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 386,
      "feedbackable_id": 81,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T09:10:05.660Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47663e25ce63fa1e328f6b71679685ba219c286355b069a04afb968a48f92236"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer f6f69bb51d01161a0246d612877e553993850bcc32e9b2075cbde7aca3569b41
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
      "id": 33,
      "user_id": 407,
      "feedbackable_id": 86,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-08T09:10:07.207Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f6f69bb51d01161a0246d612877e553993850bcc32e9b2075cbde7aca3569b41"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer cb832e88f350535dc7e398947a37b4f5bc1aa3918ce0ed2cecaed3c1a635e745
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cb832e88f350535dc7e398947a37b4f5bc1aa3918ce0ed2cecaed3c1a635e745"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/17/metadata
Content-Type: application/json
Authorization: Bearer e2da798cafd0d36f904dc9b652d1c551b0f3f4c7bc337b317d229728a61b3ea4
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
    "id": 17,
    "uploader": {
      "id": 711,
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
      "created_at": "2016-12-08T09:10:25.984Z",
      "updated_at": "2016-12-08T09:10:25.984Z"
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
    "created_at": "2016-12-08T09:10:26.057Z",
    "updated_at": "2016-12-08T09:10:26.057Z",
    "course_id": 239,
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
curl "api.goskive.com/v2/files/17/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2da798cafd0d36f904dc9b652d1c551b0f3f4c7bc337b317d229728a61b3ea4"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/87/feedbacks
Content-Type: application/json
Authorization: Bearer 1ad0008897321485e31fe269b01a1e4f459160c346a725c8cbaca0b88e538d43
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
      "user_id": 905,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:42.254Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 904,
      "feedbackable_id": 87,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:10:42.243Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/87/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ad0008897321485e31fe269b01a1e4f459160c346a725c8cbaca0b88e538d43"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 6b884a6a97eda1ba8da0c7a9ee8072bef066f2d2f3ee5132f1d72216a856376a
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 486,
      "chapter_id": 97,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:11.965Z",
      "created_at": "2016-12-08T09:10:11.965Z",
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
      "author_id": 489,
      "chapter_id": 98,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:12.101Z",
      "created_at": "2016-12-08T09:10:12.101Z",
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 492,
      "chapter_id": 99,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:12.237Z",
      "created_at": "2016-12-08T09:10:12.237Z",
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
      "author_id": 495,
      "chapter_id": 100,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:12.373Z",
      "created_at": "2016-12-08T09:10:12.373Z",
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
      "author_id": 498,
      "chapter_id": 101,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:12.511Z",
      "created_at": "2016-12-08T09:10:12.511Z",
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
	-H "Authorization: Bearer 6b884a6a97eda1ba8da0c7a9ee8072bef066f2d2f3ee5132f1d72216a856376a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer aef3949e9401acf36c408eb0fbe67571e1cf10bc44414356354aad7c035fef0b
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
      "id": 55,
      "obfuscated_id": "VX19tR4fHZ8",
      "author_id": 466,
      "chapter_id": 91,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:11.060Z",
      "created_at": "2016-12-08T09:10:11.060Z",
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
	-H "Authorization: Bearer aef3949e9401acf36c408eb0fbe67571e1cf10bc44414356354aad7c035fef0b"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/45/republish
Content-Type: application/json
Authorization: Bearer 31b0ea5da1aff3b05d90f9a4252d4d15bd9c0c310034a5807d162cd3a64352fb
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/45/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31b0ea5da1aff3b05d90f9a4252d4d15bd9c0c310034a5807d162cd3a64352fb"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/33/feedbacks
Content-Type: application/json
Authorization: Bearer da9704b90b423588e1648ae048dc025686655357bd25fcef65acc90cf44a0f8b
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
      "id": 4,
      "user_id": 99,
      "feedbackable_id": 33,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:09:40.735Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 98,
      "feedbackable_id": 33,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-08T09:09:40.724Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/33/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer da9704b90b423588e1648ae048dc025686655357bd25fcef65acc90cf44a0f8b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 654b2f9827d1f5921e5ab8246036da5df966fb356cfcb93b6b44c834ce098c37
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
      "id": 108,
      "obfuscated_id": "3MKez0MLRBM",
      "author_id": 770,
      "chapter_id": 137,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:30.947Z",
      "created_at": "2016-12-08T09:10:30.862Z",
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
    },
    {
      "id": 109,
      "obfuscated_id": "VSPyck5c2RY",
      "author_id": 773,
      "chapter_id": 138,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:31.187Z",
      "created_at": "2016-12-08T09:10:31.100Z",
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
          "id": 220,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 221,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 110,
      "obfuscated_id": "55JK4PuG2Hk",
      "author_id": 776,
      "chapter_id": 139,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:31.423Z",
      "created_at": "2016-12-08T09:10:31.337Z",
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
          "id": 222,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 223,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 111,
      "obfuscated_id": "G-D-sgMUtTw",
      "author_id": 779,
      "chapter_id": 140,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:31.665Z",
      "created_at": "2016-12-08T09:10:31.577Z",
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
          "id": 224,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 225,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 112,
      "obfuscated_id": "7Qwj1ZvbWUI",
      "author_id": 782,
      "chapter_id": 141,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:31.904Z",
      "created_at": "2016-12-08T09:10:31.823Z",
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
          "id": 226,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 227,
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
	-H "Authorization: Bearer 654b2f9827d1f5921e5ab8246036da5df966fb356cfcb93b6b44c834ce098c37"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9722a716a8a6268f76425f062821f46794a025149aa08d677cd499fd7fcb2e40
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
      "id": 107,
      "obfuscated_id": "_2rgp7tgq8o",
      "author_id": 766,
      "chapter_id": 136,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-08T09:10:30.656Z",
      "created_at": "2016-12-08T09:10:30.576Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9722a716a8a6268f76425f062821f46794a025149aa08d677cd499fd7fcb2e40"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/99/republish
Content-Type: application/json
Authorization: Bearer 3a2c9a68ca2ebb24cc6d807ec886f3f9bba69b2a7aeb7236e76c89cbfa82d5f1
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/99/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a2c9a68ca2ebb24cc6d807ec886f3f9bba69b2a7aeb7236e76c89cbfa82d5f1"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c542014625f14cd484c44e13b0c1d0449936ccca08d5ecf2e5c24e00be24a0c1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":110,"published":false}}
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
    "creator_id": 272,
    "id": 103,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 88,
    "additional_university_ids": [

    ],
    "discipline_id": 111,
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
    "updated_at": "2016-12-08T09:09:56.906Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 110,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":110,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c542014625f14cd484c44e13b0c1d0449936ccca08d5ecf2e5c24e00be24a0c1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1e98bcf6bb4789ffdb5def0980e4df742df8bf0be3d94212d8fa60406f3bcb5e
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
      "creator_id": 262,
      "id": 95,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-64",
      "html_url": "https://goskive.com/course/fu-course-64",
      "slug": "fu-course-64",
      "university_id": 85,
      "additional_university_ids": [

      ],
      "discipline_id": 103,
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
      "updated_at": "2016-12-08T09:09:55.963Z",
      "shortname": "fu-course-64",
      "topic_id": 102,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 64",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 262,
      "id": 96,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-65",
      "html_url": "https://goskive.com/course/fu-course-65",
      "slug": "fu-course-65",
      "university_id": 85,
      "additional_university_ids": [

      ],
      "discipline_id": 104,
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
      "updated_at": "2016-12-08T09:09:55.998Z",
      "shortname": "fu-course-65",
      "topic_id": 103,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 65",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 263,
      "id": 97,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-66",
      "html_url": "https://goskive.com/course/fu-course-66",
      "slug": "fu-course-66",
      "university_id": 85,
      "additional_university_ids": [

      ],
      "discipline_id": 105,
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
      "updated_at": "2016-12-08T09:09:56.041Z",
      "shortname": "fu-course-66",
      "topic_id": 104,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 66",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 263,
      "id": 98,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-67",
      "html_url": "https://goskive.com/course/fu-course-67",
      "slug": "fu-course-67",
      "university_id": 85,
      "additional_university_ids": [

      ],
      "discipline_id": 106,
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
      "chapters_updated_at": "2016-12-08T09:09:55.908Z",
      "updated_at": "2016-12-08T09:09:56.337Z",
      "shortname": "fu-course-67",
      "topic_id": 105,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 67",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e98bcf6bb4789ffdb5def0980e4df742df8bf0be3d94212d8fa60406f3bcb5e"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 226f587d9f5e484fc31022b179a7ad4f65d1f4835dbf0a58aba8526e07c36773
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
      "creator_id": 268,
      "id": 99,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-68",
      "html_url": "https://goskive.com/course/fu-course-68",
      "slug": "fu-course-68",
      "university_id": 86,
      "additional_university_ids": [

      ],
      "discipline_id": 107,
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
      "updated_at": "2016-12-08T09:09:56.504Z",
      "shortname": "fu-course-68",
      "topic_id": 106,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 68",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 268,
      "id": 100,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-69",
      "html_url": "https://goskive.com/course/fu-course-69",
      "slug": "fu-course-69",
      "university_id": 86,
      "additional_university_ids": [

      ],
      "discipline_id": 108,
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
      "updated_at": "2016-12-08T09:09:56.539Z",
      "shortname": "fu-course-69",
      "topic_id": 107,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 69",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 269,
      "id": 101,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-70",
      "html_url": "https://goskive.com/course/fu-course-70",
      "slug": "fu-course-70",
      "university_id": 86,
      "additional_university_ids": [

      ],
      "discipline_id": 109,
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
      "updated_at": "2016-12-08T09:09:56.583Z",
      "shortname": "fu-course-70",
      "topic_id": 108,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 70",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 269,
      "id": 102,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-71",
      "html_url": "https://goskive.com/course/fu-course-71",
      "slug": "fu-course-71",
      "university_id": 86,
      "additional_university_ids": [

      ],
      "discipline_id": 110,
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
      "updated_at": "2016-12-08T09:09:56.618Z",
      "shortname": "fu-course-71",
      "topic_id": 109,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 71",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 226f587d9f5e484fc31022b179a7ad4f65d1f4835dbf0a58aba8526e07c36773"
```
