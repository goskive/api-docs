---
title: "Skive API Documentation"
language_tabs:
  - json: JSON
  - shell: cURL
---

# Chapters

## Delete a chapter


### Request

#### Endpoint

```
DELETE /v2/chapters/145
Content-Type: application/json
Authorization: Bearer 4c87d66859c04842d628ff8e18f010cf19068f1bacbe219b1c000c1cd570d6ac
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/145" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4c87d66859c04842d628ff8e18f010cf19068f1bacbe219b1c000c1cd570d6ac"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/137
Content-Type: application/json
Authorization: Bearer a6b24f3003ebb829a1a5a5996963ad6fcd968c1efc97ea731ba0dab67584f9e4
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
    "id": 137,
    "updated_at": "2016-12-14T19:55:04.155Z",
    "course_id": 212,
    "author_id": 617,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-14T19:55:03.565Z",
    "questions_updated_at": "2016-12-14T19:55:03.565Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 620,
        "chapter_id": 137,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:55:04.083Z",
        "created_at": "2016-12-14T19:55:04.083Z",
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
        "id": 75,
        "obfuscated_id": "rRYuZazyhgg",
        "author_id": 621,
        "chapter_id": 137,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:55:04.130Z",
        "created_at": "2016-12-14T19:55:04.130Z",
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
        "author_id": 618,
        "chapter_id": 137,
        "position": 87,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:55:03.808Z",
        "created_at": "2016-12-14T19:55:03.704Z",
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
        "author_id": 619,
        "chapter_id": 137,
        "position": 88,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:55:04.004Z",
        "created_at": "2016-12-14T19:55:03.889Z",
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
curl "api.goskive.com/v2/chapters/137" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6b24f3003ebb829a1a5a5996963ad6fcd968c1efc97ea731ba0dab67584f9e4"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/140
Content-Type: application/json
Authorization: Bearer a121e51895a95efe930450a586309bb4df5ee58199be2fe89ff7257f79a882c1
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
    "id": 140,
    "updated_at": "2016-12-14T19:55:05.263Z",
    "course_id": 215,
    "author_id": 634,
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
curl "api.goskive.com/v2/chapters/140" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a121e51895a95efe930450a586309bb4df5ee58199be2fe89ff7257f79a882c1"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer eb23bfdf21d46189bd69d6fb624cff89e6feb48411fe44ad53f952b8dcf12123
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/55" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer eb23bfdf21d46189bd69d6fb624cff89e6feb48411fe44ad53f952b8dcf12123"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2a6f5661c5c35c92f6f2600e80d6d76277d5319a4c6ff029baa4af46cdaa5ca0
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
      "author_id": 711,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:10.496Z",
      "status": "published",
      "subject_id": 235,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 713,
      "reply_to_id": 17,
      "created_at": "2016-12-14T19:55:10.610Z",
      "status": "published",
      "subject_id": 236,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 715,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:10.720Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 717,
      "reply_to_id": 19,
      "created_at": "2016-12-14T19:55:10.825Z",
      "status": "published",
      "subject_id": 238,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 719,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:10.939Z",
      "status": "reported",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 721,
      "reply_to_id": 21,
      "created_at": "2016-12-14T19:55:11.045Z",
      "status": "published",
      "subject_id": 240,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 723,
      "reply_to_id": 21,
      "created_at": "2016-12-14T19:55:11.150Z",
      "status": "published",
      "subject_id": 241,
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
	-H "Authorization: Bearer 2a6f5661c5c35c92f6f2600e80d6d76277d5319a4c6ff029baa4af46cdaa5ca0"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 0ea69e63a572ba9d0adb0c7db1699f5584c26117ff0acd7dd737f9eeb71e3878
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
      "author_id": 726,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:11.322Z",
      "status": "published",
      "subject_id": 242,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 728,
      "reply_to_id": 24,
      "created_at": "2016-12-14T19:55:11.427Z",
      "status": "published",
      "subject_id": 243,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 730,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:11.534Z",
      "status": "published",
      "subject_id": 244,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 732,
      "reply_to_id": 26,
      "created_at": "2016-12-14T19:55:11.638Z",
      "status": "published",
      "subject_id": 245,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 734,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:11.742Z",
      "status": "reported",
      "subject_id": 246,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 736,
      "reply_to_id": 28,
      "created_at": "2016-12-14T19:55:11.845Z",
      "status": "published",
      "subject_id": 247,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 738,
      "reply_to_id": 28,
      "created_at": "2016-12-14T19:55:11.951Z",
      "status": "published",
      "subject_id": 248,
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
	-H "Authorization: Bearer 0ea69e63a572ba9d0adb0c7db1699f5584c26117ff0acd7dd737f9eeb71e3878"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 71ce5db02d1c5412fac695ec18037e653e810bf60144565d5137da8358fe980f
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
      "author_id": 743,
      "reply_to_id": 31,
      "created_at": "2016-12-14T19:55:12.223Z",
      "status": "published",
      "subject_id": 250,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 747,
      "reply_to_id": 33,
      "created_at": "2016-12-14T19:55:12.438Z",
      "status": "published",
      "subject_id": 252,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 751,
      "reply_to_id": 35,
      "created_at": "2016-12-14T19:55:12.654Z",
      "status": "published",
      "subject_id": 254,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 753,
      "reply_to_id": 35,
      "created_at": "2016-12-14T19:55:12.762Z",
      "status": "published",
      "subject_id": 255,
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
	-H "Authorization: Bearer 71ce5db02d1c5412fac695ec18037e653e810bf60144565d5137da8358fe980f"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer a0a1d5d155353d79491aa90656c81865594440754cd3f4bf28c5ebcd6e75b53b
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
      "id": 49,
      "author_id": 779,
      "reply_to_id": null,
      "created_at": "2016-12-14T19:55:14.215Z",
      "status": "reported",
      "subject_id": 267,
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
	-H "Authorization: Bearer a0a1d5d155353d79491aa90656c81865594440754cd3f4bf28c5ebcd6e75b53b"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/16/republish
Content-Type: application/json
Authorization: Bearer d6528961ebfd6c3ac411a1a3386c3cdd7ec48df8b2de05968907c84d340b6f28
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/16/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d6528961ebfd6c3ac411a1a3386c3cdd7ec48df8b2de05968907c84d340b6f28"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/204/chapters
Content-Type: application/json
Authorization: Bearer 57f63869ef76612687779905fab87d6c2791c422e0b8b31fc49bef4666f7dd43
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
    "id": 130,
    "updated_at": "2016-12-14T19:55:01.276Z",
    "course_id": 204,
    "author_id": 595,
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
curl "api.goskive.com/v2/courses/204/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 57f63869ef76612687779905fab87d6c2791c422e0b8b31fc49bef4666f7dd43"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 58b0c31b9bfe3eb71564d1f898cc8b2dfcd029bd4e5e30f8d5ee2cf60d7a6f7e
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
    "id": 131,
    "updated_at": "2016-12-14T19:55:01.446Z",
    "course_id": 205,
    "author_id": 597,
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
	-H "Authorization: Bearer 58b0c31b9bfe3eb71564d1f898cc8b2dfcd029bd4e5e30f8d5ee2cf60d7a6f7e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6e7a34a3442aa4e11ae818d116bbb177d475744f267f16aaa8849cee1c909c70
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
      "updated_at": "2016-12-14T19:54:59.643Z",
      "course_id": 198,
      "author_id": 570,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 112",
      "position": 1
    },
    {
      "id": 119,
      "updated_at": "2016-12-14T19:54:59.669Z",
      "course_id": 198,
      "author_id": 571,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 113",
      "position": 2
    },
    {
      "id": 120,
      "updated_at": "2016-12-14T19:54:59.931Z",
      "course_id": 198,
      "author_id": 572,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-14T19:54:59.514Z",
      "questions_updated_at": "2016-12-14T19:54:59.514Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 114",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6e7a34a3442aa4e11ae818d116bbb177d475744f267f16aaa8849cee1c909c70"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e2c4c866ca775bb2f1f6a68a5b98ce4b83e2a1fef181456c4ec78dad69d19b95
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
      "updated_at": "2016-12-14T19:55:00.244Z",
      "course_id": 200,
      "author_id": 579,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 115",
      "position": 1
    },
    {
      "id": 122,
      "updated_at": "2016-12-14T19:55:00.272Z",
      "course_id": 200,
      "author_id": 580,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 116",
      "position": 2
    },
    {
      "id": 123,
      "updated_at": "2016-12-14T19:55:00.299Z",
      "course_id": 200,
      "author_id": 581,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 117",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2c4c866ca775bb2f1f6a68a5b98ce4b83e2a1fef181456c4ec78dad69d19b95"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/52
Content-Type: application/json
Authorization: Bearer 03f886a834da1adc897af6d28128913ea237c5f0b909b4529cad89a46ea7f139
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
	-H "Authorization: Bearer 03f886a834da1adc897af6d28128913ea237c5f0b909b4529cad89a46ea7f139"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 875815b0129fb62b4d646782cfea036b423b87e9168933a12786684ce4009334
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
	-H "Authorization: Bearer 875815b0129fb62b4d646782cfea036b423b87e9168933a12786684ce4009334"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 5418fd54d4cce451dcd808050c35f7a49590449aad8e74e31a618ab6e3b21945
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
    "creator_id": 104,
    "id": 64,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 42,
    "additional_university_ids": [

    ],
    "discipline_id": 64,
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
    "chapters_updated_at": "2016-12-14T19:54:17.783Z",
    "updated_at": "2016-12-14T19:54:19.049Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 19,
        "obfuscated_id": "xt199h-LGto",
        "author_id": 104,
        "chapter_id": 16,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:18.820Z",
        "created_at": "2016-12-14T19:54:18.820Z",
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
        "author_id": 104,
        "chapter_id": 17,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:18.900Z",
        "created_at": "2016-12-14T19:54:18.900Z",
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
        "author_id": 104,
        "chapter_id": 16,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:18.866Z",
        "created_at": "2016-12-14T19:54:18.866Z",
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
        "id": 22,
        "obfuscated_id": "V2ZFfduV4jE",
        "author_id": 104,
        "chapter_id": 17,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:18.944Z",
        "created_at": "2016-12-14T19:54:18.944Z",
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
        "id": 23,
        "obfuscated_id": "eUsQCUPDncM",
        "author_id": 107,
        "chapter_id": 16,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:18.986Z",
        "created_at": "2016-12-14T19:54:18.986Z",
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
        "author_id": 108,
        "chapter_id": 17,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-14T19:54:19.027Z",
        "created_at": "2016-12-14T19:54:19.027Z",
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
        "id": 16,
        "updated_at": "2016-12-14T19:54:18.996Z",
        "course_id": 64,
        "author_id": 104,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-14T19:54:17.783Z",
        "questions_updated_at": "2016-12-14T19:54:17.783Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 13",
        "position": 1
      },
      {
        "id": 17,
        "updated_at": "2016-12-14T19:54:19.038Z",
        "course_id": 64,
        "author_id": 104,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-14T19:54:17.783Z",
        "questions_updated_at": "2016-12-14T19:54:17.783Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 14",
        "position": 2
      }
    ],
    "topic_id": 64,
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
	-H "Authorization: Bearer 5418fd54d4cce451dcd808050c35f7a49590449aad8e74e31a618ab6e3b21945"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/48
Content-Type: application/json
Authorization: Bearer cf0b6edfda75e61baa9339b3ba2a2e6a33cdcc6ead8278934cd3644894498039
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
    "creator_id": 64,
    "id": 48,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 26,
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
    "updated_at": "2016-12-14T19:54:12.701Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 48,
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
curl "api.goskive.com/v2/courses/48" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf0b6edfda75e61baa9339b3ba2a2e6a33cdcc6ead8278934cd3644894498039"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer efa98c6e892beeb1d1bc1da3055aa217b055f03786de2a6d73b2f56f2ee85af9
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
    "creator_id": 66,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 27,
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
    "updated_at": "2016-12-14T19:54:12.870Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 49,
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
	-H "Authorization: Bearer efa98c6e892beeb1d1bc1da3055aa217b055f03786de2a6d73b2f56f2ee85af9"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer d53081fdbed15162428047370aa8e272748213e2af04912229ef2d6c6eb57509
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
      "user_id": 865,
      "feedbackable_id": 110,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:22.015Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 869,
      "feedbackable_id": 111,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:22.278Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 873,
      "feedbackable_id": 112,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:22.537Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 877,
      "feedbackable_id": 113,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:22.804Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 881,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-14T19:55:23.073Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d53081fdbed15162428047370aa8e272748213e2af04912229ef2d6c6eb57509"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 19971fa3dbcfdd34200d3100e781532d3ba4333dbba028e5d70969e26c94ef8a
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
      "id": 23,
      "user_id": 860,
      "feedbackable_id": 109,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-14T19:55:21.714Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19971fa3dbcfdd34200d3100e781532d3ba4333dbba028e5d70969e26c94ef8a"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Content-Type: application/json
Authorization: Bearer 8a1624dce6c9566e84f8b718a8bb6b4b26c2c5578b7cc95e306b8e63c2e3c542
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a1624dce6c9566e84f8b718a8bb6b4b26c2c5578b7cc95e306b8e63c2e3c542"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/11/metadata
Content-Type: application/json
Authorization: Bearer 0694c8df04c72e90287bed0daa728d9e6d045662bd23b87c3fc3fee0f6d8799e
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
      "id": 145,
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
      "created_at": "2016-12-14T19:54:22.866Z",
      "updated_at": "2016-12-14T19:54:22.866Z"
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
    "created_at": "2016-12-14T19:54:22.962Z",
    "updated_at": "2016-12-14T19:54:22.962Z",
    "course_id": 76,
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
	-H "Authorization: Bearer 0694c8df04c72e90287bed0daa728d9e6d045662bd23b87c3fc3fee0f6d8799e"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/84/feedbacks
Content-Type: application/json
Authorization: Bearer e3a032f11f75c2a8a9f37adc593c75c845b143292830576959c60c752bc06d09
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
      "user_id": 700,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:09.796Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 16,
      "user_id": 699,
      "feedbackable_id": 84,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:55:09.786Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/84/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3a032f11f75c2a8a9f37adc593c75c845b143292830576959c60c752bc06d09"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5dd9130f4ff5c8179874ee89b9521fc17f2571af8e1edfbf92a494dbdaa366d8
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
      "id": 45,
      "obfuscated_id": "IVleRnyZemc",
      "author_id": 319,
      "chapter_id": 65,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:38.687Z",
      "created_at": "2016-12-14T19:54:38.687Z",
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
      "id": 46,
      "obfuscated_id": "urkHiAaH08E",
      "author_id": 322,
      "chapter_id": 66,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:38.853Z",
      "created_at": "2016-12-14T19:54:38.853Z",
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
      "id": 47,
      "obfuscated_id": "rpshod_7JeU",
      "author_id": 325,
      "chapter_id": 67,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:39.033Z",
      "created_at": "2016-12-14T19:54:39.033Z",
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
      "id": 48,
      "obfuscated_id": "oqXJ8Hi_AE4",
      "author_id": 328,
      "chapter_id": 68,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:39.202Z",
      "created_at": "2016-12-14T19:54:39.202Z",
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
      "author_id": 331,
      "chapter_id": 69,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:39.368Z",
      "created_at": "2016-12-14T19:54:39.368Z",
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
	-H "Authorization: Bearer 5dd9130f4ff5c8179874ee89b9521fc17f2571af8e1edfbf92a494dbdaa366d8"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 4fe89a34539560c74e919aaf374d19e0d7f40f6864e9b1d21655c3f70b710ce0
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
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 315,
      "chapter_id": 64,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:38.488Z",
      "created_at": "2016-12-14T19:54:38.488Z",
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
	-H "Authorization: Bearer 4fe89a34539560c74e919aaf374d19e0d7f40f6864e9b1d21655c3f70b710ce0"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/35/republish
Content-Type: application/json
Authorization: Bearer c21a2f8729b367fc97b6cb8f56088bcd744123a348cd66d3ba4425f530064381
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/35/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c21a2f8729b367fc97b6cb8f56088bcd744123a348cd66d3ba4425f530064381"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/71/feedbacks
Content-Type: application/json
Authorization: Bearer 6de23adbd4d335bb4623a002f3df14c36fed57cb0e8c2333da641c6dab60a3a4
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
      "id": 5,
      "user_id": 422,
      "feedbackable_id": 71,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:54:46.288Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 421,
      "feedbackable_id": 71,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-14T19:54:46.278Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/71/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6de23adbd4d335bb4623a002f3df14c36fed57cb0e8c2333da641c6dab60a3a4"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer c13058253e95ace55af89d058c80e3a4c0857e0354208c3465960e7e2779cb02
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
      "id": 42,
      "obfuscated_id": "6gppIIjkzlA",
      "author_id": 192,
      "chapter_id": 31,
      "position": 41,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:26.960Z",
      "created_at": "2016-12-14T19:54:26.868Z",
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
          "id": 83,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 84,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 43,
      "obfuscated_id": "uapnSdBCag8",
      "author_id": 195,
      "chapter_id": 32,
      "position": 42,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:27.237Z",
      "created_at": "2016-12-14T19:54:27.144Z",
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
          "id": 85,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 86,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 44,
      "obfuscated_id": "bbNlnrscV_w",
      "author_id": 198,
      "chapter_id": 33,
      "position": 43,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:27.512Z",
      "created_at": "2016-12-14T19:54:27.418Z",
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
          "id": 87,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 88,
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
      "author_id": 201,
      "chapter_id": 34,
      "position": 44,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:27.792Z",
      "created_at": "2016-12-14T19:54:27.698Z",
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
          "id": 89,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 90,
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
      "author_id": 204,
      "chapter_id": 35,
      "position": 45,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:28.062Z",
      "created_at": "2016-12-14T19:54:27.976Z",
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
          "id": 91,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 92,
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
	-H "Authorization: Bearer c13058253e95ace55af89d058c80e3a4c0857e0354208c3465960e7e2779cb02"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c4ad7dea33651888dca3cbc2b40337c696d1503b209cd8baf0875032de922402
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
      "id": 41,
      "obfuscated_id": "11qbskrctUU",
      "author_id": 188,
      "chapter_id": 30,
      "position": 40,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-14T19:54:26.639Z",
      "created_at": "2016-12-14T19:54:26.556Z",
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
          "id": 81,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 82,
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
	-H "Authorization: Bearer c4ad7dea33651888dca3cbc2b40337c696d1503b209cd8baf0875032de922402"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/50/republish
Content-Type: application/json
Authorization: Bearer e20cb34e9c394a977a579e16942d53d06cb49687732bbd7da83afee564d545b2
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/50/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e20cb34e9c394a977a579e16942d53d06cb49687732bbd7da83afee564d545b2"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0518254f3b272eecb634ba35d72e4031e5861c29e16138035b7744e62bc9b832
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":44,"published":false}}
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
    "creator_id": 59,
    "id": 44,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 22,
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
    "updated_at": "2016-12-14T19:54:11.963Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 44,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":44,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0518254f3b272eecb634ba35d72e4031e5861c29e16138035b7744e62bc9b832"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ff953aad4300adc7fa67b24c0aea8948b83f40e6f509dfbaa480ba606965cab6
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
      "creator_id": 27,
      "id": 15,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-9",
      "html_url": "https://goskive.com/course/fu-course-9",
      "slug": "fu-course-9",
      "university_id": 10,
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
      "updated_at": "2016-12-14T19:54:08.952Z",
      "shortname": "fu-course-9",
      "topic_id": 15,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 9",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 27,
      "id": 16,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-10",
      "html_url": "https://goskive.com/course/fu-course-10",
      "slug": "fu-course-10",
      "university_id": 10,
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
      "updated_at": "2016-12-14T19:54:08.984Z",
      "shortname": "fu-course-10",
      "topic_id": 16,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 10",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 28,
      "id": 17,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-11",
      "html_url": "https://goskive.com/course/fu-course-11",
      "slug": "fu-course-11",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "discipline_id": 17,
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
      "updated_at": "2016-12-14T19:54:09.022Z",
      "shortname": "fu-course-11",
      "topic_id": 17,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 11",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 28,
      "id": 18,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-12",
      "html_url": "https://goskive.com/course/fu-course-12",
      "slug": "fu-course-12",
      "university_id": 10,
      "additional_university_ids": [

      ],
      "discipline_id": 18,
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
      "chapters_updated_at": "2016-12-14T19:54:08.876Z",
      "updated_at": "2016-12-14T19:54:09.264Z",
      "shortname": "fu-course-12",
      "topic_id": 18,
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
	-H "Authorization: Bearer ff953aad4300adc7fa67b24c0aea8948b83f40e6f509dfbaa480ba606965cab6"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 535a5b1ea729a1a32f6aeca943e85d278cb55b3d7382e3a1547895cc78c8f1c8
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
      "creator_id": 34,
      "id": 19,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-13",
      "html_url": "https://goskive.com/course/fu-course-13",
      "slug": "fu-course-13",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 19,
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
      "updated_at": "2016-12-14T19:54:09.522Z",
      "shortname": "fu-course-13",
      "topic_id": 19,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 13",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 34,
      "id": 20,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-14",
      "html_url": "https://goskive.com/course/fu-course-14",
      "slug": "fu-course-14",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 20,
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
      "updated_at": "2016-12-14T19:54:09.554Z",
      "shortname": "fu-course-14",
      "topic_id": 20,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 14",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 35,
      "id": 21,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-15",
      "html_url": "https://goskive.com/course/fu-course-15",
      "slug": "fu-course-15",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 21,
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
      "updated_at": "2016-12-14T19:54:09.592Z",
      "shortname": "fu-course-15",
      "topic_id": 21,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 15",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 35,
      "id": 22,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-16",
      "html_url": "https://goskive.com/course/fu-course-16",
      "slug": "fu-course-16",
      "university_id": 12,
      "additional_university_ids": [

      ],
      "discipline_id": 22,
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
      "updated_at": "2016-12-14T19:54:09.623Z",
      "shortname": "fu-course-16",
      "topic_id": 22,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 16",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 535a5b1ea729a1a32f6aeca943e85d278cb55b3d7382e3a1547895cc78c8f1c8"
```
