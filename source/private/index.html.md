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
DELETE /v2/chapters/24
Content-Type: application/json
Authorization: Bearer 9ef8a6a8877e05aa2d40f71d55cd41a3dca93e3198d723c1a875d45a8bfd2d4f
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/24" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9ef8a6a8877e05aa2d40f71d55cd41a3dca93e3198d723c1a875d45a8bfd2d4f"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/28
Content-Type: application/json
Authorization: Bearer 90db1c7b9bffd3dbe92df040ce1d629cf9e2e7a6447c66d6b97fc8f32863ed30
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
    "id": 28,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-10-26T18:00:26.492Z",
    "course_id": 35,
    "author_id": 112,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-26T18:00:25.924Z",
    "questions_updated_at": "2016-10-26T18:00:25.924Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 27,
        "obfuscated_id": "sJgVCs3QBfA",
        "author_id": 115,
        "chapter_id": 28,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:26.436Z",
        "created_at": "2016-10-26T18:00:26.436Z",
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
        "id": 28,
        "obfuscated_id": "hO6PHFgN8Aw",
        "author_id": 116,
        "chapter_id": 28,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:26.473Z",
        "created_at": "2016-10-26T18:00:26.473Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 113,
        "chapter_id": 28,
        "position": 37,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:26.150Z",
        "created_at": "2016-10-26T18:00:26.027Z",
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
            "id": 73,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 74,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 114,
        "chapter_id": 28,
        "position": 38,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:26.361Z",
        "created_at": "2016-10-26T18:00:26.225Z",
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
            "id": 75,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 76,
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
curl "api.goskive.com/v2/chapters/28" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 90db1c7b9bffd3dbe92df040ce1d629cf9e2e7a6447c66d6b97fc8f32863ed30"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/27
Content-Type: application/json
Authorization: Bearer ea61a1ae9330fb421e339354b593bb4ea8379584a1e3dc6f2b5cacec59cdedb0
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
    "id": 27,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-26T18:00:25.894Z",
    "course_id": 34,
    "author_id": 109,
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
curl "api.goskive.com/v2/chapters/27" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ea61a1ae9330fb421e339354b593bb4ea8379584a1e3dc6f2b5cacec59cdedb0"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/55
Content-Type: application/json
Authorization: Bearer b1e16e1b9b72f7dd0741e206ea8ae4296abf0beaa3509ed9f4a848d0cd726ec0
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
	-H "Authorization: Bearer b1e16e1b9b72f7dd0741e206ea8ae4296abf0beaa3509ed9f4a848d0cd726ec0"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer e10a0e8d7e9e3429a79c6d6a345fce21757ee26a17e8e6e415a564576be80433
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
      "author_id": 665,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:17.500Z",
      "status": "published",
      "subject_id": 220,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 667,
      "reply_to_id": 24,
      "created_at": "2016-10-26T18:01:17.584Z",
      "status": "published",
      "subject_id": 221,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 669,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:17.668Z",
      "status": "published",
      "subject_id": 222,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 671,
      "reply_to_id": 26,
      "created_at": "2016-10-26T18:01:17.752Z",
      "status": "published",
      "subject_id": 223,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 673,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:17.838Z",
      "status": "reported",
      "subject_id": 224,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 29,
      "author_id": 675,
      "reply_to_id": 28,
      "created_at": "2016-10-26T18:01:17.922Z",
      "status": "published",
      "subject_id": 225,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 677,
      "reply_to_id": 28,
      "created_at": "2016-10-26T18:01:18.006Z",
      "status": "published",
      "subject_id": 226,
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
	-H "Authorization: Bearer e10a0e8d7e9e3429a79c6d6a345fce21757ee26a17e8e6e415a564576be80433"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer cfb4f4c8dac91b80dd602fd2dc2f356dcd9a30f2309bdb4f6cc377d226a008a7
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
      "id": 31,
      "author_id": 680,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:18.145Z",
      "status": "published",
      "subject_id": 227,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 682,
      "reply_to_id": 31,
      "created_at": "2016-10-26T18:01:18.293Z",
      "status": "published",
      "subject_id": 228,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 684,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:18.379Z",
      "status": "published",
      "subject_id": 229,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 686,
      "reply_to_id": 33,
      "created_at": "2016-10-26T18:01:18.490Z",
      "status": "published",
      "subject_id": 230,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 688,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:18.572Z",
      "status": "reported",
      "subject_id": 231,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 690,
      "reply_to_id": 35,
      "created_at": "2016-10-26T18:01:18.655Z",
      "status": "published",
      "subject_id": 232,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 692,
      "reply_to_id": 35,
      "created_at": "2016-10-26T18:01:18.738Z",
      "status": "published",
      "subject_id": 233,
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
	-H "Authorization: Bearer cfb4f4c8dac91b80dd602fd2dc2f356dcd9a30f2309bdb4f6cc377d226a008a7"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 5d891c98ca539a5ed2b1da1ff28a9d268ce0bb07aef5b8ffe976df07d8f07353
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
      "id": 39,
      "author_id": 697,
      "reply_to_id": 38,
      "created_at": "2016-10-26T18:01:18.963Z",
      "status": "published",
      "subject_id": 235,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 701,
      "reply_to_id": 40,
      "created_at": "2016-10-26T18:01:19.126Z",
      "status": "published",
      "subject_id": 237,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 43,
      "author_id": 705,
      "reply_to_id": 42,
      "created_at": "2016-10-26T18:01:19.290Z",
      "status": "published",
      "subject_id": 239,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 44,
      "author_id": 707,
      "reply_to_id": 42,
      "created_at": "2016-10-26T18:01:19.372Z",
      "status": "published",
      "subject_id": 240,
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
	-H "Authorization: Bearer 5d891c98ca539a5ed2b1da1ff28a9d268ce0bb07aef5b8ffe976df07d8f07353"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 160c1e083e2bbdd09ea99e49bcb4f06fb94d8a3fcdd4174a44fc43261d5eda56
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
      "id": 21,
      "author_id": 658,
      "reply_to_id": null,
      "created_at": "2016-10-26T18:01:17.215Z",
      "status": "reported",
      "subject_id": 217,
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
	-H "Authorization: Bearer 160c1e083e2bbdd09ea99e49bcb4f06fb94d8a3fcdd4174a44fc43261d5eda56"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/53/republish
Content-Type: application/json
Authorization: Bearer 1c19062f8265244fa89843911d8fada48cf29c1b40a772729d874e7e94157de5
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/53/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1c19062f8265244fa89843911d8fada48cf29c1b40a772729d874e7e94157de5"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/59/chapters
Content-Type: application/json
Authorization: Bearer 673478ca6282992d1aa577c2262fad4096bbdd35f4401d207023d293e1759ac3
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
    "id": 48,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T18:00:35.663Z",
    "course_id": 59,
    "author_id": 217,
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
curl "api.goskive.com/v2/courses/59/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 673478ca6282992d1aa577c2262fad4096bbdd35f4401d207023d293e1759ac3"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ebcd0fa18f2116280a7235eb833115b81c932d5de5e513d637ecf39453045174
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
    "id": 49,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-26T18:00:35.797Z",
    "course_id": 60,
    "author_id": 219,
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
	-H "Authorization: Bearer ebcd0fa18f2116280a7235eb833115b81c932d5de5e513d637ecf39453045174"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e2ae49b54752273faf97598c127bf80c34217d93952a55d1e9032f37d424fd3f
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
      "title": "Clever Chapter Title 48",
      "position": 1,
      "updated_at": "2016-10-26T18:00:37.174Z",
      "course_id": 68,
      "author_id": 243,
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
      "id": 61,
      "title": "Clever Chapter Title 49",
      "position": 2,
      "updated_at": "2016-10-26T18:00:37.202Z",
      "course_id": 68,
      "author_id": 244,
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
      "id": 62,
      "title": "Clever Chapter Title 50",
      "position": 3,
      "updated_at": "2016-10-26T18:00:37.525Z",
      "course_id": 68,
      "author_id": 245,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-26T18:00:37.097Z",
      "questions_updated_at": "2016-10-26T18:00:37.097Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e2ae49b54752273faf97598c127bf80c34217d93952a55d1e9032f37d424fd3f"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer e9f86bc6a77a06bc10f881fd6aaa1efb250b88e1ea3f2479d2e609237104a40e
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
      "title": "Clever Chapter Title 51",
      "position": 1,
      "updated_at": "2016-10-26T18:00:37.677Z",
      "course_id": 69,
      "author_id": 250,
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
      "id": 64,
      "title": "Clever Chapter Title 52",
      "position": 2,
      "updated_at": "2016-10-26T18:00:37.705Z",
      "course_id": 69,
      "author_id": 251,
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
      "id": 65,
      "title": "Clever Chapter Title 53",
      "position": 3,
      "updated_at": "2016-10-26T18:00:37.733Z",
      "course_id": 69,
      "author_id": 252,
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
	-H "Authorization: Bearer e9f86bc6a77a06bc10f881fd6aaa1efb250b88e1ea3f2479d2e609237104a40e"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/18
Content-Type: application/json
Authorization: Bearer 6dd129d3263853f57bcfb7708ee1c7921ca34ac5c06852b53b18da730ce8bb0f
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6dd129d3263853f57bcfb7708ee1c7921ca34ac5c06852b53b18da730ce8bb0f"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 29dc41aadf5a60ccbe97d7a4cd65f14da95812d3cb5cbb932f32174f6f4bcfaf
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
	-H "Authorization: Bearer 29dc41aadf5a60ccbe97d7a4cd65f14da95812d3cb5cbb932f32174f6f4bcfaf"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer a9545ac81cc7d1131505c648795dabe72b11769f6c4a57b7e928a1d47e36177d
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
    "creator_id": 58,
    "id": 16,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 16,
    "additional_university_ids": [

    ],
    "topic_id": 16,
    "discipline_id": 16,
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
    "chapters_updated_at": "2016-10-26T18:00:19.319Z",
    "updated_at": "2016-10-26T18:00:20.746Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 13,
        "title": "Clever Chapter Title 13",
        "position": 1,
        "updated_at": "2016-10-26T18:00:20.701Z",
        "course_id": 16,
        "author_id": 58,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T18:00:19.319Z",
        "questions_updated_at": "2016-10-26T18:00:19.319Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 14,
        "title": "Clever Chapter Title 14",
        "position": 2,
        "updated_at": "2016-10-26T18:00:20.738Z",
        "course_id": 16,
        "author_id": 58,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-26T18:00:19.319Z",
        "questions_updated_at": "2016-10-26T18:00:19.319Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 13,
        "obfuscated_id": "6UMEHi0zidE",
        "author_id": 58,
        "chapter_id": 13,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.547Z",
        "created_at": "2016-10-26T18:00:20.547Z",
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
        "author_id": 58,
        "chapter_id": 14,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.615Z",
        "created_at": "2016-10-26T18:00:20.615Z",
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
        "author_id": 58,
        "chapter_id": 13,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.586Z",
        "created_at": "2016-10-26T18:00:20.586Z",
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
        "id": 16,
        "obfuscated_id": "Drq0t9y67cE",
        "author_id": 58,
        "chapter_id": 14,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.655Z",
        "created_at": "2016-10-26T18:00:20.655Z",
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
        "id": 17,
        "obfuscated_id": "s3oqsdqLejU",
        "author_id": 61,
        "chapter_id": 13,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.691Z",
        "created_at": "2016-10-26T18:00:20.691Z",
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
        "id": 18,
        "obfuscated_id": "9KZ-wsvd6MY",
        "author_id": 62,
        "chapter_id": 14,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-26T18:00:20.728Z",
        "created_at": "2016-10-26T18:00:20.728Z",
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
	-H "Authorization: Bearer a9545ac81cc7d1131505c648795dabe72b11769f6c4a57b7e928a1d47e36177d"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/9
Content-Type: application/json
Authorization: Bearer de10501584345a9bd17eb432d55dc58ad88aa786cdeb701253d10d909caf339b
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
    "creator_id": 37,
    "id": 9,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 9,
    "additional_university_ids": [

    ],
    "topic_id": 9,
    "discipline_id": 9,
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
    "updated_at": "2016-10-26T18:00:15.771Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/9" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer de10501584345a9bd17eb432d55dc58ad88aa786cdeb701253d10d909caf339b"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 47b2ab359a214998d46a5b7d6f9de1ee2e87db85222cccbd20ec692465aae326
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
    "creator_id": 40,
    "id": 11,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 11,
    "additional_university_ids": [

    ],
    "topic_id": 11,
    "discipline_id": 11,
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
    "updated_at": "2016-10-26T18:00:16.068Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 47b2ab359a214998d46a5b7d6f9de1ee2e87db85222cccbd20ec692465aae326"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer 5b12a000684fef8d39310fc18324bda50047eb0b6e1e1d759ed24038e8a9f166
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
      "user_id": 846,
      "feedbackable_id": 121,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:01:30.388Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 25,
      "user_id": 850,
      "feedbackable_id": 122,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:01:30.687Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 26,
      "user_id": 854,
      "feedbackable_id": 123,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:01:30.983Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 27,
      "user_id": 858,
      "feedbackable_id": 124,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:01:31.278Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 28,
      "user_id": 862,
      "feedbackable_id": 125,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T18:01:31.568Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5b12a000684fef8d39310fc18324bda50047eb0b6e1e1d759ed24038e8a9f166"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 4dd522336d5ecd751c5642819c17b920cd81804abbf07971204eb3875a01d447
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
      "user_id": 841,
      "feedbackable_id": 120,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-26T18:01:30.063Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4dd522336d5ecd751c5642819c17b920cd81804abbf07971204eb3875a01d447"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/11
Content-Type: application/json
Authorization: Bearer dde030ddf9bb38c34d3a92d9eed6b3976f1b0a49f9f55c98b1103122ce6ab9cd
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/11" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dde030ddf9bb38c34d3a92d9eed6b3976f1b0a49f9f55c98b1103122ce6ab9cd"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/6/metadata
Content-Type: application/json
Authorization: Bearer 63d345809e269b66eaea9af53701c715edd796316eb44ee5edb3415ea6be366f
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
    "id": 6,
    "uploader": {
      "id": 312,
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
      "created_at": "2016-10-26T18:00:42.499Z",
      "updated_at": "2016-10-26T18:00:42.499Z"
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
    "created_at": "2016-10-26T18:00:42.573Z",
    "updated_at": "2016-10-26T18:00:42.573Z",
    "course_id": 84,
    "filename": "Pastry Making Notes.pdf",
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
| file[status] | Status |
| file[download_count] | Download count |
| file[created_at] | Created at |
| file[updated_at] | Updated at |
| file[course_id] | Course ID |
| file[category] | Category |
| file[is_anonymous] | Anonymous |


```shell
curl "api.goskive.com/v2/files/6/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 63d345809e269b66eaea9af53701c715edd796316eb44ee5edb3415ea6be366f"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/42/feedbacks
Content-Type: application/json
Authorization: Bearer 836430dbd38ce0ec3e8454cecb377f10696222fad1902b62cc019153e478fda9
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
      "user_id": 349,
      "feedbackable_id": 42,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:44.269Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 13,
      "user_id": 348,
      "feedbackable_id": 42,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:44.258Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/42/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 836430dbd38ce0ec3e8454cecb377f10696222fad1902b62cc019153e478fda9"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 329f456b4c1cd182c9e23b7aa6f4999dd42c5a606917b1da2aa98e1be8949a6a
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
      "id": 58,
      "obfuscated_id": "_S2mxc1kfck",
      "author_id": 402,
      "chapter_id": 96,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.284Z",
      "created_at": "2016-10-26T18:00:50.284Z",
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
      "chapter_id": 97,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.432Z",
      "created_at": "2016-10-26T18:00:50.432Z",
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
      "chapter_id": 98,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.574Z",
      "created_at": "2016-10-26T18:00:50.574Z",
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
      "id": 61,
      "obfuscated_id": "Acd5zhQoy8g",
      "author_id": 411,
      "chapter_id": 99,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.716Z",
      "created_at": "2016-10-26T18:00:50.716Z",
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
      "id": 62,
      "obfuscated_id": "fj_KMGohXD4",
      "author_id": 414,
      "chapter_id": 100,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.858Z",
      "created_at": "2016-10-26T18:00:50.858Z",
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
	-H "Authorization: Bearer 329f456b4c1cd182c9e23b7aa6f4999dd42c5a606917b1da2aa98e1be8949a6a"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 175468fe9416b20d9d8d464c097d2dc977645e43a9f3eef1501ec1526e4c60e7
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
      "id": 57,
      "obfuscated_id": "mCV2FECTNQs",
      "author_id": 398,
      "chapter_id": 95,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:00:50.033Z",
      "created_at": "2016-10-26T18:00:50.033Z",
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
	-H "Authorization: Bearer 175468fe9416b20d9d8d464c097d2dc977645e43a9f3eef1501ec1526e4c60e7"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/68/republish
Content-Type: application/json
Authorization: Bearer b1cc7c3a3e591506639c68e738c7ea09e16580d2e30f374218389fdab47c150d
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/68/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b1cc7c3a3e591506639c68e738c7ea09e16580d2e30f374218389fdab47c150d"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/3/feedbacks
Content-Type: application/json
Authorization: Bearer cf9cbc0b9032cb5277b036c3cffb8b54512b3d66c2c68080d3d76cdbba732e1d
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
      "user_id": 11,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:13.967Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 3,
      "user_id": 10,
      "feedbackable_id": 3,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-26T18:00:13.957Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/3/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cf9cbc0b9032cb5277b036c3cffb8b54512b3d66c2c68080d3d76cdbba732e1d"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 50c02c131485bb85234be4a64ccf01c4bb96ed174310e55c9763b474454b87ae
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
      "id": 101,
      "obfuscated_id": "PprZyBVq_gc",
      "author_id": 626,
      "chapter_id": 151,
      "position": 90,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:14.763Z",
      "created_at": "2016-10-26T18:01:14.646Z",
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
          "id": 205,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 206,
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
      "author_id": 629,
      "chapter_id": 152,
      "position": 91,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:15.038Z",
      "created_at": "2016-10-26T18:01:14.921Z",
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
          "id": 207,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 208,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 103,
      "obfuscated_id": "AVhVflMAvL0",
      "author_id": 632,
      "chapter_id": 153,
      "position": 92,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:15.309Z",
      "created_at": "2016-10-26T18:01:15.197Z",
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
          "id": 209,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 210,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 99,
      "obfuscated_id": "5fPQ9k37GTc",
      "author_id": 620,
      "chapter_id": 149,
      "position": 88,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:14.200Z",
      "created_at": "2016-10-26T18:01:14.075Z",
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
          "id": 201,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 202,
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
      "author_id": 623,
      "chapter_id": 150,
      "position": 89,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:14.478Z",
      "created_at": "2016-10-26T18:01:14.360Z",
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
          "id": 203,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 204,
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
	-H "Authorization: Bearer 50c02c131485bb85234be4a64ccf01c4bb96ed174310e55c9763b474454b87ae"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 8acaf4f7a97f11b56c33dbe9d51bb3e6e04d6230ac404443489c31b24e58eb8b
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
      "id": 93,
      "obfuscated_id": "4z_mapEg68k",
      "author_id": 600,
      "chapter_id": 143,
      "position": 82,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-26T18:01:11.848Z",
      "created_at": "2016-10-26T18:01:11.673Z",
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
          "id": 189,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 190,
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
	-H "Authorization: Bearer 8acaf4f7a97f11b56c33dbe9d51bb3e6e04d6230ac404443489c31b24e58eb8b"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/84/republish
Content-Type: application/json
Authorization: Bearer 571427c2bf07e10f7cee82add3470d56c7c9c0526e23645937a5ca18a4de7463
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/84/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 571427c2bf07e10f7cee82add3470d56c7c9c0526e23645937a5ca18a4de7463"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 886faa98b064227e6f734ffbfacaddc397cb2849d8b2a76ab4b265e9e6cf54bc
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":196,"published":false}}
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
    "creator_id": 556,
    "id": 184,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 164,
    "additional_university_ids": [

    ],
    "topic_id": 196,
    "discipline_id": 197,
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
    "updated_at": "2016-10-26T18:01:05.707Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":196,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 886faa98b064227e6f734ffbfacaddc397cb2849d8b2a76ab4b265e9e6cf54bc"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 40a9afdaefc66e3561df78074011eeefb67bf2557cb36876d368e247501f130a
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
      "creator_id": 523,
      "id": 154,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-105",
      "html_url": "https://goskive.com/course/fu-course-105",
      "slug": "fu-course-105",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 166,
      "discipline_id": 167,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 105",
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
      "updated_at": "2016-10-26T18:01:02.263Z",
      "shortname": "fu-course-105"
    },
    {
      "creator_id": 523,
      "id": 155,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-106",
      "html_url": "https://goskive.com/course/fu-course-106",
      "slug": "fu-course-106",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 167,
      "discipline_id": 168,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 106",
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
      "updated_at": "2016-10-26T18:01:02.304Z",
      "shortname": "fu-course-106"
    },
    {
      "creator_id": 524,
      "id": 156,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-107",
      "html_url": "https://goskive.com/course/fu-course-107",
      "slug": "fu-course-107",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 168,
      "discipline_id": 169,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-26T18:01:02.353Z",
      "shortname": "fu-course-107"
    },
    {
      "creator_id": 524,
      "id": 157,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-108",
      "html_url": "https://goskive.com/course/fu-course-108",
      "slug": "fu-course-108",
      "university_id": 151,
      "additional_university_ids": [

      ],
      "topic_id": 169,
      "discipline_id": 170,
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
      "chapters_updated_at": "2016-10-26T18:01:02.716Z",
      "updated_at": "2016-10-26T18:01:02.725Z",
      "shortname": "fu-course-108"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 40a9afdaefc66e3561df78074011eeefb67bf2557cb36876d368e247501f130a"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer f9caee2c89217a64e8f957365990d28f7f77a2016202e8555af259fa6bc73c1c
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
      "creator_id": 530,
      "id": 158,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-109",
      "html_url": "https://goskive.com/course/fu-course-109",
      "slug": "fu-course-109",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 170,
      "discipline_id": 171,
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
      "published": false,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-26T18:01:02.927Z",
      "shortname": "fu-course-109"
    },
    {
      "creator_id": 530,
      "id": 159,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-110",
      "html_url": "https://goskive.com/course/fu-course-110",
      "slug": "fu-course-110",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 171,
      "discipline_id": 172,
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
      "updated_at": "2016-10-26T18:01:02.968Z",
      "shortname": "fu-course-110"
    },
    {
      "creator_id": 531,
      "id": 160,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-111",
      "html_url": "https://goskive.com/course/fu-course-111",
      "slug": "fu-course-111",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 172,
      "discipline_id": 173,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-26T18:01:03.017Z",
      "shortname": "fu-course-111"
    },
    {
      "creator_id": 531,
      "id": 161,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-112",
      "html_url": "https://goskive.com/course/fu-course-112",
      "slug": "fu-course-112",
      "university_id": 153,
      "additional_university_ids": [

      ],
      "topic_id": 173,
      "discipline_id": 174,
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
      "published": true,
      "official": false,
      "has_training": true,
      "has_exam": true,
      "has_flashcards": false,
      "has_challenge_mode": true,
      "campaign_ids": [

      ],
      "chapters_updated_at": null,
      "updated_at": "2016-10-26T18:01:03.058Z",
      "shortname": "fu-course-112"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f9caee2c89217a64e8f957365990d28f7f77a2016202e8555af259fa6bc73c1c"
```
