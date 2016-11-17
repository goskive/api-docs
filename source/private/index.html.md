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
DELETE /v2/chapters/176
Content-Type: application/json
Authorization: Bearer 13a40f62b6330b81604bc774176ff1ac18ff2bd9d00c86155d0a842ae84599e6
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/176" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 13a40f62b6330b81604bc774176ff1ac18ff2bd9d00c86155d0a842ae84599e6"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/172
Content-Type: application/json
Authorization: Bearer 3002ca3fca0fa892c7fa0409624e44a59be686b401b26ca72cc7e3ce7e1cf4d3
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
    "id": 172,
    "updated_at": "2016-11-17T18:17:08.628Z",
    "course_id": 254,
    "author_id": 854,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-17T18:17:08.064Z",
    "questions_updated_at": "2016-11-17T18:17:08.064Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 857,
        "chapter_id": 172,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:17:08.570Z",
        "created_at": "2016-11-17T18:17:08.570Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 858,
        "chapter_id": 172,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:17:08.610Z",
        "created_at": "2016-11-17T18:17:08.610Z",
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
        "id": 118,
        "obfuscated_id": "ET3wO26jBck",
        "author_id": 855,
        "chapter_id": 172,
        "position": 109,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:17:08.294Z",
        "created_at": "2016-11-17T18:17:08.178Z",
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
            "id": 236,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 237,
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
        "author_id": 856,
        "chapter_id": 172,
        "position": 110,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:17:08.497Z",
        "created_at": "2016-11-17T18:17:08.370Z",
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
            "id": 238,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 239,
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
curl "api.goskive.com/v2/chapters/172" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3002ca3fca0fa892c7fa0409624e44a59be686b401b26ca72cc7e3ce7e1cf4d3"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/168
Content-Type: application/json
Authorization: Bearer 4052317b4cbb2b12039c2dfe1f04801882f884fde9ace2b8efd6e191e51f01f6
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
    "id": 168,
    "updated_at": "2016-11-17T18:17:06.966Z",
    "course_id": 250,
    "author_id": 839,
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
curl "api.goskive.com/v2/chapters/168" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4052317b4cbb2b12039c2dfe1f04801882f884fde9ace2b8efd6e191e51f01f6"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer bc42c56b456dfb0c4d8cb7e780d033fc3da6a8918cb02e0aeef6a46de51b6ddf
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/2" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bc42c56b456dfb0c4d8cb7e780d033fc3da6a8918cb02e0aeef6a46de51b6ddf"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer feb3d6418f09365451be79c5a440e84e110da6ee78ce02c2a767ec6e903d2e5f
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
      "id": 4,
      "author_id": 170,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:05.459Z",
      "status": "published",
      "subject_id": 51,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 172,
      "reply_to_id": 4,
      "created_at": "2016-11-17T18:16:05.546Z",
      "status": "published",
      "subject_id": 52,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 174,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:05.630Z",
      "status": "published",
      "subject_id": 53,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 176,
      "reply_to_id": 6,
      "created_at": "2016-11-17T18:16:05.713Z",
      "status": "published",
      "subject_id": 54,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 8,
      "author_id": 178,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:05.797Z",
      "status": "reported",
      "subject_id": 55,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 180,
      "reply_to_id": 8,
      "created_at": "2016-11-17T18:16:05.880Z",
      "status": "published",
      "subject_id": 56,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 182,
      "reply_to_id": 8,
      "created_at": "2016-11-17T18:16:05.963Z",
      "status": "published",
      "subject_id": 57,
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
	-H "Authorization: Bearer feb3d6418f09365451be79c5a440e84e110da6ee78ce02c2a767ec6e903d2e5f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a1f7f27014f904e2e116cc60f1f49f2ee45ed3ee22bc3da0707d6ade1f5cc74f
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
      "id": 11,
      "author_id": 185,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:06.139Z",
      "status": "published",
      "subject_id": 58,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 187,
      "reply_to_id": 11,
      "created_at": "2016-11-17T18:16:06.225Z",
      "status": "published",
      "subject_id": 59,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 189,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:06.313Z",
      "status": "published",
      "subject_id": 60,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 191,
      "reply_to_id": 13,
      "created_at": "2016-11-17T18:16:06.397Z",
      "status": "published",
      "subject_id": 61,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 193,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:06.481Z",
      "status": "reported",
      "subject_id": 62,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 195,
      "reply_to_id": 15,
      "created_at": "2016-11-17T18:16:06.564Z",
      "status": "published",
      "subject_id": 63,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 197,
      "reply_to_id": 15,
      "created_at": "2016-11-17T18:16:06.647Z",
      "status": "published",
      "subject_id": 64,
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
	-H "Authorization: Bearer a1f7f27014f904e2e116cc60f1f49f2ee45ed3ee22bc3da0707d6ade1f5cc74f"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 0af35758b03dd9a524c1aa68642aaebb52b339bcc4a19337c33ed80ee9fb9429
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
      "author_id": 217,
      "reply_to_id": 25,
      "created_at": "2016-11-17T18:16:07.500Z",
      "status": "published",
      "subject_id": 73,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 221,
      "reply_to_id": 27,
      "created_at": "2016-11-17T18:16:07.675Z",
      "status": "published",
      "subject_id": 75,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 225,
      "reply_to_id": 29,
      "created_at": "2016-11-17T18:16:07.851Z",
      "status": "published",
      "subject_id": 77,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 227,
      "reply_to_id": 29,
      "created_at": "2016-11-17T18:16:07.933Z",
      "status": "published",
      "subject_id": 78,
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
	-H "Authorization: Bearer 0af35758b03dd9a524c1aa68642aaebb52b339bcc4a19337c33ed80ee9fb9429"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer df7901e99a0808a7724e8593f2a07384081298563f87ed69b5e6250175101965
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
      "id": 22,
      "author_id": 208,
      "reply_to_id": null,
      "created_at": "2016-11-17T18:16:07.124Z",
      "status": "reported",
      "subject_id": 69,
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
	-H "Authorization: Bearer df7901e99a0808a7724e8593f2a07384081298563f87ed69b5e6250175101965"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/40/republish
Content-Type: application/json
Authorization: Bearer bbb8f8bd851c458528cfba94cba8296524ed5f6132b92ca4b3534df03004608a
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/40/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bbb8f8bd851c458528cfba94cba8296524ed5f6132b92ca4b3534df03004608a"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/195/chapters
Content-Type: application/json
Authorization: Bearer 65eb5a9f0e5367ad0b4db9fe2420463b26dc15d0e881cf64860de1f14854c28a
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
    "id": 127,
    "updated_at": "2016-11-17T18:16:44.126Z",
    "course_id": 195,
    "author_id": 644,
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
curl "api.goskive.com/v2/courses/195/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 65eb5a9f0e5367ad0b4db9fe2420463b26dc15d0e881cf64860de1f14854c28a"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8238df3c51713aa63bf07093cfd987fac5f06e6b3a15b7b5d4ca2e5d79e89d0e
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
    "id": 128,
    "updated_at": "2016-11-17T18:16:44.314Z",
    "course_id": 196,
    "author_id": 646,
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
	-H "Authorization: Bearer 8238df3c51713aa63bf07093cfd987fac5f06e6b3a15b7b5d4ca2e5d79e89d0e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9b16574870f2465ca8818d1362b9f801708289c4a0c10b9bf711af0a10339f4f
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
      "id": 118,
      "updated_at": "2016-11-17T18:16:42.868Z",
      "course_id": 190,
      "author_id": 623,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 118",
      "position": 1
    },
    {
      "id": 119,
      "updated_at": "2016-11-17T18:16:42.897Z",
      "course_id": 190,
      "author_id": 624,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 119",
      "position": 2
    },
    {
      "id": 120,
      "updated_at": "2016-11-17T18:16:43.240Z",
      "course_id": 190,
      "author_id": 625,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-17T18:16:42.785Z",
      "questions_updated_at": "2016-11-17T18:16:42.785Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 120",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9b16574870f2465ca8818d1362b9f801708289c4a0c10b9bf711af0a10339f4f"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1582e99d30680d233183509a6c76ab308eecf6fca97bdf63e7b4ea5167a32fa3
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
      "id": 121,
      "updated_at": "2016-11-17T18:16:43.516Z",
      "course_id": 192,
      "author_id": 632,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 121",
      "position": 1
    },
    {
      "id": 122,
      "updated_at": "2016-11-17T18:16:43.545Z",
      "course_id": 192,
      "author_id": 633,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 122",
      "position": 2
    },
    {
      "id": 123,
      "updated_at": "2016-11-17T18:16:43.574Z",
      "course_id": 192,
      "author_id": 634,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 123",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1582e99d30680d233183509a6c76ab308eecf6fca97bdf63e7b4ea5167a32fa3"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/213
Content-Type: application/json
Authorization: Bearer a3e993bbe5dd7294894a6271d8d9c9a35a8405de3598bd69fcd847b305adb780
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/213" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3e993bbe5dd7294894a6271d8d9c9a35a8405de3598bd69fcd847b305adb780"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 93619ec3fa33a84214884ac0b948f7fc0c68db0e17ab99d4dc8f47c84437dc80
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
	-H "Authorization: Bearer 93619ec3fa33a84214884ac0b948f7fc0c68db0e17ab99d4dc8f47c84437dc80"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 7c141fff6a717ae9d031c29101456e18592db020ac3229370b60e51f15732a3d
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
    "creator_id": 731,
    "id": 225,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 227,
    "additional_university_ids": [

    ],
    "discipline_id": 238,
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
    "chapters_updated_at": "2016-11-17T18:16:53.220Z",
    "updated_at": "2016-11-17T18:16:54.719Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 731,
        "chapter_id": 146,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.508Z",
        "created_at": "2016-11-17T18:16:54.508Z",
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
        "author_id": 731,
        "chapter_id": 147,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.581Z",
        "created_at": "2016-11-17T18:16:54.581Z",
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
        "author_id": 731,
        "chapter_id": 146,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.550Z",
        "created_at": "2016-11-17T18:16:54.550Z",
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
        "author_id": 731,
        "chapter_id": 147,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.622Z",
        "created_at": "2016-11-17T18:16:54.622Z",
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
        "author_id": 734,
        "chapter_id": 146,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.662Z",
        "created_at": "2016-11-17T18:16:54.662Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 735,
        "chapter_id": 147,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T18:16:54.701Z",
        "created_at": "2016-11-17T18:16:54.701Z",
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
        "id": 146,
        "updated_at": "2016-11-17T18:16:54.672Z",
        "course_id": 225,
        "author_id": 731,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T18:16:53.220Z",
        "questions_updated_at": "2016-11-17T18:16:53.220Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 143",
        "position": 1
      },
      {
        "id": 147,
        "updated_at": "2016-11-17T18:16:54.712Z",
        "course_id": 225,
        "author_id": 731,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T18:16:53.220Z",
        "questions_updated_at": "2016-11-17T18:16:53.220Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 144",
        "position": 2
      }
    ],
    "topic_id": 237,
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
	-H "Authorization: Bearer 7c141fff6a717ae9d031c29101456e18592db020ac3229370b60e51f15732a3d"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/211
Content-Type: application/json
Authorization: Bearer 895d9951b46901fb6810a4e27368e6f66c73b467f6343dab1648e7915f06d05d
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
    "creator_id": 694,
    "id": 211,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 213,
    "additional_university_ids": [

    ],
    "discipline_id": 224,
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
    "updated_at": "2016-11-17T18:16:47.642Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 223,
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
curl "api.goskive.com/v2/courses/211" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 895d9951b46901fb6810a4e27368e6f66c73b467f6343dab1648e7915f06d05d"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer ac764cb2d501b4261529765f808c1959d3190732ec3cd08ad80af2a45d0d0514
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
    "creator_id": 690,
    "id": 209,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 211,
    "additional_university_ids": [

    ],
    "discipline_id": 222,
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
    "updated_at": "2016-11-17T18:16:47.385Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 221,
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
	-H "Authorization: Bearer ac764cb2d501b4261529765f808c1959d3190732ec3cd08ad80af2a45d0d0514"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer fff8e881c9b19b5b525209733312189448902245b89f9c359863c6450d7e554f
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
      "user_id": 528,
      "feedbackable_id": 62,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:36.143Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 532,
      "feedbackable_id": 63,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:36.562Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 536,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:36.947Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 540,
      "feedbackable_id": 65,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:37.323Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 544,
      "feedbackable_id": 66,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T18:16:37.706Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fff8e881c9b19b5b525209733312189448902245b89f9c359863c6450d7e554f"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 457728af2f3b51db5c8be7bd354d65c4c516143b705218dad409a773b900b2a1
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
      "user_id": 486,
      "feedbackable_id": 52,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T18:16:32.301Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 457728af2f3b51db5c8be7bd354d65c4c516143b705218dad409a773b900b2a1"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 88034f719de5192696e3b67aeadbe8817b9c5e615efa4445d532eb01ec9a6d76
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
	-H "Authorization: Bearer 88034f719de5192696e3b67aeadbe8817b9c5e615efa4445d532eb01ec9a6d76"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 717879cc5613b511b992f3d8d76043cfea4d6b0d8aeda81195ceeb7dd0594a94
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
    "id": 11,
    "uploader": {
      "id": 437,
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
      "created_at": "2016-11-17T18:16:29.047Z",
      "updated_at": "2016-11-17T18:16:29.047Z"
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
    "created_at": "2016-11-17T18:16:29.125Z",
    "updated_at": "2016-11-17T18:16:29.125Z",
    "course_id": 144,
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
curl "api.goskive.com/v2/files/11/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 717879cc5613b511b992f3d8d76043cfea4d6b0d8aeda81195ceeb7dd0594a94"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/48/feedbacks
Content-Type: application/json
Authorization: Bearer c438354cfdecc3155223b2521464edb5daea61cc5cc72bb0da5625de515b5168
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
      "user_id": 685,
      "feedbackable_id": 48,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:46.729Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 44,
      "user_id": 684,
      "feedbackable_id": 48,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:46.718Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/48/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c438354cfdecc3155223b2521464edb5daea61cc5cc72bb0da5625de515b5168"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 8bb51fb5fb8ac09297ee1298053a0a3d54d41181e59fe48d163510087bc12e8c
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 59,
      "chapter_id": 19,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:56.119Z",
      "created_at": "2016-11-17T18:15:56.119Z",
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
      "author_id": 62,
      "chapter_id": 20,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:56.260Z",
      "created_at": "2016-11-17T18:15:56.260Z",
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
      "author_id": 65,
      "chapter_id": 21,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:56.404Z",
      "created_at": "2016-11-17T18:15:56.404Z",
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
      "author_id": 68,
      "chapter_id": 22,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:56.547Z",
      "created_at": "2016-11-17T18:15:56.547Z",
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
      "author_id": 71,
      "chapter_id": 23,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:56.682Z",
      "created_at": "2016-11-17T18:15:56.682Z",
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
	-H "Authorization: Bearer 8bb51fb5fb8ac09297ee1298053a0a3d54d41181e59fe48d163510087bc12e8c"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4705eb3b6bc9472975205ce1aae87f2633483605c42014365a26710c8017c421
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 39,
      "chapter_id": 13,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:15:55.153Z",
      "created_at": "2016-11-17T18:15:55.153Z",
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
	-H "Authorization: Bearer 4705eb3b6bc9472975205ce1aae87f2633483605c42014365a26710c8017c421"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/4/republish
Content-Type: application/json
Authorization: Bearer db32b4ad2f7ba82fe4fe1c4df6f9b23cc62fb82ac1d60fb605397f86f4362662
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/4/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db32b4ad2f7ba82fe4fe1c4df6f9b23cc62fb82ac1d60fb605397f86f4362662"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/17/feedbacks
Content-Type: application/json
Authorization: Bearer 980c098e9fd2f1df61e301b765d0df500f16fe5c02ff426c5c11d8a4e03c8434
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
      "user_id": 301,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:13.274Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 300,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T18:16:13.263Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/17/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 980c098e9fd2f1df61e301b765d0df500f16fe5c02ff426c5c11d8a4e03c8434"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 7ab58166b3f067d92154b5ecdbd242bff4b62459375c9acca87a016bdeefd50d
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
      "id": 38,
      "obfuscated_id": "8_YCqPYFnsI",
      "author_id": 368,
      "chapter_id": 62,
      "position": 34,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:21.411Z",
      "created_at": "2016-11-17T18:16:21.254Z",
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
          "id": 75,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 76,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 359,
      "chapter_id": 59,
      "position": 31,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:20.382Z",
      "created_at": "2016-11-17T18:16:20.229Z",
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
          "id": 69,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 70,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 362,
      "chapter_id": 60,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:20.724Z",
      "created_at": "2016-11-17T18:16:20.570Z",
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
          "id": 71,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 72,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 37,
      "obfuscated_id": "95m_4XdR9PU",
      "author_id": 365,
      "chapter_id": 61,
      "position": 33,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:21.070Z",
      "created_at": "2016-11-17T18:16:20.914Z",
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
          "id": 73,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 74,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 39,
      "obfuscated_id": "N0Vv2_jrTfU",
      "author_id": 371,
      "chapter_id": 63,
      "position": 35,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:21.752Z",
      "created_at": "2016-11-17T18:16:21.601Z",
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
          "id": 77,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 78,
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
	-H "Authorization: Bearer 7ab58166b3f067d92154b5ecdbd242bff4b62459375c9acca87a016bdeefd50d"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 1e7b4747b8a04ff9f8ef0837820c0edf7cb02ffe0db29fe4a64dc08231251735
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
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 339,
      "chapter_id": 53,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T18:16:18.243Z",
      "created_at": "2016-11-17T18:16:18.101Z",
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
          "id": 57,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 58,
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
	-H "Authorization: Bearer 1e7b4747b8a04ff9f8ef0837820c0edf7cb02ffe0db29fe4a64dc08231251735"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/22/republish
Content-Type: application/json
Authorization: Bearer c42b26df00eae8cbe3ca0503d7e0101b6b0847988e175c661256f394d8f97814
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/22/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c42b26df00eae8cbe3ca0503d7e0101b6b0847988e175c661256f394d8f97814"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1b955b06ff2f7e24ffc0f094e6e30f94ca4bf3a5cfceb3f3b0cbce9a71e9265e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":286,"published":false}}
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
    "creator_id": 921,
    "id": 274,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 281,
    "additional_university_ids": [

    ],
    "discipline_id": 287,
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
    "updated_at": "2016-11-17T18:17:17.237Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 286,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":286,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1b955b06ff2f7e24ffc0f094e6e30f94ca4bf3a5cfceb3f3b0cbce9a71e9265e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d040b1f13b26bfbc0270c39befef4d7b3d7758332984af20337ceadb15d61bdf
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
      "creator_id": 954,
      "id": 304,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-235",
      "html_url": "https://goskive.com/course/fu-course-235",
      "slug": "fu-course-235",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 317,
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
      "updated_at": "2016-11-17T18:17:20.482Z",
      "shortname": "fu-course-235",
      "topic_id": 316,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 235",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 954,
      "id": 305,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-236",
      "html_url": "https://goskive.com/course/fu-course-236",
      "slug": "fu-course-236",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 318,
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
      "updated_at": "2016-11-17T18:17:20.523Z",
      "shortname": "fu-course-236",
      "topic_id": 317,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 236",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 955,
      "id": 306,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-237",
      "html_url": "https://goskive.com/course/fu-course-237",
      "slug": "fu-course-237",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 319,
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
      "updated_at": "2016-11-17T18:17:20.573Z",
      "shortname": "fu-course-237",
      "topic_id": 318,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 237",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 955,
      "id": 307,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-238",
      "html_url": "https://goskive.com/course/fu-course-238",
      "slug": "fu-course-238",
      "university_id": 294,
      "additional_university_ids": [

      ],
      "discipline_id": 320,
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
      "chapters_updated_at": "2016-11-17T18:17:20.423Z",
      "updated_at": "2016-11-17T18:17:20.893Z",
      "shortname": "fu-course-238",
      "topic_id": 319,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 238",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d040b1f13b26bfbc0270c39befef4d7b3d7758332984af20337ceadb15d61bdf"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5ef5a4410d81fc5da2d84c81349a3b379a30203bb8bc3ddd7d315852eddd46cb
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
      "creator_id": 961,
      "id": 308,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-239",
      "html_url": "https://goskive.com/course/fu-course-239",
      "slug": "fu-course-239",
      "university_id": 296,
      "additional_university_ids": [

      ],
      "discipline_id": 321,
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
      "updated_at": "2016-11-17T18:17:21.104Z",
      "shortname": "fu-course-239",
      "topic_id": 320,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 239",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 961,
      "id": 309,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-240",
      "html_url": "https://goskive.com/course/fu-course-240",
      "slug": "fu-course-240",
      "university_id": 296,
      "additional_university_ids": [

      ],
      "discipline_id": 322,
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
      "updated_at": "2016-11-17T18:17:21.147Z",
      "shortname": "fu-course-240",
      "topic_id": 321,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 240",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 962,
      "id": 310,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-241",
      "html_url": "https://goskive.com/course/fu-course-241",
      "slug": "fu-course-241",
      "university_id": 296,
      "additional_university_ids": [

      ],
      "discipline_id": 323,
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
      "updated_at": "2016-11-17T18:17:21.198Z",
      "shortname": "fu-course-241",
      "topic_id": 322,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 241",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 962,
      "id": 311,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-242",
      "html_url": "https://goskive.com/course/fu-course-242",
      "slug": "fu-course-242",
      "university_id": 296,
      "additional_university_ids": [

      ],
      "discipline_id": 324,
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
      "updated_at": "2016-11-17T18:17:21.240Z",
      "shortname": "fu-course-242",
      "topic_id": 323,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 242",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ef5a4410d81fc5da2d84c81349a3b379a30203bb8bc3ddd7d315852eddd46cb"
```
