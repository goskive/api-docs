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
DELETE /v2/chapters/155
Content-Type: application/json
Authorization: Bearer fffa5e3eea5aef7613d680a1f97db965727b1f5cd562ab691eacf5f8520897d8
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/155" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fffa5e3eea5aef7613d680a1f97db965727b1f5cd562ab691eacf5f8520897d8"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/151
Content-Type: application/json
Authorization: Bearer cf7f288fde5a73364a83ce027d4e4896bae18ad5537bad95d8716e11ad0a5d9f
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
    "id": 151,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-01T13:39:04.374Z",
    "course_id": 248,
    "author_id": 748,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2015-03-12T14:00:00.000Z",
    "questions_updated_at": "2015-04-12T14:00:00.000Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 751,
        "chapter_id": 151,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T14:00:00.000Z",
        "created_at": "2016-09-01T13:39:04.340Z",
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
        "author_id": 752,
        "chapter_id": 151,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-03-12T13:59:00.000Z",
        "created_at": "2016-09-01T13:39:04.369Z",
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
        "id": 112,
        "obfuscated_id": "7Qwj1ZvbWUI",
        "author_id": 749,
        "chapter_id": 151,
        "position": 99,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T14:00:00.000Z",
        "created_at": "2016-09-01T13:39:04.189Z",
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
            "id": 227,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 228,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 113,
        "obfuscated_id": "pcyz_ZHBlMU",
        "author_id": 750,
        "chapter_id": 151,
        "position": 100,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2015-04-12T13:59:00.000Z",
        "created_at": "2016-09-01T13:39:04.266Z",
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
}
```



```shell
curl "api.goskive.com/v2/chapters/151" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf7f288fde5a73364a83ce027d4e4896bae18ad5537bad95d8716e11ad0a5d9f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/153
Content-Type: application/json
Authorization: Bearer 53632cf1f71efacdcd59a79405d4455a88eb4374fe8cee287c726a29c850032e
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
    "id": 153,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-01T13:39:04.762Z",
    "course_id": 250,
    "author_id": 757,
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
curl "api.goskive.com/v2/chapters/153" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 53632cf1f71efacdcd59a79405d4455a88eb4374fe8cee287c726a29c850032e"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/2
Content-Type: application/json
Authorization: Bearer 991d57e8f178f03d3cb0a218769a0c267cf4b2425e9fb73e3847e93666249e7b
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
	-H "Authorization: Bearer 991d57e8f178f03d3cb0a218769a0c267cf4b2425e9fb73e3847e93666249e7b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer df793e8864be45efe98c240cba7eaa7b6c5f72b9d30a01010ec147700bfa420e
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
      "author_id": 60,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:19.022Z",
      "status": "published",
      "subject_id": 21,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 5,
      "author_id": 62,
      "reply_to_id": 4,
      "created_at": "2016-09-01T13:38:19.112Z",
      "status": "published",
      "subject_id": 22,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 6,
      "author_id": 64,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:19.201Z",
      "status": "published",
      "subject_id": 23,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 7,
      "author_id": 66,
      "reply_to_id": 6,
      "created_at": "2016-09-01T13:38:19.289Z",
      "status": "published",
      "subject_id": 24,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 8,
      "author_id": 68,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:19.377Z",
      "status": "reported",
      "subject_id": 25,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 70,
      "reply_to_id": 8,
      "created_at": "2016-09-01T13:38:19.462Z",
      "status": "published",
      "subject_id": 26,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 72,
      "reply_to_id": 8,
      "created_at": "2016-09-01T13:38:19.547Z",
      "status": "published",
      "subject_id": 27,
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
	-H "Authorization: Bearer df793e8864be45efe98c240cba7eaa7b6c5f72b9d30a01010ec147700bfa420e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 7ab2651970bf81c615ed1eb87f8fcd30d5966f88a60dc26453b3d9af9e48ea95
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
      "author_id": 75,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:19.694Z",
      "status": "published",
      "subject_id": 28,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 77,
      "reply_to_id": 11,
      "created_at": "2016-09-01T13:38:19.781Z",
      "status": "published",
      "subject_id": 29,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 79,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:19.869Z",
      "status": "published",
      "subject_id": 30,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 81,
      "reply_to_id": 13,
      "created_at": "2016-09-01T13:38:19.958Z",
      "status": "published",
      "subject_id": 31,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 83,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:20.048Z",
      "status": "reported",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 85,
      "reply_to_id": 15,
      "created_at": "2016-09-01T13:38:20.137Z",
      "status": "published",
      "subject_id": 33,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 87,
      "reply_to_id": 15,
      "created_at": "2016-09-01T13:38:20.228Z",
      "status": "published",
      "subject_id": 34,
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
	-H "Authorization: Bearer 7ab2651970bf81c615ed1eb87f8fcd30d5966f88a60dc26453b3d9af9e48ea95"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer b55bec6a4f8312d631382cee306746440fd7895f02c802c71d9ba4af73e22b0c
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
      "author_id": 107,
      "reply_to_id": 25,
      "created_at": "2016-09-01T13:38:21.130Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 111,
      "reply_to_id": 27,
      "created_at": "2016-09-01T13:38:21.344Z",
      "status": "published",
      "subject_id": 45,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 115,
      "reply_to_id": 29,
      "created_at": "2016-09-01T13:38:21.527Z",
      "status": "published",
      "subject_id": 47,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 117,
      "reply_to_id": 29,
      "created_at": "2016-09-01T13:38:21.616Z",
      "status": "published",
      "subject_id": 48,
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
	-H "Authorization: Bearer b55bec6a4f8312d631382cee306746440fd7895f02c802c71d9ba4af73e22b0c"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 1fcbd8c16a4351288f648a8ecb337398e2e66ea97ff185586a5e45b85d214ea0
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
      "author_id": 128,
      "reply_to_id": null,
      "created_at": "2016-09-01T13:38:22.113Z",
      "status": "reported",
      "subject_id": 53,
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
	-H "Authorization: Bearer 1fcbd8c16a4351288f648a8ecb337398e2e66ea97ff185586a5e45b85d214ea0"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/41/republish
Content-Type: application/json
Authorization: Bearer ed45741bae78a929b774d8aca94d08bc9e1d80c9e4a8313b6eb4f3e67fe08ce7
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/41/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ed45741bae78a929b774d8aca94d08bc9e1d80c9e4a8313b6eb4f3e67fe08ce7"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/146/chapters
Content-Type: application/json
Authorization: Bearer 54e71b68c1756409c8f791b55ffb73829fc810eac7b6185be91ed541bcb35cd4
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
    "id": 77,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-01T13:38:46.044Z",
    "course_id": 146,
    "author_id": 449,
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
curl "api.goskive.com/v2/courses/146/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54e71b68c1756409c8f791b55ffb73829fc810eac7b6185be91ed541bcb35cd4"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 9385d289dce6e2a495d2b4f5203ff4140314eec373efc52da41f0c68009a7173
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
    "id": 78,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-01T13:38:46.313Z",
    "course_id": 148,
    "author_id": 453,
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
	-H "Authorization: Bearer 9385d289dce6e2a495d2b4f5203ff4140314eec373efc52da41f0c68009a7173"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ea69f232b1a4209d37a7f9407cd66c8737875d7ca4a261cbf6cde4d8cd55131e
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
      "id": 95,
      "title": "Clever Chapter Title 87",
      "position": 1,
      "updated_at": "2016-09-01T13:38:48.213Z",
      "course_id": 158,
      "author_id": 489,
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
      "id": 96,
      "title": "Clever Chapter Title 88",
      "position": 2,
      "updated_at": "2016-09-01T13:38:48.238Z",
      "course_id": 158,
      "author_id": 490,
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
      "id": 97,
      "title": "Clever Chapter Title 89",
      "position": 3,
      "updated_at": "2016-09-01T13:38:48.359Z",
      "course_id": 158,
      "author_id": 491,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-09-01T13:38:48.289Z",
      "questions_updated_at": "2016-09-01T13:38:48.349Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea69f232b1a4209d37a7f9407cd66c8737875d7ca4a261cbf6cde4d8cd55131e"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer bfe5e4eb5c4157ecd2db3fa473905ef8d943fc096e84b6b5bafcd249635328ca
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
      "id": 98,
      "title": "Clever Chapter Title 90",
      "position": 1,
      "updated_at": "2016-09-01T13:38:48.512Z",
      "course_id": 159,
      "author_id": 496,
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
      "id": 99,
      "title": "Clever Chapter Title 91",
      "position": 2,
      "updated_at": "2016-09-01T13:38:48.535Z",
      "course_id": 159,
      "author_id": 497,
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
      "id": 100,
      "title": "Clever Chapter Title 92",
      "position": 3,
      "updated_at": "2016-09-01T13:38:48.559Z",
      "course_id": 159,
      "author_id": 498,
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
	-H "Authorization: Bearer bfe5e4eb5c4157ecd2db3fa473905ef8d943fc096e84b6b5bafcd249635328ca"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 138b3c7882492d8f07230a372c050227828ccad11361c6dcaca9a7131a366c4b
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
	-H "Authorization: Bearer 138b3c7882492d8f07230a372c050227828ccad11361c6dcaca9a7131a366c4b"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/100
Content-Type: application/json
Authorization: Bearer cf8998d5f1b6a5ecc9cb54462aa848c0f8be298e52cd0eefbac658bc9211bae0
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/100" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf8998d5f1b6a5ecc9cb54462aa848c0f8be298e52cd0eefbac658bc9211bae0"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 573ff4eb959911603e8eda011e64528c838347cf2aaf1f9c8279adb38461958b
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
    "creator_id": 302,
    "id": 105,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 110,
    "additional_university_ids": [

    ],
    "topic_id": 108,
    "discipline_id": 108,
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
    "chapters_updated_at": "2016-09-01T13:38:34.558Z",
    "updated_at": "2016-09-01T13:38:34.561Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 50,
        "title": "Clever Chapter Title 50",
        "position": 1,
        "updated_at": "2016-09-01T13:38:34.527Z",
        "course_id": 105,
        "author_id": 302,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-01T13:38:34.523Z",
        "questions_updated_at": "2016-09-01T13:38:34.293Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 51,
        "title": "Clever Chapter Title 51",
        "position": 2,
        "updated_at": "2016-09-01T13:38:34.558Z",
        "course_id": 105,
        "author_id": 302,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-01T13:38:34.554Z",
        "questions_updated_at": "2016-09-01T13:38:34.359Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 302,
        "chapter_id": 50,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.410Z",
        "created_at": "2016-09-01T13:38:34.410Z",
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
        "author_id": 302,
        "chapter_id": 51,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.461Z",
        "created_at": "2016-09-01T13:38:34.461Z",
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
        "author_id": 302,
        "chapter_id": 50,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.434Z",
        "created_at": "2016-09-01T13:38:34.434Z",
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
        "author_id": 302,
        "chapter_id": 51,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.489Z",
        "created_at": "2016-09-01T13:38:34.489Z",
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
        "id": 25,
        "obfuscated_id": "HsmcIJXdRE4",
        "author_id": 305,
        "chapter_id": 50,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.523Z",
        "created_at": "2016-09-01T13:38:34.523Z",
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
        "author_id": 306,
        "chapter_id": 51,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-01T13:38:34.554Z",
        "created_at": "2016-09-01T13:38:34.554Z",
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
	-H "Authorization: Bearer 573ff4eb959911603e8eda011e64528c838347cf2aaf1f9c8279adb38461958b"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/110
Content-Type: application/json
Authorization: Bearer 98528146bcd1e76dbcb7d04d82df2b9f642945bc3b58184ad5bd5616a7a28907
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
    "creator_id": 315,
    "id": 110,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "topic_id": 113,
    "discipline_id": 113,
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
    "updated_at": "2016-09-01T13:38:35.349Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/110" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98528146bcd1e76dbcb7d04d82df2b9f642945bc3b58184ad5bd5616a7a28907"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 95b667829fb371307fdfeb5f40079f15958bc1a8c12c0552cff27858f8c4132b
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
    "creator_id": 312,
    "id": 108,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 113,
    "additional_university_ids": [

    ],
    "topic_id": 111,
    "discipline_id": 111,
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
    "updated_at": "2016-09-01T13:38:35.056Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95b667829fb371307fdfeb5f40079f15958bc1a8c12c0552cff27858f8c4132b"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 75413acd1755f86009e86f314efaed9d4fdfadafa8143e91788012da9ba5b01c
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
      "user_id": 622,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:57.328Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 626,
      "feedbackable_id": 92,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:57.504Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 630,
      "feedbackable_id": 93,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:57.680Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 634,
      "feedbackable_id": 94,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:57.860Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 638,
      "feedbackable_id": 95,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-01T13:38:58.063Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 75413acd1755f86009e86f314efaed9d4fdfadafa8143e91788012da9ba5b01c"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 3289a1745d1eec7111b8dbf89f6e4aec8d887a10e83fdac86e5e5eee07f60a8d
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
      "id": 42,
      "user_id": 696,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-01T13:39:00.621Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3289a1745d1eec7111b8dbf89f6e4aec8d887a10e83fdac86e5e5eee07f60a8d"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/41/feedbacks
Content-Type: application/json
Authorization: Bearer 5249119d53cd64c99acbbbd41bb38666cfe69dc48c847a8af7170dff4486e0f4
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
      "id": 17,
      "user_id": 439,
      "feedbackable_id": 41,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:44.116Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 438,
      "feedbackable_id": 41,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:44.101Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/41/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5249119d53cd64c99acbbbd41bb38666cfe69dc48c847a8af7170dff4486e0f4"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer dc7232d8f9cc4775166101522e199e547cd827c49d0d044bc09164e8f8006462
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
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 816,
      "chapter_id": 171,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:08.809Z",
      "created_at": "2016-09-01T13:39:08.809Z",
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
      "author_id": 819,
      "chapter_id": 172,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:08.934Z",
      "created_at": "2016-09-01T13:39:08.934Z",
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
      "author_id": 822,
      "chapter_id": 173,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:09.057Z",
      "created_at": "2016-09-01T13:39:09.057Z",
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
      "author_id": 825,
      "chapter_id": 174,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:09.183Z",
      "created_at": "2016-09-01T13:39:09.183Z",
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
      "author_id": 828,
      "chapter_id": 175,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:09.307Z",
      "created_at": "2016-09-01T13:39:09.307Z",
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
	-H "Authorization: Bearer dc7232d8f9cc4775166101522e199e547cd827c49d0d044bc09164e8f8006462"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 1b5cd73529e68af8ad41c0b0846f8d8bec4e26db526ba19fcf315731781e9cb7
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
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 844,
      "chapter_id": 180,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:39:09.996Z",
      "created_at": "2016-09-01T13:39:09.996Z",
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
	-H "Authorization: Bearer 1b5cd73529e68af8ad41c0b0846f8d8bec4e26db526ba19fcf315731781e9cb7"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/74/republish
Content-Type: application/json
Authorization: Bearer 996b25ed857f7d541906466719f5d47234355d0b4e5888b1fa6b1b53c7e0f161
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/74/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 996b25ed857f7d541906466719f5d47234355d0b4e5888b1fa6b1b53c7e0f161"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/34/feedbacks
Content-Type: application/json
Authorization: Bearer ddd2083e1ebf96a57f4a8b06d4d623e54d5c2228109aace88373fc738b39e03a
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
      "user_id": 245,
      "feedbackable_id": 34,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:28.960Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 244,
      "feedbackable_id": 34,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-01T13:38:28.947Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/34/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ddd2083e1ebf96a57f4a8b06d4d623e54d5c2228109aace88373fc738b39e03a"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 386e8ebb01cc83491b88091d9a65bae186658b0b5a06fe03b413dcba56ffeba4
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 179,
      "chapter_id": 18,
      "position": 9,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:25.636Z",
      "created_at": "2016-09-01T13:38:25.612Z",
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
          "id": 36,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 37,
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
      "author_id": 182,
      "chapter_id": 19,
      "position": 10,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:25.791Z",
      "created_at": "2016-09-01T13:38:25.767Z",
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
          "id": 38,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 39,
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
      "author_id": 176,
      "chapter_id": 17,
      "position": 8,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:25.484Z",
      "created_at": "2016-09-01T13:38:25.460Z",
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
          "id": 34,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 35,
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
      "author_id": 185,
      "chapter_id": 20,
      "position": 11,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:25.937Z",
      "created_at": "2016-09-01T13:38:25.914Z",
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
          "id": 40,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 41,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 21,
      "obfuscated_id": "XIvx1qd7-fY",
      "author_id": 188,
      "chapter_id": 21,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:26.087Z",
      "created_at": "2016-09-01T13:38:26.063Z",
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
          "id": 42,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 43,
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
	-H "Authorization: Bearer 386e8ebb01cc83491b88091d9a65bae186658b0b5a06fe03b413dcba56ffeba4"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer ca3d8f5979261928ffe2bf9253bb61eab08b9caf17e7c31bb370776595dbdaa2
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 204,
      "chapter_id": 26,
      "position": 17,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-01T13:38:26.945Z",
      "created_at": "2016-09-01T13:38:26.922Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ca3d8f5979261928ffe2bf9253bb61eab08b9caf17e7c31bb370776595dbdaa2"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/11/republish
Content-Type: application/json
Authorization: Bearer 660a302071c496306c65d4615a713318fb685acd3200dbfa74a602d6b6815713
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/11/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 660a302071c496306c65d4615a713318fb685acd3200dbfa74a602d6b6815713"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c984724948e8a7cbcedd5b33a99e88a95bbc45b63de50fcbae6aab2a9d9b7e5a
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":211,"published":false}}
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
    "creator_id": 561,
    "id": 203,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 187,
    "additional_university_ids": [

    ],
    "topic_id": 211,
    "discipline_id": 211,
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
    "updated_at": "2016-09-01T13:38:53.417Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":211,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c984724948e8a7cbcedd5b33a99e88a95bbc45b63de50fcbae6aab2a9d9b7e5a"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer e27771bc7654adc8f9eb1a518acd2eff6311fd8861423869b24a82c797cd695b
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
      "creator_id": 519,
      "id": 166,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-123",
      "html_url": "https://goskive.com/course/fu-course-123",
      "slug": "fu-course-123",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 174,
      "discipline_id": 174,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 123",
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
      "updated_at": "2016-09-01T13:38:49.936Z",
      "shortname": "fu-course-123"
    },
    {
      "creator_id": 519,
      "id": 167,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-124",
      "html_url": "https://goskive.com/course/fu-course-124",
      "slug": "fu-course-124",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 175,
      "discipline_id": 175,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 124",
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
      "updated_at": "2016-09-01T13:38:49.975Z",
      "shortname": "fu-course-124"
    },
    {
      "creator_id": 520,
      "id": 168,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-125",
      "html_url": "https://goskive.com/course/fu-course-125",
      "slug": "fu-course-125",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 176,
      "discipline_id": 176,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 125",
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
      "updated_at": "2016-09-01T13:38:50.027Z",
      "shortname": "fu-course-125"
    },
    {
      "creator_id": 520,
      "id": 169,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-126",
      "html_url": "https://goskive.com/course/fu-course-126",
      "slug": "fu-course-126",
      "university_id": 172,
      "additional_university_ids": [

      ],
      "topic_id": 177,
      "discipline_id": 177,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 126",
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
      "chapters_updated_at": "2016-09-01T13:38:50.187Z",
      "updated_at": "2016-09-01T13:38:50.189Z",
      "shortname": "fu-course-126"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e27771bc7654adc8f9eb1a518acd2eff6311fd8861423869b24a82c797cd695b"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 70564fb38b03df6e17d2752dd45cc0ac4760f6f998cfa0bdca344bbf3e042276
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
      "creator_id": 525,
      "id": 170,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-127",
      "html_url": "https://goskive.com/course/fu-course-127",
      "slug": "fu-course-127",
      "university_id": 173,
      "additional_university_ids": [

      ],
      "topic_id": 178,
      "discipline_id": 178,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 127",
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
      "updated_at": "2016-09-01T13:38:50.350Z",
      "shortname": "fu-course-127"
    },
    {
      "creator_id": 525,
      "id": 171,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-128",
      "html_url": "https://goskive.com/course/fu-course-128",
      "slug": "fu-course-128",
      "university_id": 173,
      "additional_university_ids": [

      ],
      "topic_id": 179,
      "discipline_id": 179,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 128",
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
      "updated_at": "2016-09-01T13:38:50.390Z",
      "shortname": "fu-course-128"
    },
    {
      "creator_id": 526,
      "id": 172,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-129",
      "html_url": "https://goskive.com/course/fu-course-129",
      "slug": "fu-course-129",
      "university_id": 173,
      "additional_university_ids": [

      ],
      "topic_id": 180,
      "discipline_id": 180,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 129",
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
      "updated_at": "2016-09-01T13:38:50.440Z",
      "shortname": "fu-course-129"
    },
    {
      "creator_id": 526,
      "id": 173,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-130",
      "html_url": "https://goskive.com/course/fu-course-130",
      "slug": "fu-course-130",
      "university_id": 173,
      "additional_university_ids": [

      ],
      "topic_id": 181,
      "discipline_id": 181,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 130",
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
      "updated_at": "2016-09-01T13:38:50.482Z",
      "shortname": "fu-course-130"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70564fb38b03df6e17d2752dd45cc0ac4760f6f998cfa0bdca344bbf3e042276"
```
