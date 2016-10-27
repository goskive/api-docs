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
DELETE /v2/chapters/83
Content-Type: application/json
Authorization: Bearer 12af7b3554a092f79437fd0533d1ab6d4605738cff7a16aa3051b844ffbcfaad
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/83" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 12af7b3554a092f79437fd0533d1ab6d4605738cff7a16aa3051b844ffbcfaad"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/78
Content-Type: application/json
Authorization: Bearer dc0735a143216ecd8d3892504e1a23efb9dbe5f24eeca4516a67d25534af6408
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
    "id": 78,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-27T17:15:18.205Z",
    "course_id": 83,
    "author_id": 303,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-27T17:15:17.645Z",
    "questions_updated_at": "2016-10-27T17:15:17.645Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 306,
        "chapter_id": 78,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:18.148Z",
        "created_at": "2016-10-27T17:15:18.148Z",
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
        "author_id": 307,
        "chapter_id": 78,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:18.187Z",
        "created_at": "2016-10-27T17:15:18.187Z",
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
        "author_id": 304,
        "chapter_id": 78,
        "position": 36,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:17.867Z",
        "created_at": "2016-10-27T17:15:17.749Z",
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
            "id": 101,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 102,
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
        "author_id": 305,
        "chapter_id": 78,
        "position": 37,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:18.074Z",
        "created_at": "2016-10-27T17:15:17.944Z",
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
            "id": 103,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 104,
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
curl "api.goskive.com/v2/chapters/78" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc0735a143216ecd8d3892504e1a23efb9dbe5f24eeca4516a67d25534af6408"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/77
Content-Type: application/json
Authorization: Bearer 38ec2a61cf0ba23a148d98be53adcfeafbac4743917b8d42b5c901e5f230dee9
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
    "id": 77,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-27T17:15:17.614Z",
    "course_id": 82,
    "author_id": 300,
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
curl "api.goskive.com/v2/chapters/77" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 38ec2a61cf0ba23a148d98be53adcfeafbac4743917b8d42b5c901e5f230dee9"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/20
Content-Type: application/json
Authorization: Bearer 8a930416886275eae6629fceef92eee996a5a419f009d5cf08fa11194e6f8be9
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/20" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a930416886275eae6629fceef92eee996a5a419f009d5cf08fa11194e6f8be9"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 2355c71ef8b997c3b751fb69512869ef66adde1b257875207b4ebd40d73c8455
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
      "author_id": 875,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:07.962Z",
      "status": "published",
      "subject_id": 271,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 877,
      "reply_to_id": 32,
      "created_at": "2016-10-27T17:16:08.048Z",
      "status": "published",
      "subject_id": 272,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 879,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:08.134Z",
      "status": "published",
      "subject_id": 273,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 881,
      "reply_to_id": 34,
      "created_at": "2016-10-27T17:16:08.251Z",
      "status": "published",
      "subject_id": 274,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 883,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:08.333Z",
      "status": "reported",
      "subject_id": 275,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 885,
      "reply_to_id": 36,
      "created_at": "2016-10-27T17:16:08.416Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 887,
      "reply_to_id": 36,
      "created_at": "2016-10-27T17:16:08.499Z",
      "status": "published",
      "subject_id": 277,
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
	-H "Authorization: Bearer 2355c71ef8b997c3b751fb69512869ef66adde1b257875207b4ebd40d73c8455"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e3ad04a0c3e72b73552daa57598626ee87b307f5fd1360c6c0f235a0a3cfb8d1
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
      "id": 39,
      "author_id": 890,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:08.637Z",
      "status": "published",
      "subject_id": 278,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 892,
      "reply_to_id": 39,
      "created_at": "2016-10-27T17:16:08.721Z",
      "status": "published",
      "subject_id": 279,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 894,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:08.805Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 42,
      "author_id": 896,
      "reply_to_id": 41,
      "created_at": "2016-10-27T17:16:08.888Z",
      "status": "published",
      "subject_id": 281,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 898,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:08.972Z",
      "status": "reported",
      "subject_id": 282,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 900,
      "reply_to_id": 43,
      "created_at": "2016-10-27T17:16:09.055Z",
      "status": "published",
      "subject_id": 283,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 45,
      "author_id": 902,
      "reply_to_id": 43,
      "created_at": "2016-10-27T17:16:09.145Z",
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
	-H "Authorization: Bearer e3ad04a0c3e72b73552daa57598626ee87b307f5fd1360c6c0f235a0a3cfb8d1"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer fee081deed25fb2a27e8f70b517712275756331e05b67faf2f0d28262e6fb427
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
      "author_id": 862,
      "reply_to_id": 25,
      "created_at": "2016-10-27T17:16:07.405Z",
      "status": "published",
      "subject_id": 265,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 866,
      "reply_to_id": 27,
      "created_at": "2016-10-27T17:16:07.573Z",
      "status": "published",
      "subject_id": 267,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 870,
      "reply_to_id": 29,
      "created_at": "2016-10-27T17:16:07.742Z",
      "status": "published",
      "subject_id": 269,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 872,
      "reply_to_id": 29,
      "created_at": "2016-10-27T17:16:07.826Z",
      "status": "published",
      "subject_id": 270,
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
	-H "Authorization: Bearer fee081deed25fb2a27e8f70b517712275756331e05b67faf2f0d28262e6fb427"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 1736c664d2f63a43b1eaf33fe0606bc594b202c78b7ea42a20e29cb01504d5cc
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
      "id": 50,
      "author_id": 913,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:16:09.639Z",
      "status": "reported",
      "subject_id": 289,
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
	-H "Authorization: Bearer 1736c664d2f63a43b1eaf33fe0606bc594b202c78b7ea42a20e29cb01504d5cc"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/23/republish
Content-Type: application/json
Authorization: Bearer 00ad56ab89e6a7073305b0a107e182a4fd2ef54347fd626170a9ea722ef35210
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/23/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 00ad56ab89e6a7073305b0a107e182a4fd2ef54347fd626170a9ea722ef35210"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/102/chapters
Content-Type: application/json
Authorization: Bearer 155a5d427419acdc6385a9b4f1230f579ddb771108d1ec3df505a9f1da43afd2
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
    "updated_at": "2016-10-27T17:15:23.576Z",
    "course_id": 102,
    "author_id": 368,
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
curl "api.goskive.com/v2/courses/102/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 155a5d427419acdc6385a9b4f1230f579ddb771108d1ec3df505a9f1da43afd2"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 139f3402f4c500ededb8f88da208c46e8d64455a70e58eb68beb3ce43c25d4ad
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
    "updated_at": "2016-10-27T17:15:23.931Z",
    "course_id": 105,
    "author_id": 374,
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
	-H "Authorization: Bearer 139f3402f4c500ededb8f88da208c46e8d64455a70e58eb68beb3ce43c25d4ad"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 3ab6222bcf6c791294e1e03e885b1a65829401021455987a1310a5ec6ab42cc0
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
      "id": 103,
      "title": "Clever Chapter Title 85",
      "position": 1,
      "updated_at": "2016-10-27T17:15:25.089Z",
      "course_id": 111,
      "author_id": 397,
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
      "id": 104,
      "title": "Clever Chapter Title 86",
      "position": 2,
      "updated_at": "2016-10-27T17:15:25.115Z",
      "course_id": 111,
      "author_id": 398,
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
      "id": 105,
      "title": "Clever Chapter Title 87",
      "position": 3,
      "updated_at": "2016-10-27T17:15:25.385Z",
      "course_id": 111,
      "author_id": 399,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-27T17:15:25.016Z",
      "questions_updated_at": "2016-10-27T17:15:25.016Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3ab6222bcf6c791294e1e03e885b1a65829401021455987a1310a5ec6ab42cc0"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer cbf38884cdca426b2ddce8e07b76ba4e606b114828e74a0f20404866c6510749
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
      "id": 106,
      "title": "Clever Chapter Title 88",
      "position": 1,
      "updated_at": "2016-10-27T17:15:25.764Z",
      "course_id": 113,
      "author_id": 406,
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
      "id": 107,
      "title": "Clever Chapter Title 89",
      "position": 2,
      "updated_at": "2016-10-27T17:15:25.791Z",
      "course_id": 113,
      "author_id": 407,
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
      "id": 108,
      "title": "Clever Chapter Title 90",
      "position": 3,
      "updated_at": "2016-10-27T17:15:25.817Z",
      "course_id": 113,
      "author_id": 408,
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
	-H "Authorization: Bearer cbf38884cdca426b2ddce8e07b76ba4e606b114828e74a0f20404866c6510749"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/185
Content-Type: application/json
Authorization: Bearer 18718829d01f68a8745e824e91b3d1ba08c714f273177b7a3264a1b2dfe60fe4
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/185" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18718829d01f68a8745e824e91b3d1ba08c714f273177b7a3264a1b2dfe60fe4"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 907abda73a2b8a2821a89714ebf6d3643f8953e65b028ee0725efe2a8d9bbba2
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
	-H "Authorization: Bearer 907abda73a2b8a2821a89714ebf6d3643f8953e65b028ee0725efe2a8d9bbba2"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 460390ee2f5d43ce1f8d33f7102d83fcae828d591fd6fc008605d9d40432535f
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
    "creator_id": 572,
    "id": 183,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 167,
    "additional_university_ids": [

    ],
    "topic_id": 193,
    "discipline_id": 193,
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
    "chapters_updated_at": "2016-10-27T17:15:40.872Z",
    "updated_at": "2016-10-27T17:15:42.472Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 143,
        "title": "Clever Chapter Title 119",
        "position": 1,
        "updated_at": "2016-10-27T17:15:42.424Z",
        "course_id": 183,
        "author_id": 572,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-27T17:15:40.872Z",
        "questions_updated_at": "2016-10-27T17:15:40.872Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 144,
        "title": "Clever Chapter Title 120",
        "position": 2,
        "updated_at": "2016-10-27T17:15:42.464Z",
        "course_id": 183,
        "author_id": 572,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-27T17:15:40.872Z",
        "questions_updated_at": "2016-10-27T17:15:40.872Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 69,
        "obfuscated_id": "1EDi_PBgOnI",
        "author_id": 572,
        "chapter_id": 143,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.257Z",
        "created_at": "2016-10-27T17:15:42.257Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 572,
        "chapter_id": 144,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.331Z",
        "created_at": "2016-10-27T17:15:42.331Z",
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
        "author_id": 572,
        "chapter_id": 143,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.299Z",
        "created_at": "2016-10-27T17:15:42.299Z",
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
        "author_id": 572,
        "chapter_id": 144,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.374Z",
        "created_at": "2016-10-27T17:15:42.374Z",
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
        "author_id": 575,
        "chapter_id": 143,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.413Z",
        "created_at": "2016-10-27T17:15:42.413Z",
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
        "id": 74,
        "obfuscated_id": "fL3buOIYvUI",
        "author_id": 576,
        "chapter_id": 144,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:15:42.453Z",
        "created_at": "2016-10-27T17:15:42.453Z",
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
	-H "Authorization: Bearer 460390ee2f5d43ce1f8d33f7102d83fcae828d591fd6fc008605d9d40432535f"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/177
Content-Type: application/json
Authorization: Bearer 04b410d4965cb69431621438305970d3820c535c03133b3aa2a8a91f7da8a41a
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
    "creator_id": 554,
    "id": 177,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 161,
    "additional_university_ids": [

    ],
    "topic_id": 187,
    "discipline_id": 187,
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
    "updated_at": "2016-10-27T17:15:37.153Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/177" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 04b410d4965cb69431621438305970d3820c535c03133b3aa2a8a91f7da8a41a"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer cac81c62462052f45b019e1f4f5be5f62c09ca4b9d70ab497c57e5ff634d30b5
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
    "creator_id": 558,
    "id": 179,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 163,
    "additional_university_ids": [

    ],
    "topic_id": 189,
    "discipline_id": 189,
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
    "updated_at": "2016-10-27T17:15:37.386Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cac81c62462052f45b019e1f4f5be5f62c09ca4b9d70ab497c57e5ff634d30b5"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 2a19e2ea65125b14811c4f65863320ca0fc9500106156103321af94577cc3530
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
      "user_id": 684,
      "feedbackable_id": 113,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:53.021Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 688,
      "feedbackable_id": 114,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:53.369Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 34,
      "user_id": 692,
      "feedbackable_id": 115,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:53.721Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 696,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:54.090Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 36,
      "user_id": 700,
      "feedbackable_id": 117,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-27T17:15:54.507Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2a19e2ea65125b14811c4f65863320ca0fc9500106156103321af94577cc3530"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 7dc7d84c0b22ee9a00d689fdac9934172af8756a9598c3d91709d53dd65da148
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
      "user_id": 679,
      "feedbackable_id": 112,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-27T17:15:52.624Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 7dc7d84c0b22ee9a00d689fdac9934172af8756a9598c3d91709d53dd65da148"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/13
Content-Type: application/json
Authorization: Bearer fe0dfb8dcc17c4f850d6f1d0c38ba7f715baaac7f0505c09593a6b215cf9450d
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
	-H "Authorization: Bearer fe0dfb8dcc17c4f850d6f1d0c38ba7f715baaac7f0505c09593a6b215cf9450d"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/18/metadata
Content-Type: application/json
Authorization: Bearer 74cf28547cdfe0109edc7362bf60a0f79387f004d8071846d4ae9a87bb233656
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
      "id": 960,
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
      "created_at": "2016-10-27T17:16:11.952Z",
      "updated_at": "2016-10-27T17:16:11.952Z"
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
    "created_at": "2016-10-27T17:16:12.031Z",
    "updated_at": "2016-10-27T17:16:12.031Z",
    "course_id": 308,
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
	-H "Authorization: Bearer 74cf28547cdfe0109edc7362bf60a0f79387f004d8071846d4ae9a87bb233656"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/43/feedbacks
Content-Type: application/json
Authorization: Bearer c69106e12b5be184396c84fdabf55990e5b629a6deb847d38626ee950251fb6a
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
      "user_id": 493,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:32.660Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 492,
      "feedbackable_id": 43,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:32.649Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/43/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c69106e12b5be184396c84fdabf55990e5b629a6deb847d38626ee950251fb6a"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 5631fedc0c680dd861235674619cc16872d5224ff9f80cc6bc6525578ca5244e
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
      "id": 14,
      "obfuscated_id": "gbKzjBR_8tw",
      "author_id": 122,
      "chapter_id": 28,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.395Z",
      "created_at": "2016-10-27T17:15:02.395Z",
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
      "author_id": 125,
      "chapter_id": 29,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.523Z",
      "created_at": "2016-10-27T17:15:02.523Z",
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
      "id": 16,
      "obfuscated_id": "Drq0t9y67cE",
      "author_id": 128,
      "chapter_id": 30,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.662Z",
      "created_at": "2016-10-27T17:15:02.662Z",
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
      "id": 17,
      "obfuscated_id": "s3oqsdqLejU",
      "author_id": 131,
      "chapter_id": 31,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.784Z",
      "created_at": "2016-10-27T17:15:02.784Z",
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
      "id": 18,
      "obfuscated_id": "9KZ-wsvd6MY",
      "author_id": 134,
      "chapter_id": 32,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.904Z",
      "created_at": "2016-10-27T17:15:02.904Z",
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
	-H "Authorization: Bearer 5631fedc0c680dd861235674619cc16872d5224ff9f80cc6bc6525578ca5244e"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 0cb3ad4655360763d3647ce22d210db09bd8780bd93f16a47fc6becab9dcc925
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
      "id": 13,
      "obfuscated_id": "6UMEHi0zidE",
      "author_id": 118,
      "chapter_id": 27,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:02.215Z",
      "created_at": "2016-10-27T17:15:02.215Z",
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
	-H "Authorization: Bearer 0cb3ad4655360763d3647ce22d210db09bd8780bd93f16a47fc6becab9dcc925"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/1/republish
Content-Type: application/json
Authorization: Bearer 8abddd18063ba3eef032ad5bbf86e2019a869363354c207fa172b50daa755897
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/1/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8abddd18063ba3eef032ad5bbf86e2019a869363354c207fa172b50daa755897"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/23/feedbacks
Content-Type: application/json
Authorization: Bearer 3edfe121616679e6bca06949c8c165ca94dca8fa590e5beeb0532db62fe36cb2
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
      "user_id": 198,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:07.172Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 7,
      "user_id": 197,
      "feedbackable_id": 23,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:15:07.161Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/23/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3edfe121616679e6bca06949c8c165ca94dca8fa590e5beeb0532db62fe36cb2"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer f465bc2dc9aa06e3db9fad0f041790391da6328f4109a542bd601b9e587e934b
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 219,
      "chapter_id": 51,
      "position": 21,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:09.019Z",
      "created_at": "2016-10-27T17:15:08.901Z",
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 222,
      "chapter_id": 52,
      "position": 22,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:09.295Z",
      "created_at": "2016-10-27T17:15:09.176Z",
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 216,
      "chapter_id": 50,
      "position": 20,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:08.748Z",
      "created_at": "2016-10-27T17:15:08.627Z",
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
      "id": 27,
      "obfuscated_id": "sJgVCs3QBfA",
      "author_id": 225,
      "chapter_id": 53,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:09.601Z",
      "created_at": "2016-10-27T17:15:09.479Z",
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
    },
    {
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 228,
      "chapter_id": 54,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:09.870Z",
      "created_at": "2016-10-27T17:15:09.757Z",
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
          "id": 58,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 59,
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
	-H "Authorization: Bearer f465bc2dc9aa06e3db9fad0f041790391da6328f4109a542bd601b9e587e934b"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 0d22e22ef7b36dbe591e03471bd2f0e2a237e0ed702a10e1f494db3244f5d732
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
      "id": 33,
      "obfuscated_id": "sjAD-GXxS8o",
      "author_id": 244,
      "chapter_id": 59,
      "position": 29,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:15:11.371Z",
      "created_at": "2016-10-27T17:15:11.257Z",
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
          "id": 68,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 69,
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
	-H "Authorization: Bearer 0d22e22ef7b36dbe591e03471bd2f0e2a237e0ed702a10e1f494db3244f5d732"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/42/republish
Content-Type: application/json
Authorization: Bearer b55d876bcd9b2d716497368dcb3391fc0b4dca74a0c488ae8310e8ef0df0c514
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b55d876bcd9b2d716497368dcb3391fc0b4dca74a0c488ae8310e8ef0df0c514"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 18cb397c0e055b67c16f2a8ea1da3440376c96150961f84c94f2f2aea150e3b1
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
    "creator_id": 464,
    "id": 155,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 134,
    "additional_university_ids": [

    ],
    "topic_id": 157,
    "discipline_id": 157,
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
    "updated_at": "2016-10-27T17:15:30.759Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":157,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 18cb397c0e055b67c16f2a8ea1da3440376c96150961f84c94f2f2aea150e3b1"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer ab587e3772592f8465c05e0172968fe4e5a005e222e879a525ac60884ca66e12
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
      "creator_id": 445,
      "id": 137,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 139,
      "discipline_id": 139,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 107",
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
      "updated_at": "2016-10-27T17:15:28.756Z",
      "shortname": "fu-course-107"
    },
    {
      "creator_id": 445,
      "id": 138,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 140,
      "discipline_id": 140,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 108",
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
      "updated_at": "2016-10-27T17:15:28.795Z",
      "shortname": "fu-course-108"
    },
    {
      "creator_id": 446,
      "id": 139,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 141,
      "discipline_id": 141,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 109",
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
      "updated_at": "2016-10-27T17:15:28.845Z",
      "shortname": "fu-course-109"
    },
    {
      "creator_id": 446,
      "id": 140,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 126,
      "additional_university_ids": [

      ],
      "topic_id": 142,
      "discipline_id": 142,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 110",
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
      "chapters_updated_at": "2016-10-27T17:15:29.159Z",
      "updated_at": "2016-10-27T17:15:29.167Z",
      "shortname": "fu-course-110"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ab587e3772592f8465c05e0172968fe4e5a005e222e879a525ac60884ca66e12"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 330e59475a51d6c9230824bb332999ea37ddd9ffc77aa6fd5a3522d820c1b26d
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
      "creator_id": 451,
      "id": 141,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 127,
      "additional_university_ids": [

      ],
      "topic_id": 143,
      "discipline_id": 143,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 111",
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
      "updated_at": "2016-10-27T17:15:29.314Z",
      "shortname": "fu-course-111"
    },
    {
      "creator_id": 451,
      "id": 142,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-112",
      "html_url": "https://goskive.com/course/fu-course-112",
      "slug": "fu-course-112",
      "university_id": 127,
      "additional_university_ids": [

      ],
      "topic_id": 144,
      "discipline_id": 144,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 112",
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
      "updated_at": "2016-10-27T17:15:29.353Z",
      "shortname": "fu-course-112"
    },
    {
      "creator_id": 452,
      "id": 143,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-113",
      "html_url": "https://goskive.com/course/fu-course-113",
      "slug": "fu-course-113",
      "university_id": 127,
      "additional_university_ids": [

      ],
      "topic_id": 145,
      "discipline_id": 145,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 113",
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
      "updated_at": "2016-10-27T17:15:29.401Z",
      "shortname": "fu-course-113"
    },
    {
      "creator_id": 452,
      "id": 144,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-114",
      "html_url": "https://goskive.com/course/fu-course-114",
      "slug": "fu-course-114",
      "university_id": 127,
      "additional_university_ids": [

      ],
      "topic_id": 146,
      "discipline_id": 146,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 114",
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
      "updated_at": "2016-10-27T17:15:29.440Z",
      "shortname": "fu-course-114"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 330e59475a51d6c9230824bb332999ea37ddd9ffc77aa6fd5a3522d820c1b26d"
```
