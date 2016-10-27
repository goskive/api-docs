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
DELETE /v2/chapters/71
Content-Type: application/json
Authorization: Bearer 184ebeee647bd219c0320fcb870ccf96d5e11770a9b0039666787b0944860b87
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/71" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 184ebeee647bd219c0320fcb870ccf96d5e11770a9b0039666787b0944860b87"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/78
Content-Type: application/json
Authorization: Bearer 77cb106b66edc619fb65bbb30e7284fb3fbdb683e70fa7fb4e7eb0f0ba6cc974
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
    "updated_at": "2016-10-27T17:43:27.468Z",
    "course_id": 133,
    "author_id": 413,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-10-27T17:43:26.940Z",
    "questions_updated_at": "2016-10-27T17:43:26.940Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 41,
        "obfuscated_id": "11qbskrctUU",
        "author_id": 416,
        "chapter_id": 78,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:27.413Z",
        "created_at": "2016-10-27T17:43:27.413Z",
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
        "author_id": 417,
        "chapter_id": 78,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:27.451Z",
        "created_at": "2016-10-27T17:43:27.451Z",
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
        "id": 60,
        "obfuscated_id": "XsZtONYAiuo",
        "author_id": 414,
        "chapter_id": 78,
        "position": 56,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:27.154Z",
        "created_at": "2016-10-27T17:43:27.048Z",
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
        "id": 61,
        "obfuscated_id": "Acd5zhQoy8g",
        "author_id": 415,
        "chapter_id": 78,
        "position": 57,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:27.343Z",
        "created_at": "2016-10-27T17:43:27.226Z",
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
      }
    ]
  }
}
```



```shell
curl "api.goskive.com/v2/chapters/78" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 77cb106b66edc619fb65bbb30e7284fb3fbdb683e70fa7fb4e7eb0f0ba6cc974"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/75
Content-Type: application/json
Authorization: Bearer 9295500ed3921b8f80572d08163102e424f400a138cd86dc446b5d766aa28774
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
    "id": 75,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-10-27T17:43:26.186Z",
    "course_id": 130,
    "author_id": 400,
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
curl "api.goskive.com/v2/chapters/75" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9295500ed3921b8f80572d08163102e424f400a138cd86dc446b5d766aa28774"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/1
Content-Type: application/json
Authorization: Bearer 5ca33a0b64d4a378afe595f6cf0854132dacb2cc407a6b1389788e26057d2d3a
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/1" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5ca33a0b64d4a378afe595f6cf0854132dacb2cc407a6b1389788e26057d2d3a"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 42fdd479667b5afe6a0092554f8e27f6805c73409d1e3ee4fbff817630a41273
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
      "id": 21,
      "author_id": 88,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:00.866Z",
      "status": "published",
      "subject_id": 28,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 22,
      "author_id": 90,
      "reply_to_id": 21,
      "created_at": "2016-10-27T17:43:00.945Z",
      "status": "published",
      "subject_id": 29,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 92,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:01.024Z",
      "status": "published",
      "subject_id": 30,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 94,
      "reply_to_id": 23,
      "created_at": "2016-10-27T17:43:01.102Z",
      "status": "published",
      "subject_id": 31,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 96,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:01.182Z",
      "status": "reported",
      "subject_id": 32,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 98,
      "reply_to_id": 25,
      "created_at": "2016-10-27T17:43:01.261Z",
      "status": "published",
      "subject_id": 33,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 100,
      "reply_to_id": 25,
      "created_at": "2016-10-27T17:43:01.340Z",
      "status": "published",
      "subject_id": 34,
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
	-H "Authorization: Bearer 42fdd479667b5afe6a0092554f8e27f6805c73409d1e3ee4fbff817630a41273"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer a0fa02c8ef4f1168bf5370e0fe4a58d5df960e3d9b468985c872c62207651dac
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
      "id": 35,
      "author_id": 118,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:02.079Z",
      "status": "published",
      "subject_id": 42,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 36,
      "author_id": 120,
      "reply_to_id": 35,
      "created_at": "2016-10-27T17:43:02.158Z",
      "status": "published",
      "subject_id": 43,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 37,
      "author_id": 122,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:02.239Z",
      "status": "published",
      "subject_id": 44,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 38,
      "author_id": 124,
      "reply_to_id": 37,
      "created_at": "2016-10-27T17:43:02.319Z",
      "status": "published",
      "subject_id": 45,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 39,
      "author_id": 126,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:02.400Z",
      "status": "reported",
      "subject_id": 46,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 40,
      "author_id": 128,
      "reply_to_id": 39,
      "created_at": "2016-10-27T17:43:02.484Z",
      "status": "published",
      "subject_id": 47,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 41,
      "author_id": 130,
      "reply_to_id": 39,
      "created_at": "2016-10-27T17:43:02.564Z",
      "status": "published",
      "subject_id": 48,
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
	-H "Authorization: Bearer a0fa02c8ef4f1168bf5370e0fe4a58d5df960e3d9b468985c872c62207651dac"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 661129b0cea555918acb40e59f1114a9d52ecf03ed3300f8683a4635cebf1977
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
      "id": 15,
      "author_id": 75,
      "reply_to_id": 14,
      "created_at": "2016-10-27T17:43:00.346Z",
      "status": "published",
      "subject_id": 22,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 79,
      "reply_to_id": 16,
      "created_at": "2016-10-27T17:43:00.502Z",
      "status": "published",
      "subject_id": 24,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 83,
      "reply_to_id": 18,
      "created_at": "2016-10-27T17:43:00.661Z",
      "status": "published",
      "subject_id": 26,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 85,
      "reply_to_id": 18,
      "created_at": "2016-10-27T17:43:00.741Z",
      "status": "published",
      "subject_id": 27,
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
	-H "Authorization: Bearer 661129b0cea555918acb40e59f1114a9d52ecf03ed3300f8683a4635cebf1977"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 31cd7ca541e0a5c6189d8f23f5dae01ac40d2a7d48109db32c65d29ebb71cb73
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
      "id": 32,
      "author_id": 111,
      "reply_to_id": null,
      "created_at": "2016-10-27T17:43:01.794Z",
      "status": "reported",
      "subject_id": 39,
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
	-H "Authorization: Bearer 31cd7ca541e0a5c6189d8f23f5dae01ac40d2a7d48109db32c65d29ebb71cb73"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/5/republish
Content-Type: application/json
Authorization: Bearer 1a9a2df5bbd16bff9d1068d4cadaf2bedb86e656ec437cb8671e12fc795c67a4
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/5/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 1a9a2df5bbd16bff9d1068d4cadaf2bedb86e656ec437cb8671e12fc795c67a4"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 681000815177e4cdcee4616a1312a25d17fbc74204186e0e202f4841dfb7e874
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
    "id": 35,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-27T17:43:06.906Z",
    "course_id": 66,
    "author_id": 200,
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
	-H "Authorization: Bearer 681000815177e4cdcee4616a1312a25d17fbc74204186e0e202f4841dfb7e874"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/69/chapters
Content-Type: application/json
Authorization: Bearer 0ac739ca58307499ed7e275e65b22166c8d434fe92fcb614a3611beb743803e2
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
    "id": 37,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-10-27T17:43:07.283Z",
    "course_id": 69,
    "author_id": 206,
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
curl "api.goskive.com/v2/courses/69/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0ac739ca58307499ed7e275e65b22166c8d434fe92fcb614a3611beb743803e2"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer ecf1e020902a9eb7222172ad64a1813955c57dfcb79ae8ef7a53864ce8eb1ff3
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
      "id": 17,
      "title": "Clever Chapter Title 8",
      "position": 1,
      "updated_at": "2016-10-27T17:43:04.829Z",
      "course_id": 57,
      "author_id": 161,
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
      "title": "Clever Chapter Title 9",
      "position": 2,
      "updated_at": "2016-10-27T17:43:04.852Z",
      "course_id": 57,
      "author_id": 162,
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
      "id": 19,
      "title": "Clever Chapter Title 10",
      "position": 3,
      "updated_at": "2016-10-27T17:43:05.103Z",
      "course_id": 57,
      "author_id": 163,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-10-27T17:43:04.757Z",
      "questions_updated_at": "2016-10-27T17:43:04.757Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ecf1e020902a9eb7222172ad64a1813955c57dfcb79ae8ef7a53864ce8eb1ff3"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 609b9343d6d7661817452d800df8e218b616591289af6f8fd640449f5e55f1bd
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
      "id": 20,
      "title": "Clever Chapter Title 11",
      "position": 1,
      "updated_at": "2016-10-27T17:43:05.244Z",
      "course_id": 58,
      "author_id": 168,
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
      "id": 21,
      "title": "Clever Chapter Title 12",
      "position": 2,
      "updated_at": "2016-10-27T17:43:05.267Z",
      "course_id": 58,
      "author_id": 169,
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
      "id": 22,
      "title": "Clever Chapter Title 13",
      "position": 3,
      "updated_at": "2016-10-27T17:43:05.290Z",
      "course_id": 58,
      "author_id": 170,
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
	-H "Authorization: Bearer 609b9343d6d7661817452d800df8e218b616591289af6f8fd640449f5e55f1bd"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/88
Content-Type: application/json
Authorization: Bearer a0a5d8945994f64e1e54c63ae876a5e8aae15a35579ed9b222b67ad23ea2f188
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/88" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer a0a5d8945994f64e1e54c63ae876a5e8aae15a35579ed9b222b67ad23ea2f188"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 462cf829730b0eebd216eebfdf5bb72466c63afae6f05366162c2c46f58a7749
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
	-H "Authorization: Bearer 462cf829730b0eebd216eebfdf5bb72466c63afae6f05366162c2c46f58a7749"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer e5a9fca98cc6964f05407c2e6e4317dd42724054bc9647c9c20e6376757613b4
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
    "creator_id": 315,
    "id": 104,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 104,
    "additional_university_ids": [

    ],
    "topic_id": 114,
    "discipline_id": 115,
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
    "chapters_updated_at": "2016-10-27T17:43:18.632Z",
    "updated_at": "2016-10-27T17:43:20.008Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 63,
        "title": "Clever Chapter Title 51",
        "position": 1,
        "updated_at": "2016-10-27T17:43:19.961Z",
        "course_id": 104,
        "author_id": 315,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-27T17:43:18.632Z",
        "questions_updated_at": "2016-10-27T17:43:18.632Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 64,
        "title": "Clever Chapter Title 52",
        "position": 2,
        "updated_at": "2016-10-27T17:43:20.000Z",
        "course_id": 104,
        "author_id": 315,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-10-27T17:43:18.632Z",
        "questions_updated_at": "2016-10-27T17:43:18.632Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 33,
        "obfuscated_id": "sjAD-GXxS8o",
        "author_id": 315,
        "chapter_id": 63,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.801Z",
        "created_at": "2016-10-27T17:43:19.801Z",
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
        "author_id": 315,
        "chapter_id": 64,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.872Z",
        "created_at": "2016-10-27T17:43:19.872Z",
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
        "id": 34,
        "obfuscated_id": "LRSQf_NrQzE",
        "author_id": 315,
        "chapter_id": 63,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.842Z",
        "created_at": "2016-10-27T17:43:19.842Z",
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
        "id": 36,
        "obfuscated_id": "01Tx8eTrCOA",
        "author_id": 315,
        "chapter_id": 64,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.913Z",
        "created_at": "2016-10-27T17:43:19.913Z",
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
        "id": 37,
        "obfuscated_id": "95m_4XdR9PU",
        "author_id": 318,
        "chapter_id": 63,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.952Z",
        "created_at": "2016-10-27T17:43:19.952Z",
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
        "id": 38,
        "obfuscated_id": "8_YCqPYFnsI",
        "author_id": 319,
        "chapter_id": 64,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-10-27T17:43:19.991Z",
        "created_at": "2016-10-27T17:43:19.991Z",
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
	-H "Authorization: Bearer e5a9fca98cc6964f05407c2e6e4317dd42724054bc9647c9c20e6376757613b4"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/97
Content-Type: application/json
Authorization: Bearer cfd4b1e9ac7672d9feb21222939f9d414f5e358eaf25903a06c80f6ff81c7789
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
    "creator_id": 291,
    "id": 97,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 97,
    "additional_university_ids": [

    ],
    "topic_id": 107,
    "discipline_id": 108,
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
    "updated_at": "2016-10-27T17:43:13.819Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/97" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer cfd4b1e9ac7672d9feb21222939f9d414f5e358eaf25903a06c80f6ff81c7789"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer c1232062ba5141282c8095f6d431cb686718a5e70ad47408427df6f8efc6116f
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
    "creator_id": 293,
    "id": 98,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 98,
    "additional_university_ids": [

    ],
    "topic_id": 108,
    "discipline_id": 109,
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
    "updated_at": "2016-10-27T17:43:13.958Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c1232062ba5141282c8095f6d431cb686718a5e70ad47408427df6f8efc6116f"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer f7215563e40283a0e46d5788519a489ebf8ce6397800c0944cdbafb250bda7c7
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
      "id": 38,
      "user_id": 946,
      "feedbackable_id": 130,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:09.348Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 39,
      "user_id": 950,
      "feedbackable_id": 131,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:09.646Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 40,
      "user_id": 954,
      "feedbackable_id": 132,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:09.940Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 958,
      "feedbackable_id": 133,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:10.234Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 962,
      "feedbackable_id": 134,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-27T17:44:10.532Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f7215563e40283a0e46d5788519a489ebf8ce6397800c0944cdbafb250bda7c7"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer bf028ba0cd10b567d3e710d191584d8ec1b5f133d8c9584452cc09c3514fca8a
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
      "id": 28,
      "user_id": 904,
      "feedbackable_id": 120,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-10-27T17:44:06.202Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bf028ba0cd10b567d3e710d191584d8ec1b5f133d8c9584452cc09c3514fca8a"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/19
Content-Type: application/json
Authorization: Bearer 68cccb2c75314d473f0b0302113581578dacb8feeb5bcc660206bf3535e59f72
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/19" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 68cccb2c75314d473f0b0302113581578dacb8feeb5bcc660206bf3535e59f72"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer ede71e33f74cdb40ac476c450c57c4781f5eb773ec06add9cbb662d83d772d9a
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
    "id": 13,
    "uploader": {
      "id": 796,
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
      "created_at": "2016-10-27T17:44:00.550Z",
      "updated_at": "2016-10-27T17:44:00.550Z"
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
    "created_at": "2016-10-27T17:44:00.625Z",
    "updated_at": "2016-10-27T17:44:00.625Z",
    "course_id": 270,
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
curl "api.goskive.com/v2/files/13/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ede71e33f74cdb40ac476c450c57c4781f5eb773ec06add9cbb662d83d772d9a"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/86/feedbacks
Content-Type: application/json
Authorization: Bearer 911f026c7564c5df8ae76412a1593d36c02f8aef537208d317b43bdd7b077145
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
      "id": 18,
      "user_id": 857,
      "feedbackable_id": 86,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:03.421Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 856,
      "feedbackable_id": 86,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:44:03.410Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/86/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 911f026c7564c5df8ae76412a1593d36c02f8aef537208d317b43bdd7b077145"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer ad0e797dae4b2a63f65d3b196e284ff27a99fbb66cbb554a47cb9d43bc2150a8
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
      "author_id": 507,
      "chapter_id": 106,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:36.294Z",
      "created_at": "2016-10-27T17:43:36.294Z",
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
      "author_id": 510,
      "chapter_id": 107,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:36.423Z",
      "created_at": "2016-10-27T17:43:36.423Z",
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
      "author_id": 513,
      "chapter_id": 108,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:36.555Z",
      "created_at": "2016-10-27T17:43:36.555Z",
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
      "author_id": 516,
      "chapter_id": 109,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:36.688Z",
      "created_at": "2016-10-27T17:43:36.688Z",
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
      "author_id": 519,
      "chapter_id": 110,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:36.823Z",
      "created_at": "2016-10-27T17:43:36.823Z",
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
	-H "Authorization: Bearer ad0e797dae4b2a63f65d3b196e284ff27a99fbb66cbb554a47cb9d43bc2150a8"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer d7e3da5af1623e3f44258685c0787eb47a885e82a391246f5efaf612c8b31c27
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
      "id": 59,
      "obfuscated_id": "fo0taK4dosk",
      "author_id": 551,
      "chapter_id": 120,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:38.317Z",
      "created_at": "2016-10-27T17:43:38.317Z",
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
	-H "Authorization: Bearer d7e3da5af1623e3f44258685c0787eb47a885e82a391246f5efaf612c8b31c27"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/63/republish
Content-Type: application/json
Authorization: Bearer 79199ea7c1bbcc831d7194d4ad7d2e190b08ec202d9ef67ad545c188d53641dd
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
	-H "Authorization: Bearer 79199ea7c1bbcc831d7194d4ad7d2e190b08ec202d9ef67ad545c188d53641dd"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/91/feedbacks
Content-Type: application/json
Authorization: Bearer 6b0014dae37bedb078d5dd98385f4e8b0cd082acbda135d2c284b627841db7d0
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
      "user_id": 595,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:41.904Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 4,
      "user_id": 594,
      "feedbackable_id": 91,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-10-27T17:43:41.892Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/91/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6b0014dae37bedb078d5dd98385f4e8b0cd082acbda135d2c284b627841db7d0"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 514253e5873b2a88f7aeb815d2bd23f81c5accac43dc0a27136b0bc7224b10a6
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
      "id": 84,
      "obfuscated_id": "Hu6DTUHzhWo",
      "author_id": 490,
      "chapter_id": 101,
      "position": 72,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:35.083Z",
      "created_at": "2016-10-27T17:43:34.967Z",
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
          "id": 171,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 172,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 81,
      "obfuscated_id": "jHF1owx40fU",
      "author_id": 481,
      "chapter_id": 98,
      "position": 69,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:34.259Z",
      "created_at": "2016-10-27T17:43:34.144Z",
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
          "id": 165,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 166,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 82,
      "obfuscated_id": "D5TJ6kac5FE",
      "author_id": 484,
      "chapter_id": 99,
      "position": 70,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:34.533Z",
      "created_at": "2016-10-27T17:43:34.418Z",
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
          "id": 167,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 168,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 83,
      "obfuscated_id": "FCSR-nKROLo",
      "author_id": 487,
      "chapter_id": 100,
      "position": 71,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:34.809Z",
      "created_at": "2016-10-27T17:43:34.694Z",
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
          "id": 169,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 170,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 85,
      "obfuscated_id": "xR5KgQjIo2Y",
      "author_id": 493,
      "chapter_id": 102,
      "position": 73,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:35.352Z",
      "created_at": "2016-10-27T17:43:35.244Z",
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
          "id": 173,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 174,
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
	-H "Authorization: Bearer 514253e5873b2a88f7aeb815d2bd23f81c5accac43dc0a27136b0bc7224b10a6"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer c27911491a87973c8d5fb80751bbb0fe8ab92b175806cfb55efabe449f2fa065
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
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 461,
      "chapter_id": 92,
      "position": 63,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-10-27T17:43:32.475Z",
      "created_at": "2016-10-27T17:43:32.366Z",
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
          "id": 153,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 154,
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
	-H "Authorization: Bearer c27911491a87973c8d5fb80751bbb0fe8ab92b175806cfb55efabe449f2fa065"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/67/republish
Content-Type: application/json
Authorization: Bearer 336925531ed8f10f0f1f96c3da9ca3c41a14f230ded553e2e55699f7e5066358
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/67/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 336925531ed8f10f0f1f96c3da9ca3c41a14f230ded553e2e55699f7e5066358"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer c57058848ba003cb8ef3f8a92b8c211dd0ad990b0a54c0525108f6f36043bf52
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":263,"published":false}}
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
    "creator_id": 740,
    "id": 253,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 236,
    "additional_university_ids": [

    ],
    "topic_id": 263,
    "discipline_id": 264,
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
    "updated_at": "2016-10-27T17:43:54.159Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":263,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c57058848ba003cb8ef3f8a92b8c211dd0ad990b0a54c0525108f6f36043bf52"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 2f66cc936cf8b7507b8c84bf90c6f73479f8e8caf6be439ea7cc984e3db81e8f
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
      "creator_id": 724,
      "id": 239,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-175",
      "html_url": "https://goskive.com/course/fu-course-175",
      "slug": "fu-course-175",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 249,
      "discipline_id": 250,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 175",
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
      "updated_at": "2016-10-27T17:43:52.607Z",
      "shortname": "fu-course-175"
    },
    {
      "creator_id": 724,
      "id": 240,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-176",
      "html_url": "https://goskive.com/course/fu-course-176",
      "slug": "fu-course-176",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 250,
      "discipline_id": 251,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 176",
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
      "updated_at": "2016-10-27T17:43:52.647Z",
      "shortname": "fu-course-176"
    },
    {
      "creator_id": 725,
      "id": 241,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-177",
      "html_url": "https://goskive.com/course/fu-course-177",
      "slug": "fu-course-177",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 251,
      "discipline_id": 252,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 177",
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
      "updated_at": "2016-10-27T17:43:52.695Z",
      "shortname": "fu-course-177"
    },
    {
      "creator_id": 725,
      "id": 242,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-178",
      "html_url": "https://goskive.com/course/fu-course-178",
      "slug": "fu-course-178",
      "university_id": 229,
      "additional_university_ids": [

      ],
      "topic_id": 252,
      "discipline_id": 253,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 178",
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
      "chapters_updated_at": "2016-10-27T17:43:52.979Z",
      "updated_at": "2016-10-27T17:43:52.985Z",
      "shortname": "fu-course-178"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2f66cc936cf8b7507b8c84bf90c6f73479f8e8caf6be439ea7cc984e3db81e8f"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 3175585f554c13d9317dfcee5ea73d9dd3b2ce74bb2a8394631b20b4bd928cc1
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
      "creator_id": 731,
      "id": 243,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-179",
      "html_url": "https://goskive.com/course/fu-course-179",
      "slug": "fu-course-179",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 253,
      "discipline_id": 254,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 179",
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
      "updated_at": "2016-10-27T17:43:53.197Z",
      "shortname": "fu-course-179"
    },
    {
      "creator_id": 731,
      "id": 244,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-180",
      "html_url": "https://goskive.com/course/fu-course-180",
      "slug": "fu-course-180",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 254,
      "discipline_id": 255,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 180",
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
      "updated_at": "2016-10-27T17:43:53.237Z",
      "shortname": "fu-course-180"
    },
    {
      "creator_id": 732,
      "id": 245,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-181",
      "html_url": "https://goskive.com/course/fu-course-181",
      "slug": "fu-course-181",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 255,
      "discipline_id": 256,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 181",
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
      "updated_at": "2016-10-27T17:43:53.285Z",
      "shortname": "fu-course-181"
    },
    {
      "creator_id": 732,
      "id": 246,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-182",
      "html_url": "https://goskive.com/course/fu-course-182",
      "slug": "fu-course-182",
      "university_id": 231,
      "additional_university_ids": [

      ],
      "topic_id": 256,
      "discipline_id": 257,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 182",
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
      "updated_at": "2016-10-27T17:43:53.326Z",
      "shortname": "fu-course-182"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3175585f554c13d9317dfcee5ea73d9dd3b2ce74bb2a8394631b20b4bd928cc1"
```
