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
DELETE /v2/chapters/7
Content-Type: application/json
Authorization: Bearer 21576e4ea3c06910ca6f43524b23925174207c52883340176adc292d73bca664
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/7" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 21576e4ea3c06910ca6f43524b23925174207c52883340176adc292d73bca664"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/1
Content-Type: application/json
Authorization: Bearer 00bdf5bff35ef226314739684a0efe0320f2fb986355fcd5dfe4060ba6a3d64c
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
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-12-04T11:02:53.623Z",
    "course_id": 1,
    "author_id": 10,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-04T11:02:52.702Z",
    "questions_updated_at": "2016-12-04T11:02:52.702Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 1,
        "obfuscated_id": "vnOJWgI0jGc",
        "author_id": 13,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:02:53.567Z",
        "created_at": "2016-12-04T11:02:53.567Z",
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
        "author_id": 14,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:02:53.606Z",
        "created_at": "2016-12-04T11:02:53.606Z",
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
        "author_id": 11,
        "chapter_id": 1,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:02:53.305Z",
        "created_at": "2016-12-04T11:02:53.165Z",
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
        "author_id": 12,
        "chapter_id": 1,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:02:53.488Z",
        "created_at": "2016-12-04T11:02:53.374Z",
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
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/1" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00bdf5bff35ef226314739684a0efe0320f2fb986355fcd5dfe4060ba6a3d64c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/5
Content-Type: application/json
Authorization: Bearer 7d43fcafff28bdd95a1dbfd6476ac4aa880c1644790260675ed3c5ff3c60b115
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
    "id": 5,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-12-04T11:02:54.716Z",
    "course_id": 5,
    "author_id": 29,
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
curl "api.goskive.com/v2/chapters/5" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7d43fcafff28bdd95a1dbfd6476ac4aa880c1644790260675ed3c5ff3c60b115"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/11
Content-Type: application/json
Authorization: Bearer 1482da3e6ac60b4bae8e89923584f15a71b1cbe7df7976d33ad432bf9f432aa1
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1482da3e6ac60b4bae8e89923584f15a71b1cbe7df7976d33ad432bf9f432aa1"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 3e1140ca3ee4aa357153d48e7432b4fbdd90d01b737b576aa1357d6ee4696008
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
      "id": 13,
      "author_id": 451,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:22.696Z",
      "status": "published",
      "subject_id": 152,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 14,
      "author_id": 453,
      "reply_to_id": 13,
      "created_at": "2016-12-04T11:03:22.779Z",
      "status": "published",
      "subject_id": 153,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 455,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:22.864Z",
      "status": "published",
      "subject_id": 154,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 457,
      "reply_to_id": 15,
      "created_at": "2016-12-04T11:03:22.945Z",
      "status": "published",
      "subject_id": 155,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 459,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:23.027Z",
      "status": "reported",
      "subject_id": 156,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 461,
      "reply_to_id": 17,
      "created_at": "2016-12-04T11:03:23.109Z",
      "status": "published",
      "subject_id": 157,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 463,
      "reply_to_id": 17,
      "created_at": "2016-12-04T11:03:23.188Z",
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
curl "api.goskive.com/v2/comments" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3e1140ca3ee4aa357153d48e7432b4fbdd90d01b737b576aa1357d6ee4696008"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e36d9d82a213dbb53821ca66155ad6071565a325c1d0f238977c064ec05c043c
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
      "id": 41,
      "author_id": 511,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:25.129Z",
      "status": "published",
      "subject_id": 180,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 513,
      "reply_to_id": 41,
      "created_at": "2016-12-04T11:03:25.206Z",
      "status": "published",
      "subject_id": 181,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 515,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:25.283Z",
      "status": "published",
      "subject_id": 182,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 517,
      "reply_to_id": 43,
      "created_at": "2016-12-04T11:03:25.360Z",
      "status": "published",
      "subject_id": 183,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 519,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:25.442Z",
      "status": "reported",
      "subject_id": 184,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 521,
      "reply_to_id": 45,
      "created_at": "2016-12-04T11:03:25.523Z",
      "status": "published",
      "subject_id": 185,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 523,
      "reply_to_id": 45,
      "created_at": "2016-12-04T11:03:25.606Z",
      "status": "published",
      "subject_id": 186,
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
	-H "Authorization: Bearer e36d9d82a213dbb53821ca66155ad6071565a325c1d0f238977c064ec05c043c"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 248f741eb7ce86a613eacc334f7d2d71fa040bfed7ef8a011fd6ca4dc6928bd7
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
      "id": 21,
      "author_id": 468,
      "reply_to_id": 20,
      "created_at": "2016-12-04T11:03:23.420Z",
      "status": "published",
      "subject_id": 160,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 472,
      "reply_to_id": 22,
      "created_at": "2016-12-04T11:03:23.576Z",
      "status": "published",
      "subject_id": 162,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 476,
      "reply_to_id": 24,
      "created_at": "2016-12-04T11:03:23.735Z",
      "status": "published",
      "subject_id": 164,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 478,
      "reply_to_id": 24,
      "created_at": "2016-12-04T11:03:23.815Z",
      "status": "published",
      "subject_id": 165,
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
	-H "Authorization: Bearer 248f741eb7ce86a613eacc334f7d2d71fa040bfed7ef8a011fd6ca4dc6928bd7"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 40cec6fb45371260706c79abac7516e8733d737c49f6522f169057e6975aee5d
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
      "id": 38,
      "author_id": 504,
      "reply_to_id": null,
      "created_at": "2016-12-04T11:03:24.852Z",
      "status": "reported",
      "subject_id": 177,
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
	-H "Authorization: Bearer 40cec6fb45371260706c79abac7516e8733d737c49f6522f169057e6975aee5d"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/49/republish
Content-Type: application/json
Authorization: Bearer 696d990e72ef439c9b53c4286c05ecc3e0cf160eb22dca7960330847de6c3bea
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
	-H "Authorization: Bearer 696d990e72ef439c9b53c4286c05ecc3e0cf160eb22dca7960330847de6c3bea"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer fdcd00fc42cf99e014323c8d4d0625a549563d8b5d0a4cfaf3098a16cfb3e4db
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
    "id": 91,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-12-04T11:03:21.473Z",
    "course_id": 144,
    "author_id": 427,
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
	-H "Authorization: Bearer fdcd00fc42cf99e014323c8d4d0625a549563d8b5d0a4cfaf3098a16cfb3e4db"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/147/chapters
Content-Type: application/json
Authorization: Bearer b9d0242dd1f37d13f010a7b56979aa9f0b58766b048ca323cf2994781db6e17e
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
    "id": 93,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-12-04T11:03:21.826Z",
    "course_id": 147,
    "author_id": 433,
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
curl "api.goskive.com/v2/courses/147/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b9d0242dd1f37d13f010a7b56979aa9f0b58766b048ca323cf2994781db6e17e"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer a2ba32728faeb62fa0f7cafd266775a3d7aad996cf7481acbc9e5e25268126eb
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
      "id": 76,
      "title": "Clever Chapter Title 64",
      "position": 1,
      "updated_at": "2016-12-04T11:03:19.770Z",
      "course_id": 136,
      "author_id": 392,
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
      "id": 77,
      "title": "Clever Chapter Title 65",
      "position": 2,
      "updated_at": "2016-12-04T11:03:19.793Z",
      "course_id": 136,
      "author_id": 393,
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
      "id": 78,
      "title": "Clever Chapter Title 66",
      "position": 3,
      "updated_at": "2016-12-04T11:03:20.027Z",
      "course_id": 136,
      "author_id": 394,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-04T11:03:19.702Z",
      "questions_updated_at": "2016-12-04T11:03:19.702Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a2ba32728faeb62fa0f7cafd266775a3d7aad996cf7481acbc9e5e25268126eb"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 38aeaa732f4d33242ad7556b4c5f456ce112c2730f3601c30cded5966f14ff13
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
      "id": 79,
      "title": "Clever Chapter Title 67",
      "position": 1,
      "updated_at": "2016-12-04T11:03:20.167Z",
      "course_id": 137,
      "author_id": 399,
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
      "id": 80,
      "title": "Clever Chapter Title 68",
      "position": 2,
      "updated_at": "2016-12-04T11:03:20.191Z",
      "course_id": 137,
      "author_id": 400,
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
      "id": 81,
      "title": "Clever Chapter Title 69",
      "position": 3,
      "updated_at": "2016-12-04T11:03:20.214Z",
      "course_id": 137,
      "author_id": 401,
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
	-H "Authorization: Bearer 38aeaa732f4d33242ad7556b4c5f456ce112c2730f3601c30cded5966f14ff13"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/266
Content-Type: application/json
Authorization: Bearer e6f42294945f4c037e79b07aa2ca729bdc0475afb93dddcd41191c7d1dff7a96
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/266" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e6f42294945f4c037e79b07aa2ca729bdc0475afb93dddcd41191c7d1dff7a96"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 14a5b56f841181846ea43ad7059b177e18a3c1d121aacbd9f362bc0f019ba33e
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
	-H "Authorization: Bearer 14a5b56f841181846ea43ad7059b177e18a3c1d121aacbd9f362bc0f019ba33e"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 4cfc7c0ed768b348f17a9569db2644b5fed75d6d8d0000a49beb94be396bcfee
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
    "creator_id": 865,
    "id": 277,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 262,
    "additional_university_ids": [

    ],
    "topic_id": 289,
    "discipline_id": 290,
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
    "chapters_updated_at": "2016-12-04T11:03:53.510Z",
    "updated_at": "2016-12-04T11:03:54.889Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 162,
        "title": "Clever Chapter Title 138",
        "position": 1,
        "updated_at": "2016-12-04T11:03:54.846Z",
        "course_id": 277,
        "author_id": 865,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-04T11:03:53.510Z",
        "questions_updated_at": "2016-12-04T11:03:53.510Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 163,
        "title": "Clever Chapter Title 139",
        "position": 2,
        "updated_at": "2016-12-04T11:03:54.882Z",
        "course_id": 277,
        "author_id": 865,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-04T11:03:53.510Z",
        "questions_updated_at": "2016-12-04T11:03:53.510Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 865,
        "chapter_id": 162,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.696Z",
        "created_at": "2016-12-04T11:03:54.696Z",
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
        "id": 86,
        "obfuscated_id": "7q-2LHZR3Kk",
        "author_id": 865,
        "chapter_id": 163,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.763Z",
        "created_at": "2016-12-04T11:03:54.763Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 865,
        "chapter_id": 162,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.734Z",
        "created_at": "2016-12-04T11:03:54.734Z",
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
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 865,
        "chapter_id": 163,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.802Z",
        "created_at": "2016-12-04T11:03:54.802Z",
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
        "id": 88,
        "obfuscated_id": "CDc29JqT-RA",
        "author_id": 868,
        "chapter_id": 162,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.837Z",
        "created_at": "2016-12-04T11:03:54.837Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 869,
        "chapter_id": 163,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-04T11:03:54.873Z",
        "created_at": "2016-12-04T11:03:54.873Z",
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
	-H "Authorization: Bearer 4cfc7c0ed768b348f17a9569db2644b5fed75d6d8d0000a49beb94be396bcfee"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/279
Content-Type: application/json
Authorization: Bearer 718bfa4ce41ff68e9a8668903ca54e454f20d6eaf4855a08fdc85f443c79dd12
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
    "creator_id": 877,
    "id": 279,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 264,
    "additional_university_ids": [

    ],
    "topic_id": 291,
    "discipline_id": 292,
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
    "updated_at": "2016-12-04T11:03:56.598Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/279" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 718bfa4ce41ff68e9a8668903ca54e454f20d6eaf4855a08fdc85f443c79dd12"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer d4bb2025efe68c7c8ed4dd22873f1e415f002d2f4431fb462172d23874bfcccd
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
    "creator_id": 880,
    "id": 281,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 266,
    "additional_university_ids": [

    ],
    "topic_id": 293,
    "discipline_id": 294,
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
    "updated_at": "2016-12-04T11:03:56.860Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d4bb2025efe68c7c8ed4dd22873f1e415f002d2f4431fb462172d23874bfcccd"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 559bdf160daeaca53296ab170f1fc679fc1bb343e6b8d3782ff8aaefe455b019
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
      "id": 37,
      "user_id": 680,
      "feedbackable_id": 51,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:37.449Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 38,
      "user_id": 684,
      "feedbackable_id": 52,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:37.735Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 688,
      "feedbackable_id": 53,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:38.014Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 692,
      "feedbackable_id": 54,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:38.285Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 696,
      "feedbackable_id": 55,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-04T11:03:38.565Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 559bdf160daeaca53296ab170f1fc679fc1bb343e6b8d3782ff8aaefe455b019"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 6cce72429009999efbf093100aee87af03f088f0e9b8a3b26cd41614c95803db
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
      "id": 27,
      "user_id": 638,
      "feedbackable_id": 41,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-04T11:03:34.547Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6cce72429009999efbf093100aee87af03f088f0e9b8a3b26cd41614c95803db"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/8
Content-Type: application/json
Authorization: Bearer 300bd3cb6565d979226fb089c114ed326f4b358313027303a18a00ea96b73406
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/8" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 300bd3cb6565d979226fb089c114ed326f4b358313027303a18a00ea96b73406"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/12/metadata
Content-Type: application/json
Authorization: Bearer b66ce597c32de7eb10380640bea46b6ea647b5f21feab5c2b3614350b9fa890e
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
    "id": 12,
    "uploader": {
      "id": 299,
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
      "created_at": "2016-12-04T11:03:14.666Z",
      "updated_at": "2016-12-04T11:03:14.666Z"
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
    "created_at": "2016-12-04T11:03:14.739Z",
    "updated_at": "2016-12-04T11:03:14.739Z",
    "course_id": 110,
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
curl "api.goskive.com/v2/files/12/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b66ce597c32de7eb10380640bea46b6ea647b5f21feab5c2b3614350b9fa890e"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/37/feedbacks
Content-Type: application/json
Authorization: Bearer 70e77ce95808d17f313ba5aa2e92a4a9c2d9ddca7b81127a5b4b6a493ffc5072
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
      "id": 14,
      "user_id": 343,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:16.528Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 342,
      "feedbackable_id": 37,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:16.518Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/37/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 70e77ce95808d17f313ba5aa2e92a4a9c2d9ddca7b81127a5b4b6a493ffc5072"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer ea88ea72bc93e02cd69584520ac2da8f0aa58ee771dc01c8fc42f56e5d2ded6e
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
      "id": 20,
      "obfuscated_id": "4DFpearSrHk",
      "author_id": 192,
      "chapter_id": 40,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:07.484Z",
      "created_at": "2016-12-04T11:03:07.484Z",
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
      "author_id": 195,
      "chapter_id": 41,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:07.607Z",
      "created_at": "2016-12-04T11:03:07.607Z",
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
      "author_id": 198,
      "chapter_id": 42,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:07.736Z",
      "created_at": "2016-12-04T11:03:07.736Z",
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
      "author_id": 201,
      "chapter_id": 43,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:07.908Z",
      "created_at": "2016-12-04T11:03:07.908Z",
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 204,
      "chapter_id": 44,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:08.032Z",
      "created_at": "2016-12-04T11:03:08.032Z",
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
	-H "Authorization: Bearer ea88ea72bc93e02cd69584520ac2da8f0aa58ee771dc01c8fc42f56e5d2ded6e"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer df6c6770f44cd52dd6889ad9ffd01af761f27d0bd847f90c568e11568df1d872
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 172,
      "chapter_id": 34,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:03:06.646Z",
      "created_at": "2016-12-04T11:03:06.646Z",
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
	-H "Authorization: Bearer df6c6770f44cd52dd6889ad9ffd01af761f27d0bd847f90c568e11568df1d872"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/republish
Content-Type: application/json
Authorization: Bearer a36f84e62d4223009ae95eeaeb3e71639645dbc0e727de2803c568d05e71e4ca
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/26/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a36f84e62d4223009ae95eeaeb3e71639645dbc0e727de2803c568d05e71e4ca"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/16/feedbacks
Content-Type: application/json
Authorization: Bearer 7f958b227a1c155debec7fa0ac5cca4014bdb08e8fbfa18d05104906fb91994d
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
      "user_id": 109,
      "feedbackable_id": 16,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:01.950Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 108,
      "feedbackable_id": 16,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-04T11:03:01.940Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/16/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7f958b227a1c155debec7fa0ac5cca4014bdb08e8fbfa18d05104906fb91994d"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer e6da57f94948cf77901be55f0f47ecc79f85cc03407d71c4c5bcdc4c6a797264
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
      "id": 117,
      "obfuscated_id": "BsA8mEPn8aM",
      "author_id": 931,
      "chapter_id": 178,
      "position": 104,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:02.194Z",
      "created_at": "2016-12-04T11:04:02.079Z",
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
    },
    {
      "id": 115,
      "obfuscated_id": "tgK0VZO8yq4",
      "author_id": 925,
      "chapter_id": 176,
      "position": 102,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:01.647Z",
      "created_at": "2016-12-04T11:04:01.532Z",
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
          "id": 233,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 234,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 116,
      "obfuscated_id": "PhHGVKqnHFA",
      "author_id": 928,
      "chapter_id": 177,
      "position": 103,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:01.919Z",
      "created_at": "2016-12-04T11:04:01.801Z",
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
          "id": 235,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 236,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 118,
      "obfuscated_id": "ET3wO26jBck",
      "author_id": 934,
      "chapter_id": 179,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:02.464Z",
      "created_at": "2016-12-04T11:04:02.349Z",
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
          "id": 239,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 240,
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
      "author_id": 937,
      "chapter_id": 180,
      "position": 106,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:02.735Z",
      "created_at": "2016-12-04T11:04:02.625Z",
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
          "id": 241,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 242,
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
	-H "Authorization: Bearer e6da57f94948cf77901be55f0f47ecc79f85cc03407d71c4c5bcdc4c6a797264"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 86ce0c864d4a6029d4eec9db2132ac10925b0ac75d219ad5946633f851baddb0
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
      "id": 124,
      "obfuscated_id": "TD9SVjPLZ0Q",
      "author_id": 953,
      "chapter_id": 185,
      "position": 111,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-04T11:04:04.152Z",
      "created_at": "2016-12-04T11:04:04.044Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions?status=reported" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 86ce0c864d4a6029d4eec9db2132ac10925b0ac75d219ad5946633f851baddb0"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/108/republish
Content-Type: application/json
Authorization: Bearer 577893384e521e7a6889689793ee6d0761686cdf57b8ef1ecc23d09e1f58cc8f
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/108/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 577893384e521e7a6889689793ee6d0761686cdf57b8ef1ecc23d09e1f58cc8f"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 54ca5ff76b398015322f20f49734af2e65e5b84866097882a11e94a750956c50
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":101,"published":false}}
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
    "creator_id": 262,
    "id": 94,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 73,
    "additional_university_ids": [

    ],
    "topic_id": 101,
    "discipline_id": 101,
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
    "updated_at": "2016-12-04T11:03:12.365Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":101,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54ca5ff76b398015322f20f49734af2e65e5b84866097882a11e94a750956c50"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8cd729de19ba01ecd527e57932c1632c0607f220f7786dc33ca192a7e4dcb0fd
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
      "creator_id": 220,
      "id": 57,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-44",
      "html_url": "https://goskive.com/course/fu-course-44",
      "slug": "fu-course-44",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 64,
      "discipline_id": 64,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 44",
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
      "updated_at": "2016-12-04T11:03:08.838Z",
      "shortname": "fu-course-44"
    },
    {
      "creator_id": 220,
      "id": 58,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-45",
      "html_url": "https://goskive.com/course/fu-course-45",
      "slug": "fu-course-45",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 65,
      "discipline_id": 65,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 45",
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
      "updated_at": "2016-12-04T11:03:08.873Z",
      "shortname": "fu-course-45"
    },
    {
      "creator_id": 221,
      "id": 59,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-46",
      "html_url": "https://goskive.com/course/fu-course-46",
      "slug": "fu-course-46",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 66,
      "discipline_id": 66,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 46",
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
      "updated_at": "2016-12-04T11:03:08.915Z",
      "shortname": "fu-course-46"
    },
    {
      "creator_id": 221,
      "id": 60,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-47",
      "html_url": "https://goskive.com/course/fu-course-47",
      "slug": "fu-course-47",
      "university_id": 58,
      "additional_university_ids": [

      ],
      "topic_id": 67,
      "discipline_id": 67,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 47",
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
      "chapters_updated_at": "2016-12-04T11:03:09.176Z",
      "updated_at": "2016-12-04T11:03:09.182Z",
      "shortname": "fu-course-47"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cd729de19ba01ecd527e57932c1632c0607f220f7786dc33ca192a7e4dcb0fd"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 95838896214feb959d9ded4dfb591d9d37a1be1017b0cbf9208e771653b7aae3
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
      "creator_id": 226,
      "id": 61,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-48",
      "html_url": "https://goskive.com/course/fu-course-48",
      "slug": "fu-course-48",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 68,
      "discipline_id": 68,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 48",
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
      "updated_at": "2016-12-04T11:03:09.360Z",
      "shortname": "fu-course-48"
    },
    {
      "creator_id": 226,
      "id": 62,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-49",
      "html_url": "https://goskive.com/course/fu-course-49",
      "slug": "fu-course-49",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 69,
      "discipline_id": 69,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 49",
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
      "updated_at": "2016-12-04T11:03:09.397Z",
      "shortname": "fu-course-49"
    },
    {
      "creator_id": 227,
      "id": 63,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-50",
      "html_url": "https://goskive.com/course/fu-course-50",
      "slug": "fu-course-50",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 70,
      "discipline_id": 70,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 50",
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
      "updated_at": "2016-12-04T11:03:09.441Z",
      "shortname": "fu-course-50"
    },
    {
      "creator_id": 227,
      "id": 64,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-51",
      "html_url": "https://goskive.com/course/fu-course-51",
      "slug": "fu-course-51",
      "university_id": 59,
      "additional_university_ids": [

      ],
      "topic_id": 71,
      "discipline_id": 71,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 51",
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
      "updated_at": "2016-12-04T11:03:09.478Z",
      "shortname": "fu-course-51"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 95838896214feb959d9ded4dfb591d9d37a1be1017b0cbf9208e771653b7aae3"
```
