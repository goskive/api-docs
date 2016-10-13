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
DELETE /v2/chapters/127
Content-Type: application/json
Authorization: Bearer e9d87b26990139e62d01309e50a1a7c74ce36caa67f7bd27d5997d2dd1a66315
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/127" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e9d87b26990139e62d01309e50a1a7c74ce36caa67f7bd27d5997d2dd1a66315"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/122
Content-Type: application/json
Authorization: Bearer 968da29770cfe44017df985d1a0b44dec5946ab889f7b5e4fd6848974123b28c
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
    "id": 122,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-13T12:52:24.748Z",
    "course_id": 165,
    "author_id": 612,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-13T12:52:24.145Z",
    "questions_updated_at": "2016-10-13T12:52:24.145Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 87,
        "obfuscated_id": "Jisk1d9Nmeo",
        "author_id": 615,
        "chapter_id": 122,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:24.685Z",
        "created_at": "2016-10-13T12:52:24.685Z",
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
        "author_id": 616,
        "chapter_id": 122,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:24.729Z",
        "created_at": "2016-10-13T12:52:24.729Z",
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
        "id": 89,
        "obfuscated_id": "5eRHrGHLqZk",
        "author_id": 613,
        "chapter_id": 122,
        "position": 85,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:24.390Z",
        "created_at": "2016-10-13T12:52:24.266Z",
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
            "id": 180,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 181,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 90,
        "obfuscated_id": "gX_ALSaJ0k4",
        "author_id": 614,
        "chapter_id": 122,
        "position": 86,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:24.606Z",
        "created_at": "2016-10-13T12:52:24.471Z",
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
            "id": 182,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 183,
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
curl "api.goskive.com/v2/chapters/122" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 968da29770cfe44017df985d1a0b44dec5946ab889f7b5e4fd6848974123b28c"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/125
Content-Type: application/json
Authorization: Bearer 83b4140bcd2ecbe121562bc9ad5e02d7713ac1028c1d47bc4ed807c2766bcfa2
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
    "id": 125,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-13T12:52:25.283Z",
    "course_id": 168,
    "author_id": 624,
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
curl "api.goskive.com/v2/chapters/125" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 83b4140bcd2ecbe121562bc9ad5e02d7713ac1028c1d47bc4ed807c2766bcfa2"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/22
Content-Type: application/json
Authorization: Bearer 8cbfa6806b591ebc9656b8004b79a70079f61a18e293b82c9fbb55705d37ed7e
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/22" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8cbfa6806b591ebc9656b8004b79a70079f61a18e293b82c9fbb55705d37ed7e"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 4d358611cb032a2bda70fdffd94552b127bebad1f74ad4d0bd0e968ca2d3e66a
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
      "id": 45,
      "author_id": 904,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:50.247Z",
      "status": "published",
      "subject_id": 285,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 906,
      "reply_to_id": 45,
      "created_at": "2016-10-13T12:52:50.340Z",
      "status": "published",
      "subject_id": 286,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 47,
      "author_id": 908,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:50.431Z",
      "status": "published",
      "subject_id": 287,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 910,
      "reply_to_id": 47,
      "created_at": "2016-10-13T12:52:50.521Z",
      "status": "published",
      "subject_id": 288,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 912,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:50.615Z",
      "status": "reported",
      "subject_id": 289,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 50,
      "author_id": 914,
      "reply_to_id": 49,
      "created_at": "2016-10-13T12:52:50.707Z",
      "status": "published",
      "subject_id": 290,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 51,
      "author_id": 916,
      "reply_to_id": 49,
      "created_at": "2016-10-13T12:52:50.800Z",
      "status": "published",
      "subject_id": 291,
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
	-H "Authorization: Bearer 4d358611cb032a2bda70fdffd94552b127bebad1f74ad4d0bd0e968ca2d3e66a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer f8c58ffe173d598eac33fe6f736ca86d7744ada17a7f12526c174ec0f3ac3697
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
      "id": 52,
      "author_id": 919,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:50.956Z",
      "status": "published",
      "subject_id": 292,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 53,
      "author_id": 921,
      "reply_to_id": 52,
      "created_at": "2016-10-13T12:52:51.048Z",
      "status": "published",
      "subject_id": 293,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 54,
      "author_id": 923,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:51.141Z",
      "status": "published",
      "subject_id": 294,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 55,
      "author_id": 925,
      "reply_to_id": 54,
      "created_at": "2016-10-13T12:52:51.236Z",
      "status": "published",
      "subject_id": 295,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 56,
      "author_id": 927,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:51.329Z",
      "status": "reported",
      "subject_id": 296,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 57,
      "author_id": 929,
      "reply_to_id": 56,
      "created_at": "2016-10-13T12:52:51.420Z",
      "status": "published",
      "subject_id": 297,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 58,
      "author_id": 931,
      "reply_to_id": 56,
      "created_at": "2016-10-13T12:52:51.512Z",
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
	-H "Authorization: Bearer f8c58ffe173d598eac33fe6f736ca86d7744ada17a7f12526c174ec0f3ac3697"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 2d03d6cf14d54e2779d185c74377cb234b2cc2738a56bd30ebb7d04ce3887139
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
      "author_id": 876,
      "reply_to_id": 31,
      "created_at": "2016-10-13T12:52:48.908Z",
      "status": "published",
      "subject_id": 272,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 880,
      "reply_to_id": 33,
      "created_at": "2016-10-13T12:52:49.094Z",
      "status": "published",
      "subject_id": 274,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 884,
      "reply_to_id": 35,
      "created_at": "2016-10-13T12:52:49.280Z",
      "status": "published",
      "subject_id": 276,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 886,
      "reply_to_id": 35,
      "created_at": "2016-10-13T12:52:49.373Z",
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
curl "api.goskive.com/v2/comments?level=replies" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2d03d6cf14d54e2779d185c74377cb234b2cc2738a56bd30ebb7d04ce3887139"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 9b68722fcdc2275e46d6ba51f3e4322d8f8c79bebacb0fe092c0a1a15e9f8662
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
      "author_id": 897,
      "reply_to_id": null,
      "created_at": "2016-10-13T12:52:49.924Z",
      "status": "reported",
      "subject_id": 282,
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
	-H "Authorization: Bearer 9b68722fcdc2275e46d6ba51f3e4322d8f8c79bebacb0fe092c0a1a15e9f8662"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/60/republish
Content-Type: application/json
Authorization: Bearer 0eea0ef931b6de720f9bb7c4e0d1e61bad3a5962a1d8e353f3ae281add9ede97
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/60/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0eea0ef931b6de720f9bb7c4e0d1e61bad3a5962a1d8e353f3ae281add9ede97"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/216/chapters
Content-Type: application/json
Authorization: Bearer 5833eaa669f7e8e976e82e6822773ad214c2beab0c8365ef6135c632777895bd
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
    "id": 183,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T12:52:42.242Z",
    "course_id": 216,
    "author_id": 794,
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
curl "api.goskive.com/v2/courses/216/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5833eaa669f7e8e976e82e6822773ad214c2beab0c8365ef6135c632777895bd"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 8d33da27a4fbe239529dab7aedce1bf4de95c4fd67146a51f2580b6aad611f44
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
    "id": 185,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-13T12:52:42.623Z",
    "course_id": 219,
    "author_id": 800,
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
	-H "Authorization: Bearer 8d33da27a4fbe239529dab7aedce1bf4de95c4fd67146a51f2580b6aad611f44"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 69a29feac610ff52a9c6e5ad48eaff23e6b7a836457cc1e86a7e2200c054f899
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
      "id": 174,
      "title": "Clever Chapter Title 156",
      "position": 1,
      "updated_at": "2016-10-13T12:52:41.113Z",
      "course_id": 211,
      "author_id": 773,
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
      "id": 175,
      "title": "Clever Chapter Title 157",
      "position": 2,
      "updated_at": "2016-10-13T12:52:41.140Z",
      "course_id": 211,
      "author_id": 774,
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
      "id": 176,
      "title": "Clever Chapter Title 158",
      "position": 3,
      "updated_at": "2016-10-13T12:52:41.431Z",
      "course_id": 211,
      "author_id": 775,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-13T12:52:41.031Z",
      "questions_updated_at": "2016-10-13T12:52:41.031Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 69a29feac610ff52a9c6e5ad48eaff23e6b7a836457cc1e86a7e2200c054f899"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 58bf8d3771dc93d9210252caccdfc12a01b30891146470f49436e189b35eb5fc
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
      "id": 177,
      "title": "Clever Chapter Title 159",
      "position": 1,
      "updated_at": "2016-10-13T12:52:41.582Z",
      "course_id": 212,
      "author_id": 780,
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
      "id": 178,
      "title": "Clever Chapter Title 160",
      "position": 2,
      "updated_at": "2016-10-13T12:52:41.610Z",
      "course_id": 212,
      "author_id": 781,
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
      "id": 179,
      "title": "Clever Chapter Title 161",
      "position": 3,
      "updated_at": "2016-10-13T12:52:41.637Z",
      "course_id": 212,
      "author_id": 782,
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
	-H "Authorization: Bearer 58bf8d3771dc93d9210252caccdfc12a01b30891146470f49436e189b35eb5fc"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/93
Content-Type: application/json
Authorization: Bearer 4a397dc4d3220b245530fb3ed47edf22971e90df407dd18babbb4dfd6bf36413
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/93" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4a397dc4d3220b245530fb3ed47edf22971e90df407dd18babbb4dfd6bf36413"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a863b2324567584ae53ef324db786a537674c63598dd5e557643dfcebdf72faa
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
	-H "Authorization: Bearer a863b2324567584ae53ef324db786a537674c63598dd5e557643dfcebdf72faa"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer a352f66fecea72a1810311a4f091bec48896a99eef67e3a13bd216390b9352ef
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
    "creator_id": 367,
    "id": 103,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 103,
    "additional_university_ids": [

    ],
    "topic_id": 103,
    "discipline_id": 103,
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
    "chapters_updated_at": "2016-10-13T12:52:00.060Z",
    "updated_at": "2016-10-13T12:52:01.630Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 83,
        "title": "Clever Chapter Title 77",
        "position": 1,
        "updated_at": "2016-10-13T12:52:01.576Z",
        "course_id": 103,
        "author_id": 367,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T12:52:00.060Z",
        "questions_updated_at": "2016-10-13T12:52:00.060Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 84,
        "title": "Clever Chapter Title 78",
        "position": 2,
        "updated_at": "2016-10-13T12:52:01.621Z",
        "course_id": 103,
        "author_id": 367,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-13T12:52:00.060Z",
        "questions_updated_at": "2016-10-13T12:52:00.060Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 54,
        "obfuscated_id": "cKxlQSpHm5w",
        "author_id": 367,
        "chapter_id": 83,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.400Z",
        "created_at": "2016-10-13T12:52:01.400Z",
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
        "id": 56,
        "obfuscated_id": "PgrpyPCfpqo",
        "author_id": 367,
        "chapter_id": 84,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.476Z",
        "created_at": "2016-10-13T12:52:01.476Z",
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
        "id": 55,
        "obfuscated_id": "VX19tR4fHZ8",
        "author_id": 367,
        "chapter_id": 83,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.443Z",
        "created_at": "2016-10-13T12:52:01.443Z",
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
        "id": 57,
        "obfuscated_id": "mCV2FECTNQs",
        "author_id": 367,
        "chapter_id": 84,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.520Z",
        "created_at": "2016-10-13T12:52:01.520Z",
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
        "id": 58,
        "obfuscated_id": "_S2mxc1kfck",
        "author_id": 370,
        "chapter_id": 83,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.565Z",
        "created_at": "2016-10-13T12:52:01.565Z",
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
        "id": 59,
        "obfuscated_id": "fo0taK4dosk",
        "author_id": 371,
        "chapter_id": 84,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-13T12:52:01.609Z",
        "created_at": "2016-10-13T12:52:01.609Z",
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
	-H "Authorization: Bearer a352f66fecea72a1810311a4f091bec48896a99eef67e3a13bd216390b9352ef"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/92
Content-Type: application/json
Authorization: Bearer 3a89df48592592db519b2278b3cf7a33802090fe806728f6c7393d9d1bd3b60e
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
    "creator_id": 339,
    "id": 92,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 92,
    "additional_university_ids": [

    ],
    "topic_id": 92,
    "discipline_id": 92,
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
    "updated_at": "2016-10-13T12:51:56.631Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/92" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3a89df48592592db519b2278b3cf7a33802090fe806728f6c7393d9d1bd3b60e"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer a6a302576e27ac4ceef79757592cb8c61992d2cd5c4a534615067438a9ef2c69
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
    "creator_id": 337,
    "id": 91,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 91,
    "additional_university_ids": [

    ],
    "topic_id": 91,
    "discipline_id": 91,
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
    "updated_at": "2016-10-13T12:51:56.448Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a6a302576e27ac4ceef79757592cb8c61992d2cd5c4a534615067438a9ef2c69"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer f4d528b547a1b986f2ad65e9bd913c856170e15287b451110b795f11771e15da
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
      "id": 2,
      "user_id": 52,
      "feedbackable_id": 10,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:51:33.730Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 56,
      "feedbackable_id": 11,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:51:34.039Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 60,
      "feedbackable_id": 12,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:51:34.344Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 5,
      "user_id": 64,
      "feedbackable_id": 13,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:51:34.649Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 6,
      "user_id": 68,
      "feedbackable_id": 14,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T12:51:34.958Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f4d528b547a1b986f2ad65e9bd913c856170e15287b451110b795f11771e15da"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 91b35d5d2fb9f03e71fa8e6003bcbfa869ef81a0ca46dfb4843a40928c685d13
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
      "id": 11,
      "user_id": 89,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-13T12:51:36.621Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 91b35d5d2fb9f03e71fa8e6003bcbfa869ef81a0ca46dfb4843a40928c685d13"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/6
Authorization: Bearer 3f4a23179416db7af18d723500dcffd84e78f1d7ba154d57238680add8545898
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
	-H "Authorization: Bearer 3f4a23179416db7af18d723500dcffd84e78f1d7ba154d57238680add8545898" \
	-H "Content-Type: application/x-www-form-urlencoded"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/81/feedbacks
Content-Type: application/json
Authorization: Bearer 67ce13e48cc25a232fa469a0cec9a3291c7b89aa7be552909aefe72edc210524
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
      "user_id": 534,
      "feedbackable_id": 81,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:52:18.293Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 43,
      "user_id": 533,
      "feedbackable_id": 81,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:52:18.280Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/81/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 67ce13e48cc25a232fa469a0cec9a3291c7b89aa7be552909aefe72edc210524"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 9ea3a34b0ef49ef3469e5ff30685a004e2ddaa485ad6d649a60733220db64b46
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 255,
      "chapter_id": 53,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:51.428Z",
      "created_at": "2016-10-13T12:51:51.428Z",
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
      "author_id": 258,
      "chapter_id": 54,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:51.576Z",
      "created_at": "2016-10-13T12:51:51.576Z",
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
      "author_id": 261,
      "chapter_id": 55,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:51.725Z",
      "created_at": "2016-10-13T12:51:51.725Z",
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
      "id": 25,
      "obfuscated_id": "HsmcIJXdRE4",
      "author_id": 264,
      "chapter_id": 56,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:51.871Z",
      "created_at": "2016-10-13T12:51:51.871Z",
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
      "id": 26,
      "obfuscated_id": "cWAsrz6MOVI",
      "author_id": 267,
      "chapter_id": 57,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:52.020Z",
      "created_at": "2016-10-13T12:51:52.020Z",
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
	-H "Authorization: Bearer 9ea3a34b0ef49ef3469e5ff30685a004e2ddaa485ad6d649a60733220db64b46"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer c09b5202b0d94ab2c585564860e45fc1d89b3269e5c822f398d75a7321184d1f
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
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 283,
      "chapter_id": 62,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:51:52.878Z",
      "created_at": "2016-10-13T12:51:52.878Z",
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
	-H "Authorization: Bearer c09b5202b0d94ab2c585564860e45fc1d89b3269e5c822f398d75a7321184d1f"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/42/republish
Content-Type: application/json
Authorization: Bearer 77bc0f18eefdfcabf78c0dc862161c533fd0fd5e17c067e505639f4aafc3df1a
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/42/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77bc0f18eefdfcabf78c0dc862161c533fd0fd5e17c067e505639f4aafc3df1a"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/73/feedbacks
Content-Type: application/json
Authorization: Bearer 4e0112d79cd76b4426977b97407117752b2c43a621a686ba7b77c4e128dc4db9
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
      "id": 36,
      "user_id": 442,
      "feedbackable_id": 73,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:52:11.401Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 35,
      "user_id": 441,
      "feedbackable_id": 73,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-13T12:52:11.388Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/73/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4e0112d79cd76b4426977b97407117752b2c43a621a686ba7b77c4e128dc4db9"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 3b6ce7240b8b68b4b49707b6010628a2322c31c4840ebcf530e29ea0f27458d4
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
      "id": 103,
      "obfuscated_id": "AVhVflMAvL0",
      "author_id": 676,
      "chapter_id": 140,
      "position": 99,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:30.684Z",
      "created_at": "2016-10-13T12:52:30.540Z",
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
      "id": 100,
      "obfuscated_id": "erXmBhoMZFI",
      "author_id": 667,
      "chapter_id": 137,
      "position": 96,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:29.710Z",
      "created_at": "2016-10-13T12:52:29.576Z",
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
          "id": 202,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 203,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 101,
      "obfuscated_id": "PprZyBVq_gc",
      "author_id": 670,
      "chapter_id": 138,
      "position": 97,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:30.033Z",
      "created_at": "2016-10-13T12:52:29.896Z",
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
          "id": 204,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 205,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 102,
      "obfuscated_id": "jFy90P7ldB4",
      "author_id": 673,
      "chapter_id": 139,
      "position": 98,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:30.355Z",
      "created_at": "2016-10-13T12:52:30.217Z",
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
          "id": 206,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 207,
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
      "author_id": 679,
      "chapter_id": 141,
      "position": 100,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:31.001Z",
      "created_at": "2016-10-13T12:52:30.869Z",
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
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b6ce7240b8b68b4b49707b6010628a2322c31c4840ebcf530e29ea0f27458d4"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 0b88ef9025e66ab31a1683af8ff41ca18c6396da3f1bf3811c8a5b87f4945b0a
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
      "id": 109,
      "obfuscated_id": "VSPyck5c2RY",
      "author_id": 695,
      "chapter_id": 146,
      "position": 105,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-13T12:52:32.703Z",
      "created_at": "2016-10-13T12:52:32.574Z",
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
          "id": 220,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 221,
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
	-H "Authorization: Bearer 0b88ef9025e66ab31a1683af8ff41ca18c6396da3f1bf3811c8a5b87f4945b0a"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/115/republish
Content-Type: application/json
Authorization: Bearer 43b0af1e6390f984bc55429e64a58085ac0f50508bf1af21876b288f21c01541
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/115/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 43b0af1e6390f984bc55429e64a58085ac0f50508bf1af21876b288f21c01541"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 168b715edae2aedff2de3f30cee4a6b9488fe72a731e7bc6de058b0f206406d5
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":271,"published":false}}
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
    "creator_id": 845,
    "id": 259,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 244,
    "additional_university_ids": [

    ],
    "topic_id": 271,
    "discipline_id": 272,
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
    "updated_at": "2016-10-13T12:52:47.400Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":271,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 168b715edae2aedff2de3f30cee4a6b9488fe72a731e7bc6de058b0f206406d5"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d5be89b9d08ce282d9baada6bbc7a3fe23f09df3cb9be1c5d1f8ca9978fcd260
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
      "creator_id": 805,
      "id": 224,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-156",
      "html_url": "https://goskive.com/course/fu-course-156",
      "slug": "fu-course-156",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 236,
      "discipline_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 156",
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
      "updated_at": "2016-10-13T12:52:43.054Z",
      "shortname": "fu-course-156"
    },
    {
      "creator_id": 805,
      "id": 225,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-157",
      "html_url": "https://goskive.com/course/fu-course-157",
      "slug": "fu-course-157",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 237,
      "discipline_id": 238,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 157",
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
      "updated_at": "2016-10-13T12:52:43.097Z",
      "shortname": "fu-course-157"
    },
    {
      "creator_id": 806,
      "id": 226,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-158",
      "html_url": "https://goskive.com/course/fu-course-158",
      "slug": "fu-course-158",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 238,
      "discipline_id": 239,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 158",
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
      "updated_at": "2016-10-13T12:52:43.147Z",
      "shortname": "fu-course-158"
    },
    {
      "creator_id": 806,
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-159",
      "html_url": "https://goskive.com/course/fu-course-159",
      "slug": "fu-course-159",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 239,
      "discipline_id": 240,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 159",
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
      "chapters_updated_at": "2016-10-13T12:52:43.472Z",
      "updated_at": "2016-10-13T12:52:43.480Z",
      "shortname": "fu-course-159"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5be89b9d08ce282d9baada6bbc7a3fe23f09df3cb9be1c5d1f8ca9978fcd260"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 8a01eb327057195985a02d17a4470848fda60c4b40ce30d4f8d65a4cd1a158da
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
      "creator_id": 812,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-160",
      "html_url": "https://goskive.com/course/fu-course-160",
      "slug": "fu-course-160",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 240,
      "discipline_id": 241,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 160",
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
      "updated_at": "2016-10-13T12:52:43.702Z",
      "shortname": "fu-course-160"
    },
    {
      "creator_id": 812,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-161",
      "html_url": "https://goskive.com/course/fu-course-161",
      "slug": "fu-course-161",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 241,
      "discipline_id": 242,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 161",
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
      "updated_at": "2016-10-13T12:52:43.746Z",
      "shortname": "fu-course-161"
    },
    {
      "creator_id": 813,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-162",
      "html_url": "https://goskive.com/course/fu-course-162",
      "slug": "fu-course-162",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 242,
      "discipline_id": 243,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 162",
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
      "updated_at": "2016-10-13T12:52:43.799Z",
      "shortname": "fu-course-162"
    },
    {
      "creator_id": 813,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-163",
      "html_url": "https://goskive.com/course/fu-course-163",
      "slug": "fu-course-163",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 243,
      "discipline_id": 244,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 163",
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
      "updated_at": "2016-10-13T12:52:43.844Z",
      "shortname": "fu-course-163"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 8a01eb327057195985a02d17a4470848fda60c4b40ce30d4f8d65a4cd1a158da"
```
