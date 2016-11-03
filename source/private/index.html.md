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
DELETE /v2/chapters/192
Content-Type: application/json
Authorization: Bearer 06260afd37cf44e281a7e719b8a1a2cfc443adc5f807fb5ff6011c801b4ae40b
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/192" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 06260afd37cf44e281a7e719b8a1a2cfc443adc5f807fb5ff6011c801b4ae40b"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/190
Content-Type: application/json
Authorization: Bearer 530c46a4aef1dccb958cc8e18eba77be26dc037eba9b7c4de27a6882ad8e5726
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
    "id": 190,
    "title": "Flour and eggs",
    "position": 1,
    "updated_at": "2016-11-03T12:34:41.006Z",
    "course_id": 311,
    "author_id": 958,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-11-03T12:34:40.476Z",
    "questions_updated_at": "2016-11-03T12:34:40.476Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 92,
        "obfuscated_id": "__OphzZQiQY",
        "author_id": 961,
        "chapter_id": 190,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:40.945Z",
        "created_at": "2016-11-03T12:34:40.945Z",
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
        "id": 93,
        "obfuscated_id": "4z_mapEg68k",
        "author_id": 962,
        "chapter_id": 190,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:40.989Z",
        "created_at": "2016-11-03T12:34:40.989Z",
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
        "id": 129,
        "obfuscated_id": "x8EyeGrWnN4",
        "author_id": 959,
        "chapter_id": 190,
        "position": 116,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:40.685Z",
        "created_at": "2016-11-03T12:34:40.581Z",
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
            "id": 261,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 262,
            "position": 2,
            "content": "MyText",
            "content_html": "MyText",
            "correct": false
          }
        ]
      },
      {
        "id": 130,
        "obfuscated_id": "N-qIf0IsvWM",
        "author_id": 960,
        "chapter_id": 190,
        "position": 117,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:40.872Z",
        "created_at": "2016-11-03T12:34:40.753Z",
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
            "id": 263,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 264,
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
curl "api.goskive.com/v2/chapters/190" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 530c46a4aef1dccb958cc8e18eba77be26dc037eba9b7c4de27a6882ad8e5726"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/188
Content-Type: application/json
Authorization: Bearer d387f951a3516cd41e4cb6634e9dc6f727e1f1eeabfb944a4e38426708bd393c
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
    "id": 188,
    "title": "Eggs and Flour",
    "position": 1,
    "updated_at": "2016-11-03T12:34:40.295Z",
    "course_id": 309,
    "author_id": 953,
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
curl "api.goskive.com/v2/chapters/188" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d387f951a3516cd41e4cb6634e9dc6f727e1f1eeabfb944a4e38426708bd393c"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/6
Content-Type: application/json
Authorization: Bearer e16377f52f460d0b56fa628113c8cb0c2ca94559b316d508fa4f26655890c6f1
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/6" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e16377f52f460d0b56fa628113c8cb0c2ca94559b316d508fa4f26655890c6f1"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 887a377e249d06d1a55ee555efb6dea2bee8cc43bcba804beb44c1b1c9856a6b
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
      "id": 7,
      "author_id": 275,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:47.937Z",
      "status": "published",
      "subject_id": 75,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 8,
      "author_id": 277,
      "reply_to_id": 7,
      "created_at": "2016-11-03T12:33:48.016Z",
      "status": "published",
      "subject_id": 76,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 9,
      "author_id": 279,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:48.094Z",
      "status": "published",
      "subject_id": 77,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 10,
      "author_id": 281,
      "reply_to_id": 9,
      "created_at": "2016-11-03T12:33:48.173Z",
      "status": "published",
      "subject_id": 78,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 11,
      "author_id": 283,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:48.253Z",
      "status": "reported",
      "subject_id": 79,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 12,
      "author_id": 285,
      "reply_to_id": 11,
      "created_at": "2016-11-03T12:33:48.336Z",
      "status": "published",
      "subject_id": 80,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 13,
      "author_id": 287,
      "reply_to_id": 11,
      "created_at": "2016-11-03T12:33:48.420Z",
      "status": "published",
      "subject_id": 81,
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
	-H "Authorization: Bearer 887a377e249d06d1a55ee555efb6dea2bee8cc43bcba804beb44c1b1c9856a6b"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer cf63bd2fc955e13d69a980067c00d24c0ba8f7a520283fef3e80e35344f3ffa5
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
      "id": 14,
      "author_id": 290,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:48.557Z",
      "status": "published",
      "subject_id": 82,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 15,
      "author_id": 292,
      "reply_to_id": 14,
      "created_at": "2016-11-03T12:33:48.640Z",
      "status": "published",
      "subject_id": 83,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 16,
      "author_id": 294,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:48.722Z",
      "status": "published",
      "subject_id": 84,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 17,
      "author_id": 296,
      "reply_to_id": 16,
      "created_at": "2016-11-03T12:33:48.800Z",
      "status": "published",
      "subject_id": 85,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 18,
      "author_id": 298,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:48.907Z",
      "status": "reported",
      "subject_id": 86,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 19,
      "author_id": 300,
      "reply_to_id": 18,
      "created_at": "2016-11-03T12:33:48.987Z",
      "status": "published",
      "subject_id": 87,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 20,
      "author_id": 302,
      "reply_to_id": 18,
      "created_at": "2016-11-03T12:33:49.066Z",
      "status": "published",
      "subject_id": 88,
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
	-H "Authorization: Bearer cf63bd2fc955e13d69a980067c00d24c0ba8f7a520283fef3e80e35344f3ffa5"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer 3c258856fcfff38481e4b001882120ce9e3981edbae1d16370448af2e3dbcbc4
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
      "id": 29,
      "author_id": 322,
      "reply_to_id": 28,
      "created_at": "2016-11-03T12:33:49.904Z",
      "status": "published",
      "subject_id": 97,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 326,
      "reply_to_id": 30,
      "created_at": "2016-11-03T12:33:50.066Z",
      "status": "published",
      "subject_id": 99,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 330,
      "reply_to_id": 32,
      "created_at": "2016-11-03T12:33:50.226Z",
      "status": "published",
      "subject_id": 101,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 332,
      "reply_to_id": 32,
      "created_at": "2016-11-03T12:33:50.306Z",
      "status": "published",
      "subject_id": 102,
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
	-H "Authorization: Bearer 3c258856fcfff38481e4b001882120ce9e3981edbae1d16370448af2e3dbcbc4"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 01ea7d8a43eedeefe9398f7345d6eb08ae86eb6dc76dc0d8bbf04a5b20547b3e
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
      "id": 39,
      "author_id": 343,
      "reply_to_id": null,
      "created_at": "2016-11-03T12:33:50.758Z",
      "status": "reported",
      "subject_id": 107,
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
	-H "Authorization: Bearer 01ea7d8a43eedeefe9398f7345d6eb08ae86eb6dc76dc0d8bbf04a5b20547b3e"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/3/republish
Content-Type: application/json
Authorization: Bearer 2bfde37b2c55e45dc9f1579be16c849a636ac25c8db2da14ae7a86428f4674b4
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/3/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 2bfde37b2c55e45dc9f1579be16c849a636ac25c8db2da14ae7a86428f4674b4"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/216/chapters
Content-Type: application/json
Authorization: Bearer 8ebed3c7fa9f33d0461475b2272caee30a17a8be5314297bde227212f59b9020
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
    "id": 149,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T12:34:21.540Z",
    "course_id": 216,
    "author_id": 731,
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
	-H "Authorization: Bearer 8ebed3c7fa9f33d0461475b2272caee30a17a8be5314297bde227212f59b9020"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 6b51f9fac4159239e65a97b8bf5b042a4fc4e1a30eb2e7e9bcfec17f283e0d5d
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
    "id": 150,
    "title": "Preparing the oven",
    "position": 1,
    "updated_at": "2016-11-03T12:34:21.663Z",
    "course_id": 217,
    "author_id": 733,
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
	-H "Authorization: Bearer 6b51f9fac4159239e65a97b8bf5b042a4fc4e1a30eb2e7e9bcfec17f283e0d5d"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 54abb9d605ae5648c3e844cbdd72e700415bf436c5bae02b72fb56b97f572f52
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
      "id": 140,
      "title": "Clever Chapter Title 140",
      "position": 1,
      "updated_at": "2016-11-03T12:34:20.498Z",
      "course_id": 211,
      "author_id": 710,
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
      "id": 141,
      "title": "Clever Chapter Title 141",
      "position": 2,
      "updated_at": "2016-11-03T12:34:20.521Z",
      "course_id": 211,
      "author_id": 711,
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
      "id": 142,
      "title": "Clever Chapter Title 142",
      "position": 3,
      "updated_at": "2016-11-03T12:34:20.767Z",
      "course_id": 211,
      "author_id": 712,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-11-03T12:34:20.424Z",
      "questions_updated_at": "2016-11-03T12:34:20.424Z",
      "flashcards_count": 1,
      "questions_count": 1
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 54abb9d605ae5648c3e844cbdd72e700415bf436c5bae02b72fb56b97f572f52"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 891084dd1abb3a40b4bfda888d22af4b1977a84669e6994896385dbbdda1262f
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
      "id": 143,
      "title": "Clever Chapter Title 143",
      "position": 1,
      "updated_at": "2016-11-03T12:34:20.904Z",
      "course_id": 212,
      "author_id": 717,
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
      "id": 144,
      "title": "Clever Chapter Title 144",
      "position": 2,
      "updated_at": "2016-11-03T12:34:20.928Z",
      "course_id": 212,
      "author_id": 718,
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
      "id": 145,
      "title": "Clever Chapter Title 145",
      "position": 3,
      "updated_at": "2016-11-03T12:34:20.953Z",
      "course_id": 212,
      "author_id": 719,
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
	-H "Authorization: Bearer 891084dd1abb3a40b4bfda888d22af4b1977a84669e6994896385dbbdda1262f"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/176
Content-Type: application/json
Authorization: Bearer 3c7f8c7abbd6a8aa43b88b59884cf11ad3f324c284a9a0078a83390c4927727c
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/176" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3c7f8c7abbd6a8aa43b88b59884cf11ad3f324c284a9a0078a83390c4927727c"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 3b71283acebf30bf14cd7b77b9b401e9f09a5082085540fe6df81cba04a329d5
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
	-H "Authorization: Bearer 3b71283acebf30bf14cd7b77b9b401e9f09a5082085540fe6df81cba04a329d5"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer 5146239058e913f4b454c02566ba0947018d6d7d5f7510f012383b4f03cfa4e2
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
    "creator_id": 613,
    "id": 190,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 196,
    "additional_university_ids": [

    ],
    "topic_id": 192,
    "discipline_id": 192,
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
    "chapters_updated_at": "2016-11-03T12:34:10.461Z",
    "updated_at": "2016-11-03T12:34:11.851Z",
    "shortname": "fu-choux-pastry-101",
    "chapters": [
      {
        "id": 110,
        "title": "Clever Chapter Title 110",
        "position": 1,
        "updated_at": "2016-11-03T12:34:11.807Z",
        "course_id": 190,
        "author_id": 613,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T12:34:10.461Z",
        "questions_updated_at": "2016-11-03T12:34:10.461Z",
        "flashcards_count": 3,
        "questions_count": 3
      },
      {
        "id": 111,
        "title": "Clever Chapter Title 111",
        "position": 2,
        "updated_at": "2016-11-03T12:34:11.844Z",
        "course_id": 190,
        "author_id": 613,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-11-03T12:34:10.461Z",
        "questions_updated_at": "2016-11-03T12:34:10.461Z",
        "flashcards_count": 3,
        "questions_count": 3
      }
    ],
    "flashcards": [
      {
        "id": 42,
        "obfuscated_id": "6gppIIjkzlA",
        "author_id": 613,
        "chapter_id": 110,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.655Z",
        "created_at": "2016-11-03T12:34:11.655Z",
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
        "id": 44,
        "obfuscated_id": "bbNlnrscV_w",
        "author_id": 613,
        "chapter_id": 111,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.722Z",
        "created_at": "2016-11-03T12:34:11.722Z",
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
        "author_id": 613,
        "chapter_id": 110,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.693Z",
        "created_at": "2016-11-03T12:34:11.693Z",
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
        "author_id": 613,
        "chapter_id": 111,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.760Z",
        "created_at": "2016-11-03T12:34:11.760Z",
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
        "author_id": 616,
        "chapter_id": 110,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.797Z",
        "created_at": "2016-11-03T12:34:11.797Z",
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
        "id": 47,
        "obfuscated_id": "rpshod_7JeU",
        "author_id": 617,
        "chapter_id": 111,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-11-03T12:34:11.834Z",
        "created_at": "2016-11-03T12:34:11.834Z",
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
	-H "Authorization: Bearer 5146239058e913f4b454c02566ba0947018d6d7d5f7510f012383b4f03cfa4e2"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/188
Content-Type: application/json
Authorization: Bearer 0dac592bf5877315cd7d1d063a16c612ac69080e58cbd222bb8978bf666d58ac
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
    "creator_id": 609,
    "id": 188,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 194,
    "additional_university_ids": [

    ],
    "topic_id": 190,
    "discipline_id": 190,
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
    "updated_at": "2016-11-03T12:34:10.338Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/188" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dac592bf5877315cd7d1d063a16c612ac69080e58cbd222bb8978bf666d58ac"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 52cb5e98d85cdb5145b69457a1704179092ab6b1c94db8f60e098f48edc9469a
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
    "creator_id": 606,
    "id": 186,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 192,
    "additional_university_ids": [

    ],
    "topic_id": 188,
    "discipline_id": 188,
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
    "updated_at": "2016-11-03T12:34:10.063Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101" -d '{"course":{"title":"Choux pastry 102","language_code":"fr","published":false}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 52cb5e98d85cdb5145b69457a1704179092ab6b1c94db8f60e098f48edc9469a"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer dc3517ae299c23cec70e16ee4c5f9db4818c6a9a832b05788b8325f99bd05804
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
      "id": 20,
      "user_id": 105,
      "feedbackable_id": 15,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:34.013Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 21,
      "user_id": 109,
      "feedbackable_id": 16,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:34.285Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 22,
      "user_id": 113,
      "feedbackable_id": 17,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:34.562Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 23,
      "user_id": 117,
      "feedbackable_id": 18,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:34.842Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 24,
      "user_id": 121,
      "feedbackable_id": 19,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T12:33:35.126Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer dc3517ae299c23cec70e16ee4c5f9db4818c6a9a832b05788b8325f99bd05804"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer c3edcb85ac6d817598409cbd4c6b0d5b5ba8eb2be3dc30406b7b6c5cecc81c89
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
      "id": 10,
      "user_id": 63,
      "feedbackable_id": 5,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-11-03T12:33:30.969Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer c3edcb85ac6d817598409cbd4c6b0d5b5ba8eb2be3dc30406b7b6c5cecc81c89"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/15
Content-Type: application/json
Authorization: Bearer aea20e91d7074d354f54fc0018125e7c59a14e8c6e13892c560c785f10b34dfe
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/15" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer aea20e91d7074d354f54fc0018125e7c59a14e8c6e13892c560c785f10b34dfe"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/9/metadata
Content-Type: application/json
Authorization: Bearer e3e7cf65ef73132ec7bbf1aa4c06ae8a444120e63b3d14771c5e44e41ac5fc2b
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
    "id": 9,
    "uploader": {
      "id": 529,
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
      "created_at": "2016-11-03T12:34:03.297Z",
      "updated_at": "2016-11-03T12:34:03.297Z"
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
    "created_at": "2016-11-03T12:34:03.369Z",
    "updated_at": "2016-11-03T12:34:03.369Z",
    "course_id": 162,
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
curl "api.goskive.com/v2/files/9/metadata" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e3e7cf65ef73132ec7bbf1aa4c06ae8a444120e63b3d14771c5e44e41ac5fc2b"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/70/feedbacks
Content-Type: application/json
Authorization: Bearer 94e3cb38b79b652233c028c8738fea86e2163686bd0bf7938c170cb6db4b24e0
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
      "id": 43,
      "user_id": 662,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:17.725Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 42,
      "user_id": 661,
      "feedbackable_id": 70,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:34:17.715Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/70/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 94e3cb38b79b652233c028c8738fea86e2163686bd0bf7938c170cb6db4b24e0"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer c9e944f02e941eec44e9038226d5e9958d3ed9cc19d0f706e4f2b4ed03e85416
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
      "id": 23,
      "obfuscated_id": "eUsQCUPDncM",
      "author_id": 432,
      "chapter_id": 80,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:57.049Z",
      "created_at": "2016-11-03T12:33:57.049Z",
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
      "author_id": 435,
      "chapter_id": 81,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:57.210Z",
      "created_at": "2016-11-03T12:33:57.210Z",
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
      "author_id": 438,
      "chapter_id": 82,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:57.337Z",
      "created_at": "2016-11-03T12:33:57.337Z",
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
      "author_id": 441,
      "chapter_id": 83,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:57.465Z",
      "created_at": "2016-11-03T12:33:57.465Z",
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
      "author_id": 444,
      "chapter_id": 84,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:57.593Z",
      "created_at": "2016-11-03T12:33:57.593Z",
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
	-H "Authorization: Bearer c9e944f02e941eec44e9038226d5e9958d3ed9cc19d0f706e4f2b4ed03e85416"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 73a0c845dc97ccd5927dea2050f5a15e27c11f0fda75659662ad0a458a5129d4
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
      "id": 22,
      "obfuscated_id": "V2ZFfduV4jE",
      "author_id": 428,
      "chapter_id": 79,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:56.888Z",
      "created_at": "2016-11-03T12:33:56.888Z",
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
	-H "Authorization: Bearer 73a0c845dc97ccd5927dea2050f5a15e27c11f0fda75659662ad0a458a5129d4"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/13/republish
Content-Type: application/json
Authorization: Bearer 6c4f621dca24742274514b0ab580df831d852b81c457139fca2951cddff5ca37
```

`PUT /v2/flashcards/:flashcard_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/flashcards/13/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 6c4f621dca24742274514b0ab580df831d852b81c457139fca2951cddff5ca37"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/59/feedbacks
Content-Type: application/json
Authorization: Bearer 03e22ca099e53ed5dd77eaebdfa60c78a7666563579ca025f8621516f67be0d7
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
      "id": 30,
      "user_id": 483,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:59.834Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 29,
      "user_id": 482,
      "feedbackable_id": 59,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-11-03T12:33:59.823Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/59/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 03e22ca099e53ed5dd77eaebdfa60c78a7666563579ca025f8621516f67be0d7"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 56c30d3225daffe5e7b4d8f28f3ee32e6e411611e6934b372cd19154d9fd403e
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
      "id": 28,
      "obfuscated_id": "hO6PHFgN8Aw",
      "author_id": 193,
      "chapter_id": 37,
      "position": 23,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:41.137Z",
      "created_at": "2016-11-03T12:33:41.028Z",
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
      "id": 29,
      "obfuscated_id": "rvs1sHrnKS4",
      "author_id": 196,
      "chapter_id": 38,
      "position": 24,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:41.406Z",
      "created_at": "2016-11-03T12:33:41.292Z",
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
    },
    {
      "id": 30,
      "obfuscated_id": "virmgqGG22o",
      "author_id": 199,
      "chapter_id": 39,
      "position": 25,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:41.677Z",
      "created_at": "2016-11-03T12:33:41.562Z",
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
          "id": 60,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 61,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 31,
      "obfuscated_id": "5rbCnI5XGHg",
      "author_id": 202,
      "chapter_id": 40,
      "position": 26,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:41.949Z",
      "created_at": "2016-11-03T12:33:41.833Z",
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
          "id": 62,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 63,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 32,
      "obfuscated_id": "mUuSuaqqphM",
      "author_id": 205,
      "chapter_id": 41,
      "position": 27,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:42.210Z",
      "created_at": "2016-11-03T12:33:42.101Z",
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
          "id": 64,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 65,
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
	-H "Authorization: Bearer 56c30d3225daffe5e7b4d8f28f3ee32e6e411611e6934b372cd19154d9fd403e"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 7782be735ea5dd93f2fc787a65541b2e7fca8b670d0d1e62b15f11792abf9739
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
      "id": 37,
      "obfuscated_id": "95m_4XdR9PU",
      "author_id": 221,
      "chapter_id": 46,
      "position": 32,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-11-03T12:33:43.611Z",
      "created_at": "2016-11-03T12:33:43.504Z",
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
          "id": 74,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 75,
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
	-H "Authorization: Bearer 7782be735ea5dd93f2fc787a65541b2e7fca8b670d0d1e62b15f11792abf9739"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/46/republish
Content-Type: application/json
Authorization: Bearer 3b2f121aad5de9d1d214d66ab21839f01015f4d4fd15f3ff6f5e46bec81255ce
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/46/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 3b2f121aad5de9d1d214d66ab21839f01015f4d4fd15f3ff6f5e46bec81255ce"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer fae5409f3946c9e3efa44bd1566140842e6ba5c990cd313433a3435da5408999
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":269,"published":false}}
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
    "creator_id": 802,
    "id": 265,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 249,
    "additional_university_ids": [

    ],
    "topic_id": 269,
    "discipline_id": 270,
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
    "updated_at": "2016-11-03T12:34:27.516Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ]
  }
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":269,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fae5409f3946c9e3efa44bd1566140842e6ba5c990cd313433a3435da5408999"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 675c25a20ffd5053c55370de241c149b80ca3519d8e5a24241cb388b6f140091
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
      "creator_id": 759,
      "id": 227,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-188",
      "html_url": "https://goskive.com/course/fu-course-188",
      "slug": "fu-course-188",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "topic_id": 231,
      "discipline_id": 232,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 188",
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
      "updated_at": "2016-11-03T12:34:23.668Z",
      "shortname": "fu-course-188"
    },
    {
      "creator_id": 759,
      "id": 228,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-189",
      "html_url": "https://goskive.com/course/fu-course-189",
      "slug": "fu-course-189",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "topic_id": 232,
      "discipline_id": 233,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 189",
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
      "updated_at": "2016-11-03T12:34:23.708Z",
      "shortname": "fu-course-189"
    },
    {
      "creator_id": 760,
      "id": 229,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-190",
      "html_url": "https://goskive.com/course/fu-course-190",
      "slug": "fu-course-190",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "topic_id": 233,
      "discipline_id": 234,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 190",
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
      "updated_at": "2016-11-03T12:34:23.757Z",
      "shortname": "fu-course-190"
    },
    {
      "creator_id": 760,
      "id": 230,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-191",
      "html_url": "https://goskive.com/course/fu-course-191",
      "slug": "fu-course-191",
      "university_id": 233,
      "additional_university_ids": [

      ],
      "topic_id": 234,
      "discipline_id": 235,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 191",
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
      "chapters_updated_at": "2016-11-03T12:34:24.036Z",
      "updated_at": "2016-11-03T12:34:24.043Z",
      "shortname": "fu-course-191"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 675c25a20ffd5053c55370de241c149b80ca3519d8e5a24241cb388b6f140091"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer bce8d9712cce362441ec56c1b646874736da22465d8cec5b0dbef8c5d02f403c
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
      "creator_id": 766,
      "id": 231,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-192",
      "html_url": "https://goskive.com/course/fu-course-192",
      "slug": "fu-course-192",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 235,
      "discipline_id": 236,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 192",
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
      "updated_at": "2016-11-03T12:34:24.278Z",
      "shortname": "fu-course-192"
    },
    {
      "creator_id": 766,
      "id": 232,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-193",
      "html_url": "https://goskive.com/course/fu-course-193",
      "slug": "fu-course-193",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 236,
      "discipline_id": 237,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 193",
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
      "updated_at": "2016-11-03T12:34:24.316Z",
      "shortname": "fu-course-193"
    },
    {
      "creator_id": 767,
      "id": 233,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-194",
      "html_url": "https://goskive.com/course/fu-course-194",
      "slug": "fu-course-194",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 237,
      "discipline_id": 238,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 194",
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
      "updated_at": "2016-11-03T12:34:24.362Z",
      "shortname": "fu-course-194"
    },
    {
      "creator_id": 767,
      "id": 234,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-195",
      "html_url": "https://goskive.com/course/fu-course-195",
      "slug": "fu-course-195",
      "university_id": 235,
      "additional_university_ids": [

      ],
      "topic_id": 238,
      "discipline_id": 239,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 195",
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
      "updated_at": "2016-11-03T12:34:24.400Z",
      "shortname": "fu-course-195"
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer bce8d9712cce362441ec56c1b646874736da22465d8cec5b0dbef8c5d02f403c"
```
