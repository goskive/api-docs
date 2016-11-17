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
Authorization: Bearer 8adaab1a10642d8ac4ce80c5fd67bba826a4787fc03df8f67003264f1f0efb19
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
	-H "Authorization: Bearer 8adaab1a10642d8ac4ce80c5fd67bba826a4787fc03df8f67003264f1f0efb19"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/53
Content-Type: application/json
Authorization: Bearer b8cd6fc723b3c2fb2561d98ed313e4046a9298fb3816b3d5cee4456cbd253e43
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
    "id": 53,
    "updated_at": "2016-11-17T13:25:56.175Z",
    "course_id": 70,
    "author_id": 280,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-17T13:25:55.627Z",
    "questions_updated_at": "2016-11-17T13:25:55.627Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 283,
        "chapter_id": 53,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:56.119Z",
        "created_at": "2016-11-17T13:25:56.119Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 284,
        "chapter_id": 53,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:56.157Z",
        "created_at": "2016-11-17T13:25:56.157Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 281,
        "chapter_id": 53,
        "position": 41,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:55.847Z",
        "created_at": "2016-11-17T13:25:55.733Z",
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
            "id": 92,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 93,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 282,
        "chapter_id": 53,
        "position": 42,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:25:56.046Z",
        "created_at": "2016-11-17T13:25:55.921Z",
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
            "id": 94,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 95,
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
curl "api.goskive.com/v2/chapters/53" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b8cd6fc723b3c2fb2561d98ed313e4046a9298fb3816b3d5cee4456cbd253e43"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/46
Content-Type: application/json
Authorization: Bearer 81392c5ddc1156c2e7abe31bed66531d224ded2a2cd2a5e73a37045d6fdb04b2
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
    "updated_at": "2016-11-17T13:25:53.686Z",
    "course_id": 63,
    "author_id": 256,
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
	-H "Authorization: Bearer 81392c5ddc1156c2e7abe31bed66531d224ded2a2cd2a5e73a37045d6fdb04b2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/48
Content-Type: application/json
Authorization: Bearer 5b457097de440037b05ccf8f2bc18b7cd65e40851e4e25cf384a03a5632dcfff
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/48" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b457097de440037b05ccf8f2bc18b7cd65e40851e4e25cf384a03a5632dcfff"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 5cc45c32157e18fa3557d8246a0eba94471ee12cad23675f739e3c3092087a79
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
      "id": 10,
      "author_id": 405,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:06.573Z",
      "status": "published",
      "subject_id": 98,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 407,
      "reply_to_id": 10,
      "created_at": "2016-11-17T13:26:06.655Z",
      "status": "published",
      "subject_id": 99,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 409,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:06.734Z",
      "status": "published",
      "subject_id": 100,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 411,
      "reply_to_id": 12,
      "created_at": "2016-11-17T13:26:06.812Z",
      "status": "published",
      "subject_id": 101,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 413,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:06.890Z",
      "status": "reported",
      "subject_id": 102,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 415,
      "reply_to_id": 14,
      "created_at": "2016-11-17T13:26:06.970Z",
      "status": "published",
      "subject_id": 103,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 417,
      "reply_to_id": 14,
      "created_at": "2016-11-17T13:26:07.052Z",
      "status": "published",
      "subject_id": 104,
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
	-H "Authorization: Bearer 5cc45c32157e18fa3557d8246a0eba94471ee12cad23675f739e3c3092087a79"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer aa06934a2d3316c445f34863d3976037dd721086789e2eeae67782eebf15b834
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
      "author_id": 420,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:07.217Z",
      "status": "published",
      "subject_id": 105,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 422,
      "reply_to_id": 17,
      "created_at": "2016-11-17T13:26:07.295Z",
      "status": "published",
      "subject_id": 106,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 424,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:07.375Z",
      "status": "published",
      "subject_id": 107,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 426,
      "reply_to_id": 19,
      "created_at": "2016-11-17T13:26:07.456Z",
      "status": "published",
      "subject_id": 108,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 428,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:07.566Z",
      "status": "reported",
      "subject_id": 109,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 430,
      "reply_to_id": 21,
      "created_at": "2016-11-17T13:26:07.647Z",
      "status": "published",
      "subject_id": 110,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 432,
      "reply_to_id": 21,
      "created_at": "2016-11-17T13:26:07.725Z",
      "status": "published",
      "subject_id": 111,
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
	-H "Authorization: Bearer aa06934a2d3316c445f34863d3976037dd721086789e2eeae67782eebf15b834"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer cfa5f15b50e4d13917e7549412e6ff79b783bdd6f3f64fde6aa1c086e9893927
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
      "author_id": 452,
      "reply_to_id": 31,
      "created_at": "2016-11-17T13:26:08.529Z",
      "status": "published",
      "subject_id": 120,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 456,
      "reply_to_id": 33,
      "created_at": "2016-11-17T13:26:08.691Z",
      "status": "published",
      "subject_id": 122,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 460,
      "reply_to_id": 35,
      "created_at": "2016-11-17T13:26:08.848Z",
      "status": "published",
      "subject_id": 124,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 462,
      "reply_to_id": 35,
      "created_at": "2016-11-17T13:26:08.928Z",
      "status": "published",
      "subject_id": 125,
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
	-H "Authorization: Bearer cfa5f15b50e4d13917e7549412e6ff79b783bdd6f3f64fde6aa1c086e9893927"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 8033c277cb22b14622114624570689150d2a9739c034757bd7145adeba679bf6
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
      "id": 42,
      "author_id": 473,
      "reply_to_id": null,
      "created_at": "2016-11-17T13:26:09.387Z",
      "status": "reported",
      "subject_id": 130,
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
	-H "Authorization: Bearer 8033c277cb22b14622114624570689150d2a9739c034757bd7145adeba679bf6"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/49/republish
Content-Type: application/json
Authorization: Bearer f327b845deb0d56f2580e04db3ef729a8d59bd9d0163378f7523590f004e4440
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/49/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f327b845deb0d56f2580e04db3ef729a8d59bd9d0163378f7523590f004e4440"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 908b9072fc83772091b7cffa4d5216b66139c7cdea99589ae7df42218dbc0bcb
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
    "id": 161,
    "updated_at": "2016-11-17T13:26:42.263Z",
    "course_id": 282,
    "author_id": 867,
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
	-H "Authorization: Bearer 908b9072fc83772091b7cffa4d5216b66139c7cdea99589ae7df42218dbc0bcb"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/283/chapters
Content-Type: application/json
Authorization: Bearer ce5d9f0762bebd2fc1685b12cc9a387a4542eb486624ad326b6746be7ab57f65
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
    "id": 162,
    "updated_at": "2016-11-17T13:26:42.432Z",
    "course_id": 283,
    "author_id": 869,
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
curl "api.goskive.com/v2/courses/283/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce5d9f0762bebd2fc1685b12cc9a387a4542eb486624ad326b6746be7ab57f65"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 005eb3166b6fc1ec5a9f6cad4fa7454ce7ba7a66ae8662776526dc77c31e6f50
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
      "id": 154,
      "updated_at": "2016-11-17T13:26:41.144Z",
      "course_id": 277,
      "author_id": 849,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 136",
      "position": 1
    },
    {
      "id": 155,
      "updated_at": "2016-11-17T13:26:41.170Z",
      "course_id": 277,
      "author_id": 850,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 137",
      "position": 2
    },
    {
      "id": 156,
      "updated_at": "2016-11-17T13:26:41.504Z",
      "course_id": 277,
      "author_id": 851,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-17T13:26:41.071Z",
      "questions_updated_at": "2016-11-17T13:26:41.071Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 138",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 005eb3166b6fc1ec5a9f6cad4fa7454ce7ba7a66ae8662776526dc77c31e6f50"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9d4f797663bbb5fd1574d5e87b42673291c9af29d689c5ebd1664e3d78413596
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
      "updated_at": "2016-11-17T13:26:41.655Z",
      "course_id": 278,
      "author_id": 856,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 139",
      "position": 1
    },
    {
      "id": 158,
      "updated_at": "2016-11-17T13:26:41.682Z",
      "course_id": 278,
      "author_id": 857,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 140",
      "position": 2
    },
    {
      "id": 159,
      "updated_at": "2016-11-17T13:26:41.709Z",
      "course_id": 278,
      "author_id": 858,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 141",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9d4f797663bbb5fd1574d5e87b42673291c9af29d689c5ebd1664e3d78413596"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 0de9c76119534744244916b2024600fb5a755f1d0f1042174634cf304ea5993a
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
	-H "Authorization: Bearer 0de9c76119534744244916b2024600fb5a755f1d0f1042174634cf304ea5993a"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/249
Content-Type: application/json
Authorization: Bearer ce0556162bc5f5f7012e3bb43783ac0137fa483f27c5c49b43a4111f4c54e1a0
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/249" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ce0556162bc5f5f7012e3bb43783ac0137fa483f27c5c49b43a4111f4c54e1a0"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 60311dcc08cab6a96fe0312d8386f3ce2853842eeb0e3cc1bbebd6edb98bcaf1
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
    "creator_id": 779,
    "id": 259,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 244,
    "additional_university_ids": [

    ],
    "discipline_id": 267,
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
    "chapters_updated_at": "2016-11-17T13:26:34.002Z",
    "updated_at": "2016-11-17T13:26:35.846Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 779,
        "chapter_id": 128,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.598Z",
        "created_at": "2016-11-17T13:26:35.598Z",
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
        "author_id": 779,
        "chapter_id": 129,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.683Z",
        "created_at": "2016-11-17T13:26:35.683Z",
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
        "author_id": 779,
        "chapter_id": 128,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.647Z",
        "created_at": "2016-11-17T13:26:35.647Z",
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
        "author_id": 779,
        "chapter_id": 129,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.732Z",
        "created_at": "2016-11-17T13:26:35.732Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 782,
        "chapter_id": 128,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.777Z",
        "created_at": "2016-11-17T13:26:35.777Z",
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
        "author_id": 783,
        "chapter_id": 129,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T13:26:35.823Z",
        "created_at": "2016-11-17T13:26:35.823Z",
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
        "id": 128,
        "updated_at": "2016-11-17T13:26:35.790Z",
        "course_id": 259,
        "author_id": 779,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T13:26:34.002Z",
        "questions_updated_at": "2016-11-17T13:26:34.002Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 110",
        "position": 1
      },
      {
        "id": 129,
        "updated_at": "2016-11-17T13:26:35.835Z",
        "course_id": 259,
        "author_id": 779,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T13:26:34.002Z",
        "questions_updated_at": "2016-11-17T13:26:34.002Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 111",
        "position": 2
      }
    ],
    "topic_id": 266,
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
	-H "Authorization: Bearer 60311dcc08cab6a96fe0312d8386f3ce2853842eeb0e3cc1bbebd6edb98bcaf1"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/253
Content-Type: application/json
Authorization: Bearer fcccb1069bfe13ab00ca2f3d392309a82981a9b8eacc195b82b35c1bfd0cdb74
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
    "creator_id": 756,
    "id": 253,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 238,
    "additional_university_ids": [

    ],
    "discipline_id": 261,
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
    "updated_at": "2016-11-17T13:26:28.096Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 260,
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
curl "api.goskive.com/v2/courses/253" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fcccb1069bfe13ab00ca2f3d392309a82981a9b8eacc195b82b35c1bfd0cdb74"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4e73d74022feda7cdedf2d6f6e5b4ab134d4716606287ceb2740a8717f226bd2
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
    "creator_id": 754,
    "id": 252,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 237,
    "additional_university_ids": [

    ],
    "discipline_id": 260,
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
    "updated_at": "2016-11-17T13:26:27.952Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 259,
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
	-H "Authorization: Bearer 4e73d74022feda7cdedf2d6f6e5b4ab134d4716606287ceb2740a8717f226bd2"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 7804b5794233654294b743558dd31267f1fe1747ed6c183a9b12cda984334c5a
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
      "id": 10,
      "user_id": 58,
      "feedbackable_id": 1,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:25:34.065Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 62,
      "feedbackable_id": 2,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:25:34.349Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 12,
      "user_id": 66,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:25:34.622Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 70,
      "feedbackable_id": 4,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:25:34.898Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 14,
      "user_id": 74,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T13:25:35.174Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7804b5794233654294b743558dd31267f1fe1747ed6c183a9b12cda984334c5a"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer ab8c4c5420e065533d393c6bea704c56fb5c164c502181e662de8bfaac749fa7
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
      "id": 28,
      "user_id": 132,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T13:25:39.313Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab8c4c5420e065533d393c6bea704c56fb5c164c502181e662de8bfaac749fa7"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/14
Content-Type: application/json
Authorization: Bearer bba2514eb0d8e2401f929fb0904c73b169ca7fa6c77e5095437a2a4057b6b81c
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/14" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bba2514eb0d8e2401f929fb0904c73b169ca7fa6c77e5095437a2a4057b6b81c"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/18/metadata
Content-Type: application/json
Authorization: Bearer 71ed1b90595010f443417c08c9fa9f03f56e598d5c44e49a36342a136b7a87cd
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
    "id": 18,
    "uploader": {
      "id": 621,
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
      "created_at": "2016-11-17T13:26:19.045Z",
      "updated_at": "2016-11-17T13:26:19.045Z"
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
    "created_at": "2016-11-17T13:26:19.117Z",
    "updated_at": "2016-11-17T13:26:19.117Z",
    "course_id": 203,
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
curl "api.goskive.com/v2/files/18/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 71ed1b90595010f443417c08c9fa9f03f56e598d5c44e49a36342a136b7a87cd"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/24/feedbacks
Content-Type: application/json
Authorization: Bearer f36764b2dc84b6c87b179f2ef3738db279445a4f361753e27602d1b3560eea25
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
      "id": 40,
      "user_id": 507,
      "feedbackable_id": 24,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:11.184Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 506,
      "feedbackable_id": 24,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:11.174Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/24/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f36764b2dc84b6c87b179f2ef3738db279445a4f361753e27602d1b3560eea25"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 0974d8e291631ca60a06b65e83a95efa4de5f5ae588093e4c5dd2e59970c7fa9
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
      "id": 48,
      "obfuscated_id": "oqXJ8Hi_AE4",
      "author_id": 700,
      "chapter_id": 108,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.443Z",
      "created_at": "2016-11-17T13:26:24.443Z",
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
      "id": 49,
      "obfuscated_id": "GNsH7ObIVl0",
      "author_id": 703,
      "chapter_id": 109,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.584Z",
      "created_at": "2016-11-17T13:26:24.584Z",
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
      "id": 50,
      "obfuscated_id": "3_Ybw_gc_HE",
      "author_id": 706,
      "chapter_id": 110,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.719Z",
      "created_at": "2016-11-17T13:26:24.719Z",
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
      "id": 51,
      "obfuscated_id": "fXx2Zpse_KI",
      "author_id": 709,
      "chapter_id": 111,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.856Z",
      "created_at": "2016-11-17T13:26:24.856Z",
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
      "id": 52,
      "obfuscated_id": "_rmh4zxMC_8",
      "author_id": 712,
      "chapter_id": 112,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.997Z",
      "created_at": "2016-11-17T13:26:24.997Z",
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
	-H "Authorization: Bearer 0974d8e291631ca60a06b65e83a95efa4de5f5ae588093e4c5dd2e59970c7fa9"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 9dea72e96a0f7d2c16f4ad19951ade2c26ce6548dcb4e3dd86ac77ab9fd54e33
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
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 696,
      "chapter_id": 107,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:24.268Z",
      "created_at": "2016-11-17T13:26:24.268Z",
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
	-H "Authorization: Bearer 9dea72e96a0f7d2c16f4ad19951ade2c26ce6548dcb4e3dd86ac77ab9fd54e33"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/34/republish
Content-Type: application/json
Authorization: Bearer 2719cb55f80a47d06df743163fffe3f3b60ae5c0bfb301b1c8257cf6c731139c
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/34/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2719cb55f80a47d06df743163fffe3f3b60ae5c0bfb301b1c8257cf6c731139c"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/58/feedbacks
Content-Type: application/json
Authorization: Bearer d8c9d302a184b98f13f9b1470c680333ea1c82c71d3f7e51ddfd1b29271c0c38
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
      "id": 32,
      "user_id": 342,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:01.638Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 341,
      "feedbackable_id": 58,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T13:26:01.628Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/58/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d8c9d302a184b98f13f9b1470c680333ea1c82c71d3f7e51ddfd1b29271c0c38"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 1e6c3388a8b4d93fe1406185ba2769c1aa2490ed5363fc4b5d5526e56bfe5809
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
      "author_id": 931,
      "chapter_id": 181,
      "position": 112,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:50.139Z",
      "created_at": "2016-11-17T13:26:50.025Z",
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
          "id": 249,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 250,
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
      "author_id": 934,
      "chapter_id": 182,
      "position": 113,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:50.405Z",
      "created_at": "2016-11-17T13:26:50.293Z",
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
          "id": 251,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 252,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 125,
      "obfuscated_id": "K6zw0Yc6Me8",
      "author_id": 937,
      "chapter_id": 183,
      "position": 114,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:50.674Z",
      "created_at": "2016-11-17T13:26:50.559Z",
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
          "id": 253,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 254,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 126,
      "obfuscated_id": "fKTMLttUR-w",
      "author_id": 940,
      "chapter_id": 184,
      "position": 115,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:50.945Z",
      "created_at": "2016-11-17T13:26:50.830Z",
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
      "author_id": 943,
      "chapter_id": 185,
      "position": 116,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:51.206Z",
      "created_at": "2016-11-17T13:26:51.098Z",
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
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1e6c3388a8b4d93fe1406185ba2769c1aa2490ed5363fc4b5d5526e56bfe5809"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer d6db7d088566222d6c29a453c29887400fc7b1c06621dbfd2f8afb01c1fad857
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
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 911,
      "chapter_id": 175,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T13:26:48.388Z",
      "created_at": "2016-11-17T13:26:48.280Z",
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
          "id": 237,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 238,
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
	-H "Authorization: Bearer d6db7d088566222d6c29a453c29887400fc7b1c06621dbfd2f8afb01c1fad857"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/109/republish
Content-Type: application/json
Authorization: Bearer 9cd501a643f8478c21e4010dca24b5bf908eb375d36d3c4ae06ac0d98eb206d0
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/109/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9cd501a643f8478c21e4010dca24b5bf908eb375d36d3c4ae06ac0d98eb206d0"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3e7028dc2fa17e5c0d7eec1fd9d3e83b990445c0d51c5969a41d276426abf933
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":157,"published":false}}
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
    "creator_id": 538,
    "id": 150,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 156,
    "additional_university_ids": [

    ],
    "discipline_id": 158,
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
    "updated_at": "2016-11-17T13:26:12.717Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 157,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":157,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e7028dc2fa17e5c0d7eec1fd9d3e83b990445c0d51c5969a41d276426abf933"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 78320efb9715a7d35a6feb575449c4cb8f453e7e131eafeb9f72c6445da7bc0d
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
      "creator_id": 545,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-132",
      "html_url": "https://goskive.com/course/fu-course-132",
      "slug": "fu-course-132",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 165,
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
      "updated_at": "2016-11-17T13:26:13.579Z",
      "shortname": "fu-course-132",
      "topic_id": 164,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 132",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 545,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-133",
      "html_url": "https://goskive.com/course/fu-course-133",
      "slug": "fu-course-133",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 166,
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
      "updated_at": "2016-11-17T13:26:13.622Z",
      "shortname": "fu-course-133",
      "topic_id": 165,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 133",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 546,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-134",
      "html_url": "https://goskive.com/course/fu-course-134",
      "slug": "fu-course-134",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 167,
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
      "updated_at": "2016-11-17T13:26:13.673Z",
      "shortname": "fu-course-134",
      "topic_id": 166,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 134",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 546,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-135",
      "html_url": "https://goskive.com/course/fu-course-135",
      "slug": "fu-course-135",
      "university_id": 161,
      "additional_university_ids": [

      ],
      "discipline_id": 168,
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
      "chapters_updated_at": "2016-11-17T13:26:13.513Z",
      "updated_at": "2016-11-17T13:26:14.015Z",
      "shortname": "fu-course-135",
      "topic_id": 167,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 135",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 78320efb9715a7d35a6feb575449c4cb8f453e7e131eafeb9f72c6445da7bc0d"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c713dfd622e7218bae04478ef65baf10a372f260a46401bb78aa340013290c62
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
      "creator_id": 552,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-136",
      "html_url": "https://goskive.com/course/fu-course-136",
      "slug": "fu-course-136",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 169,
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
      "updated_at": "2016-11-17T13:26:14.231Z",
      "shortname": "fu-course-136",
      "topic_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 136",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 552,
      "id": 162,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-137",
      "html_url": "https://goskive.com/course/fu-course-137",
      "slug": "fu-course-137",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 170,
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
      "updated_at": "2016-11-17T13:26:14.269Z",
      "shortname": "fu-course-137",
      "topic_id": 169,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 137",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 553,
      "id": 163,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-138",
      "html_url": "https://goskive.com/course/fu-course-138",
      "slug": "fu-course-138",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 171,
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
      "updated_at": "2016-11-17T13:26:14.315Z",
      "shortname": "fu-course-138",
      "topic_id": 170,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 138",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 553,
      "id": 164,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-139",
      "html_url": "https://goskive.com/course/fu-course-139",
      "slug": "fu-course-139",
      "university_id": 163,
      "additional_university_ids": [

      ],
      "discipline_id": 172,
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
      "updated_at": "2016-11-17T13:26:14.354Z",
      "shortname": "fu-course-139",
      "topic_id": 171,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 139",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c713dfd622e7218bae04478ef65baf10a372f260a46401bb78aa340013290c62"
```
