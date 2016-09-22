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
DELETE /v2/chapters/30
Content-Type: application/json
Authorization: Bearer a71b57ee3f5bece8a673039025610ec26026574b5b01439633507aa48017098e
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/30" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a71b57ee3f5bece8a673039025610ec26026574b5b01439633507aa48017098e"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/26
Content-Type: application/json
Authorization: Bearer 348a1feb2a476f50831dbeea7e7c34ddeb8bd6281ea4b1957e5b3fd607c43cc8
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
    "id": 26,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-09-22T08:04:17.833Z",
    "course_id": 26,
    "author_id": 88,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-09-22T08:04:17.304Z",
    "questions_updated_at": "2016-09-22T08:04:17.304Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 4,
        "obfuscated_id": "SaV_gL1ycAY",
        "author_id": 91,
        "chapter_id": 26,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:17.776Z",
        "created_at": "2016-09-22T08:04:17.776Z",
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
        "author_id": 92,
        "chapter_id": 26,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:17.815Z",
        "created_at": "2016-09-22T08:04:17.815Z",
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
        "id": 5,
        "obfuscated_id": "iw-7peoPwEU",
        "author_id": 89,
        "chapter_id": 26,
        "position": 5,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:17.520Z",
        "created_at": "2016-09-22T08:04:17.412Z",
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
            "id": 9,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 10,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 6,
        "obfuscated_id": "eyxYPTvoIb8",
        "author_id": 90,
        "chapter_id": 26,
        "position": 6,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:17.708Z",
        "created_at": "2016-09-22T08:04:17.589Z",
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
            "id": 11,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 12,
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
curl "api.goskive.com/v2/chapters/26" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 348a1feb2a476f50831dbeea7e7c34ddeb8bd6281ea4b1957e5b3fd607c43cc8"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/34
Content-Type: application/json
Authorization: Bearer 9192fb8f083f549e7baec29dcfd3be68d40a5555c55fb31f344fb5db44ced53e
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
    "id": 34,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-09-22T08:04:19.990Z",
    "course_id": 34,
    "author_id": 119,
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
curl "api.goskive.com/v2/chapters/34" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9192fb8f083f549e7baec29dcfd3be68d40a5555c55fb31f344fb5db44ced53e"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/3
Content-Type: application/json
Authorization: Bearer e10c2533a01eac52b99163e5f4512ec094e6af35dc8c202a43a32c6fe53257e8
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e10c2533a01eac52b99163e5f4512ec094e6af35dc8c202a43a32c6fe53257e8"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 0b5d46b6912634aca534ff7e0e00ac215a9b741a514d349783ea3408d09cc686
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
      "author_id": 472,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:00.585Z",
      "status": "published",
      "subject_id": 140,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 474,
      "reply_to_id": 16,
      "created_at": "2016-09-22T08:05:00.675Z",
      "status": "published",
      "subject_id": 141,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 476,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:00.765Z",
      "status": "published",
      "subject_id": 142,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 478,
      "reply_to_id": 18,
      "created_at": "2016-09-22T08:05:00.853Z",
      "status": "published",
      "subject_id": 143,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 480,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:00.941Z",
      "status": "reported",
      "subject_id": 144,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 482,
      "reply_to_id": 20,
      "created_at": "2016-09-22T08:05:01.025Z",
      "status": "published",
      "subject_id": 145,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 484,
      "reply_to_id": 20,
      "created_at": "2016-09-22T08:05:01.114Z",
      "status": "published",
      "subject_id": 146,
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
	-H "Authorization: Bearer 0b5d46b6912634aca534ff7e0e00ac215a9b741a514d349783ea3408d09cc686"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a599dd0e109f691cbc45ff47ae1b4c2d269e71f386c6263470f539437978bbde
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
      "id": 23,
      "author_id": 487,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:01.269Z",
      "status": "published",
      "subject_id": 147,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 489,
      "reply_to_id": 23,
      "created_at": "2016-09-22T08:05:01.361Z",
      "status": "published",
      "subject_id": 148,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 491,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:01.450Z",
      "status": "published",
      "subject_id": 149,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 493,
      "reply_to_id": 25,
      "created_at": "2016-09-22T08:05:01.544Z",
      "status": "published",
      "subject_id": 150,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 495,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:01.638Z",
      "status": "reported",
      "subject_id": 151,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 497,
      "reply_to_id": 27,
      "created_at": "2016-09-22T08:05:01.730Z",
      "status": "published",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 499,
      "reply_to_id": 27,
      "created_at": "2016-09-22T08:05:01.822Z",
      "status": "published",
      "subject_id": 153,
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
	-H "Authorization: Bearer a599dd0e109f691cbc45ff47ae1b4c2d269e71f386c6263470f539437978bbde"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer c03b7e71fa05ed037eeb44f0874a99782339369f1678a15d9b60f659f8611fff
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
      "id": 38,
      "author_id": 519,
      "reply_to_id": 37,
      "created_at": "2016-09-22T08:05:02.791Z",
      "status": "published",
      "subject_id": 162,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 523,
      "reply_to_id": 39,
      "created_at": "2016-09-22T08:05:02.973Z",
      "status": "published",
      "subject_id": 164,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 527,
      "reply_to_id": 41,
      "created_at": "2016-09-22T08:05:03.155Z",
      "status": "published",
      "subject_id": 166,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 529,
      "reply_to_id": 41,
      "created_at": "2016-09-22T08:05:03.243Z",
      "status": "published",
      "subject_id": 167,
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
	-H "Authorization: Bearer c03b7e71fa05ed037eeb44f0874a99782339369f1678a15d9b60f659f8611fff"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer d18478a695a224850aedcb17b60d4da969721bcd43d2dc174ca6dda0d7b2ffe2
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
      "id": 34,
      "author_id": 510,
      "reply_to_id": null,
      "created_at": "2016-09-22T08:05:02.347Z",
      "status": "reported",
      "subject_id": 158,
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
	-H "Authorization: Bearer d18478a695a224850aedcb17b60d4da969721bcd43d2dc174ca6dda0d7b2ffe2"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/6/republish
Content-Type: application/json
Authorization: Bearer 41bebc654a06c6a21c17667205472617de10da059cf90ca9edc13c481d54ece1
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 41bebc654a06c6a21c17667205472617de10da059cf90ca9edc13c481d54ece1"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6015551c37e1fbb1ed257e9ad203878dd28add1d4e7ab0445797f076101ef213
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
    "id": 2,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-22T08:04:12.134Z",
    "course_id": 3,
    "author_id": 6,
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
	-H "Authorization: Bearer 6015551c37e1fbb1ed257e9ad203878dd28add1d4e7ab0445797f076101ef213"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/4/chapters
Content-Type: application/json
Authorization: Bearer 5a7f119366e97e3f8581baf0905c7f7951bf0d368e3934b0384f107b0615f90e
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
    "id": 3,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-09-22T08:04:12.269Z",
    "course_id": 4,
    "author_id": 8,
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
curl "api.goskive.com/v2/courses/4/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a7f119366e97e3f8581baf0905c7f7951bf0d368e3934b0384f107b0615f90e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 725c73dfd69c8f1415182bc3f690fd02ca125500c91b8108a03da24b4e3a5514
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
      "id": 13,
      "title": "Clever Chapter Title 10",
      "position": 1,
      "updated_at": "2016-09-22T08:04:13.435Z",
      "course_id": 10,
      "author_id": 28,
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
      "id": 14,
      "title": "Clever Chapter Title 11",
      "position": 2,
      "updated_at": "2016-09-22T08:04:13.461Z",
      "course_id": 10,
      "author_id": 29,
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
      "id": 15,
      "title": "Clever Chapter Title 12",
      "position": 3,
      "updated_at": "2016-09-22T08:04:13.714Z",
      "course_id": 10,
      "author_id": 30,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-09-22T08:04:13.358Z",
      "questions_updated_at": "2016-09-22T08:04:13.358Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 725c73dfd69c8f1415182bc3f690fd02ca125500c91b8108a03da24b4e3a5514"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer f812622c89c8ae4d61a315a94cb14f9b3588a64fd655259d2eb89a9d58ff41ac
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
      "id": 16,
      "title": "Clever Chapter Title 13",
      "position": 1,
      "updated_at": "2016-09-22T08:04:13.962Z",
      "course_id": 12,
      "author_id": 37,
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
      "id": 17,
      "title": "Clever Chapter Title 14",
      "position": 2,
      "updated_at": "2016-09-22T08:04:13.988Z",
      "course_id": 12,
      "author_id": 38,
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
      "id": 18,
      "title": "Clever Chapter Title 15",
      "position": 3,
      "updated_at": "2016-09-22T08:04:14.013Z",
      "course_id": 12,
      "author_id": 39,
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
	-H "Authorization: Bearer f812622c89c8ae4d61a315a94cb14f9b3588a64fd655259d2eb89a9d58ff41ac"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/52
Content-Type: application/json
Authorization: Bearer db35d4028e2a46712e1b5318bdb4a7b44e66b84d0d96bd79f421980d934ab877
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/52" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db35d4028e2a46712e1b5318bdb4a7b44e66b84d0d96bd79f421980d934ab877"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 8930e638dd179f75f89402d4ef21104d2e8e23fa73e2dd96d8e65c09b647f32a
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
	-H "Authorization: Bearer 8930e638dd179f75f89402d4ef21104d2e8e23fa73e2dd96d8e65c09b647f32a"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 48391a8252e40286822e65fa634050e24883d6b8c5b918b7e37a42fdbad18d87
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
    "creator_id": 172,
    "id": 51,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 51,
    "additional_university_ids": [

    ],
    "topic_id": 56,
    "discipline_id": 56,
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
    "chapters_updated_at": "2016-09-22T08:04:28.747Z",
    "updated_at": "2016-09-22T08:04:30.146Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 44,
        "title": "Clever Chapter Title 32",
        "position": 1,
        "updated_at": "2016-09-22T08:04:30.098Z",
        "course_id": 51,
        "author_id": 172,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-22T08:04:28.747Z",
        "questions_updated_at": "2016-09-22T08:04:28.747Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 45,
        "title": "Clever Chapter Title 33",
        "position": 2,
        "updated_at": "2016-09-22T08:04:30.139Z",
        "course_id": 51,
        "author_id": 172,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-09-22T08:04:28.747Z",
        "questions_updated_at": "2016-09-22T08:04:28.747Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 26,
        "obfuscated_id": "cWAsrz6MOVI",
        "author_id": 172,
        "chapter_id": 44,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:29.941Z",
        "created_at": "2016-09-22T08:04:29.941Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 172,
        "chapter_id": 45,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:30.010Z",
        "created_at": "2016-09-22T08:04:30.010Z",
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
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 172,
        "chapter_id": 44,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:29.980Z",
        "created_at": "2016-09-22T08:04:29.980Z",
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
        "id": 29,
        "obfuscated_id": "rvs1sHrnKS4",
        "author_id": 172,
        "chapter_id": 45,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:30.049Z",
        "created_at": "2016-09-22T08:04:30.049Z",
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
        "id": 30,
        "obfuscated_id": "virmgqGG22o",
        "author_id": 175,
        "chapter_id": 44,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:30.088Z",
        "created_at": "2016-09-22T08:04:30.088Z",
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
        "id": 31,
        "obfuscated_id": "5rbCnI5XGHg",
        "author_id": 176,
        "chapter_id": 45,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-09-22T08:04:30.128Z",
        "created_at": "2016-09-22T08:04:30.128Z",
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
	-H "Authorization: Bearer 48391a8252e40286822e65fa634050e24883d6b8c5b918b7e37a42fdbad18d87"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/45
Content-Type: application/json
Authorization: Bearer b20c3a69862373fd91d18f71d1b5af8bc345b9d77cff7b3fed0fc151cf17f2c5
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
    "creator_id": 149,
    "id": 45,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 45,
    "additional_university_ids": [

    ],
    "topic_id": 50,
    "discipline_id": 50,
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
    "updated_at": "2016-09-22T08:04:23.673Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/45" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b20c3a69862373fd91d18f71d1b5af8bc345b9d77cff7b3fed0fc151cf17f2c5"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 51b1065fe327e889eac88710aaecf9116b86484752ecd404b2aac6cff057adaf
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
    "creator_id": 147,
    "id": 44,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 44,
    "additional_university_ids": [

    ],
    "topic_id": 49,
    "discipline_id": 49,
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
    "updated_at": "2016-09-22T08:04:23.527Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 51b1065fe327e889eac88710aaecf9116b86484752ecd404b2aac6cff057adaf"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 651baefd68a9e1eb3d64c5297a38925359be799a420462c08023d29cfc6c4f90
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
      "id": 25,
      "user_id": 718,
      "feedbackable_id": 97,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:18.784Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 722,
      "feedbackable_id": 98,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:19.076Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 726,
      "feedbackable_id": 99,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:19.384Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 730,
      "feedbackable_id": 100,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:19.693Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 734,
      "feedbackable_id": 101,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-22T08:05:20.000Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 651baefd68a9e1eb3d64c5297a38925359be799a420462c08023d29cfc6c4f90"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer bd4f5fb36277cabd2fd4fe403e7228064f4df399132ac7f158f2689c0f313c4f
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
      "user_id": 713,
      "feedbackable_id": 96,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-09-22T08:05:18.437Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bd4f5fb36277cabd2fd4fe403e7228064f4df399132ac7f158f2689c0f313c4f"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/38/feedbacks
Content-Type: application/json
Authorization: Bearer a4251d7f773d6fba84727d372141e57b105afa7059ceee36fafe466c26055461
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
      "id": 6,
      "user_id": 327,
      "feedbackable_id": 38,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:04:51.154Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 326,
      "feedbackable_id": 38,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:04:51.141Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/38/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a4251d7f773d6fba84727d372141e57b105afa7059ceee36fafe466c26055461"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 14937f8cb98258a7ed4fc4d2c4f508f60db73ead114499a6822e84c5f92a550f
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
      "id": 56,
      "obfuscated_id": "PgrpyPCfpqo",
      "author_id": 396,
      "chapter_id": 100,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:55.693Z",
      "created_at": "2016-09-22T08:04:55.693Z",
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
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 399,
      "chapter_id": 101,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:55.833Z",
      "created_at": "2016-09-22T08:04:55.833Z",
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 402,
      "chapter_id": 102,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:55.973Z",
      "created_at": "2016-09-22T08:04:55.973Z",
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
      "author_id": 405,
      "chapter_id": 103,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:56.114Z",
      "created_at": "2016-09-22T08:04:56.114Z",
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
      "author_id": 408,
      "chapter_id": 104,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:56.258Z",
      "created_at": "2016-09-22T08:04:56.258Z",
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
	-H "Authorization: Bearer 14937f8cb98258a7ed4fc4d2c4f508f60db73ead114499a6822e84c5f92a550f"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer ad42ad37399a46ce7ded787fb8f875c333f585b6fd1ffc9771429b598a600873
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
      "author_id": 392,
      "chapter_id": 99,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:55.513Z",
      "created_at": "2016-09-22T08:04:55.513Z",
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
	-H "Authorization: Bearer ad42ad37399a46ce7ded787fb8f875c333f585b6fd1ffc9771429b598a600873"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/republish
Content-Type: application/json
Authorization: Bearer 31dc62c572eac053538adf1d5bf03fb49f6c22d03933519fbc397f85ce68254b
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/63/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 31dc62c572eac053538adf1d5bf03fb49f6c22d03933519fbc397f85ce68254b"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/115/feedbacks
Content-Type: application/json
Authorization: Bearer 143ac1624263c22df20b98bfcaf4a2b5bdac86947e24561fa2397d291c9fd334
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
      "id": 40,
      "user_id": 815,
      "feedbackable_id": 115,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:26.666Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 814,
      "feedbackable_id": 115,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-09-22T08:05:26.651Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/115/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 143ac1624263c22df20b98bfcaf4a2b5bdac86947e24561fa2397d291c9fd334"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 4559a11771a078fbac5760cb25bd12a77a5f8b0c324b12cd75ac3a0ed6e5fe2c
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
      "id": 63,
      "obfuscated_id": "k3ebr8XrqxE",
      "author_id": 278,
      "chapter_id": 73,
      "position": 54,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:40.610Z",
      "created_at": "2016-09-22T08:04:40.492Z",
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
          "id": 126,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 127,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 60,
      "obfuscated_id": "XsZtONYAiuo",
      "author_id": 269,
      "chapter_id": 70,
      "position": 51,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:39.759Z",
      "created_at": "2016-09-22T08:04:39.644Z",
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
          "id": 120,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 121,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 272,
      "chapter_id": 71,
      "position": 52,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:40.037Z",
      "created_at": "2016-09-22T08:04:39.922Z",
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
          "id": 122,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 123,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 275,
      "chapter_id": 72,
      "position": 53,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:40.324Z",
      "created_at": "2016-09-22T08:04:40.207Z",
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
          "id": 124,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 125,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 64,
      "obfuscated_id": "H-V851w7HZg",
      "author_id": 281,
      "chapter_id": 74,
      "position": 55,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:40.919Z",
      "created_at": "2016-09-22T08:04:40.805Z",
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
          "id": 128,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 129,
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
	-H "Authorization: Bearer 4559a11771a078fbac5760cb25bd12a77a5f8b0c324b12cd75ac3a0ed6e5fe2c"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 90484890b33091dd33ed20282388243cafc5f7ac10c679782219048d2a720aee
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 265,
      "chapter_id": 69,
      "position": 50,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-09-22T08:04:39.425Z",
      "created_at": "2016-09-22T08:04:39.312Z",
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
          "id": 118,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 119,
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
	-H "Authorization: Bearer 90484890b33091dd33ed20282388243cafc5f7ac10c679782219048d2a720aee"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/48/republish
Content-Type: application/json
Authorization: Bearer fced301901558fddbfeaa36d08ed2cab59f93e7f6ad349ae05c73ce82731101d
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/48/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fced301901558fddbfeaa36d08ed2cab59f93e7f6ad349ae05c73ce82731101d"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 1a939b27b4a9f34d6e1ecda557d0289fe3dbcc71cb0e6eb2b54bcd3d68379c28
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":291,"published":false}}
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
    "creator_id": 889,
    "id": 282,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 267,
    "additional_university_ids": [

    ],
    "topic_id": 291,
    "discipline_id": 292,
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
    "updated_at": "2016-09-22T08:05:33.569Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":291,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a939b27b4a9f34d6e1ecda557d0289fe3dbcc71cb0e6eb2b54bcd3d68379c28"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer cc1aa4fe3fb2737fd4fe73c544d7ea92216aef813b932ce7d8f8df9102ce5805
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
      "creator_id": 874,
      "id": 269,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-210",
      "html_url": "https://goskive.com/course/fu-course-210",
      "slug": "fu-course-210",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "topic_id": 278,
      "discipline_id": 279,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 210",
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
      "updated_at": "2016-09-22T08:05:32.162Z",
      "shortname": "fu-course-210"
    },
    {
      "creator_id": 874,
      "id": 270,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-211",
      "html_url": "https://goskive.com/course/fu-course-211",
      "slug": "fu-course-211",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "topic_id": 279,
      "discipline_id": 280,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 211",
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
      "updated_at": "2016-09-22T08:05:32.231Z",
      "shortname": "fu-course-211"
    },
    {
      "creator_id": 875,
      "id": 271,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-212",
      "html_url": "https://goskive.com/course/fu-course-212",
      "slug": "fu-course-212",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "topic_id": 280,
      "discipline_id": 281,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 212",
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
      "updated_at": "2016-09-22T08:05:32.281Z",
      "shortname": "fu-course-212"
    },
    {
      "creator_id": 875,
      "id": 272,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-213",
      "html_url": "https://goskive.com/course/fu-course-213",
      "slug": "fu-course-213",
      "university_id": 261,
      "additional_university_ids": [

      ],
      "topic_id": 281,
      "discipline_id": 282,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 213",
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
      "chapters_updated_at": "2016-09-22T08:05:32.575Z",
      "updated_at": "2016-09-22T08:05:32.582Z",
      "shortname": "fu-course-213"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cc1aa4fe3fb2737fd4fe73c544d7ea92216aef813b932ce7d8f8df9102ce5805"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 24933d12a8f1b3e811a76729e3597ca0326da5b03b540cbd9c5b5e42022b4cb0
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
      "creator_id": 881,
      "id": 273,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-214",
      "html_url": "https://goskive.com/course/fu-course-214",
      "slug": "fu-course-214",
      "university_id": 263,
      "additional_university_ids": [

      ],
      "topic_id": 282,
      "discipline_id": 283,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 214",
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
      "updated_at": "2016-09-22T08:05:32.797Z",
      "shortname": "fu-course-214"
    },
    {
      "creator_id": 881,
      "id": 274,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-215",
      "html_url": "https://goskive.com/course/fu-course-215",
      "slug": "fu-course-215",
      "university_id": 263,
      "additional_university_ids": [

      ],
      "topic_id": 283,
      "discipline_id": 284,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 215",
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
      "updated_at": "2016-09-22T08:05:32.837Z",
      "shortname": "fu-course-215"
    },
    {
      "creator_id": 882,
      "id": 275,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-216",
      "html_url": "https://goskive.com/course/fu-course-216",
      "slug": "fu-course-216",
      "university_id": 263,
      "additional_university_ids": [

      ],
      "topic_id": 284,
      "discipline_id": 285,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 216",
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
      "updated_at": "2016-09-22T08:05:32.887Z",
      "shortname": "fu-course-216"
    },
    {
      "creator_id": 882,
      "id": 276,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-217",
      "html_url": "https://goskive.com/course/fu-course-217",
      "slug": "fu-course-217",
      "university_id": 263,
      "additional_university_ids": [

      ],
      "topic_id": 285,
      "discipline_id": 286,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 217",
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
      "updated_at": "2016-09-22T08:05:32.927Z",
      "shortname": "fu-course-217"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 24933d12a8f1b3e811a76729e3597ca0326da5b03b540cbd9c5b5e42022b4cb0"
```
