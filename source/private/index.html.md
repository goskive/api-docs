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
DELETE /v2/chapters/136
Content-Type: application/json
Authorization: Bearer d7a96eac20a8044eb058370106a988a8fe7632222ff6622db440cd09abdcb1c6
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/136" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d7a96eac20a8044eb058370106a988a8fe7632222ff6622db440cd09abdcb1c6"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/142
Content-Type: application/json
Authorization: Bearer 2ac9d5364b48dbb41a7caeaf1de563bc82c1de6d084cc2c33e90839dbb378274
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
    "id": 142,
    "updated_at": "2016-11-18T10:56:39.091Z",
    "course_id": 203,
    "author_id": 604,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-18T10:56:38.554Z",
    "questions_updated_at": "2016-11-18T10:56:38.554Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 77,
        "obfuscated_id": "v-Dlx6JosLA",
        "author_id": 607,
        "chapter_id": 142,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:39.037Z",
        "created_at": "2016-11-18T10:56:39.037Z",
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
        "id": 78,
        "obfuscated_id": "-wsYNe2w7uo",
        "author_id": 608,
        "chapter_id": 142,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:39.074Z",
        "created_at": "2016-11-18T10:56:39.074Z",
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
        "author_id": 605,
        "chapter_id": 142,
        "position": 87,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:38.776Z",
        "created_at": "2016-11-18T10:56:38.667Z",
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
            "id": 192,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 193,
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
        "author_id": 606,
        "chapter_id": 142,
        "position": 88,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:38.969Z",
        "created_at": "2016-11-18T10:56:38.850Z",
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
      }
    ],
    "title": "Flour and eggs",
    "position": 1
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/142" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ac9d5364b48dbb41a7caeaf1de563bc82c1de6d084cc2c33e90839dbb378274"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/138
Content-Type: application/json
Authorization: Bearer 607c083a4da01142e60c35b34407b6d1b0a1ea35eb20e3a07d0e2f5ca5d61d68
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
    "id": 138,
    "updated_at": "2016-11-18T10:56:37.295Z",
    "course_id": 199,
    "author_id": 589,
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
curl "api.goskive.com/v2/chapters/138" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 607c083a4da01142e60c35b34407b6d1b0a1ea35eb20e3a07d0e2f5ca5d61d68"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer 63d9ccd066e89abff9685c1916bbd7b2aa0a61b70a9dc778373e4d1e92b8f6fc
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
	-H "Authorization: Bearer 63d9ccd066e89abff9685c1916bbd7b2aa0a61b70a9dc778373e4d1e92b8f6fc"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 23d938567279f084b5c770ed5d141da6685a69d7bd09326566259174f70671cb
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
      "id": 12,
      "author_id": 647,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:42.069Z",
      "status": "published",
      "subject_id": 215,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 649,
      "reply_to_id": 12,
      "created_at": "2016-11-18T10:56:42.159Z",
      "status": "published",
      "subject_id": 216,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 651,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:42.278Z",
      "status": "published",
      "subject_id": 217,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 653,
      "reply_to_id": 14,
      "created_at": "2016-11-18T10:56:42.362Z",
      "status": "published",
      "subject_id": 218,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 655,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:42.449Z",
      "status": "reported",
      "subject_id": 219,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 657,
      "reply_to_id": 16,
      "created_at": "2016-11-18T10:56:42.540Z",
      "status": "published",
      "subject_id": 220,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 659,
      "reply_to_id": 16,
      "created_at": "2016-11-18T10:56:42.622Z",
      "status": "published",
      "subject_id": 221,
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
	-H "Authorization: Bearer 23d938567279f084b5c770ed5d141da6685a69d7bd09326566259174f70671cb"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 1a0ddafd3876f7c000d1f7ac22e2ea0c271487658b22c70162987e9d0f4bcdd2
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
      "id": 33,
      "author_id": 692,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:44.037Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 694,
      "reply_to_id": 33,
      "created_at": "2016-11-18T10:56:44.121Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 696,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:44.207Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 698,
      "reply_to_id": 35,
      "created_at": "2016-11-18T10:56:44.351Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 700,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:44.437Z",
      "status": "reported",
      "subject_id": 240,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 702,
      "reply_to_id": 37,
      "created_at": "2016-11-18T10:56:44.523Z",
      "status": "published",
      "subject_id": 241,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 704,
      "reply_to_id": 37,
      "created_at": "2016-11-18T10:56:44.609Z",
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
curl "api.goskive.com/v2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a0ddafd3876f7c000d1f7ac22e2ea0c271487658b22c70162987e9d0f4bcdd2"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer de833d1cfda62278bb5880b47da7c09bb5185547192e2dfe17dda82d2f5d1dca
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
      "id": 27,
      "author_id": 679,
      "reply_to_id": 26,
      "created_at": "2016-11-18T10:56:43.486Z",
      "status": "published",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 683,
      "reply_to_id": 28,
      "created_at": "2016-11-18T10:56:43.650Z",
      "status": "published",
      "subject_id": 232,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 687,
      "reply_to_id": 30,
      "created_at": "2016-11-18T10:56:43.819Z",
      "status": "published",
      "subject_id": 234,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 689,
      "reply_to_id": 30,
      "created_at": "2016-11-18T10:56:43.902Z",
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
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de833d1cfda62278bb5880b47da7c09bb5185547192e2dfe17dda82d2f5d1dca"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 19bffcba8648a553e08d14a622fa6b0b25a4b9862e7181a5ef29d7524b224f71
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
      "id": 44,
      "author_id": 715,
      "reply_to_id": null,
      "created_at": "2016-11-18T10:56:45.117Z",
      "status": "reported",
      "subject_id": 247,
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
	-H "Authorization: Bearer 19bffcba8648a553e08d14a622fa6b0b25a4b9862e7181a5ef29d7524b224f71"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/50/republish
Content-Type: application/json
Authorization: Bearer d8dd13c31ae0aa5c70bb98a8b785fdb82c1e65494acb9221d283fa4c1aef121a
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
	-H "Authorization: Bearer d8dd13c31ae0aa5c70bb98a8b785fdb82c1e65494acb9221d283fa4c1aef121a"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 498fff25b1c8103df17f4a2bacc66d925b02ff0f0a771ea6f1ce1469768c7797
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
    "id": 43,
    "updated_at": "2016-11-18T10:56:01.804Z",
    "course_id": 84,
    "author_id": 186,
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
	-H "Authorization: Bearer 498fff25b1c8103df17f4a2bacc66d925b02ff0f0a771ea6f1ce1469768c7797"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/86/chapters
Content-Type: application/json
Authorization: Bearer eaa7e388760f9a9591b2b5528d5eaecbdb5be9aa49bcab0a1b496dd288f1f3a5
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
    "id": 44,
    "updated_at": "2016-11-18T10:56:02.104Z",
    "course_id": 86,
    "author_id": 190,
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
curl "api.goskive.com/v2/courses/86/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eaa7e388760f9a9591b2b5528d5eaecbdb5be9aa49bcab0a1b496dd288f1f3a5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e2f190db2a09f20a0aba215169344ee7bfe38c7aeb7c2e6be0948bf1ac07c2c1
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
      "id": 60,
      "updated_at": "2016-11-18T10:56:04.186Z",
      "course_id": 95,
      "author_id": 224,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 54",
      "position": 1
    },
    {
      "id": 61,
      "updated_at": "2016-11-18T10:56:04.218Z",
      "course_id": 95,
      "author_id": 225,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 55",
      "position": 2
    },
    {
      "id": 62,
      "updated_at": "2016-11-18T10:56:04.520Z",
      "course_id": 95,
      "author_id": 226,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-18T10:56:04.104Z",
      "questions_updated_at": "2016-11-18T10:56:04.104Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 56",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2f190db2a09f20a0aba215169344ee7bfe38c7aeb7c2e6be0948bf1ac07c2c1"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 1a03a0655b7aa04da682159b8c949b3f9ca8aba072ed1fe18d92ea9d315ebe9c
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
      "id": 63,
      "updated_at": "2016-11-18T10:56:04.880Z",
      "course_id": 97,
      "author_id": 233,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 57",
      "position": 1
    },
    {
      "id": 64,
      "updated_at": "2016-11-18T10:56:04.905Z",
      "course_id": 97,
      "author_id": 234,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 58",
      "position": 2
    },
    {
      "id": 65,
      "updated_at": "2016-11-18T10:56:04.930Z",
      "course_id": 97,
      "author_id": 235,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 59",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a03a0655b7aa04da682159b8c949b3f9ca8aba072ed1fe18d92ea9d315ebe9c"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/161
Content-Type: application/json
Authorization: Bearer 048b95509eb9eb47bf4770cfafab8f277f1701c96b3b9cb36403d3cb25e0fe1d
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/161" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 048b95509eb9eb47bf4770cfafab8f277f1701c96b3b9cb36403d3cb25e0fe1d"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 7cb72f7df3bbbf9d9f762142b02a2e0112a8fe08e0ddb2926523dfbdc55ad9ae
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
	-H "Authorization: Bearer 7cb72f7df3bbbf9d9f762142b02a2e0112a8fe08e0ddb2926523dfbdc55ad9ae"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 5e1f7eafe212afbb52c5d46a5ba8ee75c65479974cb2b9f92cd05b7938618bff
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
    "creator_id": 438,
    "id": 153,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 136,
    "additional_university_ids": [

    ],
    "discipline_id": 159,
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
    "chapters_updated_at": "2016-11-18T10:56:22.398Z",
    "updated_at": "2016-11-18T10:56:23.842Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 438,
        "chapter_id": 113,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.633Z",
        "created_at": "2016-11-18T10:56:23.633Z",
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
        "id": 45,
        "obfuscated_id": "IVleRnyZemc",
        "author_id": 438,
        "chapter_id": 114,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.703Z",
        "created_at": "2016-11-18T10:56:23.703Z",
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
        "author_id": 438,
        "chapter_id": 113,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.672Z",
        "created_at": "2016-11-18T10:56:23.672Z",
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
        "id": 46,
        "obfuscated_id": "urkHiAaH08E",
        "author_id": 438,
        "chapter_id": 114,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.743Z",
        "created_at": "2016-11-18T10:56:23.743Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 441,
        "chapter_id": 113,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.782Z",
        "created_at": "2016-11-18T10:56:23.782Z",
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
        "id": 48,
        "obfuscated_id": "oqXJ8Hi_AE4",
        "author_id": 442,
        "chapter_id": 114,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-18T10:56:23.824Z",
        "created_at": "2016-11-18T10:56:23.824Z",
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
        "id": 113,
        "updated_at": "2016-11-18T10:56:23.793Z",
        "course_id": 153,
        "author_id": 438,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-18T10:56:22.398Z",
        "questions_updated_at": "2016-11-18T10:56:22.398Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 107",
        "position": 1
      },
      {
        "id": 114,
        "updated_at": "2016-11-18T10:56:23.834Z",
        "course_id": 153,
        "author_id": 438,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-18T10:56:22.398Z",
        "questions_updated_at": "2016-11-18T10:56:22.398Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 108",
        "position": 2
      }
    ],
    "topic_id": 158,
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
	-H "Authorization: Bearer 5e1f7eafe212afbb52c5d46a5ba8ee75c65479974cb2b9f92cd05b7938618bff"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/157
Content-Type: application/json
Authorization: Bearer fdad1e54d57362c74dd9581a5fe22792fa6aa5b08a6071fca00b8e11f490f3a8
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
    "creator_id": 457,
    "id": 157,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 140,
    "additional_university_ids": [

    ],
    "discipline_id": 163,
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
    "updated_at": "2016-11-18T10:56:27.194Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 162,
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
curl "api.goskive.com/v2/courses/157" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fdad1e54d57362c74dd9581a5fe22792fa6aa5b08a6071fca00b8e11f490f3a8"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 22d6a19328c979e42058542f3613b34dd113152894b006225a5c14ac83a4999f
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
    "creator_id": 462,
    "id": 160,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 143,
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
    "updated_at": "2016-11-18T10:56:27.674Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 165,
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
	-H "Authorization: Bearer 22d6a19328c979e42058542f3613b34dd113152894b006225a5c14ac83a4999f"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 6f357c3fc4956202ac7a05d9c1f9fc8d43a1872544532acbdbdf8a15ac768f9a
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
      "id": 32,
      "user_id": 897,
      "feedbackable_id": 118,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:58.622Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 901,
      "feedbackable_id": 119,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:58.909Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 905,
      "feedbackable_id": 120,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:59.207Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 909,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:59.505Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 913,
      "feedbackable_id": 122,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-18T10:56:59.803Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6f357c3fc4956202ac7a05d9c1f9fc8d43a1872544532acbdbdf8a15ac768f9a"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 70484a90f22e07b31572eaba53071a6c831345d6a216e56dab0918baf37dfac8
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
      "id": 31,
      "user_id": 892,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-18T10:56:58.290Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70484a90f22e07b31572eaba53071a6c831345d6a216e56dab0918baf37dfac8"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/17
Content-Type: application/json
Authorization: Bearer 96a129e502609f1431638884213aab922a81b289a64074a89cd5fa1f665b9681
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/17" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 96a129e502609f1431638884213aab922a81b289a64074a89cd5fa1f665b9681"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/21/metadata
Content-Type: application/json
Authorization: Bearer 0f753a87244767eb94457770c79e093c268042d7e35f15a79e7127a6e9d6f2f4
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
    "id": 21,
    "uploader": {
      "id": 766,
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
      "created_at": "2016-11-18T10:56:47.705Z",
      "updated_at": "2016-11-18T10:56:47.705Z"
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
    "created_at": "2016-11-18T10:56:47.780Z",
    "updated_at": "2016-11-18T10:56:47.780Z",
    "course_id": 266,
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
curl "api.goskive.com/v2/files/21/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0f753a87244767eb94457770c79e093c268042d7e35f15a79e7127a6e9d6f2f4"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/66/feedbacks
Content-Type: application/json
Authorization: Bearer fa6b6c286cf505842d2857dd5829c49a65ee854780bc8b9b261c54db01a77f94
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
      "id": 12,
      "user_id": 497,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:30.227Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 11,
      "user_id": 496,
      "feedbackable_id": 66,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:30.216Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/66/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fa6b6c286cf505842d2857dd5829c49a65ee854780bc8b9b261c54db01a77f94"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 2b48499053fbcaa1e65b1e570ce81c032b99f7ecf7d9b5260a79b0dbd6631c70
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
      "id": 11,
      "obfuscated_id": "KS_N8rRWCuE",
      "author_id": 307,
      "chapter_id": 81,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:11.191Z",
      "created_at": "2016-11-18T10:56:11.191Z",
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
      "id": 12,
      "obfuscated_id": "4vzz6KHlMwo",
      "author_id": 310,
      "chapter_id": 82,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:11.317Z",
      "created_at": "2016-11-18T10:56:11.317Z",
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 313,
      "chapter_id": 83,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:11.448Z",
      "created_at": "2016-11-18T10:56:11.448Z",
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 316,
      "chapter_id": 84,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:11.578Z",
      "created_at": "2016-11-18T10:56:11.578Z",
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 319,
      "chapter_id": 85,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:11.710Z",
      "created_at": "2016-11-18T10:56:11.710Z",
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
	-H "Authorization: Bearer 2b48499053fbcaa1e65b1e570ce81c032b99f7ecf7d9b5260a79b0dbd6631c70"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer c05dee1d436fbc2e43c8f554f2597c5708444e0ef79fb79cf2bad4f755550862
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 351,
      "chapter_id": 95,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:56:13.135Z",
      "created_at": "2016-11-18T10:56:13.135Z",
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
	-H "Authorization: Bearer c05dee1d436fbc2e43c8f554f2597c5708444e0ef79fb79cf2bad4f755550862"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/28/republish
Content-Type: application/json
Authorization: Bearer 5be380fcfdf0731aeb2cd871f5937629a486fd776adc8a6185be828f52f95a96
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/28/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5be380fcfdf0731aeb2cd871f5937629a486fd776adc8a6185be828f52f95a96"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/53/feedbacks
Content-Type: application/json
Authorization: Bearer 1515e89df532ab710cc3a141c6a1a9474c07e9634f64c96dce71ab1dd22d2a51
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
      "id": 8,
      "user_id": 290,
      "feedbackable_id": 53,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:10.004Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 289,
      "feedbackable_id": 53,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-18T10:56:09.993Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/53/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1515e89df532ab710cc3a141c6a1a9474c07e9634f64c96dce71ab1dd22d2a51"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 46026569746799e73dc67d42b168083de64bbfcf077eda8ae829ea7a9eff5a03
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 136,
      "chapter_id": 30,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:55.761Z",
      "created_at": "2016-11-18T10:55:55.627Z",
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
          "id": 53,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 54,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 127,
      "chapter_id": 27,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:54.877Z",
      "created_at": "2016-11-18T10:55:54.749Z",
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
          "id": 47,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 48,
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
      "author_id": 130,
      "chapter_id": 28,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:55.169Z",
      "created_at": "2016-11-18T10:55:55.040Z",
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
    },
    {
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 133,
      "chapter_id": 29,
      "position": 26,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:55.463Z",
      "created_at": "2016-11-18T10:55:55.331Z",
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
          "id": 51,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 52,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 139,
      "chapter_id": 31,
      "position": 28,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:56.050Z",
      "created_at": "2016-11-18T10:55:55.925Z",
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
          "id": 55,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 56,
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
	-H "Authorization: Bearer 46026569746799e73dc67d42b168083de64bbfcf077eda8ae829ea7a9eff5a03"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c1c6e12466e41bff0f5267f2e8b35d836f81a98c28879893affccc8574bba654
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 107,
      "chapter_id": 21,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-18T10:55:53.033Z",
      "created_at": "2016-11-18T10:55:52.908Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1c6e12466e41bff0f5267f2e8b35d836f81a98c28879893affccc8574bba654"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/36/republish
Content-Type: application/json
Authorization: Bearer 8a8190916a4fe942baf39f9cea868f76efd05d1567b45da503184464541d4c82
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/36/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a8190916a4fe942baf39f9cea868f76efd05d1567b45da503184464541d4c82"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f1f34a30c338854e1e92d45eb81533833127558f835bdd9fe62e16530e212cf1
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":4,"published":false}}
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
    "creator_id": 5,
    "id": 4,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 4,
    "additional_university_ids": [

    ],
    "discipline_id": 4,
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
    "updated_at": "2016-11-18T10:55:43.947Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 4,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":4,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f1f34a30c338854e1e92d45eb81533833127558f835bdd9fe62e16530e212cf1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0b6a76cc4d354a35b47a5f37fb5e3d3742540c8cd21717dfebd4a96a2255ab80
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
      "creator_id": 10,
      "id": 9,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-5",
      "html_url": "https://goskive.com/course/fu-course-5",
      "slug": "fu-course-5",
      "university_id": 7,
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
      "updated_at": "2016-11-18T10:55:44.363Z",
      "shortname": "fu-course-5",
      "topic_id": 9,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 10,
      "id": 10,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-6",
      "html_url": "https://goskive.com/course/fu-course-6",
      "slug": "fu-course-6",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "discipline_id": 10,
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
      "updated_at": "2016-11-18T10:55:44.401Z",
      "shortname": "fu-course-6",
      "topic_id": 10,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 11,
      "id": 11,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 7,
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
      "updated_at": "2016-11-18T10:55:44.445Z",
      "shortname": "fu-course-7",
      "topic_id": 11,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 11,
      "id": 12,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 7,
      "additional_university_ids": [

      ],
      "discipline_id": 12,
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
      "chapters_updated_at": "2016-11-18T10:55:44.310Z",
      "updated_at": "2016-11-18T10:55:44.812Z",
      "shortname": "fu-course-8",
      "topic_id": 12,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 8",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0b6a76cc4d354a35b47a5f37fb5e3d3742540c8cd21717dfebd4a96a2255ab80"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b411bfc44411451da09079d326b8713ad086ad899d4ec212f1404f6d465a48cd
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
      "creator_id": 16,
      "id": 13,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-9",
      "html_url": "https://goskive.com/course/fu-course-9",
      "slug": "fu-course-9",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "discipline_id": 13,
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
      "updated_at": "2016-11-18T10:55:44.974Z",
      "shortname": "fu-course-9",
      "topic_id": 13,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 9",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 16,
      "id": 14,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-10",
      "html_url": "https://goskive.com/course/fu-course-10",
      "slug": "fu-course-10",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "discipline_id": 14,
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
      "updated_at": "2016-11-18T10:55:45.017Z",
      "shortname": "fu-course-10",
      "topic_id": 14,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 10",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 17,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "discipline_id": 15,
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
      "updated_at": "2016-11-18T10:55:45.062Z",
      "shortname": "fu-course-11",
      "topic_id": 15,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 17,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 8,
      "additional_university_ids": [

      ],
      "discipline_id": 16,
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
      "updated_at": "2016-11-18T10:55:45.100Z",
      "shortname": "fu-course-12",
      "topic_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 12",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b411bfc44411451da09079d326b8713ad086ad899d4ec212f1404f6d465a48cd"
```
