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
DELETE /v2/chapters/166
Content-Type: application/json
Authorization: Bearer f5aaecc2ee29b912901baebe5147a0c5556960a7a1e6d0bbaeb635ca52708037
```

`DELETE /v2/chapters/:chapter_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/chapters/166" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f5aaecc2ee29b912901baebe5147a0c5556960a7a1e6d0bbaeb635ca52708037"
```
## Get a chapter


### Request

#### Endpoint

```
GET /v2/chapters/162
Content-Type: application/json
Authorization: Bearer 565a3965924c00e7a0729a9706ccf581964a7d68d67ba01999b691e8b15dcc4b
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
    "id": 162,
    "updated_at": "2016-12-15T11:57:23.294Z",
    "course_id": 215,
    "author_id": 692,
    "permissions": [
      "update",
      "delete"
    ],
    "flashcards_updated_at": "2016-12-15T11:57:22.795Z",
    "questions_updated_at": "2016-12-15T11:57:22.795Z",
    "flashcards_count": 2,
    "questions_count": 2,
    "flashcards": [
      {
        "id": 70,
        "obfuscated_id": "EDEz1xzotLc",
        "author_id": 695,
        "chapter_id": 162,
        "position": 1,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.235Z",
        "created_at": "2016-12-15T11:57:23.235Z",
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
        "id": 71,
        "obfuscated_id": "--JhLc6KEBw",
        "author_id": 696,
        "chapter_id": 162,
        "position": 2,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.276Z",
        "created_at": "2016-12-15T11:57:23.276Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 693,
        "chapter_id": 162,
        "position": 73,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.020Z",
        "created_at": "2016-12-15T11:57:22.946Z",
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
            "id": 164,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 165,
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
        "author_id": 694,
        "chapter_id": 162,
        "position": 74,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:23.173Z",
        "created_at": "2016-12-15T11:57:23.087Z",
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
            "id": 166,
            "position": 1,
            "content": "MyText",
            "content_html": "MyText",
            "correct": true
          },
          {
            "id": 167,
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
curl "api.goskive.com/v2/chapters/162" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 565a3965924c00e7a0729a9706ccf581964a7d68d67ba01999b691e8b15dcc4b"
```
## Update a chapter


### Request

#### Endpoint

```
PATCH /v2/chapters/161
Content-Type: application/json
Authorization: Bearer d5271d3016e85c5f1086e15648f29f2c00f57e9169c4e539525eec20115cf417
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
    "id": 161,
    "updated_at": "2016-12-15T11:57:22.761Z",
    "course_id": 214,
    "author_id": 689,
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
curl "api.goskive.com/v2/chapters/161" -d '{"chapter":{"title":"Eggs and Flour"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d5271d3016e85c5f1086e15648f29f2c00f57e9169c4e539525eec20115cf417"
```
# Comments

## Delete a comment


### Request

#### Endpoint

```
DELETE /v2/comments/57
Content-Type: application/json
Authorization: Bearer 4887a1c3e2b630f546a82f41444e0f4fc8de8588ae0954322c23128fa8759588
```

`DELETE /v2/comments/:comment_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/57" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 4887a1c3e2b630f546a82f41444e0f4fc8de8588ae0954322c23128fa8759588"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 56984ab6350e6e4dca693351c6b8f4c9355529df8abbdb58593ba613b6758b26
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
      "id": 22,
      "author_id": 847,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:41.236Z",
      "status": "published",
      "subject_id": 258,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 23,
      "author_id": 849,
      "reply_to_id": 22,
      "created_at": "2016-12-15T11:57:41.370Z",
      "status": "published",
      "subject_id": 259,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 24,
      "author_id": 851,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:41.500Z",
      "status": "published",
      "subject_id": 260,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 25,
      "author_id": 853,
      "reply_to_id": 24,
      "created_at": "2016-12-15T11:57:41.631Z",
      "status": "published",
      "subject_id": 261,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 26,
      "author_id": 855,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:41.766Z",
      "status": "reported",
      "subject_id": 262,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 27,
      "author_id": 857,
      "reply_to_id": 26,
      "created_at": "2016-12-15T11:57:41.904Z",
      "status": "published",
      "subject_id": 263,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 28,
      "author_id": 859,
      "reply_to_id": 26,
      "created_at": "2016-12-15T11:57:42.041Z",
      "status": "published",
      "subject_id": 264,
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
	-H "Authorization: Bearer 56984ab6350e6e4dca693351c6b8f4c9355529df8abbdb58593ba613b6758b26"
```
## Get a list of all comments


### Request

#### Endpoint

```
GET /v2/comments
Content-Type: application/json
Authorization: Bearer 28b654c787ed1219e4986b7357a863beb44a49ad8acf2b393bbe62bd26969fef
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
      "id": 29,
      "author_id": 862,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:42.245Z",
      "status": "published",
      "subject_id": 265,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 30,
      "author_id": 864,
      "reply_to_id": 29,
      "created_at": "2016-12-15T11:57:42.387Z",
      "status": "published",
      "subject_id": 266,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 31,
      "author_id": 866,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:42.525Z",
      "status": "published",
      "subject_id": 267,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 32,
      "author_id": 868,
      "reply_to_id": 31,
      "created_at": "2016-12-15T11:57:42.656Z",
      "status": "published",
      "subject_id": 268,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 33,
      "author_id": 870,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:42.787Z",
      "status": "reported",
      "subject_id": 269,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 34,
      "author_id": 872,
      "reply_to_id": 33,
      "created_at": "2016-12-15T11:57:42.925Z",
      "status": "published",
      "subject_id": 270,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 35,
      "author_id": 874,
      "reply_to_id": 33,
      "created_at": "2016-12-15T11:57:43.065Z",
      "status": "published",
      "subject_id": 271,
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
	-H "Authorization: Bearer 28b654c787ed1219e4986b7357a863beb44a49ad8acf2b393bbe62bd26969fef"
```
## Get a list of comments filtered by level


### Request

#### Endpoint

```
GET /v2/comments?level=replies
Content-Type: application/json
Authorization: Bearer e0c09922812ab7715e0ba948bf7b7b3a7655ce26e9a032c7432567e4aa6db115
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
      "id": 44,
      "author_id": 894,
      "reply_to_id": 43,
      "created_at": "2016-12-15T11:57:44.414Z",
      "status": "published",
      "subject_id": 280,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 46,
      "author_id": 898,
      "reply_to_id": 45,
      "created_at": "2016-12-15T11:57:44.803Z",
      "status": "published",
      "subject_id": 282,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 48,
      "author_id": 902,
      "reply_to_id": 47,
      "created_at": "2016-12-15T11:57:45.067Z",
      "status": "published",
      "subject_id": 284,
      "subject_type": "Course",
      "message": "Clearly this information is problematic.",
      "feedback": null
    },
    {
      "id": 49,
      "author_id": 904,
      "reply_to_id": 47,
      "created_at": "2016-12-15T11:57:45.199Z",
      "status": "published",
      "subject_id": 285,
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
	-H "Authorization: Bearer e0c09922812ab7715e0ba948bf7b7b3a7655ce26e9a032c7432567e4aa6db115"
```
## Get a list of comments filtered by status


### Request

#### Endpoint

```
GET /v2/comments?status=reported
Content-Type: application/json
Authorization: Bearer 56cccb7ae8ba9abb28182e964772390236601ebc426b6c615b547a4d3ed1dd31
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
      "id": 40,
      "author_id": 885,
      "reply_to_id": null,
      "created_at": "2016-12-15T11:57:43.835Z",
      "status": "reported",
      "subject_id": 276,
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
	-H "Authorization: Bearer 56cccb7ae8ba9abb28182e964772390236601ebc426b6c615b547a4d3ed1dd31"
```
## republishes the comment


### Request

#### Endpoint

```
PUT /v2/comments/21/republish
Content-Type: application/json
Authorization: Bearer f524ed755b39ab646cbc671a582d8513fe44016fac9d3c67f326a1350ce71ea6
```

`PUT /v2/comments/:comment_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/comments/21/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer f524ed755b39ab646cbc671a582d8513fe44016fac9d3c67f326a1350ce71ea6"
```
# Course Chapters

## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 99c13be61f1ea11ae1d57a70df4d49751b5a7dbe601c0864e022663a170b4397
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
    "id": 106,
    "updated_at": "2016-12-15T11:57:00.260Z",
    "course_id": 140,
    "author_id": 445,
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
	-H "Authorization: Bearer 99c13be61f1ea11ae1d57a70df4d49751b5a7dbe601c0864e022663a170b4397"
```
## Create a chapter


### Request

#### Endpoint

```
POST /v2/courses/141/chapters
Content-Type: application/json
Authorization: Bearer 751ca9d2186202c0872d35539e000bd168bda6f82675a121807b1ca719937087
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
    "id": 107,
    "updated_at": "2016-12-15T11:57:00.444Z",
    "course_id": 141,
    "author_id": 447,
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
curl "api.goskive.com/v2/courses/141/chapters" -d '{"chapter":{"title":"Preparing the oven"}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 751ca9d2186202c0872d35539e000bd168bda6f82675a121807b1ca719937087"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer b4d4a8444ea407252ed2c7086a72ce086a63eebd6267cc898074d8056131a4fe
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
      "id": 87,
      "updated_at": "2016-12-15T11:56:57.362Z",
      "course_id": 129,
      "author_id": 402,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 81",
      "position": 1
    },
    {
      "id": 88,
      "updated_at": "2016-12-15T11:56:57.386Z",
      "course_id": 129,
      "author_id": 403,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 82",
      "position": 2
    },
    {
      "id": 89,
      "updated_at": "2016-12-15T11:56:57.599Z",
      "course_id": 129,
      "author_id": 404,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": "2016-12-15T11:56:57.241Z",
      "questions_updated_at": "2016-12-15T11:56:57.241Z",
      "flashcards_count": 1,
      "questions_count": 1,
      "title": "Clever Chapter Title 83",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer b4d4a8444ea407252ed2c7086a72ce086a63eebd6267cc898074d8056131a4fe"
```
## Get a list of course chapters


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101/chapters
Content-Type: application/json
Authorization: Bearer 22e357448603de77592b0e6afda3564557f3053edd5c9017050c544c4436e428
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
      "id": 90,
      "updated_at": "2016-12-15T11:56:57.805Z",
      "course_id": 130,
      "author_id": 409,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 84",
      "position": 1
    },
    {
      "id": 91,
      "updated_at": "2016-12-15T11:56:57.831Z",
      "course_id": 130,
      "author_id": 410,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 85",
      "position": 2
    },
    {
      "id": 92,
      "updated_at": "2016-12-15T11:56:57.856Z",
      "course_id": 130,
      "author_id": 411,
      "permissions": [
        "update",
        "delete"
      ],
      "flashcards_updated_at": null,
      "questions_updated_at": null,
      "flashcards_count": 0,
      "questions_count": 0,
      "title": "Clever Chapter Title 86",
      "position": 3
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/courses/fu-choux-pastry-101/chapters" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 22e357448603de77592b0e6afda3564557f3053edd5c9017050c544c4436e428"
```
# Courses

## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer bd1ed4b678d1361595da8ebd01ad6a49fae1459b5eabc914f1d1141865330011
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
	-H "Authorization: Bearer bd1ed4b678d1361595da8ebd01ad6a49fae1459b5eabc914f1d1141865330011"
```
## Delete a course


### Request

#### Endpoint

```
DELETE /v2/courses/233
Content-Type: application/json
Authorization: Bearer 9db242e2e0d0c22c4da00a5ad920be200c120896da481f8dc547a522ae763c29
```

`DELETE /v2/courses/:course_slug`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/courses/233" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 9db242e2e0d0c22c4da00a5ad920be200c120896da481f8dc547a522ae763c29"
```
## Get a course


### Request

#### Endpoint

```
GET /v2/courses/fu-choux-pastry-101?include=flashcards%2C+invalid_resources
Content-Type: application/json
Authorization: Bearer c1da3f20d4ad7b9cdda67f8a21e5b86e11b40d626fb51d551896ed1acf4bfd8b
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
    "creator_id": 723,
    "id": 222,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-101",
    "html_url": "https://goskive.com/course/fu-choux-pastry-101",
    "slug": "fu-choux-pastry-101",
    "university_id": 207,
    "additional_university_ids": [

    ],
    "discipline_id": 232,
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
    "chapters_updated_at": "2016-12-15T11:57:26.414Z",
    "updated_at": "2016-12-15T11:57:27.674Z",
    "shortname": "fu-choux-pastry-101",
    "flashcards": [
      {
        "id": 80,
        "obfuscated_id": "94gVa2GR5x8",
        "author_id": 723,
        "chapter_id": 170,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.452Z",
        "created_at": "2016-12-15T11:57:27.452Z",
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
        "id": 82,
        "obfuscated_id": "D5TJ6kac5FE",
        "author_id": 723,
        "chapter_id": 171,
        "position": 1,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.529Z",
        "created_at": "2016-12-15T11:57:27.529Z",
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
        "id": 81,
        "obfuscated_id": "jHF1owx40fU",
        "author_id": 723,
        "chapter_id": 170,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.496Z",
        "created_at": "2016-12-15T11:57:27.496Z",
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
        "id": 83,
        "obfuscated_id": "FCSR-nKROLo",
        "author_id": 723,
        "chapter_id": 171,
        "position": 2,
        "reviewed": false,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.571Z",
        "created_at": "2016-12-15T11:57:27.571Z",
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
        "id": 84,
        "obfuscated_id": "Hu6DTUHzhWo",
        "author_id": 726,
        "chapter_id": 170,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.612Z",
        "created_at": "2016-12-15T11:57:27.612Z",
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
        "id": 85,
        "obfuscated_id": "xR5KgQjIo2Y",
        "author_id": 727,
        "chapter_id": 171,
        "position": 3,
        "reviewed": true,
        "upvotes_count": 0,
        "downvotes_count": 0,
        "updated_at": "2016-12-15T11:57:27.653Z",
        "created_at": "2016-12-15T11:57:27.653Z",
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
        "id": 170,
        "updated_at": "2016-12-15T11:57:27.622Z",
        "course_id": 222,
        "author_id": 723,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T11:57:26.414Z",
        "questions_updated_at": "2016-12-15T11:57:26.414Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 152",
        "position": 1
      },
      {
        "id": 171,
        "updated_at": "2016-12-15T11:57:27.664Z",
        "course_id": 222,
        "author_id": 723,
        "permissions": [
          "update",
          "delete"
        ],
        "flashcards_updated_at": "2016-12-15T11:57:26.414Z",
        "questions_updated_at": "2016-12-15T11:57:26.414Z",
        "flashcards_count": 3,
        "questions_count": 3,
        "title": "Clever Chapter Title 153",
        "position": 2
      }
    ],
    "topic_id": 232,
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
	-H "Authorization: Bearer c1da3f20d4ad7b9cdda67f8a21e5b86e11b40d626fb51d551896ed1acf4bfd8b"
```
## Update a course


### Request

#### Endpoint

```
PATCH /v2/courses/237
Content-Type: application/json
Authorization: Bearer e903e370f705e5532c492837e4d7896c55fdae40add14f5c3c4eedd7da716bc1
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
    "creator_id": 765,
    "id": 237,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 222,
    "additional_university_ids": [

    ],
    "discipline_id": 247,
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
    "updated_at": "2016-12-15T11:57:33.217Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 247,
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
curl "api.goskive.com/v2/courses/237" -d '{"course":{"title":"Choux pastry 102","language_code":"fr"}}' -X PATCH \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer e903e370f705e5532c492837e4d7896c55fdae40add14f5c3c4eedd7da716bc1"
```
## Update permitted course properties


### Request

#### Endpoint

```
PATCH /v2/courses/fu-choux-pastry-101
Content-Type: application/json
Authorization: Bearer 5c2c98ca78d9159651249d78d972d952a22a0ea915860d2abcc163278dcfb2a4
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
    "creator_id": 760,
    "id": 234,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-102",
    "html_url": "https://goskive.com/course/fu-choux-pastry-102",
    "slug": "fu-choux-pastry-102",
    "university_id": 219,
    "additional_university_ids": [

    ],
    "discipline_id": 244,
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
    "updated_at": "2016-12-15T11:57:32.668Z",
    "shortname": "fu-choux-pastry-102",
    "chapters": [

    ],
    "topic_id": 244,
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
	-H "Authorization: Bearer 5c2c98ca78d9159651249d78d972d952a22a0ea915860d2abcc163278dcfb2a4"
```
# Feedback

## Get a list of all feedbacks


### Request

#### Endpoint

```
GET /v2/feedbacks
Content-Type: application/json
Authorization: Bearer df175c4a38db139f7978e65a1114841b72d23fd7f64bb9948a234a82a017f67b
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
      "id": 16,
      "user_id": 309,
      "feedbackable_id": 36,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:56:50.389Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 17,
      "user_id": 313,
      "feedbackable_id": 37,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:56:50.708Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 18,
      "user_id": 317,
      "feedbackable_id": 38,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:56:51.019Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 19,
      "user_id": 321,
      "feedbackable_id": 39,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:56:51.329Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 20,
      "user_id": 325,
      "feedbackable_id": 40,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T11:56:51.636Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer df175c4a38db139f7978e65a1114841b72d23fd7f64bb9948a234a82a017f67b"
```
## Get a list of feedbacks filtered by status


### Request

#### Endpoint

```
GET /v2/feedbacks?status=abandoned
Content-Type: application/json
Authorization: Bearer 735c61decfc8bb9592fa106df0ed971129b0749bb30b23ce6f27c6ee1c510e68
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
      "id": 6,
      "user_id": 267,
      "feedbackable_id": 26,
      "feedbackable_type": "Question",
      "workflow_state": "abandoned",
      "updated_at": "2016-12-15T11:56:47.083Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/feedbacks?status=abandoned" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 735c61decfc8bb9592fa106df0ed971129b0749bb30b23ce6f27c6ee1c510e68"
```
# Files

## Delete a file


### Request

#### Endpoint

```
DELETE /v2/files/18
Content-Type: application/json
Authorization: Bearer d2eb3e0bbc225b6e889be080a225ec8cc6225f36a233d70e6b4eaf60574da3ef
```

`DELETE /v2/files/:file_id`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/files/18" -d '' -X DELETE \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d2eb3e0bbc225b6e889be080a225ec8cc6225f36a233d70e6b4eaf60574da3ef"
```
## Get a file metadata


### Request

#### Endpoint

```
GET /v2/files/13/metadata
Content-Type: application/json
Authorization: Bearer 4cdf0adca5375f046255156ba380fc1c27bd14cbc6983e5cbb3455e591228e99
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
      "id": 942,
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
      "created_at": "2016-12-15T11:57:47.669Z",
      "updated_at": "2016-12-15T11:57:47.669Z"
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
    "created_at": "2016-12-15T11:57:47.804Z",
    "updated_at": "2016-12-15T11:57:47.804Z",
    "course_id": 300,
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
	-H "Authorization: Bearer 4cdf0adca5375f046255156ba380fc1c27bd14cbc6983e5cbb3455e591228e99"
```
# Flashcard Feedbacks

## Get a list of flashcard feedbacks


### Request

#### Endpoint

```
GET /v2/flashcards/65/feedbacks
Content-Type: application/json
Authorization: Bearer fbdd2379b4f63c521790339848de90f66a05e9d7c47052a697cba64bfe74c32f
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
      "id": 34,
      "user_id": 660,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:21.001Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 33,
      "user_id": 659,
      "feedbackable_id": 65,
      "feedbackable_type": "Flashcard",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:20.990Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/flashcards/65/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer fbdd2379b4f63c521790339848de90f66a05e9d7c47052a697cba64bfe74c32f"
```
# Flashcards

## Get a list of all flashcards


### Request

#### Endpoint

```
GET /v2/flashcards
Content-Type: application/json
Authorization: Bearer 627f8658c9a2c20e018bec96eec73cf7059567099c9b888ae199936db5fb3c33
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
      "id": 15,
      "obfuscated_id": "j5PwoYQzNCc",
      "author_id": 104,
      "chapter_id": 23,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:30.825Z",
      "created_at": "2016-12-15T11:56:30.825Z",
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
      "author_id": 107,
      "chapter_id": 24,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:31.002Z",
      "created_at": "2016-12-15T11:56:31.002Z",
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
      "author_id": 110,
      "chapter_id": 25,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:31.211Z",
      "created_at": "2016-12-15T11:56:31.211Z",
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
      "author_id": 113,
      "chapter_id": 26,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:31.401Z",
      "created_at": "2016-12-15T11:56:31.401Z",
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
      "id": 19,
      "obfuscated_id": "xt199h-LGto",
      "author_id": 116,
      "chapter_id": 27,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:31.590Z",
      "created_at": "2016-12-15T11:56:31.590Z",
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
	-H "Authorization: Bearer 627f8658c9a2c20e018bec96eec73cf7059567099c9b888ae199936db5fb3c33"
```
## Get a list of flashcards filtered by status


### Request

#### Endpoint

```
GET /v2/flashcards?status=reported
Content-Type: application/json
Authorization: Bearer 3d7087b4aa863f7506167dbcd418da0cd95c3ae79270ca9b99af395f355ce512
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
      "id": 24,
      "obfuscated_id": "KHM5yo_z4Ds",
      "author_id": 132,
      "chapter_id": 32,
      "position": 1,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:56:32.724Z",
      "created_at": "2016-12-15T11:56:32.724Z",
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
	-H "Authorization: Bearer 3d7087b4aa863f7506167dbcd418da0cd95c3ae79270ca9b99af395f355ce512"
```
## republishes the flashcard


### Request

#### Endpoint

```
PUT /v2/flashcards/26/republish
Content-Type: application/json
Authorization: Bearer 1e5dc0b69e150ab26d190d2988825c0e9e9462b549b55bb6047d1a5bdf57f290
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
	-H "Authorization: Bearer 1e5dc0b69e150ab26d190d2988825c0e9e9462b549b55bb6047d1a5bdf57f290"
```
# Question Feedbacks

## Get a list of question feedbacks


### Request

#### Endpoint

```
GET /v2/questions/116/feedbacks
Content-Type: application/json
Authorization: Bearer d0197960700bc09d752fd01994699801b3ccf6293630111f2fa9b64d2c174a4b
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
      "id": 42,
      "user_id": 789,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:34.610Z",
      "flags": 1,
      "message": ""
    },
    {
      "id": 41,
      "user_id": 788,
      "feedbackable_id": 116,
      "feedbackable_type": "Question",
      "workflow_state": "new",
      "updated_at": "2016-12-15T11:57:34.598Z",
      "flags": 1,
      "message": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/questions/116/feedbacks" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d0197960700bc09d752fd01994699801b3ccf6293630111f2fa9b64d2c174a4b"
```
# Questions

## Get a list of all questions


### Request

#### Endpoint

```
GET /v2/questions
Content-Type: application/json
Authorization: Bearer 1c7d23de6ee58619b6836f86b9fe601bc9ab7fe2b5258db650ca4e8dcaa53795
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
      "id": 74,
      "obfuscated_id": "fL3buOIYvUI",
      "author_id": 597,
      "chapter_id": 143,
      "position": 68,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:15.091Z",
      "created_at": "2016-12-15T11:57:15.007Z",
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
          "id": 148,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 149,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 75,
      "obfuscated_id": "rRYuZazyhgg",
      "author_id": 600,
      "chapter_id": 144,
      "position": 69,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:15.366Z",
      "created_at": "2016-12-15T11:57:15.285Z",
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
          "id": 150,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 151,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 76,
      "obfuscated_id": "oK0h_-4yfUk",
      "author_id": 603,
      "chapter_id": 145,
      "position": 70,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:15.645Z",
      "created_at": "2016-12-15T11:57:15.562Z",
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
          "id": 152,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 153,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 77,
      "obfuscated_id": "v-Dlx6JosLA",
      "author_id": 606,
      "chapter_id": 146,
      "position": 71,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:15.929Z",
      "created_at": "2016-12-15T11:57:15.843Z",
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
          "id": 154,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 155,
          "position": 2,
          "content": "MyText",
          "content_html": "MyText",
          "correct": false
        }
      ]
    },
    {
      "id": 78,
      "obfuscated_id": "-wsYNe2w7uo",
      "author_id": 609,
      "chapter_id": 147,
      "position": 72,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:16.368Z",
      "created_at": "2016-12-15T11:57:16.291Z",
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
          "id": 156,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 157,
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
	-H "Authorization: Bearer 1c7d23de6ee58619b6836f86b9fe601bc9ab7fe2b5258db650ca4e8dcaa53795"
```
## Get a list of questions filtered by status


### Request

#### Endpoint

```
GET /v2/questions?status=reported
Content-Type: application/json
Authorization: Bearer 3ed5e92edaa72eacd48782eaab4e3f9dbb7b35e44da936d3797d3ca71854a08d
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
      "id": 73,
      "obfuscated_id": "LJvjpBojvP0",
      "author_id": 593,
      "chapter_id": 142,
      "position": 67,
      "reviewed": true,
      "upvotes_count": 0,
      "downvotes_count": 0,
      "updated_at": "2016-12-15T11:57:14.753Z",
      "created_at": "2016-12-15T11:57:14.676Z",
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
          "id": 146,
          "position": 1,
          "content": "MyText",
          "content_html": "MyText",
          "correct": true
        },
        {
          "id": 147,
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
	-H "Authorization: Bearer 3ed5e92edaa72eacd48782eaab4e3f9dbb7b35e44da936d3797d3ca71854a08d"
```
## Republish a question


### Request

#### Endpoint

```
PUT /v2/questions/61/republish
Content-Type: application/json
Authorization: Bearer ef9751c3c25c63508f44d14baf101c5316619afa81c259e181689a412d44ede2
```

`PUT /v2/questions/:question_id/republish`

#### Parameters


None known.


### Response

```

204 No Content
```




```shell
curl "api.goskive.com/v2/questions/61/republish" -d '' -X PUT \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer ef9751c3c25c63508f44d14baf101c5316619afa81c259e181689a412d44ede2"
```
# University Courses

## Create an unpublished course, respecting permitted properties


### Request

#### Endpoint

```
POST /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 5a3eb4443b68c9103ef8e141194fab53ee269d81e3b95b5edb23e1adcb424acb
```

`POST /v2/universities/:university_slug/courses`

#### Parameters


```json
{"course":{"title":"Choux pastry 201","topic_id":38,"published":false}}
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
    "creator_id": 43,
    "id": 38,
    "self_url": "http://api.goskive.test/api/v2/courses/fu-choux-pastry-201",
    "html_url": "https://goskive.com/course/fu-choux-pastry-201",
    "slug": "fu-choux-pastry-201",
    "university_id": 16,
    "additional_university_ids": [

    ],
    "discipline_id": 38,
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
    "updated_at": "2016-12-15T11:56:24.253Z",
    "shortname": "fu-choux-pastry-201",
    "chapters": [

    ],
    "topic_id": 38,
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
curl "api.goskive.com/v2/universities/fu-berlin/courses" -d '{"course":{"title":"Choux pastry 201","topic_id":38,"published":false}}' -X POST \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 5a3eb4443b68c9103ef8e141194fab53ee269d81e3b95b5edb23e1adcb424acb"
```
## Get a list including counts, permissions


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer d709879b5994ccec6053ae397e15c33c090c5cf1a3dfa9929cee32ed9374fb75
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
      "creator_id": 1,
      "id": 1,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-1",
      "html_url": "https://goskive.com/course/fu-course-1",
      "slug": "fu-course-1",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "discipline_id": 1,
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
      "updated_at": "2016-12-15T11:56:19.508Z",
      "shortname": "fu-course-1",
      "topic_id": 1,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 1",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 1,
      "id": 2,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-2",
      "html_url": "https://goskive.com/course/fu-course-2",
      "slug": "fu-course-2",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "discipline_id": 2,
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
      "updated_at": "2016-12-15T11:56:19.552Z",
      "shortname": "fu-course-2",
      "topic_id": 2,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 2",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 2,
      "id": 3,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-3",
      "html_url": "https://goskive.com/course/fu-course-3",
      "slug": "fu-course-3",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "discipline_id": 3,
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
      "updated_at": "2016-12-15T11:56:19.593Z",
      "shortname": "fu-course-3",
      "topic_id": 3,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 3",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 2,
      "id": 4,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-4",
      "html_url": "https://goskive.com/course/fu-course-4",
      "slug": "fu-course-4",
      "university_id": 1,
      "additional_university_ids": [

      ],
      "discipline_id": 4,
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
      "chapters_updated_at": "2016-12-15T11:56:18.154Z",
      "updated_at": "2016-12-15T11:56:20.008Z",
      "shortname": "fu-course-4",
      "topic_id": 4,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 4",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer d709879b5994ccec6053ae397e15c33c090c5cf1a3dfa9929cee32ed9374fb75"
```
## Get a list of university courses


### Request

#### Endpoint

```
GET /v2/universities/fu-berlin/courses
Content-Type: application/json
Authorization: Bearer 0dae712de63ea66a5e06e25149f99c6c96e64bab057a140f691d7197a3d6c6cb
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
      "creator_id": 7,
      "id": 5,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-5",
      "html_url": "https://goskive.com/course/fu-course-5",
      "slug": "fu-course-5",
      "university_id": 2,
      "additional_university_ids": [

      ],
      "discipline_id": 5,
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
      "updated_at": "2016-12-15T11:56:20.404Z",
      "shortname": "fu-course-5",
      "topic_id": 5,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 5",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 7,
      "id": 6,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-6",
      "html_url": "https://goskive.com/course/fu-course-6",
      "slug": "fu-course-6",
      "university_id": 2,
      "additional_university_ids": [

      ],
      "discipline_id": 6,
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
      "updated_at": "2016-12-15T11:56:20.438Z",
      "shortname": "fu-course-6",
      "topic_id": 6,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 6",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 8,
      "id": 7,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-7",
      "html_url": "https://goskive.com/course/fu-course-7",
      "slug": "fu-course-7",
      "university_id": 2,
      "additional_university_ids": [

      ],
      "discipline_id": 7,
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
      "updated_at": "2016-12-15T11:56:20.482Z",
      "shortname": "fu-course-7",
      "topic_id": 7,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 7",
      "organizational_identifier": null,
      "instructor_name": ""
    },
    {
      "creator_id": 8,
      "id": 8,
      "self_url": "http://api.goskive.test/api/v2/courses/fu-course-8",
      "html_url": "https://goskive.com/course/fu-course-8",
      "slug": "fu-course-8",
      "university_id": 2,
      "additional_university_ids": [

      ],
      "discipline_id": 8,
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
      "updated_at": "2016-12-15T11:56:20.517Z",
      "shortname": "fu-course-8",
      "topic_id": 8,
      "language_code": "de",
      "exam_months": [

      ],
      "title": "Course 8",
      "organizational_identifier": null,
      "instructor_name": ""
    }
  ]
}
```



```shell
curl "api.goskive.com/v2/universities/fu-berlin/courses" -X GET \
	-H "Content-Type: application/json" \
	-H "Authorization: Bearer 0dae712de63ea66a5e06e25149f99c6c96e64bab057a140f691d7197a3d6c6cb"
```
