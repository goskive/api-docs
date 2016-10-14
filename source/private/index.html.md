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
DELETE /v2/chapters/45
Content-Type: application/json
Authorization: Bearer 5350bde486920481bc7edb6e113325573512cc1b6e67b12d3edcd53d917770d3
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/45" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5350bde486920481bc7edb6e113325573512cc1b6e67b12d3edcd53d917770d3"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/50
Content-Type: application/json
Authorization: Bearer 64e550026de59d5a6c340f8834d9303992d47d01b9b8dfe896164a82ff1a8781
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
    "id": 50,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-14T12:01:47.240Z",
    "course_id": 66,
    "author_id": 224,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-14T12:01:46.697Z",
    "questions_updated_at": "2016-10-14T12:01:46.697Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 227,
        "chapter_id": 50,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:47.184Z",
        "created_at": "2016-10-14T12:01:47.184Z",
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
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 228,
        "chapter_id": 50,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:47.223Z",
        "created_at": "2016-10-14T12:01:47.223Z",
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
        "id": 49,
        "obfuscated_id": "GNsH7ObIVl0",
        "author_id": 225,
        "chapter_id": 50,
        "position": 49,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:46.919Z",
        "created_at": "2016-10-14T12:01:46.809Z",
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
            "id": 97,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 98,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 50,
        "obfuscated_id": "3_Ybw_gc_HE",
        "author_id": 226,
        "chapter_id": 50,
        "position": 50,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:47.113Z",
        "created_at": "2016-10-14T12:01:46.992Z",
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
            "id": 99,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 100,
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
curl "api.goskive.com/v2/chapters/50" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 64e550026de59d5a6c340f8834d9303992d47d01b9b8dfe896164a82ff1a8781"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/44
Content-Type: application/json
Authorization: Bearer 34f5e9e0c02770f7f79821aa2c96f3202e1af18182754b24a18d8b063ae502c3
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
    "id": 44,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-14T12:01:45.078Z",
    "course_id": 60,
    "author_id": 202,
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
curl "api.goskive.com/v2/chapters/44" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 34f5e9e0c02770f7f79821aa2c96f3202e1af18182754b24a18d8b063ae502c3"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/47
Content-Type: application/json
Authorization: Bearer a3196ef1f6b99f7eac849e006a842099e0e302260a83b224745c93792b7bde54
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
	-H "Authorization: Bearer a3196ef1f6b99f7eac849e006a842099e0e302260a83b224745c93792b7bde54"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c8c997e150457224262d3a13f143342bb8ad37a75728819bbcb7e082cfbd5d6f
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
      "author_id": 280,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:52.099Z",
      "status": "published",
      "subject_id": 87,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 282,
      "reply_to_id": 12,
      "created_at": "2016-10-14T12:01:52.190Z",
      "status": "published",
      "subject_id": 88,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 284,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:52.279Z",
      "status": "published",
      "subject_id": 89,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 286,
      "reply_to_id": 14,
      "created_at": "2016-10-14T12:01:52.364Z",
      "status": "published",
      "subject_id": 90,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 288,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:52.451Z",
      "status": "reported",
      "subject_id": 91,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 290,
      "reply_to_id": 16,
      "created_at": "2016-10-14T12:01:52.538Z",
      "status": "published",
      "subject_id": 92,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 292,
      "reply_to_id": 16,
      "created_at": "2016-10-14T12:01:52.630Z",
      "status": "published",
      "subject_id": 93,
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
	-H "Authorization: Bearer c8c997e150457224262d3a13f143342bb8ad37a75728819bbcb7e082cfbd5d6f"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer c1f326d786e1a20c9270e8817adb540225ade19c32bae929f1c43a1a259c633a
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
      "id": 19,
      "author_id": 295,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:52.806Z",
      "status": "published",
      "subject_id": 94,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 297,
      "reply_to_id": 19,
      "created_at": "2016-10-14T12:01:52.893Z",
      "status": "published",
      "subject_id": 95,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 299,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:52.981Z",
      "status": "published",
      "subject_id": 96,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 301,
      "reply_to_id": 21,
      "created_at": "2016-10-14T12:01:53.069Z",
      "status": "published",
      "subject_id": 97,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 303,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:53.158Z",
      "status": "reported",
      "subject_id": 98,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 305,
      "reply_to_id": 23,
      "created_at": "2016-10-14T12:01:53.244Z",
      "status": "published",
      "subject_id": 99,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 307,
      "reply_to_id": 23,
      "created_at": "2016-10-14T12:01:53.332Z",
      "status": "published",
      "subject_id": 100,
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
	-H "Authorization: Bearer c1f326d786e1a20c9270e8817adb540225ade19c32bae929f1c43a1a259c633a"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e4604c1bc59dc715f3d9d097dfb35dad024f1636087666e45615dd02c5029813
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
      "author_id": 312,
      "reply_to_id": 26,
      "created_at": "2016-10-14T12:01:53.571Z",
      "status": "published",
      "subject_id": 102,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 316,
      "reply_to_id": 28,
      "created_at": "2016-10-14T12:01:53.751Z",
      "status": "published",
      "subject_id": 104,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 320,
      "reply_to_id": 30,
      "created_at": "2016-10-14T12:01:53.934Z",
      "status": "published",
      "subject_id": 106,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 322,
      "reply_to_id": 30,
      "created_at": "2016-10-14T12:01:54.025Z",
      "status": "published",
      "subject_id": 107,
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
	-H "Authorization: Bearer e4604c1bc59dc715f3d9d097dfb35dad024f1636087666e45615dd02c5029813"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 9c5683daee19be4000cb2298251e3556970d5499349ecd7e68a5af72d7c49d0e
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
      "author_id": 348,
      "reply_to_id": null,
      "created_at": "2016-10-14T12:01:55.200Z",
      "status": "reported",
      "subject_id": 119,
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
	-H "Authorization: Bearer 9c5683daee19be4000cb2298251e3556970d5499349ecd7e68a5af72d7c49d0e"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/51/republish
Content-Type: application/json
Authorization: Bearer 948e0939e7fbe4607feaba9efeeb92f660b294fb2ac162feec7ee51a810e0837
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/51/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 948e0939e7fbe4607feaba9efeeb92f660b294fb2ac162feec7ee51a810e0837"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/181/chapters
Content-Type: application/json
Authorization: Bearer 91151fcdf5f24c72e3d1e5a7345246769e6ac2419fc4abed380de1f817b91a9e
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
    "id": 95,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T12:02:12.442Z",
    "course_id": 181,
    "author_id": 598,
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
curl "api.goskive.com/v2/courses/181/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91151fcdf5f24c72e3d1e5a7345246769e6ac2419fc4abed380de1f817b91a9e"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer c0e1b7b2bf93059cfd55b20ba3e2f192fe5350b5964cf6dc89c6658d93d8adf4
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
    "id": 97,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-14T12:02:12.831Z",
    "course_id": 184,
    "author_id": 604,
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
	-H "Authorization: Bearer c0e1b7b2bf93059cfd55b20ba3e2f192fe5350b5964cf6dc89c6658d93d8adf4"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 19e16b90ccc013cb358e03a312b803143053b8900bc3d38ace2effb0b3c57684
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
      "title": "Clever Chapter Title 83",
      "position": 1,
      "updated_at": "2016-10-14T12:02:12.943Z",
      "course_id": 185,
      "author_id": 606,
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
      "title": "Clever Chapter Title 84",
      "position": 2,
      "updated_at": "2016-10-14T12:02:12.968Z",
      "course_id": 185,
      "author_id": 607,
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
      "title": "Clever Chapter Title 85",
      "position": 3,
      "updated_at": "2016-10-14T12:02:13.254Z",
      "course_id": 185,
      "author_id": 608,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-14T12:02:12.863Z",
      "questions_updated_at": "2016-10-14T12:02:12.863Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 19e16b90ccc013cb358e03a312b803143053b8900bc3d38ace2effb0b3c57684"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b9f89a94c51285cbe378da3be044a6ebc50ec4122ee0983f662fe51fce2693c0
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
      "id": 101,
      "title": "Clever Chapter Title 86",
      "position": 1,
      "updated_at": "2016-10-14T12:02:13.409Z",
      "course_id": 186,
      "author_id": 613,
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
      "id": 102,
      "title": "Clever Chapter Title 87",
      "position": 2,
      "updated_at": "2016-10-14T12:02:13.434Z",
      "course_id": 186,
      "author_id": 614,
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
      "id": 103,
      "title": "Clever Chapter Title 88",
      "position": 3,
      "updated_at": "2016-10-14T12:02:13.459Z",
      "course_id": 186,
      "author_id": 615,
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
	-H "Authorization: Bearer b9f89a94c51285cbe378da3be044a6ebc50ec4122ee0983f662fe51fce2693c0"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/39
Content-Type: application/json
Authorization: Bearer 1fae9bf23efdca40087aeb598ed6975d5fab30b043188b000c2a57713a30caad
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/39" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1fae9bf23efdca40087aeb598ed6975d5fab30b043188b000c2a57713a30caad"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c0da06530c9a691773527bb720ff9167a1c3840d4937562b56598fdf208cbdf1
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
	-H "Authorization: Bearer c0da06530c9a691773527bb720ff9167a1c3840d4937562b56598fdf208cbdf1"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer bb7815c8991c91b6398b8c5f0bba2aae0f4a8a78f525d750a8a3316b16ecc125
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
    "creator_id": 168,
    "id": 49,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 49,
    "additional_university_ids": [

    ],
    "topic_id": 57,
    "discipline_id": 57,
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
    "chapters_updated_at": "2016-10-14T12:01:38.707Z",
    "updated_at": "2016-10-14T12:01:40.367Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 36,
        "title": "Clever Chapter Title 33",
        "position": 1,
        "updated_at": "2016-10-14T12:01:40.317Z",
        "course_id": 49,
        "author_id": 168,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T12:01:38.707Z",
        "questions_updated_at": "2016-10-14T12:01:38.707Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 37,
        "title": "Clever Chapter Title 34",
        "position": 2,
        "updated_at": "2016-10-14T12:01:40.359Z",
        "course_id": 49,
        "author_id": 168,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-14T12:01:38.707Z",
        "questions_updated_at": "2016-10-14T12:01:38.707Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 21,
        "obfuscated_id": "XIvx1qd7-fY",
        "author_id": 168,
        "chapter_id": 36,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.141Z",
        "created_at": "2016-10-14T12:01:40.141Z",
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
        "author_id": 168,
        "chapter_id": 37,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.220Z",
        "created_at": "2016-10-14T12:01:40.220Z",
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
        "author_id": 168,
        "chapter_id": 36,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.187Z",
        "created_at": "2016-10-14T12:01:40.187Z",
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
        "author_id": 168,
        "chapter_id": 37,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.265Z",
        "created_at": "2016-10-14T12:01:40.265Z",
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
        "author_id": 171,
        "chapter_id": 36,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.306Z",
        "created_at": "2016-10-14T12:01:40.306Z",
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
        "author_id": 172,
        "chapter_id": 37,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-14T12:01:40.347Z",
        "created_at": "2016-10-14T12:01:40.347Z",
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
	-H "Authorization: Bearer bb7815c8991c91b6398b8c5f0bba2aae0f4a8a78f525d750a8a3316b16ecc125"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/52
Content-Type: application/json
Authorization: Bearer 9baee1bb135b6feb535564bfb078d272866a66696567729ff8b989c8a0d8c46e
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
    "creator_id": 185,
    "id": 52,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 52,
    "additional_university_ids": [

    ],
    "topic_id": 60,
    "discipline_id": 60,
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
    "updated_at": "2016-10-14T12:01:43.989Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/52" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9baee1bb135b6feb535564bfb078d272866a66696567729ff8b989c8a0d8c46e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 98f4179f3ea54a22560f9eb5aac96f353cc68a361144379b1fba85c8c27ed7fd
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
    "creator_id": 190,
    "id": 55,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 55,
    "additional_university_ids": [

    ],
    "topic_id": 63,
    "discipline_id": 63,
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
    "updated_at": "2016-10-14T12:01:44.383Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98f4179f3ea54a22560f9eb5aac96f353cc68a361144379b1fba85c8c27ed7fd"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 98c0819efabe5a25a97612313089c75ccd3af1f87d25dd12fcb7da9074434522
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
      "id": 23,
      "user_id": 525,
      "feedbackable_id": 75,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:07.777Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 529,
      "feedbackable_id": 76,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:08.082Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 533,
      "feedbackable_id": 77,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:08.388Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 537,
      "feedbackable_id": 78,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:08.694Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 541,
      "feedbackable_id": 79,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T12:02:09.004Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 98c0819efabe5a25a97612313089c75ccd3af1f87d25dd12fcb7da9074434522"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 8b1b0cca8ca5ea0f41006a503665c40975236de2d599004d1910d8f30c210535
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
      "id": 32,
      "user_id": 562,
      "feedbackable_id": 84,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-14T12:02:10.619Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8b1b0cca8ca5ea0f41006a503665c40975236de2d599004d1910d8f30c210535"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer 5e057af87da6b99ebf77c4cd8ba68a6cd763d5c3dffb79c49b185584566a9df1
Content-Type: application/x-www-form-urlencoded
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
	-H "Authorization: Bearer 5e057af87da6b99ebf77c4cd8ba68a6cd763d5c3dffb79c49b185584566a9df1" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/65/feedbacks
Content-Type: application/json
Authorization: Bearer 3d92f253829166582c581e1413860264b73f5d708fcfd3c4fa822af59b84c143
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
      "id": 44,
      "user_id": 826,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:32.261Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 825,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:32.249Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/65/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3d92f253829166582c581e1413860264b73f5d708fcfd3c4fa822af59b84c143"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer b6cded2a3e19980dabc38f3f480060a34792995501c90314d0eaa8cddae0a8b9
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
      "id": 87,
      "obfuscated_id": "Jisk1d9Nmeo",
      "author_id": 898,
      "chapter_id": 184,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:36.215Z",
      "created_at": "2016-10-14T12:02:36.215Z",
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
      "id": 88,
      "obfuscated_id": "CDc29JqT-RA",
      "author_id": 901,
      "chapter_id": 185,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:36.355Z",
      "created_at": "2016-10-14T12:02:36.355Z",
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
      "id": 89,
      "obfuscated_id": "5eRHrGHLqZk",
      "author_id": 904,
      "chapter_id": 186,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:36.494Z",
      "created_at": "2016-10-14T12:02:36.494Z",
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
      "id": 90,
      "obfuscated_id": "gX_ALSaJ0k4",
      "author_id": 907,
      "chapter_id": 187,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:36.635Z",
      "created_at": "2016-10-14T12:02:36.635Z",
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
      "id": 91,
      "obfuscated_id": "EqPpyB0JN58",
      "author_id": 910,
      "chapter_id": 188,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:36.777Z",
      "created_at": "2016-10-14T12:02:36.777Z",
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
	-H "Authorization: Bearer b6cded2a3e19980dabc38f3f480060a34792995501c90314d0eaa8cddae0a8b9"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer bd753ead5930c5b6a7d08ea012eaf716a129661ff72344a306382296fbf799b4
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
      "id": 81,
      "obfuscated_id": "jHF1owx40fU",
      "author_id": 878,
      "chapter_id": 178,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:35.290Z",
      "created_at": "2016-10-14T12:02:35.290Z",
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
	-H "Authorization: Bearer bd753ead5930c5b6a7d08ea012eaf716a129661ff72344a306382296fbf799b4"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/69/republish
Content-Type: application/json
Authorization: Bearer 14d9c0da472c607003751f447688548df652b5d64303eb3eb5585389ea3d6df8
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/69/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 14d9c0da472c607003751f447688548df652b5d64303eb3eb5585389ea3d6df8"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/61/feedbacks
Content-Type: application/json
Authorization: Bearer 1438f4a21f1f37c36573245ae109fd4a084e370f3f8b2e7b691411683cb85b87
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
      "user_id": 430,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:00.661Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 429,
      "feedbackable_id": 61,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-14T12:02:00.650Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/61/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1438f4a21f1f37c36573245ae109fd4a084e370f3f8b2e7b691411683cb85b87"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 825ca1323d2ebfc271324478bea8e2de2f58db21323ccbff85e6ca62616e01d6
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
      "author_id": 714,
      "chapter_id": 138,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:22.144Z",
      "created_at": "2016-10-14T12:02:22.019Z",
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
          "id": 214,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 215,
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
      "author_id": 705,
      "chapter_id": 135,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:21.264Z",
      "created_at": "2016-10-14T12:02:21.143Z",
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
          "id": 208,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 209,
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
      "author_id": 708,
      "chapter_id": 136,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:21.552Z",
      "created_at": "2016-10-14T12:02:21.430Z",
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
          "id": 210,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 211,
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
      "author_id": 711,
      "chapter_id": 137,
      "position": 101,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:21.846Z",
      "created_at": "2016-10-14T12:02:21.722Z",
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
          "id": 212,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 213,
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
      "author_id": 717,
      "chapter_id": 139,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:22.435Z",
      "created_at": "2016-10-14T12:02:22.315Z",
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
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 825ca1323d2ebfc271324478bea8e2de2f58db21323ccbff85e6ca62616e01d6"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer e3ec6045feb9395d7b903e6b156d4c11f37cefc7b6fd79b695e088131a39d74a
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
      "id": 98,
      "obfuscated_id": "icApzX10lRE",
      "author_id": 685,
      "chapter_id": 129,
      "position": 93,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-14T12:02:19.374Z",
      "created_at": "2016-10-14T12:02:19.256Z",
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
          "id": 196,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 197,
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
	-H "Authorization: Bearer e3ec6045feb9395d7b903e6b156d4c11f37cefc7b6fd79b695e088131a39d74a"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/91/republish
Content-Type: application/json
Authorization: Bearer c08560156ad2b456edee099bedc4e9995b4196bd5e17f562635e6a1636e9f1c1
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/91/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c08560156ad2b456edee099bedc4e9995b4196bd5e17f562635e6a1636e9f1c1"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer b4399f3be3b9cf3212e6183c74fbd8213e946c9e7ff183368dd92ebab60833d7
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":282,"published":false}}
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
    "creator_id": 922,
    "id": 270,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 277,
    "additional_university_ids": [

    ],
    "topic_id": 282,
    "discipline_id": 283,
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
    "updated_at": "2016-10-14T12:02:39.106Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":282,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4399f3be3b9cf3212e6183c74fbd8213e946c9e7ff183368dd92ebab60833d7"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer aaef356d64177038928b539f6111692c77d6578083e9fa7938cf26fb902f4d3d
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
      "creator_id": 945,
      "id": 292,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-220",
      "html_url": "https://goskive.com/course/fu-course-220",
      "slug": "fu-course-220",
      "university_id": 287,
      "additional_university_ids": [

      ],
      "topic_id": 304,
      "discipline_id": 305,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 220",
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
      "updated_at": "2016-10-14T12:02:41.420Z",
      "shortname": "fu-course-220"
    },
    {
      "creator_id": 945,
      "id": 293,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-221",
      "html_url": "https://goskive.com/course/fu-course-221",
      "slug": "fu-course-221",
      "university_id": 287,
      "additional_university_ids": [

      ],
      "topic_id": 305,
      "discipline_id": 306,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 221",
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
      "updated_at": "2016-10-14T12:02:41.464Z",
      "shortname": "fu-course-221"
    },
    {
      "creator_id": 946,
      "id": 294,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-222",
      "html_url": "https://goskive.com/course/fu-course-222",
      "slug": "fu-course-222",
      "university_id": 287,
      "additional_university_ids": [

      ],
      "topic_id": 306,
      "discipline_id": 307,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 222",
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
      "updated_at": "2016-10-14T12:02:41.516Z",
      "shortname": "fu-course-222"
    },
    {
      "creator_id": 946,
      "id": 295,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-223",
      "html_url": "https://goskive.com/course/fu-course-223",
      "slug": "fu-course-223",
      "university_id": 287,
      "additional_university_ids": [

      ],
      "topic_id": 307,
      "discipline_id": 308,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 223",
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
      "chapters_updated_at": "2016-10-14T12:02:41.821Z",
      "updated_at": "2016-10-14T12:02:41.827Z",
      "shortname": "fu-course-223"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aaef356d64177038928b539f6111692c77d6578083e9fa7938cf26fb902f4d3d"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2600b0c9d7fe2cd7d38c3adb39eccedd8868c1cc770cd1b5b69555acdfd946c6
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
      "creator_id": 951,
      "id": 296,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-224",
      "html_url": "https://goskive.com/course/fu-course-224",
      "slug": "fu-course-224",
      "university_id": 288,
      "additional_university_ids": [

      ],
      "topic_id": 308,
      "discipline_id": 309,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 224",
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
      "updated_at": "2016-10-14T12:02:41.992Z",
      "shortname": "fu-course-224"
    },
    {
      "creator_id": 951,
      "id": 297,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-225",
      "html_url": "https://goskive.com/course/fu-course-225",
      "slug": "fu-course-225",
      "university_id": 288,
      "additional_university_ids": [

      ],
      "topic_id": 309,
      "discipline_id": 310,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 225",
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
      "updated_at": "2016-10-14T12:02:42.040Z",
      "shortname": "fu-course-225"
    },
    {
      "creator_id": 952,
      "id": 298,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-226",
      "html_url": "https://goskive.com/course/fu-course-226",
      "slug": "fu-course-226",
      "university_id": 288,
      "additional_university_ids": [

      ],
      "topic_id": 310,
      "discipline_id": 311,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 226",
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
      "updated_at": "2016-10-14T12:02:42.095Z",
      "shortname": "fu-course-226"
    },
    {
      "creator_id": 952,
      "id": 299,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-227",
      "html_url": "https://goskive.com/course/fu-course-227",
      "slug": "fu-course-227",
      "university_id": 288,
      "additional_university_ids": [

      ],
      "topic_id": 311,
      "discipline_id": 312,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 227",
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
      "updated_at": "2016-10-14T12:02:42.141Z",
      "shortname": "fu-course-227"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2600b0c9d7fe2cd7d38c3adb39eccedd8868c1cc770cd1b5b69555acdfd946c6"
```
