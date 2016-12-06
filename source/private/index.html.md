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
DELETE /v2/chapters/164
Content-Type: application/json
Authorization: Bearer 859e0ea9969fca7a021998b2f62a5311e60f808b71784d04e7057345f594b0ca
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/164" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 859e0ea9969fca7a021998b2f62a5311e60f808b71784d04e7057345f594b0ca"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/156
Content-Type: application/json
Authorization: Bearer c4fe71eb217ccabdaf66d528748165ae5f31869383c101eca39f2fde887a615f
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
    "id": 156,
    "updated_at": "2016-12-06T18:17:46.554Z",
    "course_id": 257,
    "author_id": 770,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-06T18:17:46.041Z",
    "questions_updated_at": "2016-12-06T18:17:46.041Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 79,
        "obfuscated_id": "BFjsqYG0c2I",
        "author_id": 773,
        "chapter_id": 156,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:46.503Z",
        "created_at": "2016-12-06T18:17:46.503Z",
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
        "author_id": 774,
        "chapter_id": 156,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:46.537Z",
        "created_at": "2016-12-06T18:17:46.537Z",
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
        "id": 110,
        "obfuscated_id": "55JK4PuG2Hk",
        "author_id": 771,
        "chapter_id": 156,
        "position": 97,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:46.250Z",
        "created_at": "2016-12-06T18:17:46.143Z",
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
            "id": 223,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 224,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 111,
        "obfuscated_id": "G-D-sgMUtTw",
        "author_id": 772,
        "chapter_id": 156,
        "position": 98,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:46.436Z",
        "created_at": "2016-12-06T18:17:46.319Z",
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
            "id": 225,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 226,
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
curl "api.goskive.com/v2/chapters/156" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c4fe71eb217ccabdaf66d528748165ae5f31869383c101eca39f2fde887a615f"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/160
Content-Type: application/json
Authorization: Bearer e27a2afa3f113a66d0b27cd209272bd88554ffb24ba1a0537ef88af62c6efbc2
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
    "id": 160,
    "updated_at": "2016-12-06T18:17:47.600Z",
    "course_id": 261,
    "author_id": 789,
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
curl "api.goskive.com/v2/chapters/160" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e27a2afa3f113a66d0b27cd209272bd88554ffb24ba1a0537ef88af62c6efbc2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/8
Content-Type: application/json
Authorization: Bearer 0e40b84ceeb4bfabec75954f120de3d387f702fb8a1a0714107b262ae27ffe22
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
	-H "Authorization: Bearer 0e40b84ceeb4bfabec75954f120de3d387f702fb8a1a0714107b262ae27ffe22"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 20272edb560429894039f524d41964771ab54f8b489beaf419d817a84df3c852
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
      "author_id": 72,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:49.164Z",
      "status": "published",
      "subject_id": 20,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 74,
      "reply_to_id": 11,
      "created_at": "2016-12-06T18:16:49.249Z",
      "status": "published",
      "subject_id": 21,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 76,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:49.329Z",
      "status": "published",
      "subject_id": 22,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 78,
      "reply_to_id": 13,
      "created_at": "2016-12-06T18:16:49.405Z",
      "status": "published",
      "subject_id": 23,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 80,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:49.484Z",
      "status": "reported",
      "subject_id": 24,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 82,
      "reply_to_id": 15,
      "created_at": "2016-12-06T18:16:49.563Z",
      "status": "published",
      "subject_id": 25,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 84,
      "reply_to_id": 15,
      "created_at": "2016-12-06T18:16:49.641Z",
      "status": "published",
      "subject_id": 26,
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
	-H "Authorization: Bearer 20272edb560429894039f524d41964771ab54f8b489beaf419d817a84df3c852"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2cb06e4b32dde844dee3e1720d6810d32341b75b29a56704cf59f8339a14222e
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
      "id": 32,
      "author_id": 117,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:50.972Z",
      "status": "published",
      "subject_id": 41,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 119,
      "reply_to_id": 32,
      "created_at": "2016-12-06T18:16:51.049Z",
      "status": "published",
      "subject_id": 42,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 121,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:51.128Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 123,
      "reply_to_id": 34,
      "created_at": "2016-12-06T18:16:51.208Z",
      "status": "published",
      "subject_id": 44,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 125,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:51.286Z",
      "status": "reported",
      "subject_id": 45,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 127,
      "reply_to_id": 36,
      "created_at": "2016-12-06T18:16:51.365Z",
      "status": "published",
      "subject_id": 46,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 129,
      "reply_to_id": 36,
      "created_at": "2016-12-06T18:16:51.445Z",
      "status": "published",
      "subject_id": 47,
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
	-H "Authorization: Bearer 2cb06e4b32dde844dee3e1720d6810d32341b75b29a56704cf59f8339a14222e"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 09b88b0ec21b2c1dcfcacd3051233a0978daef2e4b1d8936c0bbeb7cf61664bc
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
      "id": 19,
      "author_id": 89,
      "reply_to_id": 18,
      "created_at": "2016-12-06T18:16:49.852Z",
      "status": "published",
      "subject_id": 28,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 21,
      "author_id": 93,
      "reply_to_id": 20,
      "created_at": "2016-12-06T18:16:50.010Z",
      "status": "published",
      "subject_id": 30,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 97,
      "reply_to_id": 22,
      "created_at": "2016-12-06T18:16:50.166Z",
      "status": "published",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 99,
      "reply_to_id": 22,
      "created_at": "2016-12-06T18:16:50.243Z",
      "status": "published",
      "subject_id": 33,
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
	-H "Authorization: Bearer 09b88b0ec21b2c1dcfcacd3051233a0978daef2e4b1d8936c0bbeb7cf61664bc"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer cc10bd64da119866b2e1b1e6f196ce3f6e80c9f6b8a84b7e4205cce9e6556efe
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
      "id": 43,
      "author_id": 140,
      "reply_to_id": null,
      "created_at": "2016-12-06T18:16:51.890Z",
      "status": "reported",
      "subject_id": 52,
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
	-H "Authorization: Bearer cc10bd64da119866b2e1b1e6f196ce3f6e80c9f6b8a84b7e4205cce9e6556efe"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/48/republish
Content-Type: application/json
Authorization: Bearer 05c32408128c8b9d1bbd4dfae9d61d5f19620a553164aeaca794ba0c46967ebb
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/48/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 05c32408128c8b9d1bbd4dfae9d61d5f19620a553164aeaca794ba0c46967ebb"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer d5ee59cf56789f0f58d8c5de2fe7ca40ac8d2aa70c0054291d65e45660946c92
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
    "id": 138,
    "updated_at": "2016-12-06T18:17:39.076Z",
    "course_id": 220,
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
	-H "Authorization: Bearer d5ee59cf56789f0f58d8c5de2fe7ca40ac8d2aa70c0054291d65e45660946c92"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/222/chapters
Content-Type: application/json
Authorization: Bearer f93a0a1faa2acd92b77cf9c09b242697ba70a01834d212e1734fd3e8033d9705
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
    "id": 140,
    "updated_at": "2016-12-06T18:17:39.356Z",
    "course_id": 222,
    "author_id": 650,
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
curl "api.goskive.com/v2/courses/222/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f93a0a1faa2acd92b77cf9c09b242697ba70a01834d212e1734fd3e8033d9705"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8681782d05cb20c2e56412e370ea5bc58b96abe1bcf96a2139bf07f32c7d0780
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
      "id": 129,
      "updated_at": "2016-12-06T18:17:37.921Z",
      "course_id": 214,
      "author_id": 623,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 120",
      "position": 1
    },
    {
      "id": 130,
      "updated_at": "2016-12-06T18:17:37.944Z",
      "course_id": 214,
      "author_id": 624,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 121",
      "position": 2
    },
    {
      "id": 131,
      "updated_at": "2016-12-06T18:17:38.191Z",
      "course_id": 214,
      "author_id": 625,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-06T18:17:37.845Z",
      "questions_updated_at": "2016-12-06T18:17:37.845Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 122",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8681782d05cb20c2e56412e370ea5bc58b96abe1bcf96a2139bf07f32c7d0780"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a3dc3cc88aedd11360832e971c23840f2c6e572c808dd20d547823109a2d65e1
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
      "id": 132,
      "updated_at": "2016-12-06T18:17:38.337Z",
      "course_id": 215,
      "author_id": 630,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 123",
      "position": 1
    },
    {
      "id": 133,
      "updated_at": "2016-12-06T18:17:38.361Z",
      "course_id": 215,
      "author_id": 631,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 124",
      "position": 2
    },
    {
      "id": 134,
      "updated_at": "2016-12-06T18:17:38.383Z",
      "course_id": 215,
      "author_id": 632,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 125",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a3dc3cc88aedd11360832e971c23840f2c6e572c808dd20d547823109a2d65e1"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/123
Content-Type: application/json
Authorization: Bearer db1eb2be77b93e7ffbcfe2f2c5e8014188f996390aa82ece4c1327048fe87efe
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/123" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer db1eb2be77b93e7ffbcfe2f2c5e8014188f996390aa82ece4c1327048fe87efe"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 302d8b876a52797d0b27df4e999ac361d764c233ea1f6f83ef41c155b0ad5f88
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
	-H "Authorization: Bearer 302d8b876a52797d0b27df4e999ac361d764c233ea1f6f83ef41c155b0ad5f88"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 74cbf3600d54bfc875e44d92e580b06bbee3956bd3544752db0c45c6c643c8df
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
    "creator_id": 375,
    "id": 121,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 122,
    "additional_university_ids": [

    ],
    "discipline_id": 128,
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
    "chapters_updated_at": "2016-12-06T18:17:13.383Z",
    "updated_at": "2016-12-06T18:17:14.856Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 375,
        "chapter_id": 75,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.646Z",
        "created_at": "2016-12-06T18:17:14.646Z",
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
        "id": 43,
        "obfuscated_id": "uapnSdBCag8",
        "author_id": 375,
        "chapter_id": 76,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.718Z",
        "created_at": "2016-12-06T18:17:14.718Z",
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
        "author_id": 375,
        "chapter_id": 75,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.686Z",
        "created_at": "2016-12-06T18:17:14.686Z",
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
        "author_id": 375,
        "chapter_id": 76,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.758Z",
        "created_at": "2016-12-06T18:17:14.758Z",
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
        "author_id": 378,
        "chapter_id": 75,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.798Z",
        "created_at": "2016-12-06T18:17:14.798Z",
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
        "author_id": 379,
        "chapter_id": 76,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-06T18:17:14.838Z",
        "created_at": "2016-12-06T18:17:14.838Z",
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
        "id": 75,
        "updated_at": "2016-12-06T18:17:14.808Z",
        "course_id": 121,
        "author_id": 375,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-06T18:17:13.383Z",
        "questions_updated_at": "2016-12-06T18:17:13.383Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 69",
        "position": 1
      },
      {
        "id": 76,
        "updated_at": "2016-12-06T18:17:14.848Z",
        "course_id": 121,
        "author_id": 375,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-06T18:17:13.383Z",
        "questions_updated_at": "2016-12-06T18:17:13.383Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 70",
        "position": 2
      }
    ],
    "topic_id": 128,
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
	-H "Authorization: Bearer 74cbf3600d54bfc875e44d92e580b06bbee3956bd3544752db0c45c6c643c8df"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/114
Content-Type: application/json
Authorization: Bearer 8be9be653923ce69567484da1abae3563c4a5e65ca0a30e034269983cef13c38
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
    "creator_id": 355,
    "id": 114,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 115,
    "additional_university_ids": [

    ],
    "discipline_id": 121,
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
    "updated_at": "2016-12-06T18:17:09.674Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 121,
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
curl "api.goskive.com/v2/courses/114" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8be9be653923ce69567484da1abae3563c4a5e65ca0a30e034269983cef13c38"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 4fc7ed948f23d7860498aac8e52ba990ca31fc6316c2c5d1815ff578389d2ff8
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
    "creator_id": 359,
    "id": 116,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 117,
    "additional_university_ids": [

    ],
    "discipline_id": 123,
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
    "updated_at": "2016-12-06T18:17:09.920Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 123,
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
	-H "Authorization: Bearer 4fc7ed948f23d7860498aac8e52ba990ca31fc6316c2c5d1815ff578389d2ff8"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer ef5a3e17c52cb16b544b914e1446c457af5bfeccaaa1163dd1359076a7c49369
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
      "id": 33,
      "user_id": 911,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:54.810Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 915,
      "feedbackable_id": 122,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:55.095Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 919,
      "feedbackable_id": 123,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:55.383Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 923,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:55.668Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 37,
      "user_id": 927,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-06T18:17:55.955Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef5a3e17c52cb16b544b914e1446c457af5bfeccaaa1163dd1359076a7c49369"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 9043dd194ff3a1344989a9b38ac8ddbaf201ba0cdd2399c7f9edf094fa61fa02
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
      "user_id": 906,
      "feedbackable_id": 120,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-06T18:17:54.473Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9043dd194ff3a1344989a9b38ac8ddbaf201ba0cdd2399c7f9edf094fa61fa02"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/16
Content-Type: application/json
Authorization: Bearer 15fb59095fd465e7df3780786bd714c79088834ee8d255082c25a375b6237e8a
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
	-H "Authorization: Bearer 15fb59095fd465e7df3780786bd714c79088834ee8d255082c25a375b6237e8a"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/10/metadata
Content-Type: application/json
Authorization: Bearer c071ff7a5fd5e611a6161e1c583e8ebd18032399a54545d193c385a58d927405
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
      "id": 734,
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
      "created_at": "2016-12-06T18:17:43.965Z",
      "updated_at": "2016-12-06T18:17:43.965Z"
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
    "created_at": "2016-12-06T18:17:44.033Z",
    "updated_at": "2016-12-06T18:17:44.033Z",
    "course_id": 246,
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
	-H "Authorization: Bearer c071ff7a5fd5e611a6161e1c583e8ebd18032399a54545d193c385a58d927405"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/65/feedbacks
Content-Type: application/json
Authorization: Bearer 2ef0f3542aa736a5913c9a3b4b65184670ce4b16f4821c928d125b0847909ca4
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
      "id": 11,
      "user_id": 663,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:40.072Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 10,
      "user_id": 662,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:40.061Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/65/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2ef0f3542aa736a5913c9a3b4b65184670ce4b16f4821c928d125b0847909ca4"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer f6979f241ade6c17b682cc83304b74740448621af8b4560fae3206ba07cf0fef
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
      "id": 5,
      "obfuscated_id": "iw-7peoPwEU",
      "author_id": 170,
      "chapter_id": 21,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:53.587Z",
      "created_at": "2016-12-06T18:16:53.587Z",
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
      "id": 6,
      "obfuscated_id": "eyxYPTvoIb8",
      "author_id": 173,
      "chapter_id": 22,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:53.717Z",
      "created_at": "2016-12-06T18:16:53.717Z",
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
      "id": 7,
      "obfuscated_id": "XFkue8saGAM",
      "author_id": 176,
      "chapter_id": 23,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:53.843Z",
      "created_at": "2016-12-06T18:16:53.843Z",
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
      "id": 8,
      "obfuscated_id": "X2B_8FVuFe8",
      "author_id": 179,
      "chapter_id": 24,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:53.970Z",
      "created_at": "2016-12-06T18:16:53.970Z",
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
      "id": 9,
      "obfuscated_id": "DMbUb8tMXMw",
      "author_id": 182,
      "chapter_id": 25,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:54.096Z",
      "created_at": "2016-12-06T18:16:54.096Z",
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
	-H "Authorization: Bearer f6979f241ade6c17b682cc83304b74740448621af8b4560fae3206ba07cf0fef"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer b0d469d5c3643aafb1e3263c447660e73f3628b57b0ca645ca9a7b4440f99c76
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 214,
      "chapter_id": 35,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:55.464Z",
      "created_at": "2016-12-06T18:16:55.464Z",
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
	-H "Authorization: Bearer b0d469d5c3643aafb1e3263c447660e73f3628b57b0ca645ca9a7b4440f99c76"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/3/republish
Content-Type: application/json
Authorization: Bearer 5329299cf7779e5b5536da9e72a328bb1904024d10013040d0f43796478bfced
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/3/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5329299cf7779e5b5536da9e72a328bb1904024d10013040d0f43796478bfced"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/90/feedbacks
Content-Type: application/json
Authorization: Bearer 25c57d053357f44ed5df98c74eb2a01260d0a3a6a2f8ac937400e5577d4982db
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
      "user_id": 495,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:25.164Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 494,
      "feedbackable_id": 90,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-06T18:17:25.154Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/90/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 25c57d053357f44ed5df98c74eb2a01260d0a3a6a2f8ac937400e5577d4982db"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 9306af1ccc931dee3d3c8d9139f9afd63cd70341dcada084efadbef86f6527e3
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 258,
      "chapter_id": 49,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:59.087Z",
      "created_at": "2016-12-06T18:16:58.965Z",
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
          "id": 54,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 55,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 23,
      "obfuscated_id": "eUsQCUPDncM",
      "author_id": 249,
      "chapter_id": 46,
      "position": 19,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:58.235Z",
      "created_at": "2016-12-06T18:16:58.118Z",
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
          "id": 48,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 49,
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
      "author_id": 252,
      "chapter_id": 47,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:58.511Z",
      "created_at": "2016-12-06T18:16:58.393Z",
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
          "id": 50,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 51,
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
      "author_id": 255,
      "chapter_id": 48,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:58.805Z",
      "created_at": "2016-12-06T18:16:58.685Z",
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
    },
    {
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 261,
      "chapter_id": 50,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:59.361Z",
      "created_at": "2016-12-06T18:16:59.246Z",
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
          "id": 56,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 57,
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
	-H "Authorization: Bearer 9306af1ccc931dee3d3c8d9139f9afd63cd70341dcada084efadbef86f6527e3"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 9500bd37def41c66ea109cf66421a4e05a081f290b308030c7e96fe66a7fbff1
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 245,
      "chapter_id": 45,
      "position": 18,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-06T18:16:57.889Z",
      "created_at": "2016-12-06T18:16:57.773Z",
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
          "id": 46,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 47,
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
	-H "Authorization: Bearer 9500bd37def41c66ea109cf66421a4e05a081f290b308030c7e96fe66a7fbff1"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/40/republish
Content-Type: application/json
Authorization: Bearer 5845f152675d05673cb850bfbe526982947044b29da6e40955287b3ec0d4ebdd
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/40/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5845f152675d05673cb850bfbe526982947044b29da6e40955287b3ec0d4ebdd"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 90c5fb5fb0c4c1dda5a4661355345bc69aaaa41d5a0f23fc5d71a2f21e7f2838
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":177,"published":false}}
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
    "creator_id": 527,
    "id": 167,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 169,
    "additional_university_ids": [

    ],
    "discipline_id": 177,
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
    "updated_at": "2016-12-06T18:17:28.930Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 177,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":177,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90c5fb5fb0c4c1dda5a4661355345bc69aaaa41d5a0f23fc5d71a2f21e7f2838"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 30db7b3945c1ed6272c006b7584b6c409cc6a58ec3b7888c289e315381fed906
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
      "creator_id": 542,
      "id": 180,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-145",
      "html_url": "https://goskive.com/course/fu-course-145",
      "slug": "fu-course-145",
      "university_id": 175,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-12-06T18:17:30.239Z",
      "shortname": "fu-course-145",
      "topic_id": 190,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 145",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 542,
      "id": 181,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-146",
      "html_url": "https://goskive.com/course/fu-course-146",
      "slug": "fu-course-146",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "discipline_id": 191,
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
      "updated_at": "2016-12-06T18:17:30.277Z",
      "shortname": "fu-course-146",
      "topic_id": 191,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 146",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 543,
      "id": 182,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-147",
      "html_url": "https://goskive.com/course/fu-course-147",
      "slug": "fu-course-147",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "discipline_id": 192,
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
      "updated_at": "2016-12-06T18:17:30.323Z",
      "shortname": "fu-course-147",
      "topic_id": 192,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 147",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 543,
      "id": 183,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-148",
      "html_url": "https://goskive.com/course/fu-course-148",
      "slug": "fu-course-148",
      "university_id": 175,
      "additional_university_ids": [

      ],
      "discipline_id": 193,
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
      "chapters_updated_at": "2016-12-06T18:17:30.181Z",
      "updated_at": "2016-12-06T18:17:30.619Z",
      "shortname": "fu-course-148",
      "topic_id": 193,
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
	-H "Authorization: Bearer 30db7b3945c1ed6272c006b7584b6c409cc6a58ec3b7888c289e315381fed906"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ee1f3f634e1c6a6ae317a01864808e94ea9996d5650a38b967992a727dcec943
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
      "creator_id": 549,
      "id": 184,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-149",
      "html_url": "https://goskive.com/course/fu-course-149",
      "slug": "fu-course-149",
      "university_id": 177,
      "additional_university_ids": [

      ],
      "discipline_id": 194,
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
      "updated_at": "2016-12-06T18:17:30.817Z",
      "shortname": "fu-course-149",
      "topic_id": 194,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 149",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 549,
      "id": 185,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-150",
      "html_url": "https://goskive.com/course/fu-course-150",
      "slug": "fu-course-150",
      "university_id": 177,
      "additional_university_ids": [

      ],
      "discipline_id": 195,
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
      "updated_at": "2016-12-06T18:17:30.856Z",
      "shortname": "fu-course-150",
      "topic_id": 195,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 150",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 550,
      "id": 186,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-151",
      "html_url": "https://goskive.com/course/fu-course-151",
      "slug": "fu-course-151",
      "university_id": 177,
      "additional_university_ids": [

      ],
      "discipline_id": 196,
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
      "updated_at": "2016-12-06T18:17:30.903Z",
      "shortname": "fu-course-151",
      "topic_id": 196,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 151",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 550,
      "id": 187,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-152",
      "html_url": "https://goskive.com/course/fu-course-152",
      "slug": "fu-course-152",
      "university_id": 177,
      "additional_university_ids": [

      ],
      "discipline_id": 197,
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
      "updated_at": "2016-12-06T18:17:30.943Z",
      "shortname": "fu-course-152",
      "topic_id": 197,
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
	-H "Authorization: Bearer ee1f3f634e1c6a6ae317a01864808e94ea9996d5650a38b967992a727dcec943"
```
