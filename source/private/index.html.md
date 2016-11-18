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
DELETE /v2/chapters/57
Content-Type: application/json
Authorization: Bearer 28d8773673f5e6679e54f64b6d51ea9ca96912c1440fa24c1fdd59e4e7937fc8
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 28d8773673f5e6679e54f64b6d51ea9ca96912c1440fa24c1fdd59e4e7937fc8"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/54
Content-Type: application/json
Authorization: Bearer 2d134f172bc9b4fc25fb0c49c1776ef315abb31952ada9c13026d23d2de01261
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
    "id": 54,
    "updated_at": "2016-11-18T09:48:05.915Z",
    "course_id": 110,
    "author_id": 295,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-18T09:48:05.269Z",
    "questions_updated_at": "2016-11-18T09:48:05.269Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 298,
        "chapter_id": 54,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:05.851Z",
        "created_at": "2016-11-18T09:48:05.851Z",
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
        "id": 24,
        "obfuscated_id": "KHM5yo_z4Ds",
        "author_id": 299,
        "chapter_id": 54,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:05.893Z",
        "created_at": "2016-11-18T09:48:05.893Z",
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
        "id": 39,
        "obfuscated_id": "N0Vv2_jrTfU",
        "author_id": 296,
        "chapter_id": 54,
        "position": 35,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:05.525Z",
        "created_at": "2016-11-18T09:48:05.384Z",
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
            "id": 80,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 81,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 297,
        "chapter_id": 54,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:05.767Z",
        "created_at": "2016-11-18T09:48:05.612Z",
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
            "id": 82,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 83,
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
curl "api.goskive.com/v2/chapters/54" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d134f172bc9b4fc25fb0c49c1776ef315abb31952ada9c13026d23d2de01261"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/51
Content-Type: application/json
Authorization: Bearer 8e8599959222e38dfd1ba904d09f1df6df5f5808d7bda529c5c2a115ad6fe0db
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
    "id": 51,
    "updated_at": "2016-11-18T09:48:04.849Z",
    "course_id": 107,
    "author_id": 287,
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
curl "api.goskive.com/v2/chapters/51" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8e8599959222e38dfd1ba904d09f1df6df5f5808d7bda529c5c2a115ad6fe0db"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/16
Content-Type: application/json
Authorization: Bearer 5c012cf99c119752b14d18722af1a19f9be15d06330a93bb782a7f4d157dd024
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5c012cf99c119752b14d18722af1a19f9be15d06330a93bb782a7f4d157dd024"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 547e58cc5935ece71e9774a5359d1b58cc27ec1d321faaaa772f54a97c513c05
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
      "id": 21,
      "author_id": 384,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:13.122Z",
      "status": "published",
      "subject_id": 135,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 386,
      "reply_to_id": 21,
      "created_at": "2016-11-18T09:48:13.209Z",
      "status": "published",
      "subject_id": 136,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 388,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:13.298Z",
      "status": "published",
      "subject_id": 137,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 390,
      "reply_to_id": 23,
      "created_at": "2016-11-18T09:48:13.384Z",
      "status": "published",
      "subject_id": 138,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 392,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:13.475Z",
      "status": "reported",
      "subject_id": 139,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 394,
      "reply_to_id": 25,
      "created_at": "2016-11-18T09:48:13.562Z",
      "status": "published",
      "subject_id": 140,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 396,
      "reply_to_id": 25,
      "created_at": "2016-11-18T09:48:13.649Z",
      "status": "published",
      "subject_id": 141,
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
	-H "Authorization: Bearer 547e58cc5935ece71e9774a5359d1b58cc27ec1d321faaaa772f54a97c513c05"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer cd6731f2a0264bbc7523837557b73782dc37d25eb2670e8f7a655e032197538a
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
      "author_id": 399,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:13.799Z",
      "status": "published",
      "subject_id": 142,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 401,
      "reply_to_id": 28,
      "created_at": "2016-11-18T09:48:13.888Z",
      "status": "published",
      "subject_id": 143,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 403,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:13.976Z",
      "status": "published",
      "subject_id": 144,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 405,
      "reply_to_id": 30,
      "created_at": "2016-11-18T09:48:14.063Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 407,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:14.152Z",
      "status": "reported",
      "subject_id": 146,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 409,
      "reply_to_id": 32,
      "created_at": "2016-11-18T09:48:14.239Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 411,
      "reply_to_id": 32,
      "created_at": "2016-11-18T09:48:14.327Z",
      "status": "published",
      "subject_id": 148,
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
	-H "Authorization: Bearer cd6731f2a0264bbc7523837557b73782dc37d25eb2670e8f7a655e032197538a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 92b3eb53bfaa533bd1e1473a7b391ebef6e1d3e166ebb1a62eca02426817f9d6
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
      "id": 43,
      "author_id": 431,
      "reply_to_id": 42,
      "created_at": "2016-11-18T09:48:15.215Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 435,
      "reply_to_id": 44,
      "created_at": "2016-11-18T09:48:15.416Z",
      "status": "published",
      "subject_id": 159,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 439,
      "reply_to_id": 46,
      "created_at": "2016-11-18T09:48:15.588Z",
      "status": "published",
      "subject_id": 161,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 441,
      "reply_to_id": 46,
      "created_at": "2016-11-18T09:48:15.675Z",
      "status": "published",
      "subject_id": 162,
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
	-H "Authorization: Bearer 92b3eb53bfaa533bd1e1473a7b391ebef6e1d3e166ebb1a62eca02426817f9d6"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer d5cabff4d6e0b86cddccf2acc1e89434dcb3e468e9d1375e62d7756b38da2e84
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
      "id": 53,
      "author_id": 452,
      "reply_to_id": null,
      "created_at": "2016-11-18T09:48:16.164Z",
      "status": "reported",
      "subject_id": 167,
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
	-H "Authorization: Bearer d5cabff4d6e0b86cddccf2acc1e89434dcb3e468e9d1375e62d7756b38da2e84"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/19/republish
Content-Type: application/json
Authorization: Bearer df55df74fa09ba7f4f459f2432185e45ee714e475cf4fc319fe3a0ace9b7166d
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/19/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df55df74fa09ba7f4f459f2432185e45ee714e475cf4fc319fe3a0ace9b7166d"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/186/chapters
Content-Type: application/json
Authorization: Bearer 3cd3c1b161bd4bcd8bacb9e1d5a81a6bcf75e1ed1fdaf3f40f346f957874609c
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
    "updated_at": "2016-11-18T09:48:20.940Z",
    "course_id": 186,
    "author_id": 527,
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
curl "api.goskive.com/v2/courses/186/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3cd3c1b161bd4bcd8bacb9e1d5a81a6bcf75e1ed1fdaf3f40f346f957874609c"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f438cbd20111a60e4b55d0c71409abf8598bea76406174d98a8441513c3f3ee3
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
    "id": 93,
    "updated_at": "2016-11-18T09:48:21.122Z",
    "course_id": 187,
    "author_id": 529,
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
	-H "Authorization: Bearer f438cbd20111a60e4b55d0c71409abf8598bea76406174d98a8441513c3f3ee3"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 26ab25b1d671c0542298ac259053e642de080bb1e300479b5189e1ec58f12199
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
      "id": 77,
      "updated_at": "2016-11-18T09:48:18.991Z",
      "course_id": 178,
      "author_id": 495,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 56",
      "position": 1
    },
    {
      "id": 78,
      "updated_at": "2016-11-18T09:48:19.019Z",
      "course_id": 178,
      "author_id": 496,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 57",
      "position": 2
    },
    {
      "id": 79,
      "updated_at": "2016-11-18T09:48:19.347Z",
      "course_id": 178,
      "author_id": 497,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-18T09:48:18.914Z",
      "questions_updated_at": "2016-11-18T09:48:18.914Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 58",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 26ab25b1d671c0542298ac259053e642de080bb1e300479b5189e1ec58f12199"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8274db6a99dee4425516de4f369bfe8a8a249bf1efe3d847b9dd2d2a30c69e27
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
      "id": 80,
      "updated_at": "2016-11-18T09:48:19.503Z",
      "course_id": 179,
      "author_id": 502,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 59",
      "position": 1
    },
    {
      "id": 81,
      "updated_at": "2016-11-18T09:48:19.532Z",
      "course_id": 179,
      "author_id": 503,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 60",
      "position": 2
    },
    {
      "id": 82,
      "updated_at": "2016-11-18T09:48:19.560Z",
      "course_id": 179,
      "author_id": 504,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 61",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8274db6a99dee4425516de4f369bfe8a8a249bf1efe3d847b9dd2d2a30c69e27"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/296
Content-Type: application/json
Authorization: Bearer f087f154ec84016c0ffede3ec29fc84cc0be6b2e230692a6dfecc6d5e27a99a8
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/296" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f087f154ec84016c0ffede3ec29fc84cc0be6b2e230692a6dfecc6d5e27a99a8"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 618d650bb404a32c3326c90d561c43c06131f7f183252b1296efdb28ac61923d
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
	-H "Authorization: Bearer 618d650bb404a32c3326c90d561c43c06131f7f183252b1296efdb28ac61923d"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4dfe298cfcccc0f297cefa9db5b058972094ad001b6ff60b984736655ec8b165
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
    "creator_id": 896,
    "id": 287,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 272,
    "additional_university_ids": [

    ],
    "discipline_id": 300,
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
    "chapters_updated_at": "2016-11-18T09:48:54.000Z",
    "updated_at": "2016-11-18T09:48:55.539Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 76,
        "obfuscated_id": "oK0h_-4yfUk",
        "author_id": 896,
        "chapter_id": 180,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.318Z",
        "created_at": "2016-11-18T09:48:55.318Z",
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
        "author_id": 896,
        "chapter_id": 181,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.395Z",
        "created_at": "2016-11-18T09:48:55.395Z",
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
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 896,
        "chapter_id": 180,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.361Z",
        "created_at": "2016-11-18T09:48:55.361Z",
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
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 896,
        "chapter_id": 181,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.437Z",
        "created_at": "2016-11-18T09:48:55.437Z",
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
        "author_id": 899,
        "chapter_id": 180,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.477Z",
        "created_at": "2016-11-18T09:48:55.477Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 900,
        "chapter_id": 181,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T09:48:55.519Z",
        "created_at": "2016-11-18T09:48:55.519Z",
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
        "id": 180,
        "updated_at": "2016-11-18T09:48:55.488Z",
        "course_id": 287,
        "author_id": 896,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-18T09:48:54.000Z",
        "questions_updated_at": "2016-11-18T09:48:54.000Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 156",
        "position": 1
      },
      {
        "id": 181,
        "updated_at": "2016-11-18T09:48:55.530Z",
        "course_id": 287,
        "author_id": 896,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-18T09:48:54.000Z",
        "questions_updated_at": "2016-11-18T09:48:54.000Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 157",
        "position": 2
      }
    ],
    "topic_id": 299,
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
	-H "Authorization: Bearer 4dfe298cfcccc0f297cefa9db5b058972094ad001b6ff60b984736655ec8b165"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/295
Content-Type: application/json
Authorization: Bearer 160c8fe5654f4b9bf16d2e4119d103adc4920413f5f9e4392987e4e93129f2a1
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
    "creator_id": 923,
    "id": 295,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 280,
    "additional_university_ids": [

    ],
    "discipline_id": 308,
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
    "updated_at": "2016-11-18T09:48:59.777Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 307,
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
curl "api.goskive.com/v2/courses/295" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 160c8fe5654f4b9bf16d2e4119d103adc4920413f5f9e4392987e4e93129f2a1"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer b47689f182a9159fcef0faf20632473b08af17246045e4fd130d3924315e879c
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
    "creator_id": 918,
    "id": 292,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 277,
    "additional_university_ids": [

    ],
    "discipline_id": 305,
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
    "updated_at": "2016-11-18T09:48:59.337Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 304,
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
	-H "Authorization: Bearer b47689f182a9159fcef0faf20632473b08af17246045e4fd130d3924315e879c"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer c2e7fd0fd929696b95710040561c118527d10f69481e58b023873f5e5f8d9ab5
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
      "user_id": 597,
      "feedbackable_id": 62,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:48:26.547Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 601,
      "feedbackable_id": 63,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:48:26.930Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 30,
      "user_id": 605,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:48:27.314Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 609,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:48:27.699Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 613,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-18T09:48:28.092Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2e7fd0fd929696b95710040561c118527d10f69481e58b023873f5e5f8d9ab5"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer fc73e6b0a5effb4628e80e3f8dfa8e17d680b561995d2df6bcd8d439f2b581b4
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
      "user_id": 634,
      "feedbackable_id": 71,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-18T09:48:30.128Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fc73e6b0a5effb4628e80e3f8dfa8e17d680b561995d2df6bcd8d439f2b581b4"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer f9b3bdce30465d34b902dabb5b03ed624811ccd851c4ce3aa3fae90b10bd5f04
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
	-H "Authorization: Bearer f9b3bdce30465d34b902dabb5b03ed624811ccd851c4ce3aa3fae90b10bd5f04"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/2/metadata
Content-Type: application/json
Authorization: Bearer e9b13df9952176bf8fbf0a5a1a270202165da6444ccd91854346829f288ce728
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
    "id": 2,
    "uploader": {
      "id": 195,
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
      "created_at": "2016-11-18T09:47:54.656Z",
      "updated_at": "2016-11-18T09:47:54.656Z"
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
    "created_at": "2016-11-18T09:47:54.732Z",
    "updated_at": "2016-11-18T09:47:54.732Z",
    "course_id": 82,
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
curl "api.goskive.com/v2/files/2/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9b13df9952176bf8fbf0a5a1a270202165da6444ccd91854346829f288ce728"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/17/feedbacks
Content-Type: application/json
Authorization: Bearer 7a81fd1b33b6af8be4fdeb6ecbb5058528bf5f6487fb5332f7a6722dc6943855
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
      "id": 10,
      "user_id": 152,
      "feedbackable_id": 17,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:50.817Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 151,
      "feedbackable_id": 17,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:50.806Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/17/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7a81fd1b33b6af8be4fdeb6ecbb5058528bf5f6487fb5332f7a6722dc6943855"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer c7d382009a9ae08a81f23bf72dffae602d5da59ec1f0e11530453fa9b1cef877
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
      "author_id": 741,
      "chapter_id": 138,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:36.722Z",
      "created_at": "2016-11-18T09:48:36.722Z",
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
      "author_id": 744,
      "chapter_id": 139,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:36.862Z",
      "created_at": "2016-11-18T09:48:36.862Z",
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
      "author_id": 747,
      "chapter_id": 140,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:36.999Z",
      "created_at": "2016-11-18T09:48:36.999Z",
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
      "author_id": 750,
      "chapter_id": 141,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:37.137Z",
      "created_at": "2016-11-18T09:48:37.137Z",
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
      "author_id": 753,
      "chapter_id": 142,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:37.279Z",
      "created_at": "2016-11-18T09:48:37.279Z",
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
	-H "Authorization: Bearer c7d382009a9ae08a81f23bf72dffae602d5da59ec1f0e11530453fa9b1cef877"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 07aa95b4eab4c79e0e6f5ae0af898df9384725d5982aa601976bdbc6a86e18a9
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 721,
      "chapter_id": 132,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:35.804Z",
      "created_at": "2016-11-18T09:48:35.804Z",
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
	-H "Authorization: Bearer 07aa95b4eab4c79e0e6f5ae0af898df9384725d5982aa601976bdbc6a86e18a9"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/66/republish
Content-Type: application/json
Authorization: Bearer 232d5284c91a046facb9d2e809c7ece086f1c3dd45447f26d03473cfac9f5e47
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/66/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 232d5284c91a046facb9d2e809c7ece086f1c3dd45447f26d03473cfac9f5e47"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/21/feedbacks
Content-Type: application/json
Authorization: Bearer a1e5ba0a93e82af048d4e50c25a54aeddee934a796f24f734632bd014fcc35f8
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
      "user_id": 182,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:53.024Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 15,
      "user_id": 181,
      "feedbackable_id": 21,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T09:47:53.013Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/21/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a1e5ba0a93e82af048d4e50c25a54aeddee934a796f24f734632bd014fcc35f8"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer d576cb46a57a35f423c9deb6244a9a90d4de0bd5de8a4b9b94ce108bf9464e38
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
      "author_id": 848,
      "chapter_id": 164,
      "position": 82,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:47.016Z",
      "created_at": "2016-11-18T09:48:46.886Z",
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
      "id": 86,
      "obfuscated_id": "7q-2LHZR3Kk",
      "author_id": 839,
      "chapter_id": 161,
      "position": 79,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:46.104Z",
      "created_at": "2016-11-18T09:48:45.979Z",
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
          "id": 174,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 175,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 842,
      "chapter_id": 162,
      "position": 80,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:46.407Z",
      "created_at": "2016-11-18T09:48:46.280Z",
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
          "id": 176,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 177,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 845,
      "chapter_id": 163,
      "position": 81,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:46.712Z",
      "created_at": "2016-11-18T09:48:46.581Z",
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
          "id": 178,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 179,
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
      "author_id": 851,
      "chapter_id": 165,
      "position": 83,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:47.347Z",
      "created_at": "2016-11-18T09:48:47.226Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d576cb46a57a35f423c9deb6244a9a90d4de0bd5de8a4b9b94ce108bf9464e38"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer dbca20a9928c7a1e6c7699f53c3620d6828c2d391678c7383c5f1f6677321247
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
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 835,
      "chapter_id": 160,
      "position": 78,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T09:48:45.749Z",
      "created_at": "2016-11-18T09:48:45.627Z",
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
          "id": 172,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 173,
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
	-H "Authorization: Bearer dbca20a9928c7a1e6c7699f53c3620d6828c2d391678c7383c5f1f6677321247"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/97/republish
Content-Type: application/json
Authorization: Bearer af0e72599265ae261077619cf0470e81f8cf707447fbd7b9ad2cbdb0d23a6a5c
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/97/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer af0e72599265ae261077619cf0470e81f8cf707447fbd7b9ad2cbdb0d23a6a5c"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 18dadab74ec19deb770922c7d8d6ffba211cf9d20ea2e305f317754ed848a217
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":23,"published":false}}
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
    "creator_id": 67,
    "id": 21,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 21,
    "additional_university_ids": [

    ],
    "discipline_id": 24,
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
    "updated_at": "2016-11-18T09:47:44.042Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 23,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":23,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18dadab74ec19deb770922c7d8d6ffba211cf9d20ea2e305f317754ed848a217"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 04e9536458ad364de4771f7972a1a7f21b6e7794ce63672de162381fd299904c
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
      "creator_id": 91,
      "id": 41,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-27",
      "html_url": "https://goskive.com/course/fu-course-27",
      "slug": "fu-course-27",
      "university_id": 31,
      "additional_university_ids": [

      ],
      "discipline_id": 44,
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
      "updated_at": "2016-11-18T09:47:46.576Z",
      "shortname": "fu-course-27",
      "topic_id": 43,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 27",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 91,
      "id": 42,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-28",
      "html_url": "https://goskive.com/course/fu-course-28",
      "slug": "fu-course-28",
      "university_id": 31,
      "additional_university_ids": [

      ],
      "discipline_id": 45,
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
      "updated_at": "2016-11-18T09:47:46.615Z",
      "shortname": "fu-course-28",
      "topic_id": 44,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 28",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 92,
      "id": 43,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-29",
      "html_url": "https://goskive.com/course/fu-course-29",
      "slug": "fu-course-29",
      "university_id": 31,
      "additional_university_ids": [

      ],
      "discipline_id": 46,
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
      "updated_at": "2016-11-18T09:47:46.662Z",
      "shortname": "fu-course-29",
      "topic_id": 45,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 29",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 92,
      "id": 44,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-30",
      "html_url": "https://goskive.com/course/fu-course-30",
      "slug": "fu-course-30",
      "university_id": 31,
      "additional_university_ids": [

      ],
      "discipline_id": 47,
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
      "chapters_updated_at": "2016-11-18T09:47:46.517Z",
      "updated_at": "2016-11-18T09:47:47.005Z",
      "shortname": "fu-course-30",
      "topic_id": 46,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 30",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04e9536458ad364de4771f7972a1a7f21b6e7794ce63672de162381fd299904c"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 488e4d342d37622f175eb321c4832f6036ac578f62e36ef5d1fbefbcd07bd361
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
      "creator_id": 98,
      "id": 45,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-31",
      "html_url": "https://goskive.com/course/fu-course-31",
      "slug": "fu-course-31",
      "university_id": 33,
      "additional_university_ids": [

      ],
      "discipline_id": 48,
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
      "updated_at": "2016-11-18T09:47:47.210Z",
      "shortname": "fu-course-31",
      "topic_id": 47,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 31",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 98,
      "id": 46,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-32",
      "html_url": "https://goskive.com/course/fu-course-32",
      "slug": "fu-course-32",
      "university_id": 33,
      "additional_university_ids": [

      ],
      "discipline_id": 49,
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
      "updated_at": "2016-11-18T09:47:47.252Z",
      "shortname": "fu-course-32",
      "topic_id": 48,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 32",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 99,
      "id": 47,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-33",
      "html_url": "https://goskive.com/course/fu-course-33",
      "slug": "fu-course-33",
      "university_id": 33,
      "additional_university_ids": [

      ],
      "discipline_id": 50,
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
      "updated_at": "2016-11-18T09:47:47.299Z",
      "shortname": "fu-course-33",
      "topic_id": 49,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 33",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 99,
      "id": 48,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-34",
      "html_url": "https://goskive.com/course/fu-course-34",
      "slug": "fu-course-34",
      "university_id": 33,
      "additional_university_ids": [

      ],
      "discipline_id": 51,
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
      "updated_at": "2016-11-18T09:47:47.339Z",
      "shortname": "fu-course-34",
      "topic_id": 50,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 34",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 488e4d342d37622f175eb321c4832f6036ac578f62e36ef5d1fbefbcd07bd361"
```
