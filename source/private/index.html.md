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
DELETE /v2/chapters/6
Content-Type: application/json
Authorization: Bearer cdfe4df87b63f1f5e5a7a2bc5ef02220b8ac3f79fb7a4a092ebaee4bd90074a2
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cdfe4df87b63f1f5e5a7a2bc5ef02220b8ac3f79fb7a4a092ebaee4bd90074a2"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/1
Content-Type: application/json
Authorization: Bearer b3d64a28834614abfd2d94800f7a392a6b3d8a13886b32f4875217dc43ccbaf0
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
    "id": 1,
    "updated_at": "2016-12-04T19:23:24.609Z",
    "course_id": 1,
    "author_id": 8,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-04T19:23:23.330Z",
    "questions_updated_at": "2016-12-04T19:23:23.330Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 11,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:23:24.554Z",
        "created_at": "2016-12-04T19:23:24.554Z",
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
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 12,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:23:24.591Z",
        "created_at": "2016-12-04T19:23:24.591Z",
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
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 9,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:23:24.278Z",
        "created_at": "2016-12-04T19:23:24.162Z",
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
            "id": 1,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 2,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 2,
        "obfuscated_id": "yHhUU9c1C7Y",
        "author_id": 10,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:23:24.472Z",
        "created_at": "2016-12-04T19:23:24.349Z",
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
            "id": 3,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 4,
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
curl "api.goskive.com/v2/chapters/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b3d64a28834614abfd2d94800f7a392a6b3d8a13886b32f4875217dc43ccbaf0"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/8
Content-Type: application/json
Authorization: Bearer a2bb21f1b7a6100890d50ce7e79c704d2a77fbc9d009c8eecbd19c9167011063
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
    "id": 8,
    "updated_at": "2016-12-04T19:23:26.545Z",
    "course_id": 8,
    "author_id": 37,
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
curl "api.goskive.com/v2/chapters/8" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2bb21f1b7a6100890d50ce7e79c704d2a77fbc9d009c8eecbd19c9167011063"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer c3903666fc0dd174814490616529b105b9e45349d035141c68a2002c46bc6238
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3903666fc0dd174814490616529b105b9e45349d035141c68a2002c46bc6238"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 57750c63cfc0bcf6b96d9f68e4dc097eec6ec68f3f5a5e53b2aae63f1a3cbc1d
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
      "id": 14,
      "author_id": 508,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:00.975Z",
      "status": "published",
      "subject_id": 138,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 510,
      "reply_to_id": 14,
      "created_at": "2016-12-04T19:24:01.055Z",
      "status": "published",
      "subject_id": 139,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 512,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:01.138Z",
      "status": "published",
      "subject_id": 140,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 514,
      "reply_to_id": 16,
      "created_at": "2016-12-04T19:24:01.216Z",
      "status": "published",
      "subject_id": 141,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 516,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:01.298Z",
      "status": "reported",
      "subject_id": 142,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 518,
      "reply_to_id": 18,
      "created_at": "2016-12-04T19:24:01.378Z",
      "status": "published",
      "subject_id": 143,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 520,
      "reply_to_id": 18,
      "created_at": "2016-12-04T19:24:01.457Z",
      "status": "published",
      "subject_id": 144,
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
	-H "Authorization: Bearer 57750c63cfc0bcf6b96d9f68e4dc097eec6ec68f3f5a5e53b2aae63f1a3cbc1d"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a61b4aa029bc296240351cfb496f3a255976006ca14da73f48898245c639c77b
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
      "author_id": 523,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:01.591Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 525,
      "reply_to_id": 21,
      "created_at": "2016-12-04T19:24:01.670Z",
      "status": "published",
      "subject_id": 146,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 527,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:01.749Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 529,
      "reply_to_id": 23,
      "created_at": "2016-12-04T19:24:01.829Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 531,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:01.909Z",
      "status": "reported",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 533,
      "reply_to_id": 25,
      "created_at": "2016-12-04T19:24:01.992Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 535,
      "reply_to_id": 25,
      "created_at": "2016-12-04T19:24:02.076Z",
      "status": "published",
      "subject_id": 151,
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
	-H "Authorization: Bearer a61b4aa029bc296240351cfb496f3a255976006ca14da73f48898245c639c77b"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 58212fcdd7019a70410814664c345b356c0f6729039f3355dfcfce5f5518dfe1
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
      "id": 29,
      "author_id": 540,
      "reply_to_id": 28,
      "created_at": "2016-12-04T19:24:02.293Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 544,
      "reply_to_id": 30,
      "created_at": "2016-12-04T19:24:02.450Z",
      "status": "published",
      "subject_id": 155,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 548,
      "reply_to_id": 32,
      "created_at": "2016-12-04T19:24:02.606Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 550,
      "reply_to_id": 32,
      "created_at": "2016-12-04T19:24:02.687Z",
      "status": "published",
      "subject_id": 158,
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
	-H "Authorization: Bearer 58212fcdd7019a70410814664c345b356c0f6729039f3355dfcfce5f5518dfe1"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer da4657a14fc90104024b22533fd87873995d39e267638e9eb9275fa1c310dd4b
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
      "id": 39,
      "author_id": 561,
      "reply_to_id": null,
      "created_at": "2016-12-04T19:24:03.154Z",
      "status": "reported",
      "subject_id": 163,
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
	-H "Authorization: Bearer da4657a14fc90104024b22533fd87873995d39e267638e9eb9275fa1c310dd4b"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/12/republish
Content-Type: application/json
Authorization: Bearer 2638d6d536a7574de870cdc25d31c8aeb90a9cbc981d4397145bca904308c5f6
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
	-H "Authorization: Bearer 2638d6d536a7574de870cdc25d31c8aeb90a9cbc981d4397145bca904308c5f6"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/108/chapters
Content-Type: application/json
Authorization: Bearer 1806c9e38d7bedc18be6d545f06587169cb290d39ef1a71c4919d8ce5626f25b
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
    "id": 73,
    "updated_at": "2016-12-04T19:23:56.030Z",
    "course_id": 108,
    "author_id": 417,
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
curl "api.goskive.com/v2/courses/108/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1806c9e38d7bedc18be6d545f06587169cb290d39ef1a71c4919d8ce5626f25b"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 11d70f8dce94dcf99561a32b4668c33939416f0f29607a9427bd0a8e44298608
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
    "id": 74,
    "updated_at": "2016-12-04T19:23:56.156Z",
    "course_id": 109,
    "author_id": 419,
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
	-H "Authorization: Bearer 11d70f8dce94dcf99561a32b4668c33939416f0f29607a9427bd0a8e44298608"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 59e6c17a149dd6126a8e0fae13672572fd6f10da0256245409e87e2b57fca400
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
      "id": 91,
      "updated_at": "2016-12-04T19:23:58.115Z",
      "course_id": 120,
      "author_id": 457,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 70",
      "position": 1
    },
    {
      "id": 92,
      "updated_at": "2016-12-04T19:23:58.139Z",
      "course_id": 120,
      "author_id": 458,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 71",
      "position": 2
    },
    {
      "id": 93,
      "updated_at": "2016-12-04T19:23:58.386Z",
      "course_id": 120,
      "author_id": 459,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-04T19:23:58.042Z",
      "questions_updated_at": "2016-12-04T19:23:58.042Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 72",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 59e6c17a149dd6126a8e0fae13672572fd6f10da0256245409e87e2b57fca400"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 7b339273b4da0f319cff640f9ba2ac9cf15b1f2b28edc750714d50c358cf1da7
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
      "id": 94,
      "updated_at": "2016-12-04T19:23:58.674Z",
      "course_id": 122,
      "author_id": 466,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 73",
      "position": 1
    },
    {
      "id": 95,
      "updated_at": "2016-12-04T19:23:58.698Z",
      "course_id": 122,
      "author_id": 467,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 74",
      "position": 2
    },
    {
      "id": 96,
      "updated_at": "2016-12-04T19:23:58.726Z",
      "course_id": 122,
      "author_id": 468,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 75",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7b339273b4da0f319cff640f9ba2ac9cf15b1f2b28edc750714d50c358cf1da7"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5be2ff1f17a442a65a4e2eb24837b26a33337cd54af5e6e12ddf7d8fb4a9108b
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
	-H "Authorization: Bearer 5be2ff1f17a442a65a4e2eb24837b26a33337cd54af5e6e12ddf7d8fb4a9108b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/193
Content-Type: application/json
Authorization: Bearer 3fcf8b5ac259c614fe48189328002d02aeed03abb258f3918123d4b024a845a0
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/193" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3fcf8b5ac259c614fe48189328002d02aeed03abb258f3918123d4b024a845a0"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 32b03b71261cb98decec76f62a38cf95bc998e50774c8ab5cefb0e5070c106a3
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
    "creator_id": 650,
    "id": 196,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 198,
    "additional_university_ids": [

    ],
    "discipline_id": 206,
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
    "chapters_updated_at": "2016-12-04T19:24:11.793Z",
    "updated_at": "2016-12-04T19:24:13.147Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 40,
        "obfuscated_id": "lir5nwklJts",
        "author_id": 650,
        "chapter_id": 111,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:12.956Z",
        "created_at": "2016-12-04T19:24:12.956Z",
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
        "author_id": 650,
        "chapter_id": 112,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:13.022Z",
        "created_at": "2016-12-04T19:24:13.022Z",
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
        "author_id": 650,
        "chapter_id": 111,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:12.993Z",
        "created_at": "2016-12-04T19:24:12.993Z",
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
        "author_id": 650,
        "chapter_id": 112,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:13.059Z",
        "created_at": "2016-12-04T19:24:13.059Z",
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
        "author_id": 653,
        "chapter_id": 111,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:13.094Z",
        "created_at": "2016-12-04T19:24:13.094Z",
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
        "author_id": 654,
        "chapter_id": 112,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T19:24:13.130Z",
        "created_at": "2016-12-04T19:24:13.130Z",
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
        "id": 111,
        "updated_at": "2016-12-04T19:24:13.103Z",
        "course_id": 196,
        "author_id": 650,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-04T19:24:11.793Z",
        "questions_updated_at": "2016-12-04T19:24:11.793Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 90",
        "position": 1
      },
      {
        "id": 112,
        "updated_at": "2016-12-04T19:24:13.140Z",
        "course_id": 196,
        "author_id": 650,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-04T19:24:11.793Z",
        "questions_updated_at": "2016-12-04T19:24:11.793Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 91",
        "position": 2
      }
    ],
    "topic_id": 205,
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
	-H "Authorization: Bearer 32b03b71261cb98decec76f62a38cf95bc998e50774c8ab5cefb0e5070c106a3"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/180
Content-Type: application/json
Authorization: Bearer d39ace880c6e0a435ac91709eda85c9543d8023d46be5d763d9cd7f13f19258a
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
    "creator_id": 610,
    "id": 180,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 182,
    "additional_university_ids": [

    ],
    "discipline_id": 190,
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
    "updated_at": "2016-12-04T19:24:06.871Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 189,
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
curl "api.goskive.com/v2/courses/180" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d39ace880c6e0a435ac91709eda85c9543d8023d46be5d763d9cd7f13f19258a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 2ecd2cf142e90a8b23f2e297649a14db3074f521e508e64010084450a81e9852
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
    "creator_id": 615,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 185,
    "additional_university_ids": [

    ],
    "discipline_id": 193,
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
    "updated_at": "2016-12-04T19:24:07.230Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 192,
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
	-H "Authorization: Bearer 2ecd2cf142e90a8b23f2e297649a14db3074f521e508e64010084450a81e9852"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer a6e8064c986dd80dede3492f137b78b42919dd55c338494e8397f2cfa2aa9379
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
      "id": 19,
      "user_id": 172,
      "feedbackable_id": 28,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:37.276Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 20,
      "user_id": 176,
      "feedbackable_id": 29,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:37.550Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 180,
      "feedbackable_id": 30,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:37.851Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 184,
      "feedbackable_id": 31,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:38.134Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 188,
      "feedbackable_id": 32,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-04T19:23:38.408Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6e8064c986dd80dede3492f137b78b42919dd55c338494e8397f2cfa2aa9379"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer c463c9f604c37a8fc723ad337067c48f119b5669d19f0e00bb101d35deee7580
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
      "id": 18,
      "user_id": 167,
      "feedbackable_id": 27,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-04T19:23:36.967Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c463c9f604c37a8fc723ad337067c48f119b5669d19f0e00bb101d35deee7580"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer 1ee3c018eece009672c6d10b0ba94e3b03bf54b9352f11344cf3f454d3474f13
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/13" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1ee3c018eece009672c6d10b0ba94e3b03bf54b9352f11344cf3f454d3474f13"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/4/metadata
Content-Type: application/json
Authorization: Bearer 81f77de5368cdecdb499c458f500bc4983f02594ea047839e2ab3f37b2a30199
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
    "id": 4,
    "uploader": {
      "id": 275,
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
      "created_at": "2016-12-04T19:23:44.148Z",
      "updated_at": "2016-12-04T19:23:44.148Z"
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
    "created_at": "2016-12-04T19:23:44.218Z",
    "updated_at": "2016-12-04T19:23:44.218Z",
    "course_id": 68,
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
curl "api.goskive.com/v2/files/4/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 81f77de5368cdecdb499c458f500bc4983f02594ea047839e2ab3f37b2a30199"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/57/feedbacks
Content-Type: application/json
Authorization: Bearer 0ac56f3f8deba4a6524c0d33842ca6ad25fb00961f0e73aa7bf9213d620099e0
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
      "user_id": 767,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:24:24.404Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 766,
      "feedbackable_id": 57,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:24:24.394Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/57/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ac56f3f8deba4a6524c0d33842ca6ad25fb00961f0e73aa7bf9213d620099e0"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer a3aafb4744540d559cc16e5e34219766e08d8da76d56fb3459906fa2a3ce1ed3
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
      "id": 72,
      "obfuscated_id": "oqzxOzwzIgw",
      "author_id": 822,
      "chapter_id": 160,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:27.095Z",
      "created_at": "2016-12-04T19:24:27.095Z",
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
      "author_id": 825,
      "chapter_id": 161,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:27.251Z",
      "created_at": "2016-12-04T19:24:27.251Z",
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
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 828,
      "chapter_id": 162,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:27.374Z",
      "created_at": "2016-12-04T19:24:27.374Z",
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
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 831,
      "chapter_id": 163,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:27.504Z",
      "created_at": "2016-12-04T19:24:27.504Z",
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
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 834,
      "chapter_id": 164,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:27.628Z",
      "created_at": "2016-12-04T19:24:27.628Z",
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
	-H "Authorization: Bearer a3aafb4744540d559cc16e5e34219766e08d8da76d56fb3459906fa2a3ce1ed3"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 63c37c7aea5dde57d6a7635dcc3b945d9601fecdd4169b87f55f9fd02b3c3c89
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
      "author_id": 818,
      "chapter_id": 159,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:26.917Z",
      "created_at": "2016-12-04T19:24:26.917Z",
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
	-H "Authorization: Bearer 63c37c7aea5dde57d6a7635dcc3b945d9601fecdd4169b87f55f9fd02b3c3c89"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/82/republish
Content-Type: application/json
Authorization: Bearer d99029299acdc0fe1953e9a1bfe58ef31c4ff1b4de3ae6c37359ad93d53d74bd
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/82/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d99029299acdc0fe1953e9a1bfe58ef31c4ff1b4de3ae6c37359ad93d53d74bd"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/49/feedbacks
Content-Type: application/json
Authorization: Bearer f842d9e04a41d270e2fd5cf6b42127bf22d491932c8b894fff4f128ced5dd03b
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
      "id": 33,
      "user_id": 377,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:50.941Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 32,
      "user_id": 376,
      "feedbackable_id": 49,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T19:23:50.930Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/49/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f842d9e04a41d270e2fd5cf6b42127bf22d491932c8b894fff4f128ced5dd03b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 603ad4f446376c0ef0423cc020c8d53881c628e35e5408167fb6134f89b77c6e
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
      "id": 107,
      "obfuscated_id": "_2rgp7tgq8o",
      "author_id": 695,
      "chapter_id": 125,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:18.132Z",
      "created_at": "2016-12-04T19:24:18.015Z",
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
          "id": 217,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 218,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 104,
      "obfuscated_id": "nIg2bhYRjos",
      "author_id": 686,
      "chapter_id": 122,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:17.323Z",
      "created_at": "2016-12-04T19:24:17.208Z",
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
          "id": 211,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 212,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 105,
      "obfuscated_id": "3yX9LpVrF_M",
      "author_id": 689,
      "chapter_id": 123,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:17.595Z",
      "created_at": "2016-12-04T19:24:17.479Z",
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
          "id": 213,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 214,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 106,
      "obfuscated_id": "GEL902caNek",
      "author_id": 692,
      "chapter_id": 124,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:17.860Z",
      "created_at": "2016-12-04T19:24:17.747Z",
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
          "id": 215,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 216,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 108,
      "obfuscated_id": "3MKez0MLRBM",
      "author_id": 698,
      "chapter_id": 126,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:18.397Z",
      "created_at": "2016-12-04T19:24:18.289Z",
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
          "id": 219,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 220,
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
	-H "Authorization: Bearer 603ad4f446376c0ef0423cc020c8d53881c628e35e5408167fb6134f89b77c6e"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9c3f0aab84499a8b37a9e790cdaef430f148bcb3f6303afc3bed222afa1eaaa5
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
      "id": 113,
      "obfuscated_id": "pcyz_ZHBlMU",
      "author_id": 714,
      "chapter_id": 131,
      "position": 107,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T19:24:19.823Z",
      "created_at": "2016-12-04T19:24:19.716Z",
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
          "id": 229,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 230,
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
	-H "Authorization: Bearer 9c3f0aab84499a8b37a9e790cdaef430f148bcb3f6303afc3bed222afa1eaaa5"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/117/republish
Content-Type: application/json
Authorization: Bearer dece940e675f3561fd6a2df263c481ec874205dca7056b55d1da67e58a8c12c0
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/117/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dece940e675f3561fd6a2df263c481ec874205dca7056b55d1da67e58a8c12c0"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 654d4d1ce2c6da382c89c04d1058f7583ae7eaf5e7b8d9ccdc3254fa70d94085
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":302,"published":false}}
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
    "creator_id": 904,
    "id": 293,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 278,
    "additional_university_ids": [

    ],
    "discipline_id": 303,
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
    "updated_at": "2016-12-04T19:24:32.811Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 302,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":302,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 654d4d1ce2c6da382c89c04d1058f7583ae7eaf5e7b8d9ccdc3254fa70d94085"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8b9dff89e5010b465adf9b46c2f8f6493ea1cfca48bd7ef0d9e7131c05e227cb
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
      "creator_id": 886,
      "id": 276,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-208",
      "html_url": "https://goskive.com/course/fu-course-208",
      "slug": "fu-course-208",
      "university_id": 271,
      "additional_university_ids": [

      ],
      "discipline_id": 286,
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
      "updated_at": "2016-12-04T19:24:31.124Z",
      "shortname": "fu-course-208",
      "topic_id": 285,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 208",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 886,
      "id": 277,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-209",
      "html_url": "https://goskive.com/course/fu-course-209",
      "slug": "fu-course-209",
      "university_id": 271,
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
      "updated_at": "2016-12-04T19:24:31.160Z",
      "shortname": "fu-course-209",
      "topic_id": 286,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 209",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 887,
      "id": 278,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-210",
      "html_url": "https://goskive.com/course/fu-course-210",
      "slug": "fu-course-210",
      "university_id": 271,
      "additional_university_ids": [

      ],
      "discipline_id": 288,
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
      "updated_at": "2016-12-04T19:24:31.202Z",
      "shortname": "fu-course-210",
      "topic_id": 287,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 210",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 887,
      "id": 279,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-211",
      "html_url": "https://goskive.com/course/fu-course-211",
      "slug": "fu-course-211",
      "university_id": 271,
      "additional_university_ids": [

      ],
      "discipline_id": 289,
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
      "chapters_updated_at": "2016-12-04T19:24:31.073Z",
      "updated_at": "2016-12-04T19:24:31.475Z",
      "shortname": "fu-course-211",
      "topic_id": 288,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 211",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b9dff89e5010b465adf9b46c2f8f6493ea1cfca48bd7ef0d9e7131c05e227cb"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e3360d17bc08dd7d589ce7369d73094befe073455ac0ab00d903427565c9cff9
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
      "creator_id": 893,
      "id": 280,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-212",
      "html_url": "https://goskive.com/course/fu-course-212",
      "slug": "fu-course-212",
      "university_id": 273,
      "additional_university_ids": [

      ],
      "discipline_id": 290,
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
      "updated_at": "2016-12-04T19:24:31.662Z",
      "shortname": "fu-course-212",
      "topic_id": 289,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 212",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 893,
      "id": 281,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-213",
      "html_url": "https://goskive.com/course/fu-course-213",
      "slug": "fu-course-213",
      "university_id": 273,
      "additional_university_ids": [

      ],
      "discipline_id": 291,
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
      "updated_at": "2016-12-04T19:24:31.698Z",
      "shortname": "fu-course-213",
      "topic_id": 290,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 213",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 894,
      "id": 282,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 273,
      "additional_university_ids": [

      ],
      "discipline_id": 292,
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
      "updated_at": "2016-12-04T19:24:31.741Z",
      "shortname": "fu-course-214",
      "topic_id": 291,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 894,
      "id": 283,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 273,
      "additional_university_ids": [

      ],
      "discipline_id": 293,
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
      "updated_at": "2016-12-04T19:24:31.777Z",
      "shortname": "fu-course-215",
      "topic_id": 292,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3360d17bc08dd7d589ce7369d73094befe073455ac0ab00d903427565c9cff9"
```
