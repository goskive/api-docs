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
DELETE /v2/chapters/163
Content-Type: application/json
Authorization: Bearer 980dcf79b305327ff731615434b7c3580b3e6a45cead2d9a1819d3eda0f4c005
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/163" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 980dcf79b305327ff731615434b7c3580b3e6a45cead2d9a1819d3eda0f4c005"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/162
Content-Type: application/json
Authorization: Bearer c2390dd08ff8d789470a26881385e56fb21c941424aee2b467a5c659657f44db
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
    "id": 162,
    "updated_at": "2016-11-17T14:14:34.147Z",
    "course_id": 216,
    "author_id": 705,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-17T14:14:33.600Z",
    "questions_updated_at": "2016-11-17T14:14:33.600Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 64,
        "obfuscated_id": "H-V851w7HZg",
        "author_id": 708,
        "chapter_id": 162,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:34.090Z",
        "created_at": "2016-11-17T14:14:34.090Z",
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
        "id": 65,
        "obfuscated_id": "Pu1fo5_Q1vk",
        "author_id": 709,
        "chapter_id": 162,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:34.130Z",
        "created_at": "2016-11-17T14:14:34.130Z",
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
        "id": 94,
        "obfuscated_id": "CVi6VU_nV6k",
        "author_id": 706,
        "chapter_id": 162,
        "position": 81,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:33.821Z",
        "created_at": "2016-11-17T14:14:33.708Z",
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
            "id": 191,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 192,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 95,
        "obfuscated_id": "uTOhBSQK4CI",
        "author_id": 707,
        "chapter_id": 162,
        "position": 82,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:34.018Z",
        "created_at": "2016-11-17T14:14:33.893Z",
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
            "id": 193,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 194,
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
curl "api.goskive.com/v2/chapters/162" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c2390dd08ff8d789470a26881385e56fb21c941424aee2b467a5c659657f44db"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/167
Content-Type: application/json
Authorization: Bearer 686af9a93036e8b204fc0481571b5c8b2f1f8eaacd3b3b468eb8a5639d1801ee
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
    "id": 167,
    "updated_at": "2016-11-17T14:14:35.395Z",
    "course_id": 221,
    "author_id": 724,
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
curl "api.goskive.com/v2/chapters/167" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 686af9a93036e8b204fc0481571b5c8b2f1f8eaacd3b3b468eb8a5639d1801ee"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/58
Content-Type: application/json
Authorization: Bearer 54b4087084d5c34e486ff9ef3bffef107def4ec81fbefaebd9fbdd1c2afeafc5
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/58" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54b4087084d5c34e486ff9ef3bffef107def4ec81fbefaebd9fbdd1c2afeafc5"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 53b357c4a324c91389318c75ee818ef9e78c3ef4c88c372075383c348c34c3d3
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
      "id": 22,
      "author_id": 897,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:54.919Z",
      "status": "published",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 899,
      "reply_to_id": 22,
      "created_at": "2016-11-17T14:14:54.999Z",
      "status": "published",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 901,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:55.080Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 903,
      "reply_to_id": 24,
      "created_at": "2016-11-17T14:14:55.161Z",
      "status": "published",
      "subject_id": 281,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 905,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:55.244Z",
      "status": "reported",
      "subject_id": 282,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 907,
      "reply_to_id": 26,
      "created_at": "2016-11-17T14:14:55.326Z",
      "status": "published",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 909,
      "reply_to_id": 26,
      "created_at": "2016-11-17T14:14:55.409Z",
      "status": "published",
      "subject_id": 284,
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
	-H "Authorization: Bearer 53b357c4a324c91389318c75ee818ef9e78c3ef4c88c372075383c348c34c3d3"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer d1d95a90008e60838c9a15279debe14b197e71bd170105409d6d0fac495d76b6
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
      "id": 36,
      "author_id": 927,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:56.178Z",
      "status": "published",
      "subject_id": 292,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 929,
      "reply_to_id": 36,
      "created_at": "2016-11-17T14:14:56.258Z",
      "status": "published",
      "subject_id": 293,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 931,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:56.341Z",
      "status": "published",
      "subject_id": 294,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 933,
      "reply_to_id": 38,
      "created_at": "2016-11-17T14:14:56.424Z",
      "status": "published",
      "subject_id": 295,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 935,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:56.507Z",
      "status": "reported",
      "subject_id": 296,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 937,
      "reply_to_id": 40,
      "created_at": "2016-11-17T14:14:56.591Z",
      "status": "published",
      "subject_id": 297,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 939,
      "reply_to_id": 40,
      "created_at": "2016-11-17T14:14:56.708Z",
      "status": "published",
      "subject_id": 298,
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
	-H "Authorization: Bearer d1d95a90008e60838c9a15279debe14b197e71bd170105409d6d0fac495d76b6"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer f576932aa99e5b78913d24ef54ee2c7d3633b58400b335b42006d5a07fadc8f8
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
      "id": 51,
      "author_id": 959,
      "reply_to_id": 50,
      "created_at": "2016-11-17T14:14:57.574Z",
      "status": "published",
      "subject_id": 307,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 963,
      "reply_to_id": 52,
      "created_at": "2016-11-17T14:14:57.749Z",
      "status": "published",
      "subject_id": 309,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 967,
      "reply_to_id": 54,
      "created_at": "2016-11-17T14:14:57.913Z",
      "status": "published",
      "subject_id": 311,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 56,
      "author_id": 969,
      "reply_to_id": 54,
      "created_at": "2016-11-17T14:14:57.996Z",
      "status": "published",
      "subject_id": 312,
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
	-H "Authorization: Bearer f576932aa99e5b78913d24ef54ee2c7d3633b58400b335b42006d5a07fadc8f8"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 555c12b1ed1629cb7138bc1f479b7a9a7ed36fb034e7ef9ea4b9dcb901c08fe5
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
      "id": 47,
      "author_id": 950,
      "reply_to_id": null,
      "created_at": "2016-11-17T14:14:57.194Z",
      "status": "reported",
      "subject_id": 303,
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
	-H "Authorization: Bearer 555c12b1ed1629cb7138bc1f479b7a9a7ed36fb034e7ef9ea4b9dcb901c08fe5"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/21/republish
Content-Type: application/json
Authorization: Bearer 023d472c5703d95b7ad10d7f16d18a34398a5cce08e84217950a5c8ba8b25753
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/21/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 023d472c5703d95b7ad10d7f16d18a34398a5cce08e84217950a5c8ba8b25753"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/153/chapters
Content-Type: application/json
Authorization: Bearer 2de5af778285562309f0c4b48bdaa61ec561d5b4ea1c1124195f9f1e8511d52a
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
    "id": 136,
    "updated_at": "2016-11-17T14:14:22.431Z",
    "course_id": 153,
    "author_id": 569,
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
curl "api.goskive.com/v2/courses/153/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2de5af778285562309f0c4b48bdaa61ec561d5b4ea1c1124195f9f1e8511d52a"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 829c8fc8dce47d8842f62b49b8a11ba538dcce3390a3b1f0ecfef9dc525d96e1
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
    "id": 137,
    "updated_at": "2016-11-17T14:14:22.707Z",
    "course_id": 154,
    "author_id": 571,
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
	-H "Authorization: Bearer 829c8fc8dce47d8842f62b49b8a11ba538dcce3390a3b1f0ecfef9dc525d96e1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a3a78fa2d89d4174026161798ec5d912651c9aefb19b7d05f4ae9a989413da7e
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
      "id": 124,
      "updated_at": "2016-11-17T14:14:21.053Z",
      "course_id": 147,
      "author_id": 544,
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
      "id": 125,
      "updated_at": "2016-11-17T14:14:21.076Z",
      "course_id": 147,
      "author_id": 545,
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
      "id": 126,
      "updated_at": "2016-11-17T14:14:21.328Z",
      "course_id": 147,
      "author_id": 546,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-17T14:14:20.981Z",
      "questions_updated_at": "2016-11-17T14:14:20.981Z",
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
	-H "Authorization: Bearer a3a78fa2d89d4174026161798ec5d912651c9aefb19b7d05f4ae9a989413da7e"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer deaf29aaee9249a9916ecfceb5ac75e7d10d5d3631dd6ebbb5e2286f311db7d5
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
      "id": 127,
      "updated_at": "2016-11-17T14:14:21.574Z",
      "course_id": 149,
      "author_id": 553,
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
      "id": 128,
      "updated_at": "2016-11-17T14:14:21.597Z",
      "course_id": 149,
      "author_id": 554,
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
      "id": 129,
      "updated_at": "2016-11-17T14:14:21.620Z",
      "course_id": 149,
      "author_id": 555,
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
	-H "Authorization: Bearer deaf29aaee9249a9916ecfceb5ac75e7d10d5d3631dd6ebbb5e2286f311db7d5"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 21cc11b6478e4f8e955856f84d44373e968c078e578cc1316fa6e2362e6f9cd5
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
	-H "Authorization: Bearer 21cc11b6478e4f8e955856f84d44373e968c078e578cc1316fa6e2362e6f9cd5"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/261
Content-Type: application/json
Authorization: Bearer b90d9f507126453b9e6f9f78f39bd29fd26bd7c0727904e39d178dc7225479b1
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/261" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b90d9f507126453b9e6f9f78f39bd29fd26bd7c0727904e39d178dc7225479b1"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 25e5f38c77eeac7545de85ac59db7c4128fc681123e220e494d2888e2d77b212
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
    "creator_id": 849,
    "id": 267,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 252,
    "additional_university_ids": [

    ],
    "discipline_id": 275,
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
    "chapters_updated_at": "2016-11-17T14:14:46.633Z",
    "updated_at": "2016-11-17T14:14:48.189Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 68,
        "obfuscated_id": "yVS_7NAdP6s",
        "author_id": 849,
        "chapter_id": 184,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:47.968Z",
        "created_at": "2016-11-17T14:14:47.968Z",
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
        "author_id": 849,
        "chapter_id": 185,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.043Z",
        "created_at": "2016-11-17T14:14:48.043Z",
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
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 849,
        "chapter_id": 184,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.010Z",
        "created_at": "2016-11-17T14:14:48.010Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 849,
        "chapter_id": 185,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.086Z",
        "created_at": "2016-11-17T14:14:48.086Z",
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
        "id": 72,
        "obfuscated_id": "oqzxOzwzIgw",
        "author_id": 852,
        "chapter_id": 184,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.129Z",
        "created_at": "2016-11-17T14:14:48.129Z",
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
        "id": 73,
        "obfuscated_id": "LJvjpBojvP0",
        "author_id": 853,
        "chapter_id": 185,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-17T14:14:48.170Z",
        "created_at": "2016-11-17T14:14:48.170Z",
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
        "id": 184,
        "updated_at": "2016-11-17T14:14:48.139Z",
        "course_id": 267,
        "author_id": 849,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T14:14:46.633Z",
        "questions_updated_at": "2016-11-17T14:14:46.633Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 163",
        "position": 1
      },
      {
        "id": 185,
        "updated_at": "2016-11-17T14:14:48.181Z",
        "course_id": 267,
        "author_id": 849,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-17T14:14:46.633Z",
        "questions_updated_at": "2016-11-17T14:14:46.633Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 164",
        "position": 2
      }
    ],
    "topic_id": 274,
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
	-H "Authorization: Bearer 25e5f38c77eeac7545de85ac59db7c4128fc681123e220e494d2888e2d77b212"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/266
Content-Type: application/json
Authorization: Bearer aef151cdcfd1f8472c7fc3d8e972b6bf74d2cdfd33e900674e363b77604aabb3
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
    "creator_id": 847,
    "id": 266,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 251,
    "additional_university_ids": [

    ],
    "discipline_id": 274,
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
    "updated_at": "2016-11-17T14:14:46.565Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 273,
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
curl "api.goskive.com/v2/courses/266" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aef151cdcfd1f8472c7fc3d8e972b6bf74d2cdfd33e900674e363b77604aabb3"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 9e903ab9a6bbfd9bd96aaf5939eab1ad6204760f93130f3849d8170a093fd93b
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
    "creator_id": 845,
    "id": 265,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 250,
    "additional_university_ids": [

    ],
    "discipline_id": 273,
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
    "updated_at": "2016-11-17T14:14:46.351Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 272,
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
	-H "Authorization: Bearer 9e903ab9a6bbfd9bd96aaf5939eab1ad6204760f93130f3849d8170a093fd93b"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer ab92a781a877cb44d32725feaaf733832de658ba22639b9949820c4842e3c591
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
      "id": 6,
      "user_id": 258,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:13:59.099Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 262,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:13:59.393Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 8,
      "user_id": 266,
      "feedbackable_id": 41,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:13:59.693Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 9,
      "user_id": 270,
      "feedbackable_id": 42,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:00.007Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 274,
      "feedbackable_id": 43,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T14:14:00.316Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab92a781a877cb44d32725feaaf733832de658ba22639b9949820c4842e3c591"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 082ffd999e2cec54c2e400e640ac1cc678343c4764de7f8a9dc8833af054a7b3
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
      "id": 24,
      "user_id": 332,
      "feedbackable_id": 57,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-17T14:14:04.684Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 082ffd999e2cec54c2e400e640ac1cc678343c4764de7f8a9dc8833af054a7b3"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/7
Content-Type: application/json
Authorization: Bearer eb5f2c8fca8c3cdb47dc4cbf0e3dd43bfa75d054d9a612cc6e33e08325bfe96b
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb5f2c8fca8c3cdb47dc4cbf0e3dd43bfa75d054d9a612cc6e33e08325bfe96b"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer 7f19e1f925900c1d7b46c201d1b284f996572d956c521eb10deda23854ec9335
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
    "id": 10,
    "uploader": {
      "id": 26,
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
      "created_at": "2016-11-17T14:13:35.454Z",
      "updated_at": "2016-11-17T14:13:35.454Z"
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
    "created_at": "2016-11-17T14:13:35.525Z",
    "updated_at": "2016-11-17T14:13:35.525Z",
    "course_id": 10,
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
curl "api.goskive.com/v2/files/10/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f19e1f925900c1d7b46c201d1b284f996572d956c521eb10deda23854ec9335"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/50/feedbacks
Content-Type: application/json
Authorization: Bearer b87dd8b6409b145a094f2a133c32fd6d5688ef3377136f4ec2d9c2ffcafd7753
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
      "user_id": 613,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:25.768Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 612,
      "feedbackable_id": 50,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:25.757Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/50/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b87dd8b6409b145a094f2a133c32fd6d5688ef3377136f4ec2d9c2ffcafd7753"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 0df415d1831f4680d038b68f3e0fc6da899fac75e12319ebbd56dcdba2331b25
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
      "id": 34,
      "obfuscated_id": "LRSQf_NrQzE",
      "author_id": 484,
      "chapter_id": 102,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:17.868Z",
      "created_at": "2016-11-17T14:14:17.868Z",
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
      "id": 35,
      "obfuscated_id": "soCS52BooV0",
      "author_id": 487,
      "chapter_id": 103,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:17.995Z",
      "created_at": "2016-11-17T14:14:17.995Z",
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
      "id": 36,
      "obfuscated_id": "01Tx8eTrCOA",
      "author_id": 490,
      "chapter_id": 104,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:18.125Z",
      "created_at": "2016-11-17T14:14:18.125Z",
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
      "id": 37,
      "obfuscated_id": "95m_4XdR9PU",
      "author_id": 493,
      "chapter_id": 105,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:18.260Z",
      "created_at": "2016-11-17T14:14:18.260Z",
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
      "id": 38,
      "obfuscated_id": "8_YCqPYFnsI",
      "author_id": 496,
      "chapter_id": 106,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:18.390Z",
      "created_at": "2016-11-17T14:14:18.390Z",
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
	-H "Authorization: Bearer 0df415d1831f4680d038b68f3e0fc6da899fac75e12319ebbd56dcdba2331b25"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer cab2dea834f61cfd593d924bbfde5b57627936e05759ab32de50012b1c1ab08d
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 464,
      "chapter_id": 96,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:14:17.015Z",
      "created_at": "2016-11-17T14:14:17.015Z",
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
	-H "Authorization: Bearer cab2dea834f61cfd593d924bbfde5b57627936e05759ab32de50012b1c1ab08d"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/44/republish
Content-Type: application/json
Authorization: Bearer 379957087315df44e69e7c3714a19aabe7b5986ded49011a1b21e54dee7786f1
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/44/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 379957087315df44e69e7c3714a19aabe7b5986ded49011a1b21e54dee7786f1"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/64/feedbacks
Content-Type: application/json
Authorization: Bearer 7cfaa06335921543b8f9f1641d5fbacd57605c4432b7e3019c8f137eb307de8f
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
      "user_id": 395,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:10.092Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 31,
      "user_id": 394,
      "feedbackable_id": 64,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-17T14:14:10.080Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/64/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7cfaa06335921543b8f9f1641d5fbacd57605c4432b7e3019c8f137eb307de8f"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 4d6c16d416eaad8d7670caf6c991c0f5fd3e7cf559ec8d0de17e5130e6c0f69c
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 142,
      "chapter_id": 20,
      "position": 15,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:45.912Z",
      "created_at": "2016-11-17T14:13:45.779Z",
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 133,
      "chapter_id": 17,
      "position": 12,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:45.012Z",
      "created_at": "2016-11-17T14:13:44.882Z",
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
          "id": 27,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 28,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 136,
      "chapter_id": 18,
      "position": 13,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:45.306Z",
      "created_at": "2016-11-17T14:13:45.177Z",
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
          "id": 29,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 30,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 139,
      "chapter_id": 19,
      "position": 14,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:45.611Z",
      "created_at": "2016-11-17T14:13:45.469Z",
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 145,
      "chapter_id": 21,
      "position": 16,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:46.210Z",
      "created_at": "2016-11-17T14:13:46.082Z",
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4d6c16d416eaad8d7670caf6c991c0f5fd3e7cf559ec8d0de17e5130e6c0f69c"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 3f4d3806ca5a02888ab35b4195b1ad37b31f94915506417a0f2663f5a9fa53bb
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
      "id": 23,
      "obfuscated_id": "eUsQCUPDncM",
      "author_id": 161,
      "chapter_id": 26,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-17T14:13:47.756Z",
      "created_at": "2016-11-17T14:13:47.628Z",
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
          "id": 45,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 46,
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
	-H "Authorization: Bearer 3f4d3806ca5a02888ab35b4195b1ad37b31f94915506417a0f2663f5a9fa53bb"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/7/republish
Content-Type: application/json
Authorization: Bearer 3a67e3f83c85bbd3986fe20dae11a05c2530d439f12629a4ec12dd84c9e43665
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/7/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a67e3f83c85bbd3986fe20dae11a05c2530d439f12629a4ec12dd84c9e43665"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bfac32e27cf8885bff5b2a2dd8b20e1fcb5bfcfc0b8f8c60c8c2e35e31e9846e
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":174,"published":false}}
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
    "creator_id": 645,
    "id": 174,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 174,
    "additional_university_ids": [

    ],
    "discipline_id": 174,
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
    "updated_at": "2016-11-17T14:14:27.525Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 174,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":174,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bfac32e27cf8885bff5b2a2dd8b20e1fcb5bfcfc0b8f8c60c8c2e35e31e9846e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 56f1c1e9d407049050450520cb518d164436981d211ce45e3ad7d84b067b6b8d
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
      "creator_id": 653,
      "id": 182,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 182,
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
      "updated_at": "2016-11-17T14:14:28.663Z",
      "shortname": "fu-course-145",
      "topic_id": 182,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 653,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 183,
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
      "updated_at": "2016-11-17T14:14:28.704Z",
      "shortname": "fu-course-146",
      "topic_id": 183,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 654,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 184,
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
      "updated_at": "2016-11-17T14:14:28.754Z",
      "shortname": "fu-course-147",
      "topic_id": 184,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 654,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 180,
      "additional_university_ids": [

      ],
      "discipline_id": 185,
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
      "chapters_updated_at": "2016-11-17T14:14:28.605Z",
      "updated_at": "2016-11-17T14:14:29.056Z",
      "shortname": "fu-course-148",
      "topic_id": 185,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 148",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 56f1c1e9d407049050450520cb518d164436981d211ce45e3ad7d84b067b6b8d"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 17637f6358cb1bcacc95bac62bf777e6bb8e9a0d519a8204dd7bb4fce9f76afb
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
      "creator_id": 660,
      "id": 186,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "discipline_id": 186,
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
      "updated_at": "2016-11-17T14:14:29.261Z",
      "shortname": "fu-course-149",
      "topic_id": 186,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 660,
      "id": 187,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "discipline_id": 187,
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
      "updated_at": "2016-11-17T14:14:29.301Z",
      "shortname": "fu-course-150",
      "topic_id": 187,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 661,
      "id": 188,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "discipline_id": 188,
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
      "updated_at": "2016-11-17T14:14:29.350Z",
      "shortname": "fu-course-151",
      "topic_id": 188,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 661,
      "id": 189,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 182,
      "additional_university_ids": [

      ],
      "discipline_id": 189,
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
      "updated_at": "2016-11-17T14:14:29.390Z",
      "shortname": "fu-course-152",
      "topic_id": 189,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 152",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 17637f6358cb1bcacc95bac62bf777e6bb8e9a0d519a8204dd7bb4fce9f76afb"
```
